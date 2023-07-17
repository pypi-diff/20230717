# Comparing `tmp/pyjlyric-0.0.2.tar.gz` & `tmp/pyjlyric-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjlyric-0.0.2.tar", max compression
+gzip compressed data, was "pyjlyric-1.0.0.tar", max compression
```

## Comparing `pyjlyric-0.0.2.tar` & `pyjlyric-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1076 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/LICENSE
--rw-r--r--   0        0        0     2676 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/README.md
--rw-r--r--   0        0        0      156 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/__init__.py
--rw-r--r--   0        0        0      137 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/animap/__init__.py
--rw-r--r--   0        0        0      144 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/animap/model.py
--rw-r--r--   0        0        0     2201 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/animap/parser.py
--rw-r--r--   0        0        0      817 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/base.py
--rw-r--r--   0        0        0      137 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/evesta/__init__.py
--rw-r--r--   0        0        0      203 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/evesta/model.py
--rw-r--r--   0        0        0     2466 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/evesta/parser.py
--rw-r--r--   0        0        0      133 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/gakki/__init__.py
--rw-r--r--   0        0        0      164 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/gakki/model.py
--rw-r--r--   0        0        0     2591 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/gakki/parser.py
--rw-r--r--   0        0        0      133 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/hoick/__init__.py
--rw-r--r--   0        0        0      684 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/hoick/model.py
--rw-r--r--   0        0        0     2581 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/hoick/parser.py
--rw-r--r--   0        0        0      137 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/jlyric/__init__.py
--rw-r--r--   0        0        0      203 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/jlyric/model.py
--rw-r--r--   0        0        0     3107 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/jlyric/parser.py
--rw-r--r--   0        0        0      145 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/joysound/__init__.py
--rw-r--r--   0        0        0     4369 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/joysound/model.py
--rw-r--r--   0        0        0     2416 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/joysound/parser.py
--rw-r--r--   0        0        0      137 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/jtotal/__init__.py
--rw-r--r--   0        0        0      165 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/jtotal/model.py
--rw-r--r--   0        0        0     2717 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/jtotal/parser.py
--rw-r--r--   0        0        0      149 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/kashinavi/__init__.py
--rw-r--r--   0        0        0     1182 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/kashinavi/model.py
--rw-r--r--   0        0        0     2154 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/kashinavi/parser.py
--rw-r--r--   0        0        0     1606 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/main.py
--rw-r--r--   0        0        0      653 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/model.py
--rw-r--r--   0        0        0      149 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/musicbook/__init__.py
--rw-r--r--   0        0        0      493 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/musicbook/model.py
--rw-r--r--   0        0        0     3065 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/musicbook/parser.py
--rw-r--r--   0        0        0     2727 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/parse.py
--rw-r--r--   0        0        0      157 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/petitlyrics/__init__.py
--rw-r--r--   0        0        0      894 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/petitlyrics/model.py
--rw-r--r--   0        0        0     3520 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/petitlyrics/parser.py
--rw-r--r--   0        0        0        0 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/py.typed
--rw-r--r--   0        0        0      137 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/utamap/__init__.py
--rw-r--r--   0        0        0      144 2023-03-07 17:26:29.519329 pyjlyric-0.0.2/pyjlyric/utamap/model.py
--rw-r--r--   0        0        0     2084 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/utamap/parser.py
--rw-r--r--   0        0        0      137 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/utanet/__init__.py
--rw-r--r--   0        0        0      268 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/utanet/model.py
--rw-r--r--   0        0        0     3274 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/utanet/parser.py
--rw-r--r--   0        0        0      137 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/utaten/__init__.py
--rw-r--r--   0        0        0      268 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/utaten/model.py
--rw-r--r--   0        0        0     4173 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/utaten/parser.py
--rw-r--r--   0        0        0     2962 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyjlyric/util.py
--rw-r--r--   0        0        0     1978 2023-03-07 17:26:29.523329 pyjlyric-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 pyjlyric-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2676 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/README.md
+-rw-r--r--   0        0        0      156 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/__init__.py
+-rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/animap/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/animap/model.py
+-rw-r--r--   0        0        0     2201 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/animap/parser.py
+-rw-r--r--   0        0        0      817 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/base.py
+-rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/evesta/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/evesta/model.py
+-rw-r--r--   0        0        0     2466 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/evesta/parser.py
+-rw-r--r--   0        0        0      133 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/gakki/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/gakki/model.py
+-rw-r--r--   0        0        0     2589 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/gakki/parser.py
+-rw-r--r--   0        0        0      133 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/hoick/__init__.py
+-rw-r--r--   0        0        0      648 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/hoick/model.py
+-rw-r--r--   0        0        0     2557 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/hoick/parser.py
+-rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jlyric/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jlyric/model.py
+-rw-r--r--   0        0        0     3107 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jlyric/parser.py
+-rw-r--r--   0        0        0      145 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/joysound/__init__.py
+-rw-r--r--   0        0        0     4363 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/joysound/model.py
+-rw-r--r--   0        0        0     2426 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/joysound/parser.py
+-rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jtotal/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jtotal/model.py
+-rw-r--r--   0        0        0     2717 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/jtotal/parser.py
+-rw-r--r--   0        0        0      149 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/kashinavi/__init__.py
+-rw-r--r--   0        0        0      890 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/kashinavi/model.py
+-rw-r--r--   0        0        0     2599 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/kashinavi/parser.py
+-rw-r--r--   0        0        0     1606 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/main.py
+-rw-r--r--   0        0        0      681 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/model.py
+-rw-r--r--   0        0        0      149 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/musicbook/__init__.py
+-rw-r--r--   0        0        0      529 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/musicbook/model.py
+-rw-r--r--   0        0        0     3063 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/musicbook/parser.py
+-rw-r--r--   0        0        0     2713 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/parse.py
+-rw-r--r--   0        0        0      157 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/petitlyrics/__init__.py
+-rw-r--r--   0        0        0      985 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/petitlyrics/model.py
+-rw-r--r--   0        0        0     3538 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/petitlyrics/parser.py
+-rw-r--r--   0        0        0        0 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/py.typed
+-rw-r--r--   0        0        0      137 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utamap/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utamap/model.py
+-rw-r--r--   0        0        0     2084 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utamap/parser.py
+-rw-r--r--   0        0        0      137 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utanet/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utanet/model.py
+-rw-r--r--   0        0        0     3274 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utanet/parser.py
+-rw-r--r--   0        0        0      137 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utaten/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utaten/model.py
+-rw-r--r--   0        0        0     4173 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utaten/parser.py
+-rw-r--r--   0        0        0     2943 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/util.py
+-rw-r--r--   0        0        0     2120 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 pyjlyric-1.0.0/PKG-INFO
```

### Comparing `pyjlyric-0.0.2/LICENSE` & `pyjlyric-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/README.md` & `pyjlyric-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/animap/parser.py` & `pyjlyric-1.0.0/pyjlyric/animap/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/base.py` & `pyjlyric-1.0.0/pyjlyric/base.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/evesta/parser.py` & `pyjlyric-1.0.0/pyjlyric/evesta/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/gakki/parser.py` & `pyjlyric-1.0.0/pyjlyric/gakki/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         artist = select_one_tag(bs, "#topics > ol > li:nth-child(2) > a")
 
         lyric_chars = []
         for div in bs.select("div#chord_area > div"):
             if div.get("class") is None:
                 lyric_chars.append("\n")
             else:
