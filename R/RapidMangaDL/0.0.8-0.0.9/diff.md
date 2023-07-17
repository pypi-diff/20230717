# Comparing `tmp/RapidMangaDL-0.0.8.tar.gz` & `tmp/RapidMangaDL-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RapidMangaDL-0.0.8.tar", last modified: Mon Jul 17 08:45:44 2023, max compression
+gzip compressed data, was "RapidMangaDL-0.0.9.tar", last modified: Mon Jul 17 09:53:31 2023, max compression
```

## Comparing `RapidMangaDL-0.0.8.tar` & `RapidMangaDL-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:45:44.536531 RapidMangaDL-0.0.8/
--rw-rw-rw-   0        0        0     4716 2023-07-17 08:45:44.528525 RapidMangaDL-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3312 2023-07-17 08:26:28.000000 RapidMangaDL-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 08:45:44.444524 RapidMangaDL-0.0.8/RapidMangaDL.egg-info/
--rw-rw-rw-   0        0        0     4716 2023-07-17 08:45:42.000000 RapidMangaDL-0.0.8/RapidMangaDL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      932 2023-07-17 08:45:43.000000 RapidMangaDL-0.0.8/RapidMangaDL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:45:42.000000 RapidMangaDL-0.0.8/RapidMangaDL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-17 08:45:42.000000 RapidMangaDL-0.0.8/RapidMangaDL.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      200 2023-07-17 08:45:42.000000 RapidMangaDL-0.0.8/RapidMangaDL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:45:42.000000 RapidMangaDL-0.0.8/RapidMangaDL.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 08:45:44.459526 RapidMangaDL-0.0.8/manga_dl/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:52:51.000000 RapidMangaDL-0.0.8/manga_dl/__init__.py
--rw-rw-rw-   0        0        0     6763 2023-07-16 15:26:29.000000 RapidMangaDL-0.0.8/manga_dl/app.py
--rw-rw-rw-   0        0        0      309 2023-07-11 07:46:25.000000 RapidMangaDL-0.0.8/manga_dl/jsconfig.json
--rw-rw-rw-   0        0        0     6287 2023-07-16 16:02:19.000000 RapidMangaDL-0.0.8/manga_dl/main.py
--rw-rw-rw-   0        0        0    23640 2023-07-16 15:27:37.000000 RapidMangaDL-0.0.8/manga_dl/manga.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:45:44.491528 RapidMangaDL-0.0.8/manga_dl/public/
--rw-rw-rw-   0        0        0   232918 2023-07-11 11:05:36.000000 RapidMangaDL-0.0.8/manga_dl/public/bootstrap530.css
--rw-rw-rw-   0        0        0    80427 2023-07-11 11:07:47.000000 RapidMangaDL-0.0.8/manga_dl/public/bootstrap530.js
--rw-rw-rw-   0        0        0    65212 2023-07-10 06:53:05.000000 RapidMangaDL-0.0.8/manga_dl/public/error.png
--rw-rw-rw-   0        0        0    86663 2023-07-11 11:07:20.000000 RapidMangaDL-0.0.8/manga_dl/public/jquery321.js
--rw-rw-rw-   0        0        0   215111 2023-07-11 11:38:35.000000 RapidMangaDL-0.0.8/manga_dl/public/loading-fast.gif
--rw-rw-rw-   0        0        0     6615 2023-07-16 06:37:18.000000 RapidMangaDL-0.0.8/manga_dl/public/manga.js
--rw-rw-rw-   0        0        0     3421 2023-07-16 14:02:35.000000 RapidMangaDL-0.0.8/manga_dl/public/search.js
--rw-rw-rw-   0        0        0     4075 2023-07-16 08:35:36.000000 RapidMangaDL-0.0.8/manga_dl/public/style.css
-drwxrwxrwx   0        0        0        0 2023-07-17 08:45:44.503527 RapidMangaDL-0.0.8/manga_dl/templates/
--rw-rw-rw-   0        0        0     3699 2023-07-14 18:32:29.000000 RapidMangaDL-0.0.8/manga_dl/templates/chapter.html
--rw-rw-rw-   0        0        0     3200 2023-07-16 13:24:25.000000 RapidMangaDL-0.0.8/manga_dl/templates/layout.html
--rw-rw-rw-   0        0        0    13010 2023-07-16 06:36:57.000000 RapidMangaDL-0.0.8/manga_dl/templates/manga.html
--rw-rw-rw-   0        0        0     2287 2023-07-16 14:00:18.000000 RapidMangaDL-0.0.8/manga_dl/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-07-17 08:45:44.526525 RapidMangaDL-0.0.8/manga_dl/tools/
--rw-rw-rw-   0        0        0      130 2023-07-15 17:00:11.000000 RapidMangaDL-0.0.8/manga_dl/tools/__init__.py
--rw-rw-rw-   0        0        0     8192 2023-07-13 14:27:12.000000 RapidMangaDL-0.0.8/manga_dl/tools/create_pdf.py
--rw-rw-rw-   0        0        0     9657 2023-07-13 17:42:34.000000 RapidMangaDL-0.0.8/manga_dl/tools/download.py
--rw-rw-rw-   0        0        0     6643 2023-07-16 17:18:45.000000 RapidMangaDL-0.0.8/manga_dl/tools/downloader2.py
--rw-rw-rw-   0        0        0     8588 2023-07-14 13:14:30.000000 RapidMangaDL-0.0.8/manga_dl/tools/downloader3.py
--rw-rw-rw-   0        0        0      188 2023-07-16 05:40:17.000000 RapidMangaDL-0.0.8/manga_dl/tools/exceptions.py
--rw-rw-rw-   0        0        0     1323 2023-07-16 05:03:19.000000 RapidMangaDL-0.0.8/manga_dl/tools/models.py
--rw-rw-rw-   0        0        0    22761 2023-07-16 14:34:36.000000 RapidMangaDL-0.0.8/manga_dl/tools/sources.py
--rw-rw-rw-   0        0        0     4435 2023-07-16 15:16:03.000000 RapidMangaDL-0.0.8/manga_dl/tools/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-17 08:45:44.537530 RapidMangaDL-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2187 2023-07-17 08:45:35.000000 RapidMangaDL-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:31.893278 RapidMangaDL-0.0.9/
+-rw-rw-rw-   0        0        0     4716 2023-07-17 09:53:31.892298 RapidMangaDL-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3312 2023-07-17 08:26:28.000000 RapidMangaDL-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:31.806657 RapidMangaDL-0.0.9/RapidMangaDL.egg-info/
+-rw-rw-rw-   0        0        0     4716 2023-07-17 09:53:30.000000 RapidMangaDL-0.0.9/RapidMangaDL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-07-17 09:53:31.000000 RapidMangaDL-0.0.9/RapidMangaDL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:53:30.000000 RapidMangaDL-0.0.9/RapidMangaDL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-17 09:53:30.000000 RapidMangaDL-0.0.9/RapidMangaDL.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      190 2023-07-17 09:53:30.000000 RapidMangaDL-0.0.9/RapidMangaDL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 09:53:30.000000 RapidMangaDL-0.0.9/RapidMangaDL.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:31.815252 RapidMangaDL-0.0.9/manga_dl/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:52:51.000000 RapidMangaDL-0.0.9/manga_dl/__init__.py
+-rw-rw-rw-   0        0        0     6632 2023-07-17 09:14:07.000000 RapidMangaDL-0.0.9/manga_dl/app.py
+-rw-rw-rw-   0        0        0      309 2023-07-11 07:46:25.000000 RapidMangaDL-0.0.9/manga_dl/jsconfig.json
+-rw-rw-rw-   0        0        0     6332 2023-07-17 09:40:48.000000 RapidMangaDL-0.0.9/manga_dl/main.py
+-rw-rw-rw-   0        0        0    23646 2023-07-17 09:48:24.000000 RapidMangaDL-0.0.9/manga_dl/manga.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:31.844258 RapidMangaDL-0.0.9/manga_dl/public/
+-rw-rw-rw-   0        0        0   232918 2023-07-11 11:05:36.000000 RapidMangaDL-0.0.9/manga_dl/public/bootstrap530.css
+-rw-rw-rw-   0        0        0    80427 2023-07-11 11:07:47.000000 RapidMangaDL-0.0.9/manga_dl/public/bootstrap530.js
+-rw-rw-rw-   0        0        0    65212 2023-07-10 06:53:05.000000 RapidMangaDL-0.0.9/manga_dl/public/error.png
+-rw-rw-rw-   0        0        0    86663 2023-07-11 11:07:20.000000 RapidMangaDL-0.0.9/manga_dl/public/jquery321.js
+-rw-rw-rw-   0        0        0   215111 2023-07-11 11:38:35.000000 RapidMangaDL-0.0.9/manga_dl/public/loading-fast.gif
+-rw-rw-rw-   0        0        0     6615 2023-07-16 06:37:18.000000 RapidMangaDL-0.0.9/manga_dl/public/manga.js
+-rw-rw-rw-   0        0        0     3421 2023-07-16 14:02:35.000000 RapidMangaDL-0.0.9/manga_dl/public/search.js
+-rw-rw-rw-   0        0        0     4075 2023-07-16 08:35:36.000000 RapidMangaDL-0.0.9/manga_dl/public/style.css
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:31.858260 RapidMangaDL-0.0.9/manga_dl/templates/
+-rw-rw-rw-   0        0        0     3699 2023-07-14 18:32:29.000000 RapidMangaDL-0.0.9/manga_dl/templates/chapter.html
+-rw-rw-rw-   0        0        0     3200 2023-07-16 13:24:25.000000 RapidMangaDL-0.0.9/manga_dl/templates/layout.html
+-rw-rw-rw-   0        0        0    13010 2023-07-16 06:36:57.000000 RapidMangaDL-0.0.9/manga_dl/templates/manga.html
+-rw-rw-rw-   0        0        0     2287 2023-07-16 14:00:18.000000 RapidMangaDL-0.0.9/manga_dl/templates/search.html
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:31.885285 RapidMangaDL-0.0.9/manga_dl/tools/
+-rw-rw-rw-   0        0        0      130 2023-07-15 17:00:11.000000 RapidMangaDL-0.0.9/manga_dl/tools/__init__.py
+-rw-rw-rw-   0        0        0     8192 2023-07-13 14:27:12.000000 RapidMangaDL-0.0.9/manga_dl/tools/create_pdf.py
+-rw-rw-rw-   0        0        0     9652 2023-07-17 09:15:36.000000 RapidMangaDL-0.0.9/manga_dl/tools/download.py
+-rw-rw-rw-   0        0        0     6621 2023-07-17 09:51:56.000000 RapidMangaDL-0.0.9/manga_dl/tools/downloader2.py
+-rw-rw-rw-   0        0        0     8588 2023-07-14 13:14:30.000000 RapidMangaDL-0.0.9/manga_dl/tools/downloader3.py
+-rw-rw-rw-   0        0        0      188 2023-07-16 05:40:17.000000 RapidMangaDL-0.0.9/manga_dl/tools/exceptions.py
+-rw-rw-rw-   0        0        0     1323 2023-07-16 05:03:19.000000 RapidMangaDL-0.0.9/manga_dl/tools/models.py
+-rw-rw-rw-   0        0        0    22708 2023-07-17 09:17:08.000000 RapidMangaDL-0.0.9/manga_dl/tools/sources.py
+-rw-rw-rw-   0        0        0     4444 2023-07-17 09:26:50.000000 RapidMangaDL-0.0.9/manga_dl/tools/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:53:31.893278 RapidMangaDL-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2187 2023-07-17 09:53:13.000000 RapidMangaDL-0.0.9/setup.py
```

### Comparing `RapidMangaDL-0.0.8/PKG-INFO` & `RapidMangaDL-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.0.8
+Version: 0.0.9
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
```

### Comparing `RapidMangaDL-0.0.8/README.md` & `RapidMangaDL-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/RapidMangaDL.egg-info/PKG-INFO` & `RapidMangaDL-0.0.9/RapidMangaDL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.0.8
+Version: 0.0.9
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
```

### Comparing `RapidMangaDL-0.0.8/RapidMangaDL.egg-info/SOURCES.txt` & `RapidMangaDL-0.0.9/RapidMangaDL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/app.py` & `RapidMangaDL-0.0.9/manga_dl/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,15 @@
     mangas = Manga.search(query)
     return render_template("search.html", results=mangas, query=query)
 
 
 @app.route("/manga/<string:manga_id>", methods=["GET"])
 def manga(manga_id):
     manga = Manga.from_id(manga_id)
