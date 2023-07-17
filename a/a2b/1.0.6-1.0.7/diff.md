# Comparing `tmp/a2b-1.0.6.tar.gz` & `tmp/a2b-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2b-1.0.6.tar", last modified: Tue Mar 28 06:32:35 2023, max compression
+gzip compressed data, was "a2b-1.0.7.tar", last modified: Mon Jul 17 07:09:22 2023, max compression
```

## Comparing `a2b-1.0.6.tar` & `a2b-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 06:32:35.610979 a2b-1.0.6/
--rw-rw-rw-   0        0        0     5732 2023-03-28 06:32:35.610979 a2b-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4143 2023-03-27 17:21:02.000000 a2b-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 06:32:35.580406 a2b-1.0.6/a2b/
--rw-rw-rw-   0        0        0        0 2023-02-14 21:07:52.000000 a2b-1.0.6/a2b/__init__.py
--rw-rw-rw-   0        0        0      368 2023-03-27 15:26:54.000000 a2b-1.0.6/a2b/link_utils.py
--rw-rw-rw-   0        0        0     2580 2023-03-28 06:27:47.000000 a2b-1.0.6/a2b/main.py
--rw-rw-rw-   0        0        0     3491 2023-03-27 15:32:25.000000 a2b-1.0.6/a2b/markdown.py
--rw-rw-rw-   0        0        0      378 2023-03-27 09:03:25.000000 a2b-1.0.6/a2b/message.py
--rw-rw-rw-   0        0        0     4409 2023-03-27 14:29:22.000000 a2b-1.0.6/a2b/notion.py
--rw-rw-rw-   0        0        0     1535 2023-03-27 10:13:52.000000 a2b-1.0.6/a2b/s2.py
-drwxrwxrwx   0        0        0        0 2023-03-28 06:32:35.610979 a2b-1.0.6/a2b.egg-info/
--rw-rw-rw-   0        0        0     5732 2023-03-28 06:32:33.000000 a2b-1.0.6/a2b.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-03-28 06:32:35.000000 a2b-1.0.6/a2b.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 06:32:33.000000 a2b-1.0.6/a2b.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-03-28 06:32:33.000000 a2b-1.0.6/a2b.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-28 06:32:33.000000 a2b-1.0.6/a2b.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-03-28 06:32:33.000000 a2b-1.0.6/a2b.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      686 2023-03-28 06:31:34.000000 a2b-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-28 06:32:35.610979 a2b-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-03-27 08:18:02.000000 a2b-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:09:22.230729 a2b-1.0.7/
+-rw-rw-rw-   0        0        0     6201 2023-07-17 07:09:22.230729 a2b-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4572 2023-07-17 07:07:16.000000 a2b-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 07:09:22.090114 a2b-1.0.7/a2b/
+-rw-rw-rw-   0        0        0        0 2023-02-14 21:07:52.000000 a2b-1.0.7/a2b/__init__.py
+-rw-rw-rw-   0        0        0      368 2023-03-27 15:26:54.000000 a2b-1.0.7/a2b/link_utils.py
+-rw-rw-rw-   0        0        0     2580 2023-03-28 06:27:47.000000 a2b-1.0.7/a2b/main.py
+-rw-rw-rw-   0        0        0     3491 2023-03-27 15:32:25.000000 a2b-1.0.7/a2b/markdown.py
+-rw-rw-rw-   0        0        0      378 2023-03-27 09:03:25.000000 a2b-1.0.7/a2b/message.py
+-rw-rw-rw-   0        0        0     4411 2023-07-17 06:58:09.000000 a2b-1.0.7/a2b/notion.py
+-rw-rw-rw-   0        0        0     1535 2023-03-27 10:13:52.000000 a2b-1.0.7/a2b/s2.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:09:22.230729 a2b-1.0.7/a2b.egg-info/
+-rw-rw-rw-   0        0        0     6201 2023-07-17 07:09:21.000000 a2b-1.0.7/a2b.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-07-17 07:09:21.000000 a2b-1.0.7/a2b.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:09:21.000000 a2b-1.0.7/a2b.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-17 07:09:21.000000 a2b-1.0.7/a2b.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-28 06:32:33.000000 a2b-1.0.7/a2b.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-07-17 07:09:21.000000 a2b-1.0.7/a2b.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      686 2023-07-17 06:56:22.000000 a2b-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 07:09:22.230729 a2b-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-03-27 08:18:02.000000 a2b-1.0.7/setup.py
```

### Comparing `a2b-1.0.6/PKG-INFO` & `a2b-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: a2b
-Version: 1.0.6
+Version: 1.0.7
 Summary: Replace arxiv links in markdowns by their corresponding bibliography.
 Home-page: https://github.com/kevinkevin556/a2b
 Author: Zhen-Lun Hong
 Author-email: kevink556@gmail.com
 License: MIT
 Description: # A2B (Arxiv to Bibliography)
         
