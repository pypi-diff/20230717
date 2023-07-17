# Comparing `tmp/namedivider-python-0.2.1.tar.gz` & `tmp/namedivider_python-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namedivider-python-0.2.1.tar", last modified: Thu Jun 15 06:37:19 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `namedivider-python-0.2.1.tar` & `namedivider_python-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,26 @@
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/
--rw-rw-r--   0 ml        (1001) ml        (1001)     1063 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/LICENSE
--rw-rw-r--   0 ml        (1001) ml        (1001)       66 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/MANIFEST.in
--rw-rw-r--   0 ml        (1001) ml        (1001)      567 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/PKG-INFO
--rw-rw-r--   0 ml        (1001) ml        (1001)     4480 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/README.md
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/
--rw-rw-r--   0 ml        (1001) ml        (1001)      585 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/__init__.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/assets/
--rwxrwxr-x   0 ml        (1001) ml        (1001)    30784 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/assets/kanji.csv
--rwxrwxr-x   0 ml        (1001) ml        (1001)     5323 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/cli.py
--rwxrwxr-x   0 ml        (1001) ml        (1001)     1092 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divided_name.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/divider/
--rw-rw-r--   0 ml        (1001) ml        (1001)        0 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/__init__.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     1572 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/basic_name_divider.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     3488 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/config.py
--rw-rw-r--   0 ml        (1001) ml        (1001)      819 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/divided_name.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     2131 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/gbdt_name_divider.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     8291 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/name_divider_base.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/feature/
--rw-rw-r--   0 ml        (1001) ml        (1001)        0 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/__init__.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     4474 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/extractor.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     1263 2023-06-15 06:09:48.000000 namedivider-python-0.2.1/namedivider/feature/family_name.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     7623 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/functional.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     5406 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/kanji.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     4604 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/kanji_statistics.py
--rwxrwxr-x   0 ml        (1001) ml        (1001)    15296 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/name_divider.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/training/
--rw-rw-r--   0 ml        (1001) ml        (1001)        0 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/training/__init__.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     4549 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/training/kanji_statistics_taker.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     2001 2023-06-15 06:09:48.000000 namedivider-python-0.2.1/namedivider/util.py
--rw-rw-r--   0 ml        (1001) ml        (1001)       22 2023-06-15 06:36:27.000000 namedivider-python-0.2.1/namedivider/version.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider_python.egg-info/
--rw-rw-r--   0 ml        (1001) ml        (1001)      567 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/PKG-INFO
--rw-rw-r--   0 ml        (1001) ml        (1001)      960 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/SOURCES.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)        1 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/dependency_links.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       47 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/entry_points.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       60 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/requires.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       12 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/top_level.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       38 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/setup.cfg
--rw-rw-r--   0 ml        (1001) ml        (1001)      990 2023-06-15 06:09:48.000000 namedivider-python-0.2.1/setup.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/__init__.py
+-rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/cli.py
+-rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/divided_name.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/kanji_statistics.py
+-rwxr-xr-x   0        0        0    15134 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/name_divider.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/util.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/version.py
+-rwxr-xr-x   0        0        0    30784 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/assets/kanji.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/divider/__init__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/divider/basic_name_divider.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/divider/config.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/divider/divided_name.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/divider/gbdt_name_divider.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/divider/name_divider_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/feature/__init__.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/feature/extractor.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/feature/family_name.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/feature/functional.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/feature/kanji.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/training/__init__.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/namedivider/training/kanji_statistics_taker.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/README.md
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 namedivider_python-0.2.2/PKG-INFO
```

### Comparing `namedivider-python-0.2.1/LICENSE` & `namedivider_python-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.1/README.md` & `namedivider_python-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         ]
 }
 ```
 
 ### Notice
 
 - `names` is a list of undivided name. The maximum length of the list is 1000.
+- If you require speed or want to use GBDTNameDivider, please try [v0.2.0-beta](https://github.com/rskmoi/namedivider-rs/tree/main/api).
 
 ## CLI
 Read namedivider/cli.py for more information.
 ```
 $ nmdiv name 菅義偉
 菅 義偉
 $ nmdiv file undivided_names.txt
```

### Comparing `namedivider-python-0.2.1/namedivider/__init__.py` & `namedivider_python-0.2.2/namedivider/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from .name_divider import NameDivider
-from .divider.divided_name import DividedName
 from .divider.basic_name_divider import BasicNameDivider
+from .divider.config import BasicNameDividerConfig, NameDividerVersions
+from .divider.divided_name import DividedName
 from .divider.gbdt_name_divider import GBDTNameDivider
 from .feature.kanji import KanjiStatistics
-from .divider.config import NameDividerVersions, BasicNameDividerConfig
+from .name_divider import NameDivider
 from .version import __version__
 
-__all__ = ["NameDivider",
-           "BasicNameDivider",
-           "GBDTNameDivider",
-           "DividedName",
-           "KanjiStatistics",
-           "NameDividerVersions",
-           "BasicNameDividerConfig",
-           "__version__"]
+__all__ = [
+    "NameDivider",
+    "BasicNameDivider",
+    "GBDTNameDivider",
+    "DividedName",
+    "KanjiStatistics",
+    "NameDividerVersions",
+    "BasicNameDividerConfig",
+    "__version__",
+]
```

### Comparing `namedivider-python-0.2.1/namedivider/assets/kanji.csv` & `namedivider_python-0.2.2/namedivider/assets/kanji.csv`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.1/namedivider/cli.py` & `namedivider_python-0.2.2/namedivider/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,57 @@
+from pathlib import Path
+
 import typer
 from tqdm import tqdm
-from pathlib import Path
+
+from namedivider.divider.basic_name_divider import BasicNameDivider
+from namedivider.divider.config import BasicNameDividerConfig, GBDTNameDividerConfig
+from namedivider.divider.gbdt_name_divider import GBDTNameDivider
 from namedivider.divider.name_divider_base import _NameDivider
-from namedivider.divider.basic_name_divider import BasicNameDivider, BasicNameDividerConfig
-from namedivider.divider.gbdt_name_divider import GBDTNameDivider, GBDTNameDividerConfig
 
 CURRENT_DIR = Path(__file__).resolve().parent
 
 app = typer.Typer()
 
 
 def get_divider(mode: str, separator: str) -> _NameDivider:
     if mode == "basic":
-        config = BasicNameDividerConfig(separator=separator)
-        return BasicNameDivider(config=config)
+        basic_config = BasicNameDividerConfig(separator=separator)
+        return BasicNameDivider(config=basic_config)
     elif mode == "gbdt":
-        config = GBDTNameDividerConfig(separator=separator)
-        return GBDTNameDivider(config=config)
+        gbdt_config = GBDTNameDividerConfig(separator=separator)
+        return GBDTNameDivider(config=gbdt_config)
     else:
         raise ValueError(f"Mode must be in [basic, gbdt], but got {mode}")
 
 
 @app.command()
-def name(undivided_name: str = typer.Argument(..., help="Undivided name"),
-         separator: str = typer.Option(" ", "--separator", "-s", help="Separator between family name and given name"),
-         mode: str = typer.Option("basic", "--mode", "-m", help="Divider Mode. You can choice basic or gbdt.")):
+def name(
+    undivided_name: str = typer.Argument(..., help="Undivided name"),
+    separator: str = typer.Option(" ", "--separator", "-s", help="Separator between family name and given name"),
+    mode: str = typer.Option("basic", "--mode", "-m", help="Divider Mode. You can choice basic or gbdt."),
+) -> None:
     """
     Divides an undivided name.
     :param undivided_name: Undivided name
     :param separator: Separator between family name and given name
     """
     divider = get_divider(mode=mode, separator=separator)
     print(divider.divide_name(undivided_name))
 
 
 @app.command()
-def file(undivided_name_text: Path = typer.Argument(...,
-                                                    help="File path of text file",
-                                                    exists=True,
-                                                    dir_okay=False,
-                                                    readable=True),
-         separator: str = typer.Option(" ", "--separator", "-s", help="Separator between family name and given name"),
-         mode: str = typer.Option("basic", "--mode", "-m", help="Divider Mode. You can choice basic or gbdt."),
-         encoding: str = typer.Option("utf-8", "--encoding", "-e", help="Encoding of text file")):
+def file(
+    undivided_name_text: Path = typer.Argument(
+        ..., help="File path of text file", exists=True, dir_okay=False, readable=True
+    ),
+    separator: str = typer.Option(" ", "--separator", "-s", help="Separator between family name and given name"),
+    mode: str = typer.Option("basic", "--mode", "-m", help="Divider Mode. You can choice basic or gbdt."),
+    encoding: str = typer.Option("utf-8", "--encoding", "-e", help="Encoding of text file"),
+) -> None:
     """
     Divides names in text file.
     The text file must have one name per line.
     Text file example:
     ```
     原敬
     菅義偉
