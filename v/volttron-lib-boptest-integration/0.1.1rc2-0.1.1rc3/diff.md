# Comparing `tmp/volttron_lib_boptest_integration-0.1.1rc2.tar.gz` & `tmp/volttron_lib_boptest_integration-0.1.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_boptest_integration-0.1.1rc2.tar", max compression
+gzip compressed data, was "volttron_lib_boptest_integration-0.1.1rc3.tar", max compression
```

## Comparing `volttron_lib_boptest_integration-0.1.1rc2.tar` & `volttron_lib_boptest_integration-0.1.1rc3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11927 2023-07-15 05:26:00.995697 volttron_lib_boptest_integration-0.1.1rc2/LICENSE
--rw-r--r--   0        0        0     9418 2023-07-15 05:26:00.995697 volttron_lib_boptest_integration-0.1.1rc2/README.md
--rw-r--r--   0        0        0     1856 2023-07-15 05:27:47.983273 volttron_lib_boptest_integration-0.1.1rc2/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/__init__.py
--rw-r--r--   0        0        0    13693 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/boptest_integration.py
--rw-r--r--   0        0        0      108 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/__init__.py
--rw-r--r--   0        0        0     3252 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/controller.py
--rw-r--r--   0        0        0     1537 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pid.py
--rw-r--r--   0        0        0     4610 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pidTwoZones.py
--rw-r--r--   0        0        0     1179 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/sup.py
--rw-r--r--   0        0        0     9666 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/interface.py
--rw-r--r--   0        0        0    10690 1970-01-01 00:00:00.000000 volttron_lib_boptest_integration-0.1.1rc2/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-17 18:43:01.666518 volttron_lib_boptest_integration-0.1.1rc3/LICENSE
+-rw-r--r--   0        0        0     9625 2023-07-17 18:43:01.666518 volttron_lib_boptest_integration-0.1.1rc3/README.md
+-rw-r--r--   0        0        0     1856 2023-07-17 18:44:33.005889 volttron_lib_boptest_integration-0.1.1rc3/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-07-17 18:43:01.670518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/__init__.py
+-rw-r--r--   0        0        0    13693 2023-07-17 18:43:01.670518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/boptest_integration.py
+-rw-r--r--   0        0        0      108 2023-07-17 18:43:01.670518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/__init__.py
+-rw-r--r--   0        0        0     3252 2023-07-17 18:43:01.670518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/controller.py
+-rw-r--r--   0        0        0     1537 2023-07-17 18:43:01.674518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/pid.py
+-rw-r--r--   0        0        0     4610 2023-07-17 18:43:01.674518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/pidTwoZones.py
+-rw-r--r--   0        0        0     1179 2023-07-17 18:43:01.674518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/sup.py
+-rw-r--r--   0        0        0     9666 2023-07-17 18:43:01.674518 volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/interface.py
+-rw-r--r--   0        0        0    10897 1970-01-01 00:00:00.000000 volttron_lib_boptest_integration-0.1.1rc3/PKG-INFO
```

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/LICENSE` & `volttron_lib_boptest_integration-0.1.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/README.md` & `volttron_lib_boptest_integration-0.1.1rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,18 @@
 
    ```shell
    git clone https://github.com/ibpsa/project1-boptest ~/project1-boptest
    ```
 
 1. Install [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/).
 
+   Note: this demo run docker as a non-root user, you can
+   follow [Linux post-installation steps for Docker Engine](https://docs.docker.com/engine/install/linux-postinstall/)
+   to achieve similar setup.
+
    (Optional) Verify with `docker-compose version` to verify the installation
    ```shell
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose version
    docker-compose version 1.29.2, build unknown
    docker-py version: 5.0.3
    CPython version: 3.10.6
    OpenSSL version: OpenSSL 3.0.2 15 Mar 2022
