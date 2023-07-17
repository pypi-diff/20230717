# Comparing `tmp/idoctorai-0.7.4.tar.gz` & `tmp/idoctorai-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.7.4.tar", max compression
+gzip compressed data, was "idoctorai-0.7.5.tar", max compression
```

## Comparing `idoctorai-0.7.4.tar` & `idoctorai-0.7.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.7.4/LICENSE
--rw-r--r--   0        0        0    28301 2023-07-08 01:31:34.043216 idoctorai-0.7.4/pandasai/__init__.py
--rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 idoctorai-0.7.4/pandasai/constants.py
--rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 idoctorai-0.7.4/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.7.4/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 idoctorai-0.7.4/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 idoctorai-0.7.4/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 idoctorai-0.7.4/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.7.4/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 idoctorai-0.7.4/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3587 2023-07-07 01:01:47.985267 idoctorai-0.7.4/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 idoctorai-0.7.4/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0     4643 2023-07-08 01:22:44.839806 idoctorai-0.7.4/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.7.4/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 idoctorai-0.7.4/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11783 2023-07-07 14:00:39.631141 idoctorai-0.7.4/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.7.4/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 idoctorai-0.7.4/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 idoctorai-0.7.4/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 idoctorai-0.7.4/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     4154 2023-07-07 14:00:39.632140 idoctorai-0.7.4/pandasai/llm/model.py
--rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 idoctorai-0.7.4/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3599 2023-07-07 14:00:39.633137 idoctorai-0.7.4/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.7.4/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 idoctorai-0.7.4/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 idoctorai-0.7.4/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 idoctorai-0.7.4/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 idoctorai-0.7.4/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.7.4/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 idoctorai-0.7.4/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1349 2023-07-07 14:00:39.634134 idoctorai-0.7.4/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1125 2023-07-07 14:00:39.635132 idoctorai-0.7.4/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1295 2023-07-07 14:00:39.636130 idoctorai-0.7.4/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 idoctorai-0.7.4/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1339 2023-07-07 14:00:39.637343 idoctorai-0.7.4/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1922 2023-07-08 01:34:21.663627 idoctorai-0.7.4/pyproject.toml
--rw-r--r--   0        0        0       96 2023-07-07 14:00:39.620963 idoctorai-0.7.4/README.md
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 idoctorai-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.7.5/LICENSE
+-rw-r--r--   0        0        0    27932 2023-07-17 07:58:43.438913 idoctorai-0.7.5/pandasai/__init__.py
+-rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 idoctorai-0.7.5/pandasai/constants.py
+-rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 idoctorai-0.7.5/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.7.5/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 idoctorai-0.7.5/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 idoctorai-0.7.5/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 idoctorai-0.7.5/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.7.5/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 idoctorai-0.7.5/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3635 2023-07-17 07:57:55.760373 idoctorai-0.7.5/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 idoctorai-0.7.5/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0     4643 2023-07-08 01:22:44.839806 idoctorai-0.7.5/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-17 02:43:35.387669 idoctorai-0.7.5/pandasai/langchain/agents.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.7.5/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 idoctorai-0.7.5/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    14051 2023-07-12 13:05:59.808678 idoctorai-0.7.5/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.7.5/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 idoctorai-0.7.5/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 idoctorai-0.7.5/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 idoctorai-0.7.5/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     4154 2023-07-07 14:00:39.632140 idoctorai-0.7.5/pandasai/llm/model.py
+-rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 idoctorai-0.7.5/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3599 2023-07-07 14:00:39.633137 idoctorai-0.7.5/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.7.5/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 idoctorai-0.7.5/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 idoctorai-0.7.5/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 idoctorai-0.7.5/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 idoctorai-0.7.5/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.7.5/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 idoctorai-0.7.5/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1349 2023-07-07 14:00:39.634134 idoctorai-0.7.5/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1125 2023-07-07 14:00:39.635132 idoctorai-0.7.5/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1295 2023-07-07 14:00:39.636130 idoctorai-0.7.5/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 idoctorai-0.7.5/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1339 2023-07-07 14:00:39.637343 idoctorai-0.7.5/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     2064 2023-07-17 03:29:32.558699 idoctorai-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-07-07 14:00:39.620963 idoctorai-0.7.5/README.md
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 idoctorai-0.7.5/PKG-INFO
```

### Comparing `idoctorai-0.7.4/LICENSE` & `idoctorai-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/__init__.py` & `idoctorai-0.7.5/pandasai/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,14 +148,15 @@
         "df_columns": None,
         "num_rows": None,
         "num_columns": None,
     }
     _cache: Cache = None
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
+    _img_path: Optional[str] = None
     _middlewares: List[Middleware] = [ChartsMiddleware()]
     _additional_dependencies: List[dict] = []
     _custom_whitelisted_dependencies: List[str] = []
     _start_time: float = 0
     _enable_logging: bool = True
     _logger: logging.Logger = None
     _logs: List[str] = []
