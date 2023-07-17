# Comparing `tmp/ptvulnsearcher-0.0.1.tar.gz` & `tmp/ptvulnsearcher-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptvulnsearcher-0.0.1.tar", last modified: Tue May 24 11:35:13 2022, max compression
+gzip compressed data, was "ptvulnsearcher-0.0.2.tar", last modified: Mon Jul 17 16:49:01 2023, max compression
```

## Comparing `ptvulnsearcher-0.0.1.tar` & `ptvulnsearcher-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-05-24 11:35:13.246702 ptvulnsearcher-0.0.1/
--rwxrw-rw-   0 kali      (1000) kali      (1000)    35149 2021-12-17 14:07:29.000000 ptvulnsearcher-0.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     2705 2022-05-24 11:35:13.246702 ptvulnsearcher-0.0.1/PKG-INFO
--rwxrw-rw-   0 kali      (1000) kali      (1000)     2233 2022-05-24 11:25:14.000000 ptvulnsearcher-0.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-05-24 11:35:13.242741 ptvulnsearcher-0.0.1/ptvulnsearcher/
--rwxrw-rw-   0 kali      (1000) kali      (1000)        0 2021-12-17 14:07:29.000000 ptvulnsearcher-0.0.1/ptvulnsearcher/__init__.py
--rwxrw-rw-   0 kali      (1000) kali      (1000)     3855 2022-05-22 17:05:40.000000 ptvulnsearcher-0.0.1/ptvulnsearcher/ptvulnsearcher.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-05-24 11:35:13.246702 ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2705 2022-05-24 11:35:12.000000 ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      326 2022-05-24 11:35:12.000000 ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-05-24 11:35:12.000000 ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       70 2022-05-24 11:35:12.000000 ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2022-05-24 11:35:12.000000 ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2022-05-24 11:35:12.000000 ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/top_level.txt
--rwxrw-rw-   0 kali      (1000) kali      (1000)       38 2022-05-24 11:35:13.246702 ptvulnsearcher-0.0.1/setup.cfg
--rwxrw-rw-   0 kali      (1000) kali      (1000)      880 2022-05-24 11:33:39.000000 ptvulnsearcher-0.0.1/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 16:49:01.307324 ptvulnsearcher-0.0.2/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    35149 2023-07-16 15:42:49.000000 ptvulnsearcher-0.0.2/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3323 2023-07-17 16:49:01.307324 ptvulnsearcher-0.0.2/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2734 2023-07-17 16:45:50.000000 ptvulnsearcher-0.0.2/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 16:49:01.307324 ptvulnsearcher-0.0.2/ptvulnsearcher/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-07-16 15:54:24.000000 ptvulnsearcher-0.0.2/ptvulnsearcher/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-07-17 16:29:28.000000 ptvulnsearcher-0.0.2/ptvulnsearcher/_version.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6258 2023-07-17 16:30:25.000000 ptvulnsearcher-0.0.2/ptvulnsearcher/ptvulnsearcher.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 16:49:01.307324 ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3323 2023-07-17 16:49:01.000000 ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      343 2023-07-17 16:49:01.000000 ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-17 16:49:01.000000 ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       70 2023-07-17 16:49:01.000000 ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       22 2023-07-17 16:49:01.000000 ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-07-17 16:49:01.000000 ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-17 16:49:01.307324 ptvulnsearcher-0.0.2/setup.cfg
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)     1064 2023-07-17 16:48:30.000000 ptvulnsearcher-0.0.2/setup.py
```

### Comparing `ptvulnsearcher-0.0.1/LICENSE` & `ptvulnsearcher-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptvulnsearcher-0.0.1/PKG-INFO` & `ptvulnsearcher-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ptvulnsearcher
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool for searching CVE (Common Vulnerabilities and Exposures)
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
 # PTVULNSEARCHER
 > Common Vulnerabilities and Exposures Searcher
 
 ptvulnsearcher is a tool for searching CVE (Common Vulnerabilities and Exposures). This tool allows searching using keywords or exact CVE.
 
