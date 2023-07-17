# Comparing `tmp/fastapi-serve-0.0.2.dev9.tar.gz` & `tmp/fastapi-serve-0.0.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.2.dev9.tar", last modified: Wed Jul 12 15:32:10 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.3.dev5.tar", last modified: Mon Jul 17 17:13:14 2023, max compression
```

## Comparing `fastapi-serve-0.0.2.dev9.tar` & `fastapi-serve-0.0.3.dev5.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.656826 fastapi-serve-0.0.3.dev5/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/setup.py
```

### Comparing `fastapi-serve-0.0.2.dev9/LICENSE` & `fastapi-serve-0.0.3.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev9/PKG-INFO` & `fastapi-serve-0.0.3.dev5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,82 @@
-Metadata-Version: 2.1
-Name: fastapi-serve
-Version: 0.0.2.dev9
-Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
-Home-page: https://github.com/jina-ai/fastapi-serve/
-Author: Jina AI
-Author-email: hello@jina.ai
-License: Apache 2.0
-Download-URL: https://github.com/jina-ai/fastapi-serve/tags
-Project-URL: Documentation, https://docs.jina.ai
-Project-URL: Source, https://github.com/jina-ai/fastapi-serve/
-Project-URL: Tracker, https://github.com/jina-ai/fastapi-serve/issues
-Keywords: jina fastapi restapi cloud docker kubernetes
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <p align="center">
 <h2 align="center">FastAPI-Serve: FastAPI to the Cloud, Batteries Included! ☁️🔋🚀</h2>
 </p>
 
 <p align=center>
 <a href="https://pypi.org/project/fastapi-serve/"><img alt="PyPI" src="https://img.shields.io/pypi/v/fastapi-serve?label=Release&style=flat-square"></a>
 <a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
 <a href="https://pypistats.org/packages/fastapi-serve"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/fastapi-serve?style=flat-square"></a>
 <a href="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml"><img alt="Github CD status" src="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml/badge.svg"></a>
 </p>
 
 Welcome to **fastapi-serve**, a framework designed to take the pain out of deploying your local FastAPI applications to the cloud. Built using our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` offers out-of-the-box support for automated deployments on `cloud.jina.ai`, our scalable and robust cloud platform. 🌩️ 
 
-## Features 😍 
+## 😍 Features 
 
-- 🌐 **DNS**: Automatic URL generation for your app.
+- 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
 - ↕️ **Scaling**: Scale your app manuallly or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Tailor your deployment to suit specific needs.
-- 💾 **Storage**: Persistent and secure network storage.
+- 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
+- 💾 **App Storage**: Persistent and secure network storage for your app data.
+- 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces.
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
 
-## Requirements 📋 
-
-To use `fastapi-serve`, you need to have:
-
-- Python 3.7 or higher
-
-## Getting Started 💡
+## 💡 Getting Started
 
 First, install the `fastapi-serve` package using pip:
 
 ```bash
 pip install fastapi-serve
 ```
 
 Then, simply use the `fastapi-serve` command to deploy your FastAPI application:
 
 ```bash
-fastapi-serve .
+fastapi-serve deploy jcloud app:app
 ```
 
-You can also specify the name of your app:
+You'll get a URL to access your newly deployed application along with the Swagger UI.
 
-```bash
-fastapi-serve . --name my_awesome_app
-```
+## 📚 Examples
+
+We have a few examples to help you get acquainted with `fastapi-serve`:
+
+- 🚀 [Deploy a Simple FastAPI Application](examples/simple/)
+- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](examples/rate_limit/)
+- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](examples/authorization/)
+- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](examples/file_handling/)
 
-You'll get a URL to access your newly deployed application. 🎉 
 
-## Support 💪 
+## 🖥️ `fastapi-serve` CLI 
 
-If you encounter any problems or have questions, feel free to open an issue on the GitHub repository or reach out to us directly at support@jina.ai.
+`fastapi-serve` comes with a simple CLI that allows you to deploy your FastAPI applications to the cloud with ease.
 
-## Contribute 🤝 
+| Description | Command | 
+| --- | ---: |
+| Deploy your app locally | `fastapi-serve deploy local app:app` |
+| Deploy your app on JCloud | `fastapi-serve deploy jcloud app:app` |
+| Update existing app on JCloud | `fastapi-serve deploy jcloud app:app --app-id <app-id>` |
+| Get app status on JCloud | `fastapi-serve status <app-id>` |
+| List all apps on JCloud | `fastapi-serve list` |
+| Remove app on JCloud | `fastapi-serve remove <app-id>` |
+
+
+## ⚙️💰 Configuration and Pricing
+
+Read our [Configuration & Pricing Guide](examples/CONFIG.MD) to learn more about the various configuration options available to you and the pricing model for `fastapi-serve`.
+
+## 💪 Support
+
+If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
 
-We welcome all contributions! If you're interested in contributing, please refer to our [Contribution Guide](CONTRIBUTING.md) for details.
 
 ## Our Cloud Platform 🌐 
 
 `cloud.jina.ai` is our robust and scalable cloud platform designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
 
 ---
 
 `fastapi-serve` is more than just a deployment tool, it's a bridge that connects your local development environment with our powerful cloud infrastructure. Start using `fastapi-serve` today, and experience the joy of effortless deployments! 🎊 
-
-
```