@@ -430,19 +431,19 @@
             if is_conversational_answer is None:
                 is_conversational_answer = self._is_conversational_answer
             if is_conversational_answer:
                 answer = self.conversational_answer(prompt, answer)
                 self.log(f"Conversational answer: {answer}")
 
             self.log(f"Executed in: {time.time() - self._start_time}s")
-
+            
             return answer
         except Exception as exception:
             self.last_error = str(exception)
-            print(exception)
+            # print(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
             )
 
     def add_middlewares(self, *middlewares: List[Middleware]):
@@ -656,19 +657,22 @@
 
         """
 
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
-            code = add_save_chart(
+            obj = add_save_chart(
                 code, self._prompt_id, self._save_charts_path, not self._verbose
             )
+            # record img save path
+            code = obj[0]
+            self._img_path = obj[1]
 
-        # code = "import pandas as pd\nfrom sklearn.linear_model import LinearRegression\n\n# Load the data into a pandas DataFrame\ndf1 = pd.DataFrame({\n    'Bank Name': ['Silicon Valley Bank', 'Signature Bank', 'Almena State Bank', \n                  'First City Bank of Florida', 'First Republic Bank'],\n    'City': ['Fort Walton Beach', 'San Francisco', 'New York', 'Almena', 'Santa Clara'],\n    'State': ['CA', 'KS', 'CA', 'FL', 'NY'],\n    'Cert': [16748, 15426, 15426, 24735, 24735],\n    'Acquiring Institution': ['Flagstar Bank, N.A.', 'First Citizens Bank & Trust Company', \n                              'United Fidelity Bank, fsb', 'Equity Bank', 'JPMorgan Chase Bank, N.A.'],\n    'Closing Date': ['23-Oct-20', '10-Mar-23', '1-May-23', '12-Mar-23', '16-Oct-20'],\n    'Fund': [10538, 10538, 10539, 10537, 10539]\n})\n\n# Convert the Closing Date column to a datetime object\ndf1['Closing Date'] = pd.to_datetime(df1['Closing Date'])\n\n# Add a column for the year of the closing date\ndf1['Closing Year'] = df1['Closing Date'].apply(lambda x: x.year)\n\n# Group the data by year and count the number of bank closures\ngrouped = df1.groupby('Closing Year').count()['Bank Name']\n\n# Create a linear regression model\nX = grouped.index.values.reshape(-1, 1)\ny = grouped.values.reshape(-1, 1)\nmodel = LinearRegression()\nmodel.fit(X, y)\n\n# Predict the number of bank closures in 2024\ny_pred = model.predict([[2024]])\nprint(int(round(y_pred[0][0])))"
+        # code = "# Import libraries\nimport pandas as pd\nfrom sklearn.linear_model import LinearRegression\nfrom sklearn.model_selection import train_test_split\n\n# Load data\ndf1 = pd.read_csv('df1.csv')\n\n# Convert 'Closing Date' column to datetime and extract year\ndf1['Closing Date'] = pd.to_datetime(df1['Closing Date'])\ndf1['Year Closed'] = df1['Closing Date'].dt.year\n\n# Group data by year and count number of closures\ndf2 = df1.groupby('Year Closed')['Bank Name'].count().reset_index()\ndf2.columns = ['Year', 'Closures']\n\n# Split data into training and testing sets\nX_train, X_test, y_train, y_test = train_test_split(df2['Year'], df2['Closures'], test_size=0.2)\n\n# Fit linear regression model to training data\nreg = LinearRegression().fit(X_train.values.reshape(-1, 1), y_train)\n\n# Predict number of closures in 2024\npredicted_closures = reg.predict([[2024]])\nprint(predicted_closures)"
 
         # Get the code to run removing unsafe imports and df overwrites
         code_to_run = self._clean_code(code)
         self.last_code_executed = code_to_run
         self.log(
             f"""
 Code running:
@@ -696,15 +700,14 @@
                     code = code_to_run
                     break
                 except Exception as e:
                     if not use_error_correction_framework:
                         raise e
 
                     count += 1
-
                     code_to_run = self._retry_run_code(code, e, multiple)
 
         captured_output = output.getvalue().strip()
         if code.count("print(") > 1:
             return captured_output
 
         # Evaluate the last line and return its value or the captured output
@@ -714,27 +717,27 @@
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
 
         match = re.match(r"^print\((.*)\)$", last_line)
         if match:
             last_line = match.group(1)
 
-
         try:
             result = eval(last_line, environment)
 
             # In some cases, the result is a tuple of values. For example, when
             # the last line is `print("Hello", "World")`, the result is a tuple
             # of two strings. In this case, we want to return a string
             if isinstance(result, tuple):
                 result = " ".join([str(element) for element in result])
-
+            
             return result
-        except Exception:
-            return captured_output
+        except Exception as e:
+            raise e
+            # return captured_output
 
         
     def log(self, message: str):
         """Log a message"""
         self._logger.info(message)
         self._logs.append(message)
```

### Comparing `idoctorai-0.7.4/pandasai/constants.py` & `idoctorai-0.7.5/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/exceptions.py` & `idoctorai-0.7.5/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/helpers/_optional.py` & `idoctorai-0.7.5/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/helpers/anonymizer.py` & `idoctorai-0.7.5/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/helpers/cache.py` & `idoctorai-0.7.5/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/helpers/from_excel.py` & `idoctorai-0.7.5/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/helpers/notebook.py` & `idoctorai-0.7.5/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/helpers/save_chart.py` & `idoctorai-0.7.5/pandasai/helpers/save_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Helper functions to save charts to a file, if plt.show() is called."""
 import ast
 import logging
 import os
 from itertools import zip_longest
 from os.path import dirname
-from typing import Union
+from typing import Union, List
 
 import astor
 
 
 def compare_ast(
     node1: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
     node2: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
@@ -50,15 +50,15 @@
 
 
 def add_save_chart(
     code: str,
     folder_name: str,
     save_charts_path: str = None,
     print_save_dir: bool = True,
-) -> str:
+) -> List[str]:
     """
     Add line to code that save charts to a file, if plt.show() is called.
 
     Args:
         code (str): Code to add line to.
         folder_name (str): Name of folder to save charts to.
         save_charts_path (str): User Defined Path to save Charts
@@ -109,8 +109,9 @@
 
     chart_save_msg = f"Charts saving to: {chart_save_dir}"
     if print_save_dir:
         print(chart_save_msg)
     logging.info(chart_save_msg)
 
     new_tree = ast.Module(body=new_body)
-    return astor.to_source(new_tree).strip()
+    code = astor.to_source(new_tree).strip()
+    return [code, chart_save_path]
```

### Comparing `idoctorai-0.7.4/pandasai/helpers/shortcuts.py` & `idoctorai-0.7.5/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/langchain/__init__.py` & `idoctorai-0.7.5/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/azure_openai.py` & `idoctorai-0.7.5/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/base.py` & `idoctorai-0.7.5/pandasai/llm/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -242,14 +242,16 @@
       
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
     
     def langchain_input(self, value:str, history:list = None) -> str:
         response = self.langchain.__call__(value, history)