```

#### html2text {}

```diff
@@ -49,66 +49,68 @@
 of volttron-boptest-agent, we need to setup the boptest simulation server.
 (Please see more details about boptest quick-start at [Quick-Start to Deploy a
 Test Case](https://github.com/ibpsa/project1-boptest#quick-start-to-deploy-a-
 test-case)) 1. Download [IBPSA Project 1 - BOPTEST](https://github.com/ibpsa/
 project1-boptest) repository to . For demo purpose, let boptest_repo be `~/
 project1-boptest`. ```shell git clone https://github.com/ibpsa/project1-boptest
 ~/project1-boptest ``` 1. Install [Docker](https://docs.docker.com/get-docker/
-) and [Docker Compose](https://docs.docker.com/compose/install/). (Optional)
-Verify with `docker-compose version` to verify the installation ```shell (env)
-kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose version docker-
-compose version 1.29.2, build unknown docker-py version: 5.0.3 CPython version:
-3.10.6 OpenSSL version: OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build and deploy a
-test case. The basic command to start a test case is by using `TESTCASE=
-docker-compose up`. For demo purpose, we will build and deploy testcase1, for
-available testcases please see [testcases/](https://github.com/ibpsa/project1-
-boptest/tree/master/testcases) ```shell (env) kefei@ubuntu-22:~/sandbox/
-volttron-boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-boptest/
-docker-compose.yml up Creating network "boptest-net" with the default driver
-Creating project1-boptest_boptest_1 ... done Attaching to project1-
-boptest_boptest_1 boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Control step
-set successfully. boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test
-simulation initialized successfully to 0.0s with warmup period of 0.0s.
-boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test case scenario was set
-successfully. ... boptest_1 | * Debug mode: off boptest_1 | 07/13/2023 09:59:42
-PM UTC werkzeug INFO * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
-``` Or use detach mode ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-
-boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-
-compose.yml up --detach Starting project1-boptest_boptest_1 ... done (env)
-kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker container ls CONTAINER ID
-IMAGE COMMAND CREATED STATUS PORTS NAMES ddd0f2cc1f99 boptest_base "/bin/sh -
-c 'python â¦" 23 hours ago Up 12 seconds 127.0.0.1:5000->5000/tcp project1-
-boptest_boptest_1 ``` Note: Use `docker-compose down` to shut down the service.
-Verify boptest simulation server is running properly: ```shell (env)
-kefei@ubuntu-22:~/sandbox/volttron-boptest$ curl http://127.0.0.1:5000/name
-{"message":"Queried the name of the test case successfully.","payload":{"name":
-"testcase1"},"status":200} ``` 1. Run example usecases. There are several
-exmaple usecases available at [examples/](examples). In this demo, we will run
-[testcase1.py](examples/tescase1.py). ```shell (env) kefei@ubuntu-22:~/sandbox/
-volttron-boptest$ python volttron-lib-boptest-integration/examples/testcase1.py
-INFO:root:=========== run_workflow INFO:root: TEST CASE INFORMATION -----------
----------- INFO:root:Name: testcase1 ... INFO:root:======== run workflow
-completed.====== ======= kpi {'cost_tot': 0.075149821513246, 'emis_tot':
-0.2147137757521314, 'ener_tot': 1.073568878760657, 'idis_tot':
-508.47225004790033, 'pdih_tot': None, 'pele_tot': None, 'pgas_tot':
-0.09615811655434148, 'tdis_tot': 5.316029375566828, 'time_rat':
-1.531114146269157e-05} ``` Note: the example usecase must match the test case
-that is running. For example when TESTCASE=testcase1, we can run [testcase1.py]
-(examples/testcase1.py) and [testcase1_scenario.py](examples/
-testcase1_scenario.py), but not [testcase2.py](examples/testcase2.py). #
-Development Please see the following for contributing guidelines [contributing]
-(https://github.com/eclipse-volttron/volttron-core/blob/develop/
-CONTRIBUTING.md). Please see the following helpful guide about [developing
-modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/
-blob/develop/DEVELOPING_ON_MODULAR.md) # Disclaimer Notice This material was
-prepared as an account of work sponsored by an agency of the United States
-Government. Neither the United States Government nor the United States
-Department of Energy, nor Battelle, nor any of their employees, nor any
-jurisdiction or organization that has cooperated in the development of these
-materials, makes any warranty, express or implied, or assumes any legal
+) and [Docker Compose](https://docs.docker.com/compose/install/). Note: this
+demo run docker as a non-root user, you can follow [Linux post-installation
+steps for Docker Engine](https://docs.docker.com/engine/install/linux-
+postinstall/) to achieve similar setup. (Optional) Verify with `docker-compose
+version` to verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/
+volttron-boptest$ docker-compose version docker-compose version 1.29.2, build
+unknown docker-py version: 5.0.3 CPython version: 3.10.6 OpenSSL version:
+OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build and deploy a test case. The basic
+command to start a test case is by using `TESTCASE= docker-compose up`. For
+demo purpose, we will build and deploy testcase1, for available testcases
+please see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/
+testcases) ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml
+up Creating network "boptest-net" with the default driver Creating project1-
+boptest_boptest_1 ... done Attaching to project1-boptest_boptest_1 boptest_1 |
+07/13/2023 09:59:42 PM UTC root INFO Control step set successfully. boptest_1 |
+07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized successfully
+to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:42 PM UTC root
+INFO Test case scenario was set successfully. ... boptest_1 | * Debug mode: off
+boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running on http://
+0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose -
+-file ~/project1-boptest/docker-compose.yml up --detach Starting project1-
+boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS NAMES
+ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12 seconds
+127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use `docker-
+compose down` to shut down the service. Verify boptest simulation server is
+running properly: ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+curl http://127.0.0.1:5000/name {"message":"Queried the name of the test case
+successfully.","payload":{"name":"testcase1"},"status":200} ``` 1. Run example
+usecases. There are several exmaple usecases available at [examples/]
+(examples). In this demo, we will run [testcase1.py](examples/tescase1.py).
+```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ python volttron-lib-
+boptest-integration/examples/testcase1.py INFO:root:=========== run_workflow
+INFO:root: TEST CASE INFORMATION --------------------- INFO:root:Name:
+testcase1 ... INFO:root:======== run workflow completed.====== ======= kpi
+{'cost_tot': 0.075149821513246, 'emis_tot': 0.2147137757521314, 'ener_tot':
+1.073568878760657, 'idis_tot': 508.47225004790033, 'pdih_tot': None,
+'pele_tot': None, 'pgas_tot': 0.09615811655434148, 'tdis_tot':
+5.316029375566828, 'time_rat': 1.531114146269157e-05} ``` Note: the example
+usecase must match the test case that is running. For example when
+TESTCASE=testcase1, we can run [testcase1.py](examples/testcase1.py) and
+[testcase1_scenario.py](examples/testcase1_scenario.py), but not [testcase2.py]
+(examples/testcase2.py). # Development Please see the following for
+contributing guidelines [contributing](https://github.com/eclipse-volttron/
+volttron-core/blob/develop/CONTRIBUTING.md). Please see the following helpful
+guide about [developing modular VOLTTRON agents](https://github.com/eclipse-
+volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md) # Disclaimer
+Notice This material was prepared as an account of work sponsored by an agency
+of the United States Government. Neither the United States Government nor the
+United States Department of Energy, nor Battelle, nor any of their employees,
+nor any jurisdiction or organization that has cooperated in the development of
+these materials, makes any warranty, express or implied, or assumes any legal
 liability or responsibility for the accuracy, completeness, or usefulness or
 any information, apparatus, product, software, or process disclosed, or
 represents that its use would not infringe privately owned rights. Reference
 herein to any specific commercial product, process, or service by trade name,
 trademark, manufacturer, or otherwise does not necessarily constitute or imply
 its endorsement, recommendation, or favoring by the United States Government or
 any agency thereof, or Battelle Memorial Institute. The views and opinions of
