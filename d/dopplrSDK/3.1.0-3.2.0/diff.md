# Comparing `tmp/dopplrSDK-3.1.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-3.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5209 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    11914 b- defN 23-Jul-07 13:39 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/RECORD
-6 files, 14193 bytes uncompressed, 4343 bytes compressed:  69.4%
+Zip file size: 5490 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    12871 b- defN 23-Jul-17 11:28 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/RECORD
+6 files, 15150 bytes uncompressed, 4624 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-3.1.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-3.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-3.1.0.dist-info/METADATA
+Filename: dopplrSDK-3.2.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-3.1.0.dist-info/WHEEL
+Filename: dopplrSDK-3.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-3.1.0.dist-info/top_level.txt
+Filename: dopplrSDK-3.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-3.1.0.dist-info/RECORD
+Filename: dopplrSDK-3.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -7,105 +7,118 @@
 import base64
 import hashlib
 from Crypto.Cipher import DES3
 from Crypto.Util.Padding import unpad
 from cryptography.fernet import Fernet
 from botocore.client import Config
 from azure.storage.blob import BlobServiceClient, BlobClient
+import requests
 
 def decrypt_keys(de_key):
     keys={}
     key = "xLrwTFMdJroA8zG_5wnkQADuJvD5TTmfCKfe8RRz_xU="
-    key = hashlib.md5(key.encode("utf-8")).digest()
+    key1 = hashlib.md5(key.encode("utf-8")).digest()
     cipher_bytes = base64.b64decode(de_key)
-    cipher = DES3.new(key, DES3.MODE_ECB)
+    cipher = DES3.new(key1, DES3.MODE_ECB)
     decrypted_bytes = cipher.decrypt(cipher_bytes)
     decrypted_text = unpad(decrypted_bytes, DES3.block_size).decode("utf-8")
     data=decrypted_text.split('|')
     
     for i in data:
         a=i.split(':')
         keys[a[0]]=a[1]
-    if keys['Cloud'] == 'MinIO':
-        s3=boto3.client('s3',endpoint_url="http://20.219.94.221:9000",
+    Cloud=keys['Cloud']
+    if Cloud == 'MinIO':
+        endpoint_url=keys['endpoint_url']
+        s3=boto3.client('s3',endpoint_url=f"http://{endpoint_url}:9000",
                       aws_access_key_id=keys['Access'],
                       aws_secret_access_key=keys['Secret'],
-                      config=Config(signature_version='s3v4'),region_name="us-west-2"
-                      )
-    elif keys['Cloud'] == 'AWS':
+                      config=Config(signature_version='s3v4'),region_name=keys['region_name']
+                      )   
+        
+    elif Cloud == 'AWS':
         s3 = boto3.client('s3', aws_access_key_id=keys['Access'], aws_secret_access_key=keys['Secret'])
-    elif keys['Cloud'] == 'AZURE':
+    elif Cloud == 'AZURE':
         connect_str = "DefaultEndpointsProtocol=https;AccountName={0};AccountKey={1};EndpointSuffix=core.windows.net".format(keys['Access'],keys['Secret'])            
         s3 = BlobServiceClient.from_connection_string(connect_str)
         
-    if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':       
+    if Cloud == 'MinIO'or Cloud =='AWS':       
         ContainerName = keys['Bucket']
         file_key = 'Connections/Dopplr_Connection.ini'
         db = {}
         response = s3.get_object(Bucket=ContainerName, Key=file_key)
         file_content = response['Body'].read()
-        key = b"xLrwTFMdJroA8zG_5wnkQADuJvD5TTmfCKfe8RRz_xU="
-        fernet = Fernet(key)
+        key2=key.encode('utf-8')
+        fernet = Fernet(key2)
         decrypted_data = fernet.decrypt(file_content)
         decrypted_data = decrypted_data.decode('utf-8')
         lines = decrypted_data.split('\n')
         index=lines.index('[postgresql]\r')
-        data=lines[index+1:index+6]
+        data=lines[index+1:index+8]
 
         for i in data:
             a=i.split('=')
             db[a[0]]=a[1].replace('\r','')
