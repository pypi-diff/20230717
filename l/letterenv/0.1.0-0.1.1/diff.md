# Comparing `tmp/letterenv-0.1.0.tar.gz` & `tmp/letterenv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterenv-0.1.0.tar", max compression
+gzip compressed data, was "letterenv-0.1.1.tar", max compression
```

## Comparing `letterenv-0.1.0.tar` & `letterenv-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       13 2023-07-09 12:47:56.938597 letterenv-0.1.0/README.md
--rw-r--r--   0        0        0       42 2023-07-09 13:43:03.544543 letterenv-0.1.0/letterenv/__init__.py
--rw-r--r--   0        0        0     4698 2023-07-09 15:53:08.564143 letterenv-0.1.0/letterenv/config.py
--rw-r--r--   0        0        0     5321 2023-07-09 16:04:01.406265 letterenv-0.1.0/letterenv/letterenv.py
--rw-r--r--   0        0        0      541 2023-07-09 16:09:31.278261 letterenv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 letterenv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-07-09 12:47:56.938597 letterenv-0.1.1/README.md
+-rw-r--r--   0        0        0       42 2023-07-09 13:43:03.544543 letterenv-0.1.1/letterenv/__init__.py
+-rw-r--r--   0        0        0     5796 2023-07-17 10:48:09.177432 letterenv-0.1.1/letterenv/letterenv.py
+-rw-r--r--   0        0        0      506 2023-07-17 10:48:29.480788 letterenv-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 letterenv-0.1.1/PKG-INFO
```

### Comparing `letterenv-0.1.0/letterenv/letterenv.py` & `letterenv-0.1.1/letterenv/letterenv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,58 @@
-from itertools import product
-
 import numpy as np
 from gymnasium import Env, spaces
 
-from letterenv.config import DefaultConfig, EnvironmentConfig
-
 
 class LetterEnv(Env):
     """Letter environment."""
 
     RIGHT = 0
     LEFT = 1
     UP = 2
     DOWN = 3
 
     metadata = {"render_modes": ["ansi"], "render_fps": 1}
 
-    def __init__(self, config: EnvironmentConfig = DefaultConfig()) -> None:
+    def __init__(
+        self,
+        n_rows: int = 5,
+        n_cols: int = 5,
+        propositions: list[str] = ["A", "B", "C", "E"],
+        locations: dict[str, tuple[int, int]] = {"A": (1, 1), "B": (0, 4), "C": (4, 0)},
+        agent_start_location: tuple[int, int] = (4, 4),
+        max_observation_counts: dict[str, int | None] = {
+            "A": 1,
+            "B": None,
+            "C": None,
+            "E": None,
+        },
+        replacement_mapping: dict[str, str] = {"A": "E"},
+    ) -> None:
         super().__init__()
 
         # Setup environment configuation
-        self.config = config
-        self.prop_idx = {p: i for i, p in enumerate(self.config.propositions)}
+        self.n_rows = n_rows
+        self.n_cols = n_cols
+        self.propositions = propositions
+        self.locations = locations
+        self.agent_start_location = agent_start_location
+        self.max_observation_counts = max_observation_counts
+        self.replacement_mapping = replacement_mapping
+        self.prop_idx = {p: i for i, p in enumerate(self.propositions)}
 
         # Define environment spaces
         self.action_space = spaces.Discrete(4)
         self.observation_space = spaces.Tuple(
             spaces=(
-                spaces.Discrete(self.config.n_rows),
-                spaces.Discrete(self.config.n_cols),
+                spaces.Discrete(self.n_rows),
+                spaces.Discrete(self.n_cols),
                 spaces.Text(
                     min_length=0,
                     max_length=1,
-                    charset="".join(self.config.propositions + ["_"]),
+                    charset="".join(self.propositions + ["_"]),
                 ),
             ),
         )
         self.reward_range = (0, 1)
 
     def reset(
         self,
@@ -44,53 +60,50 @@
         options: dict | None = None,
     ):
         super().reset(seed=seed)
         # Reset number of steps taken in environment
         self.n_steps = 0
 
         # Set number of times each proposition has been observed to 0
-        self.prop_obs_counts = np.zeros((len(self.config.propositions),))
+        self.prop_obs_counts = np.zeros((len(self.propositions),))
 
         # Define active propositions for each environment location
-        self.active_propositions = {pos: p for p, pos in self.config.locations.items()}
+        self.active_propositions = {pos: p for p, pos in self.locations.items()}
 
         # Set agent initial position
-        self.agent_position = self.config.agent_start_location
+        self.agent_position = self.agent_start_location
         return self._construct_observation(), {}
 
     def step(self, action: int):
         # Move agent in environment
         self._update_agent_position(action)
 
         # Calculate which propositions are true in the environment
         if self.agent_position in self.active_propositions:
             obs_prop = self.active_propositions[self.agent_position]
 
             # Update number of times proposition has been observed
             prop_idx = self.prop_idx[obs_prop]
             self.prop_obs_counts[prop_idx] += 1
 
-            if (
-                self.prop_obs_counts[prop_idx]
-                == self.config.max_observation_counts[obs_prop]
-            ):
+            if self.prop_obs_counts[prop_idx] == self.max_observation_counts[obs_prop]:
                 # Replace proposition with next proposition in replacement mapping
                 self.active_propositions[
                     self.agent_position
-                ] = self.config.replacement_mapping[obs_prop]
+                ] = self.replacement_mapping[obs_prop]
 
         else:
             obs_prop = "_"
 
         # Determine all propositions have been observed the maximum number of times
         all_props_observed_max = True
 
         for oc, mc in zip(
             self.prop_obs_counts,
-            self.config.max_observation_counts.values(),
+            self.max_observation_counts.values(),
         ):
             if mc is None:
                 continue
 
             if oc < mc:
                 all_props_observed_max = False
                 break
@@ -116,16 +129,16 @@
             {},
         )
 
     def render(self) -> str:
         """Render the environment as a string."""
         str_repr = ""
 
-        for r in range(self.config.n_rows):
-            for c in range(self.config.n_cols):
+        for r in range(self.n_rows):
+            for c in range(self.n_cols):
                 if (r, c) == self.agent_position:
                     str_repr += "\x1b[1;37;42m" + "x" + "\x1b[0m" + " "
                 elif (r, c) in self.active_propositions:
                     str_repr += self.active_propositions[(r, c)] + " "
                 else:
                     str_repr += "." + " "
             str_repr += "\n"
@@ -133,24 +146,24 @@
 
     def _update_agent_position(self, action: int) -> None:
         """Moves that take agent out of the grid leave it in the same position."""
         row, col = self.agent_position
 
         if action == self.RIGHT:
             n_row = row
-            n_col = col + 1 if col < self.config.n_cols - 1 else col
+            n_col = col + 1 if col < self.n_cols - 1 else col
         elif action == self.LEFT:
             n_row = row
             n_col = col - 1 if col > 0 else col
         elif action == self.UP:
             n_col = col
             n_row = row - 1 if row > 0 else row
         elif action == self.DOWN:
             n_col = col
-            n_row = row + 1 if row < self.config.n_rows - 1 else row
+            n_row = row + 1 if row < self.n_rows - 1 else row
         else:
             raise ValueError(f"Invalid action {action}.")
         self.agent_position = (n_row, n_col)
 
     def _construct_observation(self):
         if self.agent_position in self.active_propositions:
             obs_props = self.active_propositions[self.agent_position]
```