-    try:
-        manga.set_info()
-    except Exception as e:
-        logger.error(e, exc_info=True)
+    manga.set_info()
 
     for chapter in manga.chapters:
         if chapter[0].endswith("/"):
             chapter[0] = chapter[0][:-1]
         chapter[0] = f"/manga/{manga_id}/{chapter[0].split('/')[-1]}"
 
     chapters = [chapter.to_json() for chapter in manga.chapters]
@@ -70,18 +67,15 @@
 def url_decode(s):
     return "".join([chr(int(i)) for i in s.split("-")])
 
 
 @app.route("/manga/<string:manga_id>/<string:chapter>", methods=["GET"])
 def manga_chapters(manga_id, chapter):
     manga = Manga.from_id(manga_id)
-    try:
-        manga.set_info()
-    except Exception as e:
-        logger.error(e, exc_info=True)
+    manga.set_info()
 
     chapter_url = None
     chapter_idx = -1
     fchapter = None
     for idx, c in enumerate(manga.chapters):
         if c[0].endswith("/"):
             c[0] = c[0][:-1]
@@ -130,15 +124,15 @@
             results = [i.to_json() for i in mangas]
         else:
             suc = False
             error = "No query provided"
     except Exception as e:
         suc = False
         error = "Unknown error"
-        logger.error(e, exc_info=True)
+        logger.error(f"Error getting search results: {e}")
 
     data = {
         "success": suc,
         "results": results,
     }
 
     if error:
