# Comparing `tmp/phc-ingestion-0.3.40.tar.gz` & `tmp/phc-ingestion-0.3.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.40.tar", last modified: Fri Jun 23 16:45:26 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.41.tar", last modified: Mon Jul 17 19:45:51 2023, max compression
```

## Comparing `phc-ingestion-0.3.40.tar` & `phc-ingestion-0.3.41.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-23 16:45:03.800337 phc-ingestion-0.3.40/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-23 16:45:03.800337 phc-ingestion-0.3.40/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-23 16:45:03.800337 phc-ingestion-0.3.40/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21663 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5907 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3142 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     5489 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8461 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-23 16:45:03.808337 phc-ingestion-0.3.40/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.40/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-07-17 19:45:25.380599 phc-ingestion-0.3.41/PYPI.md
+-rw-r--r--   0        0        0        0 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1636 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4676 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21663 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     6850 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3142 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-07-17 19:45:25.388599 phc-ingestion-0.3.41/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     5489 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8461 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-07-17 19:45:25.392599 phc-ingestion-0.3.41/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.41/PKG-INFO
```

### Comparing `phc-ingestion-0.3.40/ingestion/caris/process.py` & `phc-ingestion-0.3.41/ingestion/caris/process.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,24 +20,24 @@
         },
     }
 
     with scoped_logger(__name__) as log:
         os.makedirs(f"{outpath}", exist_ok=True)
         somatic_vcf_line_count = 0
         germline_vcf_line_count = 0
-        result, germline_case_id, file_genome_references = process_caris_json(
+        result, germline_case_id, file_genome_references, json_data = process_caris_json(
             infile, outpath, file_name, source_file_id, ingest_status, log
         )
         if "somatic_vcf" in result:
             somatic_vcf_line_count = process_caris_vcf(
-                result["somatic_vcf"], outpath, file_name, log
+                result["somatic_vcf"], json_data, outpath, file_name, log
             )
         if "germline_vcf" in result:
             germline_vcf_line_count = process_caris_vcf(
-                result["germline_vcf"], outpath, file_name, log
+                result["germline_vcf"], json_data, outpath, file_name, log
             )
         case_metadata = {
             "germline_case_id": germline_case_id,
             "somatic_vcf_line_count": somatic_vcf_line_count,
             "germline_vcf_line_count": germline_vcf_line_count,
         }
```

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.41/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.41/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.41/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.41/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/json.py` & `phc-ingestion-0.3.41/ingestion/caris/util/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,16 @@
         metadata["files"] = metadata["files"] + vcf_results
         for vcf in vcf_results:
             seq_type = vcf.get("sequenceType")
             file_genome_references[f"{seq_type}_genome_reference"] = vcf["reference"]
 
     create_yaml(metadata, file_name, ingest_status)
 
-    # Return VCF files for immediate processing
+    # Return VCF files for immediate processing, and JSON data for adding vendsig
     result = {}
 
     if somatic_filename is not None:
         result["somatic_vcf"] = f"{outpath}/{somatic_filename}"
     if germline_filename is not None:
         result["germline_vcf"] = f"{outpath}/{germline_filename}"
 
-    return (result, germline_case_id, file_genome_references)
+    return (result, germline_case_id, file_genome_references, data)
```

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.41/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.41/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.41/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.41/ingestion/caris/util/vcf.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,15 +36,50 @@
                 "reference": genome_reference,
             }
         )
 
     return vcfs
 
 
