# Comparing `tmp/httpmdhtml-0.0.8.tar.gz` & `tmp/httpmdhtml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpmdhtml-0.0.8.tar", last modified: Wed May  3 16:13:02 2023, max compression
+gzip compressed data, was "httpmdhtml-0.0.9.tar", last modified: Mon Jul 17 18:25:53 2023, max compression
```

## Comparing `httpmdhtml-0.0.8.tar` & `httpmdhtml-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-05-03 16:13:02.080493 httpmdhtml-0.0.8/
--rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-04-04 17:12:07.000000 httpmdhtml-0.0.8/LICENSE.txt
--rwxrwxrwx   0 john      (1000) john      (1000)     3582 2023-05-03 16:13:02.083211 httpmdhtml-0.0.8/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)     3147 2023-05-03 16:08:59.000000 httpmdhtml-0.0.8/README.md
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-05-03 16:13:01.686246 httpmdhtml-0.0.8/httpmdhtml/
--rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:12:07.000000 httpmdhtml-0.0.8/httpmdhtml/__init__.py
--rwxrwxrwx   0 john      (1000) john      (1000)     3590 2023-05-03 16:02:15.000000 httpmdhtml-0.0.8/httpmdhtml/md_to_html.py
--rwxrwxrwx   0 john      (1000) john      (1000)     4532 2023-05-03 16:03:35.000000 httpmdhtml-0.0.8/httpmdhtml/server.py
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-05-03 16:13:02.012376 httpmdhtml-0.0.8/httpmdhtml.egg-info/
--rwxrwxrwx   0 john      (1000) john      (1000)     3582 2023-05-03 16:13:00.000000 httpmdhtml-0.0.8/httpmdhtml.egg-info/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)      293 2023-05-03 16:13:01.000000 httpmdhtml-0.0.8/httpmdhtml.egg-info/SOURCES.txt
--rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-05-03 16:13:00.000000 httpmdhtml-0.0.8/httpmdhtml.egg-info/dependency_links.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       39 2023-05-03 16:13:00.000000 httpmdhtml-0.0.8/httpmdhtml.egg-info/requires.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       11 2023-05-03 16:13:00.000000 httpmdhtml-0.0.8/httpmdhtml.egg-info/top_level.txt
--rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-05-03 14:31:06.000000 httpmdhtml-0.0.8/pyproject.toml
--rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-05-03 16:13:02.098537 httpmdhtml-0.0.8/setup.cfg
--rwxrwxrwx   0 john      (1000) john      (1000)      923 2023-05-03 14:30:24.000000 httpmdhtml-0.0.8/setup.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-17 18:25:53.583030 httpmdhtml-0.0.9/
+-rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-04-04 17:12:07.000000 httpmdhtml-0.0.9/LICENSE.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)     3574 2023-07-17 18:25:53.585039 httpmdhtml-0.0.9/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)     3139 2023-05-03 16:16:27.000000 httpmdhtml-0.0.9/README.md
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-17 18:25:53.158159 httpmdhtml-0.0.9/httpmdhtml/
+-rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:12:07.000000 httpmdhtml-0.0.9/httpmdhtml/__init__.py
+-rwxrwxrwx   0 john      (1000) john      (1000)     3919 2023-07-17 18:18:16.000000 httpmdhtml-0.0.9/httpmdhtml/md_to_html.py
+-rwxrwxrwx   0 john      (1000) john      (1000)     4532 2023-05-03 16:03:35.000000 httpmdhtml-0.0.9/httpmdhtml/server.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-17 18:25:53.538926 httpmdhtml-0.0.9/httpmdhtml.egg-info/
+-rwxrwxrwx   0 john      (1000) john      (1000)     3574 2023-07-17 18:25:52.000000 httpmdhtml-0.0.9/httpmdhtml.egg-info/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)      293 2023-07-17 18:25:52.000000 httpmdhtml-0.0.9/httpmdhtml.egg-info/SOURCES.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-07-17 18:25:52.000000 httpmdhtml-0.0.9/httpmdhtml.egg-info/dependency_links.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)       39 2023-07-17 18:25:52.000000 httpmdhtml-0.0.9/httpmdhtml.egg-info/requires.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)       11 2023-07-17 18:25:52.000000 httpmdhtml-0.0.9/httpmdhtml.egg-info/top_level.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-05-03 14:31:06.000000 httpmdhtml-0.0.9/pyproject.toml
+-rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-07-17 18:25:53.599235 httpmdhtml-0.0.9/setup.cfg
+-rwxrwxrwx   0 john      (1000) john      (1000)      923 2023-07-17 17:47:45.000000 httpmdhtml-0.0.9/setup.py
```

### Comparing `httpmdhtml-0.0.8/LICENSE.txt` & `httpmdhtml-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpmdhtml-0.0.8/PKG-INFO` & `httpmdhtml-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: httpmdhtml
-Version: 0.0.8
+Version: 0.0.9
 Summary: HTTP server that converts markdown to HTML
 Home-page: https://github.com/treatmesubj/python-md-to-html-server
-Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.8.tar.gz
+Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.9.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/python-md-to-html-server
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -41,15 +41,15 @@
   -h, --help            show this help message and exit
   --cgi                 Run as CGI Server
   --bind ADDRESS, -b ADDRESS
                         Specify alternate bind address [default: all interfaces]
   --directory DIRECTORY, -d DIRECTORY
                         Specify alternative directory [default:current directory]
   --css_file CSS_FILE   css-file-path whose content will be written to the <style> element. Can be "none"; do not
-                            use any css
+                        use any css
   --live_md_rr LIVE_MD_RR, -l LIVE_MD_RR
                         Continuous refresh rate of MD page, in ms. Respects cache
 ```
 
 ### Markdown-to-HTML Out-File
 ```
 python -m httpmdhtml.md_to_html -i in_file.md -o out_file.html --encode_local_images
@@ -63,10 +63,10 @@
                         in-file-path; your existing markdown file
   --out_file_path OUT_FILE_PATH, -o OUT_FILE_PATH
                         out-file-path; your HTML file to be created
   --encode_local_images, -e
                         in HTML, embed base64-encoded data of local images linked to in your markdown; remove
                         dependency on presence of external local images
   --css_file CSS_FILE   css-file-path whose content will be written to the <style> element. Can be "none"; do not
-                            use any css
+                        use any css
 ```
 ![](<./scrot.png>)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zes35jps_/tmpvzxasnep_TarContainer/0/2", line 73, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_zes35jps_/tmpvzxasnep_TarContainer/0/2", line 73, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.8 Summary: HTTP server that
+Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.9 Summary: HTTP server that
 converts markdown to HTML Home-page: https://github.com/treatmesubj/python-md-
 to-html-server Download-URL: https://github.com/treatmesubj/python-md-to-html-
-server/archive/refs/tags/v0.0.8.tar.gz Author: John Hupperts Author-email:
+server/archive/refs/tags/v0.0.9.tar.gz Author: John Hupperts Author-email:
 jrock4503@hotmail.com License: gpl-3.0 Project-URL: Source, https://github.com/
 treatmesubj/python-md-to-html-server Description-Content-Type: text/markdown
 License-File: LICENSE.txt # Python Markdown-to-HTML Server It's the standard
 Python [http.server module](https://docs.python.org/3/library/http.server.html)
 but via [markdown-it-py](https://github.com/executablebooks/markdown-it-py),
 requested Markdown files are rendered and served as HTML The `http.server`
 module's `SimpleHTTPRequestHandler` class is inherited by a new class with its
```

### Comparing `httpmdhtml-0.0.8/README.md` & `httpmdhtml-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   -h, --help            show this help message and exit
   --cgi                 Run as CGI Server
   --bind ADDRESS, -b ADDRESS
                         Specify alternate bind address [default: all interfaces]
   --directory DIRECTORY, -d DIRECTORY
                         Specify alternative directory [default:current directory]
   --css_file CSS_FILE   css-file-path whose content will be written to the <style> element. Can be "none"; do not
-                            use any css
+                        use any css
   --live_md_rr LIVE_MD_RR, -l LIVE_MD_RR
                         Continuous refresh rate of MD page, in ms. Respects cache
 ```
 
 ### Markdown-to-HTML Out-File
 ```
 python -m httpmdhtml.md_to_html -i in_file.md -o out_file.html --encode_local_images
@@ -50,10 +50,10 @@
                         in-file-path; your existing markdown file
   --out_file_path OUT_FILE_PATH, -o OUT_FILE_PATH
                         out-file-path; your HTML file to be created
   --encode_local_images, -e
                         in HTML, embed base64-encoded data of local images linked to in your markdown; remove
                         dependency on presence of external local images
   --css_file CSS_FILE   css-file-path whose content will be written to the <style> element. Can be "none"; do not
-                            use any css
+                        use any css
 ```
 ![](<./scrot.png>)
```

### Comparing `httpmdhtml-0.0.8/httpmdhtml/md_to_html.py` & `httpmdhtml-0.0.9/httpmdhtml/md_to_html.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,19 +32,24 @@
     soup.select_one("head").append(soup.new_tag("style"))
     if css_file:
         if css_file == "none":
             css = ""
         else:
             with open(css_file, "r") as f:
                 css = f.read()
