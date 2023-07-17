# Comparing `tmp/codeinterpreterapi-0.0.5.tar.gz` & `tmp/codeinterpreterapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinterpreterapi-0.0.5.tar", max compression
+gzip compressed data, was "codeinterpreterapi-0.0.6.tar", max compression
```

## Comparing `codeinterpreterapi-0.0.5.tar` & `codeinterpreterapi-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.5/LICENSE
--rw-r--r--   0        0        0     2476 2023-07-16 09:17:02.062499 codeinterpreterapi-0.0.5/README.md
--rw-r--r--   0        0        0       62 2023-07-14 11:46:56.280365 codeinterpreterapi-0.0.5/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.5/codeinterpreterapi/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/functions_agent.py
--rw-r--r--   0        0        0     3054 2023-07-14 17:11:05.973711 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0     1836 2023-07-14 17:11:05.948871 codeinterpreterapi-0.0.5/codeinterpreterapi/chains/remove_download_link.py
--rw-r--r--   0        0        0      336 2023-07-14 17:11:05.942603 codeinterpreterapi-0.0.5/codeinterpreterapi/config.py
--rw-r--r--   0        0        0       78 2023-07-14 17:11:05.936317 codeinterpreterapi-0.0.5/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.5/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/__init__.py
--rw-r--r--   0        0        0     2301 2023-07-15 13:40:20.463191 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/file.py
--rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/input.py
--rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.5/codeinterpreterapi/schema/response.py
--rw-r--r--   0        0        0     7979 2023-07-16 08:46:08.541001 codeinterpreterapi-0.0.5/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      629 2023-07-16 09:23:19.074950 codeinterpreterapi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3513 2023-07-17 11:19:56.497686 codeinterpreterapi-0.0.6/README.md
+-rw-r--r--   0        0        0      104 2023-07-16 13:21:57.042269 codeinterpreterapi-0.0.6/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.6/codeinterpreterapi/callbacks.py
+-rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/functions_agent.py
+-rw-r--r--   0        0        0     1578 2023-07-17 13:27:01.999997 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0      977 2023-07-17 11:28:50.790393 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/remove_download_link.py
+-rw-r--r--   0        0        0      370 2023-07-17 13:25:52.072577 codeinterpreterapi-0.0.6/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0      225 2023-07-17 11:27:36.915415 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1379 2023-07-17 11:23:07.801403 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/modifications_check.py
+-rw-r--r--   0        0        0      959 2023-07-17 11:26:26.313924 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/remove_dl_link.py
+-rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/__init__.py
+-rw-r--r--   0        0        0     2308 2023-07-16 23:45:20.639555 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/file.py
+-rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/input.py
+-rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/response.py
+-rw-r--r--   0        0        0     8129 2023-07-17 13:26:32.320429 codeinterpreterapi-0.0.6/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      629 2023-07-17 13:28:21.645307 codeinterpreterapi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.6/PKG-INFO
```

### Comparing `codeinterpreterapi-0.0.5/LICENSE` & `codeinterpreterapi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.5/README.md` & `codeinterpreterapi-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,75 +6,110 @@
 You can run everything local except the LLM using your own OpenAI API Key.
 
 ## Features
 
 - Dataset Analysis, Stock Charting, Image Manipulation, ....
 - Internet access and auto Python package installation
 - Input `text + files` -> Receive `text + files`
