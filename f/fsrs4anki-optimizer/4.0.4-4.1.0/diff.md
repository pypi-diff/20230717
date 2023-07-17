# Comparing `tmp/fsrs4anki_optimizer-4.0.4.tar.gz` & `tmp/fsrs4anki_optimizer-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.0.4.tar", last modified: Sun Jul 16 12:09:53 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.1.0.tar", last modified: Mon Jul 17 03:40:25 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.0.4.tar` & `fsrs4anki_optimizer-4.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50143 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50266 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/setup.py
```

### Comparing `fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,23 +471,28 @@
         w[11]: next_stability_stability_gain_after_failure
         w[12]: next_stability_retrievability_gain_after_failure
         For more details about the parameters, please see: 
         https://github.com/open-spaced-repetition/fsrs4anki/wiki/Free-Spaced-Repetition-Scheduler
         '''
 
     def pretrain(self, verbose=True):
+        self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
+        self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
+        if self.dataset.empty:
+            raise ValueError('Training data is inadequate.')
         rating_stability = {}
         rating_count = {}
+        average_recall = self.dataset['y'].mean()
 
         for first_rating in ("1", "2", "3", "4"):
             group = self.S0_dataset_group[self.S0_dataset_group['r_history'] == first_rating]
             if group.empty:
                 continue
             delta_t = group['delta_t']
-            recall = group['y']['mean']
+            recall = (group['y']['mean'] * group['y']['count'] + average_recall * 1) / (group['y']['count'] + 1)
             count = group['y']['count']
             total_count = sum(count)
             if total_count < 100:
                 tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got {total_count}.')
                 continue
             params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (60 if total_count < 1000 else 365)))
             stability = params[0]
@@ -560,18 +565,14 @@
         rating_stability = {k: round(v, 2) for k, v in sorted(rating_stability.items(), key=lambda item: item[0])}
         for rating, stability in rating_stability.items():
             self.init_w[rating-1] = stability
         tqdm.write(f"Pretrain finished!")
 
     def train(self, lr: float = 4e-2, n_epoch: int = 5, n_splits: int = 5, batch_size: int = 512, verbose: bool = True):
         """Step 4"""
-        self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
-        self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
-        if self.dataset.empty:
-            raise ValueError('Training data is inadequate.')
         self.dataset['tensor'] = self.dataset.progress_apply(lambda x: lineToTensor(list(zip([x['t_history']], [x['r_history']]))[0]), axis=1)
         self.dataset['group'] = self.dataset['r_history'] + self.dataset['t_history']
         tqdm.write("Tensorized!")
 
         w = []
         plots = []
         if n_splits > 1:
```

