# Comparing `tmp/lemonai-0.1.1.tar.gz` & `tmp/lemonai-0.1.2.tar.gz`

## Comparing `lemonai-0.1.1.tar` & `lemonai-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.1.1/heatmap-example.gif
--rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.1.1/heatmap-example.png
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lemonai-0.1.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 lemonai-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 lemonai-0.1.1/docs/tools.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/__init__.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.1.1/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.1.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lemonai-0.1.1/LICENSE
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 lemonai-0.1.1/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 lemonai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.1.2/heatmap-example.gif
+-rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.1.2/heatmap-example.png
+-rw-r--r--   0        0        0    71395 2020-02-02 00:00:00.000000 lemonai-0.1.2/random.txt
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 lemonai-0.1.2/test.py
+-rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 lemonai-0.1.2/testrandom.py
+-rw-r--r--   0        0        0    58482 2020-02-02 00:00:00.000000 lemonai-0.1.2/use-case-example.png
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lemonai-0.1.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 lemonai-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lemonai-0.1.2/.vscode/launch.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lemonai-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 lemonai-0.1.2/docs/tools.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.1.2/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lemonai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 lemonai-0.1.2/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 lemonai-0.1.2/PKG-INFO
```

### Comparing `lemonai-0.1.1/heatmap-example.gif` & `lemonai-0.1.2/heatmap-example.gif`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.1/heatmap-example.png` & `lemonai-0.1.2/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.1/docs/tools.md` & `lemonai-0.1.2/docs/tools.md`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.1/src/lemonai/execute_workflow.py` & `lemonai-0.1.2/src/lemonai/execute_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from lemonai.get_integrations import get_apis_from_env
 from lemonai.api_wrapper import APIWrapper
 from lemonai.toolkit import Toolkit
 from lemonai.filter_tools import filter_tools
 from typing import Optional
 
 
-def execute_workflow(llm: BaseLLM, prompt_string: str, api_domain: Optional[str] = None):
+def execute_workflow(llm: BaseLLM, prompt_string: str, server_domain: Optional[str] = None):
 
     logfile_path = "lemonai.log"
     logger.remove(handler_id=None)
     logger.add(logfile_path, format="{time} - {extra[session_id]} - {extra[operation_name]}")
 
     api_keys_dict, access_tokens_dict = get_apis_from_env()
     session_id = uuid.uuid4()
 
-    _wrapper = APIWrapper(api_domain)
+    _wrapper = APIWrapper(llm, task=prompt_string, api_domain=server_domain)
     toolkit = Toolkit.from_api_wrapper(_wrapper, api_keys_dict, access_tokens_dict, logger, str(session_id))
     tools = toolkit.get_tools()
 
