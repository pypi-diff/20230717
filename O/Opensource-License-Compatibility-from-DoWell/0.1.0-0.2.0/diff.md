# Comparing `tmp/Opensource License Compatibility from DoWell-0.1.0.tar.gz` & `tmp/Opensource License Compatibility from DoWell-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Opensource License Compatibility from DoWell-0.1.0.tar", last modified: Mon Jul 17 16:19:57 2023, max compression
+gzip compressed data, was "Opensource License Compatibility from DoWell-0.2.0.tar", last modified: Mon Jul 17 16:30:10 2023, max compression
```

## Comparing `Opensource License Compatibility from DoWell-0.1.0.tar` & `Opensource License Compatibility from DoWell-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:57.924832 Opensource License Compatibility from DoWell-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:57.911254 Opensource License Compatibility from DoWell-0.1.0/Opensource_License_Compatibility_from_DoWell.egg-info/
--rw-rw-rw-   0        0        0    11648 2023-07-17 16:19:57.000000 Opensource License Compatibility from DoWell-0.1.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-07-17 16:19:57.000000 Opensource License Compatibility from DoWell-0.1.0/Opensource_License_Compatibility_from_DoWell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 16:19:57.000000 Opensource License Compatibility from DoWell-0.1.0/Opensource_License_Compatibility_from_DoWell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 16:19:57.000000 Opensource License Compatibility from DoWell-0.1.0/Opensource_License_Compatibility_from_DoWell.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-07-17 16:19:57.000000 Opensource License Compatibility from DoWell-0.1.0/Opensource_License_Compatibility_from_DoWell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11648 2023-07-17 16:19:57.923569 Opensource License Compatibility from DoWell-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    11168 2023-07-17 16:18:38.000000 Opensource License Compatibility from DoWell-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:57.919515 Opensource License Compatibility from DoWell-0.1.0/doWellOpensourceLicenseCompatibility/
--rw-rw-rw-   0        0        0       86 2023-07-17 16:16:50.000000 Opensource License Compatibility from DoWell-0.1.0/doWellOpensourceLicenseCompatibility/__init__.py
--rw-rw-rw-   0        0        0     5274 2023-07-17 16:16:38.000000 Opensource License Compatibility from DoWell-0.1.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py
--rw-rw-rw-   0        0        0       42 2023-07-17 16:19:57.925845 Opensource License Compatibility from DoWell-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-07-17 16:13:25.000000 Opensource License Compatibility from DoWell-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:30:10.721293 Opensource License Compatibility from DoWell-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-07-17 16:30:10.707117 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/
+-rw-rw-rw-   0        0        0    10657 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10657 2023-07-17 16:30:10.720298 Opensource License Compatibility from DoWell-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10152 2023-07-17 16:29:28.000000 Opensource License Compatibility from DoWell-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 16:30:10.712254 Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/
+-rw-rw-rw-   0        0        0       86 2023-07-17 16:16:50.000000 Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/__init__.py
+-rw-rw-rw-   0        0        0     5274 2023-07-17 16:16:38.000000 Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 16:30:10.722345 Opensource License Compatibility from DoWell-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      786 2023-07-17 16:28:39.000000 Opensource License Compatibility from DoWell-0.2.0/setup.py
```

### Comparing `Opensource License Compatibility from DoWell-0.1.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO` & `Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Opensource-License-Compatibility-from-DoWell
-Version: 0.1.0
+Version: 0.2.0
 Summary: Opensource License Compatibility from DoWell
-Author: Dennis RK.
-License: MIT
+Author: DoWell UX Living Lab
+License: Apache License 2.0
 Description-Content-Type: text/markdown
 
 # Dowell Opensource License Compatibility Library
 
