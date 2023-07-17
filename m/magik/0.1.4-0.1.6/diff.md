# Comparing `tmp/magik-0.1.4.tar.gz` & `tmp/magik-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.1.4.tar", last modified: Sat Jul 15 20:25:13 2023, max compression
+gzip compressed data, was "magik-0.1.6.tar", last modified: Mon Jul 17 11:09:33 2023, max compression
```

## Comparing `magik-0.1.4.tar` & `magik-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.917164 magik-0.1.4/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-15 20:25:13.917049 magik-0.1.4/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3738 2023-07-14 14:03:48.000000 magik-0.1.4/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.915828 magik-0.1.4/magik/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.4/magik/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2374 2023-07-15 19:12:51.000000 magik-0.1.4/magik/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-14 12:27:41.000000 magik-0.1.4/magik/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-15 19:13:30.000000 magik-0.1.4/magik/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1365 2023-07-14 12:27:39.000000 magik-0.1.4/magik/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     8985 2023-07-15 20:19:53.000000 magik-0.1.4/magik/evaluators.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.916789 magik-0.1.4/magik/examples/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.1.4/magik/examples/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2020 2023-07-14 12:27:41.000000 magik-0.1.4/magik/examples/assertions.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1355 2023-07-14 13:02:24.000000 magik-0.1.4/magik/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2161 2023-07-14 13:22:02.000000 magik-0.1.4/magik/initialize.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.4/magik/internal_logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      608 2023-07-14 12:27:41.000000 magik-0.1.4/magik/logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.4/magik/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1043 2023-07-14 12:27:41.000000 magik-0.1.4/magik/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6146 2023-07-14 12:27:41.000000 magik-0.1.4/magik/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-14 12:27:41.000000 magik-0.1.4/magik/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      299 2023-07-06 16:24:21.000000 magik-0.1.4/magik/utils.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.916569 magik-0.1.4/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      518 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/top_level.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-15 20:25:13.917203 magik-0.1.4/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-15 20:25:05.000000 magik-0.1.4/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:09:33.632375 magik-0.1.6/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-17 11:09:33.632263 magik-0.1.6/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3738 2023-07-14 14:03:48.000000 magik-0.1.6/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:09:33.630903 magik-0.1.6/magik/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.6/magik/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2379 2023-07-15 21:10:11.000000 magik-0.1.6/magik/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-14 12:27:41.000000 magik-0.1.6/magik/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-17 11:02:45.000000 magik-0.1.6/magik/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1403 2023-07-17 11:06:20.000000 magik-0.1.6/magik/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)    11769 2023-07-17 09:10:35.000000 magik-0.1.6/magik/evaluators.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:09:33.631985 magik-0.1.6/magik/examples/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.1.6/magik/examples/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2020 2023-07-14 12:27:41.000000 magik-0.1.6/magik/examples/assertions.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1355 2023-07-14 13:02:24.000000 magik-0.1.6/magik/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2161 2023-07-14 13:22:02.000000 magik-0.1.6/magik/initialize.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.6/magik/internal_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      608 2023-07-14 12:27:41.000000 magik-0.1.6/magik/logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.6/magik/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1043 2023-07-14 12:27:41.000000 magik-0.1.6/magik/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     7808 2023-07-16 16:41:49.000000 magik-0.1.6/magik/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-14 12:27:41.000000 magik-0.1.6/magik/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      451 2023-07-16 17:12:15.000000 magik-0.1.6/magik/utils.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:09:33.631795 magik-0.1.6/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-17 11:09:33.000000 magik-0.1.6/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      518 2023-07-17 11:09:33.000000 magik-0.1.6/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-17 11:09:33.000000 magik-0.1.6/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-17 11:09:33.000000 magik-0.1.6/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-17 11:09:33.000000 magik-0.1.6/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-17 11:09:33.000000 magik-0.1.6/magik.egg-info/top_level.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-17 11:09:33.632416 magik-0.1.6/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-17 11:09:20.000000 magik-0.1.6/setup.py
```

### Comparing `magik-0.1.4/PKG-INFO` & `magik-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.4
+Version: 0.1.6
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `magik-0.1.4/README.md` & `magik-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/cli.py` & `magik-0.1.6/magik/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python3
 
 import argparse
 from magik.initialize import initialize
 from magik.generate import generate_test
-from magik.run import run_tests, run_tests_in_prod
 from magik.deploy import deploy_test
 from magik.internal_logger import logger
+from magik.run import Run
 
-commands = {
-    "init": initialize,
-    "generate": generate_test,
-    "run": run_tests,
-    "deploy": deploy_test,
-}
+commands = [
+    "init",
+    "generate",
+    "run",
+    "deploy",
+]
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Generate, run, and deploy unit tests for your AI app"
     )
     parser.add_argument("cmd", help="Command to execute")
@@ -55,24 +55,27 @@
         return
 
     if cmd == "generate":
         generate_test(test_name)
         return
 
     if cmd == "run" and not is_production:
-        run_tests(test_name)
+        test_runner = Run()
+        test_runner.run_tests(test_name)
         return
 
     if cmd == "run" and is_production:
         if not start_date or not end_date:
             logger.info(
                 f"Please provide a start_date and end_date argument as well.\n\nUsage: magik run <test_name> --prod --start_date <start_date> --end_date <end_date>"
             )
             return
-        run_tests_in_prod(
+
+        test_runner = Run()
+        test_runner.run_tests_in_prod(
             start_date=start_date,
             end_date=end_date,
             prompt_slug=prompt_slug,
         )
         return
 
     if cmd == "deploy":
```