@@ -72,23 +77,22 @@
     divided_names = []
     for _undivided_name in tqdm(undivided_names):
         divided_names.append(str(divider.divide_name(_undivided_name)))
     print("\n".join(divided_names))
 
 
 @app.command()
-def accuracy(divided_name_text: Path = typer.Argument(...,
-                                                      help="File path of text file",
-                                                      exists=True,
-                                                      dir_okay=False,
-                                                      readable=True),
-             separator: str = typer.Option(" ", "--separator", "-s",
-                                           help="Separator between family name and given name"),
-             mode: str = typer.Option("basic", "--mode", "-m", help="Divider Mode. You can choice basic or gbdt."),
-             encoding: str = typer.Option("utf-8", "--encoding", "-e", help="Encoding of text file")):
+def accuracy(
+    divided_name_text: Path = typer.Argument(
+        ..., help="File path of text file", exists=True, dir_okay=False, readable=True
+    ),
+    separator: str = typer.Option(" ", "--separator", "-s", help="Separator between family name and given name"),
+    mode: str = typer.Option("basic", "--mode", "-m", help="Divider Mode. You can choice basic or gbdt."),
+    encoding: str = typer.Option("utf-8", "--encoding", "-e", help="Encoding of text file"),
+) -> None:
     """
     Check the accuracy of this tool.
     The text file must have one name per line, and name must be divided py separator.
     Text file example:
     ```
     原 敬
     菅 義偉
@@ -105,24 +109,24 @@
     100%|███████████████████████████████████████████| 5/5 [00:00<00:00, 3673.41it/s]
     0.8
     True: 滝 登喜男, Pred: 滝登 喜男
     ```
     """
     divider = get_divider(mode=mode, separator=separator)
     with open(divided_name_text, "rb") as f:
-        divided_name_text = f.read().decode(encoding).strip().split("\n")
+        divided_names = f.read().decode(encoding).strip().split("\n")
     is_correct_list = []
     wrong_list = []
-    for _divided_name in tqdm(divided_name_text):
+    for _divided_name in tqdm(divided_names):
         _undivided_name = _divided_name.replace(separator, "")
         _divided_name_pred = str(divider.divide_name(_undivided_name))
-        is_correct = (_divided_name == _divided_name_pred)
+        is_correct = _divided_name == _divided_name_pred
         is_correct_list.append(is_correct)
         if not is_correct:
             wrong_list.append(f"True: {_divided_name}, Pred: {_divided_name_pred}")
     print(f"{sum(is_correct_list) / len(is_correct_list):.04}")
     if len(wrong_list) != 0:
         print("\n".join(wrong_list))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     app()
```

### Comparing `namedivider-python-0.2.1/namedivider/divided_name.py` & `namedivider_python-0.2.2/namedivider/divided_name.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import warnings
-from typing import Dict
-from dataclasses import dataclass, asdict
+from dataclasses import asdict, dataclass
+from typing import Any, Dict
 
 
 @dataclass(frozen=True)
 class DividedName:
     """
     Divided name.
     :param family: Family name
     :param given: Given name
     :param separator: Character for separate family name and given name.
     :param score: Confidence level, from 0 to 1
     :param algorithm: The name of dividing algorithm
     """
-    warnings.warn("namedivider.divided_name.DividedName is deprecated in 0.2 and will be removed in 0.4. "
-                  "Use namedivider.divider.divided_name.DividedName if you want to use DividedName class.",
-                  category=FutureWarning)
+
+    warnings.warn(
+        "namedivider.divided_name.DividedName is deprecated in 0.2 and will be removed in 0.4. "
+        "Use namedivider.divider.divided_name.DividedName if you want to use DividedName class.",
+        category=FutureWarning,
+        stacklevel=1,
+    )
     family: str
     given: str
     separator: str = " "
-    score: float = 1.
+    score: float = 1.0
     algorithm: str = ""
 
     def __str__(self) -> str:
         """
         :return: Divided name separated by separator.
         :rtype: str
         """
         return f"{self.family}{self.separator}{self.given}"
 
-    def to_dict(self) -> Dict:
+    def to_dict(self) -> Dict[str, Any]:
         """
         :return: Dictionary of divided name
         :rtype: Dict
         """
         return asdict(self)
```

### Comparing `namedivider-python-0.2.1/namedivider/divider/basic_name_divider.py` & `namedivider_python-0.2.2/namedivider/divider/basic_name_divider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from typing import Optional
+
 from namedivider.divider.config import BasicNameDividerConfig
 from namedivider.divider.name_divider_base import _NameDivider
-from namedivider.feature.kanji import KanjiStatisticsRepository
 from namedivider.feature.extractor import SimpleFeatureExtractor
+from namedivider.feature.kanji import KanjiStatisticsRepository
 
 
 class BasicNameDivider(_NameDivider):
     """
     NameDivider with basic algorithm.
     Prior to v0.1.0, this was provided as a 'NameDivider' class.
     """
 
-    def __init__(self, config: BasicNameDividerConfig = None):
+    def __init__(self, config: Optional[BasicNameDividerConfig] = None):
         if config is None:
             config = BasicNameDividerConfig()
         super().__init__(config=config)
         repository = KanjiStatisticsRepository(path_csv=config.path_csv)
         self.only_order_score_when_4 = config.only_order_score_when_4
         self.feature_extractor = SimpleFeatureExtractor(kanji_statistics_repository=repository)
 
@@ -28,8 +30,8 @@
         name = family + given
         features = self.feature_extractor.get_features(family=family, given=given)
         order_score = (features.family_order_score + features.given_order_score) / (len(name) - 2)
         if self.only_order_score_when_4 and len(family + given) == 4:
             return order_score
         length_score = (features.family_length_score + features.given_length_score) / len(name)
 
-        return (order_score + length_score) / 2.
+        return (order_score + length_score) / 2.0
```

### Comparing `namedivider-python-0.2.1/namedivider/divider/config.py` & `namedivider_python-0.2.2/namedivider/divider/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Union
+from dataclasses import dataclass
 from enum import Enum, auto
 from pathlib import Path
-from dataclasses import dataclass
-from namedivider.util import \
-    get_kanji_csv_default_path, \
-    get_family_name_pkl_default_path, \
-    get_gbdt_model_v1_default_path
+from typing import Union
+
+from namedivider.util import (
+    get_family_name_pkl_default_path,
+    get_gbdt_model_v1_default_path,
+    get_kanji_csv_default_path,
+)
 
 KANJI_CSV_DEFAULT_PATH = get_kanji_csv_default_path()
 FAMILY_NAME_PKL_DEFAULT_PATH = get_family_name_pkl_default_path()
 GBDT_MODEL_V1_DEFAULT_PATH = get_gbdt_model_v1_default_path()
 
 
 class NameDividerVersions(Enum):
