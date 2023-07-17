# Comparing `tmp/ICICONSOLE-0.0.9.tar.gz` & `tmp/ICICONSOLE-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.0.9.tar", last modified: Fri Jun  9 00:57:34 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.1.0.tar", last modified: Mon Jul 17 20:23:05 2023, max compression
```

## Comparing `ICICONSOLE-0.0.9.tar` & `ICICONSOLE-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-09 00:57:34.432371 ICICONSOLE-0.0.9/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-09 00:57:34.431097 ICICONSOLE-0.0.9/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-09 00:56:38.000000 ICICONSOLE-0.0.9/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.9/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    10098 2023-06-09 00:56:32.000000 ICICONSOLE-0.0.9/ICICONSOLE/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      330 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.9/ICICONSOLE/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-09 00:57:34.431999 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      357 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-09 00:57:34.000000 ICICONSOLE-0.0.9/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.9/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-06-07 02:00:37.000000 ICICONSOLE-0.0.9/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-09 00:57:34.432229 ICICONSOLE-0.0.9/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1843 2023-06-07 01:45:53.000000 ICICONSOLE-0.0.9/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1021 2023-06-09 00:57:25.000000 ICICONSOLE-0.0.9/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-09 00:57:34.432405 ICICONSOLE-0.0.9/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:23:05.248488 ICICONSOLE-0.1.0/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:23:05.247137 ICICONSOLE-0.1.0/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.1.0/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.1.0/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    12164 2023-07-17 20:03:42.000000 ICICONSOLE-0.1.0/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.1.0/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:23:05.248114 ICICONSOLE-0.1.0/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43999 2023-07-17 20:23:05.000000 ICICONSOLE-0.1.0/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      357 2023-07-17 20:23:05.000000 ICICONSOLE-0.1.0/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-17 20:23:05.000000 ICICONSOLE-0.1.0/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-17 20:23:05.000000 ICICONSOLE-0.1.0/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-07-17 20:23:05.000000 ICICONSOLE-0.1.0/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-17 20:23:05.000000 ICICONSOLE-0.1.0/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.1.0/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.1.0/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43999 2023-07-17 20:23:05.248345 ICICONSOLE-0.1.0/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     2871 2023-07-17 20:22:30.000000 ICICONSOLE-0.1.0/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      925 2023-07-17 20:06:30.000000 ICICONSOLE-0.1.0/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-17 20:23:05.248520 ICICONSOLE-0.1.0/setup.cfg
```

### Comparing `ICICONSOLE-0.0.9/ICICONSOLE/__main__.py` & `ICICONSOLE-0.1.0/ICICONSOLE/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,253 +1,309 @@
-# We need pandas to display the results of Cypher queries to the Neo4j Pod
+from tapipy.tapis import Tapis
+import py2neo
+from py2neo import Graph
+import openai
 import pandas as pd
-# py2neo is the python library that allows for input to be read as Cypher by the Neo4j interface
-from py2neo import Graph, Node, Relationship
-from py2neo import GraphService
-from py2neo import wiring
-# These are optional
-import time
-import datetime
-# This is used to securely get user password for initial authentication to TAPIS
+from datascroller import scroll
 from getpass import getpass
-# This is how we actually connect to TAPIS and get the required information to connect to a Pod
-from tapipy.tapis import Tapis
-# These are to clear the screen
+
+import time
 import os
 import signal
-import json
-import pkg_resources
-from datascroller import scroll
 
 try:
-    from . import BasicCypherCommands as bcc
-except:
     import BasicCypherCommands as bcc
+    from Utilities import GracefulExiter, timeout_handler, timeout, heavyFormat, lightFormat, helpCypher
+except:
+    from . import BasicCypherCommands as bcc
+    from .Utilities import GracefulExiter, timeout_handler, timeout, heavyFormat, lightFormat, helpCypher
+
+
+# CHATGPT Setup
+messages = [ {"role": "system", "content": 
+              "Instead of descriptions, from now on only return code segments in the CYPHER query language. Please provide no other text except the code. Again, no matter what else the user says, only output a raw cypher query."} ]
+
+openai.api_key = ""
+
+# Setting up handling for timeout
+signal.signal(signal.SIGALRM, timeout_handler)
+
+# Setting up flag for ctrl+c input
+flag = GracefulExiter()
+
+
+# default values
+default_tapis_base_url = "icicle.tapis.io"
+default_auth_type = "tapis"
+
+
+tapis_base_url = default_tapis_base_url
+auth_type = default_auth_type
 