#### html2text {}

```diff
@@ -1,53 +1,51 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev9 Summary: FastAPI
-Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
-github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
-License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
-Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
-github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
-jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
-kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Environment ::
-Console Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Description-Content-Type: text/markdown
-Provides-Extra: test License-File: LICENSE
  ***** FastAPI-Serve: FastAPI to the Cloud, Batteries Included! âï¸ðð
                                      *****
                     [PyPI] [https://img.shields.io/discord/
   1106542220112302130?logo=discord&logoColor=white&style=flat-square] [PyPI_-
              Downloads_from_official_pypistats] [Github_CD_status]
 Welcome to **fastapi-serve**, a framework designed to take the pain out of
 deploying your local FastAPI applications to the cloud. Built using our open-
 source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve`
 offers out-of-the-box support for automated deployments on `cloud.jina.ai`, our
-scalable and robust cloud platform. ð©ï¸ ## Features ð - ð **DNS**:
-Automatic URL generation for your app. - ð **Protocols**: Full compatibility
-with HTTP, WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app
-manuallly or let it auto-scale based on RPS, CPU, and Memory. - ðï¸
-**Secrets**: Secure handling of secrets and environment variables. - ðï¸
-**Hardware**: Tailor your deployment to suit specific needs. - ð¾
-**Storage**: Persistent and secure network storage. - ð **Observability**:
-Integrated access to logs, metrics, and traces. - ð¦ **Containerization**:
-Effortless containerization of your Python codebase with our integrated
-registry. ## Requirements ð To use `fastapi-serve`, you need to have: -
-Python 3.7 or higher ## Getting Started ð¡ First, install the `fastapi-serve`
-package using pip: ```bash pip install fastapi-serve ``` Then, simply use the
-`fastapi-serve` command to deploy your FastAPI application: ```bash fastapi-
-serve . ``` You can also specify the name of your app: ```bash fastapi-serve .
---name my_awesome_app ``` You'll get a URL to access your newly deployed
-application. ð ## Support ðª If you encounter any problems or have
-questions, feel free to open an issue on the GitHub repository or reach out to
-us directly at support@jina.ai. ## Contribute ð¤ We welcome all
-contributions! If you're interested in contributing, please refer to our
-[Contribution Guide](CONTRIBUTING.md) for details. ## Our Cloud Platform ð
+scalable and robust cloud platform. ð©ï¸ ## ð Features - ð **HTTPS**:
+Auto-provisioned DNS and TLS certificates for your app. - ð **Protocols**:
+Full compatibility with HTTP, WebSocket, and GraphQL. - âï¸ **Scaling**:
+Scale your app manuallly or let it auto-scale based on RPS, CPU, and Memory. -
+ðï¸ **Secrets**: Secure handling of secrets and environment variables. -
+ðï¸ **Hardware**: Tailor your deployment to suit specific needs. - ð
+**Authorization**: Built-in OAuth2.0 token-based security to secure your
+endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
+your app data. - ð **Blob Storage**: Built-in support for seamless user file
+uploads and downloads. - ð **Observability**: Integrated access to logs,
+metrics, and traces. - ð¦ **Containerization**: Effortless containerization
+of your Python codebase with our integrated registry. ## ð¡ Getting Started
+First, install the `fastapi-serve` package using pip: ```bash pip install
+fastapi-serve ``` Then, simply use the `fastapi-serve` command to deploy your
+FastAPI application: ```bash fastapi-serve deploy jcloud app:app ``` You'll get
+a URL to access your newly deployed application along with the Swagger UI. ##
+ð Examples We have a few examples to help you get acquainted with `fastapi-
+serve`: - ð [Deploy a Simple FastAPI Application](examples/simple/) -
+ðï¸ [Use Secrets for Redis-Powered Rate Limiting](examples/rate_limit/) -
+ð [Secure Your Endpoints with built-in OAuth2.0 Authorization](examples/
+authorization/) - ð [Handle File Uploads and Downloads with built-in Blob
+Storage](examples/file_handling/) ## ð¥ï¸ `fastapi-serve` CLI `fastapi-
+serve` comes with a simple CLI that allows you to deploy your FastAPI
+applications to the cloud with ease. | Description | Command | | --- | ---: | |
+Deploy your app locally | `fastapi-serve deploy local app:app` | | Deploy your
+app on JCloud | `fastapi-serve deploy jcloud app:app` | | Update existing app
+on JCloud | `fastapi-serve deploy jcloud app:app --app-id ` | | Get app status
+on JCloud | `fastapi-serve status ` | | List all apps on JCloud | `fastapi-
+serve list` | | Remove app on JCloud | `fastapi-serve remove ` | ## âï¸ð°
+Configuration and Pricing Read our [Configuration & Pricing Guide](examples/
+CONFIG.MD) to learn more about the various configuration options available to
+you and the pricing model for `fastapi-serve`. ## ðª Support If you encounter
+any problems or have questions, feel free to open an issue on the GitHub
+repository. You can also join our [Discord](https://discord.jina.ai/) to get
+help from our community members and the Jina team. ## Our Cloud Platform ð
 `cloud.jina.ai` is our robust and scalable cloud platform designed to run your
 FastAPI applications with minimum hassle and maximum efficiency. With features
 like auto-scaling, integrated observability, and automated containerization, it
 provides a seamless and worry-free deployment experience. --- `fastapi-serve`
 is more than just a deployment tool, it's a bridge that connects your local
 development environment with our powerful cloud infrastructure. Start using
 `fastapi-serve` today, and experience the joy of effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/__main__.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 import click
 
 from fastapi_serve import __version__
 from fastapi_serve.cloud import (
+    get_app_status_on_jcloud,
     get_jinaai_uri,
-    hubble_options,
-    jcloud_options,
+    hubble_push_options,
+    jcloud_deploy_options,
+    jcloud_list_options,
+    list_apps_on_jcloud,
     push_app_to_hubble,
+    remove_app_on_jcloud,
     serve_on_jcloud,
 )
 from fastapi_serve.helper import syncify
 
 
 @click.group()
 @click.version_option(__version__, "-v", "--version", prog_name="fastapi-serve")
 @click.help_option("-h", "--help")
 def serve():
     """FastAPI Serve - FastAPI to the Cloud, Batteries Included! ☁️🔋🚀"""
     pass
 
 
 @serve.command(help="Push the app image to Jina AI Cloud")
-@hubble_options
+@hubble_push_options
 @click.help_option("-h", "--help")
-def push(
-    app,
-    app_dir,
-    image_name,
-    image_tag,
-    platform,
-    version,
-    verbose,
-    public,
-):
+def push(app, app_dir, image_name, image_tag, platform, version, verbose, public):
     _gateway_id = push_app_to_hubble(
         app=app,
         app_dir=app_dir,
         image_name=image_name,
         tag=image_tag,
         platform=platform,
         version=version,
@@ -43,47 +38,82 @@
         public=public,
     )
     _id, _tag = _gateway_id.split(':')
     _uri = click.style(get_jinaai_uri(_id, _tag), fg="green")
     click.echo(f'Pushed to Jina AI Cloud. Please use {_uri} to deploy.')
 
 
-@serve.command(help="Deploy the app image to Jina AI Cloud")
-@jcloud_options
+@serve.group(help="Deploy the app.")
 @click.help_option("-h", "--help")
+def deploy():
+    pass
+
+
+@deploy.command(help="Deploy the app locally")
+@click.help_option("-h", "--help")
+@syncify
+async def local():
+    pass
+
+
+@deploy.command(help="Deploy the app to Jina AI Cloud")
+@jcloud_deploy_options
 @syncify
-async def deploy(
+async def jcloud(
     app,
     app_dir,
     name,
     uses,
     app_id,
     version,
     timeout,
     platform,
     config,
     cors,
     env,
+    secret,
     verbose,
     public,
-    secret,
 ):
     await serve_on_jcloud(
         app=app,
         app_dir=app_dir,
         name=name,
         uses=uses,
         app_id=app_id,
         version=version,
         timeout=timeout,
         platform=platform,
         config=config,
         cors=cors,
         env=env,
+        secret=secret,
         verbose=verbose,
         public=public,
-        secret=secret,
     )
 
 
+@serve.command(help='List all deployed apps.')
+@jcloud_list_options
+@syncify
+async def list(phase, name):
+    await list_apps_on_jcloud(phase=phase, name=name)
+
+
+@serve.command(help='Get status of a deployed app.')
+@click.argument('app-id')
+@click.help_option('-h', '--help')
+@syncify
+async def status(app_id):
+    await get_app_status_on_jcloud(app_id)
+
+
+@serve.command(help='Remove an app.')
+@click.argument('app-id')
+@click.help_option('-h', '--help')
+@syncify
+async def remove(app_id):
+    await remove_app_on_jcloud(app_id)
+
+
 if __name__ == "__main__":
     serve()
```

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,22 +179,22 @@
         raise click.BadParameter(
             f"Invalid disk size '{e.disk_size}' found in config file."
         )
 
     return value
 
 
