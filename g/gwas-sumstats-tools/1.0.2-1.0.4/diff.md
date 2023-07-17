# Comparing `tmp/gwas_sumstats_tools-1.0.2.tar.gz` & `tmp/gwas_sumstats_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas_sumstats_tools-1.0.2.tar", max compression
+gzip compressed data, was "gwas_sumstats_tools-1.0.4.tar", max compression
```

## Comparing `gwas_sumstats_tools-1.0.2.tar` & `gwas_sumstats_tools-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.2/LICENSE
--rw-r--r--   0        0        0     5207 2023-06-06 14:58:15.047099 gwas_sumstats_tools-1.0.2/README.md
--rwxr-xr-x   0        0        0    11560 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/cli.py
--rwxr-xr-x   0        0        0     1387 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/config.py
--rwxr-xr-x   0        0        0     5380 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/format.py
--rwxr-xr-x   0        0        0    10291 2023-06-06 14:58:15.071099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/data_table.py
--rwxr-xr-x   0        0        0     7574 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/metadata.py
--rwxr-xr-x   0        0        0     3913 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/read.py
--rwxr-xr-x   0        0        0     5754 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/data_table.py
--rwxr-xr-x   0        0        0     1816 2023-06-06 14:58:15.099099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/metadata.py
--rwxr-xr-x   0        0        0     4773 2023-06-06 14:58:15.118099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/utils.py
--rwxr-xr-x   0        0        0     8337 2023-06-06 14:58:15.119099 gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/validate.py
--rw-r--r--   0        0        0      695 2023-06-21 12:34:18.075637 gwas_sumstats_tools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5207 2023-06-06 14:58:15.047099 gwas_sumstats_tools-1.0.4/README.md
+-rwxr-xr-x   0        0        0    11560 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/cli.py
+-rwxr-xr-x   0        0        0     1841 2023-07-17 16:59:13.678964 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/config.py
+-rwxr-xr-x   0        0        0     5380 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/format.py
+-rwxr-xr-x   0        0        0    10291 2023-06-06 14:58:15.071099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/interfaces/data_table.py
+-rwxr-xr-x   0        0        0     7574 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/interfaces/metadata.py
+-rwxr-xr-x   0        0        0     3913 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/read.py
+-rwxr-xr-x   0        0        0     5754 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/schema/data_table.py
+-rwxr-xr-x   0        0        0     1816 2023-06-06 14:58:15.099099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/schema/metadata.py
+-rwxr-xr-x   0        0        0     4773 2023-06-06 14:58:15.118099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/utils.py
+-rwxr-xr-x   0        0        0     8337 2023-06-06 14:58:15.119099 gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/validate.py
+-rw-r--r--   0        0        0      695 2023-07-17 16:59:13.678964 gwas_sumstats_tools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.4/PKG-INFO
```

### Comparing `gwas_sumstats_tools-1.0.2/LICENSE` & `gwas_sumstats_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/README.md` & `gwas_sumstats_tools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/cli.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/cli.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/config.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,62 @@
+import os
 
-GWAS_CAT_API_STUDIES_URL = "https://www.ebi.ac.uk/gwas/rest/api/studies/"
 