```

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/pyproject.toml` & `volttron_lib_boptest_integration-0.1.1rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-lib-boptest-integration"
-version = "0.1.1rc2"
+version = "0.1.1rc3"
 description = "A Volttron library for boptest simulation integration."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-boptest"
 repository = "https://github.com/eclipse-volttron/volttron-boptest"
```

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/boptest_integration.py` & `volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/boptest_integration.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/controller.py` & `volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pid.py` & `volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/pid.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pidTwoZones.py` & `volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/pidTwoZones.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/sup.py` & `volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/controllers/sup.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/interface.py` & `volttron_lib_boptest_integration-0.1.1rc3/src/boptest_integration/interface.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc2/PKG-INFO` & `volttron_lib_boptest_integration-0.1.1rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-boptest-integration
-Version: 0.1.1rc2
+Version: 0.1.1rc3
 Summary: A Volttron library for boptest simulation integration.
 Home-page: https://github.com/eclipse-volttron/volttron-boptest
 License: Apache-2.0
 Keywords: volttron,boptest,simulation,integration
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
@@ -151,14 +151,18 @@
 
    ```shell
    git clone https://github.com/ibpsa/project1-boptest ~/project1-boptest
    ```
 
 1. Install [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/).
 
+   Note: this demo run docker as a non-root user, you can
+   follow [Linux post-installation steps for Docker Engine](https://docs.docker.com/engine/install/linux-postinstall/)
+   to achieve similar setup.
+
    (Optional) Verify with `docker-compose version` to verify the installation
    ```shell
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose version
    docker-compose version 1.29.2, build unknown
    docker-py version: 5.0.3
    CPython version: 3.10.6
    OpenSSL version: OpenSSL 3.0.2 15 Mar 2022
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-lib-boptest-integration Version: 0.1.1rc2
+Metadata-Version: 2.1 Name: volttron-lib-boptest-integration Version: 0.1.1rc3
 Summary: A Volttron library for boptest simulation integration. Home-page:
 https://github.com/eclipse-volttron/volttron-boptest License: Apache-2.0
 Keywords: volttron,boptest,simulation,integration Author: Kefei Mo Author-
 email: kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email:
 volttron@pnnl.gov Requires-Python: >=3.10,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
@@ -66,65 +66,68 @@
 boptest simulation server. (Please see more details about boptest quick-start
 at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-
 boptest#quick-start-to-deploy-a-test-case)) 1. Download [IBPSA Project 1 -
 BOPTEST](https://github.com/ibpsa/project1-boptest) repository to . For demo
 purpose, let boptest_repo be `~/project1-boptest`. ```shell git clone https://
 github.com/ibpsa/project1-boptest ~/project1-boptest ``` 1. Install [Docker]
 (https://docs.docker.com/get-docker/) and [Docker Compose](https://
-docs.docker.com/compose/install/). (Optional) Verify with `docker-compose
-version` to verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/
-volttron-boptest$ docker-compose version docker-compose version 1.29.2, build
-unknown docker-py version: 5.0.3 CPython version: 3.10.6 OpenSSL version:
-OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build and deploy a test case. The basic
-command to start a test case is by using `TESTCASE= docker-compose up`. For
-demo purpose, we will build and deploy testcase1, for available testcases
-please see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/
-testcases) ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
-TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml
-up Creating network "boptest-net" with the default driver Creating project1-
-boptest_boptest_1 ... done Attaching to project1-boptest_boptest_1 boptest_1 |
-07/13/2023 09:59:42 PM UTC root INFO Control step set successfully. boptest_1 |
-07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized successfully
-to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:42 PM UTC root
-INFO Test case scenario was set successfully. ... boptest_1 | * Debug mode: off
-boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running on http://
-0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell (env)
-kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose -
--file ~/project1-boptest/docker-compose.yml up --detach Starting project1-
-boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
-docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS NAMES
-ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12 seconds
-127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use `docker-
-compose down` to shut down the service. Verify boptest simulation server is
-running properly: ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
-curl http://127.0.0.1:5000/name {"message":"Queried the name of the test case
-successfully.","payload":{"name":"testcase1"},"status":200} ``` 1. Run example
-usecases. There are several exmaple usecases available at [examples/]
-(examples). In this demo, we will run [testcase1.py](examples/tescase1.py).
-```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ python volttron-lib-
-boptest-integration/examples/testcase1.py INFO:root:=========== run_workflow
-INFO:root: TEST CASE INFORMATION --------------------- INFO:root:Name:
-testcase1 ... INFO:root:======== run workflow completed.====== ======= kpi
-{'cost_tot': 0.075149821513246, 'emis_tot': 0.2147137757521314, 'ener_tot':
-1.073568878760657, 'idis_tot': 508.47225004790033, 'pdih_tot': None,
-'pele_tot': None, 'pgas_tot': 0.09615811655434148, 'tdis_tot':
-5.316029375566828, 'time_rat': 1.531114146269157e-05} ``` Note: the example
-usecase must match the test case that is running. For example when
-TESTCASE=testcase1, we can run [testcase1.py](examples/testcase1.py) and
-[testcase1_scenario.py](examples/testcase1_scenario.py), but not [testcase2.py]
-(examples/testcase2.py). # Development Please see the following for
-contributing guidelines [contributing](https://github.com/eclipse-volttron/
-volttron-core/blob/develop/CONTRIBUTING.md). Please see the following helpful
-guide about [developing modular VOLTTRON agents](https://github.com/eclipse-
-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md) # Disclaimer
-Notice This material was prepared as an account of work sponsored by an agency
-of the United States Government. Neither the United States Government nor the
-United States Department of Energy, nor Battelle, nor any of their employees,
-nor any jurisdiction or organization that has cooperated in the development of
-these materials, makes any warranty, express or implied, or assumes any legal
+docs.docker.com/compose/install/). Note: this demo run docker as a non-root
+user, you can follow [Linux post-installation steps for Docker Engine](https://
+docs.docker.com/engine/install/linux-postinstall/) to achieve similar setup.
+(Optional) Verify with `docker-compose version` to verify the installation
+```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose
+version docker-compose version 1.29.2, build unknown docker-py version: 5.0.3
+CPython version: 3.10.6 OpenSSL version: OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build
+and deploy a test case. The basic command to start a test case is by using
+`TESTCASE= docker-compose up`. For demo purpose, we will build and deploy
+testcase1, for available testcases please see [testcases/](https://github.com/
+ibpsa/project1-boptest/tree/master/testcases) ```shell (env) kefei@ubuntu-22:~/
+sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-
+boptest/docker-compose.yml up Creating network "boptest-net" with the default
+driver Creating project1-boptest_boptest_1 ... done Attaching to project1-
+boptest_boptest_1 boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Control step
+set successfully. boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test
+simulation initialized successfully to 0.0s with warmup period of 0.0s.
+boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test case scenario was set
+successfully. ... boptest_1 | * Debug mode: off boptest_1 | 07/13/2023 09:59:42
+PM UTC werkzeug INFO * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
+``` Or use detach mode ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-
+boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-
+compose.yml up --detach Starting project1-boptest_boptest_1 ... done (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker container ls CONTAINER ID
+IMAGE COMMAND CREATED STATUS PORTS NAMES ddd0f2cc1f99 boptest_base "/bin/sh -
+c 'python â¦" 23 hours ago Up 12 seconds 127.0.0.1:5000->5000/tcp project1-
+boptest_boptest_1 ``` Note: Use `docker-compose down` to shut down the service.
+Verify boptest simulation server is running properly: ```shell (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ curl http://127.0.0.1:5000/name
+{"message":"Queried the name of the test case successfully.","payload":{"name":
+"testcase1"},"status":200} ``` 1. Run example usecases. There are several
+exmaple usecases available at [examples/](examples). In this demo, we will run
+[testcase1.py](examples/tescase1.py). ```shell (env) kefei@ubuntu-22:~/sandbox/
+volttron-boptest$ python volttron-lib-boptest-integration/examples/testcase1.py
+INFO:root:=========== run_workflow INFO:root: TEST CASE INFORMATION -----------
+---------- INFO:root:Name: testcase1 ... INFO:root:======== run workflow
+completed.====== ======= kpi {'cost_tot': 0.075149821513246, 'emis_tot':
+0.2147137757521314, 'ener_tot': 1.073568878760657, 'idis_tot':
+508.47225004790033, 'pdih_tot': None, 'pele_tot': None, 'pgas_tot':
+0.09615811655434148, 'tdis_tot': 5.316029375566828, 'time_rat':
+1.531114146269157e-05} ``` Note: the example usecase must match the test case
+that is running. For example when TESTCASE=testcase1, we can run [testcase1.py]
+(examples/testcase1.py) and [testcase1_scenario.py](examples/
+testcase1_scenario.py), but not [testcase2.py](examples/testcase2.py). #
+Development Please see the following for contributing guidelines [contributing]
+(https://github.com/eclipse-volttron/volttron-core/blob/develop/
+CONTRIBUTING.md). Please see the following helpful guide about [developing
+modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/
+blob/develop/DEVELOPING_ON_MODULAR.md) # Disclaimer Notice This material was
+prepared as an account of work sponsored by an agency of the United States
+Government. Neither the United States Government nor the United States
+Department of Energy, nor Battelle, nor any of their employees, nor any
+jurisdiction or organization that has cooperated in the development of these
+materials, makes any warranty, express or implied, or assumes any legal
 liability or responsibility for the accuracy, completeness, or usefulness or
 any information, apparatus, product, software, or process disclosed, or
 represents that its use would not infringe privately owned rights. Reference
 herein to any specific commercial product, process, or service by trade name,
 trademark, manufacturer, or otherwise does not necessarily constitute or imply
 its endorsement, recommendation, or favoring by the United States Government or
 any agency thereof, or Battelle Memorial Institute. The views and opinions of
```