-def resolve_jcloud_config(config, module_dir: str):
+def resolve_jcloud_config(config, app_dir: str):
     # config given from CLI takes higher priority
     if config:
         return config
 
     # Check to see if jcloud YAML/YML file exists at app dir
-    config_path_yml = os.path.join(module_dir, "jcloud.yml")
-    config_path_yaml = os.path.join(module_dir, "jcloud.yaml")
+    config_path_yml = os.path.join(app_dir, "jcloud.yml")
+    config_path_yaml = os.path.join(app_dir, "jcloud.yaml")
 
     if os.path.exists(config_path_yml):
         config_path = config_path_yml
     elif os.path.exists(config_path_yaml):
         config_path = config_path_yaml
     else:
         return None
```

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/deploy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import os
 from tempfile import TemporaryDirectory
 from typing import Dict, List, Tuple
 
 import yaml
+from dotenv import dotenv_values
 
 from fastapi_serve.cloud.config import (
     APP_LOGS_URL,
     APP_NAME,
     DEFAULT_LABEL,
     DEFAULT_TIMEOUT,
     DOCARRAY_VERSION,
     JINA_VERSION,
     PRICING_URL,
     get_jcloud_config,
 )
-from fastapi_serve.helper import asyncio_run_property
+from fastapi_serve.helper import (
+    EnvironmentVarCtxtManager,
+    asyncio_run_property,
+    get_random_name,
+)
+from fastapi_serve.utils.helper import FlowUserEnvVar, get_jina_userid
 
 
 def get_gateway_config_yaml_path() -> str:
     return os.path.join(os.path.dirname(__file__), 'config.yml')
 
 
 def get_gateway_uses(id: str) -> str:
@@ -105,18 +111,19 @@
         jcloud_config = get_jcloud_config(
             config_path=jcloud_config_path, timeout=timeout, is_websocket=is_websocket
         )
 
     _envs = {}
     if env is not None:
         # read env file and load to _envs dict
-        from dotenv import dotenv_values
-
         _envs = dict(dotenv_values(env))
 
+    # add userid to _envs dict
+    _envs.update({FlowUserEnvVar: get_jina_userid()})
+
     uses = get_gateway_uses(id=gateway_id) if jcloud else get_gateway_config_yaml_path()
     flow_dict = {
         'jtype': 'Flow',
         **(get_with_args_for_jcloud(cors, _envs) if jcloud else {}),
         'gateway': {
             'uses': uses,
             'uses_with': {
@@ -171,16 +178,14 @@
         sort_keys=False,
     )
 
 
 async def deploy_app_on_jcloud(
     flow_dict: Dict, app_id: str = None, verbose: bool = False
 ) -> Tuple[str, str]:
-    from fastapi_serve.helper import EnvironmentVarCtxtManager
-
     os.environ['JCLOUD_LOGLEVEL'] = 'INFO' if verbose else 'ERROR'
 
     from jcloud.flow import CloudFlow
 
     with TemporaryDirectory() as tmpdir:
         flow_path = os.path.join(tmpdir, 'flow.yml')
         with open(flow_path, 'w') as f:
@@ -199,14 +204,37 @@
         for k, v in jcloud_flow.endpoints.items():
             if k.lower() == 'gateway (http)' or k.lower() == 'gateway (websocket)':
                 return app_id, v
 
     return None, None
 
 
+async def patch_secret_on_jcloud(
+    flow_dict: Dict, app_id: str, secret: str, verbose: bool = False
+):
+    os.environ['JCLOUD_LOGLEVEL'] = 'INFO' if verbose else 'ERROR'
+
+    from jcloud.flow import CloudFlow
+
+    with TemporaryDirectory() as tmpdir:
+        flow_path = os.path.join(tmpdir, 'flow.yml')
+        with open(flow_path, 'w') as f:
+            yaml.safe_dump(flow_dict, f, sort_keys=False)
+
+        deploy_envs = {'JCLOUD_HIDE_SUCCESS_MSG': 'true'} if not verbose else {}
+        with EnvironmentVarCtxtManager(deploy_envs):
+            jcloud_flow = CloudFlow(path=flow_path, flow_id=app_id)
+            secrets_values = dict(dotenv_values(secret))
+            await jcloud_flow.create_secret(
+                secret_name=get_random_name(),
+                env_secret_data=secrets_values,
+                update=True,  # Important to update the Flow with the new secret
+            )
+
+
 async def get_app_status_on_jcloud(app_id: str):
     from jcloud.flow import CloudFlow
     from rich import box
     from rich.align import Align
     from rich.console import Console
     from rich.markdown import Markdown
     from rich.table import Table
@@ -285,15 +313,15 @@
         box=box.ROUNDED,
         highlight=True,
     )
 
     console = Console()
     with console.status(f'[bold]Listing all apps'):
         all_apps = await CloudFlow().list_all(
-            phase=phase, name=name, labels=f'app={APP_NAME}'
+            phase=phase, name=name, labels=f'app={DEFAULT_LABEL}'
         )
         if not all_apps:
             print('No apps found')
             return
 
         def _get_endpoint(app):
             endpoints = app.get('status', {}).get('endpoints', {})
@@ -318,58 +346,74 @@
 
 
 async def serve_on_jcloud(
     app: str,
     app_dir: str = None,
     name: str = APP_NAME,
     uses: str = None,
-    requirements: List[str] = None,
     app_id: str = None,
     version: str = 'latest',
     timeout: int = DEFAULT_TIMEOUT,
     platform: str = None,
     config: str = None,
     cors: bool = True,
     env: str = None,
+    secret: str = None,  # TODO: add support for secret
     verbose: bool = False,
     public: bool = False,
 ) -> str:
     from fastapi_serve.cloud.build import get_app_dir, push_app_to_hubble
     from fastapi_serve.cloud.config import resolve_jcloud_config
     from fastapi_serve.helper import get_random_tag
 
     app_dir, is_websocket = get_app_dir(app=app, app_dir=app_dir)
     config = resolve_jcloud_config(config=config, app_dir=app_dir)
 
     if uses is not None:
+        # If `uses` is provided, use it as gateway id
         gateway_id = uses
     else:
+        # If `uses` is not provided, push the app to hubble and get the gateway id
         gateway_id = push_app_to_hubble(
             app=app,
             app_dir=app_dir,
-            requirements=requirements,
             tag=get_random_tag(),
             version=version,
             platform=platform,
             verbose=verbose,
             public=public,
         )
 
+    # Get the flow dict
+    flow_dict = get_flow_dict(
+        app=app,
+        jcloud=True,
+        port=8080,
+        name=name,
+        timeout=timeout,
+        app_id=app_id,
+        gateway_id=gateway_id,
+        is_websocket=is_websocket,
+        jcloud_config_path=config,
+        cors=cors,
+        env=env,
+    )
+
+    # Deploy the app
     app_id, _ = await deploy_app_on_jcloud(
-        flow_dict=get_flow_dict(
-            app=app,
-            jcloud=True,
-            port=8080,
-            name=name,
-            timeout=timeout,
-            app_id=app_id,
-            gateway_id=gateway_id,
-            is_websocket=is_websocket,
-            jcloud_config_path=config,
-            cors=cors,
-            env=env,
-        ),
+        flow_dict=flow_dict,
         app_id=app_id,
         verbose=verbose,
     )
+
+    # If secret is not None, create a secret and update the app
+    if secret is not None:
+        await patch_secret_on_jcloud(
+            flow_dict=flow_dict,
+            app_id=app_id,
+            secret=secret,
+            verbose=verbose,
+        )
+
+    # Show the app status
     await get_app_status_on_jcloud(app_id=app_id)
     return app_id
```

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import click
+from jcloud.constants import Phase
 
 from fastapi_serve.cloud.config import (
     APP_NAME,
     DEFAULT_TIMEOUT,
     validate_jcloud_config_callback,
 )
 