-- Run everything local except the OpenAI API (OpenOrca or others coming soon)
+- Conversation Memory: respond based on previous inputs
+- Run everything local except the OpenAI API (OpenOrca or others maybe soon)
 - Use CodeBox API for easy scaling in production (coming soon)
 
 ## Installation
 
 Get your OpenAI API Key [here](https://platform.openai.com/account/api-keys) and install the package.
 
 ```bash
 pip install codeinterpreterapi
 ```
 
 ## Usage
 
+Make sure to set the `OPENAI_API_KEY` environment variable (or use a `.env` file)
+
 ```python
 from codeinterpreterapi import CodeInterpreterSession
 
 
 async def main():
-    # start a session
+    # create a session
     session = CodeInterpreterSession()
     await session.astart()
 
     # generate a response based on user input
     output = await session.generate_response(
         "Plot the bitcoin chart of 2023 YTD"
     )
-    # show output image in default image viewer
-    file = output.files[0]
-    file.show_image()
 
-    # show output text
-    print("AI: ", output.content)
+    # ouput the response (text + image)
+    print("AI: ", response.content)
+    for file in response.files:
+        file.show_image()
 
     # terminate the session
     await session.astop()
     
 
 if __name__ == "__main__":
-    import asyncio, os
-    os.environ["OPENAI_API_KEY"] = "sk-*********"  # or .env file
-
+    import asyncio
+    # run the async function
     asyncio.run(main())
 
 ```
 
-## Output
+![Bitcoin YTD](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/bitcoin_chart.png?raw=true)  
+Bitcoin YTD Chart Output
+
+## Dataset Analysis
+
+```python
+from codeinterpreterapi import CodeInterpreterSession, File
+
+
+async def main():
+    # context manager for auto start/stop of the session
+    async with CodeInterpreterSession() as session:
+        # define the user request
+        user_request = "Analyze this dataset and plot something interesting about it."
+        files = [
+            File.from_path("examples/assets/iris.csv"),
+        ]
+        
+        # generate the response
+        response = await session.generate_response(
+            user_request, files=files
+        )
+
+        # output to the user
+        print("AI: ", response.content)
+        for file in response.files:
+            file.show_image()
+
+
+if __name__ == "__main__":
+    import asyncio
+
+    asyncio.run(main())
+```
 
-![Bitcoin YTD](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/bitcoin_chart.png?raw=true)
+![Iris Dataset Analysis](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/iris_analysis.png?raw=true)  
+Iris Dataset Analysis Output
 
 ## Production
 
 In case you want to deploy to production you can use the CodeBox API for easy scaling.
 
 Please contact me if you interested in this, because it's still in early development.
 
 ## Contributing
 
 There are some TODOs left in the code
 so if you want to contribute feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
-Just open an issue pull request and I will review it.
+Just open an issue or pull request and I will review it.
 
 Also please submit any bugs you find as an issue
 with a minimal code example or screenshot.
 This helps me a lot to improve the code.
 
 Thanks!
```

### Comparing `codeinterpreterapi-0.0.5/codeinterpreterapi/callbacks.py` & `codeinterpreterapi-0.0.6/codeinterpreterapi/callbacks.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.5/codeinterpreterapi/chains/functions_agent.py` & `codeinterpreterapi-0.0.6/codeinterpreterapi/chains/functions_agent.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.5/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.5/codeinterpreterapi/schema/file.py` & `codeinterpreterapi-0.0.6/codeinterpreterapi/schema/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def from_path(cls, path: str):
         with open(path, "rb") as f:
             path = path.split("/")[-1]
             return cls(name=path, content=f.read())
 
     @classmethod
     async def afrom_path(cls, path: str):
-        await asyncio.to_thread(cls.from_path, path)
+        return await asyncio.to_thread(cls.from_path, path)
 
     @classmethod
     def from_url(cls, url: str):
         import requests  # type: ignore
 
         r = requests.get(url)
         return cls(name=url.split("/")[-1], content=r.content)
```

### Comparing `codeinterpreterapi-0.0.5/codeinterpreterapi/schema/response.py` & `codeinterpreterapi-0.0.6/codeinterpreterapi/schema/response.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.5/codeinterpreterapi/session.py` & `codeinterpreterapi-0.0.6/codeinterpreterapi/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import uuid, base64, re
 from io import BytesIO
+from typing import Optional
 from codeboxapi import CodeBox  # type: ignore
 from codeboxapi.schema import CodeBoxOutput  # type: ignore
 from langchain.tools import StructuredTool
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.prompts.chat import MessagesPlaceholder
 from langchain.agents import AgentExecutor, BaseSingleActionAgent
@@ -41,15 +42,15 @@
                 "Variables are preserved between runs. ",
                 func=self.run_handler,
                 coroutine=self.arun_handler,
                 args_schema=CodeInput,
             ),
         ]
 
-    def _llm(self, model: str | None, openai_api_key: str | None) -> BaseChatModel:
+    def _llm(self, model: Optional[str] = None, openai_api_key: Optional[str] = None) -> BaseChatModel:
         if model is None:
             model = "gpt-4"
 
         if openai_api_key is None:
             if settings.OPENAI_API_KEY is None:
                 raise ValueError("OpenAI API key missing.")
             else:
@@ -179,14 +180,17 @@
                 )
             else:
                 return CodeInterpreterResponse(
                     content="Sorry, something went while generating your response."
                     "Please try again or restart the session."
                 )
 