### Comparing `magik-0.1.4/magik/constants.py` & `magik-0.1.6/magik/constants.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/deploy.py` & `magik-0.1.6/magik/deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         return
 
     # read file
     with open(file_path, "rb") as f:
         file_content = f.read()
 
     # prepare data for API request
-    data = {"apiKey": api_key, "testId": test_name}
-
+    headers = {"magik-api-key": api_key}
+    data = {"testId": test_name}
     files = {"file": ("assertions.py", file_content)}
 
     # make a POST request to the API
-    response = requests.post(DEPLOY_URL, files=files, data=data)
+    response = requests.post(DEPLOY_URL, files=files, data=data, headers=headers)
 
     # check the response
     if response.status_code == 200:
         logger.info(f"Successfully uploaded {file_path}")
     else:
         logger.info(
             f"Failed to upload {file_path}. Status code: {response.status_code}"
```

### Comparing `magik-0.1.4/magik/evaluators.py` & `magik-0.1.6/magik/evaluators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Contains functions to evaluate assertions.
 import requests
+import json
 import re
 import ast
 from magik.openai_helper import OpenAI
+from magik.utils import standardize_url
 from magik.constants import OPEN_AI_DEFAULT_MODEL
 
 
 def generate_grading_prompt(output_to_evaluate, grading_criteria):
     return (
         """
     You are grading a response string according to a grading criteria given to you.
@@ -197,31 +199,36 @@
     return regex(output_to_test, r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$")
 
 
 def is_phone_number(output_to_test):
     return regex(output_to_test, r"^\+?1?\d{9,15}$")
 
 
+# Generated by chatGPT (regex might need some work)
 def contains_email(output_to_test):
     return regex(output_to_test, r"[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+")
 
 
+# Generated by chatGPT (regex might need some work)
 def contains_phone_number(output_to_test):
-    return regex(output_to_test, r"\+?1?\d{9,15}|\(\d{3}\)\s*\d{3}[-\s]?\d{4}")
+    pattern = r"\+?\d{1,3}[-\s]?\(?\d{3}\)?[-\s]?\d{3}[-\s]?\d{2,4}|\(\d{3}\)\s?\d{3}[-\s]?\d{4}"
+    return regex(output_to_test, pattern)
 
 
+# Placeholder function to be replaced by an actual sentiment score function
 def is_positive_sentiment(output_to_test):
     sentiment_grading_prompt = """
         If the string has a positive sentiment, then the test_result is True. Otherwise, it is false.
     """
     return grade_using_llm(
         output_to_test=output_to_test, eval_rubric=sentiment_grading_prompt
     )
 
 
+# Placeholder function to be replaced by an actual sentiment score function
 def is_negative_sentiment(output_to_test):
     sentiment_grading_prompt = """
         If the string has a negative sentiment, then the test passed. Otherwise, the test failed.
     """
     return grade_using_llm(
         output_to_test=output_to_test, eval_rubric=sentiment_grading_prompt
     )
@@ -242,27 +249,105 @@
     """
     return grade_using_llm(
         output_to_test=output_to_test, eval_rubric=sentiment_grading_prompt
     )
 
 
 def contains_link(output_to_test):
-    return regex(output_to_test=output_to_test, pattern=r"https?://\S+")
+    pattern = r"(?!.*@)(?:https?://)?(?:www\.)?\S+\.\S+"
+    result = bool(re.search(pattern, output_to_test))
+    if result:
+        return {"result": True, "reason": "Link found in output"}
+    else:
+        return {"result": False, "reason": "No link found in output"}
 
 
 def contains_valid_link(output_to_test):
-    link_match = re.search(pattern=r"https?://\S+", string=output_to_test)
+    pattern = r"(?!.*@)(?:https?://)?(?:www\.)?\S+\.\S+"
+    link_match = re.search(pattern=pattern, string=output_to_test)
     if link_match:
-        matched_url = link_match.group()[0]
-        response = requests.get(matched_url)
-        if response.status_code == 200:
-            return {
-                "result": True,
-                "reason": f"link {matched_url} found in output and is valid",
-            }
-        else:
-            return {
-                "result": False,
-                "reason": f"link {matched_url} found in output but is invalid",
-            }
+        matched_url = link_match.group()
+        if matched_url:
+            standardized_url = standardize_url(matched_url)
+            try:
+                response = requests.head(standardized_url)
+                if response.status_code == 200:
+                    return {
+                        "result": True,
+                        "reason": f"link {matched_url} found in output and is valid",
+                    }
+                else:
+                    return {
+                        "result": False,
+                        "reason": f"link {matched_url} found in output but is invalid",
+                    }
+            except:
+                return {
+                    "result": False,
+                    "reason": f"link {matched_url} found in output but is invalid",
+                }
+    return {"result": False, "reason": f"no link found in output"}
+
+
+def contains_credit_card_number(output_to_test):
+    pattern = r"\b(?:\d[ -]*?){13,16}\b"
+    result = bool(re.search(pattern, output_to_test))
+    if result:
+        return {"result": True, "reason": f"credit card number found in output"}
+    else:
+        return {"result": False, "reason": f"no credit card number found in output"}
+
+
+def length_less_than(output_to_test, max_length):
+    if len(output_to_test) < max_length:
+        return {
+            "result": True,
+            "reason": f"output length is less than {max_length} characters",
+        }
+    else:
+        return {
+            "result": False,
+            "reason": f"output length is greater than {max_length} characters",
+        }
+
+
+def length_greater_than(output_to_test, min_length):
+    if len(output_to_test) > min_length:
+        return {
+            "result": True,
+            "reason": f"output length is greater than {min_length} characters",
+        }
+    else:
+        return {
+            "result": False,
+            "reason": f"output length is less than {min_length} characters",
+        }
+
+
+def is_json(output_to_test):
+    try:
+        json.loads(output_to_test)
+        return {
+            "result": True,
+            "reason": f"output is valid json",
+        }
+    except ValueError:
+        return {
+            "result": False,
+            "reason": f"output is not valid json",
+        }
+
+
+def contains_json(output_to_test):
+    trimmed_output = output_to_test.strip()
+    pattern = r"^\{.*\}$|^\[.*\]$"
+    result = bool(re.search(pattern, trimmed_output, re.DOTALL))
+    if result:
+        return {
+            "result": True,
+            "reason": "Output contains JSON",
+        }
     else:
-        return {"result": False, "reason": f"no link found in output"}
+        return {
+            "result": False,
+            "reason": "Output does not contain JSON",
+        }
```

### Comparing `magik-0.1.4/magik/examples/assertions.py` & `magik-0.1.6/magik/examples/assertions.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/generate.py` & `magik-0.1.6/magik/generate.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/initialize.py` & `magik-0.1.6/magik/initialize.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/internal_logger.py` & `magik-0.1.6/magik/internal_logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/logger.py` & `magik-0.1.6/magik/logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/openai_helper.py` & `magik-0.1.6/magik/openai_helper.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik/run.py` & `magik-0.1.6/magik/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,176 +7,193 @@
 from magik.utils import substitute_vars
 from magik.openai_helper import OpenAI
 from magik.sys_exec import read_from_file, create_file
 from magik.config import get_open_ai_default_model, get_magik_api_key
 from magik.constants import TESTRUNS_DIR, TEST_DIR, RUN_URL
 
 
-def run_tests(test_name):
-    tests = _load_tests(test_name)
-    raw_prompt = _load_prompt(test_name)
-    log_file_path = _log_file_path(test_name)
-    _run_tests_for_prompt(test_name, tests, raw_prompt, log_file_path=log_file_path)
-
-
-def run_tests_in_prod(start_date, end_date, prompt_slug):
-    request_data = {
-        "source": "CLI",
-        "startDate": start_date,
-        "endDate": end_date,
-        "promptSlug": prompt_slug,
-    }
-    print(f"Sending request to {RUN_URL} with data: {request_data}")
-    requests.post(
-        RUN_URL,
-        json=request_data,
-        headers={
-            "magik-api-key": get_magik_api_key(),
-        },
-    )
-
-
-def _run_tests_for_prompt(test_name, tests, raw_prompt, log_file_path):
-    _log_to_file_and_console("---------------")
-    _log_to_file_and_console("TEST RESULTS")
-    _log_to_file_and_console("---------------")
-    _log_to_file_and_console("\n")
-
-    num_tests_passed = 0
-    for test in tests:
-        test_result = _run_individual_test_for_prompt(
-            test_name, test, raw_prompt, log_file_path
-        )
-        if test_result:
-            num_tests_passed += 1
-
-    num_tests_failed = len(tests) - num_tests_passed
-
-    logger.info("\n------------")
-    if num_tests_passed == len(tests):
-        logger.info("✅ All tests passed")
-        logger.info("\n\n")
-    else:
-        logger.info(
-            f"""
-✅ {num_tests_passed}/{len(tests)} tests passed
-❌ {num_tests_failed}/{len(tests)} tests failed
-        """
-        )
-
-
-def _run_individual_test_for_prompt(test_name, test, raw_prompt, log_file_path):
-    openai = OpenAI()
-    prompt = substitute_vars(raw_prompt, test["prompt_vars"])
-    model = get_open_ai_default_model()
-    prompt_response = openai.openai_chat_completion_message(model=model, prompt=prompt)
-    return _run_individual_test_for_prompt_response(
-        test_name, test, prompt, prompt_response, log_file_path=log_file_path
-    )
-
-
-def _run_individual_test_for_prompt_response(
-    test_name, test, prompt, prompt_response, log_file_path
-):
-    test_function_result_obj = test["eval_function"](
-        prompt_response, *test["eval_function_args"]
-    )
-    result_obj = _generate_result_object(
-        test=test,
-        test_result=test_function_result_obj,
-        prompt=prompt,
-        prompt_response=prompt_response,
-    )
-
-    _log_results(
-        result_obj,
-        log_file_path=log_file_path,
-    )
-
-    return result_obj["test_result"]["result"]
-
-
-def _load_prompt(test_name):
-    test_file_path = f"{TEST_DIR}/{test_name}/prompt.txt"
-    absolute_path = os.path.abspath(test_file_path)
-    return read_from_file(absolute_path)
-
-
-def _load_tests(test_name):
-    test_file_path = f"{TEST_DIR}/{test_name}/assertions.py"
-    # Get the absolute path by resolving against the current working directory
-    absolute_path = os.path.abspath(test_file_path)
-
-    # Get the directory path and module name from the absolute path
-    directory, module_name = os.path.split(absolute_path)
-    module_name = os.path.splitext(module_name)[0]
-
-    # Load the module dynamically
-    spec = importlib.util.spec_from_file_location(module_name, absolute_path)
-    module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
-
-    # Access the `tests` array from the module
-    return getattr(module, "tests", [])
-
-
-def _generate_result_object(test, test_result, prompt, prompt_response):
-    did_test_pass = test_result["result"]
-    failure_labels = test["failure_labels"] if not did_test_pass else []
-    test_function_name = test["eval_function"].__name__
-    return {
-        "test": {
-            **test,
-            "eval_function": test_function_name,
-        },
-        "test_result": test_result,
-        "prompt": prompt,
-        "prompt_response": prompt_response,
-        "failure_labels": failure_labels,
-    }
-
-
-def _log_results(result_obj, log_file_path=None):
-    sys.stdout.flush()  # Flush the stdout buffer to ensure immediate printing to the console
-    if log_file_path is not None:
-        create_file(log_file_path)
-        with open(log_file_path, "a") as log_file:
-            _log_prompt_results(result_obj, log_file)
-            _log_test_results(result_obj, log_file)
-    else:
-        _log_prompt_results(result_obj)
-        _log_test_results(result_obj)
-
-
-def _log_to_file_and_console(output, log_file=None):
-    if log_file is not None:
-        log_file.write(output + "\n")
-        log_file.flush()  # Ensure immediate writing to the file
-    logger.info(output)
-
-
-def _log_prompt_results(result_obj, log_file=None):
-    prompt = result_obj["prompt"]
-    prompt_response = result_obj["prompt_response"]
-    _log_to_file_and_console(f"Prompt: {prompt}", log_file)
-    _log_to_file_and_console(f"Prompt Response: {prompt_response}", log_file)
-
-
-def _log_test_results(result_obj, log_file=None):
-    test_description = result_obj["test"]["description"]
-    test_function_result_bool = result_obj["test_result"]["result"]
-    test_result_str = "✅ Passed" if test_function_result_bool else "❌ Failed"
-    test_result_reason = result_obj["test_result"]["reason"]
-    failure_labels = result_obj["failure_labels"]
-
-    _log_to_file_and_console(f"Test: {test_description}", log_file)
-    _log_to_file_and_console(f"Test Result: {test_result_str}", log_file)
-    _log_to_file_and_console(f"Reason: {test_result_reason}", log_file)
-    _log_to_file_and_console(f"Failure Labels: {failure_labels}", log_file)
-    _log_to_file_and_console("\n", log_file)
-
-
-def _log_file_path(test_name):
-    current_timestamp = datetime.now()
-    formatted_timestamp = current_timestamp.strftime("%Y-%m-%d_%H-%M-%S")
-    log_file_path = f"{TESTRUNS_DIR}/{test_name}/{formatted_timestamp}.txt"
-    return log_file_path
+class Run:
+    def __init__(self):
+        self.saved_prompt_response = ""
+
+    def run_tests(self, test_name):
+        tests = self._load_tests(test_name)
+        raw_prompt = self._load_prompt(test_name)
+        log_file_path = self._log_file_path(test_name)
+        self._run_tests_for_prompt(
+            test_name, tests, raw_prompt, log_file_path=log_file_path
+        )
+
+    def run_tests_in_prod(self, start_date, end_date, prompt_slug):
+        request_data = {
+            "source": "CLI",
+            "startDate": start_date,
+            "endDate": end_date,
+            "promptSlug": prompt_slug,
+        }
+        logger.info(f"Sending request to {RUN_URL} with data: {request_data}\n")
+        requests.post(
+            RUN_URL,
+            json=request_data,
+            headers={
+                "magik-api-key": get_magik_api_key(),
+            },
+        )
+
+    def _run_tests_for_prompt(self, test_name, tests, raw_prompt, log_file_path):
+        self._log_to_file_and_console("---------------")
+        self._log_to_file_and_console("TEST RESULTS")
+        self._log_to_file_and_console("---------------")
+        self._log_to_file_and_console("\n")
+
+        num_tests_passed = 0
+        for test in tests:
+            test_result = self._run_individual_test_for_prompt(
+                test_name, test, raw_prompt, log_file_path
+            )
+            if test_result:
+                num_tests_passed += 1
+
+        num_tests_failed = len(tests) - num_tests_passed
+
+        logger.info("\n------------")
+        if num_tests_passed == len(tests):
+            logger.info("✅ All tests passed")
+            logger.info("\n\n")
+        else:
+            logger.info(
+                f"""
+    ✅ {num_tests_passed}/{len(tests)} tests passed
+    ❌ {num_tests_failed}/{len(tests)} tests failed
+            """
+            )
+
+    def _run_individual_test_for_prompt(
+        self, test_name, test, raw_prompt, log_file_path
+    ):
+        openai = OpenAI()
+        prompt_vars = test["prompt_vars"]
+        model = get_open_ai_default_model()
+        if len(prompt_vars) == 0:
+            prompt = raw_prompt
+            if len(self.saved_prompt_response) == 0:
+                self.saved_prompt_response = openai.openai_chat_completion_message(
+                    model=model, prompt=prompt
+                )
+            prompt_response = self.saved_prompt_response
+        else:
+            prompt = substitute_vars(raw_prompt, prompt_vars)
+            prompt_response = openai.openai_chat_completion_message(
+                model=model, prompt=prompt
+            )
+
+        return self._run_individual_test_for_prompt_response(
+            test_name, test, prompt, prompt_response, log_file_path=log_file_path
+        )
+
+    def _run_individual_test_for_prompt_response(
+        self, test_name, test, prompt, prompt_response, log_file_path
+    ):
+        test_function_result_obj = test["eval_function"](
+            prompt_response, *test["eval_function_args"]
+        )
+        result_obj = self._generate_result_object(
+            test=test,
+            test_result=test_function_result_obj,
+            prompt=prompt,
+            prompt_response=prompt_response,
+        )
+
+        self._log_results(
+            result_obj,
+            log_file_path=log_file_path,
+        )
+
+        return result_obj["test_result"]["result"]
+
+    def _load_prompt(self, test_name):
+        test_file_path = f"{TEST_DIR}/{test_name}/prompt.txt"
+        absolute_path = os.path.abspath(test_file_path)
+        return read_from_file(absolute_path)
+
+    def _load_tests(self, test_name):
+        test_file_path = f"{TEST_DIR}/{test_name}/assertions.py"
+        # Get the absolute path by resolving against the current working directory
+        absolute_path = os.path.abspath(test_file_path)
+
+        # Get the directory path and module name from the absolute path
+        directory, module_name = os.path.split(absolute_path)
+        module_name = os.path.splitext(module_name)[0]
+
+        # Load the module dynamically
+        spec = importlib.util.spec_from_file_location(module_name, absolute_path)
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+
+        # Access the `tests` array from the module
+        return getattr(module, "tests", [])
+
+    def _generate_result_object(self, test, test_result, prompt, prompt_response):
+        did_test_pass = test_result["result"]
+        failure_labels = test["failure_labels"] if not did_test_pass else []
+        test_function_name = test["eval_function"].__name__
+        return {
+            "test": {
+                **test,
+                "eval_function": test_function_name,
+            },
+            "test_result": test_result,
+            "prompt": prompt,
+            "prompt_response": prompt_response,
+            "failure_labels": failure_labels,
+        }
+
+    def _log_results(self, result_obj, log_file_path=None):
+        sys.stdout.flush()  # Flush the stdout buffer to ensure immediate printing to the console
+        test_description = result_obj["test"]["description"]
+        if log_file_path is not None:
+            create_file(log_file_path)
+            with open(log_file_path, "a") as log_file:
+                self._log_to_file_and_console(
+                    f"Test: {test_description}", log_file, color="cyan"
+                )
+                self._log_to_file_and_console(f"-----", log_file, color="cyan")
+                self._log_prompt_results(result_obj, log_file)
+                self._log_test_results(result_obj, log_file)
+        else:
+            self._log_to_file_and_console(f"Test: {test_description}", color="cyan")
+            self._log_to_file_and_console(f"-----", color="cyan")
+            self._log_prompt_results(result_obj)
+            self._log_test_results(result_obj)
+
+    def _log_to_file_and_console(self, output, log_file=None, color=None):
+        if log_file is not None:
+            log_file.write(output + "\n")
+            log_file.flush()  # Ensure immediate writing to the file
+
+        if color is not None:
+            logger.log_with_color(output, color)
+        else:
+            logger.info(output)
+
+    def _log_prompt_results(self, result_obj, log_file=None):
+        prompt = result_obj["prompt"]
+        prompt_response = result_obj["prompt_response"]
+        self._log_to_file_and_console(f"Prompt: {prompt}\n", log_file)
+        self._log_to_file_and_console(f"Prompt Response: {prompt_response}\n", log_file)
+
+    def _log_test_results(self, result_obj, log_file=None):
+        test_function_result_bool = result_obj["test_result"]["result"]
+        test_result_str = "✅ Passed" if test_function_result_bool else "❌ Failed"
+        test_result_reason = result_obj["test_result"]["reason"]
+        failure_labels = result_obj["failure_labels"]
+
+        self._log_to_file_and_console(f"Test Result: {test_result_str}", log_file)
+        self._log_to_file_and_console(f"Reason: {test_result_reason}", log_file)
+        self._log_to_file_and_console(f"Failure Labels: {failure_labels}", log_file)
+        self._log_to_file_and_console("\n", log_file)
+
+    def _log_file_path(self, test_name):
+        current_timestamp = datetime.now()
+        formatted_timestamp = current_timestamp.strftime("%Y-%m-%d_%H-%M-%S")
+        log_file_path = f"{TESTRUNS_DIR}/{test_name}/{formatted_timestamp}.txt"
+        return log_file_path
```

### Comparing `magik-0.1.4/magik/sys_exec.py` & `magik-0.1.6/magik/sys_exec.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/magik.egg-info/PKG-INFO` & `magik-0.1.6/magik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.4
+Version: 0.1.6
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `magik-0.1.4/magik.egg-info/SOURCES.txt` & `magik-0.1.6/magik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magik-0.1.4/setup.py` & `magik-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.1.4",
+    version="0.1.6",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