+_help_option = [click.help_option('-h', '--help')]
+
 _common_options = [
     click.argument(
         'app',
         type=str,
         required=True,
     ),
     click.option(
@@ -119,22 +122,60 @@
         is_flag=True,
         help='Enable CORS.',
         default=True,
         show_default=True,
     ),
 ]
 
+_jcloud_list_options = [
+    click.option(
+        '--phase',
+        type=str,
+        default=','.join(
+            [
+                Phase.Serving,
+                Phase.Failed,
+                Phase.Starting,
+                Phase.Updating,
+                Phase.Paused,
+            ]
+        ),
+        help='Deployment phase for the app.',
+        show_default=True,
+    ),
+    click.option(
+        '--name',
+        type=str,
+        default=None,
+        help='Name of the app.',
+        show_default=True,
+    ),
+]
+
+
+__all__ = [
+    'hubble_push_options',
+    'jcloud_deploy_options',
+    'jcloud_list_options',
+]
 
-def hubble_options(func):
+
+def hubble_push_options(func):
     for option in reversed(
-        _common_options + _hubble_only_options + _hubble_common_options
+        _common_options + _hubble_only_options + _hubble_common_options + _help_option
     ):
         func = option(func)
     return func
 
 
-def jcloud_options(func):
+def jcloud_deploy_options(func):
     for option in reversed(
-        _common_options + _jcloud_only_options + _hubble_common_options
+        _common_options + _jcloud_only_options + _hubble_common_options + _help_option
     ):
         func = option(func)
     return func
