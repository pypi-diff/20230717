# Comparing `tmp/omgpt-0.0.7.tar.gz` & `tmp/omgpt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgpt-0.0.7.tar", max compression
+gzip compressed data, was "omgpt-0.0.8.tar", max compression
```

## Comparing `omgpt-0.0.7.tar` & `omgpt-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.7/LICENSE
--rw-r--r--   0        0        0    10570 2023-07-15 03:56:51.367413 omgpt-0.0.7/README.md
--rw-r--r--   0        0        0     2994 2023-07-15 04:09:41.068538 omgpt-0.0.7/omgpt/__init__.py
--rw-r--r--   0        0        0     2009 2023-07-15 02:06:06.594390 omgpt-0.0.7/omgpt/shtool.py
--rw-r--r--   0        0        0      677 2023-07-15 06:31:08.944043 omgpt-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    11272 1970-01-01 00:00:00.000000 omgpt-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.8/LICENSE
+-rw-r--r--   0        0        0    11143 2023-07-17 07:00:20.176648 omgpt-0.0.8/README.md
+-rw-r--r--   0        0        0     3694 2023-07-17 06:46:40.734189 omgpt-0.0.8/omgpt/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-15 02:06:06.594390 omgpt-0.0.8/omgpt/shtool.py
+-rw-r--r--   0        0        0      677 2023-07-17 07:02:34.895272 omgpt-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    11845 1970-01-01 00:00:00.000000 omgpt-0.0.8/PKG-INFO
```

### Comparing `omgpt-0.0.7/LICENSE` & `omgpt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.7/README.md` & `omgpt-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 
 3. **Command History**: OMGpt Shell keeps track of the commands you've used, allowing you to easily revisit and reuse them. This feature enhances efficiency and allows for easy repetition of commands.
 
 4. **Directory Navigation**: Easily navigate through your file system with simple commands. OMGpt Shell understands your directory change commands, making file system navigation a breeze.
 
 5. **Streaming Responses**: Get real-time feedback from OMGpt Shell. As GPT processes your commands, the responses are streamed back to you, keeping you informed every step of the way.
 
-6. **Examples of use**:
+6. **Non-Interactive Mode**: OMGpt Shell supports a non-interactive mode, allowing you to use it in scripts or batch jobs, or to execute a single command without entering the interactive shell environment.
+
+7. **Examples of use**:
 
    - **Example 1**: When you say, "Download the file at 'http://example.com/file' and save it as 'downloaded_file'", OMGpt Shell will execute the following:
      ```bash
      wget -O downloaded_file http://example.com/file
      ```
    - **Example 2**: If you tell OMGpt Shell to "Find all the Python files in the current directory", it will execute:
      ```bash
@@ -92,23 +94,31 @@
 
    or
 
    ```bash
    > Check the current status of git, track and commit the newly written source code with a nice commit message
    ```
 
+4. To use non-interactive mode, pass your command as an argument when starting OMGpt Shell. For example:
+
+   ```bash
+   omgpt -c "Download the file at 'http://example.com/file' and save it as 'downloaded_file'"
+   ```
+
+   This will start OMGpt Shell, execute the given command, and then exit. The output will be the same as if you had entered the command in interactive mode.
+
 Remember, the goal of OMGpt Shell is to understand your commands in your preferred language and convert them to appropriate shell commands.
 
 ## 🔧 Configuration
 
-To customize your user experience with OMGpt, you need to create a configuration file named `config.ini` in the root directory of your project.
+To customize your user experience with OMGpt, you need to create a configuration file named `~/.omgptrc` in your home directory.
 
-Here's a simple example of what your `config.ini` might look like:
+Here's a simple example of what your `~/.omgptrc` might look like:
 
-```
+```ini
 [api]
 openai_api_key = <your-openai-api-key>
 
 [settings]
 chat_model = gpt-4-0613
 ```
 
