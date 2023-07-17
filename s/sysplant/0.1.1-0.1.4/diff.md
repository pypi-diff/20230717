# Comparing `tmp/sysplant-0.1.1.tar.gz` & `tmp/sysplant-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysplant-0.1.1.tar", max compression
+gzip compressed data, was "sysplant-0.1.4.tar", max compression
```

## Comparing `sysplant-0.1.1.tar` & `sysplant-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1075 2023-07-16 15:31:01.935550 sysplant-0.1.1/LICENSE
--rw-r--r--   0        0        0     8634 2023-07-16 15:31:01.935550 sysplant-0.1.1/README.md
--rw-r--r--   0        0        0      864 2023-07-16 15:31:01.939550 sysplant-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/abstracts/__init__.py
--rw-r--r--   0        0        0     3492 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/abstracts/abstractFactory.py
--rw-r--r--   0        0        0     1814 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/abstracts/abstractGenerator.py
--rw-r--r--   0        0        0     3820 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/constants/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/constants/sysplantConstants.py
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/data/__init__.py
--rw-r--r--   0        0        0    43189 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/data/definitions.json
--rw-r--r--   0        0        0   332144 2023-07-16 15:31:01.939550 sysplant-0.1.1/sysplant/data/prototypes.json
--rw-r--r--   0        0        0   431123 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/data/windef.nim
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/managers/__init__.py
--rw-r--r--   0        0        0    11814 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/managers/nimGenerator.py
--rw-r--r--   0        0        0    12756 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/managers/templateManager.py
--rw-r--r--   0        0        0     6206 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/sysplant.py
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/__init__.py
--rw-r--r--   0        0        0     3018 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/base.nim
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/iterators/__init__.py
--rw-r--r--   0        0        0     3359 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/iterators/canterlot.nim
--rw-r--r--   0        0        0     2698 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/iterators/freshy.nim
--rw-r--r--   0        0        0     4461 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/iterators/halo.nim
--rw-r--r--   0        0        0     3414 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/iterators/hell.nim
--rw-r--r--   0        0        0     2561 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/iterators/syswhispers.nim
--rw-r--r--   0        0        0     4527 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/iterators/tartarus.nim
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/resolvers/__init__.py
--rw-r--r--   0        0        0       99 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/resolvers/basic.nim
--rw-r--r--   0        0        0      229 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/resolvers/random.nim
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/stubs/__init__.py
--rw-r--r--   0        0        0      509 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/stubs/direct_x64.nim
--rw-r--r--   0        0        0      568 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/templates/stubs/indirect_x64.nim
--rw-r--r--   0        0        0        0 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/utils/__init__.py
--rw-r--r--   0        0        0     3474 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/utils/loggerSingleton.py
--rw-r--r--   0        0        0      261 2023-07-16 15:31:01.943550 sysplant-0.1.1/sysplant/utils/singleton.py
--rw-r--r--   0        0        0     9171 1970-01-01 00:00:00.000000 sysplant-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-17 14:43:14.455687 sysplant-0.1.4/LICENSE
+-rw-r--r--   0        0        0     9545 2023-07-17 14:43:14.455687 sysplant-0.1.4/README.md
+-rw-r--r--   0        0        0      864 2023-07-17 14:43:14.459687 sysplant-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/abstracts/__init__.py
+-rw-r--r--   0        0        0     3492 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/abstracts/abstractFactory.py
+-rw-r--r--   0        0        0     1998 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/abstracts/abstractGenerator.py
+-rw-r--r--   0        0        0     3820 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/constants/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/constants/sysplantConstants.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/data/__init__.py
+-rw-r--r--   0        0        0    44046 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/data/definitions.json
+-rw-r--r--   0        0        0   332144 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/data/prototypes.json
+-rw-r--r--   0        0        0   431123 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/data/windef.nim
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/managers/__init__.py
+-rw-r--r--   0        0        0    12333 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/managers/nimGenerator.py
+-rw-r--r--   0        0        0    12756 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/managers/templateManager.py
+-rw-r--r--   0        0        0     6210 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/sysplant.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/__init__.py
+-rw-r--r--   0        0        0     3018 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/base.nim
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/__init__.py
+-rw-r--r--   0        0        0     3359 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/canterlot.nim
+-rw-r--r--   0        0        0     2698 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/freshy.nim
+-rw-r--r--   0        0        0     4461 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/halo.nim
+-rw-r--r--   0        0        0     3414 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/hell.nim
+-rw-r--r--   0        0        0     2561 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/syswhispers.nim
+-rw-r--r--   0        0        0     4527 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/tartarus.nim
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/resolvers/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/resolvers/basic.nim
+-rw-r--r--   0        0        0      229 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/resolvers/random.nim
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/stubs/__init__.py
+-rw-r--r--   0        0        0      509 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/stubs/direct_x64.nim
+-rw-r--r--   0        0        0      568 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/stubs/indirect_x64.nim
+-rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/utils/__init__.py
+-rw-r--r--   0        0        0     3474 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/utils/loggerSingleton.py
+-rw-r--r--   0        0        0      261 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/utils/singleton.py
+-rw-r--r--   0        0        0    10082 1970-01-01 00:00:00.000000 sysplant-0.1.4/PKG-INFO
```

### Comparing `sysplant-0.1.1/LICENSE` & `sysplant-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/README.md` & `sysplant-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,55 @@
-# SysPlant
-#### "Your Syscall Factory" *(feat. Canterlot's Gate)*
+<!-- markdownlint-disable MD033 MD041 -->
+<h1 align="center">
+..:: SysPlant ::..
+</h1>
+
+<p align="center">
+  <strong>Your Syscall Factory</strong> <i>(feat. Canterlot's Gate)</i>
+</p>
+
+<p align="center">
+  <img src="docs/assets/canterlot.jpeg" alt="Canterlot's Gate"/>
+</p>
+
+[![PyPI version](https://img.shields.io/pypi/v/sysplant.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/sysplant/)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/sysplant.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/sysplant/)
+[![Build Status](https://github.com/x42en/sysplant/actions/workflows/build.yml/badge.svg)](https://github.com/x42en/sysplant)
+[![Project Licence](https://img.shields.io/github/license/x42en/sysplant.svg)](https://github.com/x42en/sysplant/blob/main/LICENSE)
+[![PyPI downloads](https://img.shields.io/pypi/dm/sysplant.svg)](https://pypistats.org/packages/sysplant)
+[![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
-![Canterlot's Gate](docs/assets/canterlot.jpeg)
 
 SysPlant is a small implementation in NIM of the currently known syscall hooking methods. It currently supports following gates:
-- [Hell's Gate](https://github.com/am0nsec/HellsGate) : Lookup syscall by first opcodes
-- [Halos's Gate](https://blog.sektor7.net/#!res/2021/halosgate.md) : Lookup syscall by first opcodes and search nearby if first instruction is a JMP
-- [Tartarus' Gate](https://github.com/trickster0/TartarusGate) : Lookup syscall by first opcodes and search nearby if first or third instruction is a JMP
-- [FreshyCalls](https://github.com/crummie5/FreshyCalls) : Lookup syscall by name (start with Nt and not Ntdll), sort addresses to retrieve syscall number
-- [SysWhispers2](https://github.com/jthuraisamy/SysWhispers2) : Lookup syscall by name (start with Zw), sort addresses to retrieve syscall number
-- **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect padding to syscall instruction for random jumps.
-- **Custom** Allows you to choose a generation method, a syscall resolver (basic / random) and a syscall stub (direct / indirect). **Careful: some combinations means nothing so it won't work (eg: freshy iterator + random resolver + indirect stub => as Freshy return back the syscall stub entry address, your syscall number will be rewrite by a random one)**  
+  - [Hell's Gate](https://github.com/am0nsec/HellsGate) : Lookup syscall by first opcodes
+  - [Halos's Gate](https://blog.sektor7.net/#!res/2021/halosgate.md) : Lookup syscall by first opcodes and search nearby if first instruction is a JMP
+  - [Tartarus' Gate](https://github.com/trickster0/TartarusGate) : Lookup syscall by first opcodes and search nearby if first or third instruction is a JMP
+  - [FreshyCalls](https://github.com/crummie5/FreshyCalls) : Lookup syscall by name (start with Nt and not Ntdll), sort addresses to retrieve syscall number
+  - [SysWhispers2](https://github.com/jthuraisamy/SysWhispers2) : Lookup syscall by name (start with Zw), sort addresses to retrieve syscall number
+  - **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect padding to syscall instruction for random jumps.
+  - **Custom** Allows you to choose a generation method, a syscall resolver (basic / random) and a syscall stub (direct / indirect). **Careful: some combinations means nothing so it won't work (eg: freshy iterator + random resolver + indirect stub => as Freshy return back the syscall stub entry address, your syscall number will be rewrite by a random one)**  
 
 *Note: You can also generate your own combinations using the proper options... But be careful some options might not work or even make sense*
 
 > :warning: **DISCLAIMER**
 > Please only use this tool on systems you have permission to access.
 > Usage is restricted to Pentesting or Education only.
 > All credits are based on my own research, please feel free to claim any method if I made mistakes...
 
-![pipeline status](https://code.prohacktive.io/bmz/syswhispers3/badges/master/pipeline.svg)
-
----
-- Created at: 01/07/2023
-- Updated at: 16/07/2023
-- Version: 0.1.1
-
 ---
 
 ## Introduction
 This personal project aims to be a simple tool to better understand & generate different syscall retrieval methods, and being able to play with direct / indirect syscall stub. The first goal was to get my hands into NIM and then it overflow :wink: ...  
 SysPlant has been developped for Linux users, some stuff might be broken within Windows or Mac. PR are welcome if you found anything that does not work as expected.
 
 ## Installation
-This is a python project that will generate NIM source code (bit weird hu ?! :grin:). So you can use it inside your python project as an external module or directly on your device as a tool.
+
+> _Requirements: Pyton 3.8+_
+
+This is a python project that will generate NIM/C/etc... source code (bit weird hu ?! :grin:). So you can use it inside your python project as an external module or directly on your device as a tool.
 
 ### As a Python module
 If you are using standard pip3 package manager
 ```sh
 pip3 install sysplant
 ```
 
@@ -168,32 +180,35 @@
 #### Custom generation
 ```bash
 $ ./main.py generate -o syscall.nim custom -i canterlot -r random -s indirect
 ```
 
 ## Example
 A simple example (launching calc.exe) is accessible using `inject.nim`.  
-1. Be sure to install [winim](https://github.com/khchen/winim) library first: `nimble install winim`
-2. Generate the `syscall.nim` file with `./main.py -o example/syscall.nim canterlot`
-3. Compile the injection template file with `nim c -d=release -d=danger -d=strip --opt=size -d=mingw --app=console --cpu=amd64 --out=app.exe example/inject.nim` on Linux (be sure to have mingw installed)
-4. Copy the `app.exe` generated on your Windows device.
+  1. Be sure to install [winim](https://github.com/khchen/winim) library first: `nimble install winim`
+  2. Generate the `syscall.nim` file with `./main.py -o example/syscall.nim canterlot`
+  3. Compile the injection template file with `nim c -d=release -d=danger -d=strip --opt=size -d=mingw --app=console --cpu=amd64 --out=app.exe example/inject.nim` on Linux (be sure to have mingw installed)
+  4. Copy the `app.exe` generated on your Windows device.
 
 Happy Hacking :beach: !
 
 ## Credits
 Massive shout-out to these useful projects that helps me during this journey, or individuals for their reviews
-- [@alice blogpost about syscalls techniques](https://alice.climent-pommeret.red/posts/direct-syscalls-hells-halos-syswhispers2/)
-- [@redops blogpost about direct vs indirect syscalls](https://redops.at/en/blog/direct-syscalls-a-journey-from-high-to-low)
-- [@Jackson_T & @modexpblog for Syswhispers2](https://github.com/jthuraisamy/SysWhispers2)
-- [@klezvirus for syswhispers3](https://github.com/klezVirus/SysWhispers3)
+  - [@alice blogpost about syscalls techniques](https://alice.climent-pommeret.red/posts/direct-syscalls-hells-halos-syswhispers2/)
+  - [@redops blogpost about direct vs indirect syscalls](https://redops.at/en/blog/direct-syscalls-a-journey-from-high-to-low)
+  - [@Jackson_T & @modexpblog for Syswhispers2](https://github.com/jthuraisamy/SysWhispers2)
+  - [@klezvirus for syswhispers3](https://github.com/klezVirus/SysWhispers3)
 
 ## :construction: TODO
 This project is really in WIP state...  
 Some PR & reviews are more than welcome :tada: !
-- [x] Add internal names randomization
-- [ ] Add x86 support
-- [ ] Add WoW64 support
-- [-] Add some tests
-- [x] Setup documentation
+  - [x] Add internal names randomization
+  - [x] Setup documentation
+  - [-] Add some tests
+  - [ ] Add x86 support
+  - [ ] Add WoW64 support
+  - [ ] Setup C templates
+  - [ ] Setup Go templates
+  - [ ] Setup Rust? templates
 
 ## License
-This project is licensed under the [MIT License](https://www.tldrlegal.com/license/mit-license), for individuals only. If you want to integrate this work in your commercial project please contact me through `0x42en[at]gmail.com`
+This project is licensed under the [MIT License](https://www.tldrlegal.com/license/mit-license), for individuals only. If you want to integrate this work in your commercial project please contact me through `0x42en[at]gmail.com`
```

### Comparing `sysplant-0.1.1/pyproject.toml` & `sysplant-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sysplant"
-version = "0.1.1"
+version = "0.1.4"
 description = "SysPlant - Your syscall factory"
 authors = ["Ben Mz <x42en@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sysplant-0.1.1/sysplant/abstracts/abstractFactory.py` & `sysplant-0.1.4/sysplant/abstracts/abstractFactory.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/abstracts/abstractGenerator.py` & `sysplant-0.1.4/sysplant/abstracts/abstractGenerator.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,23 @@
 
     def __init__(self, log_level: int = logging.INFO) -> None:
         super().__init__()
 
         # Share logger for all childs
         self.logger = LoggerSingleton(log_level)
 
-        # Store definitions already defined
-        self.type_defined = set()
+        # Store definitions to defined
+        self.type_set = set()
+        self.__generated = set()
+
+    def register_definition(self, name: str) -> None:
+        self.__generated.add(name)
+
+    def is_generated(self, name: str) -> bool:
+        return name in self.__generated
 
     @abstractmethod
     def generate_struct(self, name: str, definition: list) -> str:
         raise NotImplementedError("Structure generation not implemented yet")
 
     @abstractmethod
     def generate_union(self, name: str, definition: list) -> str:
@@ -37,15 +44,15 @@
         raise NotImplementedError("Standard var generation not implemented yet")
 
     @abstractmethod
     def generate_enum(self, name: str, definition: list) -> str:
         raise NotImplementedError("Enum generation not implemented yet")
 
     @abstractmethod
-    def generate_seed(self, name: str, definition: list) -> str:
+    def generate_seed(self, name: str) -> str:
         raise NotImplementedError("Seed generation not implemented yet")
 
     @abstractmethod
     def generate_stub(self, name: str, params: dict, fhash: int) -> str:
         raise NotImplementedError("Stub generation not implemented yet")
 
     @abstractmethod
```

### Comparing `sysplant-0.1.1/sysplant/constants/__init__.py` & `sysplant-0.1.4/sysplant/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/constants/sysplantConstants.py` & `sysplant-0.1.4/sysplant/constants/sysplantConstants.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/data/definitions.json` & `sysplant-0.1.4/sysplant/data/definitions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9505575117370894%*

 * *Differences: {"'ENCLAVE_ROUTINE'": "OrderedDict([('dependencies', []), ('type', 'standard'), ('definition', "*

 * *                      "['LPVOID'])])",*

 * * "'MEM_EXTENDED_PARAMETER'": "OrderedDict([('dependencies', ['MEM_EXTENDED_PARAMETER_TYPE', "*

 * *                             "'MEM_EXTENDED_PARAMETER_UNION']), ('type', 'struct'), ('definition', "*

 * *                             "[['MEM_EXTENDED_PARAMETER_TYPE', 'Type'], ['DWORD', 'Reserved'], "*

 * *                             "['MEM_EXTENDED_PARAMETER_UNION', 'u1']])])",*

 * * "'MEM_EX […]*

```diff
@@ -243,28 +243,14 @@
                 "WCHAR",
                 "HeadlessRedirection"
             ]
         ],
         "dependencies": [],
         "type": "struct"
     },
-    "CLIENT_ID": {
-        "definition": [
-            [
-                "HANDLE",
-                "UniqueProcess"
-            ],
-            [
-                "HANDLE",
-                "UniqueThread"
-            ]
-        ],
-        "dependencies": [],
-        "type": "struct"
-    },
     "DEBUGOBJECTINFOCLASS": {
         "definition": [
             "DebugObjectFlags = 1",
             "MaxDebugObjectInfoClass"
         ],
         "dependencies": [],
         "type": "enum"
@@ -341,14 +327,21 @@
                 "ULONG",
                 "DriverFilePathOffset"
             ]
         ],
         "dependencies": [],
         "type": "struct"
     },
+    "ENCLAVE_ROUTINE": {
+        "definition": [
+            "LPVOID"
+        ],
+        "dependencies": [],
+        "type": "standard"
+    },
     "EVENT_INFORMATION_CLASS": {
         "definition": [
             "EventBasicInformation"
         ],
         "dependencies": [],
         "type": "enum"
     },
@@ -964,27 +957,74 @@
             "MemoryReserveUserApc",
             "MemoryReserveIoCompletion",
             "MemoryReserveTypeMax"
         ],
         "dependencies": [],
         "type": "enum"
     },
+    "MEM_EXTENDED_PARAMETER": {
+        "definition": [
+            [
+                "MEM_EXTENDED_PARAMETER_TYPE",
+                "Type"
+            ],
+            [
+                "DWORD",
+                "Reserved"
+            ],
+            [
+                "MEM_EXTENDED_PARAMETER_UNION",
+                "u1"
+            ]
+        ],
+        "dependencies": [
+            "MEM_EXTENDED_PARAMETER_TYPE",
+            "MEM_EXTENDED_PARAMETER_UNION"
+        ],
+        "type": "struct"
+    },
     "MEM_EXTENDED_PARAMETER_TYPE": {
         "definition": [
-            "MemExtendedParameterInvalidType",
+            "MemExtendedParameterInvalidType = 0",
             "MemExtendedParameterAddressRequirements",
             "MemExtendedParameterNumaNode",
             "MemExtendedParameterPartitionHandle",
             "MemExtendedParameterUserPhysicalHandle",
             "MemExtendedParameterAttributeFlags",
             "MemExtendedParameterMax"
         ],
         "dependencies": [],
         "type": "enum"
     },
+    "MEM_EXTENDED_PARAMETER_UNION": {
+        "definition": [
+            [
+                "DWORD64",
+                "ULong64"
+            ],
+            [
+                "PVOID",
+                "Pointer"
+            ],
+            [
+                "SIZE_T",
+                "Size"
+            ],
+            [
+                "HANDLE",
+                "Handle"
+            ],
+            [
+                "DWORD",
+                "ULong"
+            ]
+        ],
+        "dependencies": [],
+        "type": "union"
+    },
     "MUTANT_INFORMATION_CLASS": {
         "definition": [
             "MutantBasicInformation",
             "MutantOwnerInformation"
         ],
         "dependencies": [],
         "type": "enum"
@@ -1028,14 +1068,32 @@
             "ObjectTypeInformation",
             "ObjectAllTypesInformation",
             "ObjectHandleInformation"
         ],
         "dependencies": [],
         "type": "enum"
     },
+    "PCWNF_STATE_NAME": {
+        "definition": [
+            "WNF_STATE_NAME"
+        ],
+        "dependencies": [
+            "WNF_STATE_NAME"
+        ],
+        "type": "pointer"
+    },
+    "PCWNF_TYPE_ID": {
+        "definition": [
+            "WNF_TYPE_ID"
+        ],
+        "dependencies": [
+            "WNF_TYPE_ID"
+        ],
+        "type": "pointer"
+    },
     "PIO_APC_ROUTINE": {
         "definition": [
             [
                 "PVOID",
                 "AppContext"
             ],
             [
@@ -2120,14 +2178,21 @@
     "SEMAPHORE_INFORMATION_CLASS": {
         "definition": [
             "SemaphoreBasicInformation"
         ],
         "dependencies": [],
         "type": "enum"
     },
+    "SE_SIGNING_LEVEL": {
+        "definition": [
+            "ULONG"
+        ],
+        "dependencies": [],
+        "type": "standard"
+    },
     "SHUTDOWN_ACTION": {
         "definition": [
             "ShutdownNoReboot",
             "ShutdownReboot",
             "ShutdownPowerOff"
         ],
         "dependencies": [],
```

### Comparing `sysplant-0.1.1/sysplant/data/prototypes.json` & `sysplant-0.1.4/sysplant/data/prototypes.json`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/data/windef.nim` & `sysplant-0.1.4/sysplant/data/windef.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/managers/nimGenerator.py` & `sysplant-0.1.4/sysplant/managers/nimGenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,20 +80,25 @@
             definition (list): Structure parameters from definitions.json
 
         Returns:
             str: NIM code for basic structure definition (except type keyword for definition chaining)
         """
         result = f"{SysPlantConstants.NIM_TAB}{name}* " + "{.pure.} = object\n"
         for var in definition:
-            if len(var) >= 2:
+            if len(var) == 2:
                 result += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]}: {var[0]}\n"
 
-            # I have not found how to initialize value in NIM type definitions...
-            # elif len(var) == 3:
-            #     result += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]}: {var[0]} = {var[2]}\n"
+            elif len(var) == 3:
+                result += (
+                    f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]} "
+                    + "{.bitsize: "
+                    + str(var[2])
+                    + ".}: "
+                    + f"{var[0]}\n"
+                )
         # Always add pointer
         result += f"{SysPlantConstants.NIM_TAB}P{name}* = ptr {name}\n"
 
         return result
 
     def generate_union(self, name: str, definition: list) -> str:
         """
@@ -109,15 +114,21 @@
             str: NIM code for union structure definition (except type keyword for definition chaining)
         """
         result = f"{SysPlantConstants.NIM_TAB}{name} " + "{.pure, union.} = object\n"
         for var in definition:
             if len(var) == 2:
                 result += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]}: {var[0]}\n"
             elif len(var) == 3:
-                result += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]}: {var[0]} = {var[2]}\n"
+                result += (
+                    f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]} "
+                    + "{.bitsize: "
+                    + var[2]
+                    + ".}: "
+                    + f"{var[0]}\n"
+                )
         # Always add pointer
         result += f"{SysPlantConstants.NIM_TAB}P{name} = ptr {name}\n"
 
         return result
 
     def generate_pointer(self, name: str, definition: list) -> str:
         """
@@ -212,15 +223,15 @@
         # Build function param declaration
         stub = f"proc {name}*("
         args = list()
 
         # Loop function params
         for p in params.get("params", []):
             # Register each type var
-            self.type_defined.add(p["type"])
+            self.type_set.add(p["type"])
             args.append(f"{p['name']}: {p['type']}")
 
         # Generate NIM proc parameters
         stub += ", ".join(args)
         stub += ") {.asmNoStackFrame.} =\n"
 
         # Append stub code
@@ -248,14 +259,17 @@
         """
         typedef_code = ""
         dependencies = entry.get("dependencies", [])
 
         # Resolve dependencies first
         if len(dependencies) > 0:
             for dep in dependencies:
+                # Avoid duplicate generation
+                if self.is_generated(dep):
+                    continue
                 # Avoid defining external types
                 if self.__definitions.get(dep) is not None:
                     typedef_code += self.__generate_typedefs(
                         dep, self.__definitions.get(dep)
                     )
 
         # Generate correct entry type
@@ -271,38 +285,46 @@
         elif type_ == "standard":
             typedef_code += self.generate_standard(name, entry.get("definition", []))
         elif type_ is None:
             raise NotImplementedError(f"Missing {name} type")
         else:
             raise NotImplementedError("Unsupported definition type")
 
+        # Register definitions generated
+        self.register_definition(name)
+
         return typedef_code
 
     def generate_definitions(self) -> str:
         """
         Public method used to generate all required definitions by hooked syscall.
         It will first loop through the required functions to hook, extract all parameters type to declare
         and call the private __generate_typedefs function to generate the associated code block.
         Once all chained it will return the complete code block to integrate in template
 
         Returns:
             str: NIM code for template integration
         """
         code = ""
-        for name in self.type_defined:
+        for name in self.type_set:
             # If Winim already share this structure
             if f"{name}*" in self.__winimdef:
                 continue
 
             entry = self.__definitions.get(name)
-            # Search for pointers
+
+            # Search pointer definition
             if entry is None:
                 name = name[1:]
                 entry = self.__definitions.get(name)
 
             # Still nothing... it might be a standard struct then
             if entry is None:
                 continue
 
+            # Avoid duplicate generation
+            if self.is_generated(name):
+                continue
+
             code += self.__generate_typedefs(name, entry)
 
         return code
```

### Comparing `sysplant-0.1.1/sysplant/managers/templateManager.py` & `sysplant-0.1.4/sysplant/managers/templateManager.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/sysplant.py` & `sysplant-0.1.4/sysplant/sysplant.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             syscalls = self.__engine.list_supported_syscalls()
         elif syscalls == "common":
             self.logger.info("\t. Common supported functions selected", stripped=True)
             syscalls = self.__engine.list_common_syscalls()
         elif syscalls == "donut":
             self.logger.info("\t. Donut functions selected", stripped=True)
             syscalls = self.__engine.list_donut_syscalls()
-        elif type(syscalls) is not list:
+        elif not isinstance(syscalls, list):
             raise ValueError("Unsupported functions type")
         else:
             self.logger.info("\t. Custom set of functions selected", stripped=True)
         self.__engine.generate_stubs(syscalls)
 
         return str(self.__engine)
```

### Comparing `sysplant-0.1.1/sysplant/templates/base.nim` & `sysplant-0.1.4/sysplant/templates/base.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/templates/iterators/canterlot.nim` & `sysplant-0.1.4/sysplant/templates/iterators/canterlot.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/templates/iterators/freshy.nim` & `sysplant-0.1.4/sysplant/templates/iterators/freshy.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/templates/iterators/halo.nim` & `sysplant-0.1.4/sysplant/templates/iterators/halo.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/templates/iterators/hell.nim` & `sysplant-0.1.4/sysplant/templates/iterators/hell.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/templates/iterators/syswhispers.nim` & `sysplant-0.1.4/sysplant/templates/iterators/syswhispers.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/templates/iterators/tartarus.nim` & `sysplant-0.1.4/sysplant/templates/iterators/tartarus.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/templates/stubs/indirect_x64.nim` & `sysplant-0.1.4/sysplant/templates/stubs/indirect_x64.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/sysplant/utils/loggerSingleton.py` & `sysplant-0.1.4/sysplant/utils/loggerSingleton.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.1/PKG-INFO` & `sysplant-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 Metadata-Version: 2.1
 Name: sysplant
-Version: 0.1.1
+Version: 0.1.4
 Summary: SysPlant - Your syscall factory
 License: MIT
 Author: Ben Mz
 Author-email: x42en@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-# SysPlant
-#### "Your Syscall Factory" *(feat. Canterlot's Gate)*
+<!-- markdownlint-disable MD033 MD041 -->
+<h1 align="center">
+..:: SysPlant ::..
+</h1>
+
+<p align="center">
+  <strong>Your Syscall Factory</strong> <i>(feat. Canterlot's Gate)</i>
+</p>
+
+<p align="center">
+  <img src="docs/assets/canterlot.jpeg" alt="Canterlot's Gate"/>
+</p>
+
+[![PyPI version](https://img.shields.io/pypi/v/sysplant.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/sysplant/)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/sysplant.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/sysplant/)
+[![Build Status](https://github.com/x42en/sysplant/actions/workflows/build.yml/badge.svg)](https://github.com/x42en/sysplant)
+[![Project Licence](https://img.shields.io/github/license/x42en/sysplant.svg)](https://github.com/x42en/sysplant/blob/main/LICENSE)
+[![PyPI downloads](https://img.shields.io/pypi/dm/sysplant.svg)](https://pypistats.org/packages/sysplant)
+[![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
-![Canterlot's Gate](docs/assets/canterlot.jpeg)
 
 SysPlant is a small implementation in NIM of the currently known syscall hooking methods. It currently supports following gates:
-- [Hell's Gate](https://github.com/am0nsec/HellsGate) : Lookup syscall by first opcodes
-- [Halos's Gate](https://blog.sektor7.net/#!res/2021/halosgate.md) : Lookup syscall by first opcodes and search nearby if first instruction is a JMP
-- [Tartarus' Gate](https://github.com/trickster0/TartarusGate) : Lookup syscall by first opcodes and search nearby if first or third instruction is a JMP
-- [FreshyCalls](https://github.com/crummie5/FreshyCalls) : Lookup syscall by name (start with Nt and not Ntdll), sort addresses to retrieve syscall number
-- [SysWhispers2](https://github.com/jthuraisamy/SysWhispers2) : Lookup syscall by name (start with Zw), sort addresses to retrieve syscall number
-- **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect padding to syscall instruction for random jumps.
-- **Custom** Allows you to choose a generation method, a syscall resolver (basic / random) and a syscall stub (direct / indirect). **Careful: some combinations means nothing so it won't work (eg: freshy iterator + random resolver + indirect stub => as Freshy return back the syscall stub entry address, your syscall number will be rewrite by a random one)**  
+  - [Hell's Gate](https://github.com/am0nsec/HellsGate) : Lookup syscall by first opcodes
+  - [Halos's Gate](https://blog.sektor7.net/#!res/2021/halosgate.md) : Lookup syscall by first opcodes and search nearby if first instruction is a JMP
+  - [Tartarus' Gate](https://github.com/trickster0/TartarusGate) : Lookup syscall by first opcodes and search nearby if first or third instruction is a JMP
+  - [FreshyCalls](https://github.com/crummie5/FreshyCalls) : Lookup syscall by name (start with Nt and not Ntdll), sort addresses to retrieve syscall number
+  - [SysWhispers2](https://github.com/jthuraisamy/SysWhispers2) : Lookup syscall by name (start with Zw), sort addresses to retrieve syscall number
+  - **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect padding to syscall instruction for random jumps.
+  - **Custom** Allows you to choose a generation method, a syscall resolver (basic / random) and a syscall stub (direct / indirect). **Careful: some combinations means nothing so it won't work (eg: freshy iterator + random resolver + indirect stub => as Freshy return back the syscall stub entry address, your syscall number will be rewrite by a random one)**  
 
 *Note: You can also generate your own combinations using the proper options... But be careful some options might not work or even make sense*
 
 > :warning: **DISCLAIMER**
 > Please only use this tool on systems you have permission to access.
 > Usage is restricted to Pentesting or Education only.
 > All credits are based on my own research, please feel free to claim any method if I made mistakes...
 
-![pipeline status](https://code.prohacktive.io/bmz/syswhispers3/badges/master/pipeline.svg)
-
----
-- Created at: 01/07/2023
-- Updated at: 16/07/2023
-- Version: 0.1.1
-
 ---
 
 ## Introduction
 This personal project aims to be a simple tool to better understand & generate different syscall retrieval methods, and being able to play with direct / indirect syscall stub. The first goal was to get my hands into NIM and then it overflow :wink: ...  
 SysPlant has been developped for Linux users, some stuff might be broken within Windows or Mac. PR are welcome if you found anything that does not work as expected.
 
 ## Installation
-This is a python project that will generate NIM source code (bit weird hu ?! :grin:). So you can use it inside your python project as an external module or directly on your device as a tool.
+
+> _Requirements: Pyton 3.8+_
+
+This is a python project that will generate NIM/C/etc... source code (bit weird hu ?! :grin:). So you can use it inside your python project as an external module or directly on your device as a tool.
 
 ### As a Python module
 If you are using standard pip3 package manager
 ```sh
 pip3 install sysplant
 ```
 
@@ -184,32 +196,36 @@
 #### Custom generation
 ```bash
 $ ./main.py generate -o syscall.nim custom -i canterlot -r random -s indirect
 ```
 
 ## Example
 A simple example (launching calc.exe) is accessible using `inject.nim`.  
-1. Be sure to install [winim](https://github.com/khchen/winim) library first: `nimble install winim`
-2. Generate the `syscall.nim` file with `./main.py -o example/syscall.nim canterlot`
-3. Compile the injection template file with `nim c -d=release -d=danger -d=strip --opt=size -d=mingw --app=console --cpu=amd64 --out=app.exe example/inject.nim` on Linux (be sure to have mingw installed)
-4. Copy the `app.exe` generated on your Windows device.
+  1. Be sure to install [winim](https://github.com/khchen/winim) library first: `nimble install winim`
+  2. Generate the `syscall.nim` file with `./main.py -o example/syscall.nim canterlot`
+  3. Compile the injection template file with `nim c -d=release -d=danger -d=strip --opt=size -d=mingw --app=console --cpu=amd64 --out=app.exe example/inject.nim` on Linux (be sure to have mingw installed)
+  4. Copy the `app.exe` generated on your Windows device.
 
 Happy Hacking :beach: !
 
 ## Credits
 Massive shout-out to these useful projects that helps me during this journey, or individuals for their reviews
-- [@alice blogpost about syscalls techniques](https://alice.climent-pommeret.red/posts/direct-syscalls-hells-halos-syswhispers2/)
-- [@redops blogpost about direct vs indirect syscalls](https://redops.at/en/blog/direct-syscalls-a-journey-from-high-to-low)
-- [@Jackson_T & @modexpblog for Syswhispers2](https://github.com/jthuraisamy/SysWhispers2)
-- [@klezvirus for syswhispers3](https://github.com/klezVirus/SysWhispers3)
+  - [@alice blogpost about syscalls techniques](https://alice.climent-pommeret.red/posts/direct-syscalls-hells-halos-syswhispers2/)
+  - [@redops blogpost about direct vs indirect syscalls](https://redops.at/en/blog/direct-syscalls-a-journey-from-high-to-low)
+  - [@Jackson_T & @modexpblog for Syswhispers2](https://github.com/jthuraisamy/SysWhispers2)
+  - [@klezvirus for syswhispers3](https://github.com/klezVirus/SysWhispers3)
 
 ## :construction: TODO
 This project is really in WIP state...  
 Some PR & reviews are more than welcome :tada: !
-- [x] Add internal names randomization
-- [ ] Add x86 support
-- [ ] Add WoW64 support
-- [-] Add some tests
-- [x] Setup documentation
+  - [x] Add internal names randomization
+  - [x] Setup documentation
+  - [-] Add some tests
+  - [ ] Add x86 support
+  - [ ] Add WoW64 support
+  - [ ] Setup C templates
+  - [ ] Setup Go templates
+  - [ ] Setup Rust? templates
 
 ## License
 This project is licensed under the [MIT License](https://www.tldrlegal.com/license/mit-license), for individuals only. If you want to integrate this work in your commercial project please contact me through `0x42en[at]gmail.com`
+
```