+
+        # response = "To check the data and choose a best regression model to do the regression analysis, you can start by importing the necessary libraries and reading in the dataframe df1:\n\n```python\nimport pandas as pd\nimport numpy as np\nimport matplotlib.pyplot as plt\nimport seaborn as sns\nfrom sklearn.linear_model import LinearRegression, Lasso, Ridge\nfrom sklearn.model_selection import train_test_split, cross_val_score\nfrom sklearn.metrics import r2_score, mean_squared_error\n\ndf1 = pd.read_csv('df1.csv')\n```\n\nFrom there, you can start by exploring the data and checking for any missing values:\n\n```python\ndf1.head()\ndf1.info()\ndf1.describe()\ndf1.isnull().sum()\n```\n\nNext, you can visualize the data to see if there are any trends or patterns:\n\n```python\nsns.pairplot(df1)\nplt.show()\n```\n\nAfter that, you can start building and comparing different regression models:\n\n```python\n# Split the data into training and test sets\nX_train, X_test, y_train, y_test = train_test_split(df1.drop('Daily Mean PM2.5 Concentration', axis=1),\n                                                    df1['Daily Mean PM2.5 Concentration'],\n                                                    test_size=0.2,\n                                                    random_state=42)\n\n# Fit the linear regression model and evaluate its performance\nlr = LinearRegression()\nlr.fit(X_train, y_train)\ny_pred = lr.predict(X_test)\nprint('Linear Regression R^2:', r2_score(y_test, y_pred))\nprint('Linear Regression RMSE:', np.sqrt(mean_squared_error(y_test, y_pred)))\n\n# Fit the Lasso regression model and evaluate its performance\nlasso = Lasso(alpha=0.1)\nlasso.fit(X_train, y_train)\ny_pred = lasso.predict(X_test)\nprint('Lasso Regression R^2:', r2_score(y_test, y_pred))\nprint('Lasso Regression RMSE:', np.sqrt(mean_squared_error(y_test, y_pred)))\n\n# Fit the Ridge regression model and evaluate its performance\nridge = Ridge(alpha=0.1)\nridge.fit(X_train, y_train)\ny_pred = ridge.predict(X_test)\nprint('Ridge Regression R^2:', r2_score(y_test, y_pred))\nprint('Ridge Regression RMSE:', np.sqrt(mean_squared_error(y_test, y_pred)))\n```\n\nBased on the R^2 and RMSE scores, you can choose the best regression model for your analysis."
         
         return response
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
```

### Comparing `idoctorai-0.7.4/pandasai/llm/fake.py` & `idoctorai-0.7.5/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/falcon.py` & `idoctorai-0.7.5/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/google_palm.py` & `idoctorai-0.7.5/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/langchain.py` & `idoctorai-0.7.5/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/model.py` & `idoctorai-0.7.5/pandasai/llm/model.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/open_assistant.py` & `idoctorai-0.7.5/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/openai.py` & `idoctorai-0.7.5/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/llm/starcoder.py` & `idoctorai-0.7.5/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/middlewares/base.py` & `idoctorai-0.7.5/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/middlewares/charts.py` & `idoctorai-0.7.5/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/middlewares/streamlit.py` & `idoctorai-0.7.5/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/prompts/base.py` & `idoctorai-0.7.5/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.7.5/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.7.5/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/prompts/generate_python_code.py` & `idoctorai-0.7.5/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.7.5/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.4/pyproject.toml` & `idoctorai-0.7.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.7.4"
+version = "0.7.5"
 description = "Idoctor AI is a Python library that integrates generative artificial intelligence capabilities into Pandas."
 authors = ["FH"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -13,15 +13,23 @@
 pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
 google-cloud-aiplatform = { version = "^1.26.1", optional = true }
-langchain = { version = "^0.0.199", optional = true}
+langchain = "^0.0.234"
+scikit-learn = "^1.2.2"
+numpy = "^1.17"
+seaborn = "^0.12.2"
+streamlit = "^1.23.1"
+plotly = "^5.14.1"
+statsmodels = "^0.14.0"
+ggplot = "^0.11.5"
+tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 ruff = "^0.0.220"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
```