+    async def is_running(self) -> bool:
+        return await self.codebox.astatus() == "running"
+    
     async def astop(self) -> None:
         await self.codebox.astop()
     
     async def __aenter__(self) -> "CodeInterpreterSession":
         await self.astart()
         return self
```

### Comparing `codeinterpreterapi-0.0.5/pyproject.toml` & `codeinterpreterapi-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "codeinterpreterapi"
-version = "0.0.5"
+version = "0.0.6"
 description = "CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter."
 authors = ["Shroominic <pleurae-berets.0u@icloud.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 openai = "^0.27.8"
 langchain = "^0.0.232"
-codeboxapi = "^0.0.7"
+codeboxapi = "^0.0.8"
 
 [tool.poetry.extras]
 image_support = ["Pillow"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.1"
```

### Comparing `codeinterpreterapi-0.0.5/PKG-INFO` & `codeinterpreterapi-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: codeinterpreterapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: image-support
-Requires-Dist: codeboxapi (>=0.0.7,<0.0.8)
+Requires-Dist: codeboxapi (>=0.0.8,<0.0.9)
 Requires-Dist: langchain (>=0.0.232,<0.0.233)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Code Interpreter API
 
@@ -26,75 +26,110 @@
 You can run everything local except the LLM using your own OpenAI API Key.
 
 ## Features
 
 - Dataset Analysis, Stock Charting, Image Manipulation, ....
 - Internet access and auto Python package installation
 - Input `text + files` -> Receive `text + files`
-- Run everything local except the OpenAI API (OpenOrca or others coming soon)
+- Conversation Memory: respond based on previous inputs
+- Run everything local except the OpenAI API (OpenOrca or others maybe soon)
 - Use CodeBox API for easy scaling in production (coming soon)
 
 ## Installation
 
 Get your OpenAI API Key [here](https://platform.openai.com/account/api-keys) and install the package.
 
 ```bash
 pip install codeinterpreterapi
 ```
 
 ## Usage
 
+Make sure to set the `OPENAI_API_KEY` environment variable (or use a `.env` file)
+
 ```python
 from codeinterpreterapi import CodeInterpreterSession
 
 
 async def main():
-    # start a session
+    # create a session
     session = CodeInterpreterSession()
     await session.astart()
 
     # generate a response based on user input
     output = await session.generate_response(
         "Plot the bitcoin chart of 2023 YTD"
     )
-    # show output image in default image viewer
-    file = output.files[0]
-    file.show_image()
 
-    # show output text
-    print("AI: ", output.content)
+    # ouput the response (text + image)
+    print("AI: ", response.content)
+    for file in response.files:
+        file.show_image()
 
     # terminate the session
     await session.astop()
     
 
 if __name__ == "__main__":
-    import asyncio, os
-    os.environ["OPENAI_API_KEY"] = "sk-*********"  # or .env file
-
+    import asyncio
+    # run the async function
     asyncio.run(main())
 
 ```
 
-## Output
+![Bitcoin YTD](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/bitcoin_chart.png?raw=true)  
+Bitcoin YTD Chart Output
+
+## Dataset Analysis
+
+```python
+from codeinterpreterapi import CodeInterpreterSession, File
+
+
+async def main():
+    # context manager for auto start/stop of the session
+    async with CodeInterpreterSession() as session:
+        # define the user request
+        user_request = "Analyze this dataset and plot something interesting about it."
+        files = [
+            File.from_path("examples/assets/iris.csv"),
+        ]
+        
+        # generate the response
+        response = await session.generate_response(
+            user_request, files=files
+        )
+
+        # output to the user
+        print("AI: ", response.content)
+        for file in response.files:
+            file.show_image()
+
+
+if __name__ == "__main__":
+    import asyncio
+
+    asyncio.run(main())
+```
 
-![Bitcoin YTD](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/bitcoin_chart.png?raw=true)
+![Iris Dataset Analysis](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/iris_analysis.png?raw=true)  
+Iris Dataset Analysis Output
 
 ## Production
 
 In case you want to deploy to production you can use the CodeBox API for easy scaling.
 
 Please contact me if you interested in this, because it's still in early development.
 
 ## Contributing
 
 There are some TODOs left in the code
 so if you want to contribute feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
-Just open an issue pull request and I will review it.
+Just open an issue or pull request and I will review it.
 
 Also please submit any bugs you find as an issue
 with a minimal code example or screenshot.
 This helps me a lot to improve the code.
 
 Thanks!
```

