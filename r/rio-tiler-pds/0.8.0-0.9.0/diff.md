# Comparing `tmp/rio-tiler-pds-0.8.0.tar.gz` & `tmp/rio_tiler_pds-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-tiler-pds-0.8.0.tar", last modified: Tue Apr 11 19:04:56 2023, max compression
+gzip compressed data, was "rio_tiler_pds-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rio-tiler-pds-0.8.0.tar` & `rio_tiler_pds-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0      217 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1266 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/.gitignore
--rw-r--r--   0        0        0      795 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/AUTHORS.txt
--rw-r--r--   0        0        0     5159 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/CHANGES.md
--rw-r--r--   0        0        0     1506 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0    15113 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/README.md
--rw-r--r--   0        0        0     2152 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       99 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/__init__.py
--rw-r--r--   0        0        0      132 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/__init__.py
--rw-r--r--   0        0        0       90 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/aws/__init__.py
--rw-r--r--   0        0        0     2055 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/aws/cbers4.py
--rw-r--r--   0        0        0     2602 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/utils.py
--rw-r--r--   0        0        0      474 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/errors.py
--rw-r--r--   0        0        0      138 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/__init__.py
--rw-r--r--   0        0        0      115 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/aws/__init__.py
--rw-r--r--   0        0        0     3981 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/aws/landsat_collection2.py
--rw-r--r--   0        0        0     5249 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/utils.py
--rw-r--r--   0        0        0      132 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/__init__.py
--rw-r--r--   0        0        0      238 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/__init__.py
--rw-r--r--   0        0        0     3750 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_astraea.py
--rw-r--r--   0        0        0     3257 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_pds.py
--rw-r--r--   0        0        0    24642 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/modland_grid.py
--rw-r--r--   0        0        0     1326 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/utils.py
--rw-r--r--   0        0        0      163 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/__init__.py
--rw-r--r--   0        0        0      205 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/__init__.py
--rw-r--r--   0        0        0     2877 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel1.py
--rw-r--r--   0        0        0     9492 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel2.py
--rw-r--r--   0        0        0     5426 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/utils.py
--rw-r--r--   0        0        0     1326 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/utils.py
--rw-r--r--   0        0        0    16425 1970-01-01 00:00:00.000000 rio-tiler-pds-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-07-17 12:26:22.041819 rio_tiler_pds-0.9.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1266 2023-07-17 12:26:22.041819 rio_tiler_pds-0.9.0/.gitignore
+-rw-r--r--   0        0        0      822 2023-07-17 12:26:22.041819 rio_tiler_pds-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2023-07-17 12:26:22.041819 rio_tiler_pds-0.9.0/AUTHORS.txt
+-rw-r--r--   0        0        0     5375 2023-07-17 12:26:22.041819 rio_tiler_pds-0.9.0/CHANGES.md
+-rw-r--r--   0        0        0     1506 2023-07-17 12:26:22.041819 rio_tiler_pds-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0    15979 2023-07-17 12:26:22.041819 rio_tiler_pds-0.9.0/README.md
+-rw-r--r--   0        0        0     2161 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/cbers/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/cbers/aws/__init__.py
+-rw-r--r--   0        0        0     2055 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/cbers/aws/cbers4.py
+-rw-r--r--   0        0        0     2602 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/cbers/utils.py
+-rw-r--r--   0        0        0       81 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/copernicus/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/copernicus/aws/__init__.py
+-rw-r--r--   0        0        0     7921 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/copernicus/aws/dem.py
+-rw-r--r--   0        0        0      474 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/errors.py
+-rw-r--r--   0        0        0      138 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/landsat/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/landsat/aws/__init__.py
+-rw-r--r--   0        0        0     3981 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/landsat/aws/landsat_collection2.py
+-rw-r--r--   0        0        0     5249 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/landsat/utils.py
+-rw-r--r--   0        0        0      132 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/modis/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/modis/aws/__init__.py
+-rw-r--r--   0        0        0     3750 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/modis/aws/modis_astraea.py
+-rw-r--r--   0        0        0     3257 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/modis/aws/modis_pds.py
+-rw-r--r--   0        0        0    24642 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/modis/modland_grid.py
+-rw-r--r--   0        0        0     1326 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/modis/utils.py
+-rw-r--r--   0        0        0      163 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/aws/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/aws/sentinel1.py
+-rw-r--r--   0        0        0     9492 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/aws/sentinel2.py
+-rw-r--r--   0        0        0     5426 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/utils.py
+-rw-r--r--   0        0        0     3186 2023-07-17 12:26:22.045819 rio_tiler_pds-0.9.0/rio_tiler_pds/utils.py
+-rw-r--r--   0        0        0    17312 1970-01-01 00:00:00.000000 rio_tiler_pds-0.9.0/PKG-INFO
```

### Comparing `rio-tiler-pds-0.8.0/.gitignore` & `rio_tiler_pds-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/.pre-commit-config.yaml` & `rio_tiler_pds-0.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -27,7 +27,8 @@
     hooks:
       - id: mypy
         language_version: python
         # No reason to run if only tests have changed. They intentionally break typing.
         exclude: tests/.*
         additional_dependencies:
         - types-attrs