-                lyric_chars.extend(d.text for d in div.select("div.cd_pic.blue > div") if d.text.strip() != "")
+                lyric_chars.extend(d.text for d in div.select("div.cd_pic.blue > div") if not d.text.strip())
 
         lyric_lines = [i.replace("\n", "") for i in "\n".join(lyric_chars).strip().split("\n\n\n")]
 
         return GakkiLyricPage(
             title=select_one_tag(bs, "div.info > h2.tit > span").text[1:-1],
             page_url=parse_obj_as_url(url),
             pageid=pageid,
```

### Comparing `pyjlyric-0.0.2/pyjlyric/hoick/model.py` & `pyjlyric-1.0.0/pyjlyric/hoick/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from collections.abc import Iterator
 from typing import List, Type
 
-from pydantic import BaseModel, validator
+from pydantic import RootModel, field_validator
 from typing_extensions import Self
 
 from pyjlyric.model import LyricPage, WithUrlText
 
 
 class HoickLyricPage(LyricPage):
     artist: None
     composer: List[WithUrlText]
     lyricist: List[WithUrlText]
     arranger: None
 
 
-class HoickLyricData(BaseModel):
-    __root__: List[str]
-
+class HoickLyricData(RootModel[List[str]]):
     def __iter__(self: Self) -> Iterator[str]:  # type: ignore[override]
-        return iter(self.__root__)
+        return iter(self.root)
 
-    @validator("__root__")
+    @field_validator("root")
     @classmethod
-    def validate(cls: Type[Self], v: List[str]) -> List[str]:  # type: ignore[override]
+    def validate(cls: Type[Self], v: List[str]) -> List[str]:
         return [i for i in v if isinstance(i, str)]
```

### Comparing `pyjlyric-0.0.2/pyjlyric/hoick/parser.py` & `pyjlyric-1.0.0/pyjlyric/hoick/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,21 +55,19 @@
             for a in select_one_tag(header_div, "h2.music").select("a")
             if a.href is not None
         ]
 
         bs_lyric = get_source(f"https://hoick.jp/data.php?id={pageid}&type=4")
         if bs_lyric is None:
             raise HoickLyricPageParserError from ConnectionError