-## Version 0.1.0
+## Version 0.2.0
 
 ## Description
 
 The DoWell Legalzard Package provides a seamless interface to the Dowell Opensource License Compatibility Library powered
 by [DoWell UX Living Lab](https://uxlivinglab.com/en/).
 
 The Dowell Opensource License Compatibility Library provides access to a wide range of legal information and resources. It allows developers to retrieve
@@ -117,141 +117,141 @@
 ```
 
 Data Examples
 
 - License creation parameters
    ```json
   {
-                "license_name": "Test & Sample",
-                "license_tags": [],
-                "version": "No Version",
-                "type_of_license": "PERMISSIVE",
-                "short_description": "You can copy,modify and distribute this license as long as you fulfill license requirements.",
-                "description": "The SFL (Standard Function Library) from iMatix is a portable function library for C/C++ programs.The SFL is written in ANSI C and has been ported to MS-DOS, Windows, OS/2, Linux and other UNIX systems and Digital OpenVMS. It comes with complete sources and documentation in HTML. The SFL is free software that you may use and distribute for private or commercial purposes according to license agreement.",
-                "disclaimer": "Copyright © 1991-2000 iMatix Corporation.",
-                "risk_for_choosing_license": "This license places a lot of conditions on use and distribution of it.",
-                "limitation_of_liability": "In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.",
-                "license_url": "https://spdx.org/licenses/iMatix.html",
-                "logo_detail": {
-                    "filename": "img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png",
-                    "actual_filename": "Logo.png",
-                    "file_extension": "png",
-                    "url": "https://100080.pythonanywhere.com/media/img/img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png"
-                },
-                "recommendation": "",
-                "is_active": false,
-                "permissions": [
-                    {
-                        "action": "Patent Use",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Patent Grant",
-                        "permission": "No",
-                        "has_other_condition": false
-                    }
-                ],
-                "conditions": [
-                    {
-                        "action": "Disclose Source Code",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Network Use is for Distribution",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Release Under Same License",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "State Changes",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Code can be used in closed source project",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Copied",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Distributed",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    },
-                    {
-                        "action": "Reproduced",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Modified",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    },
-                    {
-                        "action": "Commercial Used",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    }
-                ],
-                "limitations": [
-                    {
-                        "action": "Liability",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Warranty",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Trademark use",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Redistribution",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    }
-                ],
-                "references": [],
-                "laws": "Not Fixed",
-                "sources": [
-                    {
-                        "action": "FSF Approved",
-                        "permission": "Yes"
-                    },
-                    {
-                        "action": "OSI Approved",
-                        "permission": "No"
-                    }
-                ],
-                "must_includes": [
-                    {
-                        "action": "License",
-                        "permission": "Yes"
-                    },
-                    {
-                        "action": "Copyright Notice",
-                        "permission": "Yes"
-                    }
-                ]
+        "license_name": "Test & Sample",
+        "license_tags": [],
+        "version": "No Version",
+        "type_of_license": "PERMISSIVE",
+        "short_description": "You can copy,modify and distribute this license as long as you fulfill license requirements.",
+        "description": "The SFL (Standard Function Library) from iMatix is a portable function library for C/C++ programs.The SFL is written in ANSI C and has been ported to MS-DOS, Windows, OS/2, Linux and other UNIX systems and Digital OpenVMS. It comes with complete sources and documentation in HTML. The SFL is free software that you may use and distribute for private or commercial purposes according to license agreement.",
+        "disclaimer": "Copyright © 1991-2000 iMatix Corporation.",
+        "risk_for_choosing_license": "This license places a lot of conditions on use and distribution of it.",
+        "limitation_of_liability": "In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.",
+        "license_url": "https://spdx.org/licenses/iMatix.html",
+        "logo_detail": {
+            "filename": "img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png",
+            "actual_filename": "Logo.png",
+            "file_extension": "png",
+            "url": "https://100080.pythonanywhere.com/media/img/img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png"
+        },
+        "recommendation": "",
+        "is_active": false,
+        "permissions": [
+            {
+                "action": "Patent Use",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Patent Grant",
+                "permission": "No",
+                "has_other_condition": false
             }
+        ],
+        "conditions": [
+            {
+                "action": "Disclose Source Code",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Network Use is for Distribution",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Release Under Same License",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "State Changes",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Code can be used in closed source project",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Copied",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Distributed",
+                "permission": "Yes",
+                "has_other_condition": true
+            },
+            {
+                "action": "Reproduced",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Modified",
+                "permission": "Yes",
+                "has_other_condition": true
+            },
+            {
+                "action": "Commercial Used",
+                "permission": "Yes",
+                "has_other_condition": false
+            }
+        ],
+        "limitations": [
+            {
+                "action": "Liability",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Warranty",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Trademark use",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Redistribution",
+                "permission": "Yes",
+                "has_other_condition": true
+            }
+        ],
+        "references": [],
+        "laws": "Not Fixed",
+        "sources": [
+            {
+                "action": "FSF Approved",
+                "permission": "Yes"
+            },
+            {
+                "action": "OSI Approved",
+                "permission": "No"
+            }
+        ],
+        "must_includes": [
+            {
+                "action": "License",
+                "permission": "Yes"
+            },
+            {
+                "action": "Copyright Notice",
+                "permission": "Yes"
+            }
+        ]
+    }
    ```
 - Compatibility Check parameters
    ```json
     {
     "license_event_id_one": "FB1010000000167238702450728865",
     "license_event_id_two": "FB1010000000167247184554419413",
     "user_id": 609,
```

### Comparing `Opensource License Compatibility from DoWell-0.1.0/PKG-INFO` & `Opensource License Compatibility from DoWell-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Opensource License Compatibility from DoWell
-Version: 0.1.0
+Version: 0.2.0
 Summary: Opensource License Compatibility from DoWell
-Author: Dennis RK.
-License: MIT
+Author: DoWell UX Living Lab
+License: Apache License 2.0
 Description-Content-Type: text/markdown
 
 # Dowell Opensource License Compatibility Library
 
-## Version 0.1.0
+## Version 0.2.0
 
 ## Description
 
 The DoWell Legalzard Package provides a seamless interface to the Dowell Opensource License Compatibility Library powered
 by [DoWell UX Living Lab](https://uxlivinglab.com/en/).
 
 The Dowell Opensource License Compatibility Library provides access to a wide range of legal information and resources. It allows developers to retrieve
@@ -117,141 +117,141 @@
 ```
 
 Data Examples
 
 - License creation parameters
    ```json
   {
-                "license_name": "Test & Sample",
-                "license_tags": [],
-                "version": "No Version",
-                "type_of_license": "PERMISSIVE",
-                "short_description": "You can copy,modify and distribute this license as long as you fulfill license requirements.",
-                "description": "The SFL (Standard Function Library) from iMatix is a portable function library for C/C++ programs.The SFL is written in ANSI C and has been ported to MS-DOS, Windows, OS/2, Linux and other UNIX systems and Digital OpenVMS. It comes with complete sources and documentation in HTML. The SFL is free software that you may use and distribute for private or commercial purposes according to license agreement.",
-                "disclaimer": "Copyright © 1991-2000 iMatix Corporation.",
-                "risk_for_choosing_license": "This license places a lot of conditions on use and distribution of it.",
-                "limitation_of_liability": "In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.",
-                "license_url": "https://spdx.org/licenses/iMatix.html",
-                "logo_detail": {
-                    "filename": "img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png",
-                    "actual_filename": "Logo.png",
-                    "file_extension": "png",
-                    "url": "https://100080.pythonanywhere.com/media/img/img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png"
-                },
-                "recommendation": "",
-                "is_active": false,
-                "permissions": [
-                    {
-                        "action": "Patent Use",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Patent Grant",
-                        "permission": "No",
-                        "has_other_condition": false
-                    }
-                ],
-                "conditions": [
-                    {
-                        "action": "Disclose Source Code",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Network Use is for Distribution",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Release Under Same License",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "State Changes",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Code can be used in closed source project",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Copied",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Distributed",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    },
-                    {
-                        "action": "Reproduced",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Modified",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    },
-                    {
-                        "action": "Commercial Used",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    }
-                ],
-                "limitations": [
-                    {
-                        "action": "Liability",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Warranty",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Trademark use",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Redistribution",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    }
-                ],
-                "references": [],
-                "laws": "Not Fixed",
-                "sources": [
-                    {
-                        "action": "FSF Approved",
-                        "permission": "Yes"
-                    },
-                    {
-                        "action": "OSI Approved",
-                        "permission": "No"
-                    }
-                ],
-                "must_includes": [
-                    {
-                        "action": "License",
-                        "permission": "Yes"
-                    },
-                    {
-                        "action": "Copyright Notice",
-                        "permission": "Yes"
-                    }
-                ]
+        "license_name": "Test & Sample",
+        "license_tags": [],
+        "version": "No Version",
+        "type_of_license": "PERMISSIVE",
+        "short_description": "You can copy,modify and distribute this license as long as you fulfill license requirements.",
+        "description": "The SFL (Standard Function Library) from iMatix is a portable function library for C/C++ programs.The SFL is written in ANSI C and has been ported to MS-DOS, Windows, OS/2, Linux and other UNIX systems and Digital OpenVMS. It comes with complete sources and documentation in HTML. The SFL is free software that you may use and distribute for private or commercial purposes according to license agreement.",
+        "disclaimer": "Copyright © 1991-2000 iMatix Corporation.",
+        "risk_for_choosing_license": "This license places a lot of conditions on use and distribution of it.",
+        "limitation_of_liability": "In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.",
+        "license_url": "https://spdx.org/licenses/iMatix.html",
+        "logo_detail": {
+            "filename": "img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png",
+            "actual_filename": "Logo.png",
+            "file_extension": "png",
+            "url": "https://100080.pythonanywhere.com/media/img/img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png"
+        },
+        "recommendation": "",
+        "is_active": false,
+        "permissions": [
+            {
+                "action": "Patent Use",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Patent Grant",
+                "permission": "No",
+                "has_other_condition": false
             }
+        ],
+        "conditions": [
+            {
+                "action": "Disclose Source Code",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Network Use is for Distribution",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Release Under Same License",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "State Changes",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Code can be used in closed source project",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Copied",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Distributed",
+                "permission": "Yes",
+                "has_other_condition": true
+            },
+            {
+                "action": "Reproduced",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Modified",
+                "permission": "Yes",
+                "has_other_condition": true
+            },
+            {
+                "action": "Commercial Used",
+                "permission": "Yes",
+                "has_other_condition": false
+            }
+        ],
+        "limitations": [
+            {
+                "action": "Liability",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Warranty",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Trademark use",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Redistribution",
+                "permission": "Yes",
+                "has_other_condition": true
+            }
+        ],
+        "references": [],
+        "laws": "Not Fixed",
+        "sources": [
+            {
+                "action": "FSF Approved",
+                "permission": "Yes"
+            },
+            {
+                "action": "OSI Approved",
+                "permission": "No"
+            }
+        ],
+        "must_includes": [
+            {
+                "action": "License",
+                "permission": "Yes"
+            },
+            {
+                "action": "Copyright Notice",
+                "permission": "Yes"
+            }
+        ]
+    }
    ```
 - Compatibility Check parameters
    ```json
     {
     "license_event_id_one": "FB1010000000167238702450728865",
     "license_event_id_two": "FB1010000000167247184554419413",
     "user_id": 609,
```

### Comparing `Opensource License Compatibility from DoWell-0.1.0/README.md` & `Opensource License Compatibility from DoWell-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Dowell Opensource License Compatibility Library
 
-## Version 0.1.0
+## Version 0.2.0
 
 ## Description
 
 The DoWell Legalzard Package provides a seamless interface to the Dowell Opensource License Compatibility Library powered
 by [DoWell UX Living Lab](https://uxlivinglab.com/en/).
 
 The Dowell Opensource License Compatibility Library provides access to a wide range of legal information and resources. It allows developers to retrieve
@@ -109,141 +109,141 @@
 ```
 
 Data Examples
 
 - License creation parameters
    ```json
   {
-                "license_name": "Test & Sample",
-                "license_tags": [],
-                "version": "No Version",
-                "type_of_license": "PERMISSIVE",
-                "short_description": "You can copy,modify and distribute this license as long as you fulfill license requirements.",
-                "description": "The SFL (Standard Function Library) from iMatix is a portable function library for C/C++ programs.The SFL is written in ANSI C and has been ported to MS-DOS, Windows, OS/2, Linux and other UNIX systems and Digital OpenVMS. It comes with complete sources and documentation in HTML. The SFL is free software that you may use and distribute for private or commercial purposes according to license agreement.",
-                "disclaimer": "Copyright © 1991-2000 iMatix Corporation.",
-                "risk_for_choosing_license": "This license places a lot of conditions on use and distribution of it.",
-                "limitation_of_liability": "In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.",
-                "license_url": "https://spdx.org/licenses/iMatix.html",
-                "logo_detail": {
-                    "filename": "img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png",
-                    "actual_filename": "Logo.png",
-                    "file_extension": "png",
-                    "url": "https://100080.pythonanywhere.com/media/img/img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png"
-                },
-                "recommendation": "",
-                "is_active": false,
-                "permissions": [
-                    {
-                        "action": "Patent Use",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Patent Grant",
-                        "permission": "No",
-                        "has_other_condition": false
-                    }
-                ],
-                "conditions": [
-                    {
-                        "action": "Disclose Source Code",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Network Use is for Distribution",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Release Under Same License",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "State Changes",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Code can be used in closed source project",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Copied",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Distributed",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    },
-                    {
-                        "action": "Reproduced",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Modified",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    },
-                    {
-                        "action": "Commercial Used",
-                        "permission": "Yes",
-                        "has_other_condition": false
-                    }
-                ],
-                "limitations": [
-                    {
-                        "action": "Liability",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Warranty",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Trademark use",
-                        "permission": "No",
-                        "has_other_condition": false
-                    },
-                    {
-                        "action": "Redistribution",
-                        "permission": "Yes",
-                        "has_other_condition": true
-                    }
-                ],
-                "references": [],
-                "laws": "Not Fixed",
-                "sources": [
-                    {
-                        "action": "FSF Approved",
-                        "permission": "Yes"
-                    },
-                    {
-                        "action": "OSI Approved",
-                        "permission": "No"
-                    }
-                ],
-                "must_includes": [
-                    {
-                        "action": "License",
-                        "permission": "Yes"
-                    },
-                    {
-                        "action": "Copyright Notice",
-                        "permission": "Yes"
-                    }
-                ]
+        "license_name": "Test & Sample",
+        "license_tags": [],
+        "version": "No Version",
+        "type_of_license": "PERMISSIVE",
+        "short_description": "You can copy,modify and distribute this license as long as you fulfill license requirements.",
+        "description": "The SFL (Standard Function Library) from iMatix is a portable function library for C/C++ programs.The SFL is written in ANSI C and has been ported to MS-DOS, Windows, OS/2, Linux and other UNIX systems and Digital OpenVMS. It comes with complete sources and documentation in HTML. The SFL is free software that you may use and distribute for private or commercial purposes according to license agreement.",
+        "disclaimer": "Copyright © 1991-2000 iMatix Corporation.",
+        "risk_for_choosing_license": "This license places a lot of conditions on use and distribution of it.",
+        "limitation_of_liability": "In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.",
+        "license_url": "https://spdx.org/licenses/iMatix.html",
+        "logo_detail": {
+            "filename": "img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png",
+            "actual_filename": "Logo.png",
+            "file_extension": "png",
+            "url": "https://100080.pythonanywhere.com/media/img/img_02c8ccb5-3ffb-4737-83db-effb3da529ed.png"
+        },
+        "recommendation": "",
+        "is_active": false,
+        "permissions": [
+            {
+                "action": "Patent Use",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Patent Grant",
+                "permission": "No",
+                "has_other_condition": false
             }
+        ],
+        "conditions": [
+            {
+                "action": "Disclose Source Code",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Network Use is for Distribution",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Release Under Same License",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "State Changes",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Code can be used in closed source project",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Copied",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Distributed",
+                "permission": "Yes",
+                "has_other_condition": true
+            },
+            {
+                "action": "Reproduced",
+                "permission": "Yes",
+                "has_other_condition": false
+            },
+            {
+                "action": "Modified",
+                "permission": "Yes",
+                "has_other_condition": true
+            },
+            {
+                "action": "Commercial Used",
+                "permission": "Yes",
+                "has_other_condition": false
+            }
+        ],
+        "limitations": [
+            {
+                "action": "Liability",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Warranty",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Trademark use",
+                "permission": "No",
+                "has_other_condition": false
+            },
+            {
+                "action": "Redistribution",
+                "permission": "Yes",
+                "has_other_condition": true
+            }
+        ],
+        "references": [],
+        "laws": "Not Fixed",
+        "sources": [
+            {
+                "action": "FSF Approved",
+                "permission": "Yes"
+            },
+            {
+                "action": "OSI Approved",
+                "permission": "No"
+            }
+        ],
+        "must_includes": [
+            {
+                "action": "License",
+                "permission": "Yes"
+            },
+            {
+                "action": "Copyright Notice",
+                "permission": "Yes"
+            }
+        ]
+    }
    ```
 - Compatibility Check parameters
    ```json
     {
     "license_event_id_one": "FB1010000000167238702450728865",
     "license_event_id_two": "FB1010000000167247184554419413",
     "user_id": 609,
```

### Comparing `Opensource License Compatibility from DoWell-0.1.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py` & `Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py`

 * *Files identical despite different names*

### Comparing `Opensource License Compatibility from DoWell-0.1.0/setup.py` & `Opensource License Compatibility from DoWell-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="Opensource License Compatibility from DoWell",
-    version="0.1.0",
+    version="0.2.0",
     description="Opensource License Compatibility from DoWell",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author='Dennis RK.',
-    license="MIT",
+    author='DoWell UX Living Lab',
+    license="Apache License 2.0",
     packages=["doWellOpensourceLicenseCompatibility"],
     include_package_data=True,
     install_requires=["requests"]
 )
```