@@ -164,15 +158,14 @@
     if start_url.endswith("/"):
         start_url = start_url[:-1]
     if end_url.endswith("/"):
         end_url = end_url[:-1]
 
 
     quality = int(quality)
-
     print("Download:",manga_id, start_url, end_url, quality, dtypes)
 
     manga = Manga.from_id(manga_id)
     manga.set_info()
     
     url = manga.url
     if url.endswith("/"):
@@ -191,15 +184,15 @@
             if dtype == "pdf":
                 path = manga.create_pdf(quality=quality)
             else:
                 path = manga.create_epub(quality=quality)
             paths.append(os.path.abspath(path))
         data["paths"] = paths
     except Exception as e:
-        logger.error(e, exc_info=True)
+        logger.error(f"Error downloading manga: {e}")
         data["success"] = False
         data["message"] = "Unknown error"
 
     isDownloading.value = 0  # type: ignore
 
     return jsonify(data)
```

### Comparing `RapidMangaDL-0.0.8/manga_dl/main.py` & `RapidMangaDL-0.0.9/manga_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,16 +182,16 @@
 def main():
     try:
         parser()
     except KeyboardInterrupt:
         print("Goodbye!")
         sys.exit(0)
     except Exception as e:
-        logger.error("An error occured", exc_info=True)
-        logger.info("Rest assured, all downloaded files are automatically cached.")
+        logger.error(f"Unexpected error occured {e}")
+        logger.info("Rest assured, all downloaded files are automatically cached. Run the program again to continue downloading.")
         sys.exit(1)
         
 
 if __name__ == "__main__":
     main()
