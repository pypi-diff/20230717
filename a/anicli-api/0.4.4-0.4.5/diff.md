# Comparing `tmp/anicli_api-0.4.4.tar.gz` & `tmp/anicli_api-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli_api-0.4.4.tar", max compression
+gzip compressed data, was "anicli_api-0.4.5.tar", max compression
```

## Comparing `anicli_api-0.4.4.tar` & `anicli_api-0.4.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     4216 2023-05-15 08:36:21.974286 anicli_api-0.4.4/README.MD
--rw-r--r--   0        0        0     2940 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/_http.py
--rw-r--r--   0        0        0     1511 2023-05-15 08:36:21.974286 anicli_api-0.4.4/anicli_api/_logger.py
--rw-r--r--   0        0        0     3242 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/base.py
--rw-r--r--   0        0        0      615 2023-05-15 08:38:52.517152 anicli_api-0.4.4/anicli_api/player/__init__.py
--rw-r--r--   0        0        0      921 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/__template__.py
--rw-r--r--   0        0        0     2147 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/aniboom.py
--rw-r--r--   0        0        0     1055 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/animejoy.py
--rw-r--r--   0        0        0     3434 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/base.py
--rw-r--r--   0        0        0     1198 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/csst.py
--rw-r--r--   0        0        0     1456 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/dzen.py
--rw-r--r--   0        0        0     4047 2023-07-17 10:02:25.493422 anicli_api-0.4.4/anicli_api/player/kodik.py
--rw-r--r--   0        0        0     1837 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/mailru.py
--rw-r--r--   0        0        0     1697 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/okru.py
--rw-r--r--   0        0        0     1106 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/sibnet.py
--rw-r--r--   0        0        0     1139 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/sovetromantica.py
--rw-r--r--   0        0        0     1527 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/player/vkcom.py
--rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.4.4/anicli_api/source/__init__.py
--rw-r--r--   0        0        0     2516 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/__template__.py
--rw-r--r--   0        0        0     6163 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/anilibria.py
--rw-r--r--   0        0        0    10586 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/animego.py
--rw-r--r--   0        0        0     8722 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/animejoy.py
--rw-r--r--   0        0        0     5543 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/animevost.py
--rw-r--r--   0        0        0     6462 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/source/sovetromantica.py
--rw-r--r--   0        0        0       58 2023-05-15 08:36:21.974286 anicli_api-0.4.4/anicli_api/tools/__init__.py
--rw-r--r--   0        0        0     2704 2022-12-17 13:02:20.525429 anicli_api-0.4.4/anicli_api/tools/random_useragent.py
--rw-r--r--   0        0        0      198 2023-07-14 17:47:29.562755 anicli_api-0.4.4/anicli_api/tools/utils.py
--rw-r--r--   0        0        0     2342 2023-07-17 10:02:43.744188 anicli_api-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 anicli_api-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     4216 2023-05-15 08:36:21.974286 anicli_api-0.4.5/README.MD
+-rw-r--r--   0        0        0     2940 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/_http.py
+-rw-r--r--   0        0        0     1511 2023-05-15 08:36:21.974286 anicli_api-0.4.5/anicli_api/_logger.py
+-rw-r--r--   0        0        0     3337 2023-07-17 14:57:08.210234 anicli_api-0.4.5/anicli_api/base.py
+-rw-r--r--   0        0        0      615 2023-05-15 08:38:52.517152 anicli_api-0.4.5/anicli_api/player/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/__template__.py
+-rw-r--r--   0        0        0     2147 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/aniboom.py
+-rw-r--r--   0        0        0     1055 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/animejoy.py
+-rw-r--r--   0        0        0     3434 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/base.py
+-rw-r--r--   0        0        0     1198 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/csst.py
+-rw-r--r--   0        0        0     1456 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/dzen.py
+-rw-r--r--   0        0        0     4047 2023-07-17 10:02:25.493422 anicli_api-0.4.5/anicli_api/player/kodik.py
+-rw-r--r--   0        0        0     1837 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/mailru.py
+-rw-r--r--   0        0        0     1697 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/okru.py
+-rw-r--r--   0        0        0     1106 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/sibnet.py
+-rw-r--r--   0        0        0     1139 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/sovetromantica.py
+-rw-r--r--   0        0        0     1527 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/vkcom.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.4.5/anicli_api/source/__init__.py
+-rw-r--r--   0        0        0     2516 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/__template__.py
+-rw-r--r--   0        0        0     6163 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/anilibria.py
+-rw-r--r--   0        0        0    10795 2023-07-17 15:00:57.999414 anicli_api-0.4.5/anicli_api/source/animego.py
+-rw-r--r--   0        0        0     8722 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/animejoy.py
+-rw-r--r--   0        0        0     5543 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/animevost.py
+-rw-r--r--   0        0        0     6462 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/sovetromantica.py
+-rw-r--r--   0        0        0       58 2023-05-15 08:36:21.974286 anicli_api-0.4.5/anicli_api/tools/__init__.py
+-rw-r--r--   0        0        0     2704 2022-12-17 13:02:20.525429 anicli_api-0.4.5/anicli_api/tools/random_useragent.py
+-rw-r--r--   0        0        0      198 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/tools/utils.py
+-rw-r--r--   0        0        0     2342 2023-07-17 15:02:45.656349 anicli_api-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 anicli_api-0.4.5/PKG-INFO
```

### Comparing `anicli_api-0.4.4/README.MD` & `anicli_api-0.4.5/README.MD`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/_http.py` & `anicli_api-0.4.5/anicli_api/_http.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/_logger.py` & `anicli_api-0.4.5/anicli_api/_logger.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/base.py` & `anicli_api-0.4.5/anicli_api/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import warnings
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, List, Optional, ClassVar, Type
 
+from parsel import Selector
 from scrape_schema import BaseSchema
 
 from anicli_api._http import HTTPAsync, HTTPSync
 from anicli_api.player import ALL_DECODERS
 
 if TYPE_CHECKING:
     from anicli_api.player.base import Video
 
 
 class MainSchema(BaseSchema):
+    _Selector: ClassVar[Type[Selector]] = Selector
     HTTP = HTTPSync
     HTTP_ASYNC = HTTPAsync
 
     @classmethod
     def from_kwargs(cls, **kwargs):
         """ignore fields parse and set attrs directly"""
         cls_ = cls("")
```