+        - types-cachetools
```

### Comparing `rio-tiler-pds-0.8.0/CHANGES.md` & `rio_tiler_pds-0.9.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release Notes
 
+## 0.9.0 (2023-07-13)
+
+* update rio-tiler requirement to `>=5.0,<6.0`
+* add `rio_tiler_pds.copernicus.aws.Dem30Reader` and `rio_tiler_pds.copernicus.aws.Dem90Reader` **mosaic** readers
+* add `boto3` in dependencies
+
 ## 0.8.0 (2023-04-11)
 
 * remove Landsat 8 Collection 1
 * remove python 3.7 and add python 3.10/3.11 support
 * switch to ruff
 * fix issue with latest STAC Items for Sentinel-2-l2a-cogs (author @dvd3v, https://github.com/cogeotiff/rio-tiler-pds/pull/64)
 * update rio-tiler requirement to `>=4.0,<5.0`
```

### Comparing `rio-tiler-pds-0.8.0/LICENSE.txt` & `rio_tiler_pds-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/README.md` & `rio_tiler_pds-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,23 +58,25 @@
 | [Sentinel 2][s2_l2a_jp2]                  | L2A                                         | JPEG2000                   | Sinergise / AWS            | eu-central-1 | **Requester-pays** |
 | [Sentinel 2][s2_l2a_cog]                  | L2A                                         | COG                        | Digital Earth Africa / AWS | us-west-2    | Public             |
 | [Sentinel 1][s1_l1c_cog]                  | L1C                                         | COG (Internal GCPS)        | Sinergise / AWS            | eu-central-1 | **Requester-pays** |
 | [Landsat Collection 2][landsat_c2_cog]    | L1,L2                                       | COG                        | USGS / AWS                 | us-west-2    | **Requester-pays** |
 | [CBERS 4/4A][cbers_cog]                   | L2/L4                                       | COG                        | AMS Kepler / AWS           | us-east-1    | **Requester-pays** |
 | [MODIS (modis-pds)][modis_pds]            | MCD43A4, MOD09GQ, MYD09GQ, MOD09GA, MYD09GA | GTiff (External Overviews) | -                          | us-west-2    | Public             |
 | [MODIS (astraea-opendata)][modis_astraea] | MCD43A4, MOD11A1, MOD13A1, MYD11A1 MYD13A1  | COG                        | Astraea / AWS              | us-west-2    | **Requester-pays** |
+| [Copernicus Digital Elevation Model][copernicus_dem] | GLO-30, GLO-90                   | COG                        | Sinergise / AWS            | eu-central-1    | Public |
 
 [s2_l1c_jp2]: https://registry.opendata.aws/sentinel-2/
 [s2_l2a_jp2]: https://registry.opendata.aws/sentinel-2/
 [s2_l2a_cog]: https://registry.opendata.aws/sentinel-2-l2a-cogs/
 [s1_l1c_cog]: https://registry.opendata.aws/sentinel-1/
 [landsat_c2_cog]: https://www.usgs.gov/core-science-systems/nli/landsat/landsat-commercial-cloud-data-access
 [cbers_cog]: https://registry.opendata.aws/cbers/
 [modis_pds]: https://docs.opendata.aws/modis-pds/readme.html
 [modis_astraea]: https://registry.opendata.aws/modis-astraea/
+[copernicus_dem]: https://registry.opendata.aws/copernicus-dem/
 
 **Adding more dataset**:
 
 If you know of another publicly-available dataset that can easily be described
 with a "scene id", please feel free to [open an
 issue](https://github.com/cogeotiff/rio-tiler-pds/issues/new).
 
@@ -115,14 +117,15 @@
 from rio_tiler_pds.sentinel.aws import (
     S2JP2Reader,  # JPEG2000
     S2COGReader,   # COG
 )
 
 from rio_tiler_pds.cbers.aws import CBERSReader
 from rio_tiler_pds.modis.aws import MODISPDSReader, MODISASTRAEAReader
+from rio_tiler_pds.copernicus.aws import Dem30Reader, Dem90Reader
 ```
 
 All Readers are subclass of [`rio_tiler.io.BaseReader`](https://github.com/cogeotiff/rio-tiler/blob/f917d0eaf27f8644f3bb18856a63fe45eeb4a2ef/rio_tiler/io/base.py#L17) and inherit its properties/methods.
 
 #### Properties
 - **bounds**: Scene bounding box
 - **crs**: CRS of the bounding box
@@ -320,14 +323,27 @@
         percentile_98=11227.079999999958
       )}
 
       print(stats["B01"].min)
       >> 2.0
 ```
 
+### Mosaic Reader: Copernicus DEM
+
+The Copernicus DEM GLO-30 and GLO-90 readers are not **per scene** but **mosaic** readers. This is possible because the dataset is a global dataset with file names having the `geo-location` of the COG, meaning we can easily contruct a filepath from a coordinate.
+
+```python
+from rio_tiler_pds.copernicus.aws import Dem30Reader
+
+with Dem30Reader() as dem:
+    print(dem.assets_for_point(-57.2, -11.2))
+
+>> ['s3://copernicus-dem-30m/Copernicus_DSM_COG_10_S12_00_W058_00_DEM/Copernicus_DSM_COG_10_S12_00_W058_00_DEM.tif']
+```
+
 ## Changes
 
 See [CHANGES.md](https://github.com/cogeotiff/rio-tiler-pds/blob/main/CHANGES.md).
 
 ## Contribution & Development
 
 See [CONTRIBUTING.md](https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md)
```

#### html2text {}

```diff
@@ -19,49 +19,53 @@
 L1C | COG (Internal GCPS) | Sinergise / AWS | eu-central-1 | **Requester-pays**
 | | [Landsat Collection 2][landsat_c2_cog] | L1,L2 | COG | USGS / AWS | us-
 west-2 | **Requester-pays** | | [CBERS 4/4A][cbers_cog] | L2/L4 | COG | AMS
 Kepler / AWS | us-east-1 | **Requester-pays** | | [MODIS (modis-pds)]
 [modis_pds] | MCD43A4, MOD09GQ, MYD09GQ, MOD09GA, MYD09GA | GTiff (External
 Overviews) | - | us-west-2 | Public | | [MODIS (astraea-opendata)]
 [modis_astraea] | MCD43A4, MOD11A1, MOD13A1, MYD11A1 MYD13A1 | COG | Astraea /
-AWS | us-west-2 | **Requester-pays** | [s2_l1c_jp2]: https://
-registry.opendata.aws/sentinel-2/ [s2_l2a_jp2]: https://registry.opendata.aws/
-sentinel-2/ [s2_l2a_cog]: https://registry.opendata.aws/sentinel-2-l2a-cogs/
-[s1_l1c_cog]: https://registry.opendata.aws/sentinel-1/ [landsat_c2_cog]:
-https://www.usgs.gov/core-science-systems/nli/landsat/landsat-commercial-cloud-
-data-access [cbers_cog]: https://registry.opendata.aws/cbers/ [modis_pds]:
-https://docs.opendata.aws/modis-pds/readme.html [modis_astraea]: https://
-registry.opendata.aws/modis-astraea/ **Adding more dataset**: If you know of
-another publicly-available dataset that can easily be described with a "scene
-id", please feel free to [open an issue](https://github.com/cogeotiff/rio-
-tiler-pds/issues/new). ## Warnings #### Requester-pays Buckets On AWS,
-`sentinel2`, `sentinel1`, `cbers` and `modis` (in astraea-opendata) datasets
-are stored in [_requester pays_](https://docs.aws.amazon.com/AmazonS3/latest/
-dev/RequesterPaysBuckets.html) buckets. This means that the cost of GET and
-LIST requests and egress fees for downloading files outside the AWS region will
-be charged to the _accessing users_, not the organization hosting the bucket.
-For `rio-tiler` and `rio-tiler-pds` to work with such buckets, you'll need to
-set `AWS_REQUEST_PAYER="requester"` in your shell environment. #### Partial
-reading on Cloud hosted dataset When reading data, `rio-tiler-pds` performs
-_partial_ reads when possible. Hence performance will be best on data stored as
-[Cloud Optimized GeoTIFF (COG)](http://cogeo.org). It's important to note that
+AWS | us-west-2 | **Requester-pays** | | [Copernicus Digital Elevation Model]
+[copernicus_dem] | GLO-30, GLO-90 | COG | Sinergise / AWS | eu-central-1 |
+Public | [s2_l1c_jp2]: https://registry.opendata.aws/sentinel-2/ [s2_l2a_jp2]:
+https://registry.opendata.aws/sentinel-2/ [s2_l2a_cog]: https://
+registry.opendata.aws/sentinel-2-l2a-cogs/ [s1_l1c_cog]: https://
+registry.opendata.aws/sentinel-1/ [landsat_c2_cog]: https://www.usgs.gov/core-
+science-systems/nli/landsat/landsat-commercial-cloud-data-access [cbers_cog]:
+https://registry.opendata.aws/cbers/ [modis_pds]: https://docs.opendata.aws/
+modis-pds/readme.html [modis_astraea]: https://registry.opendata.aws/modis-
+astraea/ [copernicus_dem]: https://registry.opendata.aws/copernicus-dem/
+**Adding more dataset**: If you know of another publicly-available dataset that
+can easily be described with a "scene id", please feel free to [open an issue]
+(https://github.com/cogeotiff/rio-tiler-pds/issues/new). ## Warnings ####
+Requester-pays Buckets On AWS, `sentinel2`, `sentinel1`, `cbers` and `modis`
+(in astraea-opendata) datasets are stored in [_requester pays_](https://
+docs.aws.amazon.com/AmazonS3/latest/dev/RequesterPaysBuckets.html) buckets.
+This means that the cost of GET and LIST requests and egress fees for
+downloading files outside the AWS region will be charged to the _accessing
+users_, not the organization hosting the bucket. For `rio-tiler` and `rio-
+tiler-pds` to work with such buckets, you'll need to set
+`AWS_REQUEST_PAYER="requester"` in your shell environment. #### Partial reading
+on Cloud hosted dataset When reading data, `rio-tiler-pds` performs _partial_
+reads when possible. Hence performance will be best on data stored as [Cloud
+Optimized GeoTIFF (COG)](http://cogeo.org). It's important to note that
 **Sentinel-2 scenes hosted on AWS are not in Cloud Optimized format but in
 JPEG2000**. Partial reads from JPEG2000 files are inefficient, and GDAL (the
 library underlying `rio-tiler-pds` and `rasterio`) will need to make **many GET
 requests** and transfer a lot of data. This will be both slow and expensive,
 since AWS's JPEG2000 collection of Sentinel 2 data is stored in a requester
 pays bucket. Ref: [Do you really want people using your data](https://
 medium.com/@_VincentS_/do-you-really-want-people-using-your-data-ec94cd94dc3f)
 blog post. ## Overview ### Readers Each dataset has its own submodule (e.g
 sentinel2: `rio_tiler_pds.sentinel.aws`) ```python from
 rio_tiler_pds.landsat.aws import LandsatC2Reader from
 rio_tiler_pds.sentinel.aws import S1L1CReader from rio_tiler_pds.sentinel.aws
 import ( S2JP2Reader, # JPEG2000 S2COGReader, # COG ) from
 rio_tiler_pds.cbers.aws import CBERSReader from rio_tiler_pds.modis.aws import
-MODISPDSReader, MODISASTRAEAReader ``` All Readers are subclass of
+MODISPDSReader, MODISASTRAEAReader from rio_tiler_pds.copernicus.aws import
+Dem30Reader, Dem90Reader ``` All Readers are subclass of
 [`rio_tiler.io.BaseReader`](https://github.com/cogeotiff/rio-tiler/blob/
 f917d0eaf27f8644f3bb18856a63fe45eeb4a2ef/rio_tiler/io/base.py#L17) and inherit
 its properties/methods. #### Properties - **bounds**: Scene bounding box -
 **crs**: CRS of the bounding box - **geographic_bounds**: bounding box in
 geographic projection (e.g WGS84) - **minzoom**: WebMercator MinZoom (e.g 7 for
 Landsat 8) - **maxzoom**: WebMercator MaxZoom (e.g 12 for Landsat 8) ####
 Methods - **info**: Returns band's simple info (e.g nodata, band_descriptions,
@@ -166,14 +170,22 @@
 max=15749.0, mean=1941.2052554560712, count=651247.0, sum=1264204099.0,
 std=3130.545395156859, median=329.0, majority=206.0, minority=11946.0,
 unique=13904.0, histogram=[ [479174.0, 34919.0, 27649.0, 25126.0, 24913.0,
 24119.0, 20223.0, 12097.0, 2872.0, 155.0], [1.0, 1575.8, 3150.6, 4725.4,
 6300.2, 7875.0, 9449.8, 11024.6, 12599.4, 14174.199999999999, 15749.0] ],
 valid_percent=62.11, masked_pixels=397329.0, valid_pixels=651247.0,
 percentile_2=134.0, percentile_98=11227.079999999958 )} print(stats["B01"].min)
->> 2.0 ``` ## Changes See [CHANGES.md](https://github.com/cogeotiff/rio-tiler-
-pds/blob/main/CHANGES.md). ## Contribution & Development See [CONTRIBUTING.md]
-(https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md) ## License
-See [LICENSE.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/main/
-LICENSE.txt) ## Authors The rio-tiler project was begun at Mapbox and has been
-transferred in January 2019. See [AUTHORS.txt](https://github.com/cogeotiff/
-rio-tiler-pds/blob/main/AUTHORS.txt) for a listing of individual contributors.
+>> 2.0 ``` ### Mosaic Reader: Copernicus DEM The Copernicus DEM GLO-30 and GLO-
+90 readers are not **per scene** but **mosaic** readers. This is possible
+because the dataset is a global dataset with file names having the `geo-
+location` of the COG, meaning we can easily contruct a filepath from a
+coordinate. ```python from rio_tiler_pds.copernicus.aws import Dem30Reader with
+Dem30Reader() as dem: print(dem.assets_for_point(-57.2, -11.2)) >> ['s3://
+copernicus-dem-30m/Copernicus_DSM_COG_10_S12_00_W058_00_DEM/
+Copernicus_DSM_COG_10_S12_00_W058_00_DEM.tif'] ``` ## Changes See [CHANGES.md]
+(https://github.com/cogeotiff/rio-tiler-pds/blob/main/CHANGES.md). ##
+Contribution & Development See [CONTRIBUTING.md](https://github.com/cogeotiff/
+rio-tiler/blob/main/CONTRIBUTING.md) ## License See [LICENSE.txt](https://
+github.com/cogeotiff/rio-tiler-pds/blob/main/LICENSE.txt) ## Authors The rio-
+tiler project was begun at Mapbox and has been transferred in January 2019. See
+[AUTHORS.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/main/AUTHORS.txt)
+for a listing of individual contributors.
```

### Comparing `rio-tiler-pds-0.8.0/pyproject.toml` & `rio_tiler_pds-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = ["rio-tiler>=4.0,<5.0"]
+dependencies = ["rio-tiler>=5.0,<6.0", "boto3"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 dev = ["pre-commit"]
 docs = ["mkdocs", "mkdocs-material", "pygments", "mkapi"]
 
 [project.urls]
```

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/aws/cbers4.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/cbers/aws/cbers4.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/utils.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/cbers/utils.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/aws/landsat_collection2.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/landsat/aws/landsat_collection2.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/utils.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/landsat/utils.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_astraea.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/modis/aws/modis_astraea.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_pds.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/modis/aws/modis_pds.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/modland_grid.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/modis/modland_grid.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/utils.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/modis/utils.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel1.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/aws/sentinel1.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     input: str = attr.ib()
     tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
     minzoom: int = attr.ib(default=8)
     maxzoom: int = attr.ib(default=14)
 
     reader: Type[Reader] = attr.ib(default=Reader)
-    reader_options: Dict = attr.ib(default={"options": {"nodata": 0}})
+    reader_options: Dict = attr.ib(factory=dict)
 
     productInfo: Dict = attr.ib(init=False)
     datageom: Dict = attr.ib(init=False)
 
     _scheme: str = "s3"
     bucket: str = attr.ib(default="sentinel-s1-l1c")
     prefix_pattern: str = attr.ib(
```

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel2.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/aws/sentinel2.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/utils.py` & `rio_tiler_pds-0.9.0/rio_tiler_pds/sentinel/utils.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.8.0/PKG-INFO` & `rio_tiler_pds-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: rio-tiler-pds
-Version: 0.8.0
+Version: 0.9.0
 Summary: Get mercator tile from cloud hosted dataset such as CBERS-4, Sentinel-2, Sentinel-1 and Landsat-8 AWS PDS.
 Keywords: COGEO,Cloud Optimized Geotiff,AWS PDS
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Typing :: Typed
-Requires-Dist: rio-tiler>=4.0,<5.0
+Requires-Dist: rio-tiler>=5.0,<6.0
+Requires-Dist: boto3
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: pygments ; extra == "docs"
 Requires-Dist: mkapi ; extra == "docs"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
@@ -89,23 +90,25 @@
 | [Sentinel 2][s2_l2a_jp2]                  | L2A                                         | JPEG2000                   | Sinergise / AWS            | eu-central-1 | **Requester-pays** |
 | [Sentinel 2][s2_l2a_cog]                  | L2A                                         | COG                        | Digital Earth Africa / AWS | us-west-2    | Public             |
 | [Sentinel 1][s1_l1c_cog]                  | L1C                                         | COG (Internal GCPS)        | Sinergise / AWS            | eu-central-1 | **Requester-pays** |
 | [Landsat Collection 2][landsat_c2_cog]    | L1,L2                                       | COG                        | USGS / AWS                 | us-west-2    | **Requester-pays** |
 | [CBERS 4/4A][cbers_cog]                   | L2/L4                                       | COG                        | AMS Kepler / AWS           | us-east-1    | **Requester-pays** |
 | [MODIS (modis-pds)][modis_pds]            | MCD43A4, MOD09GQ, MYD09GQ, MOD09GA, MYD09GA | GTiff (External Overviews) | -                          | us-west-2    | Public             |
 | [MODIS (astraea-opendata)][modis_astraea] | MCD43A4, MOD11A1, MOD13A1, MYD11A1 MYD13A1  | COG                        | Astraea / AWS              | us-west-2    | **Requester-pays** |
+| [Copernicus Digital Elevation Model][copernicus_dem] | GLO-30, GLO-90                   | COG                        | Sinergise / AWS            | eu-central-1    | Public |
 
 [s2_l1c_jp2]: https://registry.opendata.aws/sentinel-2/
 [s2_l2a_jp2]: https://registry.opendata.aws/sentinel-2/
 [s2_l2a_cog]: https://registry.opendata.aws/sentinel-2-l2a-cogs/
 [s1_l1c_cog]: https://registry.opendata.aws/sentinel-1/
 [landsat_c2_cog]: https://www.usgs.gov/core-science-systems/nli/landsat/landsat-commercial-cloud-data-access
 [cbers_cog]: https://registry.opendata.aws/cbers/
 [modis_pds]: https://docs.opendata.aws/modis-pds/readme.html
 [modis_astraea]: https://registry.opendata.aws/modis-astraea/
+[copernicus_dem]: https://registry.opendata.aws/copernicus-dem/
 
 **Adding more dataset**:
 
 If you know of another publicly-available dataset that can easily be described
 with a "scene id", please feel free to [open an
 issue](https://github.com/cogeotiff/rio-tiler-pds/issues/new).
 
@@ -146,14 +149,15 @@
 from rio_tiler_pds.sentinel.aws import (
     S2JP2Reader,  # JPEG2000
     S2COGReader,   # COG
 )
 
 from rio_tiler_pds.cbers.aws import CBERSReader
 from rio_tiler_pds.modis.aws import MODISPDSReader, MODISASTRAEAReader
+from rio_tiler_pds.copernicus.aws import Dem30Reader, Dem90Reader
 ```
 
 All Readers are subclass of [`rio_tiler.io.BaseReader`](https://github.com/cogeotiff/rio-tiler/blob/f917d0eaf27f8644f3bb18856a63fe45eeb4a2ef/rio_tiler/io/base.py#L17) and inherit its properties/methods.
 
 #### Properties
 - **bounds**: Scene bounding box
 - **crs**: CRS of the bounding box
@@ -351,14 +355,27 @@
         percentile_98=11227.079999999958
       )}
 
       print(stats["B01"].min)
       >> 2.0
 ```
 
+### Mosaic Reader: Copernicus DEM
+
+The Copernicus DEM GLO-30 and GLO-90 readers are not **per scene** but **mosaic** readers. This is possible because the dataset is a global dataset with file names having the `geo-location` of the COG, meaning we can easily contruct a filepath from a coordinate.
+
+```python
+from rio_tiler_pds.copernicus.aws import Dem30Reader
+
+with Dem30Reader() as dem:
+    print(dem.assets_for_point(-57.2, -11.2))
+
+>> ['s3://copernicus-dem-30m/Copernicus_DSM_COG_10_S12_00_W058_00_DEM/Copernicus_DSM_COG_10_S12_00_W058_00_DEM.tif']
+```
+
 ## Changes
 
 See [CHANGES.md](https://github.com/cogeotiff/rio-tiler-pds/blob/main/CHANGES.md).
 
 ## Contribution & Development
 
 See [CONTRIBUTING.md](https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md)
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: rio-tiler-pds Version: 0.8.0 Summary: Get mercator
+Metadata-Version: 2.1 Name: rio-tiler-pds Version: 0.9.0 Summary: Get mercator
 tile from cloud hosted dataset such as CBERS-4, Sentinel-2, Sentinel-1 and
 Landsat-8 AWS PDS. Keywords: COGEO,Cloud Optimized Geotiff,AWS PDS Author-
 email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: Typing :: Typed Requires-
-Dist: rio-tiler>=4.0,<5.0 Requires-Dist: pre-commit ; extra == "dev" Requires-
-Dist: mkdocs ; extra == "docs" Requires-Dist: mkdocs-material ; extra == "docs"
-Requires-Dist: pygments ; extra == "docs" Requires-Dist: mkapi ; extra ==
-"docs" Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-cov ;
-extra == "test" Project-URL: Documentation, https://cogeotiff.github.io/rio-
-tiler-pds/ Project-URL: Source, https://github.com/cogeotiff/rio-tiler-pds
-Provides-Extra: dev Provides-Extra: docs Provides-Extra: test # Rio-Tiler-PDS:
-A rio-tiler plugin for Public Datasets
+Dist: rio-tiler>=5.0,<6.0 Requires-Dist: boto3 Requires-Dist: pre-commit ;
+extra == "dev" Requires-Dist: mkdocs ; extra == "docs" Requires-Dist: mkdocs-
+material ; extra == "docs" Requires-Dist: pygments ; extra == "docs" Requires-
+Dist: mkapi ; extra == "docs" Requires-Dist: pytest ; extra == "test" Requires-
+Dist: pytest-cov ; extra == "test" Project-URL: Documentation, https://
+cogeotiff.github.io/rio-tiler-pds/ Project-URL: Source, https://github.com/
+cogeotiff/rio-tiler-pds Provides-Extra: dev Provides-Extra: docs Provides-
+Extra: test # Rio-Tiler-PDS: A rio-tiler plugin for Public Datasets
                                 [rio-tiler-pds]
          A rio-tiler plugin to read from publicly-available datasets.
           [Test] [Coverage] [Package_version] [Downloads] [Lincense]
 **Important** This is the new module for rio-tiler missions specific (ref:
 https://github.com/cogeotiff/rio-tiler/issues/195) --- **Documentation**:
 https://cogeotiff.github.io/rio-tiler-pds/ **Source Code**: https://github.com/
 cogeotiff/rio-tiler-pds --- ## Installation You can install rio-tiler-pds using
@@ -37,49 +37,53 @@
 L1C | COG (Internal GCPS) | Sinergise / AWS | eu-central-1 | **Requester-pays**
 | | [Landsat Collection 2][landsat_c2_cog] | L1,L2 | COG | USGS / AWS | us-
 west-2 | **Requester-pays** | | [CBERS 4/4A][cbers_cog] | L2/L4 | COG | AMS
 Kepler / AWS | us-east-1 | **Requester-pays** | | [MODIS (modis-pds)]
 [modis_pds] | MCD43A4, MOD09GQ, MYD09GQ, MOD09GA, MYD09GA | GTiff (External
 Overviews) | - | us-west-2 | Public | | [MODIS (astraea-opendata)]
 [modis_astraea] | MCD43A4, MOD11A1, MOD13A1, MYD11A1 MYD13A1 | COG | Astraea /
-AWS | us-west-2 | **Requester-pays** | [s2_l1c_jp2]: https://
-registry.opendata.aws/sentinel-2/ [s2_l2a_jp2]: https://registry.opendata.aws/
-sentinel-2/ [s2_l2a_cog]: https://registry.opendata.aws/sentinel-2-l2a-cogs/
-[s1_l1c_cog]: https://registry.opendata.aws/sentinel-1/ [landsat_c2_cog]:
-https://www.usgs.gov/core-science-systems/nli/landsat/landsat-commercial-cloud-
-data-access [cbers_cog]: https://registry.opendata.aws/cbers/ [modis_pds]:
-https://docs.opendata.aws/modis-pds/readme.html [modis_astraea]: https://
-registry.opendata.aws/modis-astraea/ **Adding more dataset**: If you know of
-another publicly-available dataset that can easily be described with a "scene
-id", please feel free to [open an issue](https://github.com/cogeotiff/rio-
-tiler-pds/issues/new). ## Warnings #### Requester-pays Buckets On AWS,
-`sentinel2`, `sentinel1`, `cbers` and `modis` (in astraea-opendata) datasets
-are stored in [_requester pays_](https://docs.aws.amazon.com/AmazonS3/latest/
-dev/RequesterPaysBuckets.html) buckets. This means that the cost of GET and
-LIST requests and egress fees for downloading files outside the AWS region will
-be charged to the _accessing users_, not the organization hosting the bucket.
-For `rio-tiler` and `rio-tiler-pds` to work with such buckets, you'll need to
-set `AWS_REQUEST_PAYER="requester"` in your shell environment. #### Partial
-reading on Cloud hosted dataset When reading data, `rio-tiler-pds` performs
-_partial_ reads when possible. Hence performance will be best on data stored as
-[Cloud Optimized GeoTIFF (COG)](http://cogeo.org). It's important to note that
+AWS | us-west-2 | **Requester-pays** | | [Copernicus Digital Elevation Model]
+[copernicus_dem] | GLO-30, GLO-90 | COG | Sinergise / AWS | eu-central-1 |
+Public | [s2_l1c_jp2]: https://registry.opendata.aws/sentinel-2/ [s2_l2a_jp2]:
+https://registry.opendata.aws/sentinel-2/ [s2_l2a_cog]: https://
+registry.opendata.aws/sentinel-2-l2a-cogs/ [s1_l1c_cog]: https://
+registry.opendata.aws/sentinel-1/ [landsat_c2_cog]: https://www.usgs.gov/core-
+science-systems/nli/landsat/landsat-commercial-cloud-data-access [cbers_cog]:
+https://registry.opendata.aws/cbers/ [modis_pds]: https://docs.opendata.aws/
+modis-pds/readme.html [modis_astraea]: https://registry.opendata.aws/modis-
+astraea/ [copernicus_dem]: https://registry.opendata.aws/copernicus-dem/
+**Adding more dataset**: If you know of another publicly-available dataset that
+can easily be described with a "scene id", please feel free to [open an issue]
+(https://github.com/cogeotiff/rio-tiler-pds/issues/new). ## Warnings ####
+Requester-pays Buckets On AWS, `sentinel2`, `sentinel1`, `cbers` and `modis`
+(in astraea-opendata) datasets are stored in [_requester pays_](https://
+docs.aws.amazon.com/AmazonS3/latest/dev/RequesterPaysBuckets.html) buckets.
+This means that the cost of GET and LIST requests and egress fees for
+downloading files outside the AWS region will be charged to the _accessing
+users_, not the organization hosting the bucket. For `rio-tiler` and `rio-
+tiler-pds` to work with such buckets, you'll need to set
+`AWS_REQUEST_PAYER="requester"` in your shell environment. #### Partial reading
+on Cloud hosted dataset When reading data, `rio-tiler-pds` performs _partial_
+reads when possible. Hence performance will be best on data stored as [Cloud
+Optimized GeoTIFF (COG)](http://cogeo.org). It's important to note that
 **Sentinel-2 scenes hosted on AWS are not in Cloud Optimized format but in
 JPEG2000**. Partial reads from JPEG2000 files are inefficient, and GDAL (the
 library underlying `rio-tiler-pds` and `rasterio`) will need to make **many GET
 requests** and transfer a lot of data. This will be both slow and expensive,
 since AWS's JPEG2000 collection of Sentinel 2 data is stored in a requester
 pays bucket. Ref: [Do you really want people using your data](https://
 medium.com/@_VincentS_/do-you-really-want-people-using-your-data-ec94cd94dc3f)
 blog post. ## Overview ### Readers Each dataset has its own submodule (e.g
 sentinel2: `rio_tiler_pds.sentinel.aws`) ```python from
 rio_tiler_pds.landsat.aws import LandsatC2Reader from
 rio_tiler_pds.sentinel.aws import S1L1CReader from rio_tiler_pds.sentinel.aws
 import ( S2JP2Reader, # JPEG2000 S2COGReader, # COG ) from
 rio_tiler_pds.cbers.aws import CBERSReader from rio_tiler_pds.modis.aws import
-MODISPDSReader, MODISASTRAEAReader ``` All Readers are subclass of
+MODISPDSReader, MODISASTRAEAReader from rio_tiler_pds.copernicus.aws import
+Dem30Reader, Dem90Reader ``` All Readers are subclass of
 [`rio_tiler.io.BaseReader`](https://github.com/cogeotiff/rio-tiler/blob/
 f917d0eaf27f8644f3bb18856a63fe45eeb4a2ef/rio_tiler/io/base.py#L17) and inherit
 its properties/methods. #### Properties - **bounds**: Scene bounding box -
 **crs**: CRS of the bounding box - **geographic_bounds**: bounding box in
 geographic projection (e.g WGS84) - **minzoom**: WebMercator MinZoom (e.g 7 for
 Landsat 8) - **maxzoom**: WebMercator MaxZoom (e.g 12 for Landsat 8) ####
 Methods - **info**: Returns band's simple info (e.g nodata, band_descriptions,
@@ -184,14 +188,22 @@
 max=15749.0, mean=1941.2052554560712, count=651247.0, sum=1264204099.0,
 std=3130.545395156859, median=329.0, majority=206.0, minority=11946.0,
 unique=13904.0, histogram=[ [479174.0, 34919.0, 27649.0, 25126.0, 24913.0,
 24119.0, 20223.0, 12097.0, 2872.0, 155.0], [1.0, 1575.8, 3150.6, 4725.4,
 6300.2, 7875.0, 9449.8, 11024.6, 12599.4, 14174.199999999999, 15749.0] ],
 valid_percent=62.11, masked_pixels=397329.0, valid_pixels=651247.0,
 percentile_2=134.0, percentile_98=11227.079999999958 )} print(stats["B01"].min)
->> 2.0 ``` ## Changes See [CHANGES.md](https://github.com/cogeotiff/rio-tiler-
-pds/blob/main/CHANGES.md). ## Contribution & Development See [CONTRIBUTING.md]
-(https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md) ## License
-See [LICENSE.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/main/
-LICENSE.txt) ## Authors The rio-tiler project was begun at Mapbox and has been
-transferred in January 2019. See [AUTHORS.txt](https://github.com/cogeotiff/
-rio-tiler-pds/blob/main/AUTHORS.txt) for a listing of individual contributors.
+>> 2.0 ``` ### Mosaic Reader: Copernicus DEM The Copernicus DEM GLO-30 and GLO-
+90 readers are not **per scene** but **mosaic** readers. This is possible
+because the dataset is a global dataset with file names having the `geo-
+location` of the COG, meaning we can easily contruct a filepath from a
+coordinate. ```python from rio_tiler_pds.copernicus.aws import Dem30Reader with
+Dem30Reader() as dem: print(dem.assets_for_point(-57.2, -11.2)) >> ['s3://
+copernicus-dem-30m/Copernicus_DSM_COG_10_S12_00_W058_00_DEM/
+Copernicus_DSM_COG_10_S12_00_W058_00_DEM.tif'] ``` ## Changes See [CHANGES.md]
+(https://github.com/cogeotiff/rio-tiler-pds/blob/main/CHANGES.md). ##
+Contribution & Development See [CONTRIBUTING.md](https://github.com/cogeotiff/
+rio-tiler/blob/main/CONTRIBUTING.md) ## License See [LICENSE.txt](https://
+github.com/cogeotiff/rio-tiler-pds/blob/main/LICENSE.txt) ## Authors The rio-
+tiler project was begun at Mapbox and has been transferred in January 2019. See
+[AUTHORS.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/main/AUTHORS.txt)
+for a listing of individual contributors.
```

