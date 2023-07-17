# Comparing `tmp/oyehr-tools-package-0.0.2.tar.gz` & `tmp/oyehr-tools-package-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oyehr-tools-package-0.0.2.tar", last modified: Mon Jul 17 02:43:41 2023, max compression
+gzip compressed data, was "oyehr-tools-package-0.0.3.tar", last modified: Mon Jul 17 03:39:08 2023, max compression
```

## Comparing `oyehr-tools-package-0.0.2.tar` & `oyehr-tools-package-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.080912 oyehr-tools-package-0.0.2/
--rw-rw-rw-   0        0        0       39 2023-07-17 02:32:40.000000 oyehr-tools-package-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      101 2023-07-17 02:43:41.080912 oyehr-tools-package-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4101 2023-07-17 02:33:30.000000 oyehr-tools-package-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.039913 oyehr-tools-package-0.0.2/oyehr_tool_package/
--rw-rw-rw-   0        0        0       82 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.055913 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/
--rw-rw-rw-   0        0        0       82 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/__init__.py
--rw-rw-rw-   0        0        0      476 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/my_tool_1.py
--rw-rw-rw-   0        0        0      697 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/my_tool_2.py
--rw-rw-rw-   0        0        0      524 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.058913 oyehr-tools-package-0.0.2/oyehr_tool_package/yamls/
--rw-rw-rw-   0        0        0      302 2023-07-17 02:42:43.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/yamls/my_tool_1.yaml
--rw-rw-rw-   0        0        0      333 2023-07-17 02:42:48.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/yamls/my_tool_2.yaml
-drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.076911 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/
--rw-rw-rw-   0        0        0      101 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 02:43:41.081912 oyehr-tools-package-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      409 2023-07-17 02:43:30.000000 oyehr-tools-package-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.078910 oyehr-tools-package-0.0.2/tests/
--rw-rw-rw-   0        0        0      711 2023-07-17 02:33:14.000000 oyehr-tools-package-0.0.2/tests/test_my_tool_1.py
--rw-rw-rw-   0        0        0      867 2023-07-17 02:33:06.000000 oyehr-tools-package-0.0.2/tests/test_my_tool_2.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:39:08.272485 oyehr-tools-package-0.0.3/
+-rw-rw-rw-   0        0        0       39 2023-07-17 02:32:40.000000 oyehr-tools-package-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      101 2023-07-17 03:39:08.271486 oyehr-tools-package-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4101 2023-07-17 02:33:30.000000 oyehr-tools-package-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 03:39:08.236241 oyehr-tools-package-0.0.3/oyehr_tool_package/
+-rw-rw-rw-   0        0        0       82 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.3/oyehr_tool_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:39:08.244241 oyehr-tools-package-0.0.3/oyehr_tool_package/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.3/oyehr_tool_package/tools/__init__.py
+-rw-rw-rw-   0        0        0      581 2023-07-17 03:37:33.000000 oyehr-tools-package-0.0.3/oyehr_tool_package/tools/my_tool_1.py
+-rw-rw-rw-   0        0        0      791 2023-07-17 03:38:18.000000 oyehr-tools-package-0.0.3/oyehr_tool_package/tools/my_tool_2.py
+-rw-rw-rw-   0        0        0      524 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.3/oyehr_tool_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:39:08.248241 oyehr-tools-package-0.0.3/oyehr_tool_package/yamls/
+-rw-rw-rw-   0        0        0      302 2023-07-17 02:42:43.000000 oyehr-tools-package-0.0.3/oyehr_tool_package/yamls/my_tool_1.yaml
+-rw-rw-rw-   0        0        0      333 2023-07-17 02:42:48.000000 oyehr-tools-package-0.0.3/oyehr_tool_package/yamls/my_tool_2.yaml
+drwxrwxrwx   0        0        0        0 2023-07-17 03:39:08.265971 oyehr-tools-package-0.0.3/oyehr_tools_package.egg-info/
+-rw-rw-rw-   0        0        0      101 2023-07-17 03:39:08.000000 oyehr-tools-package-0.0.3/oyehr_tools_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-07-17 03:39:08.000000 oyehr-tools-package-0.0.3/oyehr_tools_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 03:39:08.000000 oyehr-tools-package-0.0.3/oyehr_tools_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-17 03:39:08.000000 oyehr-tools-package-0.0.3/oyehr_tools_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 03:39:08.000000 oyehr-tools-package-0.0.3/oyehr_tools_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 03:39:08.273486 oyehr-tools-package-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-07-17 03:37:30.000000 oyehr-tools-package-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:39:08.269478 oyehr-tools-package-0.0.3/tests/
+-rw-rw-rw-   0        0        0      711 2023-07-17 02:33:14.000000 oyehr-tools-package-0.0.3/tests/test_my_tool_1.py
+-rw-rw-rw-   0        0        0      867 2023-07-17 02:33:06.000000 oyehr-tools-package-0.0.3/tests/test_my_tool_2.py
```

### Comparing `oyehr-tools-package-0.0.2/README.md` & `oyehr-tools-package-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oyehr-tools-package-0.0.2/oyehr_tool_package/tools/my_tool_2.py` & `oyehr-tools-package-0.0.3/tests/test_my_tool_1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-from promptflow.core.tool import ToolProvider, tool
+import pytest
+import unittest
+
 from promptflow.connections import CustomConnection