@@ -26,65 +27,73 @@
 
 ```
 pip install ptvulnsearcher
 ```
 
 ### Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
 ## Usage examples
 
 ```
-ptvulnsearcher -s "Apache Tomcat"             # Search CVE for the specified string
-ptvulnsearcher -cve CVE-2022-29885            # Search specified CVE
+ptvulnsearcher -cve CVE-2022-29885            
+ptvulnsearcher -vn Redhat                     
+ptvulnsearcher -pn linux                      
+ptvulnsearcher -vn Redhat -pn linux           
+ptvulnsearcher -vn Redhat -pn linux -pv 9.0   
+ptvulnsearcher -pn linux -pv 9.0              
 ```
 
 ## Options
 ```
-   -s   --search              <search>        Search keywords
-   -cve --cve                 <cve>           Search for specific CVE
-   -j   --json                                Output in JSON format
-   -v   --version                             Show script version and exit
-   -h   --help                                Show this help message and exit
+   -cve  --cve              <CVE ID>            Search based on CVE
+   -vn   --vendor_name      <vendor_name>       Search based on vendor
+   -pn   --product_name     <product_name>      Search based on product
+   -pv   --product_version  <product_version>   Search based on product version
+   -j    --json                                 Output in JSON format
+   -v    --version                              Show script version and exit
+   -h    --help                                 Show this help message and exit
 ```
 
 ## Dependencies
 ```
-- requests
-- ptlibs
+requests
+ptlibs
 ```
 
-
 ## Version History
 ```
-0.0.1 - initial release
+0.0.2
+    - New options
+0.0.1
+    - Alpha releases
 ```
-
 ## License
 
-Copyright (c) 2022 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
+
+ptvulnsearcher is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
-ptinsearcher is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-ptinsearcher is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
+ptvulnsearcher is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with ptvulnsearcher. If not, see https://www.gnu.org/licenses/.
 
-You should have received a copy of the GNU General Public License
-along with ptinsearcher.  If not, see <https://www.gnu.org/licenses/>.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptvulnsearcher-0.0.1/README.md` & `ptvulnsearcher-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
 # PTVULNSEARCHER
 > Common Vulnerabilities and Exposures Searcher
 
 ptvulnsearcher is a tool for searching CVE (Common Vulnerabilities and Exposures). This tool allows searching using keywords or exact CVE.
 
@@ -10,64 +10,73 @@
 
 ```
 pip install ptvulnsearcher
 ```
 
 ### Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
 ## Usage examples
 
 ```
-ptvulnsearcher -s "Apache Tomcat"             # Search CVE for the specified string
-ptvulnsearcher -cve CVE-2022-29885            # Search specified CVE
+ptvulnsearcher -cve CVE-2022-29885            
+ptvulnsearcher -vn Redhat                     
+ptvulnsearcher -pn linux                      
+ptvulnsearcher -vn Redhat -pn linux           
+ptvulnsearcher -vn Redhat -pn linux -pv 9.0   
+ptvulnsearcher -pn linux -pv 9.0              
 ```
 
 ## Options
 ```
-   -s   --search              <search>        Search keywords
-   -cve --cve                 <cve>           Search for specific CVE
-   -j   --json                                Output in JSON format
-   -v   --version                             Show script version and exit
-   -h   --help                                Show this help message and exit
+   -cve  --cve              <CVE ID>            Search based on CVE
+   -vn   --vendor_name      <vendor_name>       Search based on vendor
+   -pn   --product_name     <product_name>      Search based on product
+   -pv   --product_version  <product_version>   Search based on product version
+   -j    --json                                 Output in JSON format
+   -v    --version                              Show script version and exit
+   -h    --help                                 Show this help message and exit
 ```
 
 ## Dependencies
 ```
-- requests
-- ptlibs
+requests
+ptlibs
 ```
 
-
 ## Version History
 ```
-0.0.1 - initial release
+0.0.2
+    - New options
+0.0.1
+    - Alpha releases
 ```
-
 ## License
 