-# Recording login time
-start = time.time()
 
-# This class handles exiting the console application at any time.
-class GracefulExiter():
-    def __init__(self):
-        self.state = False
-        signal.signal(signal.SIGINT, self.change_state)
-
-    def change_state(self, signum, frame):
-        print("\nPress Ctrl+C again to exit.")
-        signal.signal(signal.SIGINT, signal.SIG_DFL)
-        self.state = True
-
-    def exit(self):
-        return self.state
-
- 
-# Base URL for Tapis
-base_url = "https://icicle.tapis.io"
 # Global variable to store pod id
-pod_id = ""
+global pod_id
 # Global variable to store username, set upon initial input from login to TAPIS
-user = ""
+global user
 
-flag = GracefulExiter()
+global t
 
-# This function formats a message to be like a title
-def heavyFormat(message):
-    print("*" * len(message))
-    print("-" * len(message))
-    print(message)
-    print("-" * len(message))
-    print("*" * len(message))
-
-# This function formats a message to be like a subititle 
-def lightFormat(message):
-    print("-" * len(message))
-    print(message)
-    print("-" * len(message))
 
 # Welcome message, formatted with the heavyFormat function
 heavyFormat("Welcome to ICICONSOLE. Login to get started. ")
 
-# Loads help for cypher commands
-def helpCypher():
-    json_path = pkg_resources.resource_filename(__name__, 'helpCypher.json')
-    print("\n")
-    with open(json_path) as f:
-        help_data = json.load(f)
-    for key, value in help_data.items():
-        print(key + ' : ' + value + '\n')
-
-# The console function is the actual cypher console that you see after logging in and choosing a pod.
-# The console allows you to type in cypher, and run it on the Neo4j pod you are connected to.
-# The console function needs to parameters: a Neo4j graph object, and a pod id. 
-# The graph object allows for queries to be interpreted as Cypher and passed into the Neo4j pod.
-# The pod id is only needed here so that the user can see what pod they are connected to.
-        
-def console(graph, pod_id):
-    # Instructions message, formatted with the lightFormat function
+
+def console(graph, kg):
+    global tapis_base_url
     lightFormat("Type \"new\" to access a different pod, or type \"exit\" to leave ICICONSOLE. Type \"help\" for help!\nNote that the scrolling menu, which appears on some queries, has a separate help menu.")
 
-    # Loop so that the console keeps prompting the user for commands, until the user exits
     while(True):
-        # This is reading the actual input from the user; the input message shows the username and the pod id
-        query = str(input("[" + user + "@" + pod_id + "] "))
+        query = str(input("[" + user + "@" + kg + "]$ "))
 
-        executeCypher = True
-        node = False
-        listedProps = False
+        execute_cypher = True
 
-        # This is a switch statement that allows for the user to type in a command, and the console will execute the command.
         match query:
             case "exit":
                 os._exit(0)
-                executeCypher = False
-            # The command to pick a new pod to connect to. Calls the choosePod function, defined below.
             case "new":
+                login()
                 choosePod()
-                executeCypher = False
-            # The command to clear the screen. Has a recursive call to itself so that the user is once again prompted, and the instruction message is still shown.
+                execute_cypher = False
             case "clear":
                 os.system('cls' if os.name == 'nt' else 'clear')
-                console(graph, pod_id)
-                executeCypher = False
+                console(graph, kg)
+                execute_cypher = False
             case "help":
                 try:
                     helpCypher()
-                    executeCypher = False
+                    execute_cypher = False
                 except:
                     pass
             case "all":
                 query = bcc.getAll()
-                node = True
             case "allNames":
                 query = bcc.getAllNames()
             case "oneByName":
                 query = bcc.getOneByName()