### Comparing `anicli_api-0.4.4/anicli_api/player/__init__.py` & `anicli_api-0.4.5/anicli_api/player/__init__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/__template__.py` & `anicli_api-0.4.5/anicli_api/player/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/aniboom.py` & `anicli_api-0.4.5/anicli_api/player/aniboom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/animejoy.py` & `anicli_api-0.4.5/anicli_api/player/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/base.py` & `anicli_api-0.4.5/anicli_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/csst.py` & `anicli_api-0.4.5/anicli_api/player/csst.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/dzen.py` & `anicli_api-0.4.5/anicli_api/player/dzen.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/kodik.py` & `anicli_api-0.4.5/anicli_api/player/kodik.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/mailru.py` & `anicli_api-0.4.5/anicli_api/player/mailru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/okru.py` & `anicli_api-0.4.5/anicli_api/player/okru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/sibnet.py` & `anicli_api-0.4.5/anicli_api/player/sibnet.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/sovetromantica.py` & `anicli_api-0.4.5/anicli_api/player/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/player/vkcom.py` & `anicli_api-0.4.5/anicli_api/player/vkcom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/source/__template__.py` & `anicli_api-0.4.5/anicli_api/source/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/source/anilibria.py` & `anicli_api-0.4.5/anicli_api/source/anilibria.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/source/animego.py` & `anicli_api-0.4.5/anicli_api/source/animego.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     def title(self) -> str:
         return self._script_jmespath.jmespath("name").get()
 
     @sc_param
     def alt_titles(self) -> List[str]:
         return self._script_jmespath.jmespath("alternativeHeadline").getall()
 
-    episodes_available: Sc[int, Parsel(default=0).xpath("//dl/dd[2]").re(r"\d+")[0]]
+    episodes_available: Sc[int, Parsel(default=0).xpath("//dl/dd[2]/text()").re(r"\d+")[0]]
     thumbnail: Sc[str, Parsel().css("#content img").xpath("@src").get()]
     _description: Sc[List[str], Parsel().xpath("//div[@data-readmore='content']/text()").getall()]  # mobile agent
 
     @sc_param
     def description(self) -> str:
         return " ".join(s.strip() for s in self._description)
 
@@ -154,30 +154,34 @@
     def episodes_total(self) -> int:
         return int(self._script_jmespath.jmespath("numberOfEpisodes").get())
 
     @sc_param
     def aired(self) -> str:
         if end_date := self._script_jmespath.jmespath("endDate").get():
             return self._script_jmespath.jmespath("startDate").get() + " " + end_date