+
     else:
         
         ContainerName = keys['Bucket']
         file_key = 'Connections/Dopplr_Connection.ini'
         blob_client = s3.get_blob_client(container=ContainerName, blob=file_key)
         az = blob_client.download_blob()
         file_contents = az.readall()
-        key = b"xLrwTFMdJroA8zG_5wnkQADuJvD5TTmfCKfe8RRz_xU="
-        fernet = Fernet(key)
+        key2=key.encode('utf-8')
+        fernet = Fernet(key2)
         decrypted_data = fernet.decrypt(file_contents)
         decrypted_data = decrypted_data.decode('utf-8')
         lines = decrypted_data.split('\n')
         index = lines.index('[postgresql]\r')
-        data = lines[index + 1: index + 6]
+        data = lines[index + 1: index + 8]
         db = {}
         for i in data:
             a = i.split('=')
             db[a[0]]=a[1].replace('\r', '')
         
 
     return keys,db,s3
 
-def putFileTomywrkspace(filePath,file_type,loginName,de_key):
+def putFileTomywrkspace(filePath,file_type,loginName,Project_name,de_key):
     try:
         keys,db,client=decrypt_keys(de_key)
+        api=db['api']
+        fapi=db['fastapi']
+        Cloud=keys['Cloud']
+        
 
-        query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
 
+        query="select DOR.\"OrgName\",Du.\"UserKey\",P.\"Project_key\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" \
+join doppler.\"DopplerProject\" P on P.\"UserKey\"=Du.\"UserKey\" where Du.\"LoginName\"='{0}' and p.\"ProjectName\"='{1}'".format(loginName,Project_name)
+        
         ContainerName = keys['Bucket']
         cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
     
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
         
-
-        UserKey=results[1]
+        
         OrgName=results[0]
+        UserKey=results[1]
+        ProjectKey=results[2]
         
         cur=cnxn.cursor()
         file_name = os.path.basename(filePath)
 
-        #file_name1=file_name.split('.')
         query="select count(\"TableName\") from doppler.\"DopplerLake\" DL join doppler.\"DopplerUser\" US on DL.\"UserKey\"=US.\"UserKey\" where \"TableName\"="+"'"+file_name+"'"+" and US.\"LoginName\"="+"'"+loginName+"'"
+        print(query)
         cur.execute(query)
         results = cur.fetchone()
         if results[0]<1:
-            insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'','Uploaded')"
+
+            insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'"+str(ProjectKey)+"','Uploaded')"
             cur.execute(insert_query)
             cnxn.commit()
         else:
             pass
                     
         cur1=cnxn.cursor()
         insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM doppler.\"DopplerLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name+"'"
@@ -127,78 +140,100 @@
             maxlength = max(df[name].map(str).apply(len))
             tpp=str(maxlength)
             tp=str(dtype)
             insert1="INSERT INTO doppler.\"DopplerSchema\"(\"SourceKey\",\"Column\" ,\"Type\",\"Length\") VALUES ({},'{}','{}','{}')".format(SourceKey,name,tp,tpp)
             cur_sch.execute(insert1)
             cnxn.commit()
 
-
         ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type)
         update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type+"',\"Source\"= 'MLStudio' ,\"Status\"='Uploaded',\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
         cur2=cnxn.cursor()
 
         cur2.execute(update_query)
         cnxn.commit()
+        #print("uploaded")
 
         
-        if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
-
+        if Cloud =='AWS':
+            
             client.upload_file(filePath+'.'+file_type, ContainerName, ConnectionString)
-             # Generate a pre-signed URL        
+            # Generate a pre-signed URL        
             client.put_object_acl(ACL='public-read',
                               Bucket=ContainerName,
                               Key=ConnectionString)
-            
             url = f"s3://{ContainerName}/{ConnectionString}"
             print("uri : ",url)
-            cnxn.close()
-            #print("done")
+        elif Cloud == 'MinIO':
+            client.upload_file(filePath+'.'+file_type, ContainerName, ConnectionString)
+            # Generate a pre-signed URL
+            endpoint_url=keys['endpoint_url']
+            presigned_url = client.generate_presigned_url(
+                'get_object',
+                Params={
+                    'Bucket': ContainerName,
+                    'Key': ConnectionString
+                },
+                ExpiresIn=3600  # URL expiration time in seconds (e.g., 1 hour)
+            )
+            url = f"http://{endpoint_url}:9000/{ContainerName}/{ConnectionString}"            
+            print("uri : ",url)
         else:
             #print(keys['Cloud'])
             blob_client = client.get_blob_client(container=ContainerName, blob=file_name)
             with open(filePath+'.'+file_type, "rb") as data:
                 blob_client.upload_blob(data)
             