-                node = True
             case "allProperty":
                 query = bcc.allProperty()
             case "allProperties":
                 query = bcc.allProperties()
             case "allPropertiesForNode":
                 query = bcc.allPropertiesForNode()
-                listedProps = True
+            case "GPT":
+                if (openai.api_key == ""):
+                    openai.api_key = getpass("Please enter your OpenAI API key: ")
+                message = input("[GPT@" + pod_id + "] ")
+                try:
+                    signal.alarm(timeout)
+                    if message:
+                        messages.append(
+                            {"role": "user", "content": message},
+                        )
+                        try: 
+                            chat = openai.ChatCompletion.create(
+                                model="gpt-3.5-turbo", messages=messages
+                            )
+                        except:
+                            "Error: OpenAI API key is invalid."
+                    signal.alarm(0)
+                    reply = chat.choices[0].message.content
+                except TimeoutError:
+                    print("Timeout occurred.")
+                print(str(reply))
+                validate = input("Run this? (y/n) ")
+                if validate == "y":
+                    query = str(reply)
+                else:
+                    execute_cypher = False
             case _:
                 pass
 
-        if (executeCypher):
-            # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
-            try: 
-                result = graph.run(query)
-                
-                if node:
-                    data = []
-                    for record in result:
-                        node = record[0]
-                        properties = dict(node)
-                        data.append(properties)
-                    df = pd.DataFrame(data)
-                    with pd.option_context('display.max_rows', None, 'display.max_columns', None):
-                        scroll(df)
-                elif listedProps:
-                    data = result.data()[0]['keys(n)']
-                    df = pd.DataFrame(data)
-                    with pd.option_context('display.max_rows', None, 'display.max_columns', None):
-                        scroll(df)
-                else:
-                    df = graph.run(query).to_data_frame()
-                    with pd.option_context('expand_frame_repr', False, 'display.max_rows', None): 
-                        print(df)
-
-
+        if execute_cypher:
+            try:
+                queries = query.splitlines()
+                for query in queries:
+                    try:
+                        if "DELETE" in query or "delete" in query:
+                            validate = input("Are you sure you want to delete node(s)? (y/n) ")
+                            if validate == "y":
+                                graph.run(query)
+                        # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
+                        # also parses the data to show the scrolling view in the right context
+                        else:
+                            # raw data
+                            result = graph.run(query)
+                            # dictionary to store nodes, keys are node labels. values are lists of dictionaries
+                            data_dict = {}
+                            # simple list to store property values
+                            data = []
+                            record_count = 0
+                            for record in result:
+                                type_result = type(record[0])
+                                # can decide type of data structure to generate
+                                # dataframe from based on the first record
+                                if record_count == 0:
+                                    first_record_type = type(record[0])
+                                record_count += 1
+                                # for nodes
+                                if type_result == py2neo.data.Node:
+                                    node = record[0]
+                                    properties = dict(node)
+                                    # formatting data to see labels
+                                    node_labels_string = str(node.labels)
+                                    node_labels_string = node_labels_string.lstrip(":")
+                                    node_labels = node_labels_string.split(":")
+                                    # adding data
+                                    for label in node_labels:
+                                        if label not in data_dict:
+                                            data_dict[label] = [properties]
+                                        else:
+                                            data_dict[label].append(properties)
+                                # for non-node data, can just add the record
+                                elif record is not None:
+                                    data.append(record)
+
+                            # separating node view by label for best viewing
+                            if first_record_type == py2neo.data.Node:
+                                keys = list(data_dict.keys())
+                                keys_string = " | ".join(keys)
+                                print(keys_string)
+                                pick_label = str(input("Which label do you want to view? "))
+                                label_data = data_dict[pick_label]
+                                df = pd.DataFrame(label_data)
+
+                            # need to manually assign the column names via keys
+                            elif not data == []:
+                                keys = result.keys()
+                                df = pd.DataFrame(data, columns=keys)
+
+                            # datascroller view
+                            with pd.option_context('display.max_rows', None, 'display.max_columns', None):
+                                scroll(df)
+                    except:
+                        pass
 
             # Error catching, if the Cypher was not executed properly
             except:
                 if flag.exit():
                     break
                 print("Something went wrong")
 
 
