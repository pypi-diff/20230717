# Comparing `tmp/zshgpt-0.1.1.tar.gz` & `tmp/zshgpt-0.1.2.tar.gz`

## Comparing `zshgpt-0.1.1.tar` & `zshgpt-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/__main__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/cli/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 zshgpt-0.1.1/src/zshgpt/cli/messages.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.1.1/zsh_plugin/zsh_plugin.zsh
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 zshgpt-0.1.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 zshgpt-0.1.1/README.md
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 zshgpt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 zshgpt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.1.2/Peek 2023-07-17 17-27.gif
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/__main__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/cli/__init__.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/cli/messages.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.1.2/zsh_plugin/zsh_plugin.zsh
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 zshgpt-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 zshgpt-0.1.2/README.md
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 zshgpt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 zshgpt-0.1.2/PKG-INFO
```

### Comparing `zshgpt-0.1.1/src/zshgpt/cli/__init__.py` & `zshgpt-0.1.2/src/zshgpt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.1/zsh_plugin/zsh_plugin.zsh` & `zshgpt-0.1.2/zsh_plugin/zsh_plugin.zsh`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.1/.gitignore` & `zshgpt-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.1/LICENSE.txt` & `zshgpt-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.1/README.md` & `zshgpt-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 
 -----
 
 **Table of Contents**
 
 - [About](#about)
 - [Installation](#installation)
+- [Prerequisite](#prerequisite)
+- [Future plans](#future-plans)
 - [License](#license)
 
 ## About
+![Gif of usage](<Peek 2023-07-17 17-27.gif>)
+
 Heavily inspired by the abandoned project [https://github.com/microsoft/Codex-CLI](https://github.com/microsoft/Codex-CLI)
 Made into a oh-my-zsh plugin.
 
 In your zsh console, type a question, starting with comment sign `#`, hit `ctrl+g` and get an answer.
 ```bash
 # Who edited README.MD last according to git history?
 ```
@@ -30,31 +34,53 @@
 ```bash
 # Who was Norways first prime minister?
 # Norway's first prime minister was Frederik Stang, serving from 1873 to 1880.
 ``` 
 
 ## Prerequisite
 * Python >= 3.7
+* ZSH + Oh-my-zsh
 * Valid Openai API-key
     * make sure to save under `OPENAI_API_KEY` env.
     * `export OPENAI_API_KEY='sk-...'`
 
 ## Installation
 
+With zshgpt alone, you can ask questions with `zshgpt # Show me all my drives` and it will return an answer from GPT. But the true performance boost comes when you also add the zsh plugin.
 ```bash
-pip install zshgpt
+pip install zshgpt # Or preferably install with pipx
 mkdir $ZSH_CUSTOM/plugins/zshgpt
 curl https://raw.githubusercontent.com/AndersSteenNilsen/zshgpt/main/zsh_plugin/zsh_plugin.zsh -o $ZSH_CUSTOM/plugins/zshgpt/zshgpt.plugin.zsh
 ```
 Then add zshgpt in your list of plugins in `~/.zshrc`
 
 ```
 plugins(
     ...
     zshgpt
     ...
 )
 ```
 
+## Future plans
+
+### Functionaliy
+* Remember last couple messages so you could do something like:
+```bash
+# Open README.md <-- USER
+# You can open the README.md file using a text editor of your choice. Here's an example using vim:
+
+vim README.md
+# But I don't have vim, can you open it in VSCode? <-- USER
+code README.md
+```
+* Cycle through choices
+* Give possibility to switch model
+* Give info about how many token has been used
+
+### CI/CD
+* Pre-commit.
+* Add to flatpack or similar to ease installation.
+* Publish as part of git flow.
 ## License
 
 `zshgpt` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `zshgpt-0.1.1/pyproject.toml` & `zshgpt-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.1/PKG-INFO` & `zshgpt-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zshgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Level up z shell with GPT
 Project-URL: Documentation, https://github.com/unknown/zshgpt#readme
 Project-URL: Issues, https://github.com/unknown/zshgpt/issues
 Project-URL: Source, https://github.com/unknown/zshgpt
 Author-email: Anders Steen <anders.steen@knowit.no>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -29,17 +29,21 @@
 
 -----
 
 **Table of Contents**
 
 - [About](#about)
 - [Installation](#installation)
+- [Prerequisite](#prerequisite)
+- [Future plans](#future-plans)
 - [License](#license)
 
 ## About
+![Gif of usage](<Peek 2023-07-17 17-27.gif>)
+
 Heavily inspired by the abandoned project [https://github.com/microsoft/Codex-CLI](https://github.com/microsoft/Codex-CLI)
 Made into a oh-my-zsh plugin.
 
 In your zsh console, type a question, starting with comment sign `#`, hit `ctrl+g` and get an answer.
 ```bash
 # Who edited README.MD last according to git history?
 ```
@@ -54,31 +58,53 @@
 ```bash
 # Who was Norways first prime minister?
 # Norway's first prime minister was Frederik Stang, serving from 1873 to 1880.
 ``` 
 
 ## Prerequisite
 * Python >= 3.7
+* ZSH + Oh-my-zsh
 * Valid Openai API-key
     * make sure to save under `OPENAI_API_KEY` env.
     * `export OPENAI_API_KEY='sk-...'`
 
 ## Installation
 
+With zshgpt alone, you can ask questions with `zshgpt # Show me all my drives` and it will return an answer from GPT. But the true performance boost comes when you also add the zsh plugin.
 ```bash
-pip install zshgpt
+pip install zshgpt # Or preferably install with pipx
 mkdir $ZSH_CUSTOM/plugins/zshgpt
 curl https://raw.githubusercontent.com/AndersSteenNilsen/zshgpt/main/zsh_plugin/zsh_plugin.zsh -o $ZSH_CUSTOM/plugins/zshgpt/zshgpt.plugin.zsh
 ```
 Then add zshgpt in your list of plugins in `~/.zshrc`
 
 ```
 plugins(
     ...
     zshgpt
     ...
 )
 ```
 
+## Future plans
+
+### Functionaliy
+* Remember last couple messages so you could do something like:
+```bash
+# Open README.md <-- USER
+# You can open the README.md file using a text editor of your choice. Here's an example using vim:
+
+vim README.md
+# But I don't have vim, can you open it in VSCode? <-- USER
+code README.md
+```
+* Cycle through choices
+* Give possibility to switch model
+* Give info about how many token has been used
+
+### CI/CD
+* Pre-commit.
+* Add to flatpack or similar to ease installation.
+* Publish as part of git flow.
 ## License
 
 `zshgpt` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

