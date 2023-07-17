# Comparing `tmp/pyGitInfo-0.0.5.tar.gz` & `tmp/pyGitInfo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGitInfo-0.0.5.tar", last modified: Fri Jul 14 03:07:23 2023, max compression
+gzip compressed data, was "pyGitInfo-0.0.6.tar", last modified: Mon Jul 17 13:19:52 2023, max compression
```

## Comparing `pyGitInfo-0.0.5.tar` & `pyGitInfo-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-14 03:07:23.197049 pyGitInfo-0.0.5/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1180 2023-07-14 01:52:08.000000 pyGitInfo-0.0.5/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     4660 2023-07-14 03:07:23.197049 pyGitInfo-0.0.5/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     4084 2023-07-14 02:33:28.000000 pyGitInfo-0.0.5/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-14 03:07:23.193049 pyGitInfo-0.0.5/pyGitInfo/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       25 2023-07-14 01:52:08.000000 pyGitInfo-0.0.5/pyGitInfo/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    10758 2023-07-14 01:52:08.000000 pyGitInfo-0.0.5/pyGitInfo/pyGitInfo.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-14 03:07:23.197049 pyGitInfo-0.0.5/pyGitInfo.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     4660 2023-07-14 03:07:23.000000 pyGitInfo-0.0.5/pyGitInfo.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      235 2023-07-14 03:07:23.000000 pyGitInfo-0.0.5/pyGitInfo.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-07-14 03:07:23.000000 pyGitInfo-0.0.5/pyGitInfo.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       34 2023-07-14 03:07:23.000000 pyGitInfo-0.0.5/pyGitInfo.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-07-14 03:07:23.000000 pyGitInfo-0.0.5/pyGitInfo.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-07-14 03:07:23.197049 pyGitInfo-0.0.5/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      850 2023-07-14 03:03:18.000000 pyGitInfo-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:19:52.132859 pyGitInfo-0.0.6/
+-rw-rw-rw-   0        0        0     1199 2023-07-15 01:23:25.000000 pyGitInfo-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4785 2023-07-17 13:19:52.132859 pyGitInfo-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4197 2023-07-15 20:57:44.000000 pyGitInfo-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:19:52.119132 pyGitInfo-0.0.6/pyGitInfo/
+-rw-rw-rw-   0        0        0       26 2023-07-15 01:23:25.000000 pyGitInfo-0.0.6/pyGitInfo/__init__.py
+-rw-rw-rw-   0        0        0    11119 2023-07-15 01:23:25.000000 pyGitInfo-0.0.6/pyGitInfo/pyGitInfo.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:19:52.132859 pyGitInfo-0.0.6/pyGitInfo.egg-info/
+-rw-rw-rw-   0        0        0     4785 2023-07-17 13:19:52.000000 pyGitInfo-0.0.6/pyGitInfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-17 13:19:52.000000 pyGitInfo-0.0.6/pyGitInfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:19:52.000000 pyGitInfo-0.0.6/pyGitInfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-17 13:19:52.000000 pyGitInfo-0.0.6/pyGitInfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 13:19:52.000000 pyGitInfo-0.0.6/pyGitInfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:19:52.132859 pyGitInfo-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-07-17 13:16:39.000000 pyGitInfo-0.0.6/setup.py
```

### Comparing `pyGitInfo-0.0.5/LICENSE` & `pyGitInfo-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 Gabriel Rosa, Gabriel Zaranza, Catlen Cleane, Felipe Direito, Lucas Andrade, Rafael Kenji e Vinícius de Oliveira 
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+The MIT License (MIT)
+
+Copyright (c) 2023 Gabriel Rosa, Gabriel Zaranza, Catlen Cleane, Felipe Direito, Lucas Andrade, Rafael Kenji e Vinícius de Oliveira 
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pyGitInfo-0.0.5/PKG-INFO` & `pyGitInfo-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-Metadata-Version: 2.1
-Name: pyGitInfo
-Version: 0.0.5
-Summary: Analisador de repositórios do github
-Author: ['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira']
-Author-email: catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com
-License: MIT License
-Keywords: gitInfo,github,git,relatorio,reports,gitReports
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-### Library use
-
-After downloading and configuring the library, we can start using it.  
-
-First let's import the library into the project.  
-
-```python
-from pyGitInfo import *
-```  
-
-### Notes/Standardization  
-
-**Date:** The default format for passing dates is "month-day-year" Ex: "06-07-2023" is equivalent to June 07, 2023  
-
-### Functions and Returns  
-
-- **get_commits_by_user()**  
-  Allows you to search for commits by user, passing 3 strings as a parameter, the user's name (str), a start date and an end date.  
-
-  ```python
-  get_commits_by_user('name_user','date_init','date_end')
-  ```  
-  
-  This function returns _DataFrame_ from the _Pandas_ library or an error message  
-
-- **get_commits_users()**  
-  Allows you to search for commits from all contributors, passing as a parameter 2 strings that define the time range, a start date and an end date.  
-
-  ```python
-  get_commits_users('date_init','date_end')
-  ```  
-
-  This function returns _DataFrame_ from the _Pandas_ library  
-
-- **get_coAuthor()**  
-  Search all commits with Coauthor, passing as parameters 2 strings that define the time range, a start date and an end date.  
-
-  ```python
-  get_coAuthor('date_init','date_end')
-  ```  
-
-  This function returns a _DataFrame_ from the _Pandas_ library or an error message  
-
-- **issues_month()**  
-  This function verifies how many Issues were closed per month, within the stipulated period. The function receives 2 date strings as a parameter, the start and end date.
-
-  ```python
-  issues_month('date_init','date_end')
-  ```  
-
-  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
-
-- **calculate_commit_average()**  
-  Calculates the average commits across all contributors and shows who is above or below that average. You must pass the analysis period as a parameter with 2 strings representing the dates
-
-  ```python
-  calculate_commit_average('date_init','date_end')
-  ```  
-
-  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
-
-- **commit_data()**  
-  Searches for all commits on a specific day, the function receives a string with the desired date as a parameter.
-
-  ```python
-  commit_data('date')
-  ```  
-
-  The function generates a markdown file with the information
-
-- **commit_palavra()**  
-  Searches for all commits (within a time range) that have the desired word in their description. This function receives 3 strings as a parameter, the first with the 'word' to be searched for, and the 2 'dates' referring to the time interval
-
-  ```python
-  commit_palavra('palavra','date_init','date_end')
-  ```  
-
-  The function returns a _DataFrame_ from the _Pandas_ library or an error message  
-
-- **check_extension()**  
-  It does a search for the files that are being committed by each contributor and classifies them according to their extension. You must pass the time interval for the analysis (2 strings of 'date')
-
-  ```python
-  check_extension('date_init','date_end')
-  ```  
-
-  The function returns a variable with the content written in markdown format
-
-- **title_commits()**  
-  Searches all commit titles, by user, thus facilitating the visualization of what each contributor has done (Requires a time interval) 2 strings 'data'
-
-  ```python
-  title_commits('date_init','date_end')
-  ```  
-
-  The function returns a variable with the content written in markdown format  
-
-- **gerenate_report()**  
-  Combines the functions of commit with coauthor and overall average to generate a more complete report. The function receives as parameter 2 date strings with the time interval to be analyzed ('initial_date','final_date')
-
-  ```python
-  gerenate_report('date_init','date_end')
-  ```  
-
-  Generates a "gitInfo_report.md" markdown with information about commits with coauthor and the number of commits per user
-
-- **issues_open()**  
-  Searches all Issues that are open but have not yet been signed by anyone. It takes nothing as a parameter.
-
-  ```python
-  issues_open()
-  ```  
-
-  The function returns a variable with the content written in markdown format  
+Metadata-Version: 2.1
+Name: pyGitInfo
+Version: 0.0.6
+Summary: Analisador de repositórios do github
+Author: ['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira']
+Author-email: catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com
+License: MIT License
+Keywords: gitInfo,github,git,relatorio,reports,gitReports
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### Library use
+
+After downloading and configuring the library, we can start using it.  
+
+First let's import the library into the project.  
+
+```python
+from pyGitInfo import *
+```  
+
+### Notes/Standardization  
+
+**Date:** The default format for passing dates is "month-day-year" Ex: "06-07-2023" is equivalent to June 07, 2023  
+
+### Functions and Returns  
+
+- **get_commits_by_user()**  
+  Allows you to search for commits by user, passing 3 strings as a parameter, the user's name (str), a start date and an end date.  
+
+  ```python
+  get_commits_by_user('name_user','date_init','date_end')
+  ```  
+  
+  This function returns _DataFrame_ from the _Pandas_ library or an error message  
+
+- **get_commits_users()**  
+  Allows you to search for commits from all contributors, passing as a parameter 2 strings that define the time range, a start date and an end date.  
+
+  ```python
+  get_commits_users('date_init','date_end')
+  ```  
+
+  This function returns _DataFrame_ from the _Pandas_ library  
+
+- **get_coAuthor()**  
+  Search all commits with Coauthor, passing as parameters 2 strings that define the time range, a start date and an end date.  
+
+  ```python
+  get_coAuthor('date_init','date_end')
+  ```  
+
+  This function returns a _DataFrame_ from the _Pandas_ library or an error message  
+
+- **issues_month()**  
+  This function verifies how many Issues were closed per month, within the stipulated period. The function receives 2 date strings as a parameter, the start and end date.
+
+  ```python
+  issues_month('date_init','date_end')
+  ```  
+
+  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
+
+- **calculate_commit_average()**  
+  Calculates the average commits across all contributors and shows who is above or below that average. You must pass the analysis period as a parameter with 2 strings representing the dates
+
+  ```python
+  calculate_commit_average('date_init','date_end')
+  ```  
+
+  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
+
+- **commit_data()**  
+  Searches for all commits on a specific day, the function receives a string with the desired date as a parameter.
+
+  ```python
+  commit_data('date')
+  ```  
+
+  The function generates a markdown file with the information
+
+- **commit_palavra()**  
+  Searches for all commits (within a time range) that have the desired word in their description. This function receives 3 strings as a parameter, the first with the 'word' to be searched for, and the 2 'dates' referring to the time interval
+
+  ```python
+  commit_palavra('palavra','date_init','date_end')
+  ```  
+
+  The function returns a _DataFrame_ from the _Pandas_ library or an error message  
+
+- **check_extension()**  
+  It does a search for the files that are being committed by each contributor and classifies them according to their extension. You must pass the time interval for the analysis (2 strings of 'date')
+
+  ```python
+  check_extension('date_init','date_end')
+  ```  
+
+  The function returns a variable with the content written in markdown format
+
+- **title_commits()**  
+  Searches all commit titles, by user, thus facilitating the visualization of what each contributor has done (Requires a time interval) 2 strings 'data'
+
+  ```python
+  title_commits('date_init','date_end')
+  ```  
+
+  The function returns a variable with the content written in markdown format  
+
+- **gerenate_report()**  
+  Combines the functions of commit with coauthor and overall average to generate a more complete report. The function receives as parameter 2 date strings with the time interval to be analyzed ('initial_date','final_date')
+
+  ```python
+  gerenate_report('date_init','date_end')
+  ```  
+
+  Generates a "gitInfo_report.md" markdown with information about commits with coauthor and the number of commits per user
+
+- **issues_open()**  
+  Searches all Issues that are open but have not yet been signed by anyone. It takes nothing as a parameter.
+
+  ```python
+  issues_open()
+  ```  
+
+  The function returns a variable with the content written in markdown format
```

### Comparing `pyGitInfo-0.0.5/README.md` & `pyGitInfo-0.0.6/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-### Library use
-
-After downloading and configuring the library, we can start using it.  
-
-First let's import the library into the project.  
-
-```python
-from pyGitInfo import *
-```  
-
-### Notes/Standardization  
-
-**Date:** The default format for passing dates is "month-day-year" Ex: "06-07-2023" is equivalent to June 07, 2023  
-
-### Functions and Returns  
-
-- **get_commits_by_user()**  
-  Allows you to search for commits by user, passing 3 strings as a parameter, the user's name (str), a start date and an end date.  
-
-  ```python
-  get_commits_by_user('name_user','date_init','date_end')
-  ```  
-  
-  This function returns _DataFrame_ from the _Pandas_ library or an error message  
-
-- **get_commits_users()**  
-  Allows you to search for commits from all contributors, passing as a parameter 2 strings that define the time range, a start date and an end date.  
-
-  ```python
-  get_commits_users('date_init','date_end')
-  ```  
-
-  This function returns _DataFrame_ from the _Pandas_ library  
-
-- **get_coAuthor()**  
-  Search all commits with Coauthor, passing as parameters 2 strings that define the time range, a start date and an end date.  
-
-  ```python
-  get_coAuthor('date_init','date_end')
-  ```  
-
-  This function returns a _DataFrame_ from the _Pandas_ library or an error message  
-
-- **issues_month()**  
-  This function verifies how many Issues were closed per month, within the stipulated period. The function receives 2 date strings as a parameter, the start and end date.
-
-  ```python
-  issues_month('date_init','date_end')
-  ```  
-
-  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
-
-- **calculate_commit_average()**  
-  Calculates the average commits across all contributors and shows who is above or below that average. You must pass the analysis period as a parameter with 2 strings representing the dates
-
-  ```python
-  calculate_commit_average('date_init','date_end')
-  ```  
-
-  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
-
-- **commit_data()**  
-  Searches for all commits on a specific day, the function receives a string with the desired date as a parameter.
-
-  ```python
-  commit_data('date')
-  ```  
-
-  The function generates a markdown file with the information
-
-- **commit_palavra()**  
-  Searches for all commits (within a time range) that have the desired word in their description. This function receives 3 strings as a parameter, the first with the 'word' to be searched for, and the 2 'dates' referring to the time interval
-
-  ```python
-  commit_palavra('palavra','date_init','date_end')
-  ```  
-
-  The function returns a _DataFrame_ from the _Pandas_ library or an error message  
-
-- **check_extension()**  
-  It does a search for the files that are being committed by each contributor and classifies them according to their extension. You must pass the time interval for the analysis (2 strings of 'date')
-
-  ```python
-  check_extension('date_init','date_end')
-  ```  
-
-  The function returns a variable with the content written in markdown format
-
-- **title_commits()**  
-  Searches all commit titles, by user, thus facilitating the visualization of what each contributor has done (Requires a time interval) 2 strings 'data'
-
-  ```python
-  title_commits('date_init','date_end')
-  ```  
-
-  The function returns a variable with the content written in markdown format  
-
-- **gerenate_report()**  
-  Combines the functions of commit with coauthor and overall average to generate a more complete report. The function receives as parameter 2 date strings with the time interval to be analyzed ('initial_date','final_date')
-
-  ```python
-  gerenate_report('date_init','date_end')
-  ```  
-
-  Generates a "gitInfo_report.md" markdown with information about commits with coauthor and the number of commits per user
-
-- **issues_open()**  
-  Searches all Issues that are open but have not yet been signed by anyone. It takes nothing as a parameter.
-
-  ```python
-  issues_open()
-  ```  
-
+### Library use
+
+After downloading and configuring the library, we can start using it.  
+
+First let's import the library into the project.  
+
+```python
+from pyGitInfo import *
+```  
+
+### Notes/Standardization  
+
+**Date:** The default format for passing dates is "month-day-year" Ex: "06-07-2023" is equivalent to June 07, 2023  
+
+### Functions and Returns  
+
+- **get_commits_by_user()**  
+  Allows you to search for commits by user, passing 3 strings as a parameter, the user's name (str), a start date and an end date.  
+
+  ```python
+  get_commits_by_user('name_user','date_init','date_end')
+  ```  
+  
+  This function returns _DataFrame_ from the _Pandas_ library or an error message  
+
+- **get_commits_users()**  
+  Allows you to search for commits from all contributors, passing as a parameter 2 strings that define the time range, a start date and an end date.  
+
+  ```python
+  get_commits_users('date_init','date_end')
+  ```  
+
+  This function returns _DataFrame_ from the _Pandas_ library  
+
+- **get_coAuthor()**  
+  Search all commits with Coauthor, passing as parameters 2 strings that define the time range, a start date and an end date.  
+
+  ```python
+  get_coAuthor('date_init','date_end')
+  ```  
+
+  This function returns a _DataFrame_ from the _Pandas_ library or an error message  
+
+- **issues_month()**  
+  This function verifies how many Issues were closed per month, within the stipulated period. The function receives 2 date strings as a parameter, the start and end date.
+
+  ```python
+  issues_month('date_init','date_end')
+  ```  
+
+  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
+
+- **calculate_commit_average()**  
+  Calculates the average commits across all contributors and shows who is above or below that average. You must pass the analysis period as a parameter with 2 strings representing the dates
+
+  ```python
+  calculate_commit_average('date_init','date_end')
+  ```  
+
+  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
+
+- **commit_data()**  
+  Searches for all commits on a specific day, the function receives a string with the desired date as a parameter.
+
+  ```python
+  commit_data('date')
+  ```  
+
+  The function generates a markdown file with the information
+
+- **commit_palavra()**  
+  Searches for all commits (within a time range) that have the desired word in their description. This function receives 3 strings as a parameter, the first with the 'word' to be searched for, and the 2 'dates' referring to the time interval
+
+  ```python
+  commit_palavra('palavra','date_init','date_end')
+  ```  
+
+  The function returns a _DataFrame_ from the _Pandas_ library or an error message  
+
+- **check_extension()**  
+  It does a search for the files that are being committed by each contributor and classifies them according to their extension. You must pass the time interval for the analysis (2 strings of 'date')
+
+  ```python
+  check_extension('date_init','date_end')
+  ```  
+
+  The function returns a variable with the content written in markdown format
+
+- **title_commits()**  
+  Searches all commit titles, by user, thus facilitating the visualization of what each contributor has done (Requires a time interval) 2 strings 'data'
+
+  ```python
+  title_commits('date_init','date_end')
+  ```  
+
+  The function returns a variable with the content written in markdown format  
+
+- **gerenate_report()**  
+  Combines the functions of commit with coauthor and overall average to generate a more complete report. The function receives as parameter 2 date strings with the time interval to be analyzed ('initial_date','final_date')
+
+  ```python
+  gerenate_report('date_init','date_end')
+  ```  
+
+  Generates a "gitInfo_report.md" markdown with information about commits with coauthor and the number of commits per user
+
+- **issues_open()**  
+  Searches all Issues that are open but have not yet been signed by anyone. It takes nothing as a parameter.
+
+  ```python
+  issues_open()
+  ```  
+
   The function returns a variable with the content written in markdown format