+from oyehr_tool_package.tools.my_tool_1 import my_tool
+
+
+@pytest.fixture
+def my_custom_connection() -> CustomConnection:
+    my_custom_connection = CustomConnection(
+        {
+            "api-key" : "my-api-key",
+            "api-secret" : "my-api-secret",
+            "api-url" : "my-api-url"
+        }
+    )
+    return my_custom_connection
+
+
+class TestMyTool1:
+    def test_my_tool_1(self, my_custom_connection):
+        result = my_tool(my_custom_connection, input_text="Microsoft")
+        assert result == "Hello Microsoft"
 
 
-class MyTool(ToolProvider):
-    """
-    Doc reference :
-    """
-
-    def __init__(self, connection: CustomConnection):
-        super().__init__()
-        self.connection = connection
-
-    @tool
-    def my_tool(self, input_text: str) -> str:
-        # Replace with your tool code.
-        # Usually connection contains configs to connect to an API.
-        # Use CustomConnection is a dict. You can use it like: connection.api_key, connection.api_base
-        # Not all tools need a connection. You can remove it if you don't need it.
-        return "Hello " + input_text
+# Run the unit tests
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `oyehr-tools-package-0.0.2/oyehr_tool_package/tools/utils.py` & `oyehr-tools-package-0.0.3/oyehr_tool_package/tools/utils.py`

 * *Files identical despite different names*

### Comparing `oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/SOURCES.txt` & `oyehr-tools-package-0.0.3/oyehr_tools_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oyehr-tools-package-0.0.2/tests/test_my_tool_1.py` & `oyehr-tools-package-0.0.3/tests/test_my_tool_2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import pytest
 import unittest
 
 from promptflow.connections import CustomConnection
-from oyehr_tool_package.tools.my_tool_1 import my_tool
+from oyehr_tool_package.tools.my_tool_2 import MyTool
 
 
 @pytest.fixture
 def my_custom_connection() -> CustomConnection:
     my_custom_connection = CustomConnection(
         {
             "api-key" : "my-api-key",
             "api-secret" : "my-api-secret",
             "api-url" : "my-api-url"
         }
     )
     return my_custom_connection
 
 
-class TestMyTool1:
-    def test_my_tool_1(self, my_custom_connection):
-        result = my_tool(my_custom_connection, input_text="Microsoft")
+@pytest.fixture
+def my_tool_provider(my_custom_connection) -> MyTool:
+    my_tool_provider = MyTool(my_custom_connection)
+    return my_tool_provider
+
+
+class TestMyTool2:
+    def test_my_tool_2(self, my_tool_provider: MyTool):
+        result = my_tool_provider.my_tool(input_text="Microsoft")
         assert result == "Hello Microsoft"
 
 
 # Run the unit tests
 if __name__ == "__main__":
     unittest.main()
```

