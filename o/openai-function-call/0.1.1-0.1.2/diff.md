# Comparing `tmp/openai_function_call-0.1.1.tar.gz` & `tmp/openai_function_call-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_call-0.1.1.tar", max compression
+gzip compressed data, was "openai_function_call-0.1.2.tar", max compression
```

## Comparing `openai_function_call-0.1.1.tar` & `openai_function_call-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-07-08 18:19:43.018939 openai_function_call-0.1.1/LICENSE
--rw-r--r--   0        0        0     8289 2023-07-09 04:09:54.978582 openai_function_call-0.1.1/README.md
--rw-r--r--   0        0        0      187 2023-07-08 18:19:43.033586 openai_function_call-0.1.1/openai_function_call/__init__.py
--rw-r--r--   0        0        0      151 2023-07-08 18:19:43.034089 openai_function_call-0.1.1/openai_function_call/dsl/__init__.py
--rw-r--r--   0        0        0     5773 2023-07-08 18:19:43.034296 openai_function_call-0.1.1/openai_function_call/dsl/completion.py
--rw-r--r--   0        0        0      505 2023-07-08 18:19:43.034803 openai_function_call-0.1.1/openai_function_call/dsl/messages/__init__.py
--rw-r--r--   0        0        0     1669 2023-07-08 18:19:43.035000 openai_function_call-0.1.1/openai_function_call/dsl/messages/base.py
--rw-r--r--   0        0        0     3260 2023-07-08 18:19:43.035533 openai_function_call-0.1.1/openai_function_call/dsl/messages/messages.py
--rw-r--r--   0        0        0     1486 2023-07-08 18:19:43.035798 openai_function_call-0.1.1/openai_function_call/dsl/messages/user.py
--rw-r--r--   0        0        0     2202 2023-07-08 18:19:43.036083 openai_function_call-0.1.1/openai_function_call/dsl/multitask.py
--rw-r--r--   0        0        0     6151 2023-07-08 18:19:43.036753 openai_function_call-0.1.1/openai_function_call/function_calls.py
--rw-r--r--   0        0        0      663 2023-07-09 04:59:47.039821 openai_function_call-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9023 1970-01-01 00:00:00.000000 openai_function_call-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-17 09:19:43.513220 openai_function_call-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8394 2023-07-17 09:19:43.513220 openai_function_call-0.1.2/README.md
+-rw-r--r--   0        0        0      187 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/__init__.py
+-rw-r--r--   0        0        0     5799 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/completion.py
+-rw-r--r--   0        0        0      505 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/base.py
+-rw-r--r--   0        0        0     3260 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/messages.py
+-rw-r--r--   0        0        0     1486 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/user.py
+-rw-r--r--   0        0        0     2210 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/multitask.py
+-rw-r--r--   0        0        0     6351 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/function_calls.py
+-rw-r--r--   0        0        0      663 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9128 1970-01-01 00:00:00.000000 openai_function_call-0.1.2/PKG-INFO
```

### Comparing `openai_function_call-0.1.1/LICENSE` & `openai_function_call-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.1/README.md` & `openai_function_call-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -123,36 +123,38 @@
     name: str = Field(..., description="User's name")
     age: int = Field(..., description="User's age")
 ```
 
 ### Example 3: Using the DSL
 
 ```python
+from pprint import pprint
+
 from openai_function_call import OpenAISchema
 from openai_function_call.dsl import ChatCompletion, MultiTask, messages as m
