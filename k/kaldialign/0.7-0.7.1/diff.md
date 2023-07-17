# Comparing `tmp/kaldialign-0.7-cp39-cp39-win_amd64.whl.zip` & `tmp/kaldialign-0.7.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 62802 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   116736 b- defN 23-Jul-03 16:29 _kaldialign.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-03 16:29 kaldialign/__init__.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-03 16:29 kaldialign-0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2936 b- defN 23-Jul-03 16:29 kaldialign-0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-03 16:29 kaldialign-0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-03 16:29 kaldialign-0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      561 b- defN 23-Jul-03 16:29 kaldialign-0.7.dist-info/RECORD
-7 files, 132980 bytes uncompressed, 61816 bytes compressed:  53.5%
+Zip file size: 82670 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-17 15:00 kaldialign.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-17 15:00 kaldialign-0.7.1.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-17 15:00 kaldialign/
+-rwxr-xr-x  2.0 unx   184112 b- defN 23-Jul-17 15:00 _kaldialign.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-17 15:00 kaldialign-0.7.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-17 15:00 kaldialign-0.7.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      590 b- defN 23-Jul-17 15:00 kaldialign-0.7.1.dist-info/RECORD
+-rw-r--r--  2.0 unx      148 b- defN 23-Jul-17 15:00 kaldialign-0.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     2848 b- defN 23-Jul-17 15:00 kaldialign-0.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx     1026 b- defN 23-Jul-17 15:00 kaldialign/__init__.py
+10 files, 200104 bytes uncompressed, 81304 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
-Filename: _kaldialign.cp39-win_amd64.pyd
+Filename: kaldialign.libs/
 Comment: 
 
-Filename: kaldialign/__init__.py
+Filename: kaldialign-0.7.1.dist-info/
+Comment: 
+
+Filename: kaldialign/
+Comment: 
+
+Filename: _kaldialign.cpython-39-x86_64-linux-gnu.so
+Comment: 
+
+Filename: kaldialign-0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kaldialign-0.7.dist-info/LICENSE
+Filename: kaldialign-0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: kaldialign-0.7.dist-info/METADATA
+Filename: kaldialign-0.7.1.dist-info/RECORD
 Comment: 
 
-Filename: kaldialign-0.7.dist-info/WHEEL
+Filename: kaldialign-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: kaldialign-0.7.dist-info/top_level.txt
+Filename: kaldialign-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: kaldialign-0.7.dist-info/RECORD
+Filename: kaldialign/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## kaldialign/__init__.py

```diff
@@ -1,42 +1,42 @@
-from typing import List, Tuple
-import _kaldialign
-
-
-def edit_distance(a, b, sclite_mode=False):
-    int2sym = dict(enumerate(sorted(set(a) | set(b))))
-    sym2int = {v: k for k, v in int2sym.items()}
-
-    ai: List[int] = []
-    bi: List[int] = []
-    for sym in a:
-        ai.append(sym2int[sym])
-
-    for sym in b:
-        bi.append(sym2int[sym])
-
-    return _kaldialign.edit_distance(ai, bi, sclite_mode)
-
-
-def align(a, b, eps_symbol, sclite_mode=False):
-    int2sym = dict(enumerate(sorted(set(a) | set(b) | {eps_symbol})))
-    sym2int = {v: k for k, v in int2sym.items()}
-
-    ai: List[int] = []
-    bi: List[int] = []
-
-    for sym in a:
-        ai.append(sym2int[sym])
-
-    for sym in b:
-        bi.append(sym2int[sym])
-
-    eps_int = sym2int[eps_symbol]
-    alignment: List[Tuple[int, int]] = _kaldialign.align(ai, bi, eps_int, sclite_mode)
-
-    ali = []
-    idx = 0
-    for idx in range(len(alignment)):
-        ali.append((int2sym[alignment[idx][0]], int2sym[alignment[idx][1]]))
-
-    return ali
-__version__ = '0.7'
+from typing import List, Tuple
+import _kaldialign
+
+
+def edit_distance(a, b, sclite_mode=False):
+    int2sym = dict(enumerate(sorted(set(a) | set(b))))
+    sym2int = {v: k for k, v in int2sym.items()}
+
+    ai: List[int] = []
+    bi: List[int] = []
+    for sym in a:
+        ai.append(sym2int[sym])
+
+    for sym in b:
+        bi.append(sym2int[sym])
+
+    return _kaldialign.edit_distance(ai, bi, sclite_mode)
+
+
+def align(a, b, eps_symbol, sclite_mode=False):
+    int2sym = dict(enumerate(sorted(set(a) | set(b) | {eps_symbol})))
+    sym2int = {v: k for k, v in int2sym.items()}
+
+    ai: List[int] = []
+    bi: List[int] = []
+
+    for sym in a:
+        ai.append(sym2int[sym])
+
+    for sym in b:
+        bi.append(sym2int[sym])
+
+    eps_int = sym2int[eps_symbol]
+    alignment: List[Tuple[int, int]] = _kaldialign.align(ai, bi, eps_int, sclite_mode)
+
+    ali = []
+    idx = 0
+    for idx in range(len(alignment)):
+        ali.append((int2sym[alignment[idx][0]], int2sym[alignment[idx][1]]))
+
+    return ali
+__version__ = '0.7.1'
```