@@ -25,25 +27,27 @@
     """
     separator: Characters to separate a family name and a given name.
     normalize_name: Flag whether or not to normalize Kanji characters.
     'normalize' here means to internally convert old character form(旧字体) or variant character form(異字体)
     into orthographic character form(正字体) before processing them.
     algorithm_name: Name of algorithm.
     """
+
     separator: str = " "
     normalize_name: bool = True
     algorithm_name: str = "unknown_algorithm"
 
 
 @dataclass(frozen=True)
 class BasicNameDividerConfig(NameDividerConfigBase):
     """
     path_csv: Path of the file containing the kanji information.
     only_order_score_when_4: If True, only order score is used for 4-character names. Not recommended to be True.
     """
+
     path_csv: Union[str, Path] = KANJI_CSV_DEFAULT_PATH
     only_order_score_when_4: bool = False
     algorithm_name: str = "kanji_feature"
 
 
 @dataclass(frozen=True)
 class GBDTNameDividerConfig(NameDividerConfigBase):
@@ -52,42 +56,37 @@
     path_family_names: Allows .pickle file or text file(like .txt, .log, etc...)
     - .pickle file
     Pickled object must be instance of FamilyNameRepository.
     - text file
     Path of a file with multiple family names enumerated.
     path_model: Path of a GBDT model.
     """
+
     path_csv: Union[str, Path] = KANJI_CSV_DEFAULT_PATH
     path_family_names: Union[str, Path] = FAMILY_NAME_PKL_DEFAULT_PATH
     path_model: Union[str, Path] = GBDT_MODEL_V1_DEFAULT_PATH
     algorithm_name: str = "gbdt"
 
 
 def get_config_from_version(version: NameDividerVersions) -> NameDividerConfigBase:
     if version == NameDividerVersions.BASIC_NAME_DIVIDER_V1:
         return BasicNameDividerConfig(
-            separator=" ",
-            normalize_name=False,
-            path_csv=KANJI_CSV_DEFAULT_PATH,
-            only_order_score_when_4=True
+            separator=" ", normalize_name=False, path_csv=KANJI_CSV_DEFAULT_PATH, only_order_score_when_4=True
         )
     elif version == NameDividerVersions.BASIC_NAME_DIVIDER_V2:
         return BasicNameDividerConfig(
-            separator=" ",
-            normalize_name=True,
-            path_csv=KANJI_CSV_DEFAULT_PATH,
-            only_order_score_when_4=False
+            separator=" ", normalize_name=True, path_csv=KANJI_CSV_DEFAULT_PATH, only_order_score_when_4=False
         )
     elif version == NameDividerVersions.BASIC_NAME_DIVIDER_LATEST:
         return BasicNameDividerConfig()
     elif version == NameDividerVersions.GBDT_NAME_DIVIDER_V1:
         return GBDTNameDividerConfig(
             separator=" ",
             normalize_name=True,
             path_csv=KANJI_CSV_DEFAULT_PATH,
             path_family_names=FAMILY_NAME_PKL_DEFAULT_PATH,
-            path_model=GBDT_MODEL_V1_DEFAULT_PATH
+            path_model=GBDT_MODEL_V1_DEFAULT_PATH,
         )
     elif version == NameDividerVersions.GBDT_NAME_DIVIDER_LATEST:
         return GBDTNameDividerConfig()
     else:
         raise ValueError(f"Version {version} is not in NameDividerVersions.")
```

### Comparing `namedivider-python-0.2.1/namedivider/divider/divided_name.py` & `namedivider_python-0.2.2/namedivider/divider/divided_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from typing import Dict
-from dataclasses import dataclass, asdict
+from dataclasses import asdict, dataclass
+from typing import Any, Dict
 
 
 @dataclass(frozen=True)
 class DividedName:
     """
     Divided name.
     :param family: Family name
     :param given: Given name
     :param separator: Character for separate family name and given name.
     :param score: Confidence level, from 0 to 1
     :param algorithm: The name of dividing algorithm
     """
+
     family: str
     given: str
     separator: str = " "
-    score: float = 1.
+    score: float = 1.0
     algorithm: str = ""
 
     def __str__(self) -> str:
         """
         :return: Divided name separated by separator.
         :rtype: str
         """
         return f"{self.family}{self.separator}{self.given}"
 
-    def to_dict(self) -> Dict:
+    def to_dict(self) -> Dict[str, Any]:
         """
         :return: Dictionary of divided name
         :rtype: Dict
         """
         return asdict(self)
```

### Comparing `namedivider-python-0.2.1/namedivider/divider/gbdt_name_divider.py` & `namedivider_python-0.2.2/namedivider/divider/gbdt_name_divider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,53 @@
-import pandas as pd
-import lightgbm as lgb
-import _pickle as pickle
 from dataclasses import asdict
 from pathlib import Path
-from namedivider.util import download_family_name_pickle_if_needed, download_gbdt_model_v1_if_needed
+from typing import Optional, cast
+
+import _pickle as pickle  # type: ignore
+import lightgbm as lgb
+import pandas as pd
+
 from namedivider.divider.config import GBDTNameDividerConfig
 from namedivider.divider.name_divider_base import _NameDivider
-from namedivider.feature.kanji import KanjiStatisticsRepository
-from namedivider.feature.family_name import FamilyNameRepository
 from namedivider.feature.extractor import FamilyRankingFeatureExtractor
+from namedivider.feature.family_name import FamilyNameRepository
+from namedivider.feature.kanji import KanjiStatisticsRepository
+from namedivider.util import (
+    download_family_name_pickle_if_needed,
+    download_gbdt_model_v1_if_needed,
+)
 
 
 class GBDTNameDivider(_NameDivider):
     """
     NameDivider with gradient boosting decision tree.
     """
 
-    def __init__(self, config: GBDTNameDividerConfig = None):
+    def __init__(self, config: Optional[GBDTNameDividerConfig] = None):
         if config is None:
             config = GBDTNameDividerConfig()
         super().__init__(config=config)
         download_family_name_pickle_if_needed(config.path_family_names)
         download_gbdt_model_v1_if_needed(config.path_model)
         kanji_statistics_repository = KanjiStatisticsRepository(path_csv=config.path_csv)
         if Path(config.path_family_names).suffix == ".pickle":
             with open(config.path_family_names, "rb") as f:
                 family_name_repository: FamilyNameRepository = pickle.load(f)
         else:
             family_name_repository = FamilyNameRepository(path_txt=config.path_family_names)
-        self.feature_extractor = FamilyRankingFeatureExtractor(kanji_statistics_repository=kanji_statistics_repository,
-                                                               family_name_repository=family_name_repository)
+        self.feature_extractor = FamilyRankingFeatureExtractor(
+            kanji_statistics_repository=kanji_statistics_repository, family_name_repository=family_name_repository
+        )
         self.model = lgb.Booster(model_file=config.path_model)
 
     def calc_score(self, family: str, given: str) -> float:
         """
         Calculates the score. The higher the score, the more likely the division is correct.
         :param family: Family name.
         :param given: Given name.
         :return: Score of dividing.
         """
         feature = self.feature_extractor.get_features(family=family, given=given)
         df = pd.DataFrame([asdict(feature)])
-        score = self.model.predict(df)
-        return score[0]
+        score_list = self.model.predict(df)
+        score = cast(float, score_list[0])
+        return score
```

### Comparing `namedivider-python-0.2.1/namedivider/divider/name_divider_base.py` & `namedivider_python-0.2.2/namedivider/divider/name_divider_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import abc
-import regex
+from typing import List, Optional
+
 import numpy as np
+import regex
+
+from namedivider.divider.config import (
+    NameDividerConfigBase,
+    NameDividerVersions,
+    get_config_from_version,
+)
 from namedivider.divider.divided_name import DividedName
-from namedivider.divider.config import NameDividerVersions, get_config_from_version, NameDividerConfigBase
-from typing import Optional
 
 
 class _UndividedNameHolder:
     def __init__(self, original_name: str):
         """
         Class to hold original and normalized name for dividing.
         :param original_name: Original name