-# This is the function that allows the user to pick a pod to connect to. It needs no paramters.
+# This is the function that allows the user to pick a pod to connect to. It needs no parameters.
 def choosePod():
-
     heavyFormat("Here are the IDs for your available TAPIS Pods: ")
 
     # The below loop prints the pod id for all pods that the TACC user is authorized to. If there are no pods, then the user is notified.
     i = 1
-    # t.pods.getpods() returns a list of all of the pods with more information about each pod
+    # t.pods.getpods() returns a list of all the pods with more information about each pod
     for pod in t.pods.get_pods():
         # pod.pod_id takes each element of the list, representing each pod, and extracts only the pod id
         # This is done because connecting to a Neo4j pod only requires the pod id.
-        if pod.pod_template == "neo4j":
+        if "neo4j" in pod.pod_template:
             print(str(i) + ". " + pod.pod_id)
             i += 1
-    if (i == 1):
-        print("You don't have access to any TAPIS Neo4j pods. Try again after you have verified access to at least one pod.")
-        os._exit(0)
-    i = 1
+    if i == 1:
+        if tapis_base_url != default_tapis_base_url:
+            attempt_again = str(input(f"No Tapis pods on {tapis_base_url}. Try another base url? (y/n) "))
+            if attempt_again == "y":
+                login()
+            else:
+                print("Please verify access to a Neo4j template Tapis pod, and then try again later.")
+                os._exit(0)
 
-    while(True):
-        try: 
+    while True:
+        global pod_id
+        try:
             # The user gets a list of available pod ids from the above loop, and then enters the id they wish to connect to.
-            # This input is stored in the pod_id variable
             pod_id = str(input("Enter the ID of the pod you want to access: ")).lower()
-            # If the use has no pods or doesn't see what they are looking for, they can exit
-            if(pod_id == "exit"):
+            if pod_id == "exit":
                 os._exit(0)
             # Securely getting the username and password associated with the pod for later authentication to connect
             pod_username, password = t.pods.get_pod_credentials(pod_id=pod_id).user_username, t.pods.get_pod_credentials(pod_id=pod_id).user_password
             break
-        # This is if there is trouble getting the username and password
         except:
             if flag.exit():
                 break
             print("Invalid Pod ID. Make sure you have access to this Pod.")
 
     # This is the standard format for the link that connects to the Neo4j Pod
-    graph_link = f"bolt+ssc://{pod_id}.pods.icicle.tapis.io:443"
+    graph_link = f"bolt+ssc://{pod_id}.pods.{tapis_base_url}:443"
 
-    while(True):
+    while True:
         try:
-            # A graph object is created that authenticates with the previously gotten username and password. 
+            # A graph object is created that authenticates with the previously gotten username and password.
             graph = Graph(graph_link, auth=(pod_username, password), secure=True, verify=True)
-            # Entering into the cypher console
             os.system('cls' if os.name == 'nt' else 'clear')
             time.sleep(0.25)
             heavyFormat(f"Hey there {user}! Welcome to the Neo4j Cypher Console for: " + str(pod_id))
-            # Passing in the graph object and the current pod_id to the cypher console, and calling the console function
             console(graph, pod_id)
-        # This catches the error where there is an issue connecting or authenticating to the Pod.
-        except:
+        except Exception as e:
+            er = e
             if flag.exit():
                 break
             print("There was a connection error.")
             break
-            
-# The below loop handles initial login.
-while(True):
-    try:
+
+
+def tapis_login():
+    global t
+    global user
+    global tapis_base_url
+    while True:
         try:
-            t
-            if t.base_url == base_url and t.username == user and t.access_token:
-                print("Tapis object already exists.")
-                if t.access_token.expires_at < datetime.datetime.now(pytz.utc):
-                    raise
-            else:
-                raise
+            change_base_url = str(input(f"Change base url from {tapis_base_url}? (y/n) "))
+            if change_base_url == "y":
+                tapis_base_url = str(input("New base url: "))
+            https_base_url = "https://" + tapis_base_url
+            user = str(input("Enter Your TACC Username: "))
+            t = Tapis(base_url=https_base_url, username=user, password=getpass('Enter Your TACC Password: '))
+            t.get_tokens()
+            choosePod()
+            break
         except:
