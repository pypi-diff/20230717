# Comparing `tmp/scw_gateway-0.6.0.tar.gz` & `tmp/scw_gateway-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.6.0.tar", max compression
+gzip compressed data, was "scw_gateway-0.6.1.tar", max compression
```

## Comparing `scw_gateway-0.6.0.tar` & `scw_gateway-0.6.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     3952 2023-07-13 13:11:32.491560 scw_gateway-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/__init__.py
--rw-r--r--   0        0        0     1900 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/cli.py
--rw-r--r--   0        0        0      824 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/client.py
--rw-r--r--   0        0        0      700 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/consumer.py
--rw-r--r--   0        0        0     1081 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/dev.py
--rw-r--r--   0        0        0     1276 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/domain.py
--rw-r--r--   0        0        0        0 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/human/__init__.py
--rw-r--r--   0        0        0     1971 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/human/errors.py
--rw-r--r--   0        0        0     2633 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/human/progress.py
--rw-r--r--   0        0        0     5201 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/infra.py
--rw-r--r--   0        0        0      627 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/jwt.py
--rw-r--r--   0        0        0      411 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/options.py
--rw-r--r--   0        0        0     1502 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/route.py
--rw-r--r--   0        0        0     3588 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/conf.py
--rw-r--r--   0        0        0       54 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/console.py
--rw-r--r--   0        0        0     9795 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/gateway.py
--rw-r--r--   0        0        0      281 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/__init__.py
--rw-r--r--   0        0        0     5103 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/cockpit.py
--rw-r--r--   0        0        0     6075 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/container.py
--rw-r--r--   0        0        0      519 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/function.py
--rw-r--r--   0        0        0      317 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/image.py
--rw-r--r--   0        0        0    21063 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/manager.py
--rw-r--r--   0        0        0      999 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/rdb.py
--rw-r--r--   0        0        0     2575 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/secrets.py
--rw-r--r--   0        0        0     1901 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/model.py
--rw-r--r--   0        0        0     1181 2023-07-13 13:10:44.262951 scw_gateway-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 scw_gateway-0.6.0/setup.py
--rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 scw_gateway-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2377 2023-07-17 14:09:51.135265 scw_gateway-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3564 2023-07-17 14:09:51.139265 scw_gateway-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/__init__.py
+-rw-r--r--   0        0        0     1900 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/cli.py
+-rw-r--r--   0        0        0      824 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/client.py
+-rw-r--r--   0        0        0      700 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/consumer.py
+-rw-r--r--   0        0        0     1081 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/dev.py
+-rw-r--r--   0        0        0     1276 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/domain.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/human/__init__.py
+-rw-r--r--   0        0        0     1971 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/human/errors.py
+-rw-r--r--   0        0        0     2633 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/human/progress.py
+-rw-r--r--   0        0        0     5201 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/infra.py
+-rw-r--r--   0        0        0      627 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/jwt.py
+-rw-r--r--   0        0        0      411 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/options.py
+-rw-r--r--   0        0        0     1502 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/commands/route.py
+-rw-r--r--   0        0        0     3588 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/conf.py
+-rw-r--r--   0        0        0       54 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/console.py
+-rw-r--r--   0        0        0     9795 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/gateway.py
+-rw-r--r--   0        0        0      281 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/__init__.py
+-rw-r--r--   0        0        0     5103 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/cockpit.py
+-rw-r--r--   0        0        0     6075 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/container.py
+-rw-r--r--   0        0        0      519 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/function.py
+-rw-r--r--   0        0        0      317 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/image.py
+-rw-r--r--   0        0        0    21063 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/manager.py
+-rw-r--r--   0        0        0      999 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/rdb.py
+-rw-r--r--   0        0        0     2575 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/infra/secrets.py
+-rw-r--r--   0        0        0     1901 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/cli/model.py
+-rw-r--r--   0        0        0     1973 2023-07-17 14:09:04.318787 scw_gateway-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4641 1970-01-01 00:00:00.000000 scw_gateway-0.6.1/setup.py
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 scw_gateway-0.6.1/PKG-INFO
```

### Comparing `scw_gateway-0.6.0/README.md` & `scw_gateway-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,29 @@
-# <img src="logo.png" height="32"/> Scaleway Serverless Gateway
+# <img src="https://raw.githubusercontent.com/scaleway/serverless-gateway/main/logo.png" height="32"/> Scaleway Serverless Gateway
 
 [![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)
 [![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)
 [![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)
 
 The Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).
 
 It lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.
 
-It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.
+It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your deployments.
 
 You can read all about it in [this blog post](https://www.scaleway.com/en/blog/api-gateway-early-access/).
 
 If you would like to join in the discussion on how we continue developing the project, or give us feedback, then join us on the [#api-gateway-beta](https://app.slack.com/client/T7YEXCR7X/C05H07VBKJ4) channel on the Scaleway Community Slack.
 
-## :page_with_curl: Contents
+## 📃 Contents
 
-- [ Scaleway Serverless Gateway](#-scaleway-serverless-gateway)
-  - [:page\_with\_curl: Contents](#page_with_curl-contents)
-  - [:computer: Quick-start](#computer-quick-start)
-    - [Deploy your gateway](#deploy-your-gateway)
-    - [Add a route](#add-a-route)
-    - [Delete your gateway](#delete-your-gateway)
-  - [:mortar\_board: Contributing](#mortar_board-contributing)
-  - [:mailbox: Reach us](#mailbox-reach-us)
 
 Please see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.
 
-## :computer: Quick-start
+## 💻 Quickstart
 
 To deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):
 
 ```console
 pip install scw-gateway
 ```
 
@@ -76,19 +68,19 @@
 
 To delete your gateway, you can run:
 
 ```console
 scwgw infra delete
 ```
 
-## :mortar_board: Contributing
+## 🎓 Contributing
 
 We welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).
 
 Do not hesitate to raise issues and pull requests we will have a look at them.
 
-## :mailbox: Reach us
+## 📬 Reach us
 
 We love feedback. Feel free to:
 
 - Open a [Github issue](https://github.com/scaleway/serverless-gateway/issues/new)
 - Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scw_gateway-0.6.0/cli/cli.py` & `scw_gateway-0.6.1/cli/cli.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/client.py` & `scw_gateway-0.6.1/cli/client.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/consumer.py` & `scw_gateway-0.6.1/cli/commands/consumer.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/dev.py` & `scw_gateway-0.6.1/cli/commands/dev.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/domain.py` & `scw_gateway-0.6.1/cli/commands/domain.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/human/errors.py` & `scw_gateway-0.6.1/cli/commands/human/errors.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/human/progress.py` & `scw_gateway-0.6.1/cli/commands/human/progress.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/infra.py` & `scw_gateway-0.6.1/cli/commands/infra.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/jwt.py` & `scw_gateway-0.6.1/cli/commands/jwt.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/commands/route.py` & `scw_gateway-0.6.1/cli/commands/route.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/conf.py` & `scw_gateway-0.6.1/cli/conf.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/gateway.py` & `scw_gateway-0.6.1/cli/gateway.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/infra/cockpit.py` & `scw_gateway-0.6.1/cli/infra/cockpit.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/infra/container.py` & `scw_gateway-0.6.1/cli/infra/container.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/infra/function.py` & `scw_gateway-0.6.1/cli/infra/function.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/infra/manager.py` & `scw_gateway-0.6.1/cli/infra/manager.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/infra/rdb.py` & `scw_gateway-0.6.1/cli/infra/rdb.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/infra/secrets.py` & `scw_gateway-0.6.1/cli/infra/secrets.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/cli/model.py` & `scw_gateway-0.6.1/cli/model.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.6.0/setup.py` & `scw_gateway-0.6.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,22 @@
  'scaleway>=0.12.0,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['scwgw = cli.cli:main']}
 
 setup_kwargs = {
     'name': 'scw-gateway',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem',
-    'long_description': '# <img src="logo.png" height="32"/> Scaleway Serverless Gateway\n\n[![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)\n[![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)\n[![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)\n\nThe Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).\n\nIt lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.\n\nIt is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.\n\nYou can read all about it in [this blog post](https://www.scaleway.com/en/blog/api-gateway-early-access/).\n\nIf you would like to join in the discussion on how we continue developing the project, or give us feedback, then join us on the [#api-gateway-beta](https://app.slack.com/client/T7YEXCR7X/C05H07VBKJ4) channel on the Scaleway Community Slack.\n\n## :page_with_curl: Contents\n\n- [ Scaleway Serverless Gateway](#-scaleway-serverless-gateway)\n  - [:page\\_with\\_curl: Contents](#page_with_curl-contents)\n  - [:computer: Quick-start](#computer-quick-start)\n    - [Deploy your gateway](#deploy-your-gateway)\n    - [Add a route](#add-a-route)\n    - [Delete your gateway](#delete-your-gateway)\n  - [:mortar\\_board: Contributing](#mortar_board-contributing)\n  - [:mailbox: Reach us](#mailbox-reach-us)\n\nPlease see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.\n\n## :computer: Quick-start\n\nTo deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):\n\n```console\npip install scw-gateway\n```\n\nOnce done, the following steps can be run from the root of the project, and will deploy the gateway as a Serverless Container in your Scaleway account.\n\nThe gateway image itself is packaged via our public [Serverless Gateway Docker image](https://hub.docker.com/r/scaleway/serverless-gateway).\n\n### Deploy your gateway\n\nTo deploy your gateway, you can run:\n\n```console\nscwgw infra deploy\n```\n\nFor more information on the deployment process, see the [deployment docs](https://serverless-gateway.readthedocs.io/en/latest/deployment.html).\n\n### Add a route\n\nTo check your gateway is working, you can add and remove a route:\n\n```console\n# Check no routes are configured initially\nscwgw route ls\n\n# Check the response directly from a given URL\nTARGET_URL=http://worldtimeapi.org/api/timezone/Europe/Paris\ncurl $TARGET_URL\n\n# Add a route to this URL in your gateway\nscwgw route add /time $TARGET_URL\n\n# List routes to see that it\'s been configured\nscwgw route ls\n\n# Curl the URL via the gateway\nGATEWAY_ENDPOINT=$(scwgw infra endpoint)\ncurl https://${GATEWAY_ENDPOINT}/time\n```\n\n### Delete your gateway\n\nTo delete your gateway, you can run:\n\n```console\nscwgw infra delete\n```\n\n## :mortar_board: Contributing\n\nWe welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).\n\nDo not hesitate to raise issues and pull requests we will have a look at them.\n\n## :mailbox: Reach us\n\nWe love feedback. Feel free to:\n\n- Open a [Github issue](https://github.com/scaleway/serverless-gateway/issues/new)\n- Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.\n',
+    'long_description': '# <img src="https://raw.githubusercontent.com/scaleway/serverless-gateway/main/logo.png" height="32"/> Scaleway Serverless Gateway\n\n[![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)\n[![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)\n[![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)\n\nThe Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).\n\nIt lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.\n\nIt is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your deployments.\n\nYou can read all about it in [this blog post](https://www.scaleway.com/en/blog/api-gateway-early-access/).\n\nIf you would like to join in the discussion on how we continue developing the project, or give us feedback, then join us on the [#api-gateway-beta](https://app.slack.com/client/T7YEXCR7X/C05H07VBKJ4) channel on the Scaleway Community Slack.\n\n## 📃 Contents\n\n\nPlease see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.\n\n## 💻 Quickstart\n\nTo deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):\n\n```console\npip install scw-gateway\n```\n\nOnce done, the following steps can be run from the root of the project, and will deploy the gateway as a Serverless Container in your Scaleway account.\n\nThe gateway image itself is packaged via our public [Serverless Gateway Docker image](https://hub.docker.com/r/scaleway/serverless-gateway).\n\n### Deploy your gateway\n\nTo deploy your gateway, you can run:\n\n```console\nscwgw infra deploy\n```\n\nFor more information on the deployment process, see the [deployment docs](https://serverless-gateway.readthedocs.io/en/latest/deployment.html).\n\n### Add a route\n\nTo check your gateway is working, you can add and remove a route:\n\n```console\n# Check no routes are configured initially\nscwgw route ls\n\n# Check the response directly from a given URL\nTARGET_URL=http://worldtimeapi.org/api/timezone/Europe/Paris\ncurl $TARGET_URL\n\n# Add a route to this URL in your gateway\nscwgw route add /time $TARGET_URL\n\n# List routes to see that it\'s been configured\nscwgw route ls\n\n# Curl the URL via the gateway\nGATEWAY_ENDPOINT=$(scwgw infra endpoint)\ncurl https://${GATEWAY_ENDPOINT}/time\n```\n\n### Delete your gateway\n\nTo delete your gateway, you can run:\n\n```console\nscwgw infra delete\n```\n\n## 🎓 Contributing\n\nWe welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).\n\nDo not hesitate to raise issues and pull requests we will have a look at them.\n\n## 📬 Reach us\n\nWe love feedback. Feel free to:\n\n- Open a [Github issue](https://github.com/scaleway/serverless-gateway/issues/new)\n- Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.\n',
     'author': 'Simon Shillaker',
     'author_email': 'sshillaker@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/scaleway/serverless-gateway',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scw_gateway-0.6.0/PKG-INFO` & `scw_gateway-0.6.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 Metadata-Version: 2.1
 Name: scw-gateway
-Version: 0.6.0
+Version: 0.6.1
 Summary: CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem
+Home-page: https://github.com/scaleway/serverless-gateway
+Keywords: serverless,scaleway,gateway,cloud,caas
 Author: Simon Shillaker
 Author-email: sshillaker@scaleway.com
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scaleway (>=0.12.0,<0.13.0)
+Project-URL: Documentation, https://serverless-gateway.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/scaleway/serverless-gateway
 Description-Content-Type: text/markdown
 
-# <img src="logo.png" height="32"/> Scaleway Serverless Gateway
+# <img src="https://raw.githubusercontent.com/scaleway/serverless-gateway/main/logo.png" height="32"/> Scaleway Serverless Gateway
 
 [![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)
 [![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)
 [![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)
 
 The Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).
 
 It lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.
 
-It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.
+It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your deployments.
 
 You can read all about it in [this blog post](https://www.scaleway.com/en/blog/api-gateway-early-access/).
 
 If you would like to join in the discussion on how we continue developing the project, or give us feedback, then join us on the [#api-gateway-beta](https://app.slack.com/client/T7YEXCR7X/C05H07VBKJ4) channel on the Scaleway Community Slack.
 
-## :page_with_curl: Contents
+## 📃 Contents
 
-- [ Scaleway Serverless Gateway](#-scaleway-serverless-gateway)
-  - [:page\_with\_curl: Contents](#page_with_curl-contents)
-  - [:computer: Quick-start](#computer-quick-start)
-    - [Deploy your gateway](#deploy-your-gateway)
-    - [Add a route](#add-a-route)
-    - [Delete your gateway](#delete-your-gateway)
-  - [:mortar\_board: Contributing](#mortar_board-contributing)
-  - [:mailbox: Reach us](#mailbox-reach-us)
 
 Please see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.
 
-## :computer: Quick-start
+## 💻 Quickstart
 
 To deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):
 
 ```console
 pip install scw-gateway
 ```
 
@@ -94,20 +99,20 @@
 
 To delete your gateway, you can run:
 
 ```console
 scwgw infra delete
 ```
 
-## :mortar_board: Contributing
+## 🎓 Contributing
 
 We welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).
 
 Do not hesitate to raise issues and pull requests we will have a look at them.
 
-## :mailbox: Reach us
+## 📬 Reach us
 
 We love feedback. Feel free to:
 
 - Open a [Github issue](https://github.com/scaleway/serverless-gateway/issues/new)
 - Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