@@ -118,21 +128,21 @@
 
 - `openai_api_key`: You are required to input your OpenAI API key. This allows OMGpt to communicate with the OpenAI API. You can get your OpenAI API key from the [OpenAI website](https://openai.com).
 
 ### Optional Settings
 
 These optional settings customize OMGpt to better suit your needs:
 
-- `chat_model`: Specifies the chat model that OMGpt will use. This includes "gpt-4-0613" and "gpt-3.5-turbo-0613", among others. If it's not specified, a default model will be used. ou should verify the availability of these models in your API subscription.
+- `chat_model`: Specifies the chat model that OMGpt will use. This includes "gpt-4-0613" and "gpt-3.5-turbo-0613", among others. If it's not specified, a default model will be used. You should verify the availability of these models in your API subscription.
 
 - `system_prompt`: Sets the behavior of the model used. The prompt should instruct the model about its function and how to generate responses. For instance, "You are a shell. Your name is OMGpt. You treat their time as precious. You are as concise as possible in responses. You need to run the next command sequentially, depending on the result of the previous command, without prompting the user if necessary. You should run a command to get information about system. Use friendly, appropriate emoticons when responding to users."
 
 - `temperature`: Controls the diversity of the model's responses. A higher value (nearer to 1) produces more various outputs, while a lower value creates more deterministic responses.
 
-After modifying your `config.ini`, don't forget to save it and restart OMGpt for the changes to apply. More details about the models and their behaviors can be found in the [official OpenAI API documentation](https://docs.openai.com/en/).
+After modifying your `~/.omgptrc`, don't forget to save it and restart OMGpt for the changes to apply. More details about the models and their behaviors can be found in the [official OpenAI API documentation](https://docs.openai.com/en/).
 
 ## 💡 Contributing
 
 We welcome contributions to OMGpt Shell! Whether it's reporting bugs, suggesting new features, improving documentation, or contributing code, your help is greatly appreciated.
 
 Here are some ways you can contribute:
```

### Comparing `omgpt-0.0.7/omgpt/__init__.py` & `omgpt-0.0.8/omgpt/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,15 +22,24 @@
     },
 }
 
 
 def load_config(config_file: str) -> configparser.ConfigParser:
     config = configparser.ConfigParser()
     config.read_dict(DEFAULT_CONFIG)
-    config.read(config_file)
+    if os.path.exists(config_file):
+        config.read(config_file)
+    else:
+        raise FileNotFoundError(
+            f"Configuration file '{config_file}' not found. Please create one."
+        )
+    if not config.has_section("api") or not config.has_option("api", "openai_api_key"):
+        raise ValueError(
+            "Missing required 'openai_api_key' in 'api' section in the configuration file."
+        )
     return config
 
 
 def init_agent_with_tools(tools, config, verbose):
     system_prompt = SystemMessage(content=config.get("settings", "system_prompt"))
     agent_kwargs = {
         "extra_prompt_messages": [MessagesPlaceholder(variable_name="memory")],
@@ -52,32 +61,38 @@
         verbose=verbose,
         agent_kwargs=agent_kwargs,
         memory=memory,
     )
     return agent
 
 
-def run(agent):
+def run_interactive(agent):
     home = os.path.expanduser("~")
     history = FileHistory(os.path.join(home, ".omgpt_history"))
     session = PromptSession(history=history)
 
     while True:
         user_input = session.prompt("> ")
         response_message = agent.run(user_input)
         print()
 
+def run_noninteractive(agent, command):
+    response_message = agent.run(command)
+    print()
+
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-v", "--verbose", action="store_true", help="Increase output verbosity"
     )
     parser.add_argument(
-        "-c",
+        "-c", "--command", help="Run a single command in non-interactive mode"
+    )
+    parser.add_argument(
         "--config",
         default=os.path.expanduser("~/.omgptrc"),
         help="Path to the config file",
     )
     args = parser.parse_args()
 
     config = load_config(args.config)
@@ -88,12 +103,16 @@
                 name="sh",
                 description="Useful when you need to run a shell command and get standard output and errors.",
                 args_schema=ShellToolSchema,
                 handle_tool_error=True,
             )
         ]
         agent = init_agent_with_tools(tools, config, verbose=args.verbose)
