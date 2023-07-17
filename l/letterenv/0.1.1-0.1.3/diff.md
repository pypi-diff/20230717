# Comparing `tmp/letterenv-0.1.1.tar.gz` & `tmp/letterenv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterenv-0.1.1.tar", max compression
+gzip compressed data, was "letterenv-0.1.3.tar", max compression
```

## Comparing `letterenv-0.1.1.tar` & `letterenv-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       13 2023-07-09 12:47:56.938597 letterenv-0.1.1/README.md
--rw-r--r--   0        0        0       42 2023-07-09 13:43:03.544543 letterenv-0.1.1/letterenv/__init__.py
--rw-r--r--   0        0        0     5796 2023-07-17 10:48:09.177432 letterenv-0.1.1/letterenv/letterenv.py
--rw-r--r--   0        0        0      506 2023-07-17 10:48:29.480788 letterenv-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 letterenv-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-07-17 12:55:47.855819 letterenv-0.1.3/README.md
+-rw-r--r--   0        0        0       42 2023-07-09 13:43:03.544543 letterenv-0.1.3/letterenv/__init__.py
+-rw-r--r--   0        0        0     5899 2023-07-17 13:07:17.581799 letterenv-0.1.3/letterenv/letterenv.py
+-rw-r--r--   0        0        0      506 2023-07-17 13:08:45.237161 letterenv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 letterenv-0.1.3/PKG-INFO
```

### Comparing `letterenv-0.1.1/letterenv/letterenv.py` & `letterenv-0.1.3/letterenv/letterenv.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,31 +16,33 @@
         self,
         n_rows: int = 5,
         n_cols: int = 5,
         propositions: list[str] = ["A", "B", "C", "E"],
         locations: dict[str, tuple[int, int]] = {"A": (1, 1), "B": (0, 4), "C": (4, 0)},
         agent_start_location: tuple[int, int] = (4, 4),
         max_observation_counts: dict[str, int | None] = {
-            "A": 1,
+            "A": 3,
             "B": None,
             "C": None,
             "E": None,
         },
         replacement_mapping: dict[str, str] = {"A": "E"},
+        task_string: str = "AAAEBC",
     ) -> None:
         super().__init__()
 
         # Setup environment configuation
         self.n_rows = n_rows
         self.n_cols = n_cols
         self.propositions = propositions
         self.locations = locations
         self.agent_start_location = agent_start_location
         self.max_observation_counts = max_observation_counts
         self.replacement_mapping = replacement_mapping
+        self.task_string = task_string
         self.prop_idx = {p: i for i, p in enumerate(self.propositions)}
 
         # Define environment spaces
         self.action_space = spaces.Discrete(4)
         self.observation_space = spaces.Tuple(
             spaces=(
                 spaces.Discrete(self.n_rows),
@@ -59,14 +61,17 @@
         seed: int | None = None,
         options: dict | None = None,
     ):
         super().reset(seed=seed)
         # Reset number of steps taken in environment
         self.n_steps = 0
 
+        self.task_string_idx = 0
+        self.task_failed = False
+
         # Set number of times each proposition has been observed to 0
         self.prop_obs_counts = np.zeros((len(self.propositions),))
 
         # Define active propositions for each environment location
         self.active_propositions = {pos: p for p, pos in self.locations.items()}
 
         # Set agent initial position
@@ -87,41 +92,36 @@
 
             if self.prop_obs_counts[prop_idx] == self.max_observation_counts[obs_prop]:
                 # Replace proposition with next proposition in replacement mapping
                 self.active_propositions[
                     self.agent_position
                 ] = self.replacement_mapping[obs_prop]
 
+            if obs_prop == self.task_string[self.task_string_idx]:
+                if self.task_string_idx < len(self.task_string):
+                    self.task_string_idx += 1
+            else:
+                self.task_failed = True
+                print("Failed task")
+
         else:
             obs_prop = "_"
 
-        # Determine all propositions have been observed the maximum number of times
-        all_props_observed_max = True
-
-        for oc, mc in zip(
-            self.prop_obs_counts,
-            self.max_observation_counts.values(),
-        ):
-            if mc is None:
-                continue
-
-            if oc < mc:
-                all_props_observed_max = False
-                break
-
         obs = self._construct_observation()
 
         # Determine if episode is terminated due to max number of steps
         if self.spec is not None and self.spec.max_episode_steps == self.n_steps:
             terminated = True
             # Episode ended based on condition outside MDP (interface for more details)
             truncated = True
             reward = 0
         else:
-            terminated = all_props_observed_max
+            terminated = not self.task_failed and self.task_string_idx == len(
+                self.task_string
+            )
             truncated = False
             reward = 1 if terminated else 0
 
         return (
             obs,
             reward,
             terminated,
```

