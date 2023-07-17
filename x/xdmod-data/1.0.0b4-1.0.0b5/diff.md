# Comparing `tmp/xdmod_data-1.0.0b4-py3-none-any.whl.zip` & `tmp/xdmod_data-1.0.0b5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 16265 bytes, number of entries: 13
+Zip file size: 16937 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       37 b- defN 23-Jul-11 14:04 xdmod_data/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-12 18:50 xdmod_data/__version__.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-17 17:44 xdmod_data/__version__.py
 -rw-r--r--  2.0 unx     2262 b- defN 23-Jul-11 14:04 xdmod_data/_descriptors.py
 -rw-r--r--  2.0 unx     5230 b- defN 23-Jul-11 14:04 xdmod_data/_http_requester.py
 -rw-r--r--  2.0 unx     4435 b- defN 23-Jul-11 14:04 xdmod_data/_response_processor.py
 -rw-r--r--  2.0 unx    10394 b- defN 23-Jul-11 14:04 xdmod_data/_validator.py
 -rw-r--r--  2.0 unx     3018 b- defN 23-Jul-11 14:04 xdmod_data/themes.py
--rw-r--r--  2.0 unx    16931 b- defN 23-Jul-11 14:04 xdmod_data/warehouse.py
--rw-r--r--  2.0 unx     7652 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3801 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1067 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/RECORD
-13 files, 54984 bytes uncompressed, 14483 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx    19175 b- defN 23-Jul-17 17:41 xdmod_data/warehouse.py
+-rw-r--r--  2.0 unx     7652 b- defN 23-Jul-17 17:52 xdmod_data-1.0.0b5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3824 b- defN 23-Jul-17 17:52 xdmod_data-1.0.0b5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 17:52 xdmod_data-1.0.0b5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-17 17:52 xdmod_data-1.0.0b5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Jul-17 17:52 xdmod_data-1.0.0b5.dist-info/RECORD
+13 files, 57251 bytes uncompressed, 15155 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: xdmod_data/themes.py
 Comment: 
 
 Filename: xdmod_data/warehouse.py
 Comment: 
 
-Filename: xdmod_data-1.0.0b4.dist-info/LICENSE
+Filename: xdmod_data-1.0.0b5.dist-info/LICENSE
 Comment: 
 
-Filename: xdmod_data-1.0.0b4.dist-info/METADATA
+Filename: xdmod_data-1.0.0b5.dist-info/METADATA
 Comment: 
 
-Filename: xdmod_data-1.0.0b4.dist-info/WHEEL
+Filename: xdmod_data-1.0.0b5.dist-info/WHEEL
 Comment: 
 
-Filename: xdmod_data-1.0.0b4.dist-info/top_level.txt
+Filename: xdmod_data-1.0.0b5.dist-info/top_level.txt
 Comment: 
 
-Filename: xdmod_data-1.0.0b4.dist-info/RECORD
+Filename: xdmod_data-1.0.0b5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xdmod_data/__version__.py

```diff
@@ -1,2 +1,2 @@
 __title__ = 'xdmod-data'
-__version__ = '1.0.0-beta.4'
+__version__ = '1.0.0-beta.5'
```

## xdmod_data/warehouse.py

```diff
@@ -398,14 +398,72 @@
         realm_id = _validator._find_raw_realm_id(self.__descriptors, realm)
         return self.__get_data_frame_from_descriptor(
             self.__descriptors._get_raw()[realm_id]['fields'],
             ('id', 'label', 'description'),
             'id',
         )
 
+    def compliance(self, timeframe):
+        response = self.__http_requester._request_json(
+            '/controllers/compliance.php',
+            {'timeframe_mode': timeframe},
+        )
+        return response
+
+    def resources(self):
+        names = []
+        types = []
+        resource_ids = []
+        cdata = self.compliance('to_date')
+        for resource in cdata['metaData']['fields']:
+            if resource['name'] == 'requirement':
+                continue
+            names.append(
+                resource['header'][:-7].split('>')[1].replace('-', ' ')
+            )
+            types.append(resource['status'].split('|')[0].strip())
+            resource_ids.append(resource['resource_id'])
+        return pd.Series(data=types, index=names)
+
+    def get_qualitydata(self, params, is_numpy=False):
+        type_to_title = {
+            'gpu': '% of jobs with GPU information',
+            'hardware': '% of jobs with hardware perf information',
+            'cpu': '% of jobs with cpu usage information',
+            'script': '% of jobs with Job Batch Script information',
+            'realms': '% of jobs in the SUPReMM realm compared to Jobs realm',
+        }
+        response = self.__http_requester._request_json(
+            '/rest/supremm_dataflow/quality',
+            params,
+        )
+        if response['success']:
+            result = response['result']
+            jobs = [job for job in result]
+            dates = [
+                date.strftime('%Y-%m-%d') for date in pd.date_range(
+                    params['start'],
+                    params['end'],
+                    freq='D',
+                ).date
+            ]
+            quality = np.empty((len(jobs), len(dates)))
+            for i in range(len(jobs)):
+                for j in range(len(dates)):
+                    job_i = result[jobs[i]]
+                    if job_i.get(dates[j], np.nan) != 'N/A':
+                        quality[i, j] = job_i.get(dates[j], np.nan)
+                    else:
+                        quality[i, j] = np.nan
+            if is_numpy:
+                return quality
+            df = pd.DataFrame(data=quality, index=jobs, columns=dates)
+            df.name = type_to_title[params['type']]
+            return df
+
     def _get_metric_label(self, realm, metric_id):
         d = self.__descriptors._get_aggregate()
         return d[realm]['metrics'][metric_id]['label']
 
     def _get_dimension_label(self, realm, dimension_id):
         if dimension_id == 'none':
             return None
```

