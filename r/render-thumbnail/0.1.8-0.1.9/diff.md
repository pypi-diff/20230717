# Comparing `tmp/render_thumbnail-0.1.8.tar.gz` & `tmp/render_thumbnail-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_thumbnail-0.1.8.tar", max compression
+gzip compressed data, was "render_thumbnail-0.1.9.tar", max compression
```

## Comparing `render_thumbnail-0.1.8.tar` & `render_thumbnail-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.8/README.md
--rw-r--r--   0        0        0      401 2023-07-13 18:01:34.321969 render_thumbnail-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.8/render_thumbnail/__init__.py
--rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.8/render_thumbnail/__main__.py
--rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.8/render_thumbnail/functions_tex.py
--rw-r--r--   0        0        0     2656 2023-07-13 18:01:25.938702 render_thumbnail-0.1.8/render_thumbnail/main.py
--rw-r--r--   0        0        0      304 1970-01-01 00:00:00.000000 render_thumbnail-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.9/README.md
+-rw-r--r--   0        0        0      446 2023-07-14 11:54:49.945306 render_thumbnail-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.9/render_thumbnail/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.9/render_thumbnail/__main__.py
+-rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.9/render_thumbnail/functions_tex.py
+-rw-r--r--   0        0        0     3165 2023-07-14 11:54:18.551990 render_thumbnail-0.1.9/render_thumbnail/main.py
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 render_thumbnail-0.1.9/PKG-INFO
```

### Comparing `render_thumbnail-0.1.8/render_thumbnail/functions_tex.py` & `render_thumbnail-0.1.9/render_thumbnail/functions_tex.py`

 * *Files identical despite different names*

### Comparing `render_thumbnail-0.1.8/render_thumbnail/main.py` & `render_thumbnail-0.1.9/render_thumbnail/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import click
 import os
 from .functions_tex import extract_tex_env
 from .functions_tex import files as file_list
-
+import re
 
 
 thumbnail_title=r"""
 \vspace*{\fill}
-\vtitle[\Huge{\textbf{JEE}}]
+\begin{center}
+\Huge{\textbf{JEE}}\\
+\texttt{[YEAR]}
+\end{center}
 \vspace*{\fill}
 """
 
 tikz_render=r"""
 \vspace*{\fill}
 \begin{center}
     \input{tikz.tex}
@@ -73,40 +76,55 @@
         help="nth tikz environment"
         )
 def main(inputfile, outputfile, environment, title, nthtikz):
     path_tikz = os.path.dirname(os.path.abspath(inputfile))
     os.makedirs(f'{path_tikz}/thumbnail', exist_ok=True)
     path_main = os.path.join(f'{path_tikz}/thumbnail', 'main.tex')
     
+
+    year = 1998
+    with open(inputfile, 'r') as f:
+        for line in f:
+            x = re.findall('\d{4}', line)
+            if x:
+                year = int(x[0])
+
     try:
         extract_tex_env(inputfile, outputfile, environment)
     except:
         click.echo("Failed to extract_tex_env")
 
     files = [os.path.basename(f) for f in file_list]
     with open(path_main, 'w') as file:
         file.write(f'\\documentclass{{article}}\n')
         file.write(f'\\usepackage{{v-equation}}\n')
         file.write(f'\\vgeometry[8][4.5]\n')
 
         file.write(f'\\begin{{document}}\n')
         print(files)
         if len(files) >= 1:
-            file.write(f'{thumbnail_title.replace("JEE", title)}\n')
+            file.write(f'{thumbnail_title.replace("JEE", title).replace("YEAR", year)}\n')
             file.write(f'{tikz_render.replace("tikz.tex", files[nthtikz - 1])}\n')
 
         file.write(f'\\end{{document}}')
 
 
 
     try:
-        print(os.getcwd)
         os.chdir("./thumbnail")
         try:
             os.system("pdflatex -shell-escape main.tex")
+            try:
+                os.system("vbpdf topng")
+                try:
+                    os.system("qlmanage -p main.png")
+                except:
+                    click.echo("Failed to preview the png file.")
+            except:
+                click.echo("Failed to convert png ")
         except:
             click.echo("Failed to rum pdflatex")
     except:
         click.echo("Failed to run cddir")
```