-    else:
-        css = """body { background-color: #272822; color: white; font-family: Courier; }
-        a[href] { color: #66d9ef; }
-        code { color: #ae81ff; background-color: #272b33; border-radius: 6px; }
-        table, th, td { border: 1px solid; border-collapse: collapse; padding-left: 4px; padding-right: 4px; }"""
+    else: # #272822
+        css = """
+body { background-color: #272822; color: #e6edf3; font-family: -apple-system,BlinkMacSystemFont,"Segoe UI","Noto Sans",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji"; position: relative; max-width: 960px; margin: auto }
+a[href] { color: #66d9ef; }
+code { color: #e6edf3; font-family: monospace; white-space: break-spaces; }
+p code { padding: .2em .4em; border-radius: 6px; background-color: #343941; }
+pre { padding: 1em; border-radius: 6px; background-color: #161b22; }
+table, th, td { border: 1px solid; border-collapse: collapse; padding-left: 4px; padding-right: 4px; }
+img { max-width: 100%; }
+"""
     soup.select_one("style").string = css
     if live_md_rr:
         script = (
             f"setTimeout(function(){{ document.location.reload(); }}, {live_md_rr});"
         )
         soup.select_one("head").append(soup.new_tag("script"))
         soup.select_one("script").string = script
```

### Comparing `httpmdhtml-0.0.8/httpmdhtml/server.py` & `httpmdhtml-0.0.9/httpmdhtml/server.py`

 * *Files identical despite different names*

### Comparing `httpmdhtml-0.0.8/httpmdhtml.egg-info/PKG-INFO` & `httpmdhtml-0.0.9/httpmdhtml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: httpmdhtml
-Version: 0.0.8
+Version: 0.0.9
 Summary: HTTP server that converts markdown to HTML
 Home-page: https://github.com/treatmesubj/python-md-to-html-server
-Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.8.tar.gz
+Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.9.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/python-md-to-html-server
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -41,15 +41,15 @@
   -h, --help            show this help message and exit
   --cgi                 Run as CGI Server
   --bind ADDRESS, -b ADDRESS
                         Specify alternate bind address [default: all interfaces]
   --directory DIRECTORY, -d DIRECTORY
                         Specify alternative directory [default:current directory]
   --css_file CSS_FILE   css-file-path whose content will be written to the <style> element. Can be "none"; do not
-                            use any css
+                        use any css
   --live_md_rr LIVE_MD_RR, -l LIVE_MD_RR
                         Continuous refresh rate of MD page, in ms. Respects cache
 ```
 
 ### Markdown-to-HTML Out-File
 ```
 python -m httpmdhtml.md_to_html -i in_file.md -o out_file.html --encode_local_images
@@ -63,10 +63,10 @@
                         in-file-path; your existing markdown file
   --out_file_path OUT_FILE_PATH, -o OUT_FILE_PATH
                         out-file-path; your HTML file to be created
   --encode_local_images, -e
                         in HTML, embed base64-encoded data of local images linked to in your markdown; remove
                         dependency on presence of external local images
   --css_file CSS_FILE   css-file-path whose content will be written to the <style> element. Can be "none"; do not
-                            use any css
+                        use any css
 ```
 ![](<./scrot.png>)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zes35jps_/tmpvzxasnep_TarContainer/0/9", line 73, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_zes35jps_/tmpvzxasnep_TarContainer/0/9", line 73, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.8 Summary: HTTP server that
+Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.9 Summary: HTTP server that
 converts markdown to HTML Home-page: https://github.com/treatmesubj/python-md-
 to-html-server Download-URL: https://github.com/treatmesubj/python-md-to-html-
-server/archive/refs/tags/v0.0.8.tar.gz Author: John Hupperts Author-email:
+server/archive/refs/tags/v0.0.9.tar.gz Author: John Hupperts Author-email:
 jrock4503@hotmail.com License: gpl-3.0 Project-URL: Source, https://github.com/
 treatmesubj/python-md-to-html-server Description-Content-Type: text/markdown
 License-File: LICENSE.txt # Python Markdown-to-HTML Server It's the standard
 Python [http.server module](https://docs.python.org/3/library/http.server.html)
 but via [markdown-it-py](https://github.com/executablebooks/markdown-it-py),
 requested Markdown files are rendered and served as HTML The `http.server`
 module's `SimpleHTTPRequestHandler` class is inherited by a new class with its
```

### Comparing `httpmdhtml-0.0.8/setup.py` & `httpmdhtml-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="httpmdhtml",
-    version="0.0.8",
+    version="0.0.9",
     license="gpl-3.0",
     author="John Hupperts",
     author_email="jrock4503@hotmail.com",
     description="HTTP server that converts markdown to HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/treatmesubj/python-md-to-html-server",
-    download_url="https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.8.tar.gz",
+    download_url="https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.9.tar.gz",
     packages=["httpmdhtml"],
     package_dir={"python-md-to-html-server": "httpmdhtml"},
     project_urls={
         "Source": "https://github.com/treatmesubj/python-md-to-html-server",
     },
     install_requires=[
         "markdown-it-py",
```

