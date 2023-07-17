# Comparing `tmp/evilHunter-0.2.1.tar.gz` & `tmp/evilHunter-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.2.1.tar", last modified: Mon Jul 17 14:42:48 2023, max compression
+gzip compressed data, was "evilHunter-0.2a0.tar", last modified: Fri Jul 14 14:30:56 2023, max compression
```

## Comparing `evilHunter-0.2.1.tar` & `evilHunter-0.2a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:42:48.678203 evilHunter-0.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:42:48.678203 evilHunter-0.2.1/C/
--rw-r--r--   0 root         (0) root         (0)     8001 2023-07-17 14:32:18.000000 evilHunter-0.2.1/C/evilCracker.c
--rw-r--r--   0 root         (0) root         (0)     3585 2023-07-17 14:42:48.678203 evilHunter-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3355 2023-07-14 14:26:38.000000 evilHunter-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)     4127 2023-07-12 16:38:26.000000 evilHunter-0.2.1/evilCracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:42:48.678203 evilHunter-0.2.1/evilHunter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3585 2023-07-17 14:42:48.000000 evilHunter-0.2.1/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-07-17 14:42:48.000000 evilHunter-0.2.1/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 14:42:48.000000 evilHunter-0.2.1/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-17 14:42:48.000000 evilHunter-0.2.1/evilHunter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 14:42:48.000000 evilHunter-0.2.1/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    34010 2023-07-14 14:24:21.000000 evilHunter-0.2.1/evilHunter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 14:42:48.678203 evilHunter-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      591 2023-07-17 14:41:55.000000 evilHunter-0.2.1/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:30:56.328653 evilHunter-0.2a0/
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:30:56.324653 evilHunter-0.2a0/C/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     7467 2023-07-14 14:25:30.000000 evilHunter-0.2a0/C/evilCracker.c
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3585 2023-07-14 14:30:56.328653 evilHunter-0.2a0/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3355 2023-07-14 14:26:38.000000 evilHunter-0.2a0/README.md
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     4127 2023-07-12 16:38:26.000000 evilHunter-0.2a0/evilCracker.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:30:56.328653 evilHunter-0.2a0/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3585 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      232 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       14 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        8 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    34010 2023-07-14 14:24:21.000000 evilHunter-0.2a0/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-07-14 14:30:56.328653 evilHunter-0.2a0/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      590 2023-07-14 14:09:14.000000 evilHunter-0.2a0/setup.py
```

### Comparing `evilHunter-0.2.1/C/evilCracker.c` & `evilHunter-0.2a0/C/evilCracker.c`

 * *Files 7% similar despite different names*

```diff
@@ -71,16 +71,14 @@
 
 int generate_random_length() {
     int passwd_length = (rand() % 13) + 8;
     return passwd_length;
 }
 
 long try = 0;