-        return self._script_jmespath.jmespath("startDate").get() + " " + " ?"
+        return self._script_jmespath.jmespath("startDate").get() + " " + "?"
 
     url: Sc[str, Parsel().xpath("//html/head/link[@rel='canonical']/@href").get()]
     anime_id = sc_param(lambda self: self.url.split("-")[-1])
 
     @sc_param
     def rating(self) -> float:
         return float(self._script_jmespath.jmespath("aggregateRating.ratingValue").get())
 
     @staticmethod
     def _get_dubbers(response: str) -> Dict[str, str]:
         # sel = Selector(response)
         dubbers_id: List[str] = (
             Parsel().xpath('//*[@id="video-dubbing"]/span/@data-dubbing').getall().sc_parse(response)
         )
-        dubbers_name: List[str] = Parsel().xpath('//*[@id="video-dubbing"]/span/text()').getall().sc_parse(response)
+        dubbers_name: List[str] = (Parsel()
+                                   .xpath('//*[@id="video-dubbing"]/span/span/text()')
+                                   .getall()
+                                   .fn(lambda lst: [s.strip() for s in lst])
+                                   .sc_parse(response))
         return dict(zip(dubbers_id, dubbers_name))
 
     def get_episodes(self) -> List["Episode"]:
         response = self.HTTP().get(f"https://animego.org/anime/{self.anime_id}/player?_allow=true").json()["content"]
 
         _dubbers_table = self._get_dubbers(response)
         chunks = Parsel().xpath('//*[@id="video-carousel"]/div/div').getall().sc_parse(response)
@@ -194,19 +198,19 @@
             episodes = [Episode(chunk) for chunk in chunks]
             for ep in episodes:
                 setattr(ep, "_dubbers_table", _dubbers_table)
             return episodes
 
 
 class Episode(BaseEpisode):
+    _episode_type: Sc[int, Parsel().xpath("//div/@data-episode-type").get()]
+    _dubbers_table: Dict[str, str] # setattr
     num: Sc[int, Parsel().xpath("//div/@data-episode").get()]
     title: Sc[str, Parsel().xpath("//div/@data-episode-title").get()]
 
-    _episode_type: Sc[int, Parsel().xpath("//div/@data-episode-type").get()]
-    _dubbers_table: Dict[str, str]
     data_id: Sc[int, Parsel().xpath("//div/@data-id").get()]
     released: Sc[str, Parsel().xpath("//div/@data-episode-released").get()]
 
     def __str__(self):
         return f"{self.title} {self.num} {self.released}"
 
     def get_sources(self) -> List["Source"]:
@@ -239,15 +243,15 @@
 
 
 class Source(BaseSource):
     _dubbers_table: Dict[str, str]
     _url: Sc[str, Parsel().xpath("//span/@data-player").get()]
     _data_provider: Sc[str, Parsel().xpath("//span/@data-provider").get()]
     _data_provide_dubbing: Sc[str, Parsel().xpath("//span/@data-provide-dubbing").get()]
-    name: Sc[str, Parsel().xpath("//span/span/@text").get()]
+    name: Sc[str, Parsel().xpath("//span/span/text()").get()]
     url = sc_param(lambda self: f"https:{self._url}")
     dub = sc_param(lambda self: self._dubbers_table.get(self._data_provide_dubbing))
 
     def __str__(self):
         return f"{urlsplit(self.url).netloc} {self.name} ({self.dub})"
```

### Comparing `anicli_api-0.4.4/anicli_api/source/animejoy.py` & `anicli_api-0.4.5/anicli_api/source/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/source/animevost.py` & `anicli_api-0.4.5/anicli_api/source/animevost.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/source/sovetromantica.py` & `anicli_api-0.4.5/anicli_api/source/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/anicli_api/tools/random_useragent.py` & `anicli_api-0.4.5/anicli_api/tools/random_useragent.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.4/pyproject.toml` & `anicli_api-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anicli_api"
-version = "0.4.4"
+version = "0.4.5"
 description = "Anime extractor api implementation"
 authors = ["Georgiy aka Vypivshiy"]
 license = "MIT"
 readme = "README.MD"
 packages = [{include = "anicli_api"}]
 exclude = ["tests/"]
 keywords = [
```

### Comparing `anicli_api-0.4.4/PKG-INFO` & `anicli_api-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anicli-api
-Version: 0.4.4
+Version: 0.4.5
 Summary: Anime extractor api implementation
 License: MIT
 Keywords: anime,api,ru,russia,asyncio,parser,httpx,dev
 Author: Georgiy aka Vypivshiy
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