@@ -35,36 +41,38 @@
         Get divided original name using divided normalize name.
         :param divided_normalized_name: Divided name by normalized name.
         :return: Divided name by original name.
         """
         _family_length = len(divided_normalized_name.family)
         _family = self.original_name[:_family_length]
         _given = self.original_name[_family_length:]
-        return DividedName(_family,
-                           _given,
-                           separator=divided_normalized_name.separator,
-                           score=divided_normalized_name.score,
-                           algorithm=divided_normalized_name.algorithm)
+        return DividedName(
+            _family,
+            _given,
+            separator=divided_normalized_name.separator,
+            score=divided_normalized_name.score,
+            algorithm=divided_normalized_name.algorithm,
+        )
 
 
 class _NameDivider(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def __init__(self, config: NameDividerConfigBase = None):
+    def __init__(self, config: Optional[NameDividerConfigBase] = None):
         """
         Base Class for dividing an undivided name.
         ("undivided name" means names with no space between the family name and given name.)
         All NameDividers inherit this class.
         :param config: Configuration of NameDivider.
         """
         if config is None:
             config = NameDividerConfigBase()
         self.separator = config.separator
         self.normalize_name = config.normalize_name
         self.algorithm_name = config.algorithm_name
-        self.compiled_regex_kanji = regex.compile(r'\p{Script=Han}+')
+        self.compiled_regex_kanji = regex.compile(r"\p{Script=Han}+")
 
     @abc.abstractmethod
     def calc_score(self, family: str, given: str) -> float:
         """
         Calculates the score. The higher the score, the more likely the division is correct.
         :param family: Family name.
         :param given: Given name.
@@ -79,45 +87,46 @@
         :param version: Version of divider.
         :return: NameDivider instance constructed by model version.
         :rtype: _NameDivider
         """
         config = get_config_from_version(version)
         return cls(config=config)
 
-    def _create_divided_name(self, family: str, given: str, score: float = 1., algorithm: str = "") -> DividedName:
+    def _create_divided_name(self, family: str, given: str, score: float = 1.0, algorithm: str = "") -> DividedName:
         """
         Generates DividedName.
         :param family: Family name
         :param given: Given name
         :param score: Confidence level, from 0 to 1
         :param algorithm: The name of dividing algorithm
         :return: Divided name
         :rtype: DividedName
         """
         return DividedName(family, given, separator=self.separator, score=score, algorithm=algorithm)
 
     @staticmethod
-    def _validate(undivided_name: str):
+    def _validate(undivided_name: str) -> None:
         """
         Determines if it is an assumed input.
         :param undivided_name: Names with no space between the first and last name
         """
         if len(undivided_name) < 2:
             raise ValueError("Name length needs at least 2 chars")
 
     @staticmethod
-    def _softmax(x) -> np.ndarray:
+    def _softmax(x: List[float]) -> List[float]:
         """
         Calculates softmax score
         :param x: array_like
         :return: Softmax scores
         :rtype: np.ndarray
         """
         u = np.sum(np.exp(x))
-        return np.exp(x) / u
+        softmax_val: List[float] = np.exp(x) / u
+        return softmax_val
 
     def _divide_by_rule_base(self, undivided_name: str) -> Optional[DividedName]:
         """
         Divides undivided name without using kanji statistics.
         :param undivided_name: Names with no space between the family name and given name
         :return:
             if fits the rules: Divided name
@@ -125,33 +134,33 @@
         :rtype:
             if fits the rules: DividedName
             else: None
         """
         # If the undivided name consists of 2 characters,
         # the first characters is family name, and the last characters is given name.
         if len(undivided_name) == 2:
-            return self._create_divided_name(family=undivided_name[0],
-                                             given=undivided_name[-1],
-                                             algorithm="rule")
+            return self._create_divided_name(family=undivided_name[0], given=undivided_name[-1], algorithm="rule")
 
         # If the undivided name consists of kanji and other types of characters (hiragana, katakana, etc...),
         # the undivided name will be divided where the kanji and other character types are switched.
         # The criterion for determining switched is whether "two" consecutive characters are having
         # different type of characters from first character type.
         # The reason of "two" is some family names consist of some kanji and one katakana.
         # (ex: "井ノ原", "三ツ又",　"関ヶ原" contains "ノ", "ツ", "ヶ". They are all katakana.)
         is_kanji_list = []
         for i, _char in enumerate(undivided_name):
             is_kanji = True if self.compiled_regex_kanji.fullmatch(_char) else False
             is_kanji_list.append(is_kanji)
             if i >= 2:
                 if is_kanji_list[0] != is_kanji and is_kanji_list[-2] == is_kanji:
-                    return self._create_divided_name(family=undivided_name[:i - 1],
-                                                     given=undivided_name[i - 1:],
-                                                     algorithm="rule")
+                    return self._create_divided_name(
+                        family=undivided_name[: i - 1], given=undivided_name[i - 1 :], algorithm="rule"
+                    )
+
+        return None
 
     def _divide_by_algorithm(self, undivided_name: str) -> DividedName:
         """
         Divides undivided name using kanji statistics.
         :param undivided_name: Names with no space between the family name and given name
         :return: Divided name
         :rtype: DividedName
@@ -161,18 +170,20 @@
             family = undivided_name[:i]
             given = undivided_name[i:]
             score = self.calc_score(family, given)
             total_scores.append(score)
 
         total_scores = self._softmax(total_scores)
         max_idx = np.argmax(np.array(total_scores)) + 1
-        return self._create_divided_name(family=undivided_name[:max_idx],
-                                         given=undivided_name[max_idx:],
-                                         score=total_scores[max_idx - 1],
-                                         algorithm=self.algorithm_name)
+        return self._create_divided_name(
+            family=undivided_name[:max_idx],
+            given=undivided_name[max_idx:],
+            score=total_scores[max_idx - 1],
+            algorithm=self.algorithm_name,
+        )
 
     def _divide_name(self, undivided_name: str) -> DividedName:
         """
         Divides undivided name.
         :param undivided_name: Names with no space between the family name and given name
         :return: Divided name
         :rtype: DividedName
```

### Comparing `namedivider-python-0.2.1/namedivider/feature/extractor.py` & `namedivider_python-0.2.2/namedivider/feature/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pathlib import Path
-from typing import Union
 from dataclasses import dataclass
+
 import namedivider.feature.functional as F
-from namedivider.feature.kanji import KanjiStatisticsRepository
 from namedivider.feature.family_name import FamilyNameRepository
+from namedivider.feature.kanji import KanjiStatisticsRepository
 
 
 @dataclass(frozen=True)
 class SimpleFeatures:
     """
     Features for SimpleFeatureExtractor.
     """
+
     family_order_score: float
     family_length_score: float
     given_order_score: float
     given_length_score: float
 
 
 @dataclass(frozen=True)
@@ -48,28 +48,30 @@
         :rtype: SimpleFeature
         """
         fullname_length = len(family + given)
         family_order_score = F.calc_order_score(self.kanji_statistics_repository, family, fullname_length, 0)
         family_length_score = F.calc_length_score(self.kanji_statistics_repository, family, fullname_length, 0)
         given_order_score = F.calc_order_score(self.kanji_statistics_repository, given, fullname_length, len(family))
         given_length_score = F.calc_length_score(self.kanji_statistics_repository, given, fullname_length, len(family))
-        return SimpleFeatures(family_order_score=family_order_score,
-                              family_length_score=family_length_score,
-                              given_order_score=given_order_score,
-                              given_length_score=given_length_score)
+        return SimpleFeatures(
+            family_order_score=family_order_score,
+            family_length_score=family_length_score,
+            given_order_score=given_order_score,
+            given_length_score=given_length_score,
+        )
 
 
 class FamilyRankingFeatureExtractor:
     """
     Feature extractor.Calculate the order score and the length score for each of family and given name.
     """
 