-        run(agent)
+
+        if args.command:
+            run_noninteractive(agent, args.command)
+        else:
+            run_interactive(agent)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `omgpt-0.0.7/omgpt/shtool.py` & `omgpt-0.0.8/omgpt/shtool.py`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.7/pyproject.toml` & `omgpt-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omgpt"
-version = "0.0.7"
+version = "0.0.8"
 description = "Simplify and enhance your command-line experience with the power of AI"
 authors = ["Youngwook Kim <youngwook.kim@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ywkim/omgpt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `omgpt-0.0.7/PKG-INFO` & `omgpt-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omgpt
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simplify and enhance your command-line experience with the power of AI
 Home-page: https://github.com/ywkim/omgpt
 License: MIT
 Author: Youngwook Kim
 Author-email: youngwook.kim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -54,15 +54,17 @@
 
 3. **Command History**: OMGpt Shell keeps track of the commands you've used, allowing you to easily revisit and reuse them. This feature enhances efficiency and allows for easy repetition of commands.
 
 4. **Directory Navigation**: Easily navigate through your file system with simple commands. OMGpt Shell understands your directory change commands, making file system navigation a breeze.
 
 5. **Streaming Responses**: Get real-time feedback from OMGpt Shell. As GPT processes your commands, the responses are streamed back to you, keeping you informed every step of the way.
 
-6. **Examples of use**:
+6. **Non-Interactive Mode**: OMGpt Shell supports a non-interactive mode, allowing you to use it in scripts or batch jobs, or to execute a single command without entering the interactive shell environment.
+
+7. **Examples of use**:
 
    - **Example 1**: When you say, "Download the file at 'http://example.com/file' and save it as 'downloaded_file'", OMGpt Shell will execute the following:
      ```bash
      wget -O downloaded_file http://example.com/file
      ```
    - **Example 2**: If you tell OMGpt Shell to "Find all the Python files in the current directory", it will execute:
      ```bash
@@ -111,23 +113,31 @@
 
    or
 
    ```bash
    > Check the current status of git, track and commit the newly written source code with a nice commit message
    ```
 
+4. To use non-interactive mode, pass your command as an argument when starting OMGpt Shell. For example:
+
+   ```bash
+   omgpt -c "Download the file at 'http://example.com/file' and save it as 'downloaded_file'"
+   ```
+
+   This will start OMGpt Shell, execute the given command, and then exit. The output will be the same as if you had entered the command in interactive mode.
+
 Remember, the goal of OMGpt Shell is to understand your commands in your preferred language and convert them to appropriate shell commands.
 
 ## 🔧 Configuration
 
-To customize your user experience with OMGpt, you need to create a configuration file named `config.ini` in the root directory of your project.
+To customize your user experience with OMGpt, you need to create a configuration file named `~/.omgptrc` in your home directory.
 
-Here's a simple example of what your `config.ini` might look like:
+Here's a simple example of what your `~/.omgptrc` might look like:
 
-```
+```ini
 [api]
 openai_api_key = <your-openai-api-key>
 
 [settings]
 chat_model = gpt-4-0613
 ```
 
@@ -137,21 +147,21 @@
 
 - `openai_api_key`: You are required to input your OpenAI API key. This allows OMGpt to communicate with the OpenAI API. You can get your OpenAI API key from the [OpenAI website](https://openai.com).
 
 ### Optional Settings
 
 These optional settings customize OMGpt to better suit your needs:
 
-- `chat_model`: Specifies the chat model that OMGpt will use. This includes "gpt-4-0613" and "gpt-3.5-turbo-0613", among others. If it's not specified, a default model will be used. ou should verify the availability of these models in your API subscription.
+- `chat_model`: Specifies the chat model that OMGpt will use. This includes "gpt-4-0613" and "gpt-3.5-turbo-0613", among others. If it's not specified, a default model will be used. You should verify the availability of these models in your API subscription.
 
 - `system_prompt`: Sets the behavior of the model used. The prompt should instruct the model about its function and how to generate responses. For instance, "You are a shell. Your name is OMGpt. You treat their time as precious. You are as concise as possible in responses. You need to run the next command sequentially, depending on the result of the previous command, without prompting the user if necessary. You should run a command to get information about system. Use friendly, appropriate emoticons when responding to users."
 
 - `temperature`: Controls the diversity of the model's responses. A higher value (nearer to 1) produces more various outputs, while a lower value creates more deterministic responses.
 
-After modifying your `config.ini`, don't forget to save it and restart OMGpt for the changes to apply. More details about the models and their behaviors can be found in the [official OpenAI API documentation](https://docs.openai.com/en/).
+After modifying your `~/.omgptrc`, don't forget to save it and restart OMGpt for the changes to apply. More details about the models and their behaviors can be found in the [official OpenAI API documentation](https://docs.openai.com/en/).
 
 ## 💡 Contributing
 
 We welcome contributions to OMGpt Shell! Whether it's reporting bugs, suggesting new features, improving documentation, or contributing code, your help is greatly appreciated.
 
 Here are some ways you can contribute:
```