-        lyric_lines = HoickLyricData.parse_raw(bs_lyric.text)
+        lyric_lines = HoickLyricData.model_validate_json(bs_lyric.text)
 
         return HoickLyricPage(
             title=select_one_tag(bs, "h1.detail").text,
             page_url=parse_obj_as_url(url),
             pageid=pageid,
             artist=None,
             composer=composers,
             lyricist=lyricists,
             arranger=None,
-            lyric_sections=[
-                section.strip().split("\r") for section in "".join(lyric_lines.__root__[:-1]).split("\r\r")
-            ],
+            lyric_sections=[section.strip().split("\r") for section in "".join(lyric_lines.root[:-1]).split("\r\r")],
         )
```

### Comparing `pyjlyric-0.0.2/pyjlyric/jlyric/parser.py` & `pyjlyric-1.0.0/pyjlyric/jlyric/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/joysound/model.py` & `pyjlyric-1.0.0/pyjlyric/joysound/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pydantic import BaseModel, Field
 
 from pyjlyric.model import LyricPage, WithUrlText
 
 
 class JoysoundLyricPage(LyricPage):
     artist: WithUrlText
-    composer: Optional[str]
-    lyricist: Optional[str]
+    composer: Optional[str] = None
+    lyricist: Optional[str] = None
     arranger: None
 
 
 class _LyricListItem(BaseModel):
     service_type: str = Field(..., alias="serviceType")
     service_publish_date: str = Field(..., alias="ServicePublishDate")
     status_code: str = Field(..., alias="statusCode")
@@ -92,9 +92,9 @@
     artist_name_ruby_sort: str = Field(..., alias="artistNameRubySort")
     artist_name_alphabet_search_sort: str = Field(..., alias="artistNameAlphabetSearchSort")
     artist_name_foreign: str = Field(..., alias="artistNameForeign")
     artist_name_foreign_search: str = Field(..., alias="artistNameForeignSearch")
     artist_name_foreign_sort: str = Field(..., alias="artistNameForeignSort")
     artist_dv: str = Field(..., alias="artistDv")
     myartist_flg: str = Field(..., alias="myartistFlg")
-    lyric_list: List[_LyricListItem] = Field(..., exclusiveMinimum=1, alias="lyricList")
+    lyric_list: List[_LyricListItem] = Field(..., alias="lyricList")
     outside_url_info: _OutsideUrlInfo = Field(..., alias="outsideUrlInfo")