-from openai_function_call.dsl.messages import system as s
+from openai_function_call.dsl.messages import SystemIdentity, SystemTask, SystemStyle, SystemGuidelines, SystemTips
 
 # Define a subtask you'd like to extract from then,
 # We'll use MultTask to easily map it to a List[Search]
 # so we can extract more than one
 class Search(OpenAISchema):
     id: int
     query: str
 
 tasks = (
     ChatCompletion(name="Acme Inc Email Segmentation", model="gpt-3.5-turbo-0613")
-    | s.Identity(identity="World class state of the art agent") # if no identity is provided, this is the default one
-    | s.Task(task="Segment emails into search queries")
-    | s.Style(style="Professional, clear and concise")
-    | s.Guidelines(guidelines=[
+    | SystemIdentity(identity="World class state of the art agent") # if no identity is provided, this is the default one
+    | SystemTask(task="Segment emails into search queries")
+    | SystemStyle(style="Professional, clear and concise")
+    | SystemGuidelines(guidelines=[
         'You never swear',
         'You are polite',
         'You say please and thank you often.'
     ])
-    | s.Tips(tips=[
+    | SystemTips(tips=[
         "When unsure about the correct segmentation, try to think about the task as a whole",
         "If acronyms are used expand them to their full form",
         "Use multiple phrases to describe the same thing"]
                   )
     | MultiTask(subtask_class=Search)
     | m.TaggedMessage(
         tag="email",
```

### Comparing `openai_function_call-0.1.1/openai_function_call/dsl/completion.py` & `openai_function_call-0.1.2/openai_function_call/dsl/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         Returns:
             response (OpenAISchema): The response from the OpenAI API
         """
         kwargs = self.kwargs
         completion = openai.ChatCompletion.create(**kwargs)
         if self.function:
             return self.function.from_response(completion)
+        return completion
 
     async def acreate(self):
         """
         Create a chat response from the OpenAI API asynchronously
 
         Returns:
             response (OpenAISchema): The response from the OpenAI API
```

### Comparing `openai_function_call-0.1.1/openai_function_call/dsl/messages/base.py` & `openai_function_call-0.1.2/openai_function_call/dsl/messages/base.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.1/openai_function_call/dsl/messages/messages.py` & `openai_function_call-0.1.2/openai_function_call/dsl/messages/messages.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.1/openai_function_call/dsl/messages/user.py` & `openai_function_call-0.1.2/openai_function_call/dsl/messages/user.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.1/openai_function_call/dsl/multitask.py` & `openai_function_call-0.1.2/openai_function_call/dsl/multitask.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         subtask_class (Type[OpenAISchema]): The base class to use for the MultiTask
         name (Optional[str]): The name of the MultiTask class, if None then the name
             of the subtask class is used as `Multi{subtask_class.__name__}`
         description (Optional[str]): The description of the MultiTask class, if None
             then the description is set to `Correct segmentation of `{subtask_class.__name__}` tasks`
 
     Returns:
-        OpenAISchema: A new class that can be used to segment multiple tasks
-
+        schema (OpenAISchema): A new class that can be used to segment multiple tasks
     """
     task_name = subtask_class.__name__ if name is None else name
 
     name = f"Multi{task_name}"
 
     list_tasks = (
         List[subtask_class],
```

### Comparing `openai_function_call-0.1.1/openai_function_call/function_calls.py` & `openai_function_call-0.1.2/openai_function_call/function_calls.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,14 +129,20 @@
         """
         schema = cls.schema()
         parameters = {
             k: v for k, v in schema.items() if k not in ("title", "description")
         }
         parameters["required"] = sorted(parameters["properties"])
         _remove_a_key(parameters, "title")
+
+        if "description" not in schema:
+            schema[
+                "description"
+            ] = f"Correctly extracted `{cls.__name__}` with all the required parameters with correct types"
+
         return {
             "name": schema["title"],
             "description": schema["description"],
             "parameters": parameters,
         }
 
     @classmethod
```

### Comparing `openai_function_call-0.1.1/pyproject.toml` & `openai_function_call-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-function-call"
-version = "0.1.1"
+version = "0.1.2"
 description = "Helper functions that allow us to improve openai's function_call ergonomics"
 authors = ["Jason <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "openai_function_call"}]
 repository = "https://github.com/jxnl/openai_function_call"
```

### Comparing `openai_function_call-0.1.1/PKG-INFO` & `openai_function_call-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-call
-Version: 0.1.1
+Version: 0.1.2
 Summary: Helper functions that allow us to improve openai's function_call ergonomics
 Home-page: https://github.com/jxnl/openai_function_call
 License: MIT
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -142,36 +142,38 @@
     name: str = Field(..., description="User's name")
     age: int = Field(..., description="User's age")
 ```
 
 ### Example 3: Using the DSL
 
 ```python
+from pprint import pprint
+
 from openai_function_call import OpenAISchema
 from openai_function_call.dsl import ChatCompletion, MultiTask, messages as m
-from openai_function_call.dsl.messages import system as s
+from openai_function_call.dsl.messages import SystemIdentity, SystemTask, SystemStyle, SystemGuidelines, SystemTips
 
 # Define a subtask you'd like to extract from then,
 # We'll use MultTask to easily map it to a List[Search]
 # so we can extract more than one
 class Search(OpenAISchema):
     id: int
     query: str
 
 tasks = (
     ChatCompletion(name="Acme Inc Email Segmentation", model="gpt-3.5-turbo-0613")
-    | s.Identity(identity="World class state of the art agent") # if no identity is provided, this is the default one
-    | s.Task(task="Segment emails into search queries")
-    | s.Style(style="Professional, clear and concise")
-    | s.Guidelines(guidelines=[
+    | SystemIdentity(identity="World class state of the art agent") # if no identity is provided, this is the default one
+    | SystemTask(task="Segment emails into search queries")
+    | SystemStyle(style="Professional, clear and concise")
+    | SystemGuidelines(guidelines=[
         'You never swear',
         'You are polite',
         'You say please and thank you often.'
     ])
-    | s.Tips(tips=[
+    | SystemTips(tips=[
         "When unsure about the correct segmentation, try to think about the task as a whole",
         "If acronyms are used expand them to their full form",
         "Use multiple phrases to describe the same thing"]
                   )
     | MultiTask(subtask_class=Search)
     | m.TaggedMessage(
         tag="email",
```