-    def __init__(self,
-                 kanji_statistics_repository: KanjiStatisticsRepository,
-                 family_name_repository: FamilyNameRepository):
+    def __init__(
+        self, kanji_statistics_repository: KanjiStatisticsRepository, family_name_repository: FamilyNameRepository
+    ):
         self.kanji_statistics_repository = kanji_statistics_repository
         self.family_name_repository = family_name_repository
 
     def get_features(self, family: str, given: str) -> FamilyRankingFeatures:
         """
         Calculates features.
         :param family: family name.
@@ -83,16 +85,18 @@
         given_length = len(given)
         family_order_score = F.calc_order_score(self.kanji_statistics_repository, family, fullname_length, 0)
         family_length_score = F.calc_length_score(self.kanji_statistics_repository, family, fullname_length, 0)
         given_order_score = F.calc_order_score(self.kanji_statistics_repository, given, fullname_length, len(family))
         given_length_score = F.calc_length_score(self.kanji_statistics_repository, given, fullname_length, len(family))
         # Selected 10 Kanji chars, especially those that rarely come at the beginning of a given name.
         given_startswith_specific_kanji = given.startswith(("田", "谷", "川", "島", "原", "村", "塚", "森", "井", "子"))
-        return FamilyRankingFeatures(rank=rank,
-                                     fullname_length=fullname_length,
-                                     family_length=family_length,
-                                     given_length=given_length,
-                                     family_order_score=family_order_score,
-                                     given_order_score=given_order_score,
-                                     family_length_score=family_length_score,
-                                     given_length_score=given_length_score,
-                                     given_startswith_specific_kanji=given_startswith_specific_kanji)
+        return FamilyRankingFeatures(
+            rank=rank,
+            fullname_length=fullname_length,
+            family_length=family_length,
+            given_length=given_length,
+            family_order_score=family_order_score,
+            given_order_score=given_order_score,
+            family_length_score=family_length_score,
+            given_length_score=given_length_score,
+            given_startswith_specific_kanji=given_startswith_specific_kanji,
+        )
```

### Comparing `namedivider-python-0.2.1/namedivider/feature/family_name.py` & `namedivider_python-0.2.2/namedivider/feature/family_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import numpy as np
 import os
-from typing import Union
 from pathlib import Path
+from typing import Union
+
+import numpy as np
 
 
 class FamilyNameRepository:
     def __init__(self, path_txt: Union[str, Path]):
         """
         :param path_txt: Path of a file with multiple family names enumerated.
         This is in order of the most common family names in Japan.
```

### Comparing `namedivider-python-0.2.1/namedivider/feature/functional.py` & `namedivider_python-0.2.2/namedivider/feature/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
+import numpy.typing as npt
+
 from namedivider.feature.kanji import KanjiStatisticsRepository
 
 
-def _create_order_mask(full_name_length: int, char_idx: int) -> np.ndarray:
+def _create_order_mask(full_name_length: int, char_idx: int) -> npt.NDArray[np.int32]:
     """
     Create order mask.
     Order mask is one-hot mask for calculate order score.
     :param full_name_length: Length of full name.
     :param char_idx: The order of the character in full name
     :return: Order mask
     :rtype: np.ndarray
@@ -22,41 +24,41 @@
 
     if char_idx == full_name_length - 2:
         return np.array([0, 0, 1, 1, 1, 0])
 
     return np.array([0, 1, 1, 1, 1, 0])
 
 
-def _create_length_mask(full_name_length: int, char_idx: int) -> np.ndarray:
+def _create_length_mask(full_name_length: int, char_idx: int) -> npt.NDArray[np.int32]:
     """
     Create length mask.
     Length mask is one-hot mask for calculate length score.
     :param full_name_length: Length of full name.
     :param char_idx: The order of the character in full name
     :return: Length mask
     :rtype: np.ndarray
     """
     min_family = char_idx + 1
+    min_family_idx = 4 if min_family > 4 else min_family
     max_family = full_name_length - 1
-    max_family = 4 if max_family > 4 else max_family
+    max_family_idx = 4 if max_family > 4 else max_family
     min_given = full_name_length - char_idx
+    min_given_idx = 4 if min_given > 4 else min_given
     max_given = full_name_length - 1
-    max_given = 4 if max_given > 4 else max_given
+    max_given_idx = 4 if max_given > 4 else max_given
     lc_family = np.array([0, 0, 0, 0])
     if min_family <= max_family:
-        lc_family[min_family - 1: max_family] = 1
+        lc_family[min_family_idx - 1 : max_family_idx] = 1
     lc_given = np.array([0, 0, 0, 0])
     if min_given <= max_given:
-        lc_given[min_given - 1: max_given] = 1
+        lc_given[min_given_idx - 1 : max_given_idx] = 1
     return np.concatenate([lc_family, lc_given])
 
 
-def _calc_current_order_status(piece_of_divided_name: str,
-                               idx_in_piece_of_divided_name: int,
-                               is_family: bool) -> int:
+def _calc_current_order_status(piece_of_divided_name: str, idx_in_piece_of_divided_name: int, is_family: bool) -> int:
     """
     Determine which index of order_counts the kanji corresponds to.
     :param piece_of_divided_name: Family name or given name
     :param idx_in_piece_of_divided_name: Index in family or given name
     :param is_family: True if piece_of_divided_name is family name
     :return: The index of order_counts
     :rtype: int
@@ -77,18 +79,20 @@
     :return: The index of length_counts
     :rtype: int
     """
     piece_of_divided_name_length = len(piece_of_divided_name) if len(piece_of_divided_name) <= 4 else 4
     return piece_of_divided_name_length - 1 if is_family else piece_of_divided_name_length - 1 + 4
 
 
-def calc_order_score(kanji_statistics_repository: KanjiStatisticsRepository,
-                     piece_of_divided_name: str,
-                     full_name_length: int,
-                     start_index: int = 0) -> float:
+def calc_order_score(
+    kanji_statistics_repository: KanjiStatisticsRepository,
+    piece_of_divided_name: str,
+    full_name_length: int,
+    start_index: int = 0,
+) -> float:
     """
     Calculates order score.
     Order score is a feature, which is a kind of frequency, calculated from where each kanji in full name is used.
     See this link if you need more explanation: https://rskmoi.hatenablog.com/entry/2017/01/15/190837
     :param kanji_statistics_repository: Class for managing Kanji statistics.
     :param piece_of_divided_name: Family name or given name
     :param full_name_length: Length of fullname
@@ -116,29 +120,31 @@
     for idx_in_piece_of_divided_name, _kanji in enumerate(piece_of_divided_name):
         current_idx = start_index + idx_in_piece_of_divided_name
         if current_idx == 0:
             continue
         if current_idx == full_name_length - 1:
             continue
         mask = _create_order_mask(full_name_length, current_idx)
-        current_order_status_idx = _calc_current_order_status(piece_of_divided_name,
-                                                              idx_in_piece_of_divided_name,
-                                                              is_family)
+        current_order_status_idx = _calc_current_order_status(
+            piece_of_divided_name, idx_in_piece_of_divided_name, is_family
+        )
         masked_order = kanji_statistics_repository.get(_kanji).order_counts * mask
         if np.sum(masked_order) == 0:
             continue
         cur_score = masked_order[current_order_status_idx] / np.sum(masked_order)
         scores += cur_score
     return scores
 
 