```

### Comparing `pyjlyric-0.0.2/pyjlyric/joysound/parser.py` & `pyjlyric-1.0.0/pyjlyric/joysound/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             headers={
                 "x-jsp-app-name": "0000800",
             },
         )
         if bs is None:
             raise JoysoundLyricPageParserError from ConnectionError
 
-        track_data = JoysoundLyricData.parse_raw(bs.text)
+        track_data = JoysoundLyricData.model_validate_json(bs.text)
 
         return JoysoundLyricPage(
             title=track_data.song_name,
             page_url=parse_obj_as_url(url),
             pageid=pageid,
             artist=WithUrlText(
                 text=track_data.artist_name,
```

### Comparing `pyjlyric-0.0.2/pyjlyric/jtotal/parser.py` & `pyjlyric-1.0.0/pyjlyric/jtotal/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/kashinavi/model.py` & `pyjlyric-1.0.0/pyjlyric/kashinavi/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,22 +31,12 @@
 
 class _Lyrics(BaseModel):
     _type: str = Field(..., alias="@type")
     main_entity_of_page: _MainEntityOfPage = Field(..., alias="mainEntityOfPage")
     text: str
 
 
-class JSONLD(BaseModel):
-    _context: str = Field(..., alias="@context")
-    _type: str = Field(..., alias="@type")
-    name: str
-    recorded_as: _RecordedAs = Field(..., alias="recordedAs")
-    lyricist: _Lyricist
-    composer: _Composer
-    lyrics: _Lyrics = Field(..., alias="Lyrics")
-
-
 class KashinaviLyricPage(LyricPage):
     artist: WithUrlText
     composer: str
     lyricist: str
     arranger: None
```

### Comparing `pyjlyric-0.0.2/pyjlyric/kashinavi/parser.py` & `pyjlyric-1.0.0/pyjlyric/musicbook/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,77 @@
-"""<https://kashinavi.com>"""
+"""<https://music-book.jp>"""
 
 import re
 
-from bs4 import BeautifulSoup, NavigableString, Tag
-
 from pyjlyric.base import BaseLyricPageParser, BaseLyricPageParserError
 from pyjlyric.model import WithUrlText
-from pyjlyric.util import get_captured_value, get_source, parse_obj_as_url
+from pyjlyric.util import convert_lines_into_sections, get_captured_value, get_source, parse_obj_as_url, select_one_tag
 
-from .model import JSONLD, KashinaviLyricPage
+from .model import MusicbookLyricData, MusicbookLyricPage
 
-_KASHINAVI_PATTERN = r"^https://kashinavi\.com/song_view\.html\?(?P<pageid>\d+)"
+_MUSICBOOK_PATTERN = r"^https://music-book\.jp/music/Artist/(?P<artistid>\d+)/Music/(?P<pageid>[a-z0-9]+)$"
 
 
-class KashinaviLyricPageParserError(BaseLyricPageParserError):
+class MusicbookLyricPageParserError(BaseLyricPageParserError):
     """WIP."""
 
 
-class KashinaviLyricPageParser(BaseLyricPageParser):
-    """https://kashinavi.com/song_view.html?<pageid>"""
+class MusicbookLyricPageParser(BaseLyricPageParser):
+    """https://music-book.jp/music/Artist/<artistid>/Music/<pageid>"""
 
-    _test = "https://kashinavi.com/song_view.html?155779"
+    _test = "https://music-book.jp/music/Artist/1538923/Music/aaahiqc4"
 
     @staticmethod
     def is_valid_url(url: str) -> bool:
         """Check if the url is valid."""
-        pattern = re.compile(_KASHINAVI_PATTERN)
+        pattern = re.compile(_MUSICBOOK_PATTERN)
         m = re.match(pattern, url)
-        return get_captured_value(m, "pageid") is not None
+        artistid = get_captured_value(m, "artistid")
+        pageid = get_captured_value(m, "pageid")
+
+        return artistid is not None and pageid is not None
 
     @staticmethod
-    def parse(url: str) -> KashinaviLyricPage:
+    def parse(url: str) -> MusicbookLyricPage:
         """Parse the url page and return the result as LyricPage instance."""
-        pattern = re.compile(_KASHINAVI_PATTERN)
+        pattern = re.compile(_MUSICBOOK_PATTERN)
         m = re.match(pattern, url)
+        artistid = get_captured_value(m, "artistid")
+        if artistid is None:
+            raise MusicbookLyricPageParserError from ValueError
+
         pageid = get_captured_value(m, "pageid")
         if pageid is None:
-            raise KashinaviLyricPageParserError from ValueError
+            raise MusicbookLyricPageParserError from ValueError
 
         bs = get_source(url)
         if bs is None:
-            raise KashinaviLyricPageParserError from ConnectionError
+            raise MusicbookLyricPageParserError from ConnectionError
+
+        title = select_one_tag(bs, "h1").text
+
+        artist = select_one_tag(bs, "a.text-with-icon.artist")
+        artist_name = artist.text.strip()
 
-        jsonld_tag: Tag = bs.find_all("script", type="application/ld+json")[1]
+        m = re.search(r"href=\"(?P<link>/music/Artist/\d+)\"", str(artist))
+        artist_link = get_captured_value(m, "link")
+        if artist_link is None:
+            raise MusicbookLyricPageParserError from ValueError
 
-        jsonld_source = jsonld_tag.text
-        jsonld = JSONLD.parse_raw(jsonld_source)
+        lyricist = select_one_tag(bs, "li:nth-child(1) > div > span").text.strip()
+        composer = select_one_tag(bs, "li:nth-child(2) > div > span").text.strip()
 
-        artist = jsonld.recorded_as.by_artist
+        bs_lyric = get_source(f"https://music-book.jp/music/Lyrics/Track?artistName={artist_name}&trackTitle={title}")
+        if bs_lyric is None:
+            raise MusicbookLyricPageParserError from ConnectionError
+        lyric_data = MusicbookLyricData.model_validate_json(bs_lyric.text)
 
-        return KashinaviLyricPage(
-            title=jsonld.name,
+        return MusicbookLyricPage(
+            title=title,
             page_url=parse_obj_as_url(url),
             pageid=pageid,
-            artist=WithUrlText(link=artist.url, text=artist.name),
-            composer=jsonld.composer.name,
-            lyricist=jsonld.lyricist.name,
+            artist=WithUrlText(text=artist_name, link=parse_obj_as_url(artist_link, base=url)),
+            composer=composer if composer != "-" and not composer else lyric_data.composer,
+            lyricist=lyricist if lyricist != "-" and not lyricist else lyric_data.writer,
             arranger=None,
-            lyric_sections=[
-                [i.text for i in section.children if isinstance(i, NavigableString)]
-                for section in BeautifulSoup(jsonld.lyrics.text, "lxml").find_all("p")
-            ],
+            lyric_sections=convert_lines_into_sections(lyric_data.lyrics),
         )
```

### Comparing `pyjlyric-0.0.2/pyjlyric/main.py` & `pyjlyric-1.0.0/pyjlyric/main.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/parse.py` & `pyjlyric-1.0.0/pyjlyric/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,10 +79,10 @@
             ===
             Title:\t\t{title}
             Artist:\t\t{artist or "(No data)"}
             Lyric:\t\t{lyricist or "(No data)"}
             Composer:\t{composer or "(No data)"}
             ===
             """,
-        ).strip()
-        + (linesep + linesep).join(lyric_sections).strip()
+        )
+        + (linesep * 2).join(lyric_sections).strip()
     )
```

### Comparing `pyjlyric-0.0.2/pyjlyric/petitlyrics/parser.py` & `pyjlyric-1.0.0/pyjlyric/petitlyrics/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,16 +72,16 @@
             headers={
                 "X-CSRF-Token": get_captured_value(m, "csrf_token"),
                 "X-Requested-With": "XMLHttpRequest",
             },
         )
         if not res_ajax.ok:
             raise PetitlyricsLyricPageParserError from ConnectionError
-        bs_ajax = BeautifulSoup(res_ajax.text)
-        lyric_lines = list(PetitlyricsLyricData.parse_raw(bs_ajax.text))
+        bs_ajax = BeautifulSoup(res_ajax.text, "lxml")
+        lyric_lines = list(PetitlyricsLyricData.model_validate_json(bs_ajax.text))
 
         return PetitlyricsLyricPage(
             title=select_one_tag(bs, "div.title-bar").text.strip(),
             page_url=parse_obj_as_url(url),
             pageid=pageid,
             artist=WithUrlText(text=artist.text.strip(), link=parse_obj_as_url(str(artist_link), base=url)),
             composer=None if composer is None else composer.strip(),
```

### Comparing `pyjlyric-0.0.2/pyjlyric/utamap/parser.py` & `pyjlyric-1.0.0/pyjlyric/utamap/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/utanet/parser.py` & `pyjlyric-1.0.0/pyjlyric/utanet/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/utaten/parser.py` & `pyjlyric-1.0.0/pyjlyric/utaten/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-0.0.2/pyjlyric/util.py` & `pyjlyric-1.0.0/pyjlyric/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal
 from urllib.parse import urljoin
 
 import requests
 from bs4 import BeautifulSoup, Tag
-from pydantic import HttpUrl, parse_obj_as
+from pydantic import HttpUrl, TypeAdapter
 
 from pyjlyric.model import WithUrlText
 
 if TYPE_CHECKING:
     from re import Match
 
 _UA = """
@@ -95,27 +95,27 @@
     return res
 
 
 def parse_obj_as_url(url: str, *, base: str | None = None) -> HttpUrl:
     """WIP."""
     if base is not None:
         url = urljoin(base, url)
-    return parse_obj_as(HttpUrl, url)  # type: ignore[no-any-return]
+    return TypeAdapter(HttpUrl).validate_python(url)
 
 
 def parse_text_with_optional_link(text: str, link: HttpUrl | None) -> WithUrlText | str:
     if link is None:
         return text
     return WithUrlText(text=text, link=link)
 
 
 def convert_lines_into_sections(lines: list[str]) -> list[list[str]]:
     lyric_sections = []
     now: list[str] = []
     for line in [*lines, ""]:
-        if line == "":
+        if not line:
             if len(now) > 0:
                 lyric_sections.append(now)
             now = []
         else:
             now.append(line)
     return lyric_sections
```

### Comparing `pyjlyric-0.0.2/pyproject.toml` & `pyjlyric-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 profile = "black"
 
 [tool.mypy]
 pretty = true
 python_version = "3.9"
 show_error_codes = true
 strict = true
+plugins = [
+  "pydantic.mypy"
+]
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
 
 [tool.ruff]
 select = ["ALL"]
 ignore = [
   "D",
 ]
 line-length = 120
@@ -59,27 +67,27 @@
   "japanese-songs",
 ]
 name = "pyjlyric"
 packages = [{include = "pyjlyric"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/pyjlyric"
-version = "0.0.2"
+version = "1.0.0"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pydantic = "^1.10.5"
+pydantic = ">=1.10.5,<3.0.0"
 typing-extensions = "^4.5.0"
 requests = "^2.28.2"
 beautifulsoup4 = "^4.11.2"
 lxml = "^4.9.2"
 chardet = "^5.1.0"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.2"
+mypy = ">=0.991,<1.5"
 pre-commit = ">=2.20,<4.0"
 taskipy = "^1.10.3"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.scripts]
 jrc = "pyjlyric.main:main"
```

### Comparing `pyjlyric-0.0.2/PKG-INFO` & `pyjlyric-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: pyjlyric
-Version: 0.0.2
+Version: 1.0.0
 Summary: Japanese Lyric Aggregator
 Home-page: https://github.com/eggplants/pyjlyric
 License: MIT
 Keywords: japanese,lyrics,download-lyrics,lyrics-scraping,japanese-songs
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=1.10.5,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/eggplants/pyjlyric
 Description-Content-Type: text/markdown
 
 # pyjlyric: Japanese Lyric Aggregator
```