```

### Comparing `pyGitInfo-0.0.5/pyGitInfo/pyGitInfo.py` & `pyGitInfo-0.0.6/pyGitInfo/pyGitInfo.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,362 +1,362 @@
-from collections import defaultdict
-import pandas as pd
-import os
-import io
-import datetime
-import matplotlib.pyplot as plt
-from datetime import datetime
-from dotenv import load_dotenv
-from github import Github
-
-load_dotenv()
-
-github_token = os.getenv('GITHUB_TOKEN')
-
-g=Github(github_token)
-
-repo = os.getenv('REPO')
-
-repo = g.get_repo(repo)
-
-
-def get_commits_by_user(user: str, start_date: str, end_date: str):
-    hashes = []
-    messages = []
-
-    commits = repo.get_commits()
-    for commit in commits:
-        commit_date = commit.commit.author.date
-        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-        if commit_date_str >= start_date and commit_date_str <= end_date:
-            if commit.author.login.lower() == user.lower():
-                messages.append(commit.commit.message)
-                hashes.append(commit.sha[:6])
-
-    df = pd.DataFrame({"Message":messages}, index=hashes)
-
-    if df.empty is False:
-        return df
-    else:
-        msg_error = "No commits with this user"
-        return msg_error
-
-def get_commits_users(start_date: str, end_date: str):
-
-    commit_users = []
-    commits = repo.get_commits()
-    for commit in commits:
-        commit_date = commit.commit.author.date
-        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-        if commit_date_str >= start_date and commit_date_str <= end_date:
-            author = commit.author.login
-            if author in commit_users:
-             continue
-
-            commit_users.append(author)
-
-    df = pd.DataFrame({"Users": commit_users})
-    return df
-
-def get_coAuthor(start_date: str, end_date: str):
-    coauthors = []
-    hashes = []
-    authors = []
-
-    commits = repo.get_commits()
-
-    for commit in commits:
-        commit_date = commit.commit.author.date
-        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-        if commit_date_str >= start_date and commit_date_str <= end_date:
-            commit_message = commit.commit.message
-
-            if 'Co-authored-by:' in commit_message:
-                hashes.append(commit.commit.sha[:6])
-                authors.append(commit.commit.author.name)
-
-                lines = commit_message.splitlines()
-                aux=[]
-                for row in lines:
-                    if row.startswith('Co-authored-by:'):
-                        aux.append(row[16:].strip().split('<')[0])
-                coauthors.append(aux)
-
-    df = pd.DataFrame({"authors": authors,"co-authors":coauthors}, index=hashes)
-
-    if df.empty is False:
-        return df
-    else:
-        msg = "0 commits with Coauthors"
-        return msg
-
-
-def issues_month(start_date: str, end_date: str):
-
-    months_list = pd.period_range(start =start_date,end=end_date, freq='M')
-    months_list = [month.strftime("%b-%Y") for month in months_list]
-
-    issues = repo.get_issues(state='closed')
-
-    count=[]
-
-
-    for month in months_list:
-        counter=0
-        for issue in issues:
-            if issue.pull_request is None and issue.closed_at.strftime("%b-%Y") == month:
-                counter+=1
-        count.append(counter)
-
-    df = pd.DataFrame({"num_issues": count},index=months_list)
-
-    plt.bar(months_list, df['num_issues'])
-    plt.xlabel('Months')
-    plt.ylabel('Issues')
-    plt.title('Issues per month')
-    plt.yticks(range(0,max(df['num_issues']+1)))
-    plt.xticks(rotation=13)
-    plt.savefig('closed_issues.png', format='png')
-
-    return df
-
-def calculate_commit_average(start_date: str, end_date: str):
-
-    commits = repo.get_commits()
-
-    commits_count = defaultdict(int)
-
-    for commit in commits:
-        commit_date = commit.commit.author.date
-        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-        if commit_date_str >= start_date and commit_date_str <= end_date:
-            author = commit.author
-            name = author.login if author else "Unknown"
-
-            commits_count[name] += 1
-
-
-    total_commits = sum(commits_count.values())
-    count_user = len(commits_count)
-
-    average_total = total_commits / count_user
-
-    data = {'Author': [], 'Commits': []}
-
-    for author, num_commits in commits_count.items():
-        data['Author'].append(author)
-        data['Commits'].append(num_commits)
-
-    df = pd.DataFrame(data)
-    df = df.sort_values(by='Commits', ascending=False)
-
-    df['Average'] = average_total 
-
-    plt.bar(df['Author'], df['Commits'])
-    plt.axhline(y=average_total, color='r', linestyle='-', label='Average')
-    plt.xlabel('Author')
-    plt.ylabel('Commits')
-    plt.title('Commits per Author')
-    plt.legend()
-    plt.xticks(rotation=13)
-    plt.savefig('commit_average.png', format='png')
-
-    return df
-
-def commit_data(date: str):
-    hashes = []
-    messages = []
-    authors = []
-
-    commits = repo.get_commits()
-
-    for commit in commits:
-        commit_date = commit.commit.author.date
-        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-
-        if commit_date_str == date:
-            hashes.append(commit.sha[:6])
-            authors.append(commit.commit.author.name)
-            messages.append(commit.commit.message)
-
-    # Criar o arquivo Markdown
-    with io.open("commit_data.md", "w", encoding="utf-8") as file:
-        file.write("# Commits from day {}\n\n".format(date))
-
-        if not hashes:
-            file.write("There were no commits that day.\n")
-        else:
-            for i in range(len(hashes)):
-                file.write("## Commit {}\n\n".format(i+1))
-                file.write("- Hash: {}\n".format(hashes[i]))
-                file.write("- Author: {}\n".format(authors[i]))
-                file.write("- Message: {}\n\n".format(messages[i]))
-
-
-def commit_palavra(string: str, start_date: str, end_date: str):
-
-    hashes = []
-    messages = []
-    authors = []
-
-    commits = repo.get_commits()
-
-    for commit in commits:
-        commit_date = commit.commit.author.date
-        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-        if commit_date_str >= start_date and commit_date_str <= end_date:
-
-            commit_message = commit.commit.message
-
-            if string.lower() in commit_message.lower():
-
-                hashes.append(commit.sha[:6])
-                authors.append(commit.commit.author.name)
-                messages.append(commit.commit.message)
-
-    df = pd.DataFrame({"message":messages, "author": authors}, index=hashes)
-
-    if df.empty is False:
-        return df
-    else:
-        msg = "No commits with this word"
-        return msg
-
-def check_extension(start_date: str, end_date: str):
-    try:
-        extension_by_author = defaultdict(lambda: defaultdict(list))
-
-        commits = repo.get_commits()
-
-        for commit in commits:
-            commit_date = commit.commit.author.date
-            commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-            if commit_date_str >= start_date and commit_date_str <= end_date:
-                author = commit.author.login
-                file_modify = commit.files
-
-                for file in file_modify:
-                    extension = file.filename.split('.')[-1]
-                    filename = file.filename
-
-                    extension_by_author[author][extension].append(filename)
-
-        content = '## File Extensions Report by Author\n\n'
-
-        for author, extensions in extension_by_author.items():
-            content += f'## Author: {author} \n\n'
-            content += '| Extension / Files |\n'
-            content += '| -------- | \n'
-            for extension, files in extensions.items():
-                file_list = '| \n'.join(files)
-                content += f'| **{extension}** | \n'
-                content += f' {file_list} | \n'
-            content += "\n"
-
-    except Exception as e:
-        print(f'Error: {e}')
-
-    return content
-
-def title_commits(start_date: str, end_date: str):
-
-    commits = repo.get_commits()
-
-    commit_titles = defaultdict(lambda: defaultdict(list))
-
-    for commit in commits:
-        commit_date = commit.commit.author.date
-        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
-        if commit_date_str >= start_date and commit_date_str <= end_date:
-            author = commit.author
-            if author:
-                author_name = author.login
-            else:
-                author_name = 'Unknown'
-
-            commit_title = commit.commit.message.splitlines()[0]
-
-            if author_name in commit_titles:
-                commit_titles[author_name].append(commit_title)
-            else:
-                commit_titles[author_name] = [commit_title]
-
-    content = '#File Title Commits\n\n'
-    for author, titles in commit_titles.items():
-        content += f'## User: {author}\n'
-        content += f'### Commit title:\n'
-        for title in titles:
-            content += f'- {title}\n'
-        content += '\n'
-
-    return content
-
-
-def generate_report(start_date: str, end_date: str):
-    content = '## Report from ' + start_date + ' - ' + end_date + '\n\n'
-
-    content += check_extension(start_date, end_date)
-    content += '\n\n'
-
-    content += '## List of commits with coauthor\n\n'
-
-    coaut = get_coAuthor(start_date, end_date)
-
-    content += '| Hash | Author | Coauthor |\n'
-    content += '|------|--------|----------|\n'
-
-    for index, row in coaut.iterrows():
-        content += f'|{index}'
-        for columm, value in row.items():
-            content += f'|{value}'
-            nothing = {columm}
-        content += '|\n'
-
-    content += '\n\n'
-
-    content += '## Commits per person and general avarage\n\n'
-    commits = calculate_commit_average(start_date, end_date)
-    graph_path = 'commit_average.png'
-
-    content += '| Index | Author | Commits | Averege |\n'
-    content += '|-------|--------|---------|---------|\n'
-
-    for index, row in commits.iterrows():
-        content += f'|{index}'
-        for columm, value in row.items():
-            content += f'|{value}'
-            nothing = {columm}
-        content += '|\n'
-
-    content += '\n\n'
-
-    content += f'![Commit Average Graph]({graph_path})\n\n'
-    output = 'gitInfo_report.md'
-
-    with open(output, 'w', encoding='utf-8') as f:
-
-        f.write(content)
-
-
-def issues_open():
-    issues = repo.get_issues(state='open')
-
-    content = '## Issues opened assigned\n'
-
-    content += '| Title | Number |\n'
-    content += '|-------|--------|\n'
-
-    for issue in issues:
-        if issue.assignee:
-            content += f'|{issue.title}|{issue.number}|\n'
-
-    content += '\n\n'
-    content += '## Issues opened not assigned\n'
-
-    content += '| Title | Number |\n'
-    content += '|-------|--------|\n'
-
-    for issue in issues:
-        if not issue.assignee:
-            content += f'|{issue.title}|{issue.number}|\n'
-
+from collections import defaultdict
+import pandas as pd
+import os
+import io
+import datetime
+import matplotlib.pyplot as plt
+from datetime import datetime
+from dotenv import load_dotenv
+from github import Github
+
+load_dotenv()
+
+github_token = os.getenv('GITHUB_TOKEN')
+
+g=Github(github_token)
+
+repo = os.getenv('REPO')
+
+repo = g.get_repo(repo)
+
+
+def get_commits_by_user(user: str, start_date: str, end_date: str):
+    hashes = []
+    messages = []
+
+    commits = repo.get_commits()
+    for commit in commits:
+        commit_date = commit.commit.author.date
+        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+        if commit_date_str >= start_date and commit_date_str <= end_date:
+            if commit.author.login.lower() == user.lower():
+                messages.append(commit.commit.message)
+                hashes.append(commit.sha[:6])
+
+    df = pd.DataFrame({"Message":messages}, index=hashes)
+
+    if df.empty is False:
+        return df
+    else:
+        msg_error = "No commits with this user"
+        return msg_error
+
+def get_commits_users(start_date: str, end_date: str):
+
+    commit_users = []
+    commits = repo.get_commits()
+    for commit in commits:
+        commit_date = commit.commit.author.date
+        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+        if commit_date_str >= start_date and commit_date_str <= end_date:
+            author = commit.author.login
+            if author in commit_users:
+             continue
+
+            commit_users.append(author)
+
+    df = pd.DataFrame({"Users": commit_users})
+    return df
+
+def get_coAuthor(start_date: str, end_date: str):
+    coauthors = []
+    hashes = []
+    authors = []
+
+    commits = repo.get_commits()
+
+    for commit in commits:
+        commit_date = commit.commit.author.date
+        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+        if commit_date_str >= start_date and commit_date_str <= end_date:
+            commit_message = commit.commit.message
+
+            if 'Co-authored-by:' in commit_message:
+                hashes.append(commit.commit.sha[:6])
+                authors.append(commit.commit.author.name)
+
+                lines = commit_message.splitlines()
+                aux=[]
+                for row in lines:
+                    if row.startswith('Co-authored-by:'):
+                        aux.append(row[16:].strip().split('<')[0])
+                coauthors.append(aux)
+
+    df = pd.DataFrame({"authors": authors,"co-authors":coauthors}, index=hashes)
+
+    if df.empty is False:
+        return df
+    else:
+        msg = "0 commits with Coauthors"
+        return msg
+
+
+def issues_month(start_date: str, end_date: str):
+
+    months_list = pd.period_range(start =start_date,end=end_date, freq='M')
+    months_list = [month.strftime("%b-%Y") for month in months_list]
+
+    issues = repo.get_issues(state='closed')
+
+    count=[]
+
+
+    for month in months_list:
+        counter=0
+        for issue in issues:
+            if issue.pull_request is None and issue.closed_at.strftime("%b-%Y") == month:
+                counter+=1
+        count.append(counter)
+
+    df = pd.DataFrame({"num_issues": count},index=months_list)
+
+    plt.bar(months_list, df['num_issues'])
+    plt.xlabel('Months')
+    plt.ylabel('Issues')
+    plt.title('Issues per month')
+    plt.yticks(range(0,max(df['num_issues']+1)))
+    plt.xticks(rotation=13)
+    plt.savefig('closed_issues.png', format='png')
+
+    return df
+
+def calculate_commit_average(start_date: str, end_date: str):
+
+    commits = repo.get_commits()
+
+    commits_count = defaultdict(int)
+
+    for commit in commits:
+        commit_date = commit.commit.author.date
+        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+        if commit_date_str >= start_date and commit_date_str <= end_date:
+            author = commit.author
+            name = author.login if author else "Unknown"
+
+            commits_count[name] += 1
+
+
+    total_commits = sum(commits_count.values())
+    count_user = len(commits_count)
+
+    average_total = total_commits / count_user
+
+    data = {'Author': [], 'Commits': []}
+
+    for author, num_commits in commits_count.items():
+        data['Author'].append(author)
+        data['Commits'].append(num_commits)
+
+    df = pd.DataFrame(data)
+    df = df.sort_values(by='Commits', ascending=False)
+
+    df['Average'] = average_total 
+
+    plt.bar(df['Author'], df['Commits'])
+    plt.axhline(y=average_total, color='r', linestyle='-', label='Average')
+    plt.xlabel('Author')
+    plt.ylabel('Commits')
+    plt.title('Commits per Author')
+    plt.legend()
+    plt.xticks(rotation=13)
+    plt.savefig('commit_average.png', format='png')
+
+    return df
+
+def commit_data(date: str):
+    hashes = []
+    messages = []
+    authors = []
+
+    commits = repo.get_commits()
+
+    for commit in commits:
+        commit_date = commit.commit.author.date
+        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+
+        if commit_date_str == date:
+            hashes.append(commit.sha[:6])
+            authors.append(commit.commit.author.name)
+            messages.append(commit.commit.message)
+
+    # Criar o arquivo Markdown
+    with io.open("commit_data.md", "w", encoding="utf-8") as file:
+        file.write("# Commits from day {}\n\n".format(date))
+
+        if not hashes:
+            file.write("There were no commits that day.\n")
+        else:
+            for i in range(len(hashes)):
+                file.write("## Commit {}\n\n".format(i+1))
+                file.write("- Hash: {}\n".format(hashes[i]))
+                file.write("- Author: {}\n".format(authors[i]))
+                file.write("- Message: {}\n\n".format(messages[i]))
+
+
+def commit_palavra(string: str, start_date: str, end_date: str):
+
+    hashes = []
+    messages = []
+    authors = []
+
+    commits = repo.get_commits()
+
+    for commit in commits:
+        commit_date = commit.commit.author.date
+        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+        if commit_date_str >= start_date and commit_date_str <= end_date:
+
+            commit_message = commit.commit.message
+
+            if string.lower() in commit_message.lower():
+
+                hashes.append(commit.sha[:6])
+                authors.append(commit.commit.author.name)
+                messages.append(commit.commit.message)
+
+    df = pd.DataFrame({"message":messages, "author": authors}, index=hashes)
+
+    if df.empty is False:
+        return df
+    else:
+        msg = "No commits with this word"
+        return msg
+
+def check_extension(start_date: str, end_date: str):
+    try:
+        extension_by_author = defaultdict(lambda: defaultdict(list))
+
+        commits = repo.get_commits()
+
+        for commit in commits:
+            commit_date = commit.commit.author.date
+            commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+            if commit_date_str >= start_date and commit_date_str <= end_date:
+                author = commit.author.login
+                file_modify = commit.files
+
+                for file in file_modify:
+                    extension = file.filename.split('.')[-1]
+                    filename = file.filename
+
+                    extension_by_author[author][extension].append(filename)
+
+        content = '## File Extensions Report by Author\n\n'
+
+        for author, extensions in extension_by_author.items():
+            content += f'## Author: {author} \n\n'
+            content += '| Extension / Files |\n'
+            content += '| -------- | \n'
+            for extension, files in extensions.items():
+                file_list = '| \n'.join(files)
+                content += f'| **{extension}** | \n'
+                content += f' {file_list} | \n'
+            content += "\n"
+
+    except Exception as e:
+        print(f'Error: {e}')
+
+    return content
+
+def title_commits(start_date: str, end_date: str):
+
+    commits = repo.get_commits()
+
+    commit_titles = defaultdict(lambda: defaultdict(list))
+
+    for commit in commits:
+        commit_date = commit.commit.author.date
+        commit_date_str = datetime.strftime(commit_date, "%m-%d-%Y")
+        if commit_date_str >= start_date and commit_date_str <= end_date:
+            author = commit.author
+            if author:
+                author_name = author.login
+            else:
+                author_name = 'Unknown'
+
+            commit_title = commit.commit.message.splitlines()[0]
+
+            if author_name in commit_titles:
+                commit_titles[author_name].append(commit_title)
+            else:
+                commit_titles[author_name] = [commit_title]
+
+    content = '#File Title Commits\n\n'
+    for author, titles in commit_titles.items():
+        content += f'## User: {author}\n'
+        content += f'### Commit title:\n'
+        for title in titles:
+            content += f'- {title}\n'
+        content += '\n'
+
+    return content
+
+
+def generate_report(start_date: str, end_date: str):
+    content = '## Report from ' + start_date + ' - ' + end_date + '\n\n'
+
+    content += check_extension(start_date, end_date)
+    content += '\n\n'
+
+    content += '## List of commits with coauthor\n\n'
+
+    coaut = get_coAuthor(start_date, end_date)
+
+    content += '| Hash | Author | Coauthor |\n'
+    content += '|------|--------|----------|\n'
+
+    for index, row in coaut.iterrows():
+        content += f'|{index}'
+        for columm, value in row.items():
+            content += f'|{value}'
+            nothing = {columm}
+        content += '|\n'
+
+    content += '\n\n'
+
+    content += '## Commits per person and general avarage\n\n'
+    commits = calculate_commit_average(start_date, end_date)
+    graph_path = 'commit_average.png'
+
+    content += '| Index | Author | Commits | Averege |\n'
+    content += '|-------|--------|---------|---------|\n'
+
+    for index, row in commits.iterrows():
+        content += f'|{index}'
+        for columm, value in row.items():
+            content += f'|{value}'
+            nothing = {columm}
+        content += '|\n'
+
+    content += '\n\n'
+
+    content += f'![Commit Average Graph]({graph_path})\n\n'
+    output = 'gitInfo_report.md'
+
+    with open(output, 'w', encoding='utf-8') as f:
+
+        f.write(content)
+
+
+def issues_open():
+    issues = repo.get_issues(state='open')
+
+    content = '## Issues opened assigned\n'
+
+    content += '| Title | Number |\n'
+    content += '|-------|--------|\n'
+
+    for issue in issues:
+        if issue.assignee:
+            content += f'|{issue.title}|{issue.number}|\n'
+
+    content += '\n\n'
+    content += '## Issues opened not assigned\n'
+
+    content += '| Title | Number |\n'
+    content += '|-------|--------|\n'
+
+    for issue in issues:
+        if not issue.assignee:
+            content += f'|{issue.title}|{issue.number}|\n'
+
     return content
