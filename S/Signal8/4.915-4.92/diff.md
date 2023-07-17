# Comparing `tmp/Signal8-4.915.tar.gz` & `tmp/Signal8-4.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.915.tar", last modified: Fri Jul 14 01:02:02 2023, max compression
+gzip compressed data, was "Signal8-4.92.tar", last modified: Mon Jul 17 21:39:54 2023, max compression
```

## Comparing `Signal8-4.915.tar` & `Signal8-4.92.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.845108 Signal8-4.915/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.915/LICENSE
--rw-rw-rw-   0        0        0     4770 2023-07-14 01:02:02.841109 Signal8-4.915/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.915/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.749107 Signal8-4.915/Signal8/
--rw-rw-rw-   0        0        0    11550 2023-07-14 01:00:30.000000 Signal8-4.915/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.915/Signal8/__init__.py
--rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.915/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.832108 Signal8-4.915/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.915/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5285 2023-07-14 01:01:24.000000 Signal8-4.915/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.915/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.915/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.915/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.915/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.795107 Signal8-4.915/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4770 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 01:02:02.846107 Signal8-4.915/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-07-14 01:01:03.000000 Signal8-4.915/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:39:54.362936 Signal8-4.92/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.92/LICENSE
+-rw-rw-rw-   0        0        0     4769 2023-07-17 21:39:54.361936 Signal8-4.92/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.92/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 21:39:54.300939 Signal8-4.92/Signal8/
+-rw-rw-rw-   0        0        0    11427 2023-07-17 21:38:40.000000 Signal8-4.92/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.92/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      240 2023-07-17 21:38:01.000000 Signal8-4.92/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:39:54.356937 Signal8-4.92/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.92/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5285 2023-07-14 01:01:24.000000 Signal8-4.92/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2374 2023-07-14 18:02:49.000000 Signal8-4.92/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.92/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.92/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.92/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:39:54.336936 Signal8-4.92/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4769 2023-07-17 21:39:53.000000 Signal8-4.92/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-17 21:39:54.000000 Signal8-4.92/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 21:39:53.000000 Signal8-4.92/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-17 21:39:53.000000 Signal8-4.92/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 21:39:54.363936 Signal8-4.92/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-07-17 21:38:49.000000 Signal8-4.92/setup.py
```

### Comparing `Signal8-4.915/LICENSE` & `Signal8-4.92/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.915/PKG-INFO` & `Signal8-4.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.915
+Version: 4.92
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.915/README.md` & `Signal8-4.92/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-4.915/Signal8/Signal8.py` & `Signal8-4.92/Signal8/Signal8.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         max_cycles=500,
         ):
         
         if num_agents > 1:
             raise ValueError("Signal8 currently can only support up to 1 agent.")
         
         if num_large_obstacles > 16:
-            raise ValueError("Signal8 has a maximum of 10 large obstacles.")
+            raise ValueError("Signal8 has a maximum of 16 large obstacles.")
         
         scenario = Scenario()
         world = scenario.make_world(num_agents, num_large_obstacles, num_small_obstacles)
         
         super().__init__(
             scenario=scenario, 
             world=world, 
@@ -232,33 +232,31 @@
     # Ground agents can only observe the positions of other agents, goals, and small obstacles
     def observation(self, agent, world):
         agent_pos = agent.state.p_pos
         
         num_agents = len(world.agents)
         num_small_obstacles = len(world.small_obstacles)
         
-        observed_agents = [np.zeros_like(agent_pos) for _ in range(num_agents - 1)]
-        observed_obstacles = [np.zeros_like(agent_pos) for _ in range(num_small_obstacles)]
+        other_agents = [np.zeros_like(agent_pos) for _ in range(num_agents - 1)]
+        obstacles = [np.zeros_like(agent_pos) for _ in range(num_small_obstacles)]
         
         idx = 0
         for other_agent in world.agents:
             if agent.name == other_agent.name:
                 continue
             else:
                 other_agent_pos = other_agent.state.p_pos
                 relative_pos = other_agent_pos - agent_pos
-                observed_agents[idx] = relative_pos
+                other_agents[idx] = relative_pos
                 idx += 1
         
         for i, small_obstacle in enumerate(world.small_obstacles):
             obs_pos = small_obstacle.state.p_pos
-            relative_pos = obs_pos - agent_pos
-            observed_obstacles[i] = relative_pos
+            obstacles[i] = obs_pos
                 
         goal_pos = agent.goal.state.p_pos
-        observed_goal = goal_pos - agent_pos
         
-        return np.concatenate((agent_pos, observed_goal, np.concatenate(observed_obstacles, axis=0)))
+        return np.concatenate((agent_pos, goal_pos, other_agents, np.concatenate(obstacles, axis=0)))
         
     # Reward given by agents to agents for reaching their respective goals
     def reward(self, agent, world):
         return 0
```

### Comparing `Signal8-4.915/Signal8/utils/core.py` & `Signal8-4.92/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.915/Signal8/utils/problems.py` & `Signal8-4.92/Signal8/utils/problems.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         ((0.5, 0.5), (0.45)),
         ((-0.15, -0.675), (0.225)),
         ((-0.625, 0.175), (0.175)),
         ((-0.0375, 0), (0.1125)),
         ((-0.125, 0.475), (0.075)),
         ],
     'right_arrows': [
-        ((0.4, 0.2), (0.4, -0.2), (0.7, 0)),
-        ((0.3, 0.9), (0.3, 0.5), (0.6, 0.7)),
-        ((-0.75, 0.5), (-0.75, 0.1), (-0.45, 0.3)),
-        ((-0.3, -0.45), (-0.3, -0.85), (0, -0.65)),
+        ((0.4, 0.2), (0.4, -0.2), (0.7, 0)), # middle right
+        ((0.3, 0.9), (0.3, 0.5), (0.6, 0.7)), # top right
+        ((-0.75, 0.5), (-0.75, 0.1), (-0.45, 0.3)), # top left
+        ((-0.3, -0.45), (-0.3, -0.85), (0, -0.65)), # bottom left
         ]
     }
 
 def get_problem_list():
     return list(problems.keys())
 
 def get_problem_instance(instance_name):
```

### Comparing `Signal8-4.915/Signal8/utils/simple_env.py` & `Signal8-4.92/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.915/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.92/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.915/Signal8.egg-info/PKG-INFO` & `Signal8-4.92/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.915
+Version: 4.92
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.915/setup.py` & `Signal8-4.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.915",
+    version="4.92",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