```

### Comparing `RapidMangaDL-0.0.8/manga_dl/manga.py` & `RapidMangaDL-0.0.9/manga_dl/manga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pprint
 from typing import Union
 import concurrent.futures as cf
 from ebooklib import epub
 import re
 import requests
 import os
-from alive_progress import alive_bar
+from tqdm.auto import tqdm
 import shutil
 
 from PIL import Image
 from fuzzywuzzy import fuzz
 
 
 # add tools to sys.path
@@ -415,30 +415,30 @@
     def check_img(self, file):
         _, filename = file
         path = os.path.join(self.temp_dir, filename)
         try:
             Image.open(path).close()
             return True, file
         except Exception as e:
-            logger.error(f"Manga(check_img): Failed to open {path}", exc_info=True)
+            logger.error(f"Manga(check_img): Failed to open {path}: {e}")
             return False, file
 
     def check_imgs(self, files):
         success = []
         failure = []
         with cf.ThreadPoolExecutor() as executor:
             futures = [executor.submit(self.check_img, file) for file in files]
-            with alive_bar(len(futures), title="Checking images") as bar:
+            with tqdm(total=len(futures), desc="Checking images") as bar:
                 for future in cf.as_completed(futures):
                     success_, file = future.result()
                     if success_:
                         success.append(file)
                     else:
                         failure.append(file)
-                    bar()
+                    bar.update(1)
         return success, failure
 
     def remove_files(self, filenames):
         for filename in filenames:
             path = os.path.join(self.temp_dir, filename)
             if os.path.exists(path):
                 os.remove(path)