+
+
+def jcloud_list_options(func):
+    for option in reversed(_jcloud_list_options + _help_option):
+        func = option(func)
+    return func
```

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,28 +53,28 @@
 
     def _init_fastapi_app(self):
         with EnvironmentVarCtxtManager({'JCLOUD_WORKSPACE': self.workspace}):
             self.logger.info(f"Loading app from {self._app_str}")
             self._app, _ = import_from_string(self._app_str)
 
     def _configure_cors(self):
+        from fastapi.middleware.cors import CORSMiddleware
+
         if self.cors:
             if any(
                 [
                     isinstance(middleware, CORSMiddleware)
                     for middleware in self._app.user_middleware
                 ]
             ):
                 self.logger.warning("CORS is already enabled")
                 return
 
             else:
                 self.logger.info("Enabling CORS")
-                from fastapi.middleware.cors import CORSMiddleware
-
                 self._app.add_middleware(
                     CORSMiddleware,
                     allow_origins=["*"],
                     allow_credentials=True,
                     allow_methods=["*"],
                     allow_headers=["*"],
                 )
```

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve/helper.py` & `fastapi-serve-0.0.3.dev5/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.3.dev5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev9
+Version: 0.0.3.dev5
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -37,60 +37,75 @@
 <a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
 <a href="https://pypistats.org/packages/fastapi-serve"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/fastapi-serve?style=flat-square"></a>
 <a href="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml"><img alt="Github CD status" src="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml/badge.svg"></a>
 </p>
 
 Welcome to **fastapi-serve**, a framework designed to take the pain out of deploying your local FastAPI applications to the cloud. Built using our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` offers out-of-the-box support for automated deployments on `cloud.jina.ai`, our scalable and robust cloud platform. 🌩️ 
 
-## Features 😍 
+## 😍 Features 
 
-- 🌐 **DNS**: Automatic URL generation for your app.
+- 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
 - ↕️ **Scaling**: Scale your app manuallly or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Tailor your deployment to suit specific needs.
-- 💾 **Storage**: Persistent and secure network storage.
+- 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
+- 💾 **App Storage**: Persistent and secure network storage for your app data.
+- 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces.
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
 
-## Requirements 📋 
-
-To use `fastapi-serve`, you need to have:
-
-- Python 3.7 or higher
-
-## Getting Started 💡
+## 💡 Getting Started
 
 First, install the `fastapi-serve` package using pip:
 
 ```bash
 pip install fastapi-serve
 ```
 
 Then, simply use the `fastapi-serve` command to deploy your FastAPI application:
 
 ```bash