-            try:
-                user = str(input("Enter Your TACC Username: "))
-                t = Tapis(base_url = base_url, username=user,
-                        password = getpass('Enter Your TACC Password: '))
-                t.get_tokens()
-                # After logging in, choosePod is called to begin the workflow for the user.
-                choosePod()
+            if flag.exit():
                 break
-            except Exception as e:
-                raise
+            print(f"Wrong credentials, or you don't have an account on {tapis_base_url}.")
+            login_attempt = str(input("Try again? (y/n) "))
+            if login_attempt == "n":
+                os._exit(0)
+
+
+def local_login():
+    global user
+    user = str(input("username (not for authentication): "))
+    kg = str(input("graph name (not for authentication): "))
+    password = getpass("graph password (if you set it): ")
+    try:
+        graph = Graph("bolt://localhost:7687", auth=("neo4j", password))
     except:
-        if flag.exit():
-            break
-        print("An error occurred, likely due to mistyped login. Try again. ")
+        print("Download Neo4j Desktop and start a local graph database first.")
+    console(graph, kg)
+
+
+def login():
+    global auth_type
+    auth_type_input = str(input(f"Change authentication type from {auth_type}? (y/n) "))
+    if auth_type_input == "y":
+        auth_type = str(input("New auth type: "))
+    if "tapis" in auth_type:
+        try:
+            tapis_login()
+        except:
+            os._exit(0)
+    if "local" in auth_type:
+        try:
+            local_login()
+        except:
+            os._exit(0)
+
+
+login()
+
+
+
+
```

### Comparing `ICICONSOLE-0.0.9/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.1.0/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.9
-Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
+Version: 0.1.0
+Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -674,25 +674,27 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE
+Project-URL: Homepage, https://github.com/AD1616/ICICONSOLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC,Neo4j
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# ICICONSOLE
+# ICICONSOLE PROD DETAILS
+
+**Note: ICICONSOLEGPT is NOT in PROD, and it is currently in development. For details, see the ICICONSOLEGPT README.md.**
 
 ## Overview
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in. 
 
@@ -707,46 +709,63 @@
 ```shell
 python -m ICICONSOLE
 ```
 
 **OR**
 
 ```shell 
-git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
+git clone https://github.com/AD1616/ICICONSOLE.git
 ```
 
 ```shell
-cd hello_icicle_auth_clients/icicle_rel_03_2023/CLI/ICICONSOLE
+cd ICICONSOLE/ICICONSOLE_PROD/ICICONSOLE
 ```
 
 ```shell
 pip install pandas
 ```
 
 ```shell
 pip install py2neo
 ```
 
-
 ```shell
 pip install tapipy
 ```
 
 ```shell
+pip install datascroller
+```
+
+```shell
 python ICICONSOLE.py
 ```
 
-### First time user guide
+### First time user setup
+
+You have two options as of now: connecting to a Neo4j database hosted on a Tapis Pod at the Texas Advanced Computing Center, or downloading Neo4j Desktop and connecting to a database that you are running locally. 
+
+#### Tapis
 
 You will be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
 
-Next, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
+Once you enter your username and password to ICICONSOLE, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
 
