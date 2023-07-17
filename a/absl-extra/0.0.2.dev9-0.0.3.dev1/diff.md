# Comparing `tmp/absl_extra-0.0.2.dev9.tar.gz` & `tmp/absl_extra-0.0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.2.dev9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.3.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.2.dev9.tar` & `absl_extra-0.0.3.dev1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1588 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/Readme.md
--rw-r--r--   0        0        0      713 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/__init__.py
--rw-r--r--   0        0        0       64 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/py.typed
--rw-r--r--   0        0        0        0 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/__init__.py
--rw-r--r--   0        0        0     1202 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/jax_utils.py
--rw-r--r--   0        0        0     2297 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/logging_utils.py
--rw-r--r--   0        0        0     3273 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/notifier.py
--rw-r--r--   0        0        0     4299 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/tasks.py
--rw-r--r--   0        0        0     4432 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/tf_utils.py
--rw-r--r--   0        0        0      914 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/pyproject.toml
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev9/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/Readme.md
+-rw-r--r--   0        0        0       74 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/__init__.py
+-rw-r--r--   0        0        0     1945 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/callbacks.py
+-rw-r--r--   0        0        0    16818 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/flax_utils.py
+-rw-r--r--   0        0        0     5411 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/jax_utils.py
+-rw-r--r--   0        0        0     1605 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/logging_utils.py
+-rw-r--r--   0        0        0     3238 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/notifier.py
+-rw-r--r--   0        0        0       64 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/py.typed
+-rw-r--r--   0        0        0     5702 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2301 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/testing/lifted_variants.py
+-rw-r--r--   0        0        0     4623 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/tf_utils.py
+-rw-r--r--   0        0        0     1071 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 absl_extra-0.0.3.dev1/PKG-INFO
```

### Comparing `absl_extra-0.0.2.dev9/Readme.md` & `absl_extra-0.0.3.dev1/Readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,45 +4,44 @@
 It will:
 - Notify on execution start, finish or failed.
   - By default, Notifier will just log those out to `stdout`.
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
 - Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
 - Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
+- Select registered task to run based on --task= CLI argument.
 
 Minimal example
 
 ```python
 import os
 from pymongo.collection import Collection
 from ml_collections import ConfigDict
 from absl import logging
 import tensorflow as tf
 
-from absl_extra import MongoConfig, register_task, run
-from absl_extra.notifier import SlackNotifier
-from absl_extra.tf_utils import requires_gpu, supports_mixed_precision, make_gpu_strategy
+from absl_extra import tf_utils, tasks, notifier
 
 
-@register_task
-@requires_gpu
-def main(cmd: str, config: ConfigDict, db: Collection) -> None:
-    if supports_mixed_precision():
+@tasks.register_task(
+    config_file="config.py",
+    mongo_config=dict(uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"),
+    notifier=notifier.SlackNotifier(slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"])
+)
+@tf_utils.requires_gpu
+def main(config: ConfigDict, db: Collection) -> None:
+    if tf_utils.supports_mixed_precision():
         tf.keras.mixed_precision.set_global_policy("mixed_float16")
     
-    with make_gpu_strategy().scope():
-        logging.info("Doing some heavy lifting...")    
+    with tf_utils.make_gpu_strategy().scope():
+        logging.info("Doing some heavy lifting...")
 
 
 if __name__ == "__main__":
-    run(
-        config_file="config.py",
-        mongo_config=MongoConfig(uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"),
-        notifier=SlackNotifier(slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]),
-    )
+    tasks.run()
 ```
 
 
 # Planned for:
 - global app state for different tasks
 - list of pre/post hooks 
 - keras callback with notifier
```

### Comparing `absl_extra-0.0.2.dev9/absl_extra/src/logging_utils.py` & `absl_extra-0.0.3.dev1/absl_extra/logging_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,50 @@
 from __future__ import annotations
 
 import functools
 import inspect
+import sys
 from importlib import util
 from typing import Callable, Literal, TypeVar
 
+import toolz
 from absl import logging
 