-def calc_length_score(kanji_statistics_repository: KanjiStatisticsRepository,
-                      piece_of_divided_name: str,
-                      full_name_length: int,
-                      start_index: int = 0) -> float:
+def calc_length_score(
+    kanji_statistics_repository: KanjiStatisticsRepository,
+    piece_of_divided_name: str,
+    full_name_length: int,
+    start_index: int = 0,
+) -> float:
     """
     Calculates length score.
     Length score is a feature, which is a kind of frequency,
     calculated from how long is family/given name containing the kanji.
     See this link if you need more explanation: https://rskmoi.hatenablog.com/entry/2017/01/15/190837
     :param kanji_statistics_repository: Class for managing Kanji statistics.
     :param piece_of_divided_name: Family name or given name
```

### Comparing `namedivider-python-0.2.1/namedivider/feature/kanji.py` & `namedivider_python-0.2.2/namedivider/feature/kanji.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Union
+from dataclasses import dataclass
 from pathlib import Path
-import pandas as pd
+from typing import Union
+
 import numpy as np
-from dataclasses import dataclass
+import numpy.typing as npt
+import pandas as pd
 
 
 @dataclass(frozen=True)
 class KanjiStatistics:
     """
     Statistics for a single kanji.
     :param kanji: A kanji.
@@ -74,28 +76,29 @@
             "里": [0, 1, 0, 0, 0, 0, 0, 0]
             "柴": [0, 1, 0, 0, 0, 0, 1, 0]
             "三": [0, 0, 0, 0, 0, 0, 2, 0]
             "郎": [0, 0, 0, 0, 0, 0, 2, 0]
             "田": [0, 1, 0, 0, 0, 0, 0, 0]
             "錬": [0, 0, 0, 0, 0, 0, 1, 0]
     """
+
     kanji: str
-    order_counts: np.ndarray
-    length_counts: np.ndarray
+    order_counts: npt.NDArray[np.int32]
+    length_counts: npt.NDArray[np.int32]
 
     @classmethod
     def default(cls) -> "KanjiStatistics":
         """
         Returns default kanji.
         :return: Default kanji
         :rtype: KanjiStatistics
         """
-        return cls(kanji="default",
-                   order_counts=np.array([0, 0, 0, 0, 0, 0]),
-                   length_counts=np.array([0, 0, 0, 0, 0, 0, 0, 0]))
+        return cls(
+            kanji="default", order_counts=np.array([0, 0, 0, 0, 0, 0]), length_counts=np.array([0, 0, 0, 0, 0, 0, 0, 0])
+        )
 
 
 class KanjiStatisticsRepository:
     """
     Repository class for managing KanjiStatistics.
     """
```

### Comparing `namedivider-python-0.2.1/namedivider/kanji_statistics.py` & `namedivider_python-0.2.2/namedivider/kanji_statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import warnings
-import numpy as np
 from dataclasses import dataclass
 
+import numpy as np
+import numpy.typing as npt
+
 
 @dataclass(frozen=True)
 class KanjiStatistics:
     """
     Statistics for a single kanji.
     :param kanji: A kanji.
     :param order_counts:
@@ -72,24 +74,28 @@
             "里": [0, 1, 0, 0, 0, 0, 0, 0]
             "柴": [0, 1, 0, 0, 0, 0, 1, 0]
             "三": [0, 0, 0, 0, 0, 0, 2, 0]
             "郎": [0, 0, 0, 0, 0, 0, 2, 0]
             "田": [0, 1, 0, 0, 0, 0, 0, 0]
             "錬": [0, 0, 0, 0, 0, 0, 1, 0]
     """
-    warnings.warn("namedivider.kanji_statistics.KanjiStatistics is deprecated in 0.2 and will be removed in 0.4. "
-                  "Use namedivider.feature.kanji.KanjiStatistics if you want to use KanjiStatistics class.",
-                  category=FutureWarning)
+
+    warnings.warn(
+        "namedivider.kanji_statistics.KanjiStatistics is deprecated in 0.2 and will be removed in 0.4. "
+        "Use namedivider.feature.kanji.KanjiStatistics if you want to use KanjiStatistics class.",
+        category=FutureWarning,
+        stacklevel=1,
+    )
     kanji: str
-    order_counts: np.ndarray
-    length_counts: np.ndarray
+    order_counts: npt.NDArray[np.int32]
+    length_counts: npt.NDArray[np.int32]
 
     @classmethod
     def default(cls) -> "KanjiStatistics":
         """
         Returns default kanji.
         :return: Default kanji
         :rtype: KanjiStatistics
         """
-        return cls(kanji="default",
-                   order_counts=np.array([0, 0, 0, 0, 0, 0]),
-                   length_counts=np.array([0, 0, 0, 0, 0, 0, 0, 0]))
+        return cls(
+            kanji="default", order_counts=np.array([0, 0, 0, 0, 0, 0]), length_counts=np.array([0, 0, 0, 0, 0, 0, 0, 0])
+        )
```

### Comparing `namedivider-python-0.2.1/namedivider/name_divider.py` & `namedivider_python-0.2.2/namedivider/name_divider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,64 @@
+import warnings
+from pathlib import Path
+from typing import List, Optional
+
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import regex
-import warnings
+
 from namedivider.divider.divided_name import DividedName
 from namedivider.feature.kanji import KanjiStatistics
-from pathlib import Path
-from typing import Optional
 
 CURRENT_DIR = Path(__file__).resolve().parent
 
 
 class NameDivider:
     def __init__(self, path_csv: str = f"{CURRENT_DIR}/assets/kanji.csv", separator: str = " "):
         """
         Class for dividing an undivided name
         ("undivided name" means names with no space between the family name and given name.)
         :param path_csv: Path of the file containing the kanji information
         :param separator: Characters to separate first and last names
         """
-        warnings.warn("Class NameDivider is deprecated in 0.2 and will be removed in 0.4. "
-                      "Use BasicNameDivider.from_version(NameDividerVersions.BASIC_NAME_DIVIDER_V1) "
-                      "if you want to use a class with same behavior.", category=FutureWarning)
+        warnings.warn(
+            "Class NameDivider is deprecated in 0.2 and will be removed in 0.4. "
+            "Use BasicNameDivider.from_version(NameDividerVersions.BASIC_NAME_DIVIDER_V1) "
+            "if you want to use a class with same behavior.",
+            category=FutureWarning,
+            stacklevel=1,
+        )
         kanji_records = pd.read_csv(path_csv).to_numpy()
         kanjis = kanji_records[:, 0]
         orders = kanji_records[:, 1:7]
         lengths = kanji_records[:, 7:]
 
         self.kanji_dict = {}
         for _kanji, _order, _length in zip(kanjis, orders, lengths):
             self.kanji_dict[_kanji] = KanjiStatistics(kanji=_kanji, order_counts=_order, length_counts=_length)
 
         self.default_kanji = KanjiStatistics.default()
         self.separator = separator
-        self.compiled_regex_kanji = regex.compile(r'\p{Script=Han}+')
+        self.compiled_regex_kanji = regex.compile(r"\p{Script=Han}+")
 
-    def _create_divided_name(self, family: str, given: str, score: float = 1., algorithm: str = "") -> DividedName:
+    def _create_divided_name(self, family: str, given: str, score: float = 1.0, algorithm: str = "") -> DividedName:
         """
         Generates DividedName.
         :param family: Family name
         :param given: Given name
         :param score: Confidence level, from 0 to 1
         :param algorithm: The name of dividing algorithm
         :return: Divided name
         :rtype: DividedName
         """
         return DividedName(family, given, separator=self.separator, score=score, algorithm=algorithm)
 
     @staticmethod
-    def _create_order_mask(full_name_length: int, char_idx: int) -> np.ndarray:
+    def _create_order_mask(full_name_length: int, char_idx: int) -> npt.NDArray[np.int32]:
         """
         Create order mask.
         Order mask is one-hot mask for calculate order score.
         :param full_name_length: Length of full name.
         :param char_idx: The order of the character in full name
         :return: Order mask
         :rtype: np.ndarray
