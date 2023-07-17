# Comparing `tmp/langchain_plantuml-0.0.2.tar.gz` & `tmp/langchain_plantuml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_plantuml-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "langchain_plantuml-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `langchain_plantuml-0.0.2.tar` & `langchain_plantuml-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11356 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/LICENSE
--rw-r--r--   0        0        0     2612 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/README.md
--rw-r--r--   0        0        0      573 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/__init__.py
--rw-r--r--   0        0        0      573 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/__init__.py
--rw-r--r--   0        0        0     9282 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
--rw-r--r--   0        0        0      573 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/core/__init__.py
--rw-r--r--   0        0        0     2891 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/core/plantuml_callback_handler.py
--rw-r--r--   0        0        0      888 2023-07-16 15:17:34.724287 langchain_plantuml-0.0.2/langchain_plantuml/diagram.py
--rw-r--r--   0        0        0     1749 2023-07-16 15:17:34.724287 langchain_plantuml-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3724 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2870 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/README.md
+-rw-r--r--   0        0        0      573 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/langchain_plantuml/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/__init__.py
+-rw-r--r--   0        0        0     9386 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
+-rw-r--r--   0        0        0    13242 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py
+-rw-r--r--   0        0        0      573 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/core/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/core/plantuml_callback_handler.py
+-rw-r--r--   0        0        0     1139 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/diagram.py
+-rw-r--r--   0        0        0     1749 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.3/PKG-INFO
```

### Comparing `langchain_plantuml-0.0.2/LICENSE` & `langchain_plantuml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.2/README.md` & `langchain_plantuml-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPi version](https://img.shields.io/pypi/v/langchain-plantuml.svg)](https://pypi.org/project/langchain-plantuml/)
 [![lint](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml)
 [![Build status](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/release.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/pypi/dm/langchain-plantuml)](https://pypi.org/project/langchain-plantuml/)
 
-Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
+Subscribe to events using a callback and store them in PlantUML format **Activity Diagram** and **Sequence Diagram**. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 
-![](screenshot/scene_agent.png)
+Activity Diagram 
+
+![](screenshot/activity-diagram.png)
+
+Sequence Diagram
+
+![](screenshot/sequence-diagram.png)
 
 ## Quick Start
 
 Install this library:
 
 ```shell
 pip install langchain-plantuml
@@ -24,15 +30,15 @@
 1. Add import langchain_plantuml as the first import in your Python entrypoint file
 2. Create a callback using the activity_diagram_callback function
 3. Hook into your LLM application
 4. Call the export_uml_content method of activity_diagram_callback to export the PlantUML content
 5. Save PlantUML content to a file
 6. Exporting PlantUML to PNG
 
-Running the minimal example.
+Running the minimal activity diagram example.
 
 ```python
 from langchain import OpenAI, LLMChain, PromptTemplate
 from langchain.memory import ConversationBufferMemory
 
 from langchain_plantuml import diagram
 
@@ -56,22 +62,28 @@
     memory=memory,
     callbacks=[callback_handler]
 )
 
 llm_chain.predict(human_input="Hi there my friend")
 llm_chain.predict(human_input="Not too bad - how are you?")
 
-callback_handler.save_uml_content("example.puml")
+callback_handler.save_uml_content("example-activity.puml")
 ```
 
 You will get the following PlantUML activity diagram
 
-![](screenshot/example.png)
+![](screenshot/example-activity.png)
+
+Sequence Diagram
+
+```python
+callback_handler = diagram.sequence_diagram_callback()
+```
 
 ## Exporting PlantUML to PNG
 
 You can download [plantuml.1.2023.10.jar](https://github.com/plantuml/plantuml/releases/download/v1.2023.10/plantuml-1.2023.10.jar)
 
 ```shell
-java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example.puml
+java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example-activity.puml
 ```
```

### Comparing `langchain_plantuml-0.0.2/langchain_plantuml/__init__.py` & `langchain_plantuml-0.0.3/langchain_plantuml/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/__init__.py` & `langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py` & `langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,18 @@
                 if serialized.get("name") is not None
                 else serialized["id"][len(serialized["id"]) - 1]
             )
             self._runs_metrics[run_id]["name"] = run_name
 
         return self._runs_metrics[run_id]
 
+    def _append_uml_activity(self, line):
+        self.uml_content.append(line)
+        self.step += 1
+
     def _append_uml_notes(self, align: str = "left", notes: List[str] = []):
         if len(notes) > 0:
             self._append_uml_line(f"note {align}")
             self._append_uml_multi_line(notes)
             self._append_uml_line("end note")
 
     def _wrapper_activity_name(self, method_name: str, run_name: str) -> str:
```

### Comparing `langchain_plantuml-0.0.2/langchain_plantuml/core/__init__.py` & `langchain_plantuml-0.0.3/langchain_plantuml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.2/langchain_plantuml/core/plantuml_callback_handler.py` & `langchain_plantuml-0.0.3/langchain_plantuml/core/plantuml_callback_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from typing import List
 
 from langchain.callbacks.base import BaseCallbackHandler
 
 
-class BasePlantUMLCallbackHandler(BaseCallbackHandler):
-    step: int = 0
-    uml_content: List[str] = []
-    total_tokens: int = 0
-    prompt_tokens: int = 0
-    completion_tokens: int = 0
+class BasePlantUMLCallbackHandler(BaseCallbackHandler, ABC):
     crlf: str = "⏎"
     note_max_length: int = 1000
     emojis = {
         "on_llm_start": "<:1f916:>",
         "on_llm_end": "<:1f916:>",
         "on_chain_start": "<:1f3af:>",
         "on_chain_end": "<:1f3af:>",
         "on_tool_start": "<:1f528:>",
         "on_tool_end": "<:1f528:>",
         "on_text": "<:1f4c6:>",
     }
 
     def __init__(self):
+        self.step = 0
+        self.total_tokens = 0
+        self.prompt_tokens = 0
+        self.completion_tokens = 0
+        self.uml_content = []
         self.uml_content.append("@startuml")
         self.uml_content.append("skinparam dpi 300")
         self.uml_content.append("skinparam wrapWidth 500")
         self.uml_content.append("skinparam shadowing false")
         self.uml_content.append("skinparam noteFontName Arial")
         self.uml_content.append("skinparam noteFontSize 10")
         self.uml_content.append("skinparam noteBackgroundColor #ECECEC")
@@ -58,21 +58,17 @@
         with open(file_path, "w") as f:
             for line in self.export_uml_content():
                 f.write(str(line) + "\n")
 
     def _append_uml_line(self, line):
         self.uml_content.append(line)
 
-    def _append_uml_activity(self, line):
-        self.uml_content.append(line)
-        self.step += 1
-
     def _append_uml_multi_line(self, lines: List[str]):
         for line in lines:
             self.uml_content.append(line)
 
     def _wrapper_note(self, note: str) -> List[str]:
         new_note = note.strip()
         if len(new_note) > self.note_max_length:
-            new_note = f"new_note[:line_max_limit] ... (Omit {len(new_note) - self.note_max_length} words)"
+            new_note = f"{new_note[:self.note_max_length]} ... (Omit {len(new_note) - self.note_max_length} words)"
         new_lines = [f"{line}{self.crlf}" for line in new_note.split("\n")]
         return new_lines
```

### Comparing `langchain_plantuml-0.0.2/langchain_plantuml/diagram.py` & `langchain_plantuml-0.0.3/langchain_plantuml/diagram.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,11 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from langchain.callbacks.base import BaseCallbackHandler
 
 from langchain_plantuml.activity_diagram_beta.plantuml_activity_diagram_beta_callback_handler import \
     PlantUMLActivityDiagramCallbackHandler
+from langchain_plantuml.activity_diagram_beta.plantuml_sequence_diagram_callback_handler import \
+    PlantUMLSequenceDiagramCallbackHandler
 
 
 def activity_diagram_callback() -> BaseCallbackHandler:
     return PlantUMLActivityDiagramCallbackHandler()
+
+
+def sequence_diagram_callback() -> BaseCallbackHandler:
+    return PlantUMLSequenceDiagramCallbackHandler()
```

### Comparing `langchain_plantuml-0.0.2/pyproject.toml` & `langchain_plantuml-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [build-system]
 requires = ["flit_core==3.9.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "langchain-plantuml"
-version = "0.0.2"
+version = "0.0.3"
 description = "Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze."
 authors = [{ name = "Lei Zhang", email = "zhanglei@apache.org" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "langchain==0.0.228"
@@ -45,15 +45,15 @@
     "coverage==7.2.7"
 ]
 package = [
     "flit==3.9.0"
 ]
 
 [tool.flake8]
-max-line-length = 120
+max-line-length = 180
 ignore = ['E231', 'E241', 'W291', 'W293']
 per-file-ignores = [
     '__init__.py:F401',
 ]
 count = true
 
 [project.urls]
```

### Comparing `langchain_plantuml-0.0.2/PKG-INFO` & `langchain_plantuml-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-plantuml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 Author-email: Lei Zhang <zhanglei@apache.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: langchain==0.0.228
 Requires-Dist: flake8==5.0.4 ; extra == "lint"
 Requires-Dist: pyproject-flake8==5.0.4 ; extra == "lint"
@@ -27,17 +27,23 @@
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPi version](https://img.shields.io/pypi/v/langchain-plantuml.svg)](https://pypi.org/project/langchain-plantuml/)
 [![lint](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml)
 [![Build status](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/release.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/pypi/dm/langchain-plantuml)](https://pypi.org/project/langchain-plantuml/)
 
-Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
+Subscribe to events using a callback and store them in PlantUML format **Activity Diagram** and **Sequence Diagram**. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 
-![](screenshot/scene_agent.png)
+Activity Diagram 
+
+![](screenshot/activity-diagram.png)
+
+Sequence Diagram
+
+![](screenshot/sequence-diagram.png)
 
 ## Quick Start
 
 Install this library:
 
 ```shell
 pip install langchain-plantuml
@@ -48,15 +54,15 @@
 1. Add import langchain_plantuml as the first import in your Python entrypoint file
 2. Create a callback using the activity_diagram_callback function
 3. Hook into your LLM application
 4. Call the export_uml_content method of activity_diagram_callback to export the PlantUML content
 5. Save PlantUML content to a file
 6. Exporting PlantUML to PNG
 
-Running the minimal example.
+Running the minimal activity diagram example.
 
 ```python
 from langchain import OpenAI, LLMChain, PromptTemplate
 from langchain.memory import ConversationBufferMemory
 
 from langchain_plantuml import diagram
 
@@ -80,23 +86,29 @@
     memory=memory,
     callbacks=[callback_handler]
 )
 
 llm_chain.predict(human_input="Hi there my friend")
 llm_chain.predict(human_input="Not too bad - how are you?")
 
-callback_handler.save_uml_content("example.puml")
+callback_handler.save_uml_content("example-activity.puml")
 ```
 
 You will get the following PlantUML activity diagram
 
-![](screenshot/example.png)
+![](screenshot/example-activity.png)
+
+Sequence Diagram
+
+```python
+callback_handler = diagram.sequence_diagram_callback()
+```
 
 ## Exporting PlantUML to PNG
 
 You can download [plantuml.1.2023.10.jar](https://github.com/plantuml/plantuml/releases/download/v1.2023.10/plantuml-1.2023.10.jar)
 
 ```shell
-java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example.puml
+java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example-activity.puml
 ```
```