-C = TypeVar("C", bound=Callable)
+if sys.version_info >= (3, 10):
+    from typing import ParamSpec
+else:
+    from typing_extensions import ParamSpec
 
 
-def log_exception(func: C, logger: Callable[[str], None] = logging.error) -> C:
+T = TypeVar("T")
+P = ParamSpec("P")
+
+
+@toolz.curry
+def log_exception(
+    func: Callable[P, T], logger: Callable[[str], None] = logging.error
+) -> Callable[P, T]:
     """Log raised exception, and argument which caused it."""
 
     @functools.wraps(func)
-    def wrapper(*args, **kwargs):
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         func_args = inspect.signature(func).bind(*args, **kwargs).arguments
         func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
 
         try:
             return func(*args, **kwargs)
         except Exception as ex:
             logger(
                 f"{func.__module__}.{func.__qualname__} with args ( {func_args_str} ) raised {ex}"
             )
             raise ex
 
     return wrapper
 
 
-def log_before(func: C, logger: Callable[[str], None] = logging.debug) -> C:
-    """Log argument and function name."""
-
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        func_args = inspect.signature(func).bind(*args, **kwargs).arguments
-        func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
-        logger(
-            f"Entered {func.__module__}.{func.__qualname__} with args ( {func_args_str} )"
-        )
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-def log_after(func, logger: Callable[[str], None] = logging.debug):
-    """Log's function's return value."""
-
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        retval = func(*args, **kwargs)
-        logger(
-            f"Exited {func.__module__}.{func.__qualname__}(...) with value: "
-            + repr(retval)
-        )
-        return retval
-
-    return wrapper
-
-
 def setup_logging(
     *,
     log_format: str = "%(asctime)s:[%(filename)s:%(lineno)s->%(funcName)s()]:%(levelname)s: %(message)s",
     log_level: Literal["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"] = "DEBUG",
 ):
     import logging
```

### Comparing `absl_extra-0.0.2.dev9/absl_extra/src/notifier.py` & `absl_extra-0.0.3.dev1/absl_extra/notifier.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,105 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from importlib import util
-from typing import Callable
 
 from absl import logging
 
 
 class BaseNotifier(ABC):
     @abstractmethod
-    def notify_job_started(self, name: str):
+    def notify_task_started(self, name: str):
         raise NotImplementedError
 
     @abstractmethod
-    def notify_job_finished(self, name: str):
+    def notify_task_finished(self, name: str):
         raise NotImplementedError
 
     @abstractmethod
-    def notify_job_failed(self, name: str, exception: Exception):
+    def notify_task_failed(self, name: str, exception: Exception):
         raise NotImplementedError
 
 
 class NoOpNotifier(BaseNotifier):
-    def notify_job_started(self, name: str):
+    def notify_task_started(self, name: str):
         pass
 
-    def notify_job_finished(self, name: str):
+    def notify_task_finished(self, name: str):
         pass
 
-    def notify_job_failed(self, name: str, exception: Exception):
-        raise NotImplementedError
+    def notify_task_failed(self, name: str, exception: Exception):
+        pass
 
 
 class LoggingNotifier(BaseNotifier):
-    def __init__(self, logger: Callable[[str], None] = logging.info):
-        self.logger = logger
-
-    def notify_job_started(self, name: str):
-        logging.info(f"Job {name} started.")
-
-    def notify_job_finished(self, name: str):
-        logging.info(f"Job {name} finished.")
-
-    def notify_job_failed(self, name: str, exception: Exception):
-        logging.error(f"Job {name} failed with {exception}")
+    def notify_task_started(self, name: str):
+        logging.info("-" * 50)
+        logging.info(f"Task {name} started.")
+
+    def notify_task_finished(self, name: str):
+        logging.info("-" * 50)
+        logging.info(f"Task {name} finished.")
+
+    def notify_task_failed(self, name: str, exception: Exception):
+        logging.info("-" * 50)
+        logging.error(f"Task {name} failed with {exception}")
 
 
 if util.find_spec("slack_sdk"):
     import slack_sdk
 
     class SlackNotifier(BaseNotifier):
         def __init__(self, slack_token: str, channel_id: str):
             self.slack_token = slack_token
             self.channel_id = channel_id
 