-        > Replace arXiv links (or doi links) by their corresponding bibliography in markdowns. Inspired by [Mu Li](https://www.youtube.com/watch?v=q1G0xZCqYxY&ab_channel=MuLi).
+        ![pypi](https://img.shields.io/pypi/v/a2b?color=green)  ![license](https://img.shields.io/pypi/l/a2b?color=orange)
         
+        > Replace arXiv links (or doi links) by their corresponding bibliography in markdowns / Notion databases. Inspired by [Mu Li](https://www.youtube.com/watch?v=q1G0xZCqYxY&ab_channel=MuLi).
         
-        ![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/demo.gif)
         
+        This repo provides a tool to replace arXiv/DOI links saved in
         
-        This repo provides a tool to replace arXiv/DOI links saved in 
-        
-        * [markdown files](#markdown) or
+        * [Markdown files](#markdown) or
         * [Notion database](#notion-database)
         
         with their corresponding bibliographic information, which intends to create a more convenient experience for users in needs of searching, collecting, and taking notes of literatures. The script uses the Semantic Scholar API to retrieve information such as authors, title, journal, year, and citation count for a given arXiv paper.
         
+        | [Markdown](#markdown)| [Notion Database](#notion-database) |
+        |:---:|:---:|
+        ![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/demo.gif) |![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/notion-demo.gif)|
+        
         
         ## Installation
         
         To install `a2b`, make sure you have [pip installed](https://pip.pypa.io/en/stable/installation/) and run:
         
         ```Bash
         >> pip install a2b
@@ -34,38 +37,38 @@
         
         The tool can be run from the command line, e.g. to check the installed version of `a2b`,
         
         ```Bash
         >> a2b --version
         ```
         
-        
-        ![](https://img.icons8.com/ios/2x/markdown.png)
+        ![markdown-logo](https://img.icons8.com/ios/2x/markdown.png)
         
         ### Markdown
         
         #### 1. Generate markdown from a single arXiv link or DOI
         
         For example:
         
         ```Bash
-        >> a2b --arXiv https://arXiv.org/abs/1912.08957
+        >> a2b --arxiv https://arXiv.org/abs/1912.08957
         
-        ## __Optimization for deep learning: theory and algorithms.__ *Ruoyu Sun.* __ArXiv, 2019__ [(Arxiv)](https://arXiv.org/abs/1912.08957) 
-        ## [(S2)](https://www.semanticscholar.org/paper/c23173e93f1db79a422e2af881a40afb96b8cb92) (Citations __114__)
+        ## __Optimization for deep learning: theory and algorithms.__ *Ruoyu Sun.* __ArXiv, 2019__ [(Arxiv)](ht
+        ## tps://arXiv.org/abs/1912.08957) [(S2)](https://www.semanticscholar.org/paper/c23173e93f1db79a422e2af
+        ## 881a40afb96b8cb92) (Citations __114__)
         ```
         
         Here you can use the link of pdf `https://arXiv.org/pdf/1912.08957.pdf`, instead of the link of arXiv page.
         
         ```Bash
         >> a2b --doi https://doi.org/10.1007/BF00133570
         
         ## __Snakes: Active contour models.__ *M. Kass et al.* __International Journal of Computer Vision, 2004__ 
-        ## [(Link)](https://doi.org/10.1007/BF00133570) [(S2)](https://www.semanticscholar.org/paper/9394a5d5adcb626128b6a42c8810b9505a3c6487)
-        ## (Citations __15860__)
+        ## [(Link)](https://doi.org/10.1007/BF00133570) [(S2)](https://www.semanticscholar.org/paper/9394a5d5adcb6
+        ## 26128b6a42c8810b9505a3c6487) (Citations __15860__)
         ```
         
         One can simply provide the DOI `10.1007/BF00133570` without adding the hyperlink prefix to generate bibilography from DOI.
         
         #### 2. Replace arXiv links in a single markdown file
         
         ```Bash
@@ -82,17 +85,19 @@
         
         To replace arXiv links in the markdown files **ONLY** within the directory (subdirectories excluded), use arguments `--no-recursive` or `-nr`:
         
         ```Bash
         >> a2b -nr path/to/directory
         ```
         
-        ![](https://img.icons8.com/color/2x/notion--v1.png)
+        ---
         
-        ###  Notion Database
+        ![notion-logo](https://img.icons8.com/color/2x/notion--v1.png)
+        
+        ### Notion Database
         
         To generate bibliography from links saved in a Notion database, follow the instructions below
         
         1. Create a new [Notion integration](https://www.notion.so/my-integrations) and keep the Notion API key obtained from the integration
         2. Go to the Notion database and 
             * [Connect the Notion database to the integration](https://developers.notion.com/docs/create-a-notion-integration#step-2-share-a-database-with-your-integration) you just created
             * Create these columns (with data type matched) in the Notion database
@@ -116,25 +121,25 @@
         
         ```Bash
         >> a2b --notion notion_database_id
         # or
         >> a2b --notion notion_database_url
         ```
         
-        
-        
         ## Changelog
         
+        * **Version 1.0.7**
+          * Fix the problem of arxiv and doi format confliction in Notion
+        * **Version 1.0.6**
+          * Fix version command
         * **Version 1.0.5**
           * Support Notion database
-          * Fix version command
         * **Version 1.0.4**
           * Support creating bibliography from DOI links
           * Support querying a single arXiv link from terminal
-        
 Keywords: arxiv,bibliography,markdown,Notion
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `a2b-1.0.6/README.md` & `a2b-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # A2B (Arxiv to Bibliography)
 
-> Replace arXiv links (or doi links) by their corresponding bibliography in markdowns. Inspired by [Mu Li](https://www.youtube.com/watch?v=q1G0xZCqYxY&ab_channel=MuLi).
+![pypi](https://img.shields.io/pypi/v/a2b?color=green)  ![license](https://img.shields.io/pypi/l/a2b?color=orange)
 
+> Replace arXiv links (or doi links) by their corresponding bibliography in markdowns / Notion databases. Inspired by [Mu Li](https://www.youtube.com/watch?v=q1G0xZCqYxY&ab_channel=MuLi).
 
-![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/demo.gif)
 
+This repo provides a tool to replace arXiv/DOI links saved in
 
-This repo provides a tool to replace arXiv/DOI links saved in 
-
-* [markdown files](#markdown) or
+* [Markdown files](#markdown) or
 * [Notion database](#notion-database)
 
 with their corresponding bibliographic information, which intends to create a more convenient experience for users in needs of searching, collecting, and taking notes of literatures. The script uses the Semantic Scholar API to retrieve information such as authors, title, journal, year, and citation count for a given arXiv paper.
 
+| [Markdown](#markdown)| [Notion Database](#notion-database) |
+|:---:|:---:|
+![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/demo.gif) |![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/notion-demo.gif)|
+
 
 ## Installation
 
 To install `a2b`, make sure you have [pip installed](https://pip.pypa.io/en/stable/installation/) and run:
 
 ```Bash
 >> pip install a2b
@@ -26,38 +29,38 @@
 
 The tool can be run from the command line, e.g. to check the installed version of `a2b`,
 
 ```Bash
 >> a2b --version
 ```
 
-
-![](https://img.icons8.com/ios/2x/markdown.png)
+![markdown-logo](https://img.icons8.com/ios/2x/markdown.png)
 
 ### Markdown
 
 #### 1. Generate markdown from a single arXiv link or DOI
 
 For example:
 
 ```Bash
->> a2b --arXiv https://arXiv.org/abs/1912.08957
+>> a2b --arxiv https://arXiv.org/abs/1912.08957
 
-## __Optimization for deep learning: theory and algorithms.__ *Ruoyu Sun.* __ArXiv, 2019__ [(Arxiv)](https://arXiv.org/abs/1912.08957) 
-## [(S2)](https://www.semanticscholar.org/paper/c23173e93f1db79a422e2af881a40afb96b8cb92) (Citations __114__)
+## __Optimization for deep learning: theory and algorithms.__ *Ruoyu Sun.* __ArXiv, 2019__ [(Arxiv)](ht
+## tps://arXiv.org/abs/1912.08957) [(S2)](https://www.semanticscholar.org/paper/c23173e93f1db79a422e2af
+## 881a40afb96b8cb92) (Citations __114__)
 ```
 
 Here you can use the link of pdf `https://arXiv.org/pdf/1912.08957.pdf`, instead of the link of arXiv page.
 
 ```Bash
 >> a2b --doi https://doi.org/10.1007/BF00133570
 
 ## __Snakes: Active contour models.__ *M. Kass et al.* __International Journal of Computer Vision, 2004__ 
-## [(Link)](https://doi.org/10.1007/BF00133570) [(S2)](https://www.semanticscholar.org/paper/9394a5d5adcb626128b6a42c8810b9505a3c6487)
-## (Citations __15860__)
+## [(Link)](https://doi.org/10.1007/BF00133570) [(S2)](https://www.semanticscholar.org/paper/9394a5d5adcb6
+## 26128b6a42c8810b9505a3c6487) (Citations __15860__)
 ```
 
 One can simply provide the DOI `10.1007/BF00133570` without adding the hyperlink prefix to generate bibilography from DOI.
 
 #### 2. Replace arXiv links in a single markdown file
 
 ```Bash
@@ -74,17 +77,19 @@
 
 To replace arXiv links in the markdown files **ONLY** within the directory (subdirectories excluded), use arguments `--no-recursive` or `-nr`:
 
 ```Bash
 >> a2b -nr path/to/directory
 ```
 
-![](https://img.icons8.com/color/2x/notion--v1.png)
+---
+
+![notion-logo](https://img.icons8.com/color/2x/notion--v1.png)
 
-###  Notion Database
+### Notion Database
 
 To generate bibliography from links saved in a Notion database, follow the instructions below
 
 1. Create a new [Notion integration](https://www.notion.so/my-integrations) and keep the Notion API key obtained from the integration
 2. Go to the Notion database and 
     * [Connect the Notion database to the integration](https://developers.notion.com/docs/create-a-notion-integration#step-2-share-a-database-with-your-integration) you just created
     * Create these columns (with data type matched) in the Notion database
@@ -108,17 +113,18 @@
 
 ```Bash
 >> a2b --notion notion_database_id
 # or
 >> a2b --notion notion_database_url
 ```
 
-
-
 ## Changelog
 
+* **Version 1.0.7**
+  * Fix the problem of arxiv and doi format confliction in Notion
+* **Version 1.0.6**
+  * Fix version command
 * **Version 1.0.5**
   * Support Notion database
-  * Fix version command
 * **Version 1.0.4**
   * Support creating bibliography from DOI links
-  * Support querying a single arXiv link from terminal
+  * Support querying a single arXiv link from terminal
```

### Comparing `a2b-1.0.6/a2b/main.py` & `a2b-1.0.7/a2b/main.py`

 * *Files identical despite different names*

### Comparing `a2b-1.0.6/a2b/markdown.py` & `a2b-1.0.7/a2b/markdown.py`

 * *Files identical despite different names*

### Comparing `a2b-1.0.6/a2b/notion.py` & `a2b-1.0.7/a2b/notion.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,18 +88,19 @@
 
         page_id = page.get("id")
         paper_title = page.get("properties").get(
             "Title").get("title")[0].get("plain_text")
         arxiv_id = get_arxiv_id(paper_title)
         doi = get_doi(paper_title)
 
-        if arxiv_id:
-            paper_data = connect_to_s2(arxiv_id=arxiv_id)
-        elif doi:
+
+        if doi:
             paper_data = connect_to_s2(doi=doi)
+        elif arxiv_id:
+            paper_data = connect_to_s2(arxiv_id=arxiv_id)
         else:
             paper_data = None
 
         if paper_data:
             s2_id, title, authors, journal, year, citations = extract_metadata(
                 paper_data)
             page_data = generate_page_data(
```

### Comparing `a2b-1.0.6/a2b/s2.py` & `a2b-1.0.7/a2b/s2.py`

 * *Files identical despite different names*

### Comparing `a2b-1.0.6/a2b.egg-info/PKG-INFO` & `a2b-1.0.7/a2b.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: a2b
-Version: 1.0.6
+Version: 1.0.7
 Summary: Replace arxiv links in markdowns by their corresponding bibliography.
 Home-page: https://github.com/kevinkevin556/a2b
 Author: Zhen-Lun Hong
 Author-email: kevink556@gmail.com
 License: MIT
 Description: # A2B (Arxiv to Bibliography)
         
-        > Replace arXiv links (or doi links) by their corresponding bibliography in markdowns. Inspired by [Mu Li](https://www.youtube.com/watch?v=q1G0xZCqYxY&ab_channel=MuLi).
+        ![pypi](https://img.shields.io/pypi/v/a2b?color=green)  ![license](https://img.shields.io/pypi/l/a2b?color=orange)
         
+        > Replace arXiv links (or doi links) by their corresponding bibliography in markdowns / Notion databases. Inspired by [Mu Li](https://www.youtube.com/watch?v=q1G0xZCqYxY&ab_channel=MuLi).
         
-        ![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/demo.gif)
         
+        This repo provides a tool to replace arXiv/DOI links saved in
         
-        This repo provides a tool to replace arXiv/DOI links saved in 
-        
-        * [markdown files](#markdown) or
+        * [Markdown files](#markdown) or
         * [Notion database](#notion-database)
         
         with their corresponding bibliographic information, which intends to create a more convenient experience for users in needs of searching, collecting, and taking notes of literatures. The script uses the Semantic Scholar API to retrieve information such as authors, title, journal, year, and citation count for a given arXiv paper.
         
+        | [Markdown](#markdown)| [Notion Database](#notion-database) |
+        |:---:|:---:|
+        ![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/demo.gif) |![demo](https://github.com/kevinkevin556/arxiv2bib/raw/main/notion-demo.gif)|
+        
         
         ## Installation
         
         To install `a2b`, make sure you have [pip installed](https://pip.pypa.io/en/stable/installation/) and run:
         
         ```Bash
         >> pip install a2b
@@ -34,38 +37,38 @@
         
         The tool can be run from the command line, e.g. to check the installed version of `a2b`,
         
         ```Bash
         >> a2b --version
         ```
         
-        
-        ![](https://img.icons8.com/ios/2x/markdown.png)
+        ![markdown-logo](https://img.icons8.com/ios/2x/markdown.png)
         
         ### Markdown
         
         #### 1. Generate markdown from a single arXiv link or DOI
         
         For example:
         
         ```Bash
-        >> a2b --arXiv https://arXiv.org/abs/1912.08957
+        >> a2b --arxiv https://arXiv.org/abs/1912.08957
         
-        ## __Optimization for deep learning: theory and algorithms.__ *Ruoyu Sun.* __ArXiv, 2019__ [(Arxiv)](https://arXiv.org/abs/1912.08957) 
-        ## [(S2)](https://www.semanticscholar.org/paper/c23173e93f1db79a422e2af881a40afb96b8cb92) (Citations __114__)
+        ## __Optimization for deep learning: theory and algorithms.__ *Ruoyu Sun.* __ArXiv, 2019__ [(Arxiv)](ht
+        ## tps://arXiv.org/abs/1912.08957) [(S2)](https://www.semanticscholar.org/paper/c23173e93f1db79a422e2af
+        ## 881a40afb96b8cb92) (Citations __114__)
         ```
         
         Here you can use the link of pdf `https://arXiv.org/pdf/1912.08957.pdf`, instead of the link of arXiv page.
         
         ```Bash
         >> a2b --doi https://doi.org/10.1007/BF00133570
         
         ## __Snakes: Active contour models.__ *M. Kass et al.* __International Journal of Computer Vision, 2004__ 
-        ## [(Link)](https://doi.org/10.1007/BF00133570) [(S2)](https://www.semanticscholar.org/paper/9394a5d5adcb626128b6a42c8810b9505a3c6487)
-        ## (Citations __15860__)
+        ## [(Link)](https://doi.org/10.1007/BF00133570) [(S2)](https://www.semanticscholar.org/paper/9394a5d5adcb6
+        ## 26128b6a42c8810b9505a3c6487) (Citations __15860__)
         ```
         
         One can simply provide the DOI `10.1007/BF00133570` without adding the hyperlink prefix to generate bibilography from DOI.
         
         #### 2. Replace arXiv links in a single markdown file
         
         ```Bash
@@ -82,17 +85,19 @@
         
         To replace arXiv links in the markdown files **ONLY** within the directory (subdirectories excluded), use arguments `--no-recursive` or `-nr`:
         
         ```Bash
         >> a2b -nr path/to/directory
         ```
         
-        ![](https://img.icons8.com/color/2x/notion--v1.png)
+        ---
         
-        ###  Notion Database
+        ![notion-logo](https://img.icons8.com/color/2x/notion--v1.png)
+        
+        ### Notion Database
         
         To generate bibliography from links saved in a Notion database, follow the instructions below
         
         1. Create a new [Notion integration](https://www.notion.so/my-integrations) and keep the Notion API key obtained from the integration
         2. Go to the Notion database and 
             * [Connect the Notion database to the integration](https://developers.notion.com/docs/create-a-notion-integration#step-2-share-a-database-with-your-integration) you just created
             * Create these columns (with data type matched) in the Notion database
@@ -116,25 +121,25 @@
         
         ```Bash
         >> a2b --notion notion_database_id
         # or
         >> a2b --notion notion_database_url
         ```
         
-        
-        
         ## Changelog
         
+        * **Version 1.0.7**
+          * Fix the problem of arxiv and doi format confliction in Notion
+        * **Version 1.0.6**
+          * Fix version command
         * **Version 1.0.5**
           * Support Notion database
-          * Fix version command
         * **Version 1.0.4**
           * Support creating bibliography from DOI links
           * Support querying a single arXiv link from terminal
-        
 Keywords: arxiv,bibliography,markdown,Notion
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `a2b-1.0.6/pyproject.toml` & `a2b-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "a2b"
-version = "1.0.6"
+version = "1.0.7"
 description = "Replace arxiv links in markdowns by their corresponding bibliography."
 long_description_content_type = "text/markdown"
 url = "https://github.com/kevinkevin556/a2b"
 author = "Zhen-Lun Hong"
 author_email = "kevink556@gmail.com"
 license = "MIT"
 keywords = ["arxiv", "bibliography", "markdown", "Notion"]
```

### Comparing `a2b-1.0.6/setup.py` & `a2b-1.0.7/setup.py`

 * *Files identical despite different names*