+        cnxn.close()
+        api=f"http://{api}/Workflow/WorkflowDruidSave?SourceID="+(str(SourceKey).lstrip())
+        response=requests.get(api,verify=False)
+        fapi=f"http://{fapi}/Profiling/?sourcekey="+(str(SourceKey).lstrip())
+        response=requests.get(fapi,verify=False)
+       
+
+        
+            
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
             sys.exit()
         else:
             print("Error : ",error)
 
 
+
 def getWorkspaceFile(fileName,destination,loginName,de_key):
     try:
 
         def is_file_name_same(file_path, expected_file_name):
             file_name = os.path.basename(file_path)
             return file_name == expected_file_name
 
         keys,db,client=decrypt_keys(de_key)
         
         query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
         ContainerName = keys['Bucket']
+        Cloud=keys['Cloud']
         cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
         UserKey=results[1]
         OrgName=results[0]
         folder_prefix = OrgName+'/'+loginName.upper()+'/'
         # Check if the file exists
         if os.path.exists(destination):
             print('folder exists')
         else:
             os.mkdir(destination)
-        if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
+        if Cloud == 'MinIO'or Cloud =='AWS':
             response = client.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
             destination=destination+'/'+fileName
             for obj in response['Contents']:
-                key = obj['Key']
+                key = obj['Key']               
                 is_same = is_file_name_same(key, fileName)
                 if(is_same):                
                     client.download_file(ContainerName, key, destination)
                     print("download")
         else:
             container_client = client.get_container_client(ContainerName)
 
@@ -216,41 +251,39 @@
                         
     except Exception as error:
         print("Error : ",error)
 
 def getWorkspaceFolderFiles(folder,destination,loginName,de_key):
     try:
         keys,db,client=decrypt_keys(de_key)
-        query="select DOR.\"OrgName\",Du.\"UserKey\",DL.\"ConnectionString\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" join doppler.\"DopplerLake\" DL on DL.\"UserKey\"=Du.\"UserKey\" where Du.\"LoginName\"="+"'"+loginName+"'"+" and \"TableName\"='"+folder+"'"
+        print(keys,db,client)
+        query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
         cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
         UserKey=results[1]
         OrgName=results[0]
-        folder_prefix = results[2]
-        folder_prefix=folder_prefix.replace('/'+folder,'')
+        folder_prefix = OrgName+'/'+loginName.upper()+'/'+folder
         ContainerName = keys['Bucket']
-        if os.path.exists(destination):
-            print('folder exists')
-        else:
-            os.mkdir(destination)
-        if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
+        Cloud=keys['Cloud']
+        if Cloud == 'MinIO'or Cloud =='AWS':
             response = client.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
             for obj in response['Contents']:
                 key = obj['Key']
                 if not key.endswith('/'):  # Exclude subdirectories
                     file_name = os.path.join(destination, os.path.basename(key))
                     client.download_file(ContainerName, key, file_name)  # Download the file
             print("downloaded")
         else:
             
             folder_prefix = OrgName+'/'+loginName.upper()+'/'+folder
             container_client = client.get_container_client(ContainerName)
             blobs = container_client.list_blobs(name_starts_with=folder_prefix)
+
             for blob in blobs:
                 blob_client = container_client.get_blob_client(blob.name)
                 file_path = os.path.join(destination, os.path.basename(blob.name))
                 os.makedirs(os.path.dirname(file_path), exist_ok=True)
                 with open(file_path, "wb") as file:
                     file.write(blob_client.download_blob().readall())
             print("downloaded")
```

## Comparing `dopplrSDK-3.1.0.dist-info/LICENSE.txt` & `dopplrSDK-3.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-3.1.0.dist-info/METADATA` & `dopplrSDK-3.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 3.1.0
+Version: 3.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