@@ -67,15 +74,15 @@
 
         if char_idx == full_name_length - 2:
             return np.array([0, 0, 1, 1, 1, 0])
 
         return np.array([0, 1, 1, 1, 1, 0])
 
     @staticmethod
-    def _create_length_mask(full_name_length, char_idx) -> np.ndarray:
+    def _create_length_mask(full_name_length: int, char_idx: int) -> npt.NDArray[np.int32]:
         """
         Create length mask.
         Length mask is one-hot mask for calculate length score.
         :param full_name_length: Length of full name.
         :param char_idx: The order of the character in full name
         :return: Length mask
         :rtype: np.ndarray
@@ -84,24 +91,24 @@
         max_family = full_name_length - 1
         max_family = 4 if max_family > 4 else max_family
         min_given = full_name_length - char_idx
         max_given = full_name_length - 1
         max_given = 4 if max_given > 4 else max_given
         lc_family = np.array([0, 0, 0, 0])
         if min_family <= max_family:
-            lc_family[min_family - 1: max_family] = 1
+            lc_family[min_family - 1 : max_family] = 1
         lc_given = np.array([0, 0, 0, 0])
         if min_given <= max_given:
-            lc_given[min_given - 1: max_given] = 1
+            lc_given[min_given - 1 : max_given] = 1
         return np.concatenate([lc_family, lc_given])
 
     @staticmethod
-    def _calc_current_order_status(piece_of_divided_name: str,
-                                   idx_in_piece_of_divided_name: int,
-                                   is_family: bool) -> int:
+    def _calc_current_order_status(
+        piece_of_divided_name: str, idx_in_piece_of_divided_name: int, is_family: bool
+    ) -> int:
         """
         Determine which index of order_counts the kanji corresponds to.
         :param piece_of_divided_name: Family name or given name
         :param idx_in_piece_of_divided_name: Index in family or given name
         :param is_family: True if piece_of_divided_name is family name
         :return: The index of order_counts
         :rtype: int
@@ -156,24 +163,24 @@
         for idx_in_piece_of_divided_name, _kanji in enumerate(piece_of_divided_name):
             current_idx = start_index + idx_in_piece_of_divided_name
             if current_idx == 0:
                 continue
             if current_idx == full_name_length - 1:
                 continue
             mask = self._create_order_mask(full_name_length, current_idx)
-            current_order_status_idx = self._calc_current_order_status(piece_of_divided_name,
-                                                                       idx_in_piece_of_divided_name,
-                                                                       is_family)
+            current_order_status_idx = self._calc_current_order_status(
+                piece_of_divided_name, idx_in_piece_of_divided_name, is_family
+            )
             masked_order = self.kanji_dict.get(_kanji, self.default_kanji).order_counts * mask
             if np.sum(masked_order) == 0:
                 continue
             scores += masked_order[current_order_status_idx] / np.sum(masked_order)
         return scores
 
-    def _calc_length_score(self, piece_of_divided_name, full_name_length, start_index=0) -> float:
+    def _calc_length_score(self, piece_of_divided_name: str, full_name_length: int, start_index: int = 0) -> float:
         """
         Calculates length score.
         Length score is a feature, which is a kind of frequency,
         calculated from how long is family/given name containing the kanji.
         See this link if you need more explanation: https://rskmoi.hatenablog.com/entry/2017/01/15/190837
         :param piece_of_divided_name: Family name or given name
         :param full_name_length: Length of fullname
@@ -228,15 +235,15 @@
         length_score_family = self._calc_length_score(family, len(name), 0)
         length_score_given = self._calc_length_score(given, len(name), len(family))
         length_score = (length_score_family + length_score_given) / len(name)
 
         return (order_score + length_score) / 2
 
     @staticmethod
-    def _validate(undivided_name: str):
+    def _validate(undivided_name: str) -> None:
         """
         Determines if it is an assumed input.
         :param undivided_name: Names with no space between the first and last name
         """
         if len(undivided_name) < 2:
             raise ValueError("Name length needs at least 2 chars")
 
@@ -250,44 +257,45 @@
         :rtype:
             if fits the rules: DividedName
             else: None
         """
         # If the undivided name consists of 2 characters,
         # the first characters is family name, and the last characters is given name.
         if len(undivided_name) == 2:
-            return self._create_divided_name(family=undivided_name[0],
-                                             given=undivided_name[-1],
-                                             algorithm="rule")
+            return self._create_divided_name(family=undivided_name[0], given=undivided_name[-1], algorithm="rule")
 
         # If the undivided name consists of kanji and other types of characters (hiragana, katakana, etc...),
         # the undivided name will be divided where the kanji and other character types are switched.
         # The criterion for determining switched is whether "two" consecutive characters are having
         # different type of characters from first character type.
         # The reason of "two" is some family names consist of some kanji and one katakana.
         # (ex: "井ノ原", "三ツ又",　"関ヶ原" contains "ノ", "ツ", "ヶ". They are all katakana.)
         is_kanji_list = []
         for i, _char in enumerate(undivided_name):
             is_kanji = True if self.compiled_regex_kanji.fullmatch(_char) else False
             is_kanji_list.append(is_kanji)
             if i >= 2:
                 if is_kanji_list[0] != is_kanji and is_kanji_list[-2] == is_kanji:
-                    return self._create_divided_name(family=undivided_name[:i - 1],
-                                                     given=undivided_name[i - 1:],
-                                                     algorithm="rule")
+                    return self._create_divided_name(
+                        family=undivided_name[: i - 1], given=undivided_name[i - 1 :], algorithm="rule"
+                    )
+
+        return None
 
     @staticmethod
-    def _softmax(x) -> np.ndarray:
+    def _softmax(x: List[float]) -> List[float]:
         """
         Calculates softmax score
         :param x: array_like
         :return: Softmax scores
         :rtype: np.ndarray
         """
         u = np.sum(np.exp(x))
-        return np.exp(x) / u
+        softmax_val: List[float] = np.exp(x) / u
+        return softmax_val
 
     def _divide_by_statistics(self, undivided_name: str) -> DividedName:
         """
         Divides undivided name using kanji statistics.
         :param undivided_name: Names with no space between the family name and given name
         :return: Divided name
         :rtype: DividedName
@@ -297,18 +305,20 @@
             family = undivided_name[:i]
             given = undivided_name[i:]
             score = self.calc_score(family, given)
             total_scores.append(score)
 
         total_scores = self._softmax(total_scores)
         max_idx = np.argmax(np.array(total_scores)) + 1
-        return self._create_divided_name(family=undivided_name[:max_idx],
-                                         given=undivided_name[max_idx:],
-                                         score=total_scores[max_idx - 1],
-                                         algorithm="kanji_feature")
+        return self._create_divided_name(
+            family=undivided_name[:max_idx],
+            given=undivided_name[max_idx:],
+            score=total_scores[max_idx - 1],
+            algorithm="kanji_feature",
+        )
 
     def divide_name(self, undivided_name: str) -> DividedName:
         """
         Divides undivided name.
         :param undivided_name: Names with no space between the family name and given name
         :return: Divided name
         :rtype: DividedName
```

### Comparing `namedivider-python-0.2.1/namedivider/training/kanji_statistics_taker.py` & `namedivider_python-0.2.2/namedivider/training/kanji_statistics_taker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from enum import Enum, auto
-from namedivider.feature.kanji import KanjiStatistics
-import numpy as np
+from pathlib import Path
 from typing import Dict, List, Tuple, Union
-import regex
+
+import numpy as np
 import pandas as pd
-from pathlib import Path
+import regex
+
+from namedivider.feature.kanji import KanjiStatistics
 
 
 class KanjiStatisticsMode(Enum):
     ONLY_FREQUENT_KANJI = auto()
     ONLY_KANJI = auto()
     ALL = auto()
 
 
 class KanjiStatisticsTaker:
     """
     Create assets/kanji.csv from names.
     """
 
     def __init__(self, mode: KanjiStatisticsMode = KanjiStatisticsMode.ONLY_FREQUENT_KANJI):