-GWAS_CAT_API_INGEST_STUDIES_URL = "https://wwwdev.ebi.ac.uk/gwas/ingest/api/v2/studies/"
+def _env_variable_else(env_var_name: str, default: str) -> str:
+    """Get an environment variable
+
+    Arguments:
+        env_var_name -- variable name
+        default -- default value
+
+    Returns:
+        value of environment variable
+    """
+    value = os.environ.get(env_var_name)
+    return value if value else default
+
+
+GWAS_CAT_API_STUDIES_URL = _env_variable_else(
+    "GWAS_CAT_API_STUDIES_URL", "https://www.ebi.ac.uk/gwas/rest/api/studies/"
+)
+
+GWAS_CAT_API_INGEST_STUDIES_URL = _env_variable_else(
+    "GWAS_CAT_API_INGEST_STUDIES_URL",
+    "https://www.ebi.ac.uk/gwas/ingest/api/v2/studies/",
+)
 
 GWAS_CAT_STUDY_MAPPINGS = {
-    'genotyping_technology': 'genotyping_technology',
-    'traitDescription': 'trait_description',
-    'effect_allele_frequency_lower_limit': 'minor_allele_freq_lower_limit',
-    'minor_allele_frequency_lower_limit': 'minor_allele_freq_lower_limit',
-    'summary_statistics_assembly': 'genome_assembly',
-    'analysisSoftware': 'analysis_software',
-    'imputationPanel': 'imputation_panel',
-    'imputationSoftware': 'imputation_software',
-    'adjustedCovariates': 'adjusted_covariates',
-    'ontologyMapping': 'ontology_mapping',
-    'readme_file': 'author_notes',
-    'readme_text': 'author_notes',
-    'coordinateSystem': 'coordinate_system',
-    'sex': 'sex'
-    }
+    "genotyping_technology": "genotyping_technology",
+    "traitDescription": "trait_description",
+    "effect_allele_frequency_lower_limit": "minor_allele_freq_lower_limit",
+    "minor_allele_frequency_lower_limit": "minor_allele_freq_lower_limit",
+    "summary_statistics_assembly": "genome_assembly",
+    "analysisSoftware": "analysis_software",
+    "imputationPanel": "imputation_panel",
+    "imputationSoftware": "imputation_software",
+    "adjustedCovariates": "adjusted_covariates",
+    "ontologyMapping": "ontology_mapping",
+    "readme_file": "author_notes",
+    "readme_text": "author_notes",
+    "coordinateSystem": "coordinate_system",
+    "sex": "sex",
+}
 
 GWAS_CAT_SAMPLE_MAPPINGS = {
-    'size': 'sample_size',
-    'ancestry': 'sample_ancestry',
-    'ancestryMethod': 'ancestry_method',
-    'caseControlStudy': 'case_control_study',
-    'caseCount': 'case_count',
-    'controlCount': 'control_count'
+    "size": "sample_size",
+    "ancestry": "sample_ancestry",
+    "ancestryMethod": "ancestry_method",
+    "caseControlStudy": "case_control_study",
+    "caseCount": "case_count",
+    "controlCount": "control_count",
 }
 
-GENOME_ASSEMBLY_MAPPINGS = {
-    '36': 'GRCh36',
-    '37': 'GRCh37',
-    '38': 'GRCh38'
-    }
-
-STUDY_FIELD_TO_SPLIT = ('genotyping_technology', 'trait_description', 'ontology_mapping', 'adjusted_covariates')
+GENOME_ASSEMBLY_MAPPINGS = {"36": "GRCh36", "37": "GRCh37", "38": "GRCh38"}
 
-SAMPLE_FIELD_TO_SPLIT = ('ancestry_method', 'sample_ancestry')
+STUDY_FIELD_TO_SPLIT = (
+    "genotyping_technology",
+    "trait_description",
+    "ontology_mapping",
+    "adjusted_covariates",
+)
 
+SAMPLE_FIELD_TO_SPLIT = ("ancestry_method", "sample_ancestry")
```

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/format.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/format.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/data_table.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/interfaces/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/interfaces/metadata.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/interfaces/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/read.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/read.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/data_table.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/schema/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/schema/metadata.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/utils.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/utils.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/gwas_sumstats_tools/validate.py` & `gwas_sumstats_tools-1.0.4/gwas_sumstats_tools/validate.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.2/pyproject.toml` & `gwas_sumstats_tools-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwas-sumstats-tools"
-version = "1.0.2"
+version = "1.0.4"
 description = ""
 authors = ["jdhayhurst <jhayhurst@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "gwas_sumstats_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gwas_sumstats_tools-1.0.2/PKG-INFO` & `gwas_sumstats_tools-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas-sumstats-tools
-Version: 1.0.2
+Version: 1.0.4
 Summary: 
 Author: jdhayhurst
 Author-email: jhayhurst@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