## Comparing `xdmod_data-1.0.0b4.dist-info/LICENSE` & `xdmod_data-1.0.0b5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xdmod_data-1.0.0b4.dist-info/METADATA` & `xdmod_data-1.0.0b5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdmod-data
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Python package for XDMoD data access
 Author: Aaron Weeden, Joseph P. White
 Maintainer: Aaron Weeden, Joseph P. White
 Project-URL: Source Code, https://github.com/ubccr/xdmod-data
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -51,17 +51,18 @@
 
     ![Screenshot of "Copy API Token to Clipboard" button](https://raw.githubusercontent.com/ubccr/xdmod-data/main/docs/images/api-token/copy.jpg)
 
     **Note:** If you lose your token, simply delete it and generate a new one.
 
 ## Support
 For support, please see [this page](https://open.xdmod.org/support.html). If you email for support, please include the following:
-* `xdmod-data` version number, obtained by running the command:
+* `xdmod-data` version number, obtained by running this Python code:
     ```
-    python3 -m pip freeze | grep xdmod-data
+    from xdmod_data import __version__
+    print(__version__)
     ```
 * Operating system version.
 * A description of the problem you are experiencing.
 * Detailed steps to reproduce the problem.
 
 ## License
 `xdmod-data` is released under the GNU Lesser General Public License ("LGPL") Version 3.0. See the [LICENSE](LICENSE) file for details.
```

## Comparing `xdmod_data-1.0.0b4.dist-info/RECORD` & `xdmod_data-1.0.0b5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 xdmod_data/__init__.py,sha256=e3S0EcDGJlWIp2hddSFjvt633jfeZ4W7VyAeLpfTWVM,37
-xdmod_data/__version__.py,sha256=mtscD2fli52hysFpfP78r-oPIMOIc7UJF4-dBuA062Y,54
+xdmod_data/__version__.py,sha256=jDYQ7nLb6SKQ51PV5S_KvuVbLw1xG47RXF6_3dVctUo,54
 xdmod_data/_descriptors.py,sha256=uUbC65oW5Vur-DhFEs__NrYTpCt5FrngTYVgu08FgwE,2262
 xdmod_data/_http_requester.py,sha256=7936UGqjrKrW4vY0bEsONRx0CYfPQojr-YEVieEkosg,5230
 xdmod_data/_response_processor.py,sha256=Vslz3-DtlhhoukJ11yJWcLi0wIcZSCIHMLlETzA9WEU,4435
 xdmod_data/_validator.py,sha256=GWHH_U5r_QVcZG9C_yo1xMGoxIFXmC__5l94-hqLcPE,10394
 xdmod_data/themes.py,sha256=eSD7_dJsFhiB3qrMW7FP54IFPXh9tr1XjHXIB6nvx-c,3018
-xdmod_data/warehouse.py,sha256=W7vMIAp_BiKEa15oipiRfZRmVBTfShqie4hFuj6TMdQ,16931
-xdmod_data-1.0.0b4.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
-xdmod_data-1.0.0b4.dist-info/METADATA,sha256=wdrB_MtdxlWLtoaBDnJrcOcotH1L5qvy3TDPrVOESEo,3801
-xdmod_data-1.0.0b4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-xdmod_data-1.0.0b4.dist-info/top_level.txt,sha256=ph-NOi5tK19CfM5XnNOGuId1orUYaKQPxOPiS-geLPk,11
-xdmod_data-1.0.0b4.dist-info/RECORD,,
+xdmod_data/warehouse.py,sha256=Glz9LY2baii3DEpe1nOlyTYTMTordLdy4rVM2ddwMKM,19175
+xdmod_data-1.0.0b5.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
+xdmod_data-1.0.0b5.dist-info/METADATA,sha256=KHjOx8dOLD4ox6vxsY0CrwYN2oJsXa7YlTFemu5Knzo,3824
+xdmod_data-1.0.0b5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+xdmod_data-1.0.0b5.dist-info/top_level.txt,sha256=ph-NOi5tK19CfM5XnNOGuId1orUYaKQPxOPiS-geLPk,11
+xdmod_data-1.0.0b5.dist-info/RECORD,,
```

