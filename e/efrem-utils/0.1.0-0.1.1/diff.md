# Comparing `tmp/efrem_utils-0.1.0.tar.gz` & `tmp/efrem_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.1.0.tar", max compression
+gzip compressed data, was "efrem_utils-0.1.1.tar", max compression
```

## Comparing `efrem_utils-0.1.0.tar` & `efrem_utils-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2189 2023-07-14 09:31:24.930214 efrem_utils-0.1.0/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0      361 2023-07-15 19:42:35.485880 efrem_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2560 2023-07-15 19:46:30.761405 efrem_utils-0.1.0/README.md
--rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 efrem_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2676 2023-07-17 12:25:28.408764 efrem_utils-0.1.1/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.1/LICENSE
+-rw-r--r--   0        0        0      361 2023-07-17 12:23:38.859527 efrem_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3008 2023-07-17 12:30:21.529798 efrem_utils-0.1.1/README.md
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.1.1/PKG-INFO
```

### Comparing `efrem_utils-0.1.0/LICENSE` & `efrem_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.1.0/README.md` & `efrem_utils-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,69 @@
-# `efrem-utils`
-
-A package with utility functions to abstract some logic. 
-
-## `explanation`
-
-### `validated_input` usage:
-
-The `validated_input` exists to simplify getting a valid input from a user that passes some criterias.
-
-Its signature/definition might be a bit hard to read, so a bit of an explanation:
-```py
----
-msg: A string / None (by default), will be used as the prompt for the input() calls.
-If its None - it defaults to f"Enter a {constructor}: "
---- # After msg, all arguments are keyword-only
-precomp(utational function): A function which has to take a string and return.. anything, pretty much.
-Honourable mentions: str.strip, str.lower, str.split. Defaults to None so it doesnt mutate the input.
----
-validators: An iterable with tuples (pairs) of function:error_message.
-
-The functions needs to accept the same type that the precomp function returns.
-
-The error_message is displayed when either an exception is raised during the attempt of validation [Which leads to a neat trick for getting a valid input of some type], or when the value it returns is falsy.
-
-The error message can be either None (in this case it wont be displayed), or a static string, or a template-string [i.e "{buffer} is not an integer". Consider that `buffer` is the keyword for the users input here, which gets passed with a .format(buffer=buffer) call]
-
-Defaults to None and gets replaced by a typecheck using the constructor and a short-circuit logic. [constructor(buffer) or True]
----
-constructor: A function which needs to take the same type that the precomp function returns and it will be used to actually return the value once the input has been validated.
-
-Defaults to str :D
----
-The function returns another function so you can then call it with no arguments and get a validated input.
-```
-
-```py
-# Some examples:
-
-get_float = efrem_utils.validated_input(constructor=float) # Works because of validators defaulting to a float typecheck and msg defaulting to f"Enter a {float}"
-
-choices = ["a", "bob", "yes"]
-get_choice = efrem_utils.validated_input(
-    msg=f"Enter your choice [Choose from <{','.join(choices)}>]: ",
-    validators=[
-        (lambda buffer: buffer in choices, "{buffer} is not a valid choice") # the {buffer} in the template string is important
-    ],
-    precomp=lambda buffer: buffer.lower().strip() # using lambda to combine multiple precomputation functions
-)
-```
-
-**For more information check:** [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
+Metadata-Version: 2.1
+Name: efrem-utils
+Version: 0.1.1
+Summary: Efrem's utilities
+Home-page: https://github.com/NikitaNightBot/efrem-utils
+Author: lone_druid
+Author-email: enikita332@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/NikitaNightBot/efrem-utils
+Description-Content-Type: text/markdown
+
+# `efrem-utils`
+
+A package with utility functions to abstract some logic. 
+
+## `explanation`
+
+### `validated_input` usage:
+
+The `validated_input` exists to simplify getting a valid input from a user that passes some criterias.
+
+Its signature/definition might be a bit hard to read, so a bit of an explanation:
+```py
+---
+msg: A string / None (by default), will be used as the prompt for the input() calls.
+If its None - it defaults to f"Enter a {constructor}: "
+---
+precomp(utational function): A function which has to take a string and return.. anything, pretty much.
+Honourable mentions: str.strip, str.lower, str.split. Defaults to None so it doesnt mutate the input.
+!! The constructor is applied when returning the value, so be careful with typecasting in precomputation, i.e if you use `int` as a precomputational function but constructor stays at default (str) -> a string will be returned !!
+---
+# Added in 0.1.1
+precomp_error: A string / a callable that accepts a string and returns a string / a template string (format keyword = buffer). This prints when precomp(input) raises an exception (i.e tried to use int as precomp -> entered a non-integer)
+---
+validators: An iterable with tuples (pairs) of function:error_message.
+
+The functions needs to accept the same type that the precomp function returns.
+
+The error_message is displayed when either an exception is raised during the attempt of validation [Which leads to a neat trick for getting a valid input of some type], or when the value it returns is falsy.
+
+The error message can be either None (in this case it wont be displayed), or a static string, or a template-string [i.e "{buffer} is not an integer". Consider that `buffer` is the keyword for the users input here, which gets passed with a .format(buffer=buffer) call]
+
+Defaults to None and gets replaced by a typecheck using the constructor and a short-circuit logic. [constructor(buffer) or True]
+---
+constructor: A function which needs to take the same type that the precomp function returns and it will be used to actually return the value once the input has been validated.
+
+Defaults to str :D
+---
+The function returns another function so you can then call it with no arguments and get a validated input.
+```
+
+```py
+# Some examples:
+
+get_float = efrem_utils.validated_input(constructor=float) # Works because of validators defaulting to a float typecheck and msg defaulting to f"Enter a {float}"
+
+choices = ["a", "bob", "yes"]
+get_choice = efrem_utils.validated_input(
+    msg=f"Enter your choice [Choose from <{','.join(choices)}>]: ",
+    validators=[
+        (lambda buffer: buffer in choices, "{buffer} is not a valid choice") # the {buffer} in the template string is important
+    ],
+    precomp=lambda buffer: buffer.lower().strip() # using lambda to combine multiple precomputation functions
+)
+```
+
+**For more information check:** [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
```

### Comparing `efrem_utils-0.1.0/PKG-INFO` & `efrem_utils-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,56 @@
-Metadata-Version: 2.1
-Name: efrem-utils
-Version: 0.1.0
-Summary: Efrem's utilities
-Home-page: https://github.com/NikitaNightBot/efrem-utils
-Author: lone_druid
-Author-email: enikita332@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/NikitaNightBot/efrem-utils
-Description-Content-Type: text/markdown
-
-# `efrem-utils`
-
-A package with utility functions to abstract some logic. 
-
-## `explanation`
-
-### `validated_input` usage:
-
-The `validated_input` exists to simplify getting a valid input from a user that passes some criterias.
-
-Its signature/definition might be a bit hard to read, so a bit of an explanation:
-```py
----
-msg: A string / None (by default), will be used as the prompt for the input() calls.
-If its None - it defaults to f"Enter a {constructor}: "
---- # After msg, all arguments are keyword-only
-precomp(utational function): A function which has to take a string and return.. anything, pretty much.
-Honourable mentions: str.strip, str.lower, str.split. Defaults to None so it doesnt mutate the input.
----
-validators: An iterable with tuples (pairs) of function:error_message.
-
-The functions needs to accept the same type that the precomp function returns.
-
-The error_message is displayed when either an exception is raised during the attempt of validation [Which leads to a neat trick for getting a valid input of some type], or when the value it returns is falsy.
-
-The error message can be either None (in this case it wont be displayed), or a static string, or a template-string [i.e "{buffer} is not an integer". Consider that `buffer` is the keyword for the users input here, which gets passed with a .format(buffer=buffer) call]
-
-Defaults to None and gets replaced by a typecheck using the constructor and a short-circuit logic. [constructor(buffer) or True]
----
-constructor: A function which needs to take the same type that the precomp function returns and it will be used to actually return the value once the input has been validated.
-
-Defaults to str :D
----
-The function returns another function so you can then call it with no arguments and get a validated input.
-```
-
-```py
-# Some examples:
-
-get_float = efrem_utils.validated_input(constructor=float) # Works because of validators defaulting to a float typecheck and msg defaulting to f"Enter a {float}"
-
-choices = ["a", "bob", "yes"]
-get_choice = efrem_utils.validated_input(
-    msg=f"Enter your choice [Choose from <{','.join(choices)}>]: ",
-    validators=[
-        (lambda buffer: buffer in choices, "{buffer} is not a valid choice") # the {buffer} in the template string is important
-    ],
-    precomp=lambda buffer: buffer.lower().strip() # using lambda to combine multiple precomputation functions
-)
-```
-
-**For more information check:** [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
+# `efrem-utils`
+
+A package with utility functions to abstract some logic. 
+
+## `explanation`
+
+### `validated_input` usage:
+
+The `validated_input` exists to simplify getting a valid input from a user that passes some criterias.
+
+Its signature/definition might be a bit hard to read, so a bit of an explanation:
+```py
+---
+msg: A string / None (by default), will be used as the prompt for the input() calls.
+If its None - it defaults to f"Enter a {constructor}: "
+---
+precomp(utational function): A function which has to take a string and return.. anything, pretty much.
+Honourable mentions: str.strip, str.lower, str.split. Defaults to None so it doesnt mutate the input.
+!! The constructor is applied when returning the value, so be careful with typecasting in precomputation, i.e if you use `int` as a precomputational function but constructor stays at default (str) -> a string will be returned !!
+---
+# Added in 0.1.1
+precomp_error: A string / a callable that accepts a string and returns a string / a template string (format keyword = buffer). This prints when precomp(input) raises an exception (i.e tried to use int as precomp -> entered a non-integer)
+---
+validators: An iterable with tuples (pairs) of function:error_message.
+
+The functions needs to accept the same type that the precomp function returns.
+
+The error_message is displayed when either an exception is raised during the attempt of validation [Which leads to a neat trick for getting a valid input of some type], or when the value it returns is falsy.
+
+The error message can be either None (in this case it wont be displayed), or a static string, or a template-string [i.e "{buffer} is not an integer". Consider that `buffer` is the keyword for the users input here, which gets passed with a .format(buffer=buffer) call]
+
+Defaults to None and gets replaced by a typecheck using the constructor and a short-circuit logic. [constructor(buffer) or True]
+---
+constructor: A function which needs to take the same type that the precomp function returns and it will be used to actually return the value once the input has been validated.
+
+Defaults to str :D
+---
+The function returns another function so you can then call it with no arguments and get a validated input.
+```
+
+```py
+# Some examples:
+
+get_float = efrem_utils.validated_input(constructor=float) # Works because of validators defaulting to a float typecheck and msg defaulting to f"Enter a {float}"
+
+choices = ["a", "bob", "yes"]
+get_choice = efrem_utils.validated_input(
+    msg=f"Enter your choice [Choose from <{','.join(choices)}>]: ",
+    validators=[
+        (lambda buffer: buffer in choices, "{buffer} is not a valid choice") # the {buffer} in the template string is important
+    ],
+    precomp=lambda buffer: buffer.lower().strip() # using lambda to combine multiple precomputation functions
+)
+```
+
+**For more information check:** [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
```