-    prompt = f"Your task is '{prompt_string}'. Focus on the ordering of the tasks given. Do not use a workflow unless it is mentioned. Give your action input as a valid JSON object where the keys are the params and the values are the value for each input parameter. The description of the tool may provide the JSON structure of the action input using round brackets () instead of curly brackets. Follow this structure for your action input. Your final answer should give a brief conversational overview of what you did."    
+    prompt = f"Your task is '{prompt_string}'. Focus on the ordering of the tasks given. Do not use a workflow unless it is mentioned. Your action input should be a valid JSON object where the keys are the params and the values are the value for each input parameter. The description of the tool may provide the JSON structure of the action input using round brackets () instead of curly brackets. Follow this structure for your action input. Ensure all strings in the action input are valid and terminated correctly. Your final answer should give a brief conversational overview of what you did."    
     filtered_tools = filter_tools(llm=llm, task=prompt_string, tools=tools)
     
     agent = initialize_agent(
         tools=filtered_tools,
         llm=llm,
         agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION,
         verbose=True
```

### Comparing `lemonai-0.1.1/src/lemonai/filter_tools.py` & `lemonai-0.1.2/src/lemonai/filter_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from langchain.llms.base import BaseLLM 
 from lemonai.tool import Tool
 from typing import List
 
 def filter_tools(llm: BaseLLM, task: str, tools: List[Tool]) -> List[Tool]:
 
     tool_names = [tool.name for tool in tools]
-    prompt = f"Given the following list of tools: {tool_names}, return a list of possible tools to be used to complete the following task: '{task}'. If the task mentions any workflow, you MUST include this workflow in your final answer. You should split the task into subtasks and for each subtask, think about the possible tools that could be used to complete each subtask. Pay attention to tool names mentioned and verbs that are used (and their synonyms). Return as a single list which tools could be used to complete this task."
+    prompt = f"Given the following list of tools: {tool_names}, return a list of possible tools to be used to complete the following task: '{task}'. Consider only the tools given in the list. If the task mentions any workflow, you MUST include this workflow in your final answer. The only time you should suggest a workflow in your answer is if it explicitly stated in the task. You should split the task into subtasks and for each subtask, think about the possible tools that could be used to complete each subtask. Pay attention to tool names mentioned and verbs that are used (and their synonyms). Your answer should be a single valid list of the names of the tools that can be used to complete the given task."
 
     answer = llm.generate(prompts=[prompt]).generations[0][0].text
     list_string = answer.strip()
 
     filtered_tool_names = eval(list_string)
 
     filtered_tools = list(filter(lambda x: x.name in filtered_tool_names, tools))
```

### Comparing `lemonai-0.1.1/src/lemonai/get_integrations.py` & `lemonai-0.1.2/src/lemonai/get_integrations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Dict, Tuple
 
 def get_apis_from_env() -> Tuple[Dict[str, str], Dict[str, str]]:
 
     api_key_search_strings = ['_API_KEY', '_SECRET_KEY', '_SUBSCRIPTION_KEY', '_ACCESS_KEY']
-    access_token_search_strings = ['_ACCESS_TOKEN', '_SECRET_TOKEN', '_WEBHOOK_URL']
+    access_token_search_strings = ['_ACCESS_TOKEN', '_SECRET_TOKEN', '_WEBHOOK_URL', '_API_TOKEN']
 
     api_keys = {}
     access_tokens = {}
 
     for key, value in os.environ.items():
         for search_string in api_key_search_strings:
             if search_string in key:
```

### Comparing `lemonai-0.1.1/src/lemonai/tool.py` & `lemonai-0.1.2/src/lemonai/tool.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.1/src/lemonai/toolkit.py` & `lemonai-0.1.2/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.1/.gitignore` & `lemonai-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.1/LICENSE` & `lemonai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.1/README.md` & `lemonai-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <div align="center">
   <h1>🍋 Lemon AI</h1>
   <h3>Gateway to empower LLM agents to interact with the world</h3>
   <a href="https://discord.gg/bsgzjEpw">
 <img alt="Discord" src="https://img.shields.io/badge/Join Discord-x?style=flat&logo=discord&logoColor=white&label&labelColor=gray&color=5865F2">
   </a>
   <a href="https://twitter.com/getlemonai">
-    <img alt="Twitter" src="https://img.shields.io/badge/Follow Twitter-x?style=flat&logo=twitter&logoColor=white&label&labelColor=gray&color=1DA1F2">
+    <img alt="Twitter" src="https://img.shields.io/badge/Tweet at us-x?style=flat&logo=twitter&logoColor=white&label&labelColor=gray&color=1DA1F2">
   </a>
   <a href="https://github.com/trpc/trpc/blob/main/LICENSE">
-    <img alt="MIT License" src="https://img.shields.io/github/license/felixbrock/lemonai-py-client?labelColor=gray&color=yellow" />
+    <img alt="MIT License" src="https://img.shields.io/github/license/felixbrock/lemonai?labelColor=gray&color=yellow" />
   </a>
   <br />
-    <a href="">
+    <a href="https://python.langchain.com/docs/modules/agents/tools/integrations/lemonai">
     <img alt="Run Notebook in LangChain Docs" src="https://img.shields.io/badge/Run Notebook From LangChain Docs-x?style=for-the-badge&logoColor=white&label&labelColor=gray&color=gray">
   </a>
   <br />
   <br />
   <figure>
     <img src="heatmap-example.gif" alt="Demo" />
   </figure>
@@ -33,15 +33,15 @@
 
 Requires Python 3.8.1 and above.
 
 ### 2. Installing
 
 To use Lemon AI in your Python project run `pip install lemonai`. The following example uses an OpenAI model. Therefore, we also need to `pip install openai`. Depending on which model you want to use this install is optional.
 
-### 3. (Optional) Launch the Server
+### 3. (Optional) Launch the server
 
 The interaction of your agents and all Lemon AI tools is provided by the [Lemon AI Server](https://github.com/felixbrock/lemonai-server). Per default the Lemon AI Python client is sending requests to a hosted server version. To run the Lemon AI server on-prem please refer to the [Server Documentation](https://github.com/felixbrock/lemonai-server).
 
 ### 4. Use Lemon AI with LangChain
 
 The easiest way to give Lemon AI a try is via the Jupyter Notebook you can find in the [LangChain Docs](https://python.langchain.com/docs/modules/agents/tools/integrations/lemonai).
 
@@ -51,67 +51,73 @@
 
 ```Python
 import os
 from lemonai import execute_workflow
 from langchain import OpenAI
 ```
 
-#### Load API Keys and Access Tokens
+#### Load API keys and access tokens
 
 To use tools that require authentication, you have to store the corresponding access credentials in your environment in the format "{tool name}\_{authentication string}" where the authentication string is one of ["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN".
 
 ```Python
 """ Load all relevant API Keys and Access Tokens into your environment variables """
 os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*"
-os.environ["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*"
+os.environ["GITHUB_API_KEY"] = "*INSERT GITHUB API KEY HERE*"
+os.environ["DISCORD_WEBHOOK_URL"] = "*INSERT DISCORD CHANNEL WEBHOOK URL HERE*"
 ```
 
-#### Define your prompt and execute the LangChain Agent
+#### Example of defining your prompt and executing the Langchain Agent
+
+The following example makes use of several Lemon AI tools to
+
+1. Retrieve details about a personal repository on GitHub
+2. Get the top growing starred repositories of my account
+3. Send a Discord message with results and review.
+
+![Use Case Example](use-case-example.png)
 
 ```Python
-hackernews_username = "*INSERT HACKERNEWS USERNAME HERE*"
-"""
-Guidelines on identifying Airtable ids here:
-https://www.highviewapps.com/kb/where-can-i-find-the-airtable-base-id-and-table-id/
-"""
-airtable_base_id = "*INSERT BASE ID HERE*"
-airtable_table_id = "*INSERT TABLE ID HERE*"
+lemonai_repo_owner = "Abdus2609"
+github_username = "Abdus2609"
 
 """ Define your instruction to be given to your LLM """
-prompt = f"""Read information from Hackernews for user {hackernews_username} and then write the results to
-Airtable (baseId: {airtable_base_id}, tableId: {airtable_table_id}). Only write the fields "username", "karma"
-and "created_at_i". Please make sure that Airtable does NOT automatically convert the field types.
-"""
+prompt = f"""Get the description for a repository I am working with called lemonai (owner {lemonai_repo_owner}).
+Also, get my top growing starred repositories (username {github_username}). Analyze the descriptions of both
+the LemonAI repository and my top-starred repositories. Then, send a Discord message that first displays a
+numerically bullet-pointed leaderboard of the top growing starred repositories and their growth, and secondly
+discuss how each tool could be useful specifically to lemonai's use case based on your analysis of the
+descriptions of each repository."""
 
 """
 Use the Lemon AI execute_workflow wrapper
 to run your LangChain agent in combination with Lemon AI
 """
 model = OpenAI(temperature=0)
 
 execute_workflow(llm=model, prompt_string=prompt)
 ```
 
 #### (Optional) Define your Lemon AI Functions
 
-Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-other-api-updates), Lemon AI provides the option to define workflows as reusable functions. These functions can be defined for use cases where it is especially important to move as close as possible to near-deterministic behavior. Specific workflows can be defined in a separate lemonai.json. You can find the corresponding tool ids (e.g. `hackernews-get-user`) in the [Tool Docs](https://github.com/felixbrock/lemonai-py-client/blob/main/docs/tools.md):
+Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-other-api-updates), Lemon AI provides the option to define workflows as reusable functions. These functions can be defined for use cases where it is especially important to move as close as possible to near-deterministic behavior. Specific workflows can be defined in a separate lemonai.json. You can find the corresponding tool ids (e.g. `hackernews-get-user`) in the [Tool Docs](https://github.com/felixbrock/lemonai/blob/main/docs/tools.md):
 
 ```json
 [
   {
     "name": "Hackernews Airtable User Workflow",
     "description": "retrieves user data from Hackernews and appends it to a table in Airtable",
     "tools": ["hackernews-get-user", "airtable-append-data"]
   }
 ]
 ```
 
 Your model will have access to these functions and will prefer them over self-selecting tools to solve a given task. All you have to do is to let the agent know that it should use a given function by including the function name in the prompt (e.g. `prompt = f"""Execute the Hackernews Airtable user workflow...`).
 
-### 4. Gain transparency on your Agent's decision making
+### 5. Gain transparency on your Agent's decision making
 
 To gain transparency on how your Agent interacts with Lemon AI tools to solve a given task, all decisions made, tools used and operations performed are written to a local `lemonai.log` file. Every time your LLM agent is interacting with the Lemon AI tool stack a corresponding log entry is created:
 
 ```log
 2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - hackernews-get-user
 2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - airtable-append-data
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - hackernews-get-user
@@ -120,15 +126,15 @@
 
 By using the [Lemon AI Analytics Tool](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which order tools are used. As a result, you can identify weak spots in your agent’s decision-making capabilities and move to a more deterministic behavior by defining Lemon AI functions.
 
 ![Heatmap Example](heatmap-example.png)
 
 ## 🧩 Supported Tools
 
-We already allow agents to interact with over [120 tools](https://github.com/felixbrock/lemonai-py-client/blob/main/docs/tools.md) across the following services:
+We already allow agents to interact with over [120 tools](https://github.com/felixbrock/lemonai/blob/main/docs/tools.md) across the following services:
 
 - HackerNews
 - Airtable
 - Slack
 - HubSpot
 - Github
 - Notion
@@ -147,32 +153,23 @@
 - [ ] Stripe
 - [ ] Medium
 - [ ] Google Cloud Realtime Database
 - [ ] Salesforce
 
 ## 🦸 Contributing
 
-Great to see you here! We are extremely open to contributions! You can find more information in our [CONTRIBUTING.md](https://github.com/felixbrock/lemonai-py-client/blob/main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop us a message on <a href="https://discord.gg/bsgzjEpw">Discord</a>.
+Great to see you here! We are extremely open to contributions! You can find more information in our [CONTRIBUTING.md](https://github.com/felixbrock/lemonai/blob/main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop us a message on <a href="https://discord.gg/bsgzjEpw">Discord</a>.
 
-## ❤️‍🔥 Team
+## ❤️‍🔥 Contributors
 
-<table cellspacing="0" cellpadding="0" style="border:none;">
-  <tr style="border:none;">
-    <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" style="border-radius: 50%;" width="100px;" alt=""/><br /><sub><b>Felix</b></sub></a></td>
-    <td style="border:none;">Hey there 🥳 I am Felix, the creator of Lemon AI. Always happy to chat and answer any questions you might have! So feel free to reachout on <a href="https://twitter.com/felixbrockm">Twitter</a> or <a href="mailto:fe.brockmeier@gmail.com">Email</a> </td>
-  </tr>
-</table>
-
-### Active Contributors
-
-> Team members and people who actively help out improving the codebase by making PRs and reviewing code.
+> Those are the team members and people who actively help out improving the codebase by making PRs and reviewing code. We are beyond grateful for your help!
 
 <table cellspacing="0" cellpadding="0" style="border:none;">
   <tbody>
     <tr style="border:none;">
+      <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Felix Brockmeier</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/mohammed-abdus-samad-hannan-3a2687202/"><img src="https://avatars.githubusercontent.com/u/72310364?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Mohammed Hannan</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/haiphunghiem/"><img src="https://avatars.githubusercontent.com/u/16231195?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Hai Nghiem</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://twitter.com/schroeerclemens"><img src="https://avatars.githubusercontent.com/u/84038864?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Clemens Schroeer</b></sub></a></td>
-      <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Felix Brockmeier</b></sub></a></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                           ****** ð Lemon AI ******
       **** Gateway to empower LLM agents to interact with the world ****
                       [Discord] [Twitter] [MIT_License]
-                       [Run Notebook in LangChain Docs]
+                       [Run_Notebook_in_LangChain_Docs]
 
                                     [Demo]
 **Lemon AI helps you build powerful AI assistants in minutes and automate
 workflows by allowing for accurate and reliable read and write operations in
 [tools](#ð§©-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack
 and Github.** Most connectors available today are focused on read-only
 operations, limiting the potential of LLMs. Agents, on the other hand, have a
@@ -14,89 +14,91 @@
 defined APIs for reliable read and write operations. In addition, Lemon AI
 functions allow you to further reduce the risk of hallucinations by providing a
 way to statically define workflows that the model can rely on in case of
 uncertainty. ## â¡ï¸ Getting Started ### 1. Prerequisites Requires Python
 3.8.1 and above. ### 2. Installing To use Lemon AI in your Python project run
 `pip install lemonai`. The following example uses an OpenAI model. Therefore,
 we also need to `pip install openai`. Depending on which model you want to use
-this install is optional. ### 3. (Optional) Launch the Server The interaction
+this install is optional. ### 3. (Optional) Launch the server The interaction
 of your agents and all Lemon AI tools is provided by the [Lemon AI Server]
 (https://github.com/felixbrock/lemonai-server). Per default the Lemon AI Python
 client is sending requests to a hosted server version. To run the Lemon AI
 server on-prem please refer to the [Server Documentation](https://github.com/
 felixbrock/lemonai-server). ### 4. Use Lemon AI with LangChain The easiest way
 to give Lemon AI a try is via the Jupyter Notebook you can find in the
 [LangChain Docs](https://python.langchain.com/docs/modules/agents/tools/
 integrations/lemonai). Lemon AI automatically solves given tasks by finding the
 right combination of relevant tools or uses Lemon AI Functions as an
 alternative. The following example demonstrates how to retrieve a user from
 Hackernews and write it to a table in Airtable: #### Include Lemon AI in your
 LangChain project ```Python import os from lemonai import execute_workflow from
-langchain import OpenAI ``` #### Load API Keys and Access Tokens To use tools
+langchain import OpenAI ``` #### Load API keys and access tokens To use tools
 that require authentication, you have to store the corresponding access
 credentials in your environment in the format "{tool name}\_{authentication
 string}" where the authentication string is one of ["API_KEY", "SECRET_KEY",
 "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN",
 "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY",
 "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN". ```Python """ Load all
 relevant API Keys and Access Tokens into your environment variables """
 os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*" os.environ
-["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*" ``` #### Define your
-prompt and execute the LangChain Agent ```Python hackernews_username = "*INSERT
-HACKERNEWS USERNAME HERE*" """ Guidelines on identifying Airtable ids here:
-https://www.highviewapps.com/kb/where-can-i-find-the-airtable-base-id-and-
-table-id/ """ airtable_base_id = "*INSERT BASE ID HERE*" airtable_table_id =
-"*INSERT TABLE ID HERE*" """ Define your instruction to be given to your LLM
-""" prompt = f"""Read information from Hackernews for user
-{hackernews_username} and then write the results to Airtable (baseId:
-{airtable_base_id}, tableId: {airtable_table_id}). Only write the fields
-"username", "karma" and "created_at_i". Please make sure that Airtable does NOT
-automatically convert the field types. """ """ Use the Lemon AI
+["GITHUB_API_KEY"] = "*INSERT GITHUB API KEY HERE*" os.environ
+["DISCORD_WEBHOOK_URL"] = "*INSERT DISCORD CHANNEL WEBHOOK URL HERE*" ``` ####
+Example of defining your prompt and executing the Langchain Agent The following
+example makes use of several Lemon AI tools to 1. Retrieve details about a
+personal repository on GitHub 2. Get the top growing starred repositories of my
+account 3. Send a Discord message with results and review. ![Use Case Example]
+(use-case-example.png) ```Python lemonai_repo_owner = "Abdus2609"
+github_username = "Abdus2609" """ Define your instruction to be given to your
+LLM """ prompt = f"""Get the description for a repository I am working with
+called lemonai (owner {lemonai_repo_owner}). Also, get my top growing starred
+repositories (username {github_username}). Analyze the descriptions of both the
+LemonAI repository and my top-starred repositories. Then, send a Discord
+message that first displays a numerically bullet-pointed leaderboard of the top
+growing starred repositories and their growth, and secondly discuss how each
+tool could be useful specifically to lemonai's use case based on your analysis
+of the descriptions of each repository.""" """ Use the Lemon AI
 execute_workflow wrapper to run your LangChain agent in combination with Lemon
 AI """ model = OpenAI(temperature=0) execute_workflow(llm=model,
 prompt_string=prompt) ``` #### (Optional) Define your Lemon AI Functions
 Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-
 other-api-updates), Lemon AI provides the option to define workflows as
 reusable functions. These functions can be defined for use cases where it is
 especially important to move as close as possible to near-deterministic
 behavior. Specific workflows can be defined in a separate lemonai.json. You can
 find the corresponding tool ids (e.g. `hackernews-get-user`) in the [Tool Docs]
-(https://github.com/felixbrock/lemonai-py-client/blob/main/docs/tools.md):
-```json [ { "name": "Hackernews Airtable User Workflow", "description":
-"retrieves user data from Hackernews and appends it to a table in Airtable",
-"tools": ["hackernews-get-user", "airtable-append-data"] } ] ``` Your model
-will have access to these functions and will prefer them over self-selecting
-tools to solve a given task. All you have to do is to let the agent know that
-it should use a given function by including the function name in the prompt
-(e.g. `prompt = f"""Execute the Hackernews Airtable user workflow...`). ### 4.
-Gain transparency on your Agent's decision making To gain transparency on how
-your Agent interacts with Lemon AI tools to solve a given task, all decisions
-made, tools used and operations performed are written to a local `lemonai.log`
-file. Every time your LLM agent is interacting with the Lemon AI tool stack a
+(https://github.com/felixbrock/lemonai/blob/main/docs/tools.md): ```json [
+{ "name": "Hackernews Airtable User Workflow", "description": "retrieves user
+data from Hackernews and appends it to a table in Airtable", "tools":
+["hackernews-get-user", "airtable-append-data"] } ] ``` Your model will have
+access to these functions and will prefer them over self-selecting tools to
+solve a given task. All you have to do is to let the agent know that it should
+use a given function by including the function name in the prompt (e.g. `prompt
+= f"""Execute the Hackernews Airtable user workflow...`). ### 5. Gain
+transparency on your Agent's decision making To gain transparency on how your
+Agent interacts with Lemon AI tools to solve a given task, all decisions made,
+tools used and operations performed are written to a local `lemonai.log` file.
+Every time your LLM agent is interacting with the Lemon AI tool stack a
 corresponding log entry is created: ```log 2023-06-26T11:50:27.708785+0100 -
 b5f91c59-8487-45c2-800a-156eac0c7dae - hackernews-get-user 2023-06-26T11:50:
 39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - airtable-append-data
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d -
 hackernews-get-user 2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-
 55b50007ed9d - airtable-append-data ``` By using the [Lemon AI Analytics Tool]
 (https://github.com/felixbrock/lemonai-analytics) you can easily gain a better
 understanding of how frequently and in which order tools are used. As a result,
 you can identify weak spots in your agentâs decision-making capabilities and
 move to a more deterministic behavior by defining Lemon AI functions. ![Heatmap
 Example](heatmap-example.png) ## ð§© Supported Tools We already allow agents
-to interact with over [120 tools](https://github.com/felixbrock/lemonai-py-
-client/blob/main/docs/tools.md) across the following services: - HackerNews -
-Airtable - Slack - HubSpot - Github - Notion - Discord ## ð©» Next Up - [x]
-Github - [x] Notion - [x] Discord - [ ] Gmail - [ ] Google Calendar - [ ] Kafka
-- [ ] Pipedrive - [ ] Monday.com - [ ] Stripe - [ ] Medium - [ ] Google Cloud
+to interact with over [120 tools](https://github.com/felixbrock/lemonai/blob/
+main/docs/tools.md) across the following services: - HackerNews - Airtable -
+Slack - HubSpot - Github - Notion - Discord ## ð©» Next Up - [x] Github - [x]
+Notion - [x] Discord - [ ] Gmail - [ ] Google Calendar - [ ] Kafka - [ ]
+Pipedrive - [ ] Monday.com - [ ] Stripe - [ ] Medium - [ ] Google Cloud
 Realtime Database - [ ] Salesforce ## ð¦¸ Contributing Great to see you here!
 We are extremely open to contributions! You can find more information in our
-[CONTRIBUTING.md](https://github.com/felixbrock/lemonai-py-client/blob/
-main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop
-us a message on Discord. ## â¤ï¸âð¥ Team
-      Hey there ð¥³ I am Felix, the creator of Lemon AI. Always happy to chat and
-Felix answer any questions you might have! So feel free to reachout on Twitter or
-      Email
-### Active Contributors > Team members and people who actively help out
-improving the codebase by making PRs and reviewing code.
+[CONTRIBUTING.md](https://github.com/felixbrock/lemonai/blob/main/.github/
+CONTRIBUTING.md). If you have any more questions feel free to drop us a message
+on Discord. ## â¤ï¸âð¥ Contributors > Those are the team members and
+people who actively help out improving the codebase by making PRs and reviewing
+code. We are beyond grateful for your help!
 
-Mohammed_Hannan Hai_Nghiem Clemens_Schroeer Felix_Brockmeier
+Felix_Brockmeier Mohammed_Hannan Hai_Nghiem Clemens_Schroeer
```

### Comparing `lemonai-0.1.1/pyproject.toml` & `lemonai-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `lemonai-0.1.1/PKG-INFO` & `lemonai-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.
 Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/issues
 Author-email: Felix Brockmeier <fe.brockmeier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -17,21 +17,21 @@
 <div align="center">
   <h1>🍋 Lemon AI</h1>
   <h3>Gateway to empower LLM agents to interact with the world</h3>
   <a href="https://discord.gg/bsgzjEpw">
 <img alt="Discord" src="https://img.shields.io/badge/Join Discord-x?style=flat&logo=discord&logoColor=white&label&labelColor=gray&color=5865F2">
   </a>
   <a href="https://twitter.com/getlemonai">
-    <img alt="Twitter" src="https://img.shields.io/badge/Follow Twitter-x?style=flat&logo=twitter&logoColor=white&label&labelColor=gray&color=1DA1F2">
+    <img alt="Twitter" src="https://img.shields.io/badge/Tweet at us-x?style=flat&logo=twitter&logoColor=white&label&labelColor=gray&color=1DA1F2">
   </a>
   <a href="https://github.com/trpc/trpc/blob/main/LICENSE">
-    <img alt="MIT License" src="https://img.shields.io/github/license/felixbrock/lemonai-py-client?labelColor=gray&color=yellow" />
+    <img alt="MIT License" src="https://img.shields.io/github/license/felixbrock/lemonai?labelColor=gray&color=yellow" />
   </a>
   <br />
-    <a href="">
+    <a href="https://python.langchain.com/docs/modules/agents/tools/integrations/lemonai">
     <img alt="Run Notebook in LangChain Docs" src="https://img.shields.io/badge/Run Notebook From LangChain Docs-x?style=for-the-badge&logoColor=white&label&labelColor=gray&color=gray">
   </a>
   <br />
   <br />
   <figure>
     <img src="heatmap-example.gif" alt="Demo" />
   </figure>
@@ -49,15 +49,15 @@
 
 Requires Python 3.8.1 and above.
 
 ### 2. Installing
 
 To use Lemon AI in your Python project run `pip install lemonai`. The following example uses an OpenAI model. Therefore, we also need to `pip install openai`. Depending on which model you want to use this install is optional.
 
-### 3. (Optional) Launch the Server
+### 3. (Optional) Launch the server
 
 The interaction of your agents and all Lemon AI tools is provided by the [Lemon AI Server](https://github.com/felixbrock/lemonai-server). Per default the Lemon AI Python client is sending requests to a hosted server version. To run the Lemon AI server on-prem please refer to the [Server Documentation](https://github.com/felixbrock/lemonai-server).
 
 ### 4. Use Lemon AI with LangChain
 
 The easiest way to give Lemon AI a try is via the Jupyter Notebook you can find in the [LangChain Docs](https://python.langchain.com/docs/modules/agents/tools/integrations/lemonai).
 
@@ -67,67 +67,73 @@
 
 ```Python
 import os
 from lemonai import execute_workflow
 from langchain import OpenAI
 ```
 
-#### Load API Keys and Access Tokens
+#### Load API keys and access tokens
 
 To use tools that require authentication, you have to store the corresponding access credentials in your environment in the format "{tool name}\_{authentication string}" where the authentication string is one of ["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN".
 
 ```Python
 """ Load all relevant API Keys and Access Tokens into your environment variables """
 os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*"
-os.environ["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*"
+os.environ["GITHUB_API_KEY"] = "*INSERT GITHUB API KEY HERE*"
+os.environ["DISCORD_WEBHOOK_URL"] = "*INSERT DISCORD CHANNEL WEBHOOK URL HERE*"
 ```
 
-#### Define your prompt and execute the LangChain Agent
+#### Example of defining your prompt and executing the Langchain Agent
+
+The following example makes use of several Lemon AI tools to
+
+1. Retrieve details about a personal repository on GitHub
+2. Get the top growing starred repositories of my account
+3. Send a Discord message with results and review.
+
+![Use Case Example](use-case-example.png)
 
 ```Python
-hackernews_username = "*INSERT HACKERNEWS USERNAME HERE*"
-"""
-Guidelines on identifying Airtable ids here:
-https://www.highviewapps.com/kb/where-can-i-find-the-airtable-base-id-and-table-id/
-"""
-airtable_base_id = "*INSERT BASE ID HERE*"
-airtable_table_id = "*INSERT TABLE ID HERE*"
+lemonai_repo_owner = "Abdus2609"
+github_username = "Abdus2609"
 
 """ Define your instruction to be given to your LLM """
-prompt = f"""Read information from Hackernews for user {hackernews_username} and then write the results to
-Airtable (baseId: {airtable_base_id}, tableId: {airtable_table_id}). Only write the fields "username", "karma"
-and "created_at_i". Please make sure that Airtable does NOT automatically convert the field types.
-"""
+prompt = f"""Get the description for a repository I am working with called lemonai (owner {lemonai_repo_owner}).
+Also, get my top growing starred repositories (username {github_username}). Analyze the descriptions of both
+the LemonAI repository and my top-starred repositories. Then, send a Discord message that first displays a
+numerically bullet-pointed leaderboard of the top growing starred repositories and their growth, and secondly
+discuss how each tool could be useful specifically to lemonai's use case based on your analysis of the
+descriptions of each repository."""
 
 """
 Use the Lemon AI execute_workflow wrapper
 to run your LangChain agent in combination with Lemon AI
 """
 model = OpenAI(temperature=0)
 
 execute_workflow(llm=model, prompt_string=prompt)
 ```
 
 #### (Optional) Define your Lemon AI Functions
 
-Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-other-api-updates), Lemon AI provides the option to define workflows as reusable functions. These functions can be defined for use cases where it is especially important to move as close as possible to near-deterministic behavior. Specific workflows can be defined in a separate lemonai.json. You can find the corresponding tool ids (e.g. `hackernews-get-user`) in the [Tool Docs](https://github.com/felixbrock/lemonai-py-client/blob/main/docs/tools.md):
+Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-other-api-updates), Lemon AI provides the option to define workflows as reusable functions. These functions can be defined for use cases where it is especially important to move as close as possible to near-deterministic behavior. Specific workflows can be defined in a separate lemonai.json. You can find the corresponding tool ids (e.g. `hackernews-get-user`) in the [Tool Docs](https://github.com/felixbrock/lemonai/blob/main/docs/tools.md):
 
 ```json
 [
   {
     "name": "Hackernews Airtable User Workflow",
     "description": "retrieves user data from Hackernews and appends it to a table in Airtable",
     "tools": ["hackernews-get-user", "airtable-append-data"]
   }
 ]
 ```
 
 Your model will have access to these functions and will prefer them over self-selecting tools to solve a given task. All you have to do is to let the agent know that it should use a given function by including the function name in the prompt (e.g. `prompt = f"""Execute the Hackernews Airtable user workflow...`).
 
-### 4. Gain transparency on your Agent's decision making
+### 5. Gain transparency on your Agent's decision making
 
 To gain transparency on how your Agent interacts with Lemon AI tools to solve a given task, all decisions made, tools used and operations performed are written to a local `lemonai.log` file. Every time your LLM agent is interacting with the Lemon AI tool stack a corresponding log entry is created:
 
 ```log
 2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - hackernews-get-user
 2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - airtable-append-data
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - hackernews-get-user
@@ -136,15 +142,15 @@
 
 By using the [Lemon AI Analytics Tool](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which order tools are used. As a result, you can identify weak spots in your agent’s decision-making capabilities and move to a more deterministic behavior by defining Lemon AI functions.
 
 ![Heatmap Example](heatmap-example.png)
 
 ## 🧩 Supported Tools
 
-We already allow agents to interact with over [120 tools](https://github.com/felixbrock/lemonai-py-client/blob/main/docs/tools.md) across the following services:
+We already allow agents to interact with over [120 tools](https://github.com/felixbrock/lemonai/blob/main/docs/tools.md) across the following services:
 
 - HackerNews
 - Airtable
 - Slack
 - HubSpot
 - Github
 - Notion
@@ -163,32 +169,23 @@
 - [ ] Stripe
 - [ ] Medium
 - [ ] Google Cloud Realtime Database
 - [ ] Salesforce
 
 ## 🦸 Contributing
 
-Great to see you here! We are extremely open to contributions! You can find more information in our [CONTRIBUTING.md](https://github.com/felixbrock/lemonai-py-client/blob/main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop us a message on <a href="https://discord.gg/bsgzjEpw">Discord</a>.
+Great to see you here! We are extremely open to contributions! You can find more information in our [CONTRIBUTING.md](https://github.com/felixbrock/lemonai/blob/main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop us a message on <a href="https://discord.gg/bsgzjEpw">Discord</a>.
 
-## ❤️‍🔥 Team
+## ❤️‍🔥 Contributors
 
-<table cellspacing="0" cellpadding="0" style="border:none;">
-  <tr style="border:none;">
-    <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" style="border-radius: 50%;" width="100px;" alt=""/><br /><sub><b>Felix</b></sub></a></td>
-    <td style="border:none;">Hey there 🥳 I am Felix, the creator of Lemon AI. Always happy to chat and answer any questions you might have! So feel free to reachout on <a href="https://twitter.com/felixbrockm">Twitter</a> or <a href="mailto:fe.brockmeier@gmail.com">Email</a> </td>
-  </tr>
-</table>
-
-### Active Contributors
-
-> Team members and people who actively help out improving the codebase by making PRs and reviewing code.
+> Those are the team members and people who actively help out improving the codebase by making PRs and reviewing code. We are beyond grateful for your help!
 
 <table cellspacing="0" cellpadding="0" style="border:none;">
   <tbody>
     <tr style="border:none;">
+      <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Felix Brockmeier</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/mohammed-abdus-samad-hannan-3a2687202/"><img src="https://avatars.githubusercontent.com/u/72310364?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Mohammed Hannan</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/haiphunghiem/"><img src="https://avatars.githubusercontent.com/u/16231195?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Hai Nghiem</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://twitter.com/schroeerclemens"><img src="https://avatars.githubusercontent.com/u/84038864?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Clemens Schroeer</b></sub></a></td>
-      <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Felix Brockmeier</b></sub></a></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: lemonai Version: 0.1.1 Summary: Lemon AI's A Python
+Metadata-Version: 2.1 Name: lemonai Version: 0.1.2 Summary: Lemon AI's A Python
 client. Grant your LLM agents access to a wide range of APIs for read and write
 operations, creating copilots in minutes and unlocking the true potential of
 LLMs. Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/
 issues Author-email: Felix Brockmeier
 brockmeier@gmail.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8.1
 Requires-Dist: langchain Requires-Dist: loguru Description-Content-Type: text/
 markdown
                           ****** ð Lemon AI ******
       **** Gateway to empower LLM agents to interact with the world ****
                       [Discord] [Twitter] [MIT_License]
-                       [Run Notebook in LangChain Docs]
+                       [Run_Notebook_in_LangChain_Docs]
 
                                     [Demo]
 **Lemon AI helps you build powerful AI assistants in minutes and automate
 workflows by allowing for accurate and reliable read and write operations in
 [tools](#ð§©-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack
 and Github.** Most connectors available today are focused on read-only
 operations, limiting the potential of LLMs. Agents, on the other hand, have a
@@ -25,89 +25,91 @@
 defined APIs for reliable read and write operations. In addition, Lemon AI
 functions allow you to further reduce the risk of hallucinations by providing a
 way to statically define workflows that the model can rely on in case of
 uncertainty. ## â¡ï¸ Getting Started ### 1. Prerequisites Requires Python
 3.8.1 and above. ### 2. Installing To use Lemon AI in your Python project run
 `pip install lemonai`. The following example uses an OpenAI model. Therefore,
 we also need to `pip install openai`. Depending on which model you want to use
-this install is optional. ### 3. (Optional) Launch the Server The interaction
+this install is optional. ### 3. (Optional) Launch the server The interaction
 of your agents and all Lemon AI tools is provided by the [Lemon AI Server]
 (https://github.com/felixbrock/lemonai-server). Per default the Lemon AI Python
 client is sending requests to a hosted server version. To run the Lemon AI
 server on-prem please refer to the [Server Documentation](https://github.com/
 felixbrock/lemonai-server). ### 4. Use Lemon AI with LangChain The easiest way
 to give Lemon AI a try is via the Jupyter Notebook you can find in the
 [LangChain Docs](https://python.langchain.com/docs/modules/agents/tools/
 integrations/lemonai). Lemon AI automatically solves given tasks by finding the
 right combination of relevant tools or uses Lemon AI Functions as an
 alternative. The following example demonstrates how to retrieve a user from
 Hackernews and write it to a table in Airtable: #### Include Lemon AI in your
 LangChain project ```Python import os from lemonai import execute_workflow from
-langchain import OpenAI ``` #### Load API Keys and Access Tokens To use tools
+langchain import OpenAI ``` #### Load API keys and access tokens To use tools
 that require authentication, you have to store the corresponding access
 credentials in your environment in the format "{tool name}\_{authentication
 string}" where the authentication string is one of ["API_KEY", "SECRET_KEY",
 "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN",
 "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY",
 "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN". ```Python """ Load all
 relevant API Keys and Access Tokens into your environment variables """
 os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*" os.environ
-["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*" ``` #### Define your
-prompt and execute the LangChain Agent ```Python hackernews_username = "*INSERT
-HACKERNEWS USERNAME HERE*" """ Guidelines on identifying Airtable ids here:
-https://www.highviewapps.com/kb/where-can-i-find-the-airtable-base-id-and-
-table-id/ """ airtable_base_id = "*INSERT BASE ID HERE*" airtable_table_id =
-"*INSERT TABLE ID HERE*" """ Define your instruction to be given to your LLM
-""" prompt = f"""Read information from Hackernews for user
-{hackernews_username} and then write the results to Airtable (baseId:
-{airtable_base_id}, tableId: {airtable_table_id}). Only write the fields
-"username", "karma" and "created_at_i". Please make sure that Airtable does NOT
-automatically convert the field types. """ """ Use the Lemon AI
+["GITHUB_API_KEY"] = "*INSERT GITHUB API KEY HERE*" os.environ
+["DISCORD_WEBHOOK_URL"] = "*INSERT DISCORD CHANNEL WEBHOOK URL HERE*" ``` ####
+Example of defining your prompt and executing the Langchain Agent The following
+example makes use of several Lemon AI tools to 1. Retrieve details about a
+personal repository on GitHub 2. Get the top growing starred repositories of my
+account 3. Send a Discord message with results and review. ![Use Case Example]
+(use-case-example.png) ```Python lemonai_repo_owner = "Abdus2609"
+github_username = "Abdus2609" """ Define your instruction to be given to your
+LLM """ prompt = f"""Get the description for a repository I am working with
+called lemonai (owner {lemonai_repo_owner}). Also, get my top growing starred
+repositories (username {github_username}). Analyze the descriptions of both the
+LemonAI repository and my top-starred repositories. Then, send a Discord
+message that first displays a numerically bullet-pointed leaderboard of the top
+growing starred repositories and their growth, and secondly discuss how each
+tool could be useful specifically to lemonai's use case based on your analysis
+of the descriptions of each repository.""" """ Use the Lemon AI
 execute_workflow wrapper to run your LangChain agent in combination with Lemon
 AI """ model = OpenAI(temperature=0) execute_workflow(llm=model,
 prompt_string=prompt) ``` #### (Optional) Define your Lemon AI Functions
 Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-
 other-api-updates), Lemon AI provides the option to define workflows as
 reusable functions. These functions can be defined for use cases where it is
 especially important to move as close as possible to near-deterministic
 behavior. Specific workflows can be defined in a separate lemonai.json. You can
 find the corresponding tool ids (e.g. `hackernews-get-user`) in the [Tool Docs]
-(https://github.com/felixbrock/lemonai-py-client/blob/main/docs/tools.md):
-```json [ { "name": "Hackernews Airtable User Workflow", "description":
-"retrieves user data from Hackernews and appends it to a table in Airtable",
-"tools": ["hackernews-get-user", "airtable-append-data"] } ] ``` Your model
-will have access to these functions and will prefer them over self-selecting
-tools to solve a given task. All you have to do is to let the agent know that
-it should use a given function by including the function name in the prompt
-(e.g. `prompt = f"""Execute the Hackernews Airtable user workflow...`). ### 4.
-Gain transparency on your Agent's decision making To gain transparency on how
-your Agent interacts with Lemon AI tools to solve a given task, all decisions
-made, tools used and operations performed are written to a local `lemonai.log`
-file. Every time your LLM agent is interacting with the Lemon AI tool stack a
+(https://github.com/felixbrock/lemonai/blob/main/docs/tools.md): ```json [
+{ "name": "Hackernews Airtable User Workflow", "description": "retrieves user
+data from Hackernews and appends it to a table in Airtable", "tools":
+["hackernews-get-user", "airtable-append-data"] } ] ``` Your model will have
+access to these functions and will prefer them over self-selecting tools to
+solve a given task. All you have to do is to let the agent know that it should
+use a given function by including the function name in the prompt (e.g. `prompt
+= f"""Execute the Hackernews Airtable user workflow...`). ### 5. Gain
+transparency on your Agent's decision making To gain transparency on how your
+Agent interacts with Lemon AI tools to solve a given task, all decisions made,
+tools used and operations performed are written to a local `lemonai.log` file.
+Every time your LLM agent is interacting with the Lemon AI tool stack a
 corresponding log entry is created: ```log 2023-06-26T11:50:27.708785+0100 -
 b5f91c59-8487-45c2-800a-156eac0c7dae - hackernews-get-user 2023-06-26T11:50:
 39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - airtable-append-data
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d -
 hackernews-get-user 2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-
 55b50007ed9d - airtable-append-data ``` By using the [Lemon AI Analytics Tool]
 (https://github.com/felixbrock/lemonai-analytics) you can easily gain a better
 understanding of how frequently and in which order tools are used. As a result,
 you can identify weak spots in your agentâs decision-making capabilities and
 move to a more deterministic behavior by defining Lemon AI functions. ![Heatmap
 Example](heatmap-example.png) ## ð§© Supported Tools We already allow agents
-to interact with over [120 tools](https://github.com/felixbrock/lemonai-py-
-client/blob/main/docs/tools.md) across the following services: - HackerNews -
-Airtable - Slack - HubSpot - Github - Notion - Discord ## ð©» Next Up - [x]
-Github - [x] Notion - [x] Discord - [ ] Gmail - [ ] Google Calendar - [ ] Kafka
-- [ ] Pipedrive - [ ] Monday.com - [ ] Stripe - [ ] Medium - [ ] Google Cloud
+to interact with over [120 tools](https://github.com/felixbrock/lemonai/blob/
+main/docs/tools.md) across the following services: - HackerNews - Airtable -
+Slack - HubSpot - Github - Notion - Discord ## ð©» Next Up - [x] Github - [x]
+Notion - [x] Discord - [ ] Gmail - [ ] Google Calendar - [ ] Kafka - [ ]
+Pipedrive - [ ] Monday.com - [ ] Stripe - [ ] Medium - [ ] Google Cloud
 Realtime Database - [ ] Salesforce ## ð¦¸ Contributing Great to see you here!
 We are extremely open to contributions! You can find more information in our
-[CONTRIBUTING.md](https://github.com/felixbrock/lemonai-py-client/blob/
-main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop
-us a message on Discord. ## â¤ï¸âð¥ Team
-      Hey there ð¥³ I am Felix, the creator of Lemon AI. Always happy to chat and
-Felix answer any questions you might have! So feel free to reachout on Twitter or
-      Email
-### Active Contributors > Team members and people who actively help out
-improving the codebase by making PRs and reviewing code.
+[CONTRIBUTING.md](https://github.com/felixbrock/lemonai/blob/main/.github/
+CONTRIBUTING.md). If you have any more questions feel free to drop us a message
+on Discord. ## â¤ï¸âð¥ Contributors > Those are the team members and
+people who actively help out improving the codebase by making PRs and reviewing
+code. We are beyond grateful for your help!
 
-Mohammed_Hannan Hai_Nghiem Clemens_Schroeer Felix_Brockmeier
+Felix_Brockmeier Mohammed_Hannan Hai_Nghiem Clemens_Schroeer
```