## Comparing `kaldialign-0.7.dist-info/LICENSE` & `kaldialign-0.7.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `kaldialign-0.7.dist-info/METADATA` & `kaldialign-0.7.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-Metadata-Version: 2.1
-Name: kaldialign
-Version: 0.7
-Summary: Kaldi alignment methods wrapped into Python
-Home-page: https://github.com/pzelasko/kaldialign
-Author: Piotr Żelasko
-Author-email: pzelasko@jhu.edu
-License: Apache licensed, as found in the LICENSE file
-Keywords: natural language processing,speech recognition,machine learning
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Linguistic
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# kaldialign
-
-A small package that exposes edit distance computation functions from [Kaldi](https://github.com/kaldi-asr/kaldi). It uses the original Kaldi code and wraps it using pybind11.
-
-## Installation
-
-```bash
-conda install -c kaldialign kaldialign
-```
-
-or
-
-```bash
-pip install --verbose kaldialign
-```
-
-or
-
-```bash
-pip install --verbose -U git+https://github.com/pzelasko/kaldialign.git
-```
-
-or
-
-```bash
-git clone https://github.com/pzelasko/kaldialign.git
-cd kaldialign
-python3 -m pip install --verbose .
-```
-
-## Examples
-
-- `align(seq1, seq2, epsilon)` - used to obtain the alignment between two string sequences. `epsilon` should be a null symbol (indicating deletion/insertion) that doesn't exist in either sequence.
-
-```python
-from kaldialign import align
-
-EPS = '*'
-a = ['a', 'b', 'c']
-b = ['a', 's', 'x', 'c']
-ali = align(a, b, EPS)
-assert ali == [('a', 'a'), ('b', 's'), (EPS, 'x'), ('c', 'c')]
-```
-
-- `edit_distance(seq1, seq2)` - used to obtain the total edit distance, as well as the number of insertions, deletions and substitutions.
-
-```python
-from kaldialign import edit_distance
-
-a = ['a', 'b', 'c']
-b = ['a', 's', 'x', 'c']
-results = edit_distance(a, b)
-assert results == {
-    'ins': 1,
-    'del': 0,
-    'sub': 1,
-    'total': 2
-}
-```
-
-- For both of the above examples, you can pass `sclite_mode=True` to compute WER or alignments
-based on SCLITE style weights, i.e., insertion/deletion cost 3 and substitution cost 4.
-
-## Motivation
-
-The need for this arised from the fact that practically all implementations of the Levenshtein distance have slight differences, making it impossible to use a different scoring tool than Kaldi and get the same error rate results. This package copies code from Kaldi directly and wraps it using Cython, avoiding the issue altogether.
+Metadata-Version: 2.1
+Name: kaldialign
+Version: 0.7.1
+Summary: Kaldi alignment methods wrapped into Python
+Home-page: https://github.com/pzelasko/kaldialign
+Author: Piotr Żelasko
+Author-email: pzelasko@jhu.edu
+License: Apache licensed, as found in the LICENSE file
+Keywords: natural language processing,speech recognition,machine learning
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# kaldialign
+
+A small package that exposes edit distance computation functions from [Kaldi](https://github.com/kaldi-asr/kaldi). It uses the original Kaldi code and wraps it using pybind11.
+
+## Installation
+
+```bash
+conda install -c kaldialign kaldialign
+```
+
+or
+
+```bash
+pip install --verbose kaldialign
+```
+
+or
+
+```bash
+pip install --verbose -U git+https://github.com/pzelasko/kaldialign.git
+```
+
+or
+
+```bash
+git clone https://github.com/pzelasko/kaldialign.git
+cd kaldialign
+python3 -m pip install --verbose .
+```
+
+## Examples
+
+- `align(seq1, seq2, epsilon)` - used to obtain the alignment between two string sequences. `epsilon` should be a null symbol (indicating deletion/insertion) that doesn't exist in either sequence.
+
+```python
+from kaldialign import align
+
+EPS = '*'
+a = ['a', 'b', 'c']
+b = ['a', 's', 'x', 'c']
+ali = align(a, b, EPS)
+assert ali == [('a', 'a'), ('b', 's'), (EPS, 'x'), ('c', 'c')]
+```
+
+- `edit_distance(seq1, seq2)` - used to obtain the total edit distance, as well as the number of insertions, deletions and substitutions.
+
+```python
+from kaldialign import edit_distance
+
+a = ['a', 'b', 'c']
+b = ['a', 's', 'x', 'c']
+results = edit_distance(a, b)
+assert results == {
+    'ins': 1,
+    'del': 0,
+    'sub': 1,
+    'total': 2
+}
+```
+
+- For both of the above examples, you can pass `sclite_mode=True` to compute WER or alignments
+based on SCLITE style weights, i.e., insertion/deletion cost 3 and substitution cost 4.
+
+## Motivation
+
+The need for this arised from the fact that practically all implementations of the Levenshtein distance have slight differences, making it impossible to use a different scoring tool than Kaldi and get the same error rate results. This package copies code from Kaldi directly and wraps it using Cython, avoiding the issue altogether.
```