```

### Comparing `pyGitInfo-0.0.5/pyGitInfo.egg-info/PKG-INFO` & `pyGitInfo-0.0.6/pyGitInfo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-Metadata-Version: 2.1
-Name: pyGitInfo
-Version: 0.0.5
-Summary: Analisador de repositórios do github
-Author: ['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira']
-Author-email: catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com
-License: MIT License
-Keywords: gitInfo,github,git,relatorio,reports,gitReports
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-### Library use
-
-After downloading and configuring the library, we can start using it.  
-
-First let's import the library into the project.  
-
-```python
-from pyGitInfo import *
-```  
-
-### Notes/Standardization  
-
-**Date:** The default format for passing dates is "month-day-year" Ex: "06-07-2023" is equivalent to June 07, 2023  
-
-### Functions and Returns  
-
-- **get_commits_by_user()**  
-  Allows you to search for commits by user, passing 3 strings as a parameter, the user's name (str), a start date and an end date.  
-
-  ```python
-  get_commits_by_user('name_user','date_init','date_end')
-  ```  
-  
-  This function returns _DataFrame_ from the _Pandas_ library or an error message  
-
-- **get_commits_users()**  
-  Allows you to search for commits from all contributors, passing as a parameter 2 strings that define the time range, a start date and an end date.  
-
-  ```python
-  get_commits_users('date_init','date_end')
-  ```  
-
-  This function returns _DataFrame_ from the _Pandas_ library  
-
-- **get_coAuthor()**  
-  Search all commits with Coauthor, passing as parameters 2 strings that define the time range, a start date and an end date.  
-
-  ```python
-  get_coAuthor('date_init','date_end')
-  ```  
-
-  This function returns a _DataFrame_ from the _Pandas_ library or an error message  
-
-- **issues_month()**  
-  This function verifies how many Issues were closed per month, within the stipulated period. The function receives 2 date strings as a parameter, the start and end date.
-
-  ```python
-  issues_month('date_init','date_end')
-  ```  
-
-  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
-
-- **calculate_commit_average()**  
-  Calculates the average commits across all contributors and shows who is above or below that average. You must pass the analysis period as a parameter with 2 strings representing the dates
-
-  ```python
-  calculate_commit_average('date_init','date_end')
-  ```  
-
-  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
-
-- **commit_data()**  
-  Searches for all commits on a specific day, the function receives a string with the desired date as a parameter.
-
-  ```python
-  commit_data('date')
-  ```  
-
-  The function generates a markdown file with the information
-
-- **commit_palavra()**  
-  Searches for all commits (within a time range) that have the desired word in their description. This function receives 3 strings as a parameter, the first with the 'word' to be searched for, and the 2 'dates' referring to the time interval
-
-  ```python
-  commit_palavra('palavra','date_init','date_end')
-  ```  
-
-  The function returns a _DataFrame_ from the _Pandas_ library or an error message  
-
-- **check_extension()**  
-  It does a search for the files that are being committed by each contributor and classifies them according to their extension. You must pass the time interval for the analysis (2 strings of 'date')
-
-  ```python
-  check_extension('date_init','date_end')
-  ```  
-
-  The function returns a variable with the content written in markdown format
-
-- **title_commits()**  
-  Searches all commit titles, by user, thus facilitating the visualization of what each contributor has done (Requires a time interval) 2 strings 'data'
-
-  ```python
-  title_commits('date_init','date_end')
-  ```  
-
-  The function returns a variable with the content written in markdown format  
-
-- **gerenate_report()**  
-  Combines the functions of commit with coauthor and overall average to generate a more complete report. The function receives as parameter 2 date strings with the time interval to be analyzed ('initial_date','final_date')
-
-  ```python
-  gerenate_report('date_init','date_end')
-  ```  
-
-  Generates a "gitInfo_report.md" markdown with information about commits with coauthor and the number of commits per user
-
-- **issues_open()**  
-  Searches all Issues that are open but have not yet been signed by anyone. It takes nothing as a parameter.
-
-  ```python
-  issues_open()
-  ```  
-
-  The function returns a variable with the content written in markdown format  
+Metadata-Version: 2.1
+Name: pyGitInfo
+Version: 0.0.6
+Summary: Analisador de repositórios do github
+Author: ['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira']
+Author-email: catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com
+License: MIT License
+Keywords: gitInfo,github,git,relatorio,reports,gitReports
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### Library use
+
+After downloading and configuring the library, we can start using it.  
+
+First let's import the library into the project.  
+
+```python
+from pyGitInfo import *
+```  
+
+### Notes/Standardization  
+
+**Date:** The default format for passing dates is "month-day-year" Ex: "06-07-2023" is equivalent to June 07, 2023  
+
+### Functions and Returns  
+
+- **get_commits_by_user()**  
+  Allows you to search for commits by user, passing 3 strings as a parameter, the user's name (str), a start date and an end date.  
+
+  ```python
+  get_commits_by_user('name_user','date_init','date_end')
+  ```  
+  
+  This function returns _DataFrame_ from the _Pandas_ library or an error message  
+
+- **get_commits_users()**  
+  Allows you to search for commits from all contributors, passing as a parameter 2 strings that define the time range, a start date and an end date.  
+
+  ```python
+  get_commits_users('date_init','date_end')
+  ```  
+
+  This function returns _DataFrame_ from the _Pandas_ library  
+
+- **get_coAuthor()**  
+  Search all commits with Coauthor, passing as parameters 2 strings that define the time range, a start date and an end date.  
+
+  ```python
+  get_coAuthor('date_init','date_end')
+  ```  
+
+  This function returns a _DataFrame_ from the _Pandas_ library or an error message  
+
+- **issues_month()**  
+  This function verifies how many Issues were closed per month, within the stipulated period. The function receives 2 date strings as a parameter, the start and end date.
+
+  ```python
+  issues_month('date_init','date_end')
+  ```  
+
+  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
+
+- **calculate_commit_average()**  
+  Calculates the average commits across all contributors and shows who is above or below that average. You must pass the analysis period as a parameter with 2 strings representing the dates
+
+  ```python
+  calculate_commit_average('date_init','date_end')
+  ```  
+
+  The function returns _DataFrame_ from the _Pandas_ library and also generates a png graphic
+
+- **commit_data()**  
+  Searches for all commits on a specific day, the function receives a string with the desired date as a parameter.
+
+  ```python
+  commit_data('date')
+  ```  
+
+  The function generates a markdown file with the information
+
+- **commit_palavra()**  
+  Searches for all commits (within a time range) that have the desired word in their description. This function receives 3 strings as a parameter, the first with the 'word' to be searched for, and the 2 'dates' referring to the time interval
+
+  ```python
+  commit_palavra('palavra','date_init','date_end')
+  ```  
+
+  The function returns a _DataFrame_ from the _Pandas_ library or an error message  
+
+- **check_extension()**  
+  It does a search for the files that are being committed by each contributor and classifies them according to their extension. You must pass the time interval for the analysis (2 strings of 'date')
+
+  ```python
+  check_extension('date_init','date_end')
+  ```  
+
+  The function returns a variable with the content written in markdown format
+
+- **title_commits()**  
+  Searches all commit titles, by user, thus facilitating the visualization of what each contributor has done (Requires a time interval) 2 strings 'data'
+
+  ```python
+  title_commits('date_init','date_end')
+  ```  
+
+  The function returns a variable with the content written in markdown format  
+
+- **gerenate_report()**  
+  Combines the functions of commit with coauthor and overall average to generate a more complete report. The function receives as parameter 2 date strings with the time interval to be analyzed ('initial_date','final_date')
+
+  ```python
+  gerenate_report('date_init','date_end')
+  ```  
+
+  Generates a "gitInfo_report.md" markdown with information about commits with coauthor and the number of commits per user
+
+- **issues_open()**  
+  Searches all Issues that are open but have not yet been signed by anyone. It takes nothing as a parameter.
+
+  ```python
+  issues_open()
+  ```  
+
+  The function returns a variable with the content written in markdown format
```

### Comparing `pyGitInfo-0.0.5/setup.py` & `pyGitInfo-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup
-
-from setuptools import setup
-
-with open("README.md", "r") as arq:
-    readme = arq.read()
-
-setup(name='pyGitInfo',
-    version='0.0.5',
-    license='MIT License',
-    author=['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira'],
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    author_email='catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com',
-    keywords=["gitInfo", "github", "git", "relatorio", "reports", "gitReports"],
-    description=u'Analisador de repositórios do github',
-    packages=['pyGitInfo'],
-    install_requires=["pandas>=1.4.0", "matplotlib", "pygithub"],)
+from setuptools import setup
+
+from setuptools import setup
+
+with open("README.md", "r") as arq:
+    readme = arq.read()
+
+setup(name='pyGitInfo',
+    version='0.0.6',
+    license='MIT License',
+    author=['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira'],
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    author_email='catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com',
+    keywords=["gitInfo", "github", "git", "relatorio", "reports", "gitReports"],
+    description=u'Analisador de repositórios do github',
+    packages=['pyGitInfo'],
+    install_requires=["pandas>=1.4.0", "matplotlib", "pygithub", "python-dotenv"],)
```