-bool password_found = false;  // Variable compartida que indica si se encontró la contraseña
-pthread_mutex_t lock;  // Mutex para sincronización
 
 char* generate_random_password(char letts[], int size, int long_passwd) {
     char* passwd = (char*)malloc((long_passwd + 1) * sizeof(char));
     for (int i = 0; i < long_passwd; ++i) {
         int position = rand() % size;
         passwd[i] = letts[position];
     }
@@ -91,15 +89,15 @@
 
 char* decrypt_packets(const char* password, const char* network_to_attack, const char* file) {
     char command[300];
     snprintf(command, sizeof(command), "airdecap-ng -p %s -e %s %s", password, network_to_attack, file);
 
     FILE* fp = popen(command, "r");
     if (fp == NULL) {
-        fprintf(stderr, "\n\nError occurred while try to decrypt\n");
+        fprintf(stderr, "Error occurred while executing command\n");
         exit(1);
     }
 
     // Descartar las primeras 7 líneas
     char buffer[100];
     for (int i = 0; i < 7; i++) {
         fgets(buffer, sizeof(buffer), fp);
@@ -159,103 +157,95 @@
         // lo demás
     } else {
         regfree(&regex);
         return 0;
     }
 }
 
+bool password_found = false;  // Variable compartida que indica si se encontró la contraseña
+pthread_mutex_t lock;  // Mutex para sincronización
+
 void* generate_passwords(void* arg) {
 
     //Arrgelamos argumentos
     ThreadArguments* args = (ThreadArguments*)arg;
     int char_of_passwd = args->char_of_passwd;
     const char* network_to_attack = args->network_to_attack;
     const char* file = args->file;
 
-    srand(time(NULL));
+    srand((unsigned)time(NULL));
 
-    char letters[] = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";
-    int letters_size = sizeof(letters) - 1;
+    char letters[] = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ";
+    int digits[] = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9};
+    int letters_size = sizeof(letters) / sizeof(letters[0]);
 
     Node* passwordsList;
     initialize_password_list(&passwordsList);
 
-    int size = char_of_passwd;
-    bool random_length;
+    char* password; 
+    int size = 0;
 
-    if (char_of_passwd == 0) {
-        random_length = true;
-    }
-    
     while (!password_found) {
-        if(random_length)
-            size = (rand() % 13) + 8;        
 
-        char* password = password = generate_random_password(letters, letters_size, size);
+        if (char_of_passwd == 0) {
+            size = generate_random_length(); 
+        } else {
+            size = char_of_passwd;
+        }
 
-        if(try == 10000)
-            strcpy(password, "18AC98B6E9C35FC23BA5");
-            
-        pthread_mutex_lock(&lock); // Bloqueamos el mutex para evitar acceso simultáneo a password_found
-        if (!password_found && !is_password_used(password, passwordsList)) {
+        password = generate_random_password(letters, letters_size, size);
+
+        if (!is_password_used(password, passwordsList)) {
             add_password(password, &passwordsList);
-            pthread_mutex_unlock(&lock);
 
-            char* result = decrypt_packets(password, network_to_attack, file); 
+            char* result = decrypt_packets(password, network_to_attack, file);
+             
             int comprobe = confirm_packets(result);
-            free(result);
 
             if (comprobe > 0) { 
-                pthread_mutex_lock(&lock); // Bloqueamos el mutex para evitar acceso simultáneo a password_found
-                if (!password_found)
-                    password_found = true; 
-
+                password_found = true;       // Establecer el estado de la variable compartida 
+                
                 //mostramos contraseña
                 printf("\n\n\t\t%s[!]%s PASSWORD FOUND%s -----> %s%s%s", y, b, y, r, password, end);
                 printf("\n\t\t%s[*]%s Decrypted Packets%s -----> %d %s\n\n", y, b, y, comprobe, end);
 
                 //Liberamos memoria
+                free(result);
                 free_password_list(&passwordsList);
-                pthread_mutex_unlock(&lock); // Desbloqueamos el mutex
-                free(password); 
-                break;
-                
+                return NULL;
             }
 
-            printf("\t%s[♦] Attempt:%s %ld     \t%sPASSWD: %s%s\r", y, b, try, y, b,password);
+            printf("\t%s[♦] Attempt:%s %ld     \t%sPASSWD:%s%s\r", y, b, try, y, b,password);
             try++;
             
         }
 
+        free(password);
     }
-    return NULL;
+
+    free_password_list(&passwordsList);
 }
 
 int init_crack_cap(int large, char* network_to_attack, char* file, int threads){
     //Variables para iniciar
     pthread_t thread_ids[threads]; 
     ThreadArguments args;
     args.char_of_passwd = large;
     args.network_to_attack = network_to_attack;
     args.file = file;
  
-    pthread_mutex_init(&lock, NULL); // Inicializamos el mutex
-    
-    //Creamos hilos
+
     for(int i = 0; i < threads; i++) {
         pthread_create(&thread_ids[i], NULL, generate_passwords, (void*)&args);
     }
 
-    // Esperamos a que terminen
     for (int i = 0; i < threads; i++){
         pthread_join(thread_ids[i], NULL);
     }
 
-    pthread_mutex_destroy(&lock); // Destruimos el mutex
-
     return 0;
 }
 
 int main() {
     //Varibles necesarias
     int char_of_passwd = 0;
     int threads = 500;
```

### Comparing `evilHunter-0.2.1/PKG-INFO` & `evilHunter-0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.2.1
+Version: 0.2a0
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.2.1/README.md` & `evilHunter-0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `evilHunter-0.2.1/evilCracker.py` & `evilHunter-0.2a0/evilCracker.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.2.1/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.2a0/evilHunter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.2.1
+Version: 0.2a0
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.2.1/evilHunter.py` & `evilHunter-0.2a0/evilHunter.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.2.1/setup.py` & `evilHunter-0.2a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.2.1",
+    version="0.2a",
     description="Cracking WiFi(KCRACK)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words", "C"],
```

