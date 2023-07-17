# Comparing `tmp/HawaData-0.7.6.tar.gz` & `tmp/HawaData-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.7.6.tar", last modified: Mon Jun 26 06:30:02 2023, max compression
+gzip compressed data, was "HawaData-0.7.7.tar", last modified: Mon Jul 17 07:07:39 2023, max compression
```

## Comparing `HawaData-0.7.6.tar` & `HawaData-0.7.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.060936 HawaData-0.7.6/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.049295 HawaData-0.7.6/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3207 2023-06-26 06:30:01.000000 HawaData-0.7.6/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-06-26 06:30:02.000000 HawaData-0.7.6/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-26 06:30:01.000000 HawaData-0.7.6/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-26 06:30:01.000000 HawaData-0.7.6/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3207 2023-06-26 06:30:02.060658 HawaData-0.7.6/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.6/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.049834 HawaData-0.7.6/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.6/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.052650 HawaData-0.7.6/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.6/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.6/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.6/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.6/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.6/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.054354 HawaData-0.7.6/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.6/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    15442 2023-06-26 06:26:56.000000 HawaData-0.7.6/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6169 2023-06-26 06:18:33.000000 HawaData-0.7.6/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.6/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2696 2023-06-26 02:08:50.000000 HawaData-0.7.6/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.057923 HawaData-0.7.6/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.6/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.6/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.6/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.6/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.7.6/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-21 13:09:45.000000 HawaData-0.7.6/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.6/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.059306 HawaData-0.7.6/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.6/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28407 2023-06-26 01:39:47.000000 HawaData-0.7.6/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.6/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-26 06:30:02.061024 HawaData-0.7.6/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.6/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.060058 HawaData-0.7.6/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.6/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.796785 HawaData-0.7.7/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.784547 HawaData-0.7.7/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3239 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3239 2023-07-17 07:07:39.796414 HawaData-0.7.7/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.7/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.785225 HawaData-0.7.7/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.7/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.788105 HawaData-0.7.7/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.7/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.7/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.7/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.7/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.7/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.789379 HawaData-0.7.7/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.7/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    15412 2023-07-17 07:06:20.000000 HawaData-0.7.7/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6169 2023-07-17 07:07:13.000000 HawaData-0.7.7/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.7/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2696 2023-06-26 02:08:50.000000 HawaData-0.7.7/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.793272 HawaData-0.7.7/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.7/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.7/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.7/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.7/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.7.7/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1055 2023-07-17 06:57:10.000000 HawaData-0.7.7/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.7/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.795181 HawaData-0.7.7/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.7/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28407 2023-06-26 01:39:47.000000 HawaData-0.7.7/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5373 2023-07-17 07:05:31.000000 HawaData-0.7.7/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-17 07:07:39.796893 HawaData-0.7.7/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.7/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.795535 HawaData-0.7.7/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.7/test/test_query.py
```

### Comparing `HawaData-0.7.6/HawaData.egg-info/PKG-INFO` & `HawaData-0.7.7/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.6
+Version: 0.7.7
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -108,7 +108,8 @@
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
 - 0.7.5 add ch key for dim_field data
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
+- 0.7.7 add school mht api data
```

### Comparing `HawaData-0.7.6/HawaData.egg-info/SOURCES.txt` & `HawaData-0.7.7/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/PKG-INFO` & `HawaData-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.6
+Version: 0.7.7
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -108,7 +108,8 @@
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
 - 0.7.5 add ch key for dim_field data
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
+- 0.7.7 add school mht api data
```

### Comparing `HawaData-0.7.6/README.md` & `HawaData-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/base/db.py` & `HawaData-0.7.7/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/base/init.py` & `HawaData-0.7.7/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/common/data.py` & `HawaData-0.7.7/hawa/common/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     last_year = None
     last_year_code_scores: Optional[pd.DataFrame] = field(default_factory=pd.DataFrame)
 
     def __post_init__(self):
         # 初始化数据
         init_functions = [i for i in dir(self) if i.startswith('_to_init_')]
         for func in init_functions:
-            print(f"{func=}")
             getattr(self, func)()
 
         # 构建辅助工具
         self._to_build_helper()
 
         # 计算数据
         count_functions = [i for i in dir(self) if i.startswith('_to_count_')]
```

### Comparing `HawaData-0.7.6/hawa/common/query.py` & `HawaData-0.7.7/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/common/utils.py` & `HawaData-0.7.7/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/config.py` & `HawaData-0.7.7/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/data/klass.py` & `HawaData-0.7.7/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/data/province.py` & `HawaData-0.7.7/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/data/school.py` & `HawaData-0.7.7/hawa/data/school.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 
 from hawa.paper.health import HealthReportData, HealthApiData
-from hawa.paper.mht import MhtWebData
+from hawa.paper.mht import MhtWebData, MhtApiData
 
 
 @dataclass
 class SchoolMixin:
     """为了在 __mro__ 中有更高的优先级， mixin 在继承时，应该放在最前"""
     meta_unit_type: str = 'school'
 
@@ -23,10 +23,15 @@
 
 @dataclass
 class SchoolHealthReportData(SchoolMixin, HealthReportData):
     pass
 
 
 @dataclass
+class SchoolMhtApiData(SchoolMixin, MhtApiData):
+    meta_unit_type: str = 'school'
+
+
+@dataclass
 class SchoolMhtWebData(SchoolMixin, MhtWebData):
     meta_unit_type: str = 'school'
     pass
```

### Comparing `HawaData-0.7.6/hawa/data/student.py` & `HawaData-0.7.7/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/paper/health.py` & `HawaData-0.7.7/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/hawa/paper/mht.py` & `HawaData-0.7.7/hawa/paper/mht.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from hawa.common.data import CommonData
 from hawa.config import project
 
 
 @dataclass
 class MhtData(CommonData):
-    test_type: str = 'mht'
+    test_types: list[str] = field(default_factory=lambda: ['mht', 'mhtPlus'])
     code_word_list: Set[str] = field(default_factory=lambda: {'mht'})
 
     # 计算数据
     scale_student_score: dict = field(default_factory=dict)
     sub_scale_score: dict = field(default_factory=dict)
     grade_scale_student_score: dict = field(default_factory=list)
     grade_sub_scale_score: dict = field(default_factory=dict)
@@ -128,7 +128,12 @@
             "y_axis": y_axis,
         }
 
 
 @dataclass
 class MhtWebData(MhtData):
     pass
+
+
+@dataclass
+class MhtApiData(MhtData):
+    pass
```

### Comparing `HawaData-0.7.6/setup.py` & `HawaData-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.6/test/test_query.py` & `HawaData-0.7.7/test/test_query.py`

 * *Files identical despite different names*