-def process_caris_vcf(infile, outpath, file_name, log: Logger):
+def get_vendsig_dict(json_data, log: Logger):
+    # Return a dicitionary of {'chr:star_pos:ref:alt' : 'vendsig'}
+    vendsig_dict = {}
+    for test in json_data["tests"]:
+        for result in test["testResults"]:
+            if (
+                "genomicAlteration" in result.keys()
+                and "alterationDetails" in result["genomicAlteration"].keys()
+            ):
+                vendsig = map_vendsig(result["genomicAlteration"]["result"])
+                sv = result["genomicAlteration"]["alterationDetails"]["transcriptAlterationDetails"]
+                vendsig_dict.update(
+                    {
+                        f'{result["genomicAlteration"]["chromosome"]}:{sv["transcriptStartPosition"]}:{sv["referenceNucleotide"]}:{sv["observedNucleotide"]}': vendsig
+                    }
+                )
+
+    return vendsig_dict
+
+
+def map_vendsig(ci: str) -> str:
+    if ci in ["Pathogenic Variant", "Pathogenic"]:
+        return "VENDSIG=Pathogenic"
+    elif ci in ["Likely Pathogenic Variant", "Likely Pathogenic"]:
+        return "VENDSIG=Likely pathogenic"
+    elif ci in ["Benign Variant", "Benign"]:
+        return "VENDSIG=Benign"
+    elif ci in ["Likely Benign Variant", "Likely Benign"]:
+        return "VENDSIG=Likely benign"
+    elif ci in ["Variant of Uncertain Significance", "VUS"]:
+        return "VENDSIG=Uncertain significance"
+    else:
+        return "VENDSIG=Unknown"
+
+
+def process_caris_vcf(infile, json_data, outpath, file_name, log: Logger):
     line_count = 0
     if "germline.vcf" in infile:
         out_vcf = f"{outpath}/{file_name}.modified.germline.vcf"
     else:
         out_vcf = f"{outpath}/{file_name}.modified.somatic.vcf"
 
     if infile.endswith(".gz"):
@@ -59,14 +94,17 @@
                     )
                 )
                 sys.exit(9)
             fin = subprocess.Popen("unzip -p " + infile, shell=True, stdout=subprocess.PIPE).stdout
         else:
             fin = open(infile, "rb")
 
+    # Read in a dictionary of variants with VENDSIG from the JSON file
+    vendsig_dict = get_vendsig_dict(json_data, log)
+
     foutW = gzip.open(f"{out_vcf}.gz", "wt")
 
     foutW.write("##fileformat=VCFv4.1\n")
     foutW.write("##filedate=" + datetime.datetime.now().isoformat() + "\n")
     foutW.write('##FILTER=<ID=PASS,Description="All filters passed">\n')
     foutW.write('##FILTER=<ID=R8,Description="IndelRepeatLength is greater than 8">\n')
     foutW.write(
@@ -129,35 +167,19 @@
         for data in info_field_list:
             if data.split("=")[0] == "DP":
                 depth = data.split("=")[1]
 
         # We need to put this in the proper format for ingestion into omics explore.
         new_sample_field = ":".join([sample_field_list[0], sample_field_list[2], depth])
 
-        # Retaining the Clinical Impact field
-        ci = re.sub(
-            '"', "", "".join([data for data in info_field_list if data.split("=")[0] == "CI"])
+        # Adding a VENDSIG field to the INFO
+        vendsig_lookup = vendsig_dict.get(
+            f"{recList[0]}:{recList[1]}:{recList[3]}:{recList[4]}", "VENDSIG=Unknown"
         )
-        mapped_ci = map_vendsig(ci)
 
-        vcf_info = f"AF={sample_field_list[1]};{mapped_ci}"
+        vcf_info = f"AF={sample_field_list[1]};{vendsig_lookup}"
 
         foutW.write("\t".join([genomic_record, vcf_info, vcf_format, new_sample_field]) + "\n")
 
     finR.close()
     foutW.close()
     return line_count
-
-
-def map_vendsig(ci: str) -> str:
-    if ci in ["CI=PathogenicVariant", "CI=Pathogenic"]:
-        return "VENDSIG=Pathogenic"
-    elif ci in ["CI=LikelyPathogenicVariant", "CI=Likely_Pathogenic"]:
-        return "VENDSIG=Likely pathogenic"
-    elif ci in ["CI=BenignVariant", "CI=Benign"]:
-        return "VENDSIG=Benign"
-    elif ci in ["CI=LikelyBenignVariant", "CI=Likely_Benign"]:
-        return "VENDSIG=Likely benign"
-    elif ci in ["CI=VariantofUncertainSignificance", "CI=VUS"]:
-        return "VENDSIG=Uncertain significance"
-    else:
-        return "VENDSIG=Unknown"
```

### Comparing `phc-ingestion-0.3.40/ingestion/foundation/process.py` & `phc-ingestion-0.3.41/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.41/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.41/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.41/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.41/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/nextgen/process.py` & `phc-ingestion-0.3.41/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.41/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.41/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.41/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.41/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.41/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.41/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.41/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.41/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.41/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.40/pyproject.toml` & `phc-ingestion-0.3.41/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.40"
+version = "0.3.41"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