-        self.statistics: Dict[str: KanjiStatistics] = {}
+        self.statistics: Dict[str, KanjiStatistics] = {}
         self.mode = mode
-        self.compiled_regex_kanji = regex.compile(r'\p{Script=Han}+')
+        self.compiled_regex_kanji = regex.compile(r"\p{Script=Han}+")
 
-    def is_target(self, target_kanji_statistics: KanjiStatistics):
+    def is_target(self, target_kanji_statistics: KanjiStatistics) -> bool:
         if self.mode == KanjiStatisticsMode.ALL:
             return True
         elif self.mode == KanjiStatisticsMode.ONLY_KANJI:
             if self.compiled_regex_kanji.fullmatch(target_kanji_statistics.kanji):
                 return True
             return False
         elif self.mode == KanjiStatisticsMode.ONLY_FREQUENT_KANJI:
@@ -50,66 +52,71 @@
             if idx == len(name) - 1:
                 return 5
             if idx == 0:
                 return 3
             return 4
 
     @staticmethod
-    def get_length(name, is_family: bool):
+    def get_length(name: str, is_family: bool) -> int:
         if is_family:
             return min(len(name) - 1, 3)
         else:
             return min(len(name) - 1 + 4, 7)
 
-    def set_kanji(self, text: str):
+    def set_kanji(self, text: str) -> None:
         for _kanji in text:
             if _kanji not in self.statistics:
-                self.statistics[_kanji] = KanjiStatistics(kanji=_kanji,
-                                                          order_counts=np.array([0, 0, 0, 0, 0, 0]),
-                                                          length_counts=np.array([0, 0, 0, 0, 0, 0, 0, 0]))
+                self.statistics[_kanji] = KanjiStatistics(
+                    kanji=_kanji,
+                    order_counts=np.array([0, 0, 0, 0, 0, 0]),
+                    length_counts=np.array([0, 0, 0, 0, 0, 0, 0, 0]),
+                )
 
-    def set_count(self, kanji: str, order: int, length: int):
+    def set_count(self, kanji: str, order: int, length: int) -> None:
         self.statistics[kanji].order_counts[order] += 1
         self.statistics[kanji].length_counts[length] += 1
 
-    def append(self, family: str, given: str):
+    def append(self, family: str, given: str) -> None:
         self.set_kanji(family + given)
         for i, _kanji in enumerate(family):
             _order = self.get_order(family, i, is_family=True)
             _length = self.get_length(family, is_family=True)
             self.set_count(kanji=_kanji, order=_order, length=_length)
         for i, _kanji in enumerate(given):
             _order = self.get_order(given, i, is_family=False)
             _length = self.get_length(given, is_family=False)
             self.set_count(kanji=_kanji, order=_order, length=_length)
 
-    def to_csv(self, dst: Union[str, Path]):
+    def to_csv(self, dst: Union[str, Path]) -> None:
         stats: List[Tuple[str, KanjiStatistics]] = sorted(self.statistics.items(), key=lambda x: x[0])
         items = []
         for _key, _stat in stats:
             if not self.is_target(_stat):
                 continue
-            items.append({"kanji": _stat.kanji,
-                          "oc_family_first": _stat.order_counts[0],
-                          "oc_family_other": _stat.order_counts[1],
-                          "oc_family_last": _stat.order_counts[2],
-                          "oc_given_first": _stat.order_counts[3],
-                          "oc_given_other": _stat.order_counts[4],
-                          "oc_given_last": _stat.order_counts[5],
-                          "lc_family_1": _stat.length_counts[0],
-                          "lc_family_2": _stat.length_counts[1],
-                          "lc_family_3": _stat.length_counts[2],
-                          "lc_family_4": _stat.length_counts[3],
-                          "lc_given_1": _stat.length_counts[4],
-                          "lc_given_2": _stat.length_counts[5],
-                          "lc_given_3": _stat.length_counts[6],
-                          "lc_given_4": _stat.length_counts[7]
-                          })
+            items.append(
+                {
+                    "kanji": _stat.kanji,
+                    "oc_family_first": _stat.order_counts[0],
+                    "oc_family_other": _stat.order_counts[1],
+                    "oc_family_last": _stat.order_counts[2],
+                    "oc_given_first": _stat.order_counts[3],
+                    "oc_given_other": _stat.order_counts[4],
+                    "oc_given_last": _stat.order_counts[5],
+                    "lc_family_1": _stat.length_counts[0],
+                    "lc_family_2": _stat.length_counts[1],
+                    "lc_family_3": _stat.length_counts[2],
+                    "lc_family_4": _stat.length_counts[3],
+                    "lc_given_1": _stat.length_counts[4],
+                    "lc_given_2": _stat.length_counts[5],
+                    "lc_given_3": _stat.length_counts[6],
+                    "lc_given_4": _stat.length_counts[7],
+                }
+            )
         df = pd.DataFrame(items)
         df.to_csv(dst, index=False)
 
-    def show(self):
+    def show(self) -> None:
         stats = sorted(self.statistics.items(), key=lambda x: x[0])
         for _key, _stat in stats:
             if not self.is_target(_stat):
                 continue
             print(_stat)
```

### Comparing `namedivider-python-0.2.1/namedivider/util.py` & `namedivider_python-0.2.2/namedivider/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import requests
 from pathlib import Path
 from typing import Union
 
+import requests
+
 CURRENT_DIR = Path(__file__).resolve().parent
 DEFAULT_CACHE_DIR = Path("~/.cache/namedivider-python").expanduser()
 GBDT_MODEL_V1_URL = "https://github.com/rskmoi/namedivider-python/releases/download/Models/gbdt_model_v1.txt"
-FAMILY_NAME_REPOSITORY_URL = \
+FAMILY_NAME_REPOSITORY_URL = (
     "https://github.com/rskmoi/namedivider-python/releases/download/Models/family_name_repository.pickle"
+)
 
 
 def get_kanji_csv_default_path() -> Path:
     """
     Returns the default path of kanji.csv.
     """
     return CURRENT_DIR / "assets" / "kanji.csv"
@@ -26,34 +28,36 @@
 def get_gbdt_model_v1_default_path() -> Path:
     """
     Returns the default path of gbdt_model_v1.txt
     """
     return (DEFAULT_CACHE_DIR / "gbdt_model_v1.txt").expanduser()
 
 
-def download_family_name_pickle_if_needed(path: Union[str, Path]):
+def download_family_name_pickle_if_needed(path: Union[str, Path]) -> None:
     """
     When a default path is provided, download from the Internet if not already downloaded.
     """
-    if Path(path) != get_family_name_pkl_default_path():
+    path = Path(path)
+    if path != get_family_name_pkl_default_path():
         return None
     if path.exists():
         return None
     DEFAULT_CACHE_DIR.mkdir(exist_ok=True, parents=True)
     print("Download FamilyNameRepository from GitHub...")
     content = requests.get(FAMILY_NAME_REPOSITORY_URL).content
     with open(path, "wb") as f:
         f.write(content)
 
 
-def download_gbdt_model_v1_if_needed(path: Union[str, Path]):
+def download_gbdt_model_v1_if_needed(path: Union[str, Path]) -> None:
     """
     When a default path is provided, download from the Internet if not already downloaded.
     """
-    if Path(path) != get_gbdt_model_v1_default_path():
+    path = Path(path)
+    if path != get_gbdt_model_v1_default_path():
         return None
     if path.exists():
         return None
     DEFAULT_CACHE_DIR.mkdir(exist_ok=True, parents=True)
     print("Download GBDT Model from GitHub...")
     content = requests.get(GBDT_MODEL_V1_URL).content
     with open(path, "wb") as f:
```