-        def notify_job_started(self, name: str):
+        def notify_task_started(self, name: str):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
                 channel=self.channel_id,
                 blocks=[
                     {
                         "type": "section",
                         "text": {
                             "type": "mrkdwn",
-                            "text": f" :ballot_box_with_check: Job {name} started.",
+                            "text": f" :ballot_box_with_check: Task {name} started.",
                         },
                     }
                 ],
-                text="Job Started!",
+                text="Task Started!",
             )
 
-        def notify_job_finished(self, name: str):
+        def notify_task_finished(self, name: str):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
                 channel=self.channel_id,
                 blocks=[
                     {
                         "type": "section",
                         "text": {
                             "type": "mrkdwn",
-                            "text": f":white_check_mark: Job {name} finished execution.",
+                            "text": f":white_check_mark: Task {name} finished execution.",
                         },
                     }
                 ],
-                text="Job Finished!",
+                text="Task Finished!",
             )
 
-        def notify_job_failed(self, name: str, exception: Exception):
+        def notify_task_failed(self, name: str, exception: Exception):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
                 channel=self.channel_id,
                 blocks=[
                     {
                         "type": "section",
                         "text": {
                             "type": "mrkdwn",
-                            "text": f":x: Job {name} failed, reason:\n ```{exception}```",
+                            "text": f":x: Task {name} failed, reason:\n ```{exception}```",
                         },
                     }
                 ],
-                text="Job Failed!",
+                text="Task Failed!",
             )
 
 else:
     logging.warning("slack_sdk not installed.")
```

### Comparing `absl_extra-0.0.2.dev9/absl_extra/src/tf_utils.py` & `absl_extra-0.0.3.dev1/absl_extra/tf_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 from __future__ import annotations
 
 import functools
 import logging
 import platform
+import sys
 from contextlib import contextmanager
 from typing import Callable, ContextManager, Protocol, Type, TypeVar
 
+import toolz
+
+if sys.version_info >= (3, 10):
+    from typing import ParamSpec
+else:
+    from typing_extensions import ParamSpec
+
 import tensorflow as tf
 
-C = TypeVar("C", bound=Callable)
+T = TypeVar("T")
+P = ParamSpec("P")
 
 
-def requires_gpu(func: C, linux_only: bool = False) -> C:
+@toolz.curry
+def requires_gpu(func: Callable[P, T], linux_only: bool = False) -> Callable[P, T]:
     """
     Fail if function is executing on host without access to GPU(s).
     Useful for early detecting container runtime misconfigurations.
 
     Parameters
     ----------
     func:
@@ -29,16 +39,16 @@
 
     func:
         Function with the same signature as original one.
 
     """
 
     @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> R:
-        if linux_only and platform.system() != "linux":
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+        if linux_only and platform.system().lower() != "linux":
             logging.info(
                 "Not running on linux, and linux_only==True, ignoring GPU strategy check."
             )
             return func(*args, **kwargs)
 
         gpus = tf.config.list_physical_devices("GPU")
         logging.info(f"Available GPUs -> {gpus}")
@@ -55,15 +65,15 @@
 
 
 class NoOpStrategy:
     def __init__(self, **kwargs):
         pass
 
     @contextmanager