@@ -447,17 +447,17 @@
         self, book: Union[epub.EpubBook, PDF], quality=None
     ) -> Union[list[epub.EpubHtml], list[PDFChapter]]:
         if quality == 100:
             quality = None
 
         with cf.ThreadPoolExecutor() as executor:
             futures = [executor.submit(i.get_chapter_imgs) for i in self.chapters]
-            with alive_bar(len(futures), title="Getting chapter Imgs") as bar:
+            with tqdm(total=len(futures), desc="Getting Chapter Imgs") as bar:
                 for future in cf.as_completed(futures):
-                    bar()
+                    bar.update(1)
 
         img_urls = []
         img_url_to_chapter: dict[str, Chapter] = {}
         for chapter in self.chapters:
             chapter_imgs = chapter.img_urls
             img_urls.extend(chapter_imgs)
             for img_url in chapter_imgs:
@@ -504,22 +504,22 @@
 
         if quality is not None:
             with cf.ThreadPoolExecutor() as executor:
                 futures = [
                     executor.submit(self.lower_quality, i, quality)
                     for i in img_filenames_chapter.keys()
                 ]
-                with alive_bar(
-                    len(futures), title=f"Lowering quality to {quality}"
+                with tqdm(
+                    total=len(futures), decc=f"Lowering quality to {quality}"
                 ) as bar:
                     for future in cf.as_completed(futures):
                         filename, qfilename = future.result()
                         chapter = img_filenames_chapter[filename]
                         chapter.add_qfile((filename, qfilename))
-                        bar()
+                        bar.update(1)
 
             for chapter in self.chapters:
                 chapter.order_qfiles()
 
         items = []
         for chapter in self.chapters:
             title = chapter.title
@@ -553,19 +553,19 @@
 
             def create_chapter(item):
                 title, paths = item
                 return book.create_chapter(title, paths)
 
             nitems = items.copy()
             items = []
-            with alive_bar(total=len(items), title="Creating PDF chapters") as bar:
+            with tqdm(total=len(items), desc="Creating PDF chapters") as bar:
                 with cf.ThreadPoolExecutor() as executor:
                     for item in executor.map(create_chapter, nitems):
                         items.append(item)
-                        bar()
+                        bar.update(1)
 
         return items
 
     def create_epub(self, quality=None, path: str = ""):
         book = epub.EpubBook()
 
         self._quality = quality
```

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/bootstrap530.css` & `RapidMangaDL-0.0.9/manga_dl/public/bootstrap530.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/bootstrap530.js` & `RapidMangaDL-0.0.9/manga_dl/public/bootstrap530.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/error.png` & `RapidMangaDL-0.0.9/manga_dl/public/error.png`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/jquery321.js` & `RapidMangaDL-0.0.9/manga_dl/public/jquery321.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/loading-fast.gif` & `RapidMangaDL-0.0.9/manga_dl/public/loading-fast.gif`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/manga.js` & `RapidMangaDL-0.0.9/manga_dl/public/manga.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/search.js` & `RapidMangaDL-0.0.9/manga_dl/public/search.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/public/style.css` & `RapidMangaDL-0.0.9/manga_dl/public/style.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/templates/chapter.html` & `RapidMangaDL-0.0.9/manga_dl/templates/chapter.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/templates/layout.html` & `RapidMangaDL-0.0.9/manga_dl/templates/layout.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/templates/manga.html` & `RapidMangaDL-0.0.9/manga_dl/templates/manga.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/templates/search.html` & `RapidMangaDL-0.0.9/manga_dl/templates/search.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/tools/create_pdf.py` & `RapidMangaDL-0.0.9/manga_dl/tools/create_pdf.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/tools/download.py` & `RapidMangaDL-0.0.9/manga_dl/tools/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,30 @@
         self.save_queue = Queue()
     
     def delete_file(self, path: str):
         try:
             if os.path.exists(path):
                 os.remove(path)
         except Exception as e:
-            logger.error(f"Failed to delete {path}")
+            logger.error(f"Failed to delete {path}: {e}")
     
     def convert_to_jpeg(self, path: str):
         save_path = jpeg_file(path)
         if os.path.exists(save_path):
             self.save_queue.put((path, save_path))
             return save_path
         try:
             im = Image.open(path)
             im.convert("RGB").save(save_path, "JPEG", optimize=True, quality=85)
             im.close()
             self.delete_file(path)
             self.save_queue.put((path, save_path))
             return save_path
         except Exception as e:
-            logger.error(f"Failed to convert {path} to jpeg", exc_info=True)
+            logger.error(f"Failed to convert {path} to jpeg: {e}")
             self.save_queue.put((path, path))
             return path
         
     def convert_to_jpegs(self, paths: list[str]) -> list[tuple[str, str]]: # list[original_path, jpeg_path]
         with tqdm(total=len(paths), desc="Converting to jpeg") as pbar:
             with cf.ThreadPoolExecutor() as executor:
                 futures = [executor.submit(self.convert_to_jpeg, path) for path in paths]
```

### Comparing `RapidMangaDL-0.0.8/manga_dl/tools/downloader2.py` & `RapidMangaDL-0.0.9/manga_dl/tools/downloader2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import json
 import logging
 from multiprocessing import Manager
 import hashlib
 import aiofiles
-from alive_progress import alive_bar
 import requests
 from fake_headers import Headers
 import time
 from .utils import (
     create_failure_image,
     compress_file_path,
     get_file_name,
     jpeg_compress,
     safe_remove,
     auto_scaled_divide,
 )
 from .models import URLFile
 import asyncio
 import aiohttp
+from tqdm.auto import tqdm
 
 import platform
 
 if platform.system() == "Windows":
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 logger_name = os.environ.get("LOGGER_NAME", "manga")
@@ -95,20 +95,20 @@
 
                 self.downloaded_files.append(URLFile(url, filepath))
 
             except Exception as e:
                 print(f"Failed to download {url}: {e}")
                 self.failed_urls.append(url)
                 return
-        pbar()
+        pbar.update(1)
         self.share_pbar()
         self.total_urls -= 1
 
     async def download_all(self):
-        with alive_bar(total=len(self.urls), bar="smooth", title="Downloading") as pbar:
+        with tqdm(total=len(self.urls), desc="Downloading") as pbar:
             timeout = aiohttp.ClientTimeout(total=auto_scaled_divide(self.total_urls))
             async with aiohttp.ClientSession(
                 headers=self.headers, timeout=timeout
             ) as session:
                 tasks = []
                 for url in self.urls:
                     task = asyncio.create_task(self.download_file(session, url, pbar))
```

### Comparing `RapidMangaDL-0.0.8/manga_dl/tools/downloader3.py` & `RapidMangaDL-0.0.9/manga_dl/tools/downloader3.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/tools/models.py` & `RapidMangaDL-0.0.9/manga_dl/tools/models.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.8/manga_dl/tools/sources.py` & `RapidMangaDL-0.0.9/manga_dl/tools/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,26 +180,24 @@
             try:
                 with open(path, "r") as f:
                     data = json.load(f)
                     if not data:
                         raise Exception(f"Error loading cache from {path}")
                     return data
             except Exception as e:
-                logger.error(f"Error loading info from {path}")
-                logger.error(e)
+                logger.error(f"Error loading info from {path}: {e}")
                 safe_remove(path)
         else:
             data = func(*args, **kwargs)
             if data:
                 try:
                     with open(path, "w") as f:
                         json.dump(data, f)
                 except Exception as e:
-                    logger.error(f"Error saving info to {path}")
-                    logger.error(e)
+                    logger.error(f"Error saving info to {path}: {e}")
                     safe_remove(path)
 
             return data
 
     return wrapper
 
 
@@ -456,15 +454,15 @@
                 "views": views,
                 "rating": rating,
                 "chapters": [c.to_json() for c in chapters],
             }
             return data
 
         except Exception as e:
