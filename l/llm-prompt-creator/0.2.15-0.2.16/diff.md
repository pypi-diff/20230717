# Comparing `tmp/llm_prompt_creator-0.2.15.tar.gz` & `tmp/llm_prompt_creator-0.2.16.tar.gz`

## Comparing `llm_prompt_creator-0.2.15.tar` & `llm_prompt_creator-0.2.16.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/main.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/prompter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/src/llm_prompt_creator/__init__.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/src/llm_prompt_creator/prompt.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/LICENSE
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/README.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/pyproject.toml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/PKG-INFO
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/main.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/prompter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/src/llm_prompt_creator/__init__.py
+-rw-r--r--   0        0        0     7689 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/src/llm_prompt_creator/prompt.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/LICENSE
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/README.md
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/pyproject.toml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.16/PKG-INFO
```

### Comparing `llm_prompt_creator-0.2.15/main.py` & `llm_prompt_creator-0.2.16/main.py`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.15/prompter.py` & `llm_prompt_creator-0.2.16/prompter.py`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.15/src/llm_prompt_creator/prompt.py` & `llm_prompt_creator-0.2.16/src/llm_prompt_creator/prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,17 +50,17 @@
     with open(f"{outdir}/training_data.json", 'w') as f:
         json.dump(training_data_str, f)
     with open(f"{outdir}/chunks.json", 'w') as f:
         json.dump(chunks, f)
     with open(f"{outdir}/failed_files.json", 'w') as f:
         json.dump(failed_files, f)
 
-def create_store(filepath:str="chunks.json", persistdir:str="db", model:str="gpt-3.5-turbo"):
+def create_store(filepath:str="chunks.json", persistdir:str="db", model:str="text-embedding-ada-002"):
     """Create the vector store to utilize for other commands (currently limited to OpenAI). Consumes filepath (JSON format) that defaults to a local 
-    'chunks.json' to match default behavior of data-chunker module. 
+    'chunks.json' to match default behavior of data-chunker module. Utilizes an API call to OpenAI embedders; defaults to using the text-embedding-ada-002 model
     
     Returns a Chroma store."""
     
     #TODO: make an ephemeral option
     #TODO: make a for loop to iterate over a potential suite of JSON files
 
     str_chunks = []
@@ -79,18 +79,20 @@
     
 def search_store(store: Chroma, text: str):
     """Perform a similarity search against the Chroma vector store based on the text provided."""
     store_chunks = store.similarity_search(text)
 
     return store_chunks
 
-def prompt(store: Chroma, show_context=False, templateFilePath:str=None):
+def prompt(store: Chroma, show_context=False, templateFilePath:str=None, model:str="gpt-3.5-turbo"):
     """Setup a chat session with the LLM (currently limited to OpenAI). The session maintains history by storing the
     previous answers into a history list and appending them to each future prompt, meaning there is a limit for number of 
     questions per individual session (you will eventually reach the token limit per model).
+
+    Defaults to using OpenAI's GPT-3.5-Turbo
     
     Will continue the chat session until the user types 'exit' as their prompt."""
 
     history = ""
 
     # Load the promptTemplate for model context :
     if templateFilePath != None:
@@ -129,18 +131,18 @@
             for i, chunk in enumerate(chunks):
                 contexts.append(f"Context {i}:\n{chunk.page_content}")
             with open('contexts.json', 'w') as f:
                 json.dump(contexts, f)
             joined_contexts = "\n\n".join(contexts)
             
             prompt = Prompt(template=promptTemplate, input_variables=["context", "question", "history"])
-            llmChain = LLMChain(prompt=prompt, llm=ChatOpenAI(model="gpt-3.5-turbo",temperature=0))
+            llmChain = LLMChain(prompt=prompt, llm=ChatOpenAI(model=model,temperature=0))
             # If user's asked to show the context, provide it to them (chunks of text from their vector store):
             if (show_context):
-                print(f"Context Provided: {joined_contexts}")
+                print(f"Context Provided: \n{joined_contexts}")
 
             # For each message to OpenAI, print tokens used for each part and in total
             question_tokens = llmChain.llm.get_num_tokens(question)
             contexts_tokens = llmChain.llm.get_num_tokens(joined_contexts)
             history_tokens = llmChain.llm.get_num_tokens(history)
             print("Question tokens: " + str(question_tokens) + "\n" +
                 "Contexts' tokens: " + str(contexts_tokens) + "\n" +
```

### Comparing `llm_prompt_creator-0.2.15/LICENSE` & `llm_prompt_creator-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.15/README.md` & `llm_prompt_creator-0.2.16/README.md`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.15/pyproject.toml` & `llm_prompt_creator-0.2.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "archive/",
     "venv/",
     "*.json",
 ]
 
 [project]
 name = "llm_prompt_creator"
-version = "0.2.15"
+version = "0.2.16"
 authors = [
     {name="Chris Mills", email="cmills@breakfreesolutions.com"},
     {name="Zak Alford", email="zalford@breakfreesolutions.com"}
 ]
 description = "Takes a given directory and parses its contents to create a text vectorstore to be consumed in prompts for various LLM models."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `llm_prompt_creator-0.2.15/PKG-INFO` & `llm_prompt_creator-0.2.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_prompt_creator
-Version: 0.2.15
+Version: 0.2.16
 Summary: Takes a given directory and parses its contents to create a text vectorstore to be consumed in prompts for various LLM models.
 Project-URL: Homepage, https://github.com/break-free/fineract-unit-tests-openai
 Project-URL: Issues, https://github.com/break-free/fineract-unit-tests-openai/issues
 Author-email: Chris Mills <cmills@breakfreesolutions.com>, Zak Alford <zalford@breakfreesolutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

