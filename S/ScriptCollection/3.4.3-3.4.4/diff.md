# Comparing `tmp/ScriptCollection-3.4.3-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 62381 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat    19068 b- defN 23-Jul-09 10:07 ScriptCollection/Executables.py
+Zip file size: 62443 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat    19324 b- defN 23-Jul-17 20:11 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34378 b- defN 23-Jun-27 21:57 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    96083 b- defN 23-Jul-11 10:23 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   144215 b- defN 23-Jul-11 10:23 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    96159 b- defN 23-Jul-17 20:11 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   144595 b- defN 23-Jul-17 20:11 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/RECORD
-14 files, 324034 bytes uncompressed, 60199 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-17 20:12 ScriptCollection-3.4.4.dist-info/RECORD
+14 files, 324746 bytes uncompressed, 60261 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.4.3.dist-info/METADATA
+Filename: ScriptCollection-3.4.4.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.4.3.dist-info/WHEEL
+Filename: ScriptCollection-3.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.4.3.dist-info/entry_points.txt
+Filename: ScriptCollection-3.4.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.3.dist-info/top_level.txt
+Filename: ScriptCollection-3.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.3.dist-info/RECORD
+Filename: ScriptCollection-3.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/Executables.py

```diff
@@ -315,42 +315,46 @@
     args = parser.parse_args()
     ScriptCollectionCore().generate_certificate_authority(os.getcwd(), args.name, args.subj_c, args.subj_st, args.subj_l, args.subj_o, args.subj_ou, args.days_until_expire, args.password)
     return 0
 
 
 def GenerateCertificate() -> int:
     parser = argparse.ArgumentParser()
+    parser.add_argument('--filename', required=True)
     parser.add_argument('--domain', required=True)
     parser.add_argument('--subj_c', required=True)
     parser.add_argument('--subj_st', required=True)
     parser.add_argument('--subj_l', required=True)
     parser.add_argument('--subj_o', required=True)
     parser.add_argument('--subj_ou', required=True)
     parser.add_argument('--days_until_expire', required=False, default=None, type=int)
     parser.add_argument('--password', required=False, default=None)
     args = parser.parse_args()
-    ScriptCollectionCore().generate_certificate(os.getcwd(), args.domain, args.subj_c, args.subj_st, args.subj_l, args.subj_o, args.subj_ou, args.days_until_expire, args.password)
+    ScriptCollectionCore().generate_certificate(os.getcwd(), args.domain, args.filename, args.subj_c, args.subj_st,
+                                                args.subj_l, args.subj_o, args.subj_ou, args.days_until_expire, args.password)
     return 0
 
 
 def GenerateCertificateSignRequest() -> int:
     parser = argparse.ArgumentParser()
+    parser.add_argument('--filename', required=True)
     parser.add_argument('--domain', required=True)
     parser.add_argument('--subj_c', required=True)
     parser.add_argument('--subj_st', required=True)
     parser.add_argument('--subj_l', required=True)
     parser.add_argument('--subj_o', required=True)
     parser.add_argument('--subj_ou', required=True)
     args = parser.parse_args()
-    ScriptCollectionCore().generate_certificate_sign_request(os.getcwd(), args.domain, args.subj_c, args.subj_st, args.subj_l, args.subj_o, args.sub_ou)
+    ScriptCollectionCore().generate_certificate_sign_request(os.getcwd(), args.domain, args.filename, args.subj_c, args.subj_st, args.subj_l, args.subj_o, args.sub_ou)
     return 0
 
 
 def SignCertificate() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--cafolder', required=True)
     parser.add_argument('--caname', required=True)
     parser.add_argument('--targetcertificate', required=True)
+    parser.add_argument('--filename', required=True)
     parser.add_argument('--days_until_expire', required=False, default=None, type=int)
     args = parser.parse_args()
-    ScriptCollectionCore().sign_certificate(os.getcwd(), args.cafolder, args.caname, args.targetcertificate, args.args.days_until_expire)
+    ScriptCollectionCore().sign_certificate(os.getcwd(), args.cafolder, args.caname, args.targetcertificate, args.filename, args.args.days_until_expire)
     return 0
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -25,15 +25,15 @@
 import PyPDF2
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.4.3"
+version = "3.4.4"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -1542,27 +1542,27 @@
         if password is None:
             password = GeneralUtilities.generate_password()
         self.run_program("openssl", f'req -new -newkey ec -pkeyopt ec_paramgen_curve:prime256v1 -days {days_until_expire} -nodes -x509 -subj ' +
                          f'/C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={name}/OU={subj_ou} -passout pass:{password} ' +
                          f'-keyout {name}.key -out {name}.crt', folder)
 
     @GeneralUtilities.check_arguments
-    def generate_certificate(self, folder: str, domain: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,
+    def generate_certificate(self, folder: str,  domain: str,filename:str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,
                              days_until_expire: int = None, password: str = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         if password is None:
             password = GeneralUtilities.generate_password()
         rsa_key_length = 4096
-        self.run_program("openssl", f'genrsa -out {domain}.key {rsa_key_length}', folder)
+        self.run_program("openssl", f'genrsa -out {filename}.key {rsa_key_length}', folder)
         self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} -x509 ' +
-                         f'-key {domain}.key -out {domain}.unsigned.crt -days {days_until_expire}', folder)
-        self.run_program("openssl", f'pkcs12 -export -out {domain}.selfsigned.pfx -password pass:{password} -inkey {domain}.key -in {domain}.unsigned.crt', folder)
-        GeneralUtilities.write_text_to_file(os.path.join(folder, f"{domain}.password"), password)
-        GeneralUtilities.write_text_to_file(os.path.join(folder, f"{domain}.san.conf"), f"""[ req ]
+                         f'-key {filename}.key -out {filename}.unsigned.crt -days {days_until_expire}', folder)
+        self.run_program("openssl", f'pkcs12 -export -out {filename}.selfsigned.pfx -password pass:{password} -inkey {filename}.key -in {filename}.unsigned.crt', folder)
+        GeneralUtilities.write_text_to_file(os.path.join(folder, f"{filename}.password"), password)
+        GeneralUtilities.write_text_to_file(os.path.join(folder, f"{filename}.san.conf"), f"""[ req ]
 default_bits        = {rsa_key_length}
 distinguished_name  = req_distinguished_name
 req_extensions      = v3_req
 default_md          = sha256
 dirstring_type      = nombstr
 prompt              = no
 
@@ -1578,28 +1578,28 @@
 subjectAltName      = @subject_alt_name
 
 [ subject_alt_name ]
 DNS                 = {domain}
 """)
 
     @GeneralUtilities.check_arguments
-    def generate_certificate_sign_request(self, folder: str, domain: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str) -> None:
+    def generate_certificate_sign_request(self, folder: str, domain: str,filename:str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str) -> None:
         self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} ' +
-                         f'-key {domain}.key -out {domain}.csr -config {domain}.san.conf', folder)
+                         f'-key {filename}.key -out {filename}.csr -config {filename}.san.conf', folder)
 
     @GeneralUtilities.check_arguments
-    def sign_certificate(self, folder: str, ca_folder: str, ca_name: str, domain: str, days_until_expire: int = None) -> None:
+    def sign_certificate(self, folder: str, ca_folder: str, ca_name: str, domain: str,filename:str, days_until_expire: int = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         ca = os.path.join(ca_folder, ca_name)
-        password_file = os.path.join(folder, f"{domain}.password")
+        password_file = os.path.join(folder, f"{filename}.password")
         password = GeneralUtilities.read_text_from_file(password_file)
-        self.run_program("openssl", f'x509 -req -in {domain}.csr -CA {ca}.crt -CAkey {ca}.key -CAcreateserial -CAserial {ca}.srl ' +
-                         f'-out {domain}.crt -days {days_until_expire} -sha256 -extensions v3_req -extfile {domain}.san.conf', folder)
-        self.run_program("openssl", f'pkcs12 -export -out {domain}.pfx -inkey {domain}.key -in {domain}.crt -password pass:{password}', folder)
+        self.run_program("openssl", f'x509 -req -in {filename}.csr -CA {ca}.crt -CAkey {ca}.key -CAcreateserial -CAserial {ca}.srl ' +
+                         f'-out {filename}.crt -days {days_until_expire} -sha256 -extensions v3_req -extfile {filename}.san.conf', folder)
+        self.run_program("openssl", f'pkcs12 -export -out {filename}.pfx -inkey {filename}.key -in {filename}.crt -password pass:{password}', folder)
 
     @GeneralUtilities.check_arguments
     def update_dependencies_of_python_in_requirementstxt_file(self, file: str, verbosity: int):
         lines = GeneralUtilities.read_lines_from_file(file)
         new_lines = []
         for line in lines:
             new_lines.append(self.__get_updated_line_for_python_requirements(line.strip()))
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -1005,22 +1005,26 @@
 
     @GeneralUtilities.check_arguments
     def assert_no_uncommitted_changes(self, repository_folder: str):
         if self.__sc.git_repository_has_uncommitted_changes(repository_folder):
             raise ValueError(f"Repository '{repository_folder}' has uncommitted changes.")
 
     @GeneralUtilities.check_arguments
-    def generate_certificate_for_nonproductive_purposes(self, codeunit_folder: str,
-                                                        resource_name: str = "DevelopmentCertificate"):
-        resources_folder = os.path.join(codeunit_folder, "Other", "Resources")
-        certificate_folder = os.path.join(resources_folder, resource_name)
-        dev_ca_name = "DevelopmentCertificateAuthority"
-        ca_folder = os.path.join(resources_folder, dev_ca_name)
+    def generate_certificate_for_development_purposes(self, codeunit_folder: str, domain: str = None):
         codeunit_name = os.path.basename(codeunit_folder)
-        domain = f"{codeunit_name.lower()}.test.local"
+        if domain is None:
+            domain = f"{codeunit_name}.test.local"
+        domain = domain.lower()
+        resources_folder: str = os.path.join(codeunit_folder, "Other", "Resources")
+        resource_name: str = "DevelopmentCertificate"
+        certificate_folder: str = os.path.join(resources_folder, resource_name)
+        resource_content_filename: str = codeunit_name+resource_name
+        ca_resource_name: str = f"{resource_name}Authority"
+        dev_ca_name = codeunit_name+ca_resource_name
+        ca_folder = os.path.join(resources_folder, ca_resource_name)
         certificate_file = os.path.join(certificate_folder, f"{domain}.crt")
         unsignedcertificate_file = os.path.join(certificate_folder, f"{domain}.unsigned.crt")
         certificate_exists = os.path.exists(certificate_file)
         if certificate_exists:
             certificate_expired = GeneralUtilities.certificate_is_expired(certificate_file)
             generate_new_certificate = certificate_expired
         else:
@@ -1028,17 +1032,17 @@
         if generate_new_certificate:
             GeneralUtilities.ensure_directory_does_not_exist(certificate_folder)
             GeneralUtilities.ensure_directory_exists(certificate_folder)
             GeneralUtilities.ensure_directory_does_not_exist(ca_folder)
             GeneralUtilities.ensure_directory_exists(ca_folder)
             GeneralUtilities.write_message_to_stdout("Generate TLS-certificate for development-purposes.")
             self.__sc.generate_certificate_authority(ca_folder, dev_ca_name, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
-            self.__sc.generate_certificate(certificate_folder, domain, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
-            self.__sc.generate_certificate_sign_request(certificate_folder, domain, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
-            self.__sc.sign_certificate(certificate_folder, ca_folder, dev_ca_name, domain)
+            self.__sc.generate_certificate(certificate_folder, domain, resource_content_filename, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
+            self.__sc.generate_certificate_sign_request(certificate_folder, domain, resource_content_filename, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
+            self.__sc.sign_certificate(certificate_folder, ca_folder, dev_ca_name, domain, resource_content_filename)
             GeneralUtilities.ensure_file_does_not_exist(unsignedcertificate_file)
 
     @GeneralUtilities.check_arguments
     def get_codeunits(self, repository_folder: str) -> list[str]:
         result: list[str] = []
         for direct_subfolder in GeneralUtilities.get_direct_folders_of_folder(repository_folder):
             subfoldername = os.path.basename(direct_subfolder)
@@ -1516,30 +1520,33 @@
             return ""
         elif length == 1:
             return results[0]
         else:
             raise ValueError("Too many results found.")
 
     @GeneralUtilities.check_arguments
-    def set_constants_for_certificate_public_information(self, codeunit_folder: str, source_constant_name: str = "DevelopmentCertificate"):
+    def set_constants_for_certificate_public_information(self, codeunit_folder: str, source_constant_name: str = "DevelopmentCertificate", domain: str = None):
         """Expects a certificate-resource and generates a constant for its public information"""
         codeunit_name = os.path.basename(codeunit_folder)
-        domain = f"{codeunit_name}.test.local"
+        if domain is None:
+            domain = f"{codeunit_name}.test.local"
+        domain = domain.lower()
         certificate_file = os.path.join(codeunit_folder, "Other", "Resources", source_constant_name, f"{domain}.crt")
         with open(certificate_file, encoding="utf-8") as text_wrapper:
             certificate = crypto.load_certificate(crypto.FILETYPE_PEM, text_wrapper.read())
         certificate_publickey = crypto.dump_publickey(crypto.FILETYPE_PEM, certificate.get_pubkey()).decode("utf-8")
         self.set_constant(codeunit_folder, source_constant_name+"PublicKey", certificate_publickey)
 
     @GeneralUtilities.check_arguments
     def set_constants_for_certificate_private_information(self, codeunit_folder: str, certificate_resource_name: str = "DevelopmentCertificate", domain: str = None):
         """Expects a certificate-resource and generates a constant for its sensitive information in hex-format"""
+        codeunit_name = os.path.basename(codeunit_folder)
         if domain is None:
-            codeunit_name = os.path.basename(codeunit_folder)
-            domain = codeunit_name
+            domain = f"{codeunit_name}.test.local"
+        domain = domain.lower()
         self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.pfx", "PFX")
         self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.password", "Password")
 
     @GeneralUtilities.check_arguments
     def generate_constant_from_resource_by_filename(self, codeunit_folder: str, resource_name: str, filename: str, constant_name: str):
         certificate_resource_folder = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
         resource_file = os.path.join(certificate_resource_folder, filename)
```

## Comparing `ScriptCollection-3.4.3.dist-info/METADATA` & `ScriptCollection-3.4.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.4.3
+Version: 3.4.4
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
@@ -19,15 +19,15 @@
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: coverage (>=7.2.7)
-Requires-Dist: cyclonedx-bom (>=3.11.0)
+Requires-Dist: cyclonedx-bom (>=3.11.2)
 Requires-Dist: defusedxml (>=0.7.1)
 Requires-Dist: keyboard (>=0.13.5)
 Requires-Dist: lxml (>=4.9.3)
 Requires-Dist: ntplib (>=0.4.0)
 Requires-Dist: Pillow (>=10.0.0)
 Requires-Dist: pycdlib (>=1.14.0)
 Requires-Dist: Pygments (>=2.15.1)
```

## Comparing `ScriptCollection-3.4.3.dist-info/entry_points.txt` & `ScriptCollection-3.4.4.dist-info/entry_points.txt`

 * *Files identical despite different names*