-            logger.error(e, exc_info=True)
+            logger.error(f"Error getting manga info for {self.url}: {e}")
             raise MangaNotFound(f"Manga not found: {self.url}")
 
     @exists
     def get_chapter_img_urls(self, chapter_url: str) -> list:
         if chapter_url.startswith("/"):
             chapter_url = f"{self.url}{chapter_url}"
 
@@ -473,15 +471,15 @@
             soup = BeautifulSoup(res.text, "html.parser")
             imgs = soup.select(".container-chapter-reader img")  # type: ignore
             imgs = [i.get("src") for i in imgs]  # type: ignore
             imgs: list[str] = [i for i in imgs if self.manganato_id in i]  # type: ignore
 
         except Exception as e:
             logger.error(
-                f"Error getting chapter images for {chapter_url}", exc_info=True
+                f"Error getting chapter images for {chapter_url}: {e}",
             )
             imgs = []
 
         return imgs
 
     @staticmethod
     def all_domains() -> list[str]:
@@ -524,15 +522,15 @@
             try:
                 with open(path, 'r') as f:
                     results = json.load(f)
                     if not results:
                         raise Exception(f"No data found in the `{query}` cache in {path}")
                 return results
             except Exception as e:
-                logger.error(f"Failed to load `{query}` cache from {path}")
+                logger.error(f"Failed to load `{query}` cache from {path}: {e}")
 
         results = []
         try:
             headers = Headers().generate()
             headers.update(
                 {
                     "referer": "https://1stkissmanga.me/",
@@ -628,15 +626,15 @@
                 "last_updated": release,
                 "total_comments": total_comments,
                 "total_bookmarked": total_bookmarked,
                 "type": type_,
             }
 
         except Exception as e:
-            logger.error(f"Error getting manga info for {self.url}", exc_info=True)
+            logger.error(f"Error getting manga info for {self.url}: {e}")
             data = {}
 
         return data
 
     @exists
     def get_chapter_img_urls(self, chapter_url: str) -> list:
         if chapter_url.startswith("/"):
@@ -646,15 +644,15 @@
             res = scraper.get(chapter_url)
             soup = BeautifulSoup(res.text, "html.parser")
             imgs = soup.select(".entry-content img")  # type: ignore
             imgs = [i.get("src") for i in imgs]  # type: ignore
 
         except Exception as e:
             logger.error(
-                f"Error getting chapter images for {chapter_url}", exc_info=True
+                f"Error getting chapter images for {chapter_url}: {e}"
             )
             imgs = []
 
         return imgs
 
 
 sources = [
```

### Comparing `RapidMangaDL-0.0.8/manga_dl/tools/utils.py` & `RapidMangaDL-0.0.9/manga_dl/tools/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import json
 from typing import Union
 from PIL import Image, ImageDraw, ImageFont
 import textwrap
 import hashlib
 import logging
 import os
 import colorama
 import re
 import math
 
 
-
 logger = logging.getLogger(os.environ.get("LOGGER_NAME", "tools"))
 _utils_path = os.path.dirname(os.path.abspath(__file__))
 error_img_path = os.path.join(os.path.dirname(_utils_path), "public", "error.png")
 
+
 def auto_scaled_divide(value):
     scaling_factor = math.log10(1 + abs(value)) * 0.5
     return math.ceil(value // scaling_factor)
 
+
 def replace_unimportant(text: str, but: Union[list, None] = None) -> str:
     # replace all characters except a-z, A-Z, 0-9, and but
     if but is None:
         but = []
     but = [re.escape(c) for c in but]
     buts = "".join(but)
     return re.sub(f"[^{buts}a-zA-Z0-9]", "", text)
@@ -55,15 +55,15 @@
 logger = logging.getLogger(logger_name)
 logger.setLevel(logging_level)
 
 file_handler = logging.FileHandler("manga.log")
 stream_handler = logging.StreamHandler()
 
 formatter = ColorFormatter(
-    "[%(levelname)s] %(asctime)s - %(message)s", datefmt="%B, %Y %I:%M %p"
+    "[%(asctime)s | %(filename)s:%(lineno)s (%(funcName)s)] %(levelname)s - %(message)s", datefmt="%I:%M %p"
 )
 file_handler.setFormatter(formatter)
 stream_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
 logger.addHandler(stream_handler)
 
 
@@ -99,15 +99,15 @@
 
 
 def safe_remove(path: str):
     if os.path.exists(path):
         try:
             os.remove(path)
         except Exception as e:
-            logger.error(f"Failed to delete {path}", exc_info=True)
+            logger.error(f"Failed to delete {path}: {e}")
 
 
 def get_hash(url: str) -> str:
     return hashlib.md5(url.encode()).hexdigest()
 
 
 def get_file_name(url: str, check_extension: bool = False):
@@ -141,9 +141,7 @@
 def http_split(txt, sep):
     parts = txt.strip().split(f"{sep}http")
     url1 = parts[0]
     rest = []
     for p in parts[1:]:
         rest.append(f"http{p}")
     return [url1] + rest
-
-
```

### Comparing `RapidMangaDL-0.0.8/setup.py` & `RapidMangaDL-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 from setuptools import setup, find_packages
 
 package_name = "RapidMangaDL"
-package_version = "0.0.8"
+package_version = "0.0.9"
 package_description = "Swiftly download manga from multiple sources."
 package_author = "sifat"
 package_author_email = "hossain0338@gmail.com"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
```

