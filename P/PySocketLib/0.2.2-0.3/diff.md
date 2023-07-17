# Comparing `tmp/PySocketLib-0.2.2.tar.gz` & `tmp/PySocketLib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySocketLib-0.2.2.tar", last modified: Sat Jun 10 15:05:21 2023, max compression
+gzip compressed data, was "PySocketLib-0.3.tar", last modified: Mon Jul 17 11:18:43 2023, max compression
```

## Comparing `PySocketLib-0.2.2.tar` & `PySocketLib-0.3.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.779314 PySocketLib-0.2.2/
--rw-rw-r--   0 igors     (1000) igors     (1000)     1069 2023-06-10 09:19:23.000000 PySocketLib-0.2.2/LICENSE
--rw-rw-r--   0 igors     (1000) igors     (1000)      966 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)      439 2023-06-10 15:03:43.000000 PySocketLib-0.2.2/README.md
--rw-rw-r--   0 igors     (1000) igors     (1000)      511 2023-06-10 15:04:25.000000 PySocketLib-0.2.2/pyproject.toml
--rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-06-10 15:05:21.779314 PySocketLib-0.2.2/setup.cfg
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/
--rw-rw-r--   0 igors     (1000) igors     (1000)      409 2023-06-10 14:30:53.000000 PySocketLib-0.2.2/src/ExampleClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)     1143 2023-06-10 14:30:45.000000 PySocketLib-0.2.2/src/ExampleServer.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/CExceptions/
--rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.2.2/src/PySocketLib/CExceptions/InitExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       74 2023-06-05 14:38:04.000000 PySocketLib-0.2.2/src/PySocketLib/CExceptions/ProtocolExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       61 2023-06-03 17:39:57.000000 PySocketLib-0.2.2/src/PySocketLib/CExceptions/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/Client/
--rw-rw-r--   0 igors     (1000) igors     (1000)      964 2023-06-10 14:30:50.000000 PySocketLib-0.2.2/src/PySocketLib/Client/Client.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      214 2023-06-02 19:35:46.000000 PySocketLib-0.2.2/src/PySocketLib/Client/ConnectedClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       71 2023-06-03 13:07:20.000000 PySocketLib-0.2.2/src/PySocketLib/Client/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib/Server/
--rw-rw-r--   0 igors     (1000) igors     (1000)     3126 2023-06-10 14:30:39.000000 PySocketLib-0.2.2/src/PySocketLib/Server/Server.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      773 2023-06-10 14:31:48.000000 PySocketLib-0.2.2/src/PySocketLib/Server/TCPServer.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       59 2023-06-03 13:06:22.000000 PySocketLib-0.2.2/src/PySocketLib/Server/__init__.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       67 2023-06-10 06:43:20.000000 PySocketLib-0.2.2/src/PySocketLib/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-06-10 15:05:21.775314 PySocketLib-0.2.2/src/PySocketLib.egg-info/
--rw-rw-r--   0 igors     (1000) igors     (1000)      966 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)      608 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/SOURCES.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/dependency_links.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)       40 2023-06-10 15:05:21.000000 PySocketLib-0.2.2/src/PySocketLib.egg-info/top_level.txt
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1070 2023-07-17 11:03:51.000000 PySocketLib-0.3/LICENSE
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1145 2023-07-17 11:18:43.216003 PySocketLib-0.3/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      621 2023-07-17 11:16:00.000000 PySocketLib-0.3/README.md
+-rw-rw-r--   0 igors     (1000) igors     (1000)      509 2023-07-17 11:03:17.000000 PySocketLib-0.3/pyproject.toml
+-rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-07-17 11:18:43.216003 PySocketLib-0.3/setup.cfg
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      351 2023-07-17 10:27:23.000000 PySocketLib-0.3/src/ExampleClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      537 2023-07-17 09:50:41.000000 PySocketLib-0.3/src/ExampleServer.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/PySocketLib/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/PySocketLib/CExceptions/
+-rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/InitExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       37 2023-07-15 13:04:00.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/ProtocolExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       95 2023-07-17 09:15:35.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/RunTime.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       83 2023-07-16 12:01:42.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Client/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      674 2023-07-16 12:30:42.000000 PySocketLib-0.3/src/PySocketLib/Client/Client.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      438 2023-07-16 06:23:18.000000 PySocketLib-0.3/src/PySocketLib/Client/ConnectedClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1411 2023-07-16 12:34:03.000000 PySocketLib-0.3/src/PySocketLib/Client/TCPClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1507 2023-07-17 10:43:54.000000 PySocketLib-0.3/src/PySocketLib/Client/UDPClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      177 2023-06-11 13:47:22.000000 PySocketLib-0.3/src/PySocketLib/Client/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Server/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     4069 2023-07-17 09:50:52.000000 PySocketLib-0.3/src/PySocketLib/Server/Server.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3518 2023-07-17 09:51:12.000000 PySocketLib-0.3/src/PySocketLib/Server/TCPServer.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     2504 2023-07-17 10:44:38.000000 PySocketLib-0.3/src/PySocketLib/Server/UDPServer.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       92 2023-07-15 14:41:30.000000 PySocketLib-0.3/src/PySocketLib/Server/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Utility/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Utility/Protocol/
+-rw-rw-r--   0 igors     (1000) igors     (1000)       68 2023-06-11 12:59:17.000000 PySocketLib-0.3/src/PySocketLib/Utility/Protocol/Protocol.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       30 2023-06-11 12:28:03.000000 PySocketLib-0.3/src/PySocketLib/Utility/Protocol/__init__.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       22 2023-06-11 12:28:52.000000 PySocketLib-0.3/src/PySocketLib/Utility/__init__.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       89 2023-06-11 12:28:40.000000 PySocketLib-0.3/src/PySocketLib/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/PySocketLib.egg-info/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1145 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      881 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/SOURCES.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/dependency_links.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)       40 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/top_level.txt
```

### Comparing `PySocketLib-0.2.2/LICENSE` & `PySocketLib-0.3/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