-fastapi-serve .
+fastapi-serve deploy jcloud app:app
 ```
 
-You can also specify the name of your app:
+You'll get a URL to access your newly deployed application along with the Swagger UI.
+
+## 📚 Examples
+
+We have a few examples to help you get acquainted with `fastapi-serve`:
+
+- 🚀 [Deploy a Simple FastAPI Application](examples/simple/)
+- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](examples/rate_limit/)
+- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](examples/authorization/)
+- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](examples/file_handling/)
+
+
+## 🖥️ `fastapi-serve` CLI 
+
+`fastapi-serve` comes with a simple CLI that allows you to deploy your FastAPI applications to the cloud with ease.
+
+| Description | Command | 
+| --- | ---: |
+| Deploy your app locally | `fastapi-serve deploy local app:app` |
+| Deploy your app on JCloud | `fastapi-serve deploy jcloud app:app` |
+| Update existing app on JCloud | `fastapi-serve deploy jcloud app:app --app-id <app-id>` |
+| Get app status on JCloud | `fastapi-serve status <app-id>` |
+| List all apps on JCloud | `fastapi-serve list` |
+| Remove app on JCloud | `fastapi-serve remove <app-id>` |
 
-```bash
-fastapi-serve . --name my_awesome_app
-```
 
-You'll get a URL to access your newly deployed application. 🎉 
+## ⚙️💰 Configuration and Pricing
 
-## Support 💪 
+Read our [Configuration & Pricing Guide](examples/CONFIG.MD) to learn more about the various configuration options available to you and the pricing model for `fastapi-serve`.
 
-If you encounter any problems or have questions, feel free to open an issue on the GitHub repository or reach out to us directly at support@jina.ai.
+## 💪 Support
 
-## Contribute 🤝 
+If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
 
-We welcome all contributions! If you're interested in contributing, please refer to our [Contribution Guide](CONTRIBUTING.md) for details.
 
 ## Our Cloud Platform 🌐 
 
 `cloud.jina.ai` is our robust and scalable cloud platform designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev9 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev5 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -20,34 +20,49 @@
                     [PyPI] [https://img.shields.io/discord/
   1106542220112302130?logo=discord&logoColor=white&style=flat-square] [PyPI_-
              Downloads_from_official_pypistats] [Github_CD_status]
 Welcome to **fastapi-serve**, a framework designed to take the pain out of
 deploying your local FastAPI applications to the cloud. Built using our open-
 source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve`
 offers out-of-the-box support for automated deployments on `cloud.jina.ai`, our
