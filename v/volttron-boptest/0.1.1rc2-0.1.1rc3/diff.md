# Comparing `tmp/volttron_boptest-0.1.1rc2.tar.gz` & `tmp/volttron_boptest-0.1.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_boptest-0.1.1rc2.tar", max compression
+gzip compressed data, was "volttron_boptest-0.1.1rc3.tar", max compression
```

## Comparing `volttron_boptest-0.1.1rc2.tar` & `volttron_boptest-0.1.1rc3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11927 2023-07-15 05:26:00.991696 volttron_boptest-0.1.1rc2/LICENSE
--rw-r--r--   0        0        0    17029 2023-07-15 05:26:00.991696 volttron_boptest-0.1.1rc2/README.md
--rw-r--r--   0        0        0     1845 2023-07-15 05:27:46.163212 volttron_boptest-0.1.1rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-15 05:26:00.995697 volttron_boptest-0.1.1rc2/src/boptest/__init__.py
--rw-r--r--   0        0        0    15888 2023-07-15 05:26:00.995697 volttron_boptest-0.1.1rc2/src/boptest/agent.py
--rw-r--r--   0        0        0     1525 2023-07-15 05:26:00.995697 volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/README.md
--rw-r--r--   0        0        0       77 2023-07-15 05:26:00.995697 volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-15 05:26:00.995697 volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/custom_kpi_calculator.py
--rw-r--r--   0        0        0      499 2023-07-15 05:26:00.995697 volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/custom_kpis_example.config
--rw-r--r--   0        0        0     1152 2023-07-15 05:26:00.995697 volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/custom_kpis_example.py
--rw-r--r--   0        0        0    18313 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1rc2/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-17 18:43:01.662518 volttron_boptest-0.1.1rc3/LICENSE
+-rw-r--r--   0        0        0    17236 2023-07-17 18:43:01.662518 volttron_boptest-0.1.1rc3/README.md
+-rw-r--r--   0        0        0     1845 2023-07-17 18:44:31.405902 volttron_boptest-0.1.1rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/__init__.py
+-rw-r--r--   0        0        0    15888 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/agent.py
+-rw-r--r--   0        0        0     1525 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/README.md
+-rw-r--r--   0        0        0       77 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpi_calculator.py
+-rw-r--r--   0        0        0      499 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpis_example.config
+-rw-r--r--   0        0        0     1152 2023-07-17 18:43:01.666518 volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpis_example.py
+-rw-r--r--   0        0        0    18520 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1rc3/PKG-INFO
```

### Comparing `volttron_boptest-0.1.1rc2/LICENSE` & `volttron_boptest-0.1.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc2/README.md` & `volttron_boptest-0.1.1rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,18 @@
 
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
@@ -45,87 +45,89 @@
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
-demo purpose, we will build and deploy testcase1, for avialbe testcases please
-see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/
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
-successfully.","payload":{"name":"testcase1"},"status":200} ``` ### Install
-volttron boptest agent 1. Install the "volttron-boptest" dependency. There are
-two options to install volttron-boptest. You can install this library using the
-version on PyPi or install it from the source code (`git clone` might be
-required.) Note: the `vctl install` command in the following step can handle
-dependency installation using pypi. However, in this demo we demonstrate what
-is happening under the neath the hood by separating the dependency installation
-and agent registry steps. ```shell # option 1: install from pypi pip install
-volttron-boptest # option 2: install from the source code (Note: `-e` option to
-use editable mode, useful for development.) pip install [-e] /volttron-boptest/
-``` 1. Install and start the "volttron-boptest" agent. We will use the
-[testcase1.config](examples/testcase1.config) as the agent config for this
-demo. Please see [examples/](examples) for other example config files. Use
-`vctl install` command to register to the volttron home path. Note: for demo
-purposes and reproducibility, we assign vip-identity as
-"volttron_boptest_agent", but you can choose any other valid agent identity as
-desired. ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl
-install volttron-boptest \ --agent-config volttron-boptest-agent/examples/
-testcase1.config \ --vip-identity volttron_boptest_agent \ --start Agent
-a0fd6f5c-3751-4312-9f59-ca541b8aac4e installed and started [4980] ``` Observe
-Data The volttron-boptest agent publishes events on the message bus. To see
-these events in the Volttron log file, install a [Listener Agent](https://
-pypi.org/project/volttron-listener/): ``` vctl install volttron-listener --
-start ``` (Optional) Use `vctl stauts` to verify the installation ```shell
-(env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl status UUID AGENT
-IDENTITY TAG PRIORITY STATUS HEALTH a volttron-boptest-agent-0.0.1
-volttron_boptest_agent running [59108] GOOD 2 volttron-listener-0.2.0rc0
-volttron-listener-0.2.0rc0_1 running [59096] GOOD ``` 1. (optional) Inspect the
-volttron.log file   Within the volttron.log, we should see similar logs as
-follows ```shell # Create config file place holders KPI RESULTS ----------
-- 2023-07-13 18:27:51,124 (volttron-boptest-agent-0.0.1 59108) root(186) INFO:
-emis_tot: 0.2147137757521314 KgCO2/m$^2$ 2023-07-13 18:27:51,174 (volttron-
-boptest-agent-0.0.1 59108) root(186) INFO: ener_tot: 1.073568878760657 kWh/
-m$^2$ 2023-07-13 18:27:51,223 (volttron-boptest-agent-0.0.1 59108) root(186)
-INFO: idis_tot: 508.47225004790033 ppmh/zone 2023-07-13 18:27:51,280 (volttron-
-boptest-agent-0.0.1 59108) root(186) INFO: pdih_tot: None kW/m$^2$ 2023-07-13
-18:27:51,330 (volttron-boptest-agent-0.0.1 59108) root(186) INFO: pele_tot:
-None kW/m$^2$ 2023-07-13 18:27:51,381 (volttron-boptest-agent-0.0.1 59108) root
-(186) INFO: pgas_tot: 0.09615811655434148 kW/m$^2$ 2023-07-13 18:27:51,436
-(volttron-boptest-agent-0.0.1 59108) root(186) INFO: tdis_tot:
-5.316029375566828 Kh/zone 2023-07-13 18:27:51,494 (volttron-boptest-agent-0.0.1
-59108) root(186) INFO: time_rat: 0.001856946445725582 s/s 2023-07-13 18:27:
-51,550 (volttron-boptest-agent-0.0.1 59108) root(202) INFO: ======== run
-workflow completed.====== 2023-07-13 18:27:51,553 (volttron-boptest-agent-0.0.1
-59108) (0) INFO: ["======= kpi {'cost_tot': 0.075149821513246, 'emis_tot':
-0.2147137757521314, 'ener_tot': 1.073568878760657, 'idis_tot':
+docs.docker.com/compose/install/). Note: this demo run docker as a non-root
+user, you can follow [Linux post-installation steps for Docker Engine](https://
+docs.docker.com/engine/install/linux-postinstall/) to achieve similar setup.
+(Optional) Verify with `docker-compose version` to verify the installation
+```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose
+version docker-compose version 1.29.2, build unknown docker-py version: 5.0.3
+CPython version: 3.10.6 OpenSSL version: OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build
+and deploy a test case. The basic command to start a test case is by using
+`TESTCASE= docker-compose up`. For demo purpose, we will build and deploy
+testcase1, for avialbe testcases please see [testcases/](https://github.com/
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
+"testcase1"},"status":200} ``` ### Install volttron boptest agent 1. Install
+the "volttron-boptest" dependency. There are two options to install volttron-
+boptest. You can install this library using the version on PyPi or install it
+from the source code (`git clone` might be required.) Note: the `vctl install`
+command in the following step can handle dependency installation using pypi.
+However, in this demo we demonstrate what is happening under the neath the hood
+by separating the dependency installation and agent registry steps. ```shell #
+option 1: install from pypi pip install volttron-boptest # option 2: install
+from the source code (Note: `-e` option to use editable mode, useful for
+development.) pip install [-e] /volttron-boptest/ ``` 1. Install and start the
+"volttron-boptest" agent. We will use the [testcase1.config](examples/
+testcase1.config) as the agent config for this demo. Please see [examples/]
+(examples) for other example config files. Use `vctl install` command to
+register to the volttron home path. Note: for demo purposes and
+reproducibility, we assign vip-identity as "volttron_boptest_agent", but you
+can choose any other valid agent identity as desired. ```shell (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl install volttron-boptest \ --
+agent-config volttron-boptest-agent/examples/testcase1.config \ --vip-identity
+volttron_boptest_agent \ --start Agent a0fd6f5c-3751-4312-9f59-ca541b8aac4e
+installed and started [4980] ``` Observe Data The volttron-boptest agent
+publishes events on the message bus. To see these events in the Volttron log
+file, install a [Listener Agent](https://pypi.org/project/volttron-listener/):
+``` vctl install volttron-listener --start ``` (Optional) Use `vctl stauts` to
+verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-
+boptest$ vctl status UUID AGENT IDENTITY TAG PRIORITY STATUS HEALTH a volttron-
+boptest-agent-0.0.1 volttron_boptest_agent running [59108] GOOD 2 volttron-
+listener-0.2.0rc0 volttron-listener-0.2.0rc0_1 running [59096] GOOD ``` 1.
+(optional) Inspect the volttron.log file   Within the volttron.log, we should
+see similar logs as follows ```shell # Create config file place holders KPI
+RESULTS ----------- 2023-07-13 18:27:51,124 (volttron-boptest-agent-0.0.1
+59108) root(186) INFO: emis_tot: 0.2147137757521314 KgCO2/m$^2$ 2023-07-13 18:
+27:51,174 (volttron-boptest-agent-0.0.1 59108) root(186) INFO: ener_tot:
+1.073568878760657 kWh/m$^2$ 2023-07-13 18:27:51,223 (volttron-boptest-agent-
+0.0.1 59108) root(186) INFO: idis_tot: 508.47225004790033 ppmh/zone 2023-07-13
+18:27:51,280 (volttron-boptest-agent-0.0.1 59108) root(186) INFO: pdih_tot:
+None kW/m$^2$ 2023-07-13 18:27:51,330 (volttron-boptest-agent-0.0.1 59108) root
+(186) INFO: pele_tot: None kW/m$^2$ 2023-07-13 18:27:51,381 (volttron-boptest-
+agent-0.0.1 59108) root(186) INFO: pgas_tot: 0.09615811655434148 kW/m$^2$ 2023-
+07-13 18:27:51,436 (volttron-boptest-agent-0.0.1 59108) root(186) INFO:
+tdis_tot: 5.316029375566828 Kh/zone 2023-07-13 18:27:51,494 (volttron-boptest-
+agent-0.0.1 59108) root(186) INFO: time_rat: 0.001856946445725582 s/s 2023-07-
+13 18:27:51,550 (volttron-boptest-agent-0.0.1 59108) root(202) INFO: ========
+run workflow completed.====== 2023-07-13 18:27:51,553 (volttron-boptest-agent-
+0.0.1 59108) (0) INFO: ["======= kpi {'cost_tot': 0.075149821513246,
+'emis_tot': 0.2147137757521314, 'ener_tot': 1.073568878760657, 'idis_tot':
 508.47225004790033, 'pdih_tot': None, 'pele_tot': None, 'pgas_tot':
 0.09615811655434148, 'tdis_tot': 5.316029375566828, 'time_rat':
 0.001856946445725582}"] 2023-07-13 18:27:51,558 (volttron-boptest-agent-0.0.1
 59108) root(129) INFO: =========== refactoring onstart 2023-07-13 18:27:52,067
 (volttron-listener-0.2.0rc0 59096) listener.agent(104) INFO: Peer: pubsub,
 Sender: volttron_boptest_agent:, Bus: , Topic: PNNL/BUILDING/UNIT/kpi, Headers:
 {'min_compatible_version': '3.0', 'max_compatible_version': ''}, Message: ("
```

### Comparing `volttron_boptest-0.1.1rc2/pyproject.toml` & `volttron_boptest-0.1.1rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-boptest"
-version = "0.1.1rc2"
+version = "0.1.1rc3"
 description = "A Volttron agent that runs boptest simulation."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-boptest"
 repository = "https://github.com/eclipse-volttron/volttron-boptest"
@@ -37,15 +37,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-volttron-lib-boptest-integration = "^0.1.1rc2"
+volttron-lib-boptest-integration = "^0.1.1rc3"
 numpy = ">0.0.0"
 pandas = ">0.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=6.2.4"
 pytest-cov = ">=3.0.0"
 pytest-env = ">0.0.0"
```

### Comparing `volttron_boptest-0.1.1rc2/src/boptest/agent.py` & `volttron_boptest-0.1.1rc3/src/boptest/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/README.md` & `volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/README.md`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/custom_kpi_calculator.py` & `volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpi_calculator.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc2/src/boptest/custom_kpi/custom_kpis_example.py` & `volttron_boptest-0.1.1rc3/src/boptest/custom_kpi/custom_kpis_example.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1rc2/PKG-INFO` & `volttron_boptest-0.1.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-boptest
-Version: 0.1.1rc2
+Version: 0.1.1rc3
 Summary: A Volttron agent that runs boptest simulation.
 Home-page: https://github.com/eclipse-volttron/volttron-boptest
 License: Apache-2.0
 Keywords: volttron,agent,boptest,simulation,application
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Dist: numpy (>0.0.0)
 Requires-Dist: pandas (>0.0.0)
-Requires-Dist: volttron-lib-boptest-integration (>=0.1.1rc2,<0.2.0)
+Requires-Dist: volttron-lib-boptest-integration (>=0.1.1rc3,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/eclipse-volttron/volttron-boptest/issues
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-boptest
 Description-Content-Type: text/markdown
 
 # boptest-agent
 
 The volttron-boptest-agent utilizes the volttron-lib-boptest-integration library to perform simulation control and
@@ -142,14 +142,18 @@
 
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
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1rc2 Summary: A
+Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1rc3 Summary: A
 Volttron agent that runs boptest simulation. Home-page: https://github.com/
 eclipse-volttron/volttron-boptest License: Apache-2.0 Keywords:
 volttron,agent,boptest,simulation,application Author: Kefei Mo Author-email:
 kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Home Automation Classifier:
 Topic :: Software Development :: Embedded Systems Requires-Dist: numpy (>0.0.0)
 Requires-Dist: pandas (>0.0.0) Requires-Dist: volttron-lib-boptest-integration
-(>=0.1.1rc2,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
+(>=0.1.1rc3,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
 volttron/volttron-boptest/issues Project-URL: Repository, https://github.com/
 eclipse-volttron/volttron-boptest Description-Content-Type: text/markdown #
 boptest-agent The volttron-boptest-agent utilizes the volttron-lib-boptest-
 integration library to perform simulation control and benchmark tasks. BOPTEST
 is designed to facilitate the performance evaluation and benchmarking of
 building control strategies, which contains these key components: 1. Run-Time
 Environment (RTE): Deployed with Docker and accessed with a RESTful HTTP API,
@@ -62,87 +62,89 @@
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
-demo purpose, we will build and deploy testcase1, for avialbe testcases please
-see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/
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
-successfully.","payload":{"name":"testcase1"},"status":200} ``` ### Install
-volttron boptest agent 1. Install the "volttron-boptest" dependency. There are
-two options to install volttron-boptest. You can install this library using the
-version on PyPi or install it from the source code (`git clone` might be
-required.) Note: the `vctl install` command in the following step can handle
-dependency installation using pypi. However, in this demo we demonstrate what
-is happening under the neath the hood by separating the dependency installation
-and agent registry steps. ```shell # option 1: install from pypi pip install
-volttron-boptest # option 2: install from the source code (Note: `-e` option to
-use editable mode, useful for development.) pip install [-e] /volttron-boptest/
-``` 1. Install and start the "volttron-boptest" agent. We will use the
-[testcase1.config](examples/testcase1.config) as the agent config for this
-demo. Please see [examples/](examples) for other example config files. Use
-`vctl install` command to register to the volttron home path. Note: for demo
-purposes and reproducibility, we assign vip-identity as
-"volttron_boptest_agent", but you can choose any other valid agent identity as
-desired. ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl
-install volttron-boptest \ --agent-config volttron-boptest-agent/examples/
-testcase1.config \ --vip-identity volttron_boptest_agent \ --start Agent
-a0fd6f5c-3751-4312-9f59-ca541b8aac4e installed and started [4980] ``` Observe
-Data The volttron-boptest agent publishes events on the message bus. To see
-these events in the Volttron log file, install a [Listener Agent](https://
-pypi.org/project/volttron-listener/): ``` vctl install volttron-listener --
-start ``` (Optional) Use `vctl stauts` to verify the installation ```shell
-(env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl status UUID AGENT
-IDENTITY TAG PRIORITY STATUS HEALTH a volttron-boptest-agent-0.0.1
-volttron_boptest_agent running [59108] GOOD 2 volttron-listener-0.2.0rc0
-volttron-listener-0.2.0rc0_1 running [59096] GOOD ``` 1. (optional) Inspect the
-volttron.log file   Within the volttron.log, we should see similar logs as
-follows ```shell # Create config file place holders KPI RESULTS ----------
-- 2023-07-13 18:27:51,124 (volttron-boptest-agent-0.0.1 59108) root(186) INFO:
-emis_tot: 0.2147137757521314 KgCO2/m$^2$ 2023-07-13 18:27:51,174 (volttron-
-boptest-agent-0.0.1 59108) root(186) INFO: ener_tot: 1.073568878760657 kWh/
-m$^2$ 2023-07-13 18:27:51,223 (volttron-boptest-agent-0.0.1 59108) root(186)
-INFO: idis_tot: 508.47225004790033 ppmh/zone 2023-07-13 18:27:51,280 (volttron-
-boptest-agent-0.0.1 59108) root(186) INFO: pdih_tot: None kW/m$^2$ 2023-07-13
-18:27:51,330 (volttron-boptest-agent-0.0.1 59108) root(186) INFO: pele_tot:
-None kW/m$^2$ 2023-07-13 18:27:51,381 (volttron-boptest-agent-0.0.1 59108) root
-(186) INFO: pgas_tot: 0.09615811655434148 kW/m$^2$ 2023-07-13 18:27:51,436
-(volttron-boptest-agent-0.0.1 59108) root(186) INFO: tdis_tot:
-5.316029375566828 Kh/zone 2023-07-13 18:27:51,494 (volttron-boptest-agent-0.0.1
-59108) root(186) INFO: time_rat: 0.001856946445725582 s/s 2023-07-13 18:27:
-51,550 (volttron-boptest-agent-0.0.1 59108) root(202) INFO: ======== run
-workflow completed.====== 2023-07-13 18:27:51,553 (volttron-boptest-agent-0.0.1
-59108) (0) INFO: ["======= kpi {'cost_tot': 0.075149821513246, 'emis_tot':
-0.2147137757521314, 'ener_tot': 1.073568878760657, 'idis_tot':
+docs.docker.com/compose/install/). Note: this demo run docker as a non-root
+user, you can follow [Linux post-installation steps for Docker Engine](https://
+docs.docker.com/engine/install/linux-postinstall/) to achieve similar setup.
+(Optional) Verify with `docker-compose version` to verify the installation
+```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose
+version docker-compose version 1.29.2, build unknown docker-py version: 5.0.3
+CPython version: 3.10.6 OpenSSL version: OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build
+and deploy a test case. The basic command to start a test case is by using
+`TESTCASE= docker-compose up`. For demo purpose, we will build and deploy
+testcase1, for avialbe testcases please see [testcases/](https://github.com/
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
+"testcase1"},"status":200} ``` ### Install volttron boptest agent 1. Install
+the "volttron-boptest" dependency. There are two options to install volttron-
+boptest. You can install this library using the version on PyPi or install it
+from the source code (`git clone` might be required.) Note: the `vctl install`
+command in the following step can handle dependency installation using pypi.
+However, in this demo we demonstrate what is happening under the neath the hood
+by separating the dependency installation and agent registry steps. ```shell #
+option 1: install from pypi pip install volttron-boptest # option 2: install
+from the source code (Note: `-e` option to use editable mode, useful for
+development.) pip install [-e] /volttron-boptest/ ``` 1. Install and start the
+"volttron-boptest" agent. We will use the [testcase1.config](examples/
+testcase1.config) as the agent config for this demo. Please see [examples/]
+(examples) for other example config files. Use `vctl install` command to
+register to the volttron home path. Note: for demo purposes and
+reproducibility, we assign vip-identity as "volttron_boptest_agent", but you
+can choose any other valid agent identity as desired. ```shell (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl install volttron-boptest \ --
+agent-config volttron-boptest-agent/examples/testcase1.config \ --vip-identity
+volttron_boptest_agent \ --start Agent a0fd6f5c-3751-4312-9f59-ca541b8aac4e
+installed and started [4980] ``` Observe Data The volttron-boptest agent
+publishes events on the message bus. To see these events in the Volttron log
+file, install a [Listener Agent](https://pypi.org/project/volttron-listener/):
+``` vctl install volttron-listener --start ``` (Optional) Use `vctl stauts` to
+verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-
+boptest$ vctl status UUID AGENT IDENTITY TAG PRIORITY STATUS HEALTH a volttron-
+boptest-agent-0.0.1 volttron_boptest_agent running [59108] GOOD 2 volttron-
+listener-0.2.0rc0 volttron-listener-0.2.0rc0_1 running [59096] GOOD ``` 1.
+(optional) Inspect the volttron.log file   Within the volttron.log, we should
+see similar logs as follows ```shell # Create config file place holders KPI
+RESULTS ----------- 2023-07-13 18:27:51,124 (volttron-boptest-agent-0.0.1
+59108) root(186) INFO: emis_tot: 0.2147137757521314 KgCO2/m$^2$ 2023-07-13 18:
+27:51,174 (volttron-boptest-agent-0.0.1 59108) root(186) INFO: ener_tot:
+1.073568878760657 kWh/m$^2$ 2023-07-13 18:27:51,223 (volttron-boptest-agent-
+0.0.1 59108) root(186) INFO: idis_tot: 508.47225004790033 ppmh/zone 2023-07-13
+18:27:51,280 (volttron-boptest-agent-0.0.1 59108) root(186) INFO: pdih_tot:
+None kW/m$^2$ 2023-07-13 18:27:51,330 (volttron-boptest-agent-0.0.1 59108) root
+(186) INFO: pele_tot: None kW/m$^2$ 2023-07-13 18:27:51,381 (volttron-boptest-
+agent-0.0.1 59108) root(186) INFO: pgas_tot: 0.09615811655434148 kW/m$^2$ 2023-
+07-13 18:27:51,436 (volttron-boptest-agent-0.0.1 59108) root(186) INFO:
+tdis_tot: 5.316029375566828 Kh/zone 2023-07-13 18:27:51,494 (volttron-boptest-
+agent-0.0.1 59108) root(186) INFO: time_rat: 0.001856946445725582 s/s 2023-07-
+13 18:27:51,550 (volttron-boptest-agent-0.0.1 59108) root(202) INFO: ========
+run workflow completed.====== 2023-07-13 18:27:51,553 (volttron-boptest-agent-
+0.0.1 59108) (0) INFO: ["======= kpi {'cost_tot': 0.075149821513246,
+'emis_tot': 0.2147137757521314, 'ener_tot': 1.073568878760657, 'idis_tot':
 508.47225004790033, 'pdih_tot': None, 'pele_tot': None, 'pgas_tot':
 0.09615811655434148, 'tdis_tot': 5.316029375566828, 'time_rat':
 0.001856946445725582}"] 2023-07-13 18:27:51,558 (volttron-boptest-agent-0.0.1
 59108) root(129) INFO: =========== refactoring onstart 2023-07-13 18:27:52,067
 (volttron-listener-0.2.0rc0 59096) listener.agent(104) INFO: Peer: pubsub,
 Sender: volttron_boptest_agent:, Bus: , Topic: PNNL/BUILDING/UNIT/kpi, Headers:
 {'min_compatible_version': '3.0', 'max_compatible_version': ''}, Message: ("
```