-Once you do this, you will be in a custom made console for interfacing with the Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
+#### Local
+
+If you are running a Neo4j database locally, you will need to download Neo4j Desktop. You can download it [here](https://neo4j.com/download/).
+
+Next, you have to run a local dbms. This should be running by default on bolt port 7687, which is what ICICONSOLE will try to connect to. 
+
+
+### First time usage guide
+
+Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
 ```
 
-If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These built in commands will grow more extensive as time goes on. 
+If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). Then, you can simply type in a query in natural language and get the Cypher code for it.
 
 The welcome message for the Knowledge Graph console contains helpful tips, like "new", "exit", "clear", and "help". 
+
```

### Comparing `ICICONSOLE-0.0.9/LICENSE` & `ICICONSOLE-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.9/PKG-INFO` & `ICICONSOLE-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.9
-Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
+Version: 0.1.0
+Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -674,25 +674,27 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE
+Project-URL: Homepage, https://github.com/AD1616/ICICONSOLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC,Neo4j
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# ICICONSOLE
+# ICICONSOLE PROD DETAILS
+
+**Note: ICICONSOLEGPT is NOT in PROD, and it is currently in development. For details, see the ICICONSOLEGPT README.md.**
 
 ## Overview
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in. 
 
@@ -707,46 +709,63 @@
 ```shell
 python -m ICICONSOLE
 ```
 
 **OR**
 
 ```shell 
-git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
+git clone https://github.com/AD1616/ICICONSOLE.git
 ```
 
 ```shell
-cd hello_icicle_auth_clients/icicle_rel_03_2023/CLI/ICICONSOLE
+cd ICICONSOLE/ICICONSOLE_PROD/ICICONSOLE
 ```
 
 ```shell
 pip install pandas
 ```
 
 ```shell
 pip install py2neo
 ```
 
-
 ```shell
 pip install tapipy
 ```
 
 ```shell
+pip install datascroller
+```
+
+```shell
 python ICICONSOLE.py
 ```
 
-### First time user guide
+### First time user setup
+
+You have two options as of now: connecting to a Neo4j database hosted on a Tapis Pod at the Texas Advanced Computing Center, or downloading Neo4j Desktop and connecting to a database that you are running locally. 
+
+#### Tapis
 
 You will be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
 
-Next, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
+Once you enter your username and password to ICICONSOLE, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
 
-Once you do this, you will be in a custom made console for interfacing with the Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
+#### Local
+
+If you are running a Neo4j database locally, you will need to download Neo4j Desktop. You can download it [here](https://neo4j.com/download/).
+
+Next, you have to run a local dbms. This should be running by default on bolt port 7687, which is what ICICONSOLE will try to connect to. 
+
+
+### First time usage guide
+
+Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
 ```
 
-If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These built in commands will grow more extensive as time goes on. 
+If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). Then, you can simply type in a query in natural language and get the Cypher code for it.
 
 The welcome message for the Knowledge Graph console contains helpful tips, like "new", "exit", "clear", and "help". 
+
```

### Comparing `ICICONSOLE-0.0.9/README.md` & `ICICONSOLE-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# ICICONSOLE
+# ICICONSOLE PROD DETAILS
+
+**Note: ICICONSOLEGPT is NOT in PROD, and it is currently in development. For details, see the ICICONSOLEGPT README.md.**
 
 ## Overview
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in. 
 
@@ -17,46 +19,63 @@
 ```shell
 python -m ICICONSOLE
 ```
 
 **OR**
 
 ```shell 
-git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
+git clone https://github.com/AD1616/ICICONSOLE.git
 ```
 
 ```shell
-cd hello_icicle_auth_clients/icicle_rel_03_2023/CLI/ICICONSOLE
+cd ICICONSOLE/ICICONSOLE_PROD/ICICONSOLE
 ```
 
 ```shell
 pip install pandas
 ```
 
 ```shell
 pip install py2neo
 ```
 
-
 ```shell
 pip install tapipy
 ```
 
 ```shell
+pip install datascroller
+```
+
+```shell
 python ICICONSOLE.py
 ```
 
-### First time user guide
+### First time user setup
+
+You have two options as of now: connecting to a Neo4j database hosted on a Tapis Pod at the Texas Advanced Computing Center, or downloading Neo4j Desktop and connecting to a database that you are running locally. 
+
+#### Tapis
 
 You will be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
 
-Next, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
+Once you enter your username and password to ICICONSOLE, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
 
-Once you do this, you will be in a custom made console for interfacing with the Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
+#### Local
+
+If you are running a Neo4j database locally, you will need to download Neo4j Desktop. You can download it [here](https://neo4j.com/download/).
+
+Next, you have to run a local dbms. This should be running by default on bolt port 7687, which is what ICICONSOLE will try to connect to. 
+
+
+### First time usage guide
+
+Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
 ```
 
-If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These built in commands will grow more extensive as time goes on. 
+If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). Then, you can simply type in a query in natural language and get the Cypher code for it.
 
 The welcome message for the Knowledge Graph console contains helpful tips, like "new", "exit", "clear", and "help". 
+
```