-    def scope(self) -> ContextManager:
+    def scope(self):
         yield
 
 
 def make_tpu_strategy() -> StrategyLike:
     """
     Used for testing locally scripts, which them must run on Colab TPUs. Allows to keep the same scripts,
     without changing strategy assignment.
```

### Comparing `absl_extra-0.0.2.dev9/pyproject.toml` & `absl_extra-0.0.3.dev1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 [project]
 name = "absl_extra"
-version = "0.0.2dev9"
+version = "0.0.3dev1"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
 ]
 dependencies = [
-    "absl_py"
+    "absl_py",
+    "toolz",
+    "typing_extensions; python_version < '3.10'"
 ]
 [project.optional-dependencies]
 dev = [
     "black",
     "pytest",
-    "absl_extra[mongo,ml_collections,slack,tensorflow]"
+    "chex",
+    "absl_extra[mongo,ml_collections,slack,tensorflow,jax,flax]"
 ]
 mongo = ["pymongo"]
 ml_collections = ["ml_collections"]
 slack = ["slack_sdk"]
 tensorflow = [
     "tensorflow; sys_platform == 'linux'",
     "tensorflow_macos; sys_platform == 'darwin'"
 ]
 jax = [
+    "jaxtyping",
     "jax",
     "jaxlib"
 ]
+flax = [
+    "absl_extra[jax]",
+    "flax",
+    "clu"
+]
 
 
 [project.urls]
 "Homepage" = "https://github.com/aaarrti/absl_extra"
 
 
 [build-system]
```

### Comparing `absl_extra-0.0.2.dev9/PKG-INFO` & `absl_extra-0.0.3.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.2.dev9
+Version: 0.0.3.dev1
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
+Requires-Dist: toolz
+Requires-Dist: typing_extensions; python_version < '3.10'
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: absl_extra[mongo,ml_collections,slack,tensorflow] ; extra == "dev"
+Requires-Dist: chex ; extra == "dev"
+Requires-Dist: absl_extra[mongo,ml_collections,slack,tensorflow,jax,flax] ; extra == "dev"
+Requires-Dist: absl_extra[jax] ; extra == "flax"
+Requires-Dist: flax ; extra == "flax"
+Requires-Dist: clu ; extra == "flax"
+Requires-Dist: jaxtyping ; extra == "jax"
 Requires-Dist: jax ; extra == "jax"
 Requires-Dist: jaxlib ; extra == "jax"
 Requires-Dist: ml_collections ; extra == "ml_collections"
 Requires-Dist: pymongo ; extra == "mongo"
 Requires-Dist: slack_sdk ; extra == "slack"
 Requires-Dist: tensorflow ; extra == "tensorflow" and ( sys_platform == 'linux')
 Requires-Dist: tensorflow_macos ; extra == "tensorflow" and ( sys_platform == 'darwin')
 Project-URL: Homepage, https://github.com/aaarrti/absl_extra
 Provides-Extra: dev
+Provides-Extra: flax
 Provides-Extra: jax
 Provides-Extra: ml_collections
 Provides-Extra: mongo
 Provides-Extra: slack
 Provides-Extra: tensorflow
 
 ### ABSL-Extra
@@ -32,45 +40,44 @@
 It will:
 - Notify on execution start, finish or failed.
   - By default, Notifier will just log those out to `stdout`.
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
 - Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
 - Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
+- Select registered task to run based on --task= CLI argument.
 
 Minimal example
 
 ```python
 import os
 from pymongo.collection import Collection
 from ml_collections import ConfigDict
 from absl import logging
 import tensorflow as tf
 
-from absl_extra import MongoConfig, register_task, run
-from absl_extra.notifier import SlackNotifier
-from absl_extra.tf_utils import requires_gpu, supports_mixed_precision, make_gpu_strategy
+from absl_extra import tf_utils, tasks, notifier
 
 
-@register_task
-@requires_gpu
-def main(cmd: str, config: ConfigDict, db: Collection) -> None:
-    if supports_mixed_precision():
+@tasks.register_task(
+    config_file="config.py",
+    mongo_config=dict(uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"),
+    notifier=notifier.SlackNotifier(slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"])
+)
+@tf_utils.requires_gpu
+def main(config: ConfigDict, db: Collection) -> None:
+    if tf_utils.supports_mixed_precision():
         tf.keras.mixed_precision.set_global_policy("mixed_float16")
     
-    with make_gpu_strategy().scope():
-        logging.info("Doing some heavy lifting...")    
+    with tf_utils.make_gpu_strategy().scope():
+        logging.info("Doing some heavy lifting...")
 
 
 if __name__ == "__main__":
-    run(
-        config_file="config.py",
-        mongo_config=MongoConfig(uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"),
-        notifier=SlackNotifier(slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]),
-    )
+    tasks.run()
 ```
 
 
 # Planned for:
 - global app state for different tasks
 - list of pre/post hooks 
 - keras callback with notifier
```