-Copyright (c) 2022 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
+
+ptvulnsearcher is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+ptvulnsearcher is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-ptinsearcher is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-ptinsearcher is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with ptvulnsearcher. If not, see https://www.gnu.org/licenses/.
 
-You should have received a copy of the GNU General Public License
-along with ptinsearcher.  If not, see <https://www.gnu.org/licenses/>.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
-or malicious use of this code. Be Ethical!
+or malicious use of this code. Be Ethical!
```

### Comparing `ptvulnsearcher-0.0.1/ptvulnsearcher.egg-info/PKG-INFO` & `ptvulnsearcher-0.0.2/ptvulnsearcher.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ptvulnsearcher
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool for searching CVE (Common Vulnerabilities and Exposures)
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
 # PTVULNSEARCHER
 > Common Vulnerabilities and Exposures Searcher
 
 ptvulnsearcher is a tool for searching CVE (Common Vulnerabilities and Exposures). This tool allows searching using keywords or exact CVE.
 
@@ -26,65 +27,73 @@
 
 ```
 pip install ptvulnsearcher
 ```
 
 ### Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
 ## Usage examples
 
 ```
-ptvulnsearcher -s "Apache Tomcat"             # Search CVE for the specified string
-ptvulnsearcher -cve CVE-2022-29885            # Search specified CVE
+ptvulnsearcher -cve CVE-2022-29885            
+ptvulnsearcher -vn Redhat                     
+ptvulnsearcher -pn linux                      
+ptvulnsearcher -vn Redhat -pn linux           
+ptvulnsearcher -vn Redhat -pn linux -pv 9.0   
+ptvulnsearcher -pn linux -pv 9.0              
 ```
 
 ## Options
 ```
-   -s   --search              <search>        Search keywords
-   -cve --cve                 <cve>           Search for specific CVE
-   -j   --json                                Output in JSON format
-   -v   --version                             Show script version and exit
-   -h   --help                                Show this help message and exit
+   -cve  --cve              <CVE ID>            Search based on CVE
+   -vn   --vendor_name      <vendor_name>       Search based on vendor
+   -pn   --product_name     <product_name>      Search based on product
+   -pv   --product_version  <product_version>   Search based on product version
+   -j    --json                                 Output in JSON format
+   -v    --version                              Show script version and exit
+   -h    --help                                 Show this help message and exit
 ```
 
 ## Dependencies
 ```
-- requests
-- ptlibs
+requests
+ptlibs
 ```
 
-
 ## Version History
 ```
-0.0.1 - initial release
+0.0.2
+    - New options
+0.0.1
+    - Alpha releases
 ```
-
 ## License
 
-Copyright (c) 2022 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
+
+ptvulnsearcher is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
-ptinsearcher is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-ptinsearcher is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
+ptvulnsearcher is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with ptvulnsearcher. If not, see https://www.gnu.org/licenses/.
 
-You should have received a copy of the GNU General Public License
-along with ptinsearcher.  If not, see <https://www.gnu.org/licenses/>.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptvulnsearcher-0.0.1/setup.py` & `ptvulnsearcher-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import setuptools
+from ptvulnsearcher._version import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ptvulnsearcher",
     description="Tool for searching CVE (Common Vulnerabilities and Exposures)",
-    version="0.0.1",
-    url="https://www.penterep.com/",
+    version=__version__,
     author="Penterep",
     author_email="info@penterep.com",
+    url="https://www.penterep.com/",
     license="GPLv3+",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Environment :: Console"
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Environment :: Console",
+        "Topic :: Security",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
     ],
     python_requires='>=3.6',
-    install_requires=["ptlibs", "requests"],
-    entry_points={'console_scripts': [
-        'ptvulnsearcher = ptvulnsearcher.ptvulnsearcher:main']},
+    install_requires=["ptlibs>=1,<2", "requests"],
+    entry_points={'console_scripts': ['ptvulnsearcher = ptvulnsearcher.ptvulnsearcher:main']},
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
-)
+)
```