-scalable and robust cloud platform. ð©ï¸ ## Features ð - ð **DNS**:
-Automatic URL generation for your app. - ð **Protocols**: Full compatibility
-with HTTP, WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app
-manuallly or let it auto-scale based on RPS, CPU, and Memory. - ðï¸
-**Secrets**: Secure handling of secrets and environment variables. - ðï¸
-**Hardware**: Tailor your deployment to suit specific needs. - ð¾
-**Storage**: Persistent and secure network storage. - ð **Observability**:
-Integrated access to logs, metrics, and traces. - ð¦ **Containerization**:
-Effortless containerization of your Python codebase with our integrated
-registry. ## Requirements ð To use `fastapi-serve`, you need to have: -
-Python 3.7 or higher ## Getting Started ð¡ First, install the `fastapi-serve`
-package using pip: ```bash pip install fastapi-serve ``` Then, simply use the
-`fastapi-serve` command to deploy your FastAPI application: ```bash fastapi-
-serve . ``` You can also specify the name of your app: ```bash fastapi-serve .
---name my_awesome_app ``` You'll get a URL to access your newly deployed
-application. ð ## Support ðª If you encounter any problems or have
-questions, feel free to open an issue on the GitHub repository or reach out to
-us directly at support@jina.ai. ## Contribute ð¤ We welcome all
-contributions! If you're interested in contributing, please refer to our
-[Contribution Guide](CONTRIBUTING.md) for details. ## Our Cloud Platform ð
+scalable and robust cloud platform. ð©ï¸ ## ð Features - ð **HTTPS**:
+Auto-provisioned DNS and TLS certificates for your app. - ð **Protocols**:
+Full compatibility with HTTP, WebSocket, and GraphQL. - âï¸ **Scaling**:
+Scale your app manuallly or let it auto-scale based on RPS, CPU, and Memory. -
+ðï¸ **Secrets**: Secure handling of secrets and environment variables. -
+ðï¸ **Hardware**: Tailor your deployment to suit specific needs. - ð
+**Authorization**: Built-in OAuth2.0 token-based security to secure your
+endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
+your app data. - ð **Blob Storage**: Built-in support for seamless user file
+uploads and downloads. - ð **Observability**: Integrated access to logs,
+metrics, and traces. - ð¦ **Containerization**: Effortless containerization
+of your Python codebase with our integrated registry. ## ð¡ Getting Started
+First, install the `fastapi-serve` package using pip: ```bash pip install
+fastapi-serve ``` Then, simply use the `fastapi-serve` command to deploy your
+FastAPI application: ```bash fastapi-serve deploy jcloud app:app ``` You'll get
+a URL to access your newly deployed application along with the Swagger UI. ##
+ð Examples We have a few examples to help you get acquainted with `fastapi-
+serve`: - ð [Deploy a Simple FastAPI Application](examples/simple/) -
+ðï¸ [Use Secrets for Redis-Powered Rate Limiting](examples/rate_limit/) -
+ð [Secure Your Endpoints with built-in OAuth2.0 Authorization](examples/
+authorization/) - ð [Handle File Uploads and Downloads with built-in Blob
+Storage](examples/file_handling/) ## ð¥ï¸ `fastapi-serve` CLI `fastapi-
+serve` comes with a simple CLI that allows you to deploy your FastAPI
+applications to the cloud with ease. | Description | Command | | --- | ---: | |
+Deploy your app locally | `fastapi-serve deploy local app:app` | | Deploy your
+app on JCloud | `fastapi-serve deploy jcloud app:app` | | Update existing app
+on JCloud | `fastapi-serve deploy jcloud app:app --app-id ` | | Get app status
+on JCloud | `fastapi-serve status ` | | List all apps on JCloud | `fastapi-
+serve list` | | Remove app on JCloud | `fastapi-serve remove ` | ## âï¸ð°
+Configuration and Pricing Read our [Configuration & Pricing Guide](examples/
+CONFIG.MD) to learn more about the various configuration options available to
+you and the pricing model for `fastapi-serve`. ## ðª Support If you encounter
+any problems or have questions, feel free to open an issue on the GitHub
+repository. You can also join our [Discord](https://discord.jina.ai/) to get
+help from our community members and the Jina team. ## Our Cloud Platform ð
 `cloud.jina.ai` is our robust and scalable cloud platform designed to run your
 FastAPI applications with minimum hassle and maximum efficiency. With features
 like auto-scaling, integrated observability, and automated containerization, it
 provides a seamless and worry-free deployment experience. --- `fastapi-serve`
 is more than just a deployment tool, it's a bridge that connects your local
 development environment with our powerful cloud infrastructure. Start using
 `fastapi-serve` today, and experience the joy of effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.2.dev9/setup.py` & `fastapi-serve-0.0.3.dev5/setup.py`

 * *Files identical despite different names*

