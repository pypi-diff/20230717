# Comparing `tmp/ebcpy-0.3.2.tar.gz` & `tmp/ebcpy-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebcpy-0.3.2.tar", last modified: Fri Sep  2 06:19:41 2022, max compression
+gzip compressed data, was "ebcpy-0.3.6.tar", last modified: Mon Jul 17 14:05:50 2023, max compression
```

## Comparing `ebcpy-0.3.2.tar` & `ebcpy-0.3.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-09-02 06:19:41.154037 ebcpy-0.3.2/
--rw-rw-rw-   0        0        0     1642 2022-03-29 12:55:29.000000 ebcpy-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     6717 2022-09-02 06:19:41.154037 ebcpy-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5649 2022-08-21 15:28:50.000000 ebcpy-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2022-09-02 06:19:41.123404 ebcpy-0.3.2/ebcpy/
--rw-rw-rw-   0        0        0      324 2022-08-31 15:38:17.000000 ebcpy-0.3.2/ebcpy/__init__.py
--rw-rw-rw-   0        0        0    22251 2022-08-31 15:38:17.000000 ebcpy-0.3.2/ebcpy/data_types.py
-drwxrwxrwx   0        0        0        0 2022-09-02 06:19:41.139409 ebcpy-0.3.2/ebcpy/modelica/
--rw-rw-rw-   0        0        0     5850 2022-03-29 12:55:29.000000 ebcpy-0.3.2/ebcpy/modelica/__init__.py
--rw-rw-rw-   0        0        0     5960 2022-03-29 12:55:29.000000 ebcpy-0.3.2/ebcpy/modelica/manipulate_ds.py
--rw-rw-rw-   0        0        0    13959 2022-03-29 12:55:29.000000 ebcpy-0.3.2/ebcpy/modelica/simres.py
--rw-rw-rw-   0        0        0    19662 2022-08-21 15:28:50.000000 ebcpy-0.3.2/ebcpy/optimization.py
--rw-rw-rw-   0        0        0    24772 2022-03-29 12:55:29.000000 ebcpy-0.3.2/ebcpy/preprocessing.py
-drwxrwxrwx   0        0        0        0 2022-09-02 06:19:41.144402 ebcpy-0.3.2/ebcpy/simulationapi/
--rw-rw-rw-   0        0        0    19578 2022-09-02 06:19:11.000000 ebcpy-0.3.2/ebcpy/simulationapi/__init__.py
--rw-rw-rw-   0        0        0    50277 2022-09-02 06:19:11.000000 ebcpy-0.3.2/ebcpy/simulationapi/dymola_api.py
--rw-rw-rw-   0        0        0    15337 2022-09-02 06:19:11.000000 ebcpy-0.3.2/ebcpy/simulationapi/fmu.py
-drwxrwxrwx   0        0        0        0 2022-09-02 06:19:41.152404 ebcpy-0.3.2/ebcpy/utils/
--rw-rw-rw-   0        0        0     1427 2022-03-29 12:55:29.000000 ebcpy-0.3.2/ebcpy/utils/__init__.py
--rw-rw-rw-   0        0        0     8721 2022-03-29 12:55:29.000000 ebcpy-0.3.2/ebcpy/utils/conversion.py
--rw-rw-rw-   0        0        0    12237 2022-09-02 06:19:11.000000 ebcpy-0.3.2/ebcpy/utils/reproduction.py
--rw-rw-rw-   0        0        0     6921 2022-03-29 12:55:29.000000 ebcpy-0.3.2/ebcpy/utils/statistics_analyzer.py
-drwxrwxrwx   0        0        0        0 2022-09-02 06:19:41.134402 ebcpy-0.3.2/ebcpy.egg-info/
--rw-rw-rw-   0        0        0     6717 2022-09-02 06:19:40.000000 ebcpy-0.3.2/ebcpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2022-09-02 06:19:40.000000 ebcpy-0.3.2/ebcpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-02 06:19:40.000000 ebcpy-0.3.2/ebcpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2022-09-02 06:19:40.000000 ebcpy-0.3.2/ebcpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-02 06:19:40.000000 ebcpy-0.3.2/ebcpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-09-02 06:19:41.156057 ebcpy-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2457 2022-09-02 06:19:11.000000 ebcpy-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-17 06:41:21.000000 ebcpy-0.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-07-17 14:05:50.615875 ebcpy-0.3.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5514 2023-07-17 06:41:21.000000 ebcpy-0.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.611875 ebcpy-0.3.6/ebcpy/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22850 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/data_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy/modelica/
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/modelica/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5817 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/modelica/manipulate_ds.py
+-rw-rw-rw-   0 root         (0) root         (0)    13625 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/modelica/simres.py
+-rw-rw-rw-   0 root         (0) root         (0)    19180 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)    24847 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy/simulationapi/
+-rw-rw-rw-   0 root         (0) root         (0)    22023 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/simulationapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49673 2023-07-17 08:02:29.000000 ebcpy-0.3.6/ebcpy/simulationapi/dymola_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15299 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/simulationapi/fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8478 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    13536 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/reproduction.py
+-rw-rw-rw-   0 root         (0) root         (0)     6736 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/statistics_analyzer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-17 14:05:50.615875 ebcpy-0.3.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2023-07-17 13:55:15.000000 ebcpy-0.3.6/setup.py
```

### Comparing `ebcpy-0.3.2/LICENSE` & `ebcpy-0.3.6/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2021 RWTH Aachen University - E.ON Energy Research Center - Institute for Energy Efficient Buildings and Indoor Climate
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2021 RWTH Aachen University - E.ON Energy Research Center - Institute for Energy Efficient Buildings and Indoor Climate
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `ebcpy-0.3.2/PKG-INFO` & `ebcpy-0.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-Metadata-Version: 2.1
-Name: ebcpy
-Version: 0.3.2
-Summary: Python Library used for different python modules for the analysis and optimization of energy systems, buildings and indoor climate 
-Home-page: https://github.com/RWTH-EBC/ebcpy
-Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
-Author-email: fabian.wuellhorst@eonerc.rwth-aachen.de
-License: BSD 3-Clause
-Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.2.tar.gz
-Keywords: simulation,building,energy,time-series-data,comfort,black-box optimization
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE
-
-![E.ON EBC RWTH Aachen University](./docs/EBC_Logo.png)
-
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.03861/status.svg)](https://doi.org/10.21105/joss.03861)
-[![pylint](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.svg )](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.html)
-[![documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/doc.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html)
-[![coverage](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage/badge.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage)
-[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![build](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)
-
-
-# ebcpy
-
-This **PY**thon package provides generic functions and classes commonly
-used for the analysis and optimization of **e**nergy systems, **b**uildings and indoor **c**limate (**EBC**).
-
-Key features are:
-
-* `TimeSeriesData`
-* `SimulationAPI`'s
-* Optimization wrapper
-* Pre-/Postprocessing
-* Modelica utilities
-
-It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further reserach. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
-
-# Installation
-
-To install, simply run
-```
-pip install ebcpy
-```
-
-In order to use all optional dependencies (e.g. `pymoo` optimization), install via:
-
-```
-pip install ebcpy[full]
-```
-
-If you encounter an error with the installation of `scikit-learn`, first install `scikit-learn` separatly and then install `ebcpy`:
-
-```
-pip install scikit-learn
-pip install ebcpy
-```
-
-If this still does not work, we refer to the troubleshooting section of `scikit-learn`: https://scikit-learn.org/stable/install.html#troubleshooting. Also check [issue 23](https://github.com/RWTH-EBC/ebcpy/issues/23) for updates.
-
-In order to help development, install it as an egg:
-
-```
-git clone https://github.com/RWTH-EBC/ebcpy
-pip install -e ebcpy
-```
-
-# How to get started?
-
-We recommend running our jupyter-notebook to be guided through a **helpful tutorial**.  
-For this, run the following code:
-```
-# If jupyter is not already installed:
-pip install jupyter
-# Go into your ebcpy-folder (cd \path_to_\ebcpy) or change the path to tutorial.ipynb and run:
-jupyter notebook tutorial\tutorial.ipynb
-```
-
-Or, clone this repo and look at the examples\README.md file.
-Here you will find several examples to execute.
-
-# How to cite ebcpy
-
-Please use the following metadata to cite `ebcpy` in your research:
-
-```
-@article{WÃ¼llhorst2022,
-  doi = {10.21105/joss.03861},
-  url = {https://doi.org/10.21105/joss.03861},
-  year = {2022},
-  publisher = {The Open Journal},
-  volume = {7},
-  number = {72},
-  pages = {3861},
-  author = {Fabian WÃ¼llhorst and Thomas Storek and Philipp Mehrfeld and Dirk MÃ¼ller},
-  title = {AixCaliBuHA: Automated calibration of building and HVAC systems},
-  journal = {Journal of Open Source Software}
-}
-```
-
-# TimeSeriesData
-Note that we use our own `TimeSeriesData` object which inherits from `pd.DataFrame`. The aim is to make tasks like loading different filetypes or applying multiple tags to one variable more convenient, while conserving the powerful tools of the DataFrame.
-Just a quick intro here:
-
-## Variables and tags
-```
->>> from ebcpy.data_types import TimeSeriesData
->>> tsd = TimeSeriesData(r"path_to_a_supported_file")
->>> print(tsd)
-Variables    T_heater              T_heater_1            
-Tags             meas         sim        meas         sim
-Time                                                     
-0.0        313.165863  313.165863  293.173126  293.173126
-1.0        312.090271  310.787750  293.233002  293.352448
-2.0        312.090027  310.796753  293.385925  293.719055
-3.0        312.109436  310.870331  293.589233  294.141754
-```
-
-As you can see, our first column level is always a variable, and the second one a tag.
-This is especially handy when dealing with calibration or processing tasks, where you will have multiple
-versions (tags) for one variable. The default tag is `raw` to indicate the unmodified data.
-To access a variable, you have to call `.loc`. To access multiple variables that all hold one tag use `xs`:
-```python
-# All tags:
-tsd.loc[:, "variable_name"]
-# One specific tag:
-tsd.loc[:, ("variable_name", "tag_name")]
-# One tag, all variables:
-tsd.xs("tag_name", axis=1, level=1)
-```
-## FloatIndex and DateTimeIndex
-Measured data typically holds a datetime stamps (`DateTimeIndex`) while simulation result files hold absolute seconds (`FloatIndex`). 
-You can easily convert back and forth using:
-```python
-# From Datetime to float
-tsd.to_float_index()
-# From float to datetime
-tsd.to_datetime_index()
-# To clean your data and create a common frequency:
-tsd.clean_and_space_equally(desired_freq="1s")
-```
-
-# Documentation
-Visit hour official [Documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html).
-
-# Problems?
-Please [raise an issue here](https://github.com/RWTH-EBC/ebcpy/issues/new).
-
-
+Metadata-Version: 2.1
+Name: ebcpy
+Version: 0.3.6
+Summary: Python Library used for different python modules for the analysis and optimization of energy systems, buildings and indoor climate 
+Home-page: https://github.com/RWTH-EBC/ebcpy
+Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
+Author-email: fabian.wuellhorst@eonerc.rwth-aachen.de
+License: BSD 3-Clause
+Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.6.tar.gz
+Keywords: simulation,building,energy,time-series-data,comfort,black-box optimization
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: full
+License-File: LICENSE
+
+![E.ON EBC RWTH Aachen University](./docs/EBC_Logo.png)
+
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.03861/status.svg)](https://doi.org/10.21105/joss.03861)
+[![pylint](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.svg )](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.html)
+[![documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/doc.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html)
+[![coverage](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage/badge.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![build](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)
+
+
+# ebcpy
+
+This **PY**thon package provides generic functions and classes commonly
+used for the analysis and optimization of **e**nergy systems, **b**uildings and indoor **c**limate (**EBC**).
+
+Key features are:
+
+* `TimeSeriesData`
+* `SimulationAPI`'s
+* Optimization wrapper
+* Pre-/Postprocessing
+* Modelica utilities
+
+It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further reserach. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
+
+# Installation
+
+To install, simply run
+```
+pip install ebcpy
+```
+
+In order to use all optional dependencies (e.g. `pymoo` optimization), install via:
+
+```
+pip install ebcpy[full]
+```
+
+If you encounter an error with the installation of `scikit-learn`, first install `scikit-learn` separatly and then install `ebcpy`:
+
+```
+pip install scikit-learn
+pip install ebcpy
+```
+
+If this still does not work, we refer to the troubleshooting section of `scikit-learn`: https://scikit-learn.org/stable/install.html#troubleshooting. Also check [issue 23](https://github.com/RWTH-EBC/ebcpy/issues/23) for updates.
+
+In order to help development, install it as an egg:
+
+```
+git clone https://github.com/RWTH-EBC/ebcpy
+pip install -e ebcpy
+```
+
+# How to get started?
+
+We recommend running our jupyter-notebook to be guided through a **helpful tutorial**.  
+For this, run the following code:
+```
+# If jupyter is not already installed:
+pip install jupyter
+# Go into your ebcpy-folder (cd \path_to_\ebcpy) or change the path to tutorial.ipynb and run:
+jupyter notebook tutorial\tutorial.ipynb
+```
+
+Or, clone this repo and look at the examples\README.md file.
+Here you will find several examples to execute.
+
+# How to cite ebcpy
+
+Please use the following metadata to cite `ebcpy` in your research:
+
+```
+@article{Wuellhorst2022,
+  doi = {10.21105/joss.03861},
+  url = {https://doi.org/10.21105/joss.03861},
+  year = {2022},
+  publisher = {The Open Journal},
+  volume = {7},
+  number = {72},
+  pages = {3861},
+  author = {Fabian Wüllhorst and Thomas Storek and Philipp Mehrfeld and Dirk Müller},
+  title = {AixCaliBuHA: Automated calibration of building and HVAC systems},
+  journal = {Journal of Open Source Software}
+}
+```
+
+# TimeSeriesData
+Note that we use our own `TimeSeriesData` object which inherits from `pd.DataFrame`. The aim is to make tasks like loading different filetypes or applying multiple tags to one variable more convenient, while conserving the powerful tools of the DataFrame.
+Just a quick intro here:
+
+## Variables and tags
+```
+>>> from ebcpy.data_types import TimeSeriesData
+>>> tsd = TimeSeriesData(r"path_to_a_supported_file")
+>>> print(tsd)
+Variables    T_heater              T_heater_1            
+Tags             meas         sim        meas         sim
+Time                                                     
+0.0        313.165863  313.165863  293.173126  293.173126
+1.0        312.090271  310.787750  293.233002  293.352448
+2.0        312.090027  310.796753  293.385925  293.719055
+3.0        312.109436  310.870331  293.589233  294.141754
+```
+
+As you can see, our first column level is always a variable, and the second one a tag.
+This is especially handy when dealing with calibration or processing tasks, where you will have multiple
+versions (tags) for one variable. The default tag is `raw` to indicate the unmodified data.
+To access a variable, you have to call `.loc`. To access multiple variables that all hold one tag use `xs`:
+```python
+# All tags:
+tsd.loc[:, "variable_name"]
+# One specific tag:
+tsd.loc[:, ("variable_name", "tag_name")]
+# One tag, all variables:
+tsd.xs("tag_name", axis=1, level=1)
+```
+## FloatIndex and DateTimeIndex
+Measured data typically holds a datetime stamps (`DateTimeIndex`) while simulation result files hold absolute seconds (`FloatIndex`). 
+You can easily convert back and forth using:
+```python
+# From Datetime to float
+tsd.to_float_index()
+# From float to datetime
+tsd.to_datetime_index()
+# To clean your data and create a common frequency:
+tsd.clean_and_space_equally(desired_freq="1s")
+```
+
+# Documentation
+Visit our official [Documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html).
+
+# Problems?
+Please [raise an issue here](https://github.com/RWTH-EBC/ebcpy/issues/new).
+
+
```

### Comparing `ebcpy-0.3.2/README.md` & `ebcpy-0.3.6/ebcpy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,158 @@
-![E.ON EBC RWTH Aachen University](./docs/EBC_Logo.png)
-
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.03861/status.svg)](https://doi.org/10.21105/joss.03861)
-[![pylint](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.svg )](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.html)
-[![documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/doc.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html)
-[![coverage](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage/badge.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage)
-[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![build](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)
-
-
-# ebcpy
-
-This **PY**thon package provides generic functions and classes commonly
-used for the analysis and optimization of **e**nergy systems, **b**uildings and indoor **c**limate (**EBC**).
-
-Key features are:
-
-* `TimeSeriesData`
-* `SimulationAPI`'s
-* Optimization wrapper
-* Pre-/Postprocessing
-* Modelica utilities
-
-It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further reserach. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
-
-# Installation
-
-To install, simply run
-```
-pip install ebcpy
-```
-
-In order to use all optional dependencies (e.g. `pymoo` optimization), install via:
-
-```
-pip install ebcpy[full]
-```
-
-If you encounter an error with the installation of `scikit-learn`, first install `scikit-learn` separatly and then install `ebcpy`:
-
-```
-pip install scikit-learn
-pip install ebcpy
-```
-
-If this still does not work, we refer to the troubleshooting section of `scikit-learn`: https://scikit-learn.org/stable/install.html#troubleshooting. Also check [issue 23](https://github.com/RWTH-EBC/ebcpy/issues/23) for updates.
-
-In order to help development, install it as an egg:
-
-```
-git clone https://github.com/RWTH-EBC/ebcpy
-pip install -e ebcpy
-```
-
-# How to get started?
-
-We recommend running our jupyter-notebook to be guided through a **helpful tutorial**.  
-For this, run the following code:
-```
-# If jupyter is not already installed:
-pip install jupyter
-# Go into your ebcpy-folder (cd \path_to_\ebcpy) or change the path to tutorial.ipynb and run:
-jupyter notebook tutorial\tutorial.ipynb
-```
-
-Or, clone this repo and look at the examples\README.md file.
-Here you will find several examples to execute.
-
-# How to cite ebcpy
-
-Please use the following metadata to cite `ebcpy` in your research:
-
-```
-@article{Wüllhorst2022,
-  doi = {10.21105/joss.03861},
-  url = {https://doi.org/10.21105/joss.03861},
-  year = {2022},
-  publisher = {The Open Journal},
-  volume = {7},
-  number = {72},
-  pages = {3861},
-  author = {Fabian Wüllhorst and Thomas Storek and Philipp Mehrfeld and Dirk Müller},
-  title = {AixCaliBuHA: Automated calibration of building and HVAC systems},
-  journal = {Journal of Open Source Software}
-}
-```
-
-# TimeSeriesData
-Note that we use our own `TimeSeriesData` object which inherits from `pd.DataFrame`. The aim is to make tasks like loading different filetypes or applying multiple tags to one variable more convenient, while conserving the powerful tools of the DataFrame.
-Just a quick intro here:
-
-## Variables and tags
-```
->>> from ebcpy.data_types import TimeSeriesData
->>> tsd = TimeSeriesData(r"path_to_a_supported_file")
->>> print(tsd)
-Variables    T_heater              T_heater_1            
-Tags             meas         sim        meas         sim
-Time                                                     
-0.0        313.165863  313.165863  293.173126  293.173126
-1.0        312.090271  310.787750  293.233002  293.352448
-2.0        312.090027  310.796753  293.385925  293.719055
-3.0        312.109436  310.870331  293.589233  294.141754
-```
-
-As you can see, our first column level is always a variable, and the second one a tag.
-This is especially handy when dealing with calibration or processing tasks, where you will have multiple
-versions (tags) for one variable. The default tag is `raw` to indicate the unmodified data.
-To access a variable, you have to call `.loc`. To access multiple variables that all hold one tag use `xs`:
-```python
-# All tags:
-tsd.loc[:, "variable_name"]
-# One specific tag:
-tsd.loc[:, ("variable_name", "tag_name")]
-# One tag, all variables:
-tsd.xs("tag_name", axis=1, level=1)
-```
-## FloatIndex and DateTimeIndex
-Measured data typically holds a datetime stamps (`DateTimeIndex`) while simulation result files hold absolute seconds (`FloatIndex`). 
-You can easily convert back and forth using:
-```python
-# From Datetime to float
-tsd.to_float_index()
-# From float to datetime
-tsd.to_datetime_index()
-# To clean your data and create a common frequency:
-tsd.clean_and_space_equally(desired_freq="1s")
-```
-
-# Documentation
-Visit hour official [Documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html).
-
-# Problems?
-Please [raise an issue here](https://github.com/RWTH-EBC/ebcpy/issues/new).
+Metadata-Version: 2.1
+Name: ebcpy
+Version: 0.3.6
+Summary: Python Library used for different python modules for the analysis and optimization of energy systems, buildings and indoor climate 
+Home-page: https://github.com/RWTH-EBC/ebcpy
+Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
+Author-email: fabian.wuellhorst@eonerc.rwth-aachen.de
+License: BSD 3-Clause
+Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.6.tar.gz
+Keywords: simulation,building,energy,time-series-data,comfort,black-box optimization
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: full
+License-File: LICENSE
+
+![E.ON EBC RWTH Aachen University](./docs/EBC_Logo.png)
+
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.03861/status.svg)](https://doi.org/10.21105/joss.03861)
+[![pylint](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.svg )](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.html)
+[![documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/doc.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html)
+[![coverage](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage/badge.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![build](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)
+
+
+# ebcpy
+
+This **PY**thon package provides generic functions and classes commonly
+used for the analysis and optimization of **e**nergy systems, **b**uildings and indoor **c**limate (**EBC**).
+
+Key features are:
+
+* `TimeSeriesData`
+* `SimulationAPI`'s
+* Optimization wrapper
+* Pre-/Postprocessing
+* Modelica utilities
+
+It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further reserach. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
+
+# Installation
+
+To install, simply run
+```
+pip install ebcpy
+```
+
+In order to use all optional dependencies (e.g. `pymoo` optimization), install via:
+
+```
+pip install ebcpy[full]
+```
+
+If you encounter an error with the installation of `scikit-learn`, first install `scikit-learn` separatly and then install `ebcpy`:
+
+```
+pip install scikit-learn
+pip install ebcpy
+```
+
+If this still does not work, we refer to the troubleshooting section of `scikit-learn`: https://scikit-learn.org/stable/install.html#troubleshooting. Also check [issue 23](https://github.com/RWTH-EBC/ebcpy/issues/23) for updates.
+
+In order to help development, install it as an egg:
+
+```
+git clone https://github.com/RWTH-EBC/ebcpy
+pip install -e ebcpy
+```
+
+# How to get started?
+
+We recommend running our jupyter-notebook to be guided through a **helpful tutorial**.  
+For this, run the following code:
+```
+# If jupyter is not already installed:
+pip install jupyter
+# Go into your ebcpy-folder (cd \path_to_\ebcpy) or change the path to tutorial.ipynb and run:
+jupyter notebook tutorial\tutorial.ipynb
+```
+
+Or, clone this repo and look at the examples\README.md file.
+Here you will find several examples to execute.
+
+# How to cite ebcpy
+
+Please use the following metadata to cite `ebcpy` in your research:
+
+```
+@article{Wuellhorst2022,
+  doi = {10.21105/joss.03861},
+  url = {https://doi.org/10.21105/joss.03861},
+  year = {2022},
+  publisher = {The Open Journal},
+  volume = {7},
+  number = {72},
+  pages = {3861},
+  author = {Fabian Wüllhorst and Thomas Storek and Philipp Mehrfeld and Dirk Müller},
+  title = {AixCaliBuHA: Automated calibration of building and HVAC systems},
+  journal = {Journal of Open Source Software}
+}
+```
+
+# TimeSeriesData
+Note that we use our own `TimeSeriesData` object which inherits from `pd.DataFrame`. The aim is to make tasks like loading different filetypes or applying multiple tags to one variable more convenient, while conserving the powerful tools of the DataFrame.
+Just a quick intro here:
+
+## Variables and tags
+```
+>>> from ebcpy.data_types import TimeSeriesData
+>>> tsd = TimeSeriesData(r"path_to_a_supported_file")
+>>> print(tsd)
+Variables    T_heater              T_heater_1            
+Tags             meas         sim        meas         sim
+Time                                                     
+0.0        313.165863  313.165863  293.173126  293.173126
+1.0        312.090271  310.787750  293.233002  293.352448
+2.0        312.090027  310.796753  293.385925  293.719055
+3.0        312.109436  310.870331  293.589233  294.141754
+```
+
+As you can see, our first column level is always a variable, and the second one a tag.
+This is especially handy when dealing with calibration or processing tasks, where you will have multiple
+versions (tags) for one variable. The default tag is `raw` to indicate the unmodified data.
+To access a variable, you have to call `.loc`. To access multiple variables that all hold one tag use `xs`:
+```python
+# All tags:
+tsd.loc[:, "variable_name"]
+# One specific tag:
+tsd.loc[:, ("variable_name", "tag_name")]
+# One tag, all variables:
+tsd.xs("tag_name", axis=1, level=1)
+```
+## FloatIndex and DateTimeIndex
+Measured data typically holds a datetime stamps (`DateTimeIndex`) while simulation result files hold absolute seconds (`FloatIndex`). 
+You can easily convert back and forth using:
+```python
+# From Datetime to float
+tsd.to_float_index()
+# From float to datetime
+tsd.to_datetime_index()
+# To clean your data and create a common frequency:
+tsd.clean_and_space_equally(desired_freq="1s")
+```
+
+# Documentation
+Visit our official [Documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html).
+
+# Problems?
+Please [raise an issue here](https://github.com/RWTH-EBC/ebcpy/issues/new).
+
+
```

### Comparing `ebcpy-0.3.2/ebcpy/modelica/__init__.py` & `ebcpy-0.3.6/ebcpy/modelica/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-"""
-This package aims to help manipulate simulation files (dsfinal.txt or dsin.txt)
-or to load simulation result files (.mat) efficiently into a pandas.DataFrame
-"""
-import re
-from typing import Union, List
-
-
-def get_expressions(filepath_model: str,
-                    get_protected: bool = False,
-                    modelica_type: Union[str, List] = "parameters",
-                    excludes: List = None):
-    """
-    This function extracts specific expressions out of modelica models.
-
-    :param str,os.path.normpath filepath_model:
-        Full path of modelica model on the given os
-        e.g. path_model = "C://MyLibrary//TestModel.mo"
-    :param str,list modelica_type:
-        Type you want to have matched. "parameters" and "variables"
-        have a special regex pattern.
-        For other models, you can parse a string like:
-        "replaceable package Medium" and it will yield all
-        afflicted lines. You can also give a list of strings if
-        multiple strings are relevant to you.
-        Special cases:
-        parameters:
-        - include: ["parameter"]
-        - excludes: ["final", "in", "of", "replaceable"]
-        variables: Note: The case for already imported SIUnits is not considered here.
-        - include: ["Modelica.SIunits", "Real", "Boolean", "Integer"]
-        - excludes: ["parameter", "import", "constant"]
-    :param list excludes:
-        List of strings to exclude from expression. Default is None.
-    :param Boolean get_protected:
-        Whether to extract protected parameters or not. Default is false
-
-    :return: list matches
-        List with all lines matching the given expression.
-    """
-    if excludes is None:
-        excludes = []
-    if modelica_type == "parameters":
-        _includes = ["parameter"]
-        _excludes = ["final", "in", "of", "replaceable"] + excludes
-    elif modelica_type == "variables":
-        _includes = ["Modelica.SIunits", "Real", "Boolean", "Integer"]
-        _excludes = ["parameter", "import", "constant"] + excludes
-    else:
-        _includes = [modelica_type]
-        _excludes = excludes
-    if _excludes:
-        _exclude_str = r"(?<!" + r"\s)(?<!".join(_excludes) + r"\s)"
-    else:  # Case if list is empty
-        _exclude_str = ""
-    _pattern = r'((?:\s.+)?{}({})(.|\n)*?;)'.format(_exclude_str,
-                                                    "|".join(_includes))
-
-    # Open the file
-    with open(filepath_model, "r") as file:
-        file.seek(0)
-        script = file.read()
-
-    # Find desired expression in modelica script
-    expr = re.findall(_pattern, script, re.MULTILINE)
-
-    expr_filtered = [" ".join(expr_unfiltered[0].split()) for expr_unfiltered in expr]
-
-    if not get_protected:
-        return expr_filtered
-
-    # Get position of expressions
-    pos_expr = []
-    for match in re.finditer(_pattern, script, re.MULTILINE):
-        pos_expr.append(match.span()[0])
-
-    # Check if parameter are protected
-    expr_unprotected = []
-    expr_protected = []
-
-    # Get position of "protected"-expression
-    protected = re.search(r'protected', script)
-
-    if protected:
-        pos_protected = protected.span()[0]
-        for i, temp_expr in enumerate(expr):
-            # If expressions is before 'proteceted' --> refer to expr_unprotected
-            if pos_expr[i] < pos_protected:
-                expr_unprotected.append(temp_expr)
-            # If expressions is after 'proteceted' --> refer to expr_protected
-            else:
-                expr_protected.append(temp_expr)
-    else:
-        expr_unprotected = expr
-
-    return expr_unprotected, expr_protected
-
-
-def get_names_and_values_of_lines(lines: List[str]) -> dict:
-    """
-    All unnecessary code is deleted (annotations, doc).
-    Only the name of the variable and the value is extracted.
-
-    :param List[str] lines:
-        List of strings with lines from a modelica file.
-
-    :return:
-        dict: Containing the names as key and values as value.
-
-    Example:
-
-    >>> lines = ['parameter Boolean my_boolean=true "Some description"',
-    >>>          'parameter Real my_real=12.0 "Some description" annotation("Some annotation")']
-    >>> output = get_names_and_values_of_lines(lines=lines)
-    >>> print(output)
-    {'my_boolean': True, 'my_real': 12.0}
-    """
-    res = {}
-    for line in lines:
-        line = line.replace(";", "")
-
-        # Check if line is a commented line and if so, skip the line:
-        if line.startswith("//"):
-            continue
-
-        # Remove part behind possible annotation:
-        loc = line.find("annotation")
-        if loc >= 0:
-            line = line[:loc]
-        # Remove possible brackets, like "param(min=0, start=5)
-        line = re.sub(r'[\(\[].*?[\)\]]', '', line)
-        # And now any quotes / doc / strings
-        line = re.sub(r'".*"', '', line)
-        # If a value is present (e.g. for parameters, one = sign is still present (always)
-        if line.find("=") >= 0:
-            name_str, val_str = line.split("=")
-            name_str = name_str.strip()
-            name = name_str.split(" ")[-1].replace(" ", "")
-            val_str_stripped = val_str.replace(" ", "")
-            if val_str_stripped in ["true", "false"]:
-                value = val_str_stripped == "true"
-            else:
-                try:
-                    value = float(val_str_stripped)
-                except ValueError:
-                    # Neither float, integer nor boolean, hence None
-                    value = None
-        # else no value is stored in the line
-        else:
-            line = line.strip()
-            name = line.split(" ")[-1].replace(" ", "")
-            value = None
-        res.update({name: value})
-
-    return res
+"""
+This package aims to help manipulate simulation files (dsfinal.txt or dsin.txt)
+or to load simulation result files (.mat) efficiently into a pandas.DataFrame
+"""
+import re
+from typing import Union, List
+
+
+def get_expressions(filepath_model: str,
+                    get_protected: bool = False,
+                    modelica_type: Union[str, List] = "parameters",
+                    excludes: List = None):
+    """
+    This function extracts specific expressions out of modelica models.
+
+    :param str,os.path.normpath filepath_model:
+        Full path of modelica model on the given os
+        e.g. path_model = "C://MyLibrary//TestModel.mo"
+    :param str,list modelica_type:
+        Type you want to have matched. "parameters" and "variables"
+        have a special regex pattern.
+        For other models, you can parse a string like:
+        "replaceable package Medium" and it will yield all
+        afflicted lines. You can also give a list of strings if
+        multiple strings are relevant to you.
+        Special cases:
+        parameters:
+        - include: ["parameter"]
+        - excludes: ["final", "in", "of", "replaceable"]
+        variables: Note: The case for already imported SIUnits is not considered here.
+        - include: ["Modelica.SIunits", "Real", "Boolean", "Integer"]
+        - excludes: ["parameter", "import", "constant"]
+    :param list excludes:
+        List of strings to exclude from expression. Default is None.
+    :param Boolean get_protected:
+        Whether to extract protected parameters or not. Default is false
+
+    :return: list matches
+        List with all lines matching the given expression.
+    """
+    if excludes is None:
+        excludes = []
+    if modelica_type == "parameters":
+        _includes = ["parameter"]
+        _excludes = ["final", "in", "of", "replaceable"] + excludes
+    elif modelica_type == "variables":
+        _includes = ["Modelica.SIunits", "Real", "Boolean", "Integer"]
+        _excludes = ["parameter", "import", "constant"] + excludes
+    else:
+        _includes = [modelica_type]
+        _excludes = excludes
+    if _excludes:
+        _exclude_str = r"(?<!" + r"\s)(?<!".join(_excludes) + r"\s)"
+    else:  # Case if list is empty
+        _exclude_str = ""
+    _pattern = r'((?:\s.+)?{}({})(.|\n)*?;)'.format(_exclude_str,
+                                                    "|".join(_includes))
+
+    # Open the file
+    with open(filepath_model, "r") as file:
+        file.seek(0)
+        script = file.read()
+
+    # Find desired expression in modelica script
+    expr = re.findall(_pattern, script, re.MULTILINE)
+
+    expr_filtered = [" ".join(expr_unfiltered[0].split()) for expr_unfiltered in expr]
+
+    if not get_protected:
+        return expr_filtered
+
+    # Get position of expressions
+    pos_expr = []
+    for match in re.finditer(_pattern, script, re.MULTILINE):
+        pos_expr.append(match.span()[0])
+
+    # Check if parameter are protected
+    expr_unprotected = []
+    expr_protected = []
+
+    # Get position of "protected"-expression
+    protected = re.search(r'protected', script)
+
+    if protected:
+        pos_protected = protected.span()[0]
+        for i, temp_expr in enumerate(expr):
+            # If expressions is before 'proteceted' --> refer to expr_unprotected
+            if pos_expr[i] < pos_protected:
+                expr_unprotected.append(temp_expr)
+            # If expressions is after 'proteceted' --> refer to expr_protected
+            else:
+                expr_protected.append(temp_expr)
+    else:
+        expr_unprotected = expr
+
+    return expr_unprotected, expr_protected
+
+
+def get_names_and_values_of_lines(lines: List[str]) -> dict:
+    """
+    All unnecessary code is deleted (annotations, doc).
+    Only the name of the variable and the value is extracted.
+
+    :param List[str] lines:
+        List of strings with lines from a modelica file.
+
+    :return:
+        dict: Containing the names as key and values as value.
+
+    Example:
+
+    >>> lines = ['parameter Boolean my_boolean=true "Some description"',
+    >>>          'parameter Real my_real=12.0 "Some description" annotation("Some annotation")']
+    >>> output = get_names_and_values_of_lines(lines=lines)
+    >>> print(output)
+    {'my_boolean': True, 'my_real': 12.0}
+    """
+    res = {}
+    for line in lines:
+        line = line.replace(";", "")
+
+        # Check if line is a commented line and if so, skip the line:
+        if line.startswith("//"):
+            continue
+
+        # Remove part behind possible annotation:
+        loc = line.find("annotation")
+        if loc >= 0:
+            line = line[:loc]
+        # Remove possible brackets, like "param(min=0, start=5)
+        line = re.sub(r'[\(\[].*?[\)\]]', '', line)
+        # And now any quotes / doc / strings
+        line = re.sub(r'".*"', '', line)
+        # If a value is present (e.g. for parameters, one = sign is still present (always)
+        if line.find("=") >= 0:
+            name_str, val_str = line.split("=")
+            name_str = name_str.strip()
+            name = name_str.split(" ")[-1].replace(" ", "")
+            val_str_stripped = val_str.replace(" ", "")
+            if val_str_stripped in ["true", "false"]:
+                value = val_str_stripped == "true"
+            else:
+                try:
+                    value = float(val_str_stripped)
+                except ValueError:
+                    # Neither float, integer nor boolean, hence None
+                    value = None
+        # else no value is stored in the line
+        else:
+            line = line.strip()
+            name = line.split(" ")[-1].replace(" ", "")
+            value = None
+        res.update({name: value})
+
+    return res
```

### Comparing `ebcpy-0.3.2/ebcpy/modelica/manipulate_ds.py` & `ebcpy-0.3.6/ebcpy/modelica/manipulate_ds.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-"""Functions to manipulate (or extract information of) the
-dsfinal.txt and dsin.txt files created by Modelica."""
-
-from io import StringIO
-import pandas as pd
-
-
-def convert_ds_file_to_dataframe(filename):
-    """
-    Function to convert a given dsfinal or dsfin file to a DataFrame.
-    The index is the name of the variable. Further,
-    the following columns are used analog to the dsfinal:
-    column 1: Type of initial value:
-    = -2: special case: for continuing simulation (column 2 = value)
-    = -1: fixed value (column 2 = fixed value)
-    =  0: free value, i.e., no restriction (column 2 = initial value)
-    >  0: desired value (column 1 = weight for optimization,
-    column 2 = desired value)
-    use weight=1, since automatic scaling usually
-    leads to equally weighted terms
-    column 2: fixed, free or desired value according to column 1.
-    column 3: Minimum value (ignored, if Minimum >= Maximum).
-    column 4: Maximum value (ignored, if Minimum >= Maximum).
-    Minimum and maximum restrict the search range in initial
-    value calculation. They might also be used for scaling.
-    column 5: Category of variable:
-    = 1: parameter.
-    = 2: state.
-    = 3: state derivative.
-    = 4: output.
-    = 5: input.
-    = 6: auxiliary variable.
-    column 6: Data type of variable and flags according to dsBaseType
-
-    :param str,os.path.normpath filename:
-        Filepath to the dsfinal or dsinto be loaded.
-    :return: pd.DataFrame
-        Converted DataFrame
-    """
-    # Define relevant parameters
-    number_line_initial_name = 104  # Line where the string char initialName(,) is always stored
-
-    # Open file and get relevant content by splitting the lines.
-    with open(filename, "r") as file:
-        content = file.read().split("\n")
-
-    # Gets the X out of 'char initialName(X,Y)'
-    size_initial_names = int(content[number_line_initial_name].split("(")[-1].split(",")[0])
-    # Number of line below line "double initialValue(X,Y)"
-    number_line_initial_value = number_line_initial_name + size_initial_names + 3
-
-    # Check if two or on-line dsfinal / dsin
-    if "#" in content[number_line_initial_value]:
-        step_size = 1
-    else:
-        step_size = 2
-
-    # trim content:
-    ini_val_list = content[number_line_initial_value: (number_line_initial_value +
-                                                       step_size * size_initial_names)]
-    # Alter list to create one-lined list.
-    if step_size == 2:
-        ini_val_list_one_line = []
-        for i in range(0, len(ini_val_list), 2):
-            # Concat two line into one line
-            ini_val_list_one_line.append(ini_val_list[i] + ini_val_list[i + 1])
-    else:
-        ini_val_list_one_line = ini_val_list
-
-    # Convert to DataFrame. Use a csv-method as it is much faster.
-    out = StringIO()
-    # csv_writer = writer(out)
-    out.write("1;2;3;4;5;6;initialName\n")
-    # df = pd.DataFrame({1:[], 2:[], 3:[], 4:[], 5:[], 6:[], "initialName":[]})
-    for line in ini_val_list_one_line:
-        # Get only the string of the initialName
-        ini_name = line.split("#")[-1].replace(" ", "").replace("\n", "")
-        vals = line.split("#")[0].split()
-        vals.append(ini_name)
-        out.write(";".join(vals) + "\n")
-    out.seek(0)
-    df = pd.read_csv(out, header=0, sep=";", dtype=object)
-    df = df.set_index("initialName")
-    return df
-
-
-def eliminate_parameters_from_ds_file(filename, savepath, exclude_paras, del_aux_paras=True):
-    """
-    Create a new dsfinal file out of the given dsfinal.txt
-    All parameters except those listed in exclude_paras
-    will be eliminated from the dsfinal file.
-    Used for continuing of simulation in calibration problems.
-
-    :param str,os.path.normpath filename:
-        Filepath to the dsfinal or dsin file
-    :param str,os.path.normpath savepath:
-        .txt-file for storing output of this function
-    :param list exclude_paras:
-        List of parameters to exclude.
-    :param bool del_aux_paras:
-        Whether to delete auxiliary parameters or not.
-        Default value is True.
-    """
-
-    # Check types
-    if not savepath.endswith(".txt"):
-        raise TypeError('File %s is not of type .txt' % savepath)
-    if not isinstance(exclude_paras, list):
-        raise TypeError(f"Given exclude_paras is of type {type(exclude_paras).__name__} "
-                        f"but should be of type list")
-
-    df = convert_ds_file_to_dataframe(filename)
-
-    # Manipulate DataFrame
-    if del_aux_paras:
-        # Delete all rows with a parameter or an auxiliary value
-        df = df[(df["5"] != "1") & (df["5"] != "6") | [idx in exclude_paras for idx in df.index]]
-    else:
-        df = df[(df["5"] != "1") | [idx in exclude_paras for idx in df.index]]
-
-    # Generate string out of trimmed DataFrame
-    longest_name = len(max(df.index, key=len))
-    char_initial_name = "char initialName(%s,%s)" % (len(df.index), longest_name)
-    char_initial_name += "\n" + "\n".join(df.index)
-    double_initial_value = "double initialValue(%s,6)" % len(df.index)  # Always 6
-    for index, row in df.iterrows():
-        double_initial_value += "\n" + " ".join(row) + " # " + index
-
-    # Create resulting dsFinal string
-    string_new_ds_final = char_initial_name + "\n\n" + double_initial_value
-
-    # Reuses the experiment, tuning parameters etc. settings
-    number_line_initial_name = 104  # Line where the string char initialName(,) is always stored
-    with open(filename, "r") as file:
-        content = file.read().split("\n")
-
-    new_content = "\n".join(content[:number_line_initial_name])
-    new_content += "\n" + string_new_ds_final
-    # Save new content to given savepath
-    with open(savepath, "a+") as file:
-        file.seek(0)
-        file.truncate()  # Delete all content of the given file
-        file.write(new_content)
+"""Functions to manipulate (or extract information of) the
+dsfinal.txt and dsin.txt files created by Modelica."""
+
+from io import StringIO
+import pandas as pd
+
+
+def convert_ds_file_to_dataframe(filename):
+    """
+    Function to convert a given dsfinal or dsfin file to a DataFrame.
+    The index is the name of the variable. Further,
+    the following columns are used analog to the dsfinal:
+    column 1: Type of initial value:
+    = -2: special case: for continuing simulation (column 2 = value)
+    = -1: fixed value (column 2 = fixed value)
+    =  0: free value, i.e., no restriction (column 2 = initial value)
+    >  0: desired value (column 1 = weight for optimization,
+    column 2 = desired value)
+    use weight=1, since automatic scaling usually
+    leads to equally weighted terms
+    column 2: fixed, free or desired value according to column 1.
+    column 3: Minimum value (ignored, if Minimum >= Maximum).
+    column 4: Maximum value (ignored, if Minimum >= Maximum).
+    Minimum and maximum restrict the search range in initial
+    value calculation. They might also be used for scaling.
+    column 5: Category of variable:
+    = 1: parameter.
+    = 2: state.
+    = 3: state derivative.
+    = 4: output.
+    = 5: input.
+    = 6: auxiliary variable.
+    column 6: Data type of variable and flags according to dsBaseType
+
+    :param str,os.path.normpath filename:
+        Filepath to the dsfinal or dsinto be loaded.
+    :return: pd.DataFrame
+        Converted DataFrame
+    """
+    # Define relevant parameters
+    number_line_initial_name = 104  # Line where the string char initialName(,) is always stored
+
+    # Open file and get relevant content by splitting the lines.
+    with open(filename, "r") as file:
+        content = file.read().split("\n")
+
+    # Gets the X out of 'char initialName(X,Y)'
+    size_initial_names = int(content[number_line_initial_name].split("(")[-1].split(",")[0])
+    # Number of line below line "double initialValue(X,Y)"
+    number_line_initial_value = number_line_initial_name + size_initial_names + 3
+
+    # Check if two or on-line dsfinal / dsin
+    if "#" in content[number_line_initial_value]:
+        step_size = 1
+    else:
+        step_size = 2
+
+    # trim content:
+    ini_val_list = content[number_line_initial_value: (number_line_initial_value +
+                                                       step_size * size_initial_names)]
+    # Alter list to create one-lined list.
+    if step_size == 2:
+        ini_val_list_one_line = []
+        for i in range(0, len(ini_val_list), 2):
+            # Concat two line into one line
+            ini_val_list_one_line.append(ini_val_list[i] + ini_val_list[i + 1])
+    else:
+        ini_val_list_one_line = ini_val_list
+
+    # Convert to DataFrame. Use a csv-method as it is much faster.
+    out = StringIO()
+    # csv_writer = writer(out)
+    out.write("1;2;3;4;5;6;initialName\n")
+    # df = pd.DataFrame({1:[], 2:[], 3:[], 4:[], 5:[], 6:[], "initialName":[]})
+    for line in ini_val_list_one_line:
+        # Get only the string of the initialName
+        ini_name = line.split("#")[-1].replace(" ", "").replace("\n", "")
+        vals = line.split("#")[0].split()
+        vals.append(ini_name)
+        out.write(";".join(vals) + "\n")
+    out.seek(0)
+    df = pd.read_csv(out, header=0, sep=";", dtype=object)
+    df = df.set_index("initialName")
+    return df
+
+
+def eliminate_parameters_from_ds_file(filename, savepath, exclude_paras, del_aux_paras=True):
+    """
+    Create a new dsfinal file out of the given dsfinal.txt
+    All parameters except those listed in exclude_paras
+    will be eliminated from the dsfinal file.
+    Used for continuing of simulation in calibration problems.
+
+    :param str,os.path.normpath filename:
+        Filepath to the dsfinal or dsin file
+    :param str,os.path.normpath savepath:
+        .txt-file for storing output of this function
+    :param list exclude_paras:
+        List of parameters to exclude.
+    :param bool del_aux_paras:
+        Whether to delete auxiliary parameters or not.
+        Default value is True.
+    """
+
+    # Check types
+    if not savepath.endswith(".txt"):
+        raise TypeError('File %s is not of type .txt' % savepath)
+    if not isinstance(exclude_paras, list):
+        raise TypeError(f"Given exclude_paras is of type {type(exclude_paras).__name__} "
+                        f"but should be of type list")
+
+    df = convert_ds_file_to_dataframe(filename)
+
+    # Manipulate DataFrame
+    if del_aux_paras:
+        # Delete all rows with a parameter or an auxiliary value
+        df = df[(df["5"] != "1") & (df["5"] != "6") | [idx in exclude_paras for idx in df.index]]
+    else:
+        df = df[(df["5"] != "1") | [idx in exclude_paras for idx in df.index]]
+
+    # Generate string out of trimmed DataFrame
+    longest_name = len(max(df.index, key=len))
+    char_initial_name = "char initialName(%s,%s)" % (len(df.index), longest_name)
+    char_initial_name += "\n" + "\n".join(df.index)
+    double_initial_value = "double initialValue(%s,6)" % len(df.index)  # Always 6
+    for index, row in df.iterrows():
+        double_initial_value += "\n" + " ".join(row) + " # " + index
+
+    # Create resulting dsFinal string
+    string_new_ds_final = char_initial_name + "\n\n" + double_initial_value
+
+    # Reuses the experiment, tuning parameters etc. settings
+    number_line_initial_name = 104  # Line where the string char initialName(,) is always stored
+    with open(filename, "r") as file:
+        content = file.read().split("\n")
+
+    new_content = "\n".join(content[:number_line_initial_name])
+    new_content += "\n" + string_new_ds_final
+    # Save new content to given savepath
+    with open(savepath, "a+") as file:
+        file.seek(0)
+        file.truncate()  # Delete all content of the given file
+        file.write(new_content)
```

### Comparing `ebcpy-0.3.2/ebcpy/modelica/simres.py` & `ebcpy-0.3.6/ebcpy/modelica/simres.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,334 +1,334 @@
-# Copyright (c) 2010-2014, Kevin Davies, Hawaii Natural Energy Institute (HNEI),
-# and Georgia Tech Research Corporation (GTRC).
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions are met:
-#
-#     * Redistributions of source code must retain the above copyright notice,
-#       this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above copyright notice,
-#       this list of conditions and the following disclaimer in the documentation
-#       and/or other materials provided with the distribution.
-#     * Neither the name of Georgia Tech Research Corporation nor the names of
-#       its contributors may be used to endorse or promote products derived from
-#       this software without specific prior written permission.
-#     * This software is controlled under the jurisdiction of the United States
-#       Department of Commerce and subject to Export Administration Regulations.
-#       By downloading or using the Software, you are agreeing to comply with
-#       U. S. export controls.  Diversion contrary to law is prohibited.  The
-#       software cannot be exported or reexported to sanctioned countries that
-#       are controlled for Anti-Terrorism (15 CFR Part 738 Supplement 1) or to
-#       denied parties, http://beta-www.bis.doc.gov/index.php/policy-guidance/lists-of-parties-of-concern.
-#       EAR99 items cannot be exported or reexported to Iraq for a military
-#       purpose or to a military end-user (15 CFR Part 746.3).  Export and
-#       reexport include any release of technology to a foreign national within
-#       the United States.  Technology is released for export when it is
-#       available to foreign nationals for visual inspection, when technology is
-#       exchanged orally or when technology is made available by practice or
-#       application under the guidance of persons with knowledge of the
-#       technology.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL GEORGIA TECH RESEARCH CORPORATION BE LIABLE FOR
-# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-"""
-Module based on the simres module of modelicares. As no new content is going to be
-merged upstream, this "fork" of the to_pandas() function is used.
-
-Update 18.01.2021:
-As modelicares is no longer compatible with matplotlib > 3.3.2, we integrated all
-necessary functions from modelicares to still be able and use loadsim functions.
-
-.. versionadded:: 0.1.7
-"""
-from itertools import count
-from collections import namedtuple
-from scipy.io import loadmat
-from scipy.io.matlab.mio_utils import chars_to_strings
-import pandas as pd
-import numpy as np
-
-
-# Namedtuple to store the time and value information of each variable
-Samples = namedtuple('Samples', ['times', 'values', 'negated'])
-
-
-def loadsim(fname, constants_only=False):
-    r"""Load Dymola\ :sup:`®` or OpenModelica simulation results.
-
-    **Arguments:**
-
-    - *fname*: Name of the results file, including the path
-
-         The file extension ('.mat') is optional.
-
-    - *constants_only*: *True* to load only the variables from the first data
-      matrix
-
-         The first data matrix usually contains all of the constants,
-         parameters, and variables that don't vary.  If only that information is
-         needed, it may save resources to set *constants_only* to *True*.
-
-    **Returns:** An instance of dict
-    """
-    # This does the task of mfiles/traj/tload.m from the Dymola installation.
-
-    def parse(description):
-        """Parse the variable description string into description, unit, and
-        displayUnit.
-        """
-        description = description.rstrip(']')
-        display_unit = ''
-        try:
-            description, unit = description.rsplit('[', 1)
-        except ValueError:
-            unit = ''
-        else:
-            try:
-                unit, display_unit = unit.rsplit('|', 1)
-            except ValueError:
-                pass # (displayUnit = '')
-        description = description.rstrip()
-
-        return description, unit, display_unit
-
-    # Load the file.
-    mat, aclass = read(fname, constants_only)
-
-    # Check the type of results.
-    if aclass[0] == 'AlinearSystem':
-        raise AssertionError(fname + ' is a linearization result.  Use LinRes '
-                             'instead.')
-    if aclass[0] != 'Atrajectory':
-        raise AssertionError(fname + ' is not a simulation or '
-                                     'linearization result.')
-
-    # Determine if the data is transposed.
-    try:
-        transposed = aclass[3] == 'binTrans'
-    except IndexError:
-        transposed = False
-    else:
-        if not (transposed or aclass[3] == 'binNormal'):
-            raise AssertionError\
-                ('The orientation of the Dymola/OpenModelica results is not '
-                 'recognized.  The third line of the "Aclass" variable is "%s", but '
-                 'it should be "binNormal" or "binTrans".' % aclass[3])
-
-    # Get the format version.
-    version = aclass[1]
-
-    # Process the name, description, parts of dataInfo, and data_i variables.
-    # This section has been optimized for speed.  All time and value data
-    # remains linked to the memory location where it is loaded by scipy.  The
-    # negated variable is carried through so that copies are not necessary.  If
-    # changes are made to this code, be sure to compare the performance (e.g.,
-    # using %timeit in IPython).
-    if version == '1.0':
-        data = mat['data'].T if transposed else mat['data']
-        times = data[:, 0]
-        names = get_strings(mat['names'].T if transposed else mat['names'])
-        variables = {name: Variable(Samples(times, data[:, i], False),
-                                    '', '', '')
-                     for i, name in enumerate(names)}
-    elif version != '1.1':
-        raise AssertionError('The version of the Dymola/OpenModelica '
-                             f'result file ({version}) is not '
-                             'supported.')
-    else:
-        names = get_strings(mat['name'].T if transposed else mat['name'])
-        descriptions = get_strings(mat['description'].T if transposed else
-                                   mat['description'])
-        data_info = mat['dataInfo'] if transposed else mat['dataInfo'].T
-        data_sets = data_info[0, :]
-        sign_cols = data_info[1, :]
-        variables = dict()
-        for i in count(1):
-            try:
-                data = (mat['data_%i' % i].T if transposed else
-                        mat['data_%i' % i])
-            except KeyError:
-                break # There are no more "data_i" variables.
-            else:
-                if data.shape[1] > 1: # In case the data set is empty.
-                    times = data[:, 0]
-                    variables.update({name:
-                                      Variable(Samples(times,
-                                                       data[:,
-                                                            abs(sign_col) - 1],
-                                                       sign_col < 0),
-                                               *parse(description))
-                                      for (name, description, data_set,
-                                           sign_col)
-                                      in zip(names, descriptions, data_sets,
-                                             sign_cols)
-                                      if data_set == i})
-
-        # Time is from the last data set.
-        variables['Time'] = Variable(Samples(times, times, False),
-                                     'Time', 's', '')
-
-    return variables
-
-
-def read(fname, constants_only=False):
-    r"""Read variables from a MATLAB\ :sup:`®` file with Dymola\ :sup:`®` or
-    OpenModelica results.
-
-    **Arguments:**
-
-    - *fname*: Name of the results file, including the path
-
-         This may be from a simulation or linearization.
-
-    - *constants_only*: *True* to load only the variables from the first data
-      matrix, if the result is from a simulation
-
-    **Returns:**
-
-    1. A dictionary of variables
-
-    2. A list of strings from the lines of the 'Aclass' matrix
-    """
-
-    # Load the file.
-    try:
-        if constants_only:
-            mat = loadmat(fname, chars_as_strings=False, appendmat=False,
-                          variable_names=['Aclass', 'class', 'name', 'names',
-                                          'description', 'dataInfo', 'data',
-                                          'data_1', 'ABCD', 'nx', 'xuyName'])
-        else:
-            mat = loadmat(fname, chars_as_strings=False, appendmat=False)
-    except IOError as error:
-        raise IOError(f'"{fname}" could not be opened.'
-                      '  Check that it exists.') from error
-
-    # Check if the file contains the Aclass variable.
-    try:
-        aclass = mat['Aclass']
-    except KeyError as error:
-        raise TypeError(f'"{fname}" does not appear to be a Dymola or OpenModelica '
-                        'result file.  The "Aclass" variable is '
-                        'missing.') from error
-
-    return mat, get_strings(aclass)
-
-
-def get_strings(str_arr):
-    """Return a list of strings from a character array.
-
-    Strip the whitespace from the right and recode it as utf-8.
-    """
-    return [line.rstrip(' \0').encode('latin-1').decode('utf-8')
-            for line in chars_to_strings(str_arr)]
-
-
-class Variable(namedtuple('VariableNamedTuple', ['samples', 'description', 'unit', 'displayUnit'])):
-    """Special namedtuple to represent a variable in a simulation, with
-    methods to retrieve and perform calculations on its values
-
-    This class is usually not instantiated directly by the user, but instances
-    are returned when indexing a variable name from a simulation result
-    (:class:`SimRes` instance).
-    """
-
-    def times(self):
-        """Return sample times"""
-        return self.samples.times
-
-    def values(self):
-        """Return sample values"""
-        return -self.samples.values if self.samples.negated else self.samples.values
-
-
-def mat_to_pandas(fname='dsres.mat',
-                  names=None,
-                  aliases=None,
-                  with_unit=True,
-                  constants_only=False):
-    """
-    Return a `pandas.DataFrame` with values from selected variables
-    for the given .mat file.
-
-    The index is time. The column headings indicate the variable names and
-    units.
-
-    :param str fname:
-        The mat file to load.
-    :param list names:
-        If None (default), then all variables are included.
-    :param dict aliases:
-        Dictionary of aliases for the variable names
-
-        The keys are the "official" variable names from the Modelica model
-        and the values are the names as they should be included in the
-        column headings. Any variables not in this list will not be
-        aliased. Any unmatched aliases will not be used.
-    :param bool with_unit:
-        Boolean to determine format of keys. Default value is True.
-
-        If set to True, the unit will be added to the key. As not all modelica-
-        result files export the unit information, using with_unit=True can lead
-        to errors.
-    :param bool constants_only:
-        The first data matrix usually contains all of the constants,
-        parameters, and variables that don't vary.  If only that information is
-        needed, it may save resources to set *constants_only* to *True*.
-    """
-    _variables = loadsim(fname, constants_only)
-    # Avoid mutable argument
-    if aliases is None:
-        aliases = {}
-
-    # Create the list of variable names.
-    if names:
-        if 'Time' not in names:
-            names.append('Time')
-    else:
-        names = _variables.keys()
-
-    # Create a dictionary of names and values.
-    times = _variables['Time'].values()
-    data = {}
-    for name in names:
-
-        # Get the values.
-        if np.array_equal(_variables[name].times(), times):
-            values = _variables[name].values()  # Save computation.
-        # Check if all values are constant to save resampling time
-        elif np.count_nonzero(_variables[name].values() -
-                              np.max(_variables[name].values())) == 0:
-            # Passing a scalar converts automatically to an array.
-            values = np.max(_variables[name].values())
-        else:
-            values = _variables[name].values(t=times)  # Resample.
-
-        unit = _variables[name].unit
-
-        # Apply an alias if available.
-        try:
-            name = aliases[name]
-        except KeyError:
-            pass
-
-        if unit and with_unit:
-            data.update({name + ' / ' + unit: values})
-        else:
-            data.update({name: values})
-
-    # Create the pandas data frame.
-    if with_unit:
-        time_key = 'Time / s'
-    else:
-        time_key = 'Time'
-    return pd.DataFrame(data).set_index(time_key)
+# Copyright (c) 2010-2014, Kevin Davies, Hawaii Natural Energy Institute (HNEI),
+# and Georgia Tech Research Corporation (GTRC).
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+#     * Redistributions of source code must retain the above copyright notice,
+#       this list of conditions and the following disclaimer.
+#     * Redistributions in binary form must reproduce the above copyright notice,
+#       this list of conditions and the following disclaimer in the documentation
+#       and/or other materials provided with the distribution.
+#     * Neither the name of Georgia Tech Research Corporation nor the names of
+#       its contributors may be used to endorse or promote products derived from
+#       this software without specific prior written permission.
+#     * This software is controlled under the jurisdiction of the United States
+#       Department of Commerce and subject to Export Administration Regulations.
+#       By downloading or using the Software, you are agreeing to comply with
+#       U. S. export controls.  Diversion contrary to law is prohibited.  The
+#       software cannot be exported or reexported to sanctioned countries that
+#       are controlled for Anti-Terrorism (15 CFR Part 738 Supplement 1) or to
+#       denied parties, http://beta-www.bis.doc.gov/index.php/policy-guidance/lists-of-parties-of-concern.
+#       EAR99 items cannot be exported or reexported to Iraq for a military
+#       purpose or to a military end-user (15 CFR Part 746.3).  Export and
+#       reexport include any release of technology to a foreign national within
+#       the United States.  Technology is released for export when it is
+#       available to foreign nationals for visual inspection, when technology is
+#       exchanged orally or when technology is made available by practice or
+#       application under the guidance of persons with knowledge of the
+#       technology.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL GEORGIA TECH RESEARCH CORPORATION BE LIABLE FOR
+# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+"""
+Module based on the simres module of modelicares. As no new content is going to be
+merged upstream, this "fork" of the to_pandas() function is used.
+
+Update 18.01.2021:
+As modelicares is no longer compatible with matplotlib > 3.3.2, we integrated all
+necessary functions from modelicares to still be able and use loadsim functions.
+
+.. versionadded:: 0.1.7
+"""
+from itertools import count
+from collections import namedtuple
+from scipy.io import loadmat
+from scipy.io.matlab.mio_utils import chars_to_strings
+import pandas as pd
+import numpy as np
+
+
+# Namedtuple to store the time and value information of each variable
+Samples = namedtuple('Samples', ['times', 'values', 'negated'])
+
+
+def loadsim(fname, constants_only=False):
+    r"""Load Dymola\ :sup:`®` or OpenModelica simulation results.
+
+    **Arguments:**
+
+    - *fname*: Name of the results file, including the path
+
+         The file extension ('.mat') is optional.
+
+    - *constants_only*: *True* to load only the variables from the first data
+      matrix
+
+         The first data matrix usually contains all of the constants,
+         parameters, and variables that don't vary.  If only that information is
+         needed, it may save resources to set *constants_only* to *True*.
+
+    **Returns:** An instance of dict
+    """
+    # This does the task of mfiles/traj/tload.m from the Dymola installation.
+
+    def parse(description):
+        """Parse the variable description string into description, unit, and
+        displayUnit.
+        """
+        description = description.rstrip(']')
+        display_unit = ''
+        try:
+            description, unit = description.rsplit('[', 1)
+        except ValueError:
+            unit = ''
+        else:
+            try:
+                unit, display_unit = unit.rsplit('|', 1)
+            except ValueError:
+                pass # (displayUnit = '')
+        description = description.rstrip()
+
+        return description, unit, display_unit
+
+    # Load the file.
+    mat, aclass = read(fname, constants_only)
+
+    # Check the type of results.
+    if aclass[0] == 'AlinearSystem':
+        raise AssertionError(fname + ' is a linearization result.  Use LinRes '
+                             'instead.')
+    if aclass[0] != 'Atrajectory':
+        raise AssertionError(fname + ' is not a simulation or '
+                                     'linearization result.')
+
+    # Determine if the data is transposed.
+    try:
+        transposed = aclass[3] == 'binTrans'
+    except IndexError:
+        transposed = False
+    else:
+        if not (transposed or aclass[3] == 'binNormal'):
+            raise AssertionError\
+                ('The orientation of the Dymola/OpenModelica results is not '
+                 'recognized.  The third line of the "Aclass" variable is "%s", but '
+                 'it should be "binNormal" or "binTrans".' % aclass[3])
+
+    # Get the format version.
+    version = aclass[1]
+
+    # Process the name, description, parts of dataInfo, and data_i variables.
+    # This section has been optimized for speed.  All time and value data
+    # remains linked to the memory location where it is loaded by scipy.  The
+    # negated variable is carried through so that copies are not necessary.  If
+    # changes are made to this code, be sure to compare the performance (e.g.,
+    # using %timeit in IPython).
+    if version == '1.0':
+        data = mat['data'].T if transposed else mat['data']
+        times = data[:, 0]
+        names = get_strings(mat['names'].T if transposed else mat['names'])
+        variables = {name: Variable(Samples(times, data[:, i], False),
+                                    '', '', '')
+                     for i, name in enumerate(names)}
+    elif version != '1.1':
+        raise AssertionError('The version of the Dymola/OpenModelica '
+                             f'result file ({version}) is not '
+                             'supported.')
+    else:
+        names = get_strings(mat['name'].T if transposed else mat['name'])
+        descriptions = get_strings(mat['description'].T if transposed else
+                                   mat['description'])
+        data_info = mat['dataInfo'] if transposed else mat['dataInfo'].T
+        data_sets = data_info[0, :]
+        sign_cols = data_info[1, :]
+        variables = dict()
+        for i in count(1):
+            try:
+                data = (mat['data_%i' % i].T if transposed else
+                        mat['data_%i' % i])
+            except KeyError:
+                break # There are no more "data_i" variables.
+            else:
+                if data.shape[1] > 1: # In case the data set is empty.
+                    times = data[:, 0]
+                    variables.update({name:
+                                      Variable(Samples(times,
+                                                       data[:,
+                                                            abs(sign_col) - 1],
+                                                       sign_col < 0),
+                                               *parse(description))
+                                      for (name, description, data_set,
+                                           sign_col)
+                                      in zip(names, descriptions, data_sets,
+                                             sign_cols)
+                                      if data_set == i})
+
+        # Time is from the last data set.
+        variables['Time'] = Variable(Samples(times, times, False),
+                                     'Time', 's', '')
+
+    return variables
+
+
+def read(fname, constants_only=False):
+    r"""Read variables from a MATLAB\ :sup:`®` file with Dymola\ :sup:`®` or
+    OpenModelica results.
+
+    **Arguments:**
+
+    - *fname*: Name of the results file, including the path
+
+         This may be from a simulation or linearization.
+
+    - *constants_only*: *True* to load only the variables from the first data
+      matrix, if the result is from a simulation
+
+    **Returns:**
+
+    1. A dictionary of variables
+
+    2. A list of strings from the lines of the 'Aclass' matrix
+    """
+
+    # Load the file.
+    try:
+        if constants_only:
+            mat = loadmat(fname, chars_as_strings=False, appendmat=False,
+                          variable_names=['Aclass', 'class', 'name', 'names',
+                                          'description', 'dataInfo', 'data',
+                                          'data_1', 'ABCD', 'nx', 'xuyName'])
+        else:
+            mat = loadmat(fname, chars_as_strings=False, appendmat=False)
+    except IOError as error:
+        raise IOError(f'"{fname}" could not be opened.'
+                      '  Check that it exists.') from error
+
+    # Check if the file contains the Aclass variable.
+    try:
+        aclass = mat['Aclass']
+    except KeyError as error:
+        raise TypeError(f'"{fname}" does not appear to be a Dymola or OpenModelica '
+                        'result file.  The "Aclass" variable is '
+                        'missing.') from error
+
+    return mat, get_strings(aclass)
+
+
+def get_strings(str_arr):
+    """Return a list of strings from a character array.
+
+    Strip the whitespace from the right and recode it as utf-8.
+    """
+    return [line.rstrip(' \0').encode('latin-1').decode('utf-8')
+            for line in chars_to_strings(str_arr)]
+
+
+class Variable(namedtuple('VariableNamedTuple', ['samples', 'description', 'unit', 'displayUnit'])):
+    """Special namedtuple to represent a variable in a simulation, with
+    methods to retrieve and perform calculations on its values
+
+    This class is usually not instantiated directly by the user, but instances
+    are returned when indexing a variable name from a simulation result
+    (:class:`SimRes` instance).
+    """
+
+    def times(self):
+        """Return sample times"""
+        return self.samples.times
+
+    def values(self):
+        """Return sample values"""
+        return -self.samples.values if self.samples.negated else self.samples.values
+
+
+def mat_to_pandas(fname='dsres.mat',
+                  names=None,
+                  aliases=None,
+                  with_unit=True,
+                  constants_only=False):
+    """
+    Return a `pandas.DataFrame` with values from selected variables
+    for the given .mat file.
+
+    The index is time. The column headings indicate the variable names and
+    units.
+
+    :param str fname:
+        The mat file to load.
+    :param list names:
+        If None (default), then all variables are included.
+    :param dict aliases:
+        Dictionary of aliases for the variable names
+
+        The keys are the "official" variable names from the Modelica model
+        and the values are the names as they should be included in the
+        column headings. Any variables not in this list will not be
+        aliased. Any unmatched aliases will not be used.
+    :param bool with_unit:
+        Boolean to determine format of keys. Default value is True.
+
+        If set to True, the unit will be added to the key. As not all modelica-
+        result files export the unit information, using with_unit=True can lead
+        to errors.
+    :param bool constants_only:
+        The first data matrix usually contains all of the constants,
+        parameters, and variables that don't vary.  If only that information is
+        needed, it may save resources to set *constants_only* to *True*.
+    """
+    _variables = loadsim(fname, constants_only)
+    # Avoid mutable argument
+    if aliases is None:
+        aliases = {}
+
+    # Create the list of variable names.
+    if names:
+        if 'Time' not in names:
+            names.append('Time')
+    else:
+        names = _variables.keys()
+
+    # Create a dictionary of names and values.
+    times = _variables['Time'].values()
+    data = {}
+    for name in names:
+
+        # Get the values.
+        if np.array_equal(_variables[name].times(), times):
+            values = _variables[name].values()  # Save computation.
+        # Check if all values are constant to save resampling time
+        elif np.count_nonzero(_variables[name].values() -
+                              np.max(_variables[name].values())) == 0:
+            # Passing a scalar converts automatically to an array.
+            values = np.max(_variables[name].values())
+        else:
+            values = _variables[name].values(t=times)  # Resample.
+
+        unit = _variables[name].unit
+
+        # Apply an alias if available.
+        try:
+            name = aliases[name]
+        except KeyError:
+            pass
+
+        if unit and with_unit:
+            data.update({name + ' / ' + unit: values})
+        else:
+            data.update({name: values})
+
+    # Create the pandas data frame.
+    if with_unit:
+        time_key = 'Time / s'
+    else:
+        time_key = 'Time'
+    return pd.DataFrame(data).set_index(time_key)
```

### Comparing `ebcpy-0.3.2/ebcpy/optimization.py` & `ebcpy-0.3.6/ebcpy/optimization.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,482 +1,482 @@
-"""Base-module for the whole optimization pacakge.
-Used to define Base-Classes such as Optimizer and
-Calibrator."""
-
-import os
-from typing import List, Tuple, Union
-from collections import namedtuple
-from abc import abstractmethod
-import numpy as np
-from ebcpy.utils import setup_logger
-# pylint: disable=import-outside-toplevel
-# pylint: disable=broad-except
-
-
-class Optimizer:
-    """
-    Base class for optimization in ebcpy. All classes
-    performing optimization tasks must inherit from this
-    class.
-    The main feature of this class is the common interface
-    for different available solvers in python. This makes the
-    testing of different solvers and methods more easy.
-    For available frameworks/solvers, check the function
-    self.optimize().
-
-
-    :param str,os.path.normpath cd:
-        Directory for storing all output of optimization via a logger.
-    :keyword list bounds:
-        The boundaries for the optimization variables.
-    """
-
-    # Used to display number of obj-function-calls
-    _counter = 0
-    # Used to access the current parameter set if an optimization-step fails
-    _current_iterate = np.array([])
-    # Used to access the best iterate if an optimization step fails
-    _current_best_iterate = {"Objective": np.inf}
-    # List storing every objective value for plotting and logging.
-    # Can be used, but will enlarge runtime
-    _obj_his = []
-
-    def __init__(self, cd=None, **kwargs):
-        """Instantiate class parameters"""
-        if cd is None:
-            self._cd = None
-        else:
-            self.cd = cd
-
-        self.logger = setup_logger(cd=self.cd, name=self.__class__.__name__)
-        # Set kwargs
-        self.bounds = kwargs.get("bounds", None)
-
-    @abstractmethod
-    def obj(self, xk, *args):
-        """
-        Base objective function. Overload this function and create your own
-        objective function. Make sure that the return value is a scalar.
-        Furthermore, the parameter vector xk is always a numpy array.
-
-        :param np.array xk:
-            Array with parameters for optimization
-
-        :return: float result:
-            A scalar (float/ 1d) value for the optimization framework.
-        """
-        raise NotImplementedError(f'{self.__class__.__name__}.obj function is not defined')
-
-    @abstractmethod
-    def mp_obj(self, x, *args):
-        """
-        Objective function for Multiprocessing.
-
-        :param np.array x:
-            Array with parameters for optimization.
-            Shape of the array is (number_of_evaluations x number_of_variables).
-            For instance, optimizating 10 variables and evaluating
-            900 objectives in parallel, the shape would be 900 x 10.
-        :param int n_cpu:
-            Number of logical Processors to run optimization on.
-        """
-        raise NotImplementedError(f'{self.__class__.__name__}.obj function is not defined')
-
-    @property
-    def supported_frameworks(self):
-        """
-        List with all frameworks supported by this
-        wrapper class.
-        """
-        return ["scipy_minimize",
-                "scipy_differential_evolution",
-                "dlib_minimize",
-                "pymoo"]
-
-    @property
-    def cd(self) -> str:
-        """The current working directory"""
-        return self._cd
-
-    @cd.setter
-    def cd(self, cd: str):
-        """Set current working directory"""
-        os.makedirs(cd, exist_ok=True)
-        self._cd = cd
-
-    @property
-    def bounds(self) -> List[Union[Tuple, List]]:
-        """The boundaries of the optimization problem."""
-        return self._bounds
-
-    @bounds.setter
-    def bounds(self, bounds):
-        """Set the boundaries to the optimization variables"""
-        self._bounds = bounds
-
-    def optimize(self, framework, method=None, n_cpu=1, **kwargs):
-        """
-        Perform the optimization based on the given method and framework.
-
-        :param str framework:
-            The framework (python module) you want to use to perform the optimization.
-            Currently, "scipy_minimize", "dlib_minimize" and "scipy_differential_evolution"
-            are supported options. To further inform yourself about these frameworks, please see:
-            - `dlib <http://dlib.net/python/index.html>`_
-            - `scipy minimize <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html>`_
-            - `scipy differential evolution <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.differential_evolution.html>`_
-            - 'pymoo' <https://pymoo.org/index.html>
-        :param str method:
-            The method you pass depends on the methods available in the framework
-            you chose when setting up the class. Some frameworks don't require a
-            method, as only one exists. This is the case for dlib. For any framework
-            with different methods, you must provide one.
-            For the scipy.differential_evolution function, method is equal to the
-            strategy.
-            For the pymoo function, method is equal to the
-            algorithm.
-        :param int n_cpu:
-            Number of parallel processes used for the evaluation.
-            Ignored if the framework-method combination does not
-            support multi-processing.
-
-        Keyword arguments:
-            Depending on the framework an method you use, you can fine-tune the
-            optimization tool using extra arguments. We refer to the documentation of
-            each framework for a listing of what parameters are supported and how
-            to set them.
-            E.g. For scipy.optimize.minimize one could
-            add "tol=1e-3" as a kwarg.
-
-        :return: res
-            Optimization result.
-        """
-        # Choose the framework
-        minimize_func, requires_method = self._choose_framework(framework)
-        if method is None and requires_method:
-            raise ValueError(f"{framework} requires a method, but None is "
-                             f"provided. Please choose one.")
-        # Perform minimization
-        res = minimize_func(method=method, n_cpu=n_cpu, **kwargs)
-        return res
-
-    def _choose_framework(self, framework):
-        """
-        Function to select the functions for optimization
-        and for executing said functions.
-
-        :param str framework:
-            String for selection of the relevant function. Supported options are:
-            - scipy_minimize
-            - dlib_minimize
-            - scipy_differential_evolution
-            - pymoo
-        """
-        if framework.lower() == "scipy_minimize":
-            return self._scipy_minimize, True
-        if framework.lower() == "dlib_minimize":
-            return self._dlib_minimize, False
-        if framework.lower() == "scipy_differential_evolution":
-            return self._scipy_differential_evolution, True
-        if framework.lower() == "pymoo":
-            return self._pymoo, True
-        raise TypeError(f"Given framework {framework} is currently not supported.")
-
-    def _scipy_minimize(self, method, n_cpu=1, **kwargs):
-        """
-        Possible kwargs for the scipy minimize function with default values:
-
-        x0: Required
-        tol = None
-        options = None
-        constraints = {}
-        jac = None
-        hess = None
-        hessp = None
-        """
-        default_kwargs = self.get_default_config(framework="scipy_minimize")
-        default_kwargs.update(kwargs)
-        try:
-            import scipy.optimize as opt
-        except ImportError as error:
-            raise ImportError("Please install scipy to use "
-                              "the minimize_scipy function.") from error
-
-        try:
-            if "x0" not in kwargs:
-                raise KeyError("An initial guess (x0) is required "
-                               "for scipy.minimize. You passed None")
-            res = opt.minimize(
-                fun=self.obj,
-                x0=kwargs["x0"],
-                method=method,
-                jac=default_kwargs["jac"],
-                hess=default_kwargs["hess"],
-                hessp=default_kwargs["hessp"],
-                bounds=self.bounds,
-                constraints=default_kwargs["constraints"],
-                tol=default_kwargs["tol"],
-                options=default_kwargs["options"]
-            )
-            return res
-        except (KeyboardInterrupt, Exception) as error:
-            # pylint: disable=inconsistent-return-statements
-            self._handle_error(error)
-
-    def _dlib_minimize(self, method=None, n_cpu=1, **kwargs):
-        """
-        Possible kwargs for the dlib minimize function with default values:
-
-        is_integer_variable = None
-        solver_epsilon = 0
-        num_function_calls = int(1e9)
-        """
-        default_kwargs = self.get_default_config(framework="dlib_minimize")
-        default_kwargs.update(kwargs)
-        try:
-            import dlib
-        except ImportError as error:
-            raise ImportError("Please install dlib to use the minimize_dlib function.") from error
-        try:
-            _bounds_2d = np.array(self.bounds)
-            _bound_min = list(_bounds_2d[:, 0])
-            _bound_max = list(_bounds_2d[:, 1])
-            if "is_integer_variable" not in kwargs:
-                is_integer_variable = list(np.zeros(len(_bound_max)))
-            else:
-                is_integer_variable = kwargs["is_integer_variable"]
-
-            # This check is only necessary as the error-messages from dlib are quite indirect.
-            # Any new user would not get that these parameters cause the error.
-            for key in ["solver_epsilon", "num_function_calls"]:
-                value = kwargs.get(key)
-                if value is not None:
-                    if not isinstance(value, (float, int)):
-                        raise TypeError(
-                            f"Given {key} is of type {type(value).__name__} but "
-                            f"should be type float or int"
-                        )
-
-            x_res, f_res = dlib.find_min_global(
-                f=self._dlib_obj,
-                bound1=_bound_min,
-                bound2=_bound_max,
-                is_integer_variable=is_integer_variable,
-                num_function_calls=int(default_kwargs["num_function_calls"]),
-                solver_epsilon=float(default_kwargs["solver_epsilon"])
-            )
-            res_tuple = namedtuple("res_tuple", "x fun")
-            res = res_tuple(x=x_res, fun=f_res)
-            return res
-        except (KeyboardInterrupt, Exception) as error:
-            # pylint: disable=inconsistent-return-statements
-            self._handle_error(error)
-
-    def _scipy_differential_evolution(self, method="best1bin", n_cpu=1, **kwargs):
-        """
-        Possible kwargs for the dlib minimize function with default values:
-
-        maxiter = 1000
-        popsize = 15
-        tol = None
-        mutation = (0.5, 1)
-        recombination = 0.7
-        seed = None
-        polish = True
-        init = 'latinhypercube'
-        atol = 0
-        """
-        default_kwargs = self.get_default_config(framework="scipy_differential_evolution")
-        default_kwargs.update(kwargs)
-        try:
-            import scipy.optimize as opt
-        except ImportError as error:
-            raise ImportError("Please install scipy to use the minimize_scipy function.") from error
-
-        try:
-            if self.bounds is None:
-                raise ValueError("For the differential evolution approach, you need to specify "
-                                 "boundaries. Currently, no bounds are specified.")
-
-            res = opt.differential_evolution(
-                func=self.obj,
-                bounds=self.bounds,
-                strategy=method,
-                maxiter=default_kwargs["maxiter"],
-                popsize=default_kwargs["popsize"],
-                tol=default_kwargs["tol"],
-                mutation=default_kwargs["mutation"],
-                recombination=default_kwargs["recombination"],
-                seed=default_kwargs["seed"],
-                disp=False,  # We have our own logging
-                polish=default_kwargs["polish"],
-                init=default_kwargs["init"],
-                atol=default_kwargs["atol"]
-            )
-            return res
-        except (KeyboardInterrupt, Exception) as error:
-            # pylint: disable=inconsistent-return-statements
-            self._handle_error(error)
-
-    def _pymoo(self, method="NSGA2", n_cpu=1, **kwargs):
-        """
-        Possible kwargs for the dlib minimize function with default values:
-
-        algorithm=NGSA2
-        termination=None
-        seed=None
-        verbose=False
-        display=None
-        callback=None
-        save_history=False
-        copy_algorithm=False
-        copy_termination=False
-        """
-        default_kwargs = self.get_default_config(framework="pymoo")
-
-        try:
-            from pymoo.optimize import minimize
-            from pymoo.problems.single import Problem
-            from pymoo.factory import get_algorithm, get_sampling, get_mutation, get_crossover, get_selection
-        except ImportError as error:
-            raise ImportError("Please install pymoo to use this function.") from error
-
-        class EBCPYProblem(Problem):
-            """Construct wrapper problem class."""
-            def __init__(self,
-                         ebcpy_class: Optimizer
-                         ):
-                self.ebcpy_class = ebcpy_class
-                super().__init__(n_var=len(ebcpy_class.bounds),
-                                 n_obj=1,
-                                 n_constr=0,
-                                 xl=np.array([bound[0] for bound in ebcpy_class.bounds]),
-                                 xu=np.array([bound[1] for bound in ebcpy_class.bounds])
-                                 )
-
-            def _evaluate(self, x, out, *args, **kwargs):
-                if n_cpu > 1:
-                    out["F"] = self.ebcpy_class.mp_obj(x, n_cpu, *args)
-                else:
-                    out["F"] = np.array([self.ebcpy_class.obj(xk=_x, *args) for _x in x])
-
-        try:
-            if self.bounds is None:
-                raise ValueError("For pymoo, you need to specify "
-                                 "boundaries. Currently, no bounds are specified.")
-
-            termination = default_kwargs.pop("termination")
-            if termination is None:
-                termination = ("n_gen", default_kwargs.pop("n_gen"))
-            seed = default_kwargs.pop("seed")
-            verbose = default_kwargs.pop("verbose")
-            save_history = default_kwargs.pop("save_history")
-            copy_algorithm = default_kwargs.pop("copy_algorithm")
-            copy_termination = default_kwargs.pop("copy_termination")
-
-            # Init algorithm
-            if method.lower() == "ga":
-                from pymoo.algorithms.soo.nonconvex.ga import GA
-                # GA:
-                pop_size = kwargs["pop_size"]
-                sampling = get_sampling(name=kwargs["sampling"])
-                selection = get_selection(name=kwargs["selection"])
-                crossover = get_crossover(name=kwargs["crossover"])
-                mutation = get_mutation(name=kwargs["mutation"])
-                eliminate_duplicates = kwargs["eliminate_duplicates"]
-                n_offsprings = kwargs["n_offsprings"]
-                algorithm = GA(pop_size=pop_size,
-                               sampling=sampling,
-                               selection=selection,
-                               crossover=crossover,
-                               mutation=mutation,
-                               eliminate_duplicates=eliminate_duplicates,
-                               n_offsprings=n_offsprings
-                               )
-            else:
-                default_kwargs.update(kwargs)
-                algorithm = get_algorithm(name=method.lower(),
-                                          **default_kwargs)
-
-            res = minimize(
-                problem=EBCPYProblem(ebcpy_class=self),
-                algorithm=algorithm,
-                termination=termination,
-                seed=seed,
-                verbose=verbose,
-                display=None,
-                callback=None,
-                save_history=save_history,
-                copy_algorithm=copy_algorithm,
-                copy_termination=copy_termination,
-            )
-            res_tuple = namedtuple("res_tuple", "x fun")
-            res = res_tuple(x=res.X, fun=res.F[0])
-            return res
-        except (KeyboardInterrupt, Exception) as error:
-            # pylint: disable=inconsistent-return-statements
-            self._handle_error(error)
-
-    def _dlib_obj(self, *args):
-        """
-        This function is needed as the signature for the dlib-obj
-        is different than the standard signature. dlib will parse a number of
-        parameters
-        """
-        return self.obj(np.array(args))
-
-    def _handle_error(self, error):
-        """
-        Function to handle the case when an optimization step fails (e.g. simulation-fail).
-        The parameter set which caused the failure and the best iterate until this point
-        are of interest for the user in such case.
-        :param error:
-            Any Exception that may occur
-        """
-        self.logger.error(f"Parameter set which caused the failure: {self._current_iterate}")
-        self.logger.error("Current best objective and parameter set:")
-        self.logger.error("\n".join([f"{key}: {value}"
-                                     for key, value in self._current_best_iterate.items()]))
-        raise error
-
-    @staticmethod
-    def get_default_config(framework: str) -> dict:
-        """
-        Return the default config or kwargs for the
-        given framework.
-
-        The default values are extracted of the corresponding
-        framework directly.
-        """
-        if framework.lower() == "scipy_minimize":
-            return {"tol": None,
-                    "options": None,
-                    "constraints": None,
-                    "jac": None,
-                    "hess": None,
-                    "hessp": None}
-        if framework.lower() == "dlib_minimize":
-            return {"num_function_calls": int(1e9),
-                    "solver_epsilon": 0}
-        if framework.lower() == "scipy_differential_evolution":
-            return {"maxiter": 1000,
-                    "popsize": 15,
-                    "tol": 0.01,
-                    "mutation": (0.5, 1),
-                    "recombination": 0.7,
-                    "seed": None,
-                    "polish": True,
-                    "init": 'latinhypercube',
-                    "atol": 0
-                    }
-        if framework.lower() == "pymoo":
-            return {"n_gen": 1000,
-                    "termination": None,
-                    "seed": 1,
-                    "verbose": False,
-                    "display": None,
-                    "callback": None,
-                    "save_history": False,
-                    "copy_algorithm": False,
-                    "copy_termination": False
-                    }
-        return {}
+"""Base-module for the whole optimization pacakge.
+Used to define Base-Classes such as Optimizer and
+Calibrator."""
+
+import os
+from typing import List, Tuple, Union
+from collections import namedtuple
+from abc import abstractmethod
+import numpy as np
+from ebcpy.utils import setup_logger
+# pylint: disable=import-outside-toplevel
+# pylint: disable=broad-except
+
+
+class Optimizer:
+    """
+    Base class for optimization in ebcpy. All classes
+    performing optimization tasks must inherit from this
+    class.
+    The main feature of this class is the common interface
+    for different available solvers in python. This makes the
+    testing of different solvers and methods more easy.
+    For available frameworks/solvers, check the function
+    self.optimize().
+
+
+    :param str,os.path.normpath cd:
+        Directory for storing all output of optimization via a logger.
+    :keyword list bounds:
+        The boundaries for the optimization variables.
+    """
+
+    # Used to display number of obj-function-calls
+    _counter = 0
+    # Used to access the current parameter set if an optimization-step fails
+    _current_iterate = np.array([])
+    # Used to access the best iterate if an optimization step fails
+    _current_best_iterate = {"Objective": np.inf}
+    # List storing every objective value for plotting and logging.
+    # Can be used, but will enlarge runtime
+    _obj_his = []
+
+    def __init__(self, cd=None, **kwargs):
+        """Instantiate class parameters"""
+        if cd is None:
+            self._cd = None
+        else:
+            self.cd = cd
+
+        self.logger = setup_logger(cd=self.cd, name=self.__class__.__name__)
+        # Set kwargs
+        self.bounds = kwargs.get("bounds", None)
+
+    @abstractmethod
+    def obj(self, xk, *args):
+        """
+        Base objective function. Overload this function and create your own
+        objective function. Make sure that the return value is a scalar.
+        Furthermore, the parameter vector xk is always a numpy array.
+
+        :param np.array xk:
+            Array with parameters for optimization
+
+        :return: float result:
+            A scalar (float/ 1d) value for the optimization framework.
+        """
+        raise NotImplementedError(f'{self.__class__.__name__}.obj function is not defined')
+
+    @abstractmethod
+    def mp_obj(self, x, *args):
+        """
+        Objective function for Multiprocessing.
+
+        :param np.array x:
+            Array with parameters for optimization.
+            Shape of the array is (number_of_evaluations x number_of_variables).
+            For instance, optimizating 10 variables and evaluating
+            900 objectives in parallel, the shape would be 900 x 10.
+        :param int n_cpu:
+            Number of logical Processors to run optimization on.
+        """
+        raise NotImplementedError(f'{self.__class__.__name__}.obj function is not defined')
+
+    @property
+    def supported_frameworks(self):
+        """
+        List with all frameworks supported by this
+        wrapper class.
+        """
+        return ["scipy_minimize",
+                "scipy_differential_evolution",
+                "dlib_minimize",
+                "pymoo"]
+
+    @property
+    def cd(self) -> str:
+        """The current working directory"""
+        return self._cd
+
+    @cd.setter
+    def cd(self, cd: str):
+        """Set current working directory"""
+        os.makedirs(cd, exist_ok=True)
+        self._cd = cd
+
+    @property
+    def bounds(self) -> List[Union[Tuple, List]]:
+        """The boundaries of the optimization problem."""
+        return self._bounds
+
+    @bounds.setter
+    def bounds(self, bounds):
+        """Set the boundaries to the optimization variables"""
+        self._bounds = bounds
+
+    def optimize(self, framework, method=None, n_cpu=1, **kwargs):
+        """
+        Perform the optimization based on the given method and framework.
+
+        :param str framework:
+            The framework (python module) you want to use to perform the optimization.
+            Currently, "scipy_minimize", "dlib_minimize" and "scipy_differential_evolution"
+            are supported options. To further inform yourself about these frameworks, please see:
+            - `dlib <http://dlib.net/python/index.html>`_
+            - `scipy minimize <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html>`_
+            - `scipy differential evolution <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.differential_evolution.html>`_
+            - 'pymoo' <https://pymoo.org/index.html>
+        :param str method:
+            The method you pass depends on the methods available in the framework
+            you chose when setting up the class. Some frameworks don't require a
+            method, as only one exists. This is the case for dlib. For any framework
+            with different methods, you must provide one.
+            For the scipy.differential_evolution function, method is equal to the
+            strategy.
+            For the pymoo function, method is equal to the
+            algorithm.
+        :param int n_cpu:
+            Number of parallel processes used for the evaluation.
+            Ignored if the framework-method combination does not
+            support multi-processing.
+
+        Keyword arguments:
+            Depending on the framework an method you use, you can fine-tune the
+            optimization tool using extra arguments. We refer to the documentation of
+            each framework for a listing of what parameters are supported and how
+            to set them.
+            E.g. For scipy.optimize.minimize one could
+            add "tol=1e-3" as a kwarg.
+
+        :return: res
+            Optimization result.
+        """
+        # Choose the framework
+        minimize_func, requires_method = self._choose_framework(framework)
+        if method is None and requires_method:
+            raise ValueError(f"{framework} requires a method, but None is "
+                             f"provided. Please choose one.")
+        # Perform minimization
+        res = minimize_func(method=method, n_cpu=n_cpu, **kwargs)
+        return res
+
+    def _choose_framework(self, framework):
+        """
+        Function to select the functions for optimization
+        and for executing said functions.
+
+        :param str framework:
+            String for selection of the relevant function. Supported options are:
+            - scipy_minimize
+            - dlib_minimize
+            - scipy_differential_evolution
+            - pymoo
+        """
+        if framework.lower() == "scipy_minimize":
+            return self._scipy_minimize, True
+        if framework.lower() == "dlib_minimize":
+            return self._dlib_minimize, False
+        if framework.lower() == "scipy_differential_evolution":
+            return self._scipy_differential_evolution, True
+        if framework.lower() == "pymoo":
+            return self._pymoo, True
+        raise TypeError(f"Given framework {framework} is currently not supported.")
+
+    def _scipy_minimize(self, method, n_cpu=1, **kwargs):
+        """
+        Possible kwargs for the scipy minimize function with default values:
+
+        x0: Required
+        tol = None
+        options = None
+        constraints = {}
+        jac = None
+        hess = None
+        hessp = None
+        """
+        default_kwargs = self.get_default_config(framework="scipy_minimize")
+        default_kwargs.update(kwargs)
+        try:
+            import scipy.optimize as opt
+        except ImportError as error:
+            raise ImportError("Please install scipy to use "
+                              "the minimize_scipy function.") from error
+
+        try:
+            if "x0" not in kwargs:
+                raise KeyError("An initial guess (x0) is required "
+                               "for scipy.minimize. You passed None")
+            res = opt.minimize(
+                fun=self.obj,
+                x0=kwargs["x0"],
+                method=method,
+                jac=default_kwargs["jac"],
+                hess=default_kwargs["hess"],
+                hessp=default_kwargs["hessp"],
+                bounds=self.bounds,
+                constraints=default_kwargs["constraints"],
+                tol=default_kwargs["tol"],
+                options=default_kwargs["options"]
+            )
+            return res
+        except (KeyboardInterrupt, Exception) as error:
+            # pylint: disable=inconsistent-return-statements
+            self._handle_error(error)
+
+    def _dlib_minimize(self, method=None, n_cpu=1, **kwargs):
+        """
+        Possible kwargs for the dlib minimize function with default values:
+
+        is_integer_variable = None
+        solver_epsilon = 0
+        num_function_calls = int(1e9)
+        """
+        default_kwargs = self.get_default_config(framework="dlib_minimize")
+        default_kwargs.update(kwargs)
+        try:
+            import dlib
+        except ImportError as error:
+            raise ImportError("Please install dlib to use the minimize_dlib function.") from error
+        try:
+            _bounds_2d = np.array(self.bounds)
+            _bound_min = list(_bounds_2d[:, 0])
+            _bound_max = list(_bounds_2d[:, 1])
+            if "is_integer_variable" not in kwargs:
+                is_integer_variable = list(np.zeros(len(_bound_max)))
+            else:
+                is_integer_variable = kwargs["is_integer_variable"]
+
+            # This check is only necessary as the error-messages from dlib are quite indirect.
+            # Any new user would not get that these parameters cause the error.
+            for key in ["solver_epsilon", "num_function_calls"]:
+                value = kwargs.get(key)
+                if value is not None:
+                    if not isinstance(value, (float, int)):
+                        raise TypeError(
+                            f"Given {key} is of type {type(value).__name__} but "
+                            f"should be type float or int"
+                        )
+
+            x_res, f_res = dlib.find_min_global(
+                f=self._dlib_obj,
+                bound1=_bound_min,
+                bound2=_bound_max,
+                is_integer_variable=is_integer_variable,
+                num_function_calls=int(default_kwargs["num_function_calls"]),
+                solver_epsilon=float(default_kwargs["solver_epsilon"])
+            )
+            res_tuple = namedtuple("res_tuple", "x fun")
+            res = res_tuple(x=x_res, fun=f_res)
+            return res
+        except (KeyboardInterrupt, Exception) as error:
+            # pylint: disable=inconsistent-return-statements
+            self._handle_error(error)
+
+    def _scipy_differential_evolution(self, method="best1bin", n_cpu=1, **kwargs):
+        """
+        Possible kwargs for the dlib minimize function with default values:
+
+        maxiter = 1000
+        popsize = 15
+        tol = None
+        mutation = (0.5, 1)
+        recombination = 0.7
+        seed = None
+        polish = True
+        init = 'latinhypercube'
+        atol = 0
+        """
+        default_kwargs = self.get_default_config(framework="scipy_differential_evolution")
+        default_kwargs.update(kwargs)
+        try:
+            import scipy.optimize as opt
+        except ImportError as error:
+            raise ImportError("Please install scipy to use the minimize_scipy function.") from error
+
+        try:
+            if self.bounds is None:
+                raise ValueError("For the differential evolution approach, you need to specify "
+                                 "boundaries. Currently, no bounds are specified.")
+
+            res = opt.differential_evolution(
+                func=self.obj,
+                bounds=self.bounds,
+                strategy=method,
+                maxiter=default_kwargs["maxiter"],
+                popsize=default_kwargs["popsize"],
+                tol=default_kwargs["tol"],
+                mutation=default_kwargs["mutation"],
+                recombination=default_kwargs["recombination"],
+                seed=default_kwargs["seed"],
+                disp=False,  # We have our own logging
+                polish=default_kwargs["polish"],
+                init=default_kwargs["init"],
+                atol=default_kwargs["atol"]
+            )
+            return res
+        except (KeyboardInterrupt, Exception) as error:
+            # pylint: disable=inconsistent-return-statements
+            self._handle_error(error)
+
+    def _pymoo(self, method="NSGA2", n_cpu=1, **kwargs):
+        """
+        Possible kwargs for the dlib minimize function with default values:
+
+        algorithm=NGSA2
+        termination=None
+        seed=None
+        verbose=False
+        display=None
+        callback=None
+        save_history=False
+        copy_algorithm=False
+        copy_termination=False
+        """
+        default_kwargs = self.get_default_config(framework="pymoo")
+
+        try:
+            from pymoo.optimize import minimize
+            from pymoo.problems.single import Problem
+            from pymoo.factory import get_algorithm, get_sampling, get_mutation, get_crossover, get_selection
+        except ImportError as error:
+            raise ImportError("Please install pymoo to use this function.") from error
+
+        class EBCPYProblem(Problem):
+            """Construct wrapper problem class."""
+            def __init__(self,
+                         ebcpy_class: Optimizer
+                         ):
+                self.ebcpy_class = ebcpy_class
+                super().__init__(n_var=len(ebcpy_class.bounds),
+                                 n_obj=1,
+                                 n_constr=0,
+                                 xl=np.array([bound[0] for bound in ebcpy_class.bounds]),
+                                 xu=np.array([bound[1] for bound in ebcpy_class.bounds])
+                                 )
+
+            def _evaluate(self, x, out, *args, **kwargs):
+                if n_cpu > 1:
+                    out["F"] = self.ebcpy_class.mp_obj(x, n_cpu, *args)
+                else:
+                    out["F"] = np.array([self.ebcpy_class.obj(xk=_x, *args) for _x in x])
+
+        try:
+            if self.bounds is None:
+                raise ValueError("For pymoo, you need to specify "
+                                 "boundaries. Currently, no bounds are specified.")
+
+            termination = default_kwargs.pop("termination")
+            if termination is None:
+                termination = ("n_gen", default_kwargs.pop("n_gen"))
+            seed = default_kwargs.pop("seed")
+            verbose = default_kwargs.pop("verbose")
+            save_history = default_kwargs.pop("save_history")
+            copy_algorithm = default_kwargs.pop("copy_algorithm")
+            copy_termination = default_kwargs.pop("copy_termination")
+
+            # Init algorithm
+            if method.lower() == "ga":
+                from pymoo.algorithms.soo.nonconvex.ga import GA
+                # GA:
+                pop_size = kwargs["pop_size"]
+                sampling = get_sampling(name=kwargs["sampling"])
+                selection = get_selection(name=kwargs["selection"])
+                crossover = get_crossover(name=kwargs["crossover"])
+                mutation = get_mutation(name=kwargs["mutation"])
+                eliminate_duplicates = kwargs["eliminate_duplicates"]
+                n_offsprings = kwargs["n_offsprings"]
+                algorithm = GA(pop_size=pop_size,
+                               sampling=sampling,
+                               selection=selection,
+                               crossover=crossover,
+                               mutation=mutation,
+                               eliminate_duplicates=eliminate_duplicates,
+                               n_offsprings=n_offsprings
+                               )
+            else:
+                default_kwargs.update(kwargs)
+                algorithm = get_algorithm(name=method.lower(),
+                                          **default_kwargs)
+
+            res = minimize(
+                problem=EBCPYProblem(ebcpy_class=self),
+                algorithm=algorithm,
+                termination=termination,
+                seed=seed,
+                verbose=verbose,
+                display=None,
+                callback=None,
+                save_history=save_history,
+                copy_algorithm=copy_algorithm,
+                copy_termination=copy_termination,
+            )
+            res_tuple = namedtuple("res_tuple", "x fun")
+            res = res_tuple(x=res.X, fun=res.F[0])
+            return res
+        except (KeyboardInterrupt, Exception) as error:
+            # pylint: disable=inconsistent-return-statements
+            self._handle_error(error)
+
+    def _dlib_obj(self, *args):
+        """
+        This function is needed as the signature for the dlib-obj
+        is different than the standard signature. dlib will parse a number of
+        parameters
+        """
+        return self.obj(np.array(args))
+
+    def _handle_error(self, error):
+        """
+        Function to handle the case when an optimization step fails (e.g. simulation-fail).
+        The parameter set which caused the failure and the best iterate until this point
+        are of interest for the user in such case.
+        :param error:
+            Any Exception that may occur
+        """
+        self.logger.error(f"Parameter set which caused the failure: {self._current_iterate}")
+        self.logger.error("Current best objective and parameter set:")
+        self.logger.error("\n".join([f"{key}: {value}"
+                                     for key, value in self._current_best_iterate.items()]))
+        raise error
+
+    @staticmethod
+    def get_default_config(framework: str) -> dict:
+        """
+        Return the default config or kwargs for the
+        given framework.
+
+        The default values are extracted of the corresponding
+        framework directly.
+        """
+        if framework.lower() == "scipy_minimize":
+            return {"tol": None,
+                    "options": None,
+                    "constraints": None,
+                    "jac": None,
+                    "hess": None,
+                    "hessp": None}
+        if framework.lower() == "dlib_minimize":
+            return {"num_function_calls": int(1e9),
+                    "solver_epsilon": 0}
+        if framework.lower() == "scipy_differential_evolution":
+            return {"maxiter": 1000,
+                    "popsize": 15,
+                    "tol": 0.01,
+                    "mutation": (0.5, 1),
+                    "recombination": 0.7,
+                    "seed": None,
+                    "polish": True,
+                    "init": 'latinhypercube',
+                    "atol": 0
+                    }
+        if framework.lower() == "pymoo":
+            return {"n_gen": 1000,
+                    "termination": None,
+                    "seed": 1,
+                    "verbose": False,
+                    "display": None,
+                    "callback": None,
+                    "save_history": False,
+                    "copy_algorithm": False,
+                    "copy_termination": False
+                    }
+        return {}
```

### Comparing `ebcpy-0.3.2/ebcpy/preprocessing.py` & `ebcpy-0.3.6/ebcpy/preprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,644 +1,664 @@
-"""
-This general overview may help you find the function you need:
-
-- Remove duplicate rows by averaging the values
-  (``build_average_on_duplicate_rows``)
-- Convert any integer or float index into a datetime index
-  (``convert_index_to_datetime_index``)
-- Resample a given time-series on a given frequency
-  (``clean_and_space_equally_time_series``)
-- Apply a low-pass-filter (``low_pass_filter``)
-- Apply a moving average to flatten disturbances
-  in your measured data (``moving_average``)
-- Convert e.g. an electrical power signal into a binary
-  control signal (on-off) based on a threshold (``create_on_off_signal``)
-- Find the number of lines without any values in it (``number_lines_totally_na``)
-- Split a data-set into training and test set according to
-  cross-validation (``cross_validation``)
-
-All functions in the pre-processing module should have a doctest. We refer to the example
-in this doctest for a better understanding of the functions. If you don't understand
-the behaviour of a function or the meaning, please raise an issue.
-"""
-import warnings
-import logging
-from datetime import datetime
-from scipy import signal
-from sklearn import model_selection
-from pandas.tseries.frequencies import to_offset
-import numpy as np
-import pandas as pd
-import scipy.stats as st
-from ebcpy import data_types
-
-logger = logging.getLogger(__name__)
-
-
-def build_average_on_duplicate_rows(df):
-    """
-    If the dataframe has duplicate-indexes, the average
-    value of all those indexes is calculated and given to
-    the first occurrence of this duplicate index. Therefore,
-    any dataFrame should be already sorted before calling this
-    function.
-
-    :param pd.DataFame df:
-        DataFrame with the data to process
-    :return: pd.DataFame
-        The processed DataFame
-
-    Example:
-
-    >>> df = pd.DataFrame({"idx": np.ones(5), "val": np.arange(5)}).set_index("idx")
-    >>> df = convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1))
-    >>> print(df)
-                         val
-    idx
-    2007-01-01 00:00:01    0
-    2007-01-01 00:00:01    1
-    2007-01-01 00:00:01    2
-    2007-01-01 00:00:01    3
-    2007-01-01 00:00:01    4
-    >>> print(build_average_on_duplicate_rows(df))
-                         val
-    idx
-    2007-01-01 00:00:01  2.0
-    """
-    # Find entries that are exactly the same timestamp
-    double_ind = df.index[df.index.duplicated()].unique()
-    # Calculate the mean value
-    mean_values = []
-    for item in double_ind:
-        mean_values.append(df.loc[item].values.mean(axis=0))
-    # Delete duplicate indices
-    df_dropped = df[~df.index.duplicated(keep='first')].copy()
-
-    # Set mean values in rows that were duplicates before
-    for idx, values in zip(double_ind, mean_values):
-        df_dropped.loc[idx] = values
-
-    return df_dropped
-
-
-def convert_index_to_datetime_index(df, unit_of_index="s", origin=datetime.now()):
-    """
-    Converts the index of the given DataFrame to a
-    pandas.core.indexes.datetimes.DatetimeIndex.
-
-    :param pd.DataFrame df:
-        dataframe with index not being a DateTime.
-        Only numeric indexes are supported. Every integer
-        is interpreted with the given unit, standard form
-        is in seocnds.
-    :param str unit_of_index: default 's'
-        The unit of the given index. Used to convert to
-        total_seconds later on.
-    :param datetime.datetime origin:
-        The reference datetime object for the first index.
-        Default is the current system time.
-    :return: df
-        DataFrame with correct index for usage in this
-        framework.
-
-    Example:
-
-    >>> import pandas as pd
-    >>> df = pd.DataFrame(np.ones([3, 4]), columns=list('ABCD'))
-    >>> print(df)
-         A    B    C    D
-    0  1.0  1.0  1.0  1.0
-    1  1.0  1.0  1.0  1.0
-    2  1.0  1.0  1.0  1.0
-    >>> print(convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1)))
-                           A    B    C    D
-    2007-01-01 00:00:00  1.0  1.0  1.0  1.0
-    2007-01-01 00:00:01  1.0  1.0  1.0  1.0
-    2007-01-01 00:00:02  1.0  1.0  1.0  1.0
-
-    """
-    # Check for unit of given index. Maybe one uses hour-based data.
-    _unit_conversion_to_seconds = {"ms": 1e-3,
-                                   "s": 1,
-                                   "min": 1/60,
-                                   "h": 1/3600,
-                                   "d": 1/86400}
-    if unit_of_index not in _unit_conversion_to_seconds:
-        raise ValueError("Given unit_of_index is not supported.")
-    _unit_factor_to_seconds = _unit_conversion_to_seconds.get(unit_of_index)
-
-    #Convert
-    old_index = df.index.copy()
-    # Check if already converted:
-    if isinstance(old_index, pd.DatetimeIndex):
-        return df
-    # Convert strings to numeric values.
-    old_index = pd.to_numeric(old_index)
-    # Convert to seconds.
-    old_index *= _unit_factor_to_seconds
-    # Alter the index
-    df.index = pd.to_datetime(old_index, unit="s", origin=origin)
-
-    return df
-
-
-def convert_datetime_index_to_float_index(df, offset=0):
-    """
-    Convert a datetime-based index to FloatIndex (in seconds).
-    Seconds are used as a standard unit as simulation software
-    outputs data in seconds (e.g. Modelica)
-
-    :param pd.DataFrame df:
-        DataFrame to be converted to FloatIndex
-    :param float offset:
-        Offset in seconds
-    :return: pd.DataFrame df:
-        DataFrame with correct index
-
-    Example:
-
-    >>> import pandas as pd
-    >>> df = pd.DataFrame(np.ones([3, 4]), columns=list('ABCD'))
-    >>> print(convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1)))
-                           A    B    C    D
-    2007-01-01 00:00:00  1.0  1.0  1.0  1.0
-    2007-01-01 00:00:01  1.0  1.0  1.0  1.0
-    2007-01-01 00:00:02  1.0  1.0  1.0  1.0
-    >>> print(convert_datetime_index_to_float_index(df))
-           A    B    C    D
-    0.0  1.0  1.0  1.0  1.0
-    1.0  1.0  1.0  1.0  1.0
-    2.0  1.0  1.0  1.0  1.0
-    """
-    # Check correct input
-    if not isinstance(df.index, pd.DatetimeIndex):
-        raise IndexError("Given DataFrame has no DatetimeIndex, conversion not possible")
-
-    new_index = pd.to_timedelta(df.index - df.index[0]).total_seconds()
-    df.index = np.round(new_index, 4) + offset
-    return df
-
-
-def time_based_weighted_mean(df):
-    """
-    Creates the weighted mean according to time index that does not need to be equidistant.
-    Further info:
-    https://stackoverflow.com/questions/26343252/create-a-weighted-mean-for-a-irregular-timeseries-in-pandas
-
-    :param pd.DataFrame df:
-        A pandas DataFrame with DatetimeIndex.
-    :return np.array:
-        A numpy array containing weighted means of all columns
-
-    Example:
-
-    >>> from datetime import datetime
-    >>> import numpy as np
-    >>> import pandas as pd
-    >>> time_vec = [datetime(2007,1,1,0,0),
-    >>>             datetime(2007,1,1,0,0),
-    >>>             datetime(2007,1,1,0,5),
-    >>>             datetime(2007,1,1,0,7),
-    >>>             datetime(2007,1,1,0,10)]
-    >>> df = pd.DataFrame({'A': [1,2,4,3,6], 'B': [11,12,14,13,16]}, index=time_vec)
-    >>> print(time_based_weighted_mean(df=df))
-    [  3.55  13.55]
-    """
-
-    if not isinstance(df.index, pd.DatetimeIndex):
-        raise IndexError(f"df.index must be DatetimeIndex, but it is {type(df.index)}.")
-
-    time_delta = [(x-y).total_seconds() for x, y in zip(df.index[1:], df.index[:-1])]
-    weights = [x+y for x, y in zip([0] + time_delta, time_delta + [0])]
-    # Create empty numpy array
-    res = np.empty(len(df.columns))
-    res[:] = np.nan
-    for i, col_name in enumerate(df.columns):
-        res[i] = np.average(df[col_name], weights=weights)
-    return res
-
-
-def clean_and_space_equally_time_series(df, desired_freq, confidence_warning=0.95):
-    """
-    Function for cleaning of the given dataFrame and interpolating
-    based on the the given desired frequency. Linear interpolation
-    is used.
-
-    :param pd.DataFrame df:
-        Unclean DataFrame. Needs to have a pd.DateTimeIndex
-    :param str desired_freq:
-        Frequency to determine number of elements in processed dataframe.
-        Options are for example:
-        - s: second-based
-        - 5s: Every 5 seconds
-        - 6min: Every 6 minutes
-        This also works for h, d, m, y, ms etc.
-    :param float confidence_warning:
-        Value to check the confidence interval of input data without
-        a defined frequency. If the desired frequency is outside of
-        the resulting confidence interval, a warning is issued.
-    :return: pd.DataFrame
-        Cleaned and equally spaced data-frame
-
-    Example:
-    **Note:** The example is for random data. Try out different sampling
-    frequencys. You will be warned if the samping rate is to high or to low.
-
-    >>> df = pd.DataFrame(np.random.randint(0,100,size=(100, 4)),
-    >>>                   columns=list('ABCD')).set_index("A").sort_index()
-    >>> df = convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1))
-    >>> clean_and_space_equally_time_series(df, "30s")
-    >>> import matplotlib.pyplot as plt
-    >>> plt.plot(df["B"], label="Raw data")
-    >>> df = clean_and_space_equally_time_series(df.copy(), "1500ms")
-    >>> plt.plot(df["B"], label="Clead and spaced equally")
-    >>> plt.legend()
-    >>> plt.show()
-
-    .. versionchanged:: 0.1.7
-    """
-    # Convert indexes to datetime_index:
-    if not isinstance(df.index, pd.DatetimeIndex):
-        if isinstance(df, data_types.TimeSeriesData):
-            raise TypeError("DataFrame needs a DateTimeIndex for executing this function. "
-                            "Call to_datetime_index() to convert any index to "
-                            "a DateTimeIndex")
-        # Else
-        raise TypeError("DataFrame needs a DateTimeIndex for executing this function. "
-                        "Call convert_index_to_datetime_index() to convert any index to "
-                        "a DateTimeIndex")
-    #%% Check DataFrame for NANs
-    # Create a pandas Series with number of invalid values for each column of df
-    series_with_na = df.isnull().sum()
-    for name in series_with_na.index:
-        if series_with_na.loc[name] > 0:
-            # Print only columns with invalid values
-            logger.info("%s has following number of invalid "
-                        "values\n %s", name, series_with_na.loc[name])
-    # Drop all rows where at least one NA exists
-    df = df.dropna(how='any')
-
-    # Check if DataFrame still has non-numeric-values:
-    if not all(df.apply(lambda s: pd.to_numeric(s, errors='coerce').notnull().all())):
-        raise ValueError("Given DataFrame contains non-numeric values.")
-
-    # Merge duplicate rows using mean.
-    df = build_average_on_duplicate_rows(df)
-
-    # Make user warning for two cases: Upsampling and data input without a freq:
-    # Check if the frequency differs
-    old_freq = df.index.freq
-    if old_freq is None:
-        # Construct a frequency by converting it first to int, then to timedelta back again:
-        _artificial_freq = df.index.to_series().diff().dropna().values.astype(np.int64)
-        cfd_int = st.t.interval(confidence_warning,
-                                len(_artificial_freq)-1,
-                                loc=np.mean(_artificial_freq),
-                                scale=st.sem(_artificial_freq))
-        # Convert back to timedelta
-        cfd_int = pd.to_timedelta(cfd_int)
-        _td_freq = pd.to_timedelta(desired_freq)
-        if (_td_freq < cfd_int[0]) or (_td_freq > cfd_int[1]):
-            _ns_to_s = 1e9
-            in_seconds = np.array(cfd_int.values.tolist()) / _ns_to_s  # From nanoseconds
-            warnings.warn(f"Input data has no frequency, but the desired frequency "
-                          f"{_td_freq.value / _ns_to_s} seconds is outside the given "
-                          f"confidence interval {in_seconds} (in seconds). "
-                          "Carefully check the result to see if you "
-                          "introduced errors to the data.")
-
-    #%% Re-sampling to new frequency with linear interpolation
-    # Create new equally spaced DatetimeIndex. Last entry is always < df.index[-1]
-    time_index = pd.date_range(start=df.index[0], end=df.index[-1], freq=desired_freq)
-
-    # Check if the user is trying to upsample the data:
-    if old_freq:
-        if time_index.freq > old_freq:
-            warnings.warn("You are upsampling your data. This may be dangerous. "
-                          "Carefully check the result to see if you introduced errors to the data.")
-
-    # Create an empty data frame
-    # If multi-columns is used, first get the old index and make it empty:
-    multi_cols = df.columns
-    if isinstance(multi_cols, pd.MultiIndex):
-        empty_multi_cols = pd.MultiIndex.from_product([[] for _ in range(multi_cols.nlevels)],
-                                                      names=multi_cols.names)
-        df_time_temp = pd.DataFrame(index=time_index, columns=empty_multi_cols)
-    else:
-        df_time_temp = pd.DataFrame(index=time_index)
-
-    # Insert temporary time_index into df. fill_value = 0 can only be used,
-    # since all NaNs should be eliminated prior
-    df = df.radd(df_time_temp, axis='index', fill_value=0)
-    del df_time_temp
-
-    # Interpolate linearly according to time index
-    df.interpolate(method='time', axis=0, inplace=True)
-    # Determine Timedelta between current first index entry
-    # in df and the first index entry that would be created
-    # when applying df.resample() without loffset
-    delta_time = df.index[0] - df.resample(rule=desired_freq).first().first(desired_freq).index[0]
-    # Resample to equally spaced index.
-    # All fields should already have a value. Thus NaNs and maybe +/- infs
-    # should have been filtered beforehand.
-
-    # Check if given dataframe was a TimeSeriesData object and of so, convert it as such
-    if isinstance(df, data_types.TimeSeriesData):
-        df = df.resample(rule=desired_freq).first()
-        df.index = df.index + to_offset(delta_time)
-        df = data_types.TimeSeriesData(df)
-    else:
-        df = df.resample(rule=desired_freq).first()
-        df.index = df.index + to_offset(delta_time)
-    del delta_time
-
-    return df
-
-
-def low_pass_filter(data, crit_freq, filter_order):
-    """
-    Create a low pass filter with given order and frequency.
-
-    :param numpy.ndarray data:
-        For dataframe e.g. df['a_col_name'].values
-    :param float crit_freq:
-        The critical frequency or frequencies.
-    :param int filter_order:
-        The order of the filter
-    :return: numpy.ndarray
-
-    Example:
-
-    >>> import numpy as np
-    >>> import matplotlib.pyplot as plt
-    >>> rand_series = np.random.rand(100)
-    >>> plt.plot(rand_series, label="reference")
-    >>> plt.plot(low_pass_filter(rand_series, 0.2, 2), label="filtered")
-    >>> plt.legend()
-    >>> plt.show()
-
-    """
-    if len(data.shape) > 1:  # Check if given data has multiple dimensions
-        if data.shape[1] == 1:
-            data = data[:, 0]  # Resize to 1D-Array
-        else:
-            raise ValueError("Given data has multiple dimensions. "
-                             "Only one-dimensional arrays are supported in this function.")
-    _filter_order = int(filter_order)
-    numerator, denominator = signal.butter(N=_filter_order, Wn=crit_freq,
-                                           btype='low', analog=False, output='ba')
-    output = signal.filtfilt(numerator, denominator, data)
-    return output
-
-
-def moving_average(data, window):
-    """
-    Creates a pandas Series as moving average of the input series.
-
-    :param pd.Series values:
-        For dataframe e.g. df['a_col_name'].values
-    :param int window:
-        sample rate of input
-    :return: numpy.array
-        shape has (###,). First and last points of input Series are extrapolated as constant
-        values (hold first and last point).
-
-    Example:
-
-    >>> import numpy as np
-    >>> import matplotlib.pyplot as plt
-    >>> series = np.sin(np.linspace(-30, 30, 1000))
-    >>> plt.plot(series, label="reference")
-    >>> plt.plot(moving_average(series, 10), label="window=10")
-    >>> plt.plot(moving_average(series, 50), label="window=50")
-    >>> plt.plot(moving_average(series, 100), label="window=100")
-    >>> plt.legend()
-    >>> plt.show()
-
-    """
-    if len(data.shape) > 1: # Check if given data has multiple dimensions
-        if data.shape[1] == 1:
-            data = data[:, 0]  # Resize to 1D-Array
-        else:
-            raise ValueError("Given data has multiple dimensions. "
-                             "Only one-dimensional arrays are supported in this function.")
-    window = int(window)
-    weights = np.repeat(1.0, window) / window
-    sma = np.convolve(data, weights, 'valid')
-    # Create array with first entries and window/2 elements
-    fill_start = np.full((int(np.floor(window/2)), 1), sma[0])
-    # Same with last value of -data-
-    fill_end = np.full((int(np.ceil(window/2)) - 1, 1), sma[-1])
-    # Stack the arrays
-    sma = np.concatenate((fill_start[:, 0], sma, fill_end[:, 0]), axis=0)
-    return sma
-
-
-def create_on_off_signal(df, col_names, threshold, col_names_new,
-                         tags="raw", new_tag="converted_signal"):
-    """
-    Create on and off signals based on the given threshold for all column names.
-
-    :param pd.DataFame df:
-        DataFrame with the data to process
-    :param list col_names:
-        Column names of variables to convert to signals
-    :param float,list threshold:
-        Threshold for all column-names (single float) or
-        a list with specific thresholds for specific columns.
-    :param list col_names_new:
-        New name for the signal-column
-    :param str,list tags:
-        If a 2-Level DataFrame for TimeSeriesData is used, one has to
-        specify the tag of the variables. Default value is to use the "raw"
-        tag set in the TimeSeriesClass. However one can specify a list
-        (Different tag for each variable), or on can pass a string
-        (same tags for all given variables)
-    :param str new_tag:
-        The tag the newly created variable will hold. This can be used to
-        indicate where the signal was converted from.
-    :return: pd.DataFrame
-        Now with the created signals.
-
-    Example:
-
-    >>> import matplotlib.pyplot as plt
-    >>> import numpy as np
-    >>> df = pd.DataFrame({"P_el": np.sin(np.linspace(-20, 20, 10000))*100})
-    >>> df = create_on_off_signal(df, col_names=["P_el"],
-    >>>                           threshold=25, col_names_new=["Device On"])
-    >>> plt.plot(df)
-    >>> plt.show()
-    """
-    if len(col_names) != len(col_names_new):
-        raise IndexError(f"Given lists differ in length. col_names: {len(col_names)}, "
-                         f"col_names_new: {len(col_names_new)}")
-    if isinstance(threshold, list):
-        if len(col_names) != len(threshold):
-            raise IndexError(f"Given lists differ in length. col_names: {len(col_names)}, "
-                             f"threshold: {len(threshold)}")
-    else:
-        threshold = [threshold for _ in enumerate(col_names)]
-    # Do on_off signal creation for all desired columns
-    if isinstance(df.columns, pd.MultiIndex):
-        # Convert given tags to a list
-        if isinstance(tags, str):
-            tags = [tags for _ in enumerate(col_names)]
-
-        for i, _ in enumerate(col_names):
-            # Create zero-array
-            df.loc[:, (col_names_new[i], new_tag)] = 0.0
-            # Change all values to 1.0 according to threshold
-            df.loc[df[col_names[i], tags[i]] >= threshold[i], (col_names_new[i], new_tag)] = 1.0
-    else:
-        for i, _ in enumerate(col_names):
-            # Create zero-array
-            df.loc[:, col_names_new[i]] = 0.0
-            # Change all values to 1.0 according to threshold
-            df.loc[df[col_names[i]] >= threshold[i], col_names_new[i]] = 1.0
-    return df
-
-
-def number_lines_totally_na(df):
-    """
-    Returns the number of rows in the given dataframe
-    that are filled with NaN-values.
-
-    :param pd.DataFrame df:
-        Given dataframe to process
-    :return: int
-        Number of NaN-Rows.
-
-    Example:
-
-    >>> import numpy as np
-    >>> import pandas as pd
-    >>> dim = np.random.randint(100) + 10
-    >>> nan_col = [np.NaN for i in range(dim)]
-    >>> col = [i for i in range(dim)]
-    >>> df_nan = pd.DataFrame({"col_1":nan_col, "col_2":nan_col})
-    >>> df_normal = pd.DataFrame({"col_1":nan_col, "col_2":col})
-    >>> print(number_lines_totally_na(df_nan)-dim)
-    0
-    >>> print(number_lines_totally_na(df_normal))
-    0
-    """
-    if not isinstance(df, pd.DataFrame):
-        raise TypeError('Input must be a pandas data frame')
-    counter = 0
-    for _, row in df.iterrows():
-        # Check if the whole row is filled with NaNs.
-        if all(row.isnull()):
-            counter += 1
-    return counter
-
-
-def z_score(x, limit=3):
-    """
-    Calculate the z-score using the mea
-    and standard deviation of the given data.
-
-    :param np.array x:
-        For dataframe e.g. df['a_col_name'].values
-    :param float limit: default 3
-        Lower limit for required z-score
-    :return: np.array iqr:
-        modified z score
-
-    Example:
-
-    >>> import numpy as np
-    >>> normal_dis = np.random.normal(0, 1, 1000)
-    >>> res = z_score(normal_dis, limit=2)
-    >>> values = normal_dis[res]
-
-    """
-    mean = np.mean(x)
-    standard_deviation = np.std(x)
-    z_score_value = (x-mean)/standard_deviation
-    return np.where(np.abs(z_score_value) > limit)[0]
-
-
-def modified_z_score(x, limit=3.5):
-    """
-    Calculate the modified z-score using the median
-    and median average deviation of the given data.
-
-    :param np.array x:
-        For dataframe e.g. df['a_col_name'].values
-    :param float limit: default 3.5
-        Lower limit for required z-score
-    :return: np.array iqr:
-        modified z score
-
-    Example:
-
-    >>> import numpy as np
-    >>> normal_dis = np.random.normal(0, 1, 1000)
-    >>> res = modified_z_score(normal_dis, limit=2)
-    >>> values = normal_dis[res]
-
-    """
-    median = np.median(x)
-    median_average_deviation = np.median(np.abs(x-median))
-    z_score_mod = 0.6745*(x-median)/median_average_deviation
-    return np.where(np.abs(z_score_mod) > limit)[0]
-
-
-def interquartile_range(x):
-    """
-    Calculate interquartile range of given array.
-    Returns the indices of values outside of the interquartile range.
-
-    :param np.array x:
-        For dataframe e.g. df['a_col_name'].values
-    :return: np.array iqr:
-        Array matching the interquartile-range
-
-    Example:
-
-    >>> import numpy as np
-    >>> normal_dis = np.random.normal(0, 1, 1000)
-    >>> res = interquartile_range(normal_dis)
-    >>> values = normal_dis[res]
-
-    """
-    quartile_1, quartile_3 = np.percentile(x, [25, 75])
-    iqr = quartile_3 - quartile_1
-    lower = quartile_1 - (iqr * 1.5)
-    upper = quartile_3 + (iqr * 1.5)
-    return np.where((x > upper) | (x < lower))[0]
-
-
-def cross_validation(x, y, test_size=0.3):
-    """
-    Split data set randomly with test_size
-    (if test_size = 0.30 --> 70 % are training data).
-    You can use this function for segmentation tasks.
-    Time-series-data may not be splitted with this function
-    as the results are not coherent (time-wise).
-
-    :param x:
-        Indexables with same length / shape[0] as y.
-        Allowed inputs are lists, numpy arrays, scipy-sparse
-        matrices or pandas dataframes.
-    :param list,np.ndarray,pd.DataFrame y:
-        Indexables with same length / shape[0] as x.
-        Allowed inputs are lists, numpy arrays, scipy-sparse
-        matrices or pandas dataframes.
-    :param float test_size:
-        Value between 0 and 1 specifying what percentage of the data
-        will be used for testing.
-    :return: list
-        Split data into 4 objects. The order is:
-        x_train, x_test, y_train, y_test
-
-    Example:
-
-    >>> import numpy as np
-    >>> x = np.random.rand(100)
-    >>> y = np.random.rand(100)
-    >>> ret = cross_validation(x, y)
-    >>> len(ret)
-    4
-    """
-    return model_selection.train_test_split(x, y, test_size=test_size)
+"""
+This general overview may help you find the function you need:
+
+- Remove duplicate rows by averaging the values
+  (``build_average_on_duplicate_rows``)
+- Convert any integer or float index into a datetime index
+  (``convert_index_to_datetime_index``)
+- Resample a given time-series on a given frequency
+  (``clean_and_space_equally_time_series``)
+- Apply a low-pass-filter (``low_pass_filter``)
+- Apply a moving average to flatten disturbances
+  in your measured data (``moving_average``)
+- Convert e.g. an electrical power signal into a binary
+  control signal (on-off) based on a threshold (``create_on_off_signal``)
+- Find the number of lines without any values in it (``number_lines_totally_na``)
+- Split a data-set into training and test set according to
+  cross-validation (``cross_validation``)
+
+All functions in the pre-processing module should have a doctest. We refer to the example
+in this doctest for a better understanding of the functions. If you don't understand
+the behaviour of a function or the meaning, please raise an issue.
+"""
+import warnings
+import logging
+from datetime import datetime
+from scipy import signal
+from sklearn import model_selection
+from pandas.tseries.frequencies import to_offset
+import numpy as np
+import pandas as pd
+import scipy.stats as st
+from ebcpy import data_types
+
+logger = logging.getLogger(__name__)
+
+
+def build_average_on_duplicate_rows(df):
+    """
+    If the dataframe has duplicate-indexes, the average
+    value of all those indexes is calculated and given to
+    the first occurrence of this duplicate index. Therefore,
+    any dataFrame should be already sorted before calling this
+    function.
+
+    :param pd.DataFame df:
+        DataFrame with the data to process
+    :return: pd.DataFame
+        The processed DataFame
+
+    Example:
+
+    >>> df = pd.DataFrame({"idx": np.ones(5), "val": np.arange(5)}).set_index("idx")
+    >>> df = convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1))
+    >>> print(df)
+                         val
+    idx
+    2007-01-01 00:00:01    0
+    2007-01-01 00:00:01    1
+    2007-01-01 00:00:01    2
+    2007-01-01 00:00:01    3
+    2007-01-01 00:00:01    4
+    >>> print(build_average_on_duplicate_rows(df))
+                         val
+    idx
+    2007-01-01 00:00:01  2.0
+    """
+    # Find entries that are exactly the same timestamp
+    double_ind = df.index[df.index.duplicated()].unique()
+    # Calculate the mean value
+    mean_values = []
+    for item in double_ind:
+        mean_values.append(df.loc[item].values.mean(axis=0))
+    # Delete duplicate indices
+    df_dropped = df[~df.index.duplicated(keep='first')].copy()
+
+    # Set mean values in rows that were duplicates before
+    for idx, values in zip(double_ind, mean_values):
+        df_dropped.loc[idx] = values
+
+    return df_dropped
+
+
+def convert_index_to_datetime_index(df, unit_of_index="s", origin=datetime.now()):
+    """
+    Converts the index of the given DataFrame to a
+    pandas.core.indexes.datetimes.DatetimeIndex.
+
+    :param pd.DataFrame df:
+        dataframe with index not being a DateTime.
+        Only numeric indexes are supported. Every integer
+        is interpreted with the given unit, standard form
+        is in seocnds.
+    :param str unit_of_index: default 's'
+        The unit of the given index. Used to convert to
+        total_seconds later on.
+    :param datetime.datetime origin:
+        The reference datetime object for the first index.
+        Default is the current system time.
+    :return: df
+        DataFrame with correct index for usage in this
+        framework.
+
+    Example:
+
+    >>> import pandas as pd
+    >>> df = pd.DataFrame(np.ones([3, 4]), columns=list('ABCD'))
+    >>> print(df)
+         A    B    C    D
+    0  1.0  1.0  1.0  1.0
+    1  1.0  1.0  1.0  1.0
+    2  1.0  1.0  1.0  1.0
+    >>> print(convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1)))
+                           A    B    C    D
+    2007-01-01 00:00:00  1.0  1.0  1.0  1.0
+    2007-01-01 00:00:01  1.0  1.0  1.0  1.0
+    2007-01-01 00:00:02  1.0  1.0  1.0  1.0
+
+    """
+    # Check for unit of given index. Maybe one uses hour-based data.
+    _unit_conversion_to_seconds = {"ms": 1e-3,
+                                   "s": 1,
+                                   "min": 1/60,
+                                   "h": 1/3600,
+                                   "d": 1/86400}
+    if unit_of_index not in _unit_conversion_to_seconds:
+        raise ValueError("Given unit_of_index is not supported.")
+    _unit_factor_to_seconds = _unit_conversion_to_seconds.get(unit_of_index)
+
+    #Convert
+    old_index = df.index.copy()
+    # Check if already converted:
+    if isinstance(old_index, pd.DatetimeIndex):
+        return df
+    # Convert strings to numeric values.
+    old_index = pd.to_numeric(old_index)
+    # Convert to seconds.
+    old_index /= _unit_factor_to_seconds
+    # Alter the index
+    df.index = pd.to_datetime(old_index, unit="s", origin=origin)
+
+    return df
+
+
+def convert_datetime_index_to_float_index(df, offset=0):
+    """
+    Convert a datetime-based index to FloatIndex (in seconds).
+    Seconds are used as a standard unit as simulation software
+    outputs data in seconds (e.g. Modelica)
+
+    :param pd.DataFrame df:
+        DataFrame to be converted to FloatIndex
+    :param float offset:
+        Offset in seconds
+    :return: pd.DataFrame df:
+        DataFrame with correct index
+
+    Example:
+
+    >>> import pandas as pd
+    >>> df = pd.DataFrame(np.ones([3, 4]), columns=list('ABCD'))
+    >>> print(convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1)))
+                           A    B    C    D
+    2007-01-01 00:00:00  1.0  1.0  1.0  1.0
+    2007-01-01 00:00:01  1.0  1.0  1.0  1.0
+    2007-01-01 00:00:02  1.0  1.0  1.0  1.0
+    >>> print(convert_datetime_index_to_float_index(df))
+           A    B    C    D
+    0.0  1.0  1.0  1.0  1.0
+    1.0  1.0  1.0  1.0  1.0
+    2.0  1.0  1.0  1.0  1.0
+    """
+    # Check correct input
+    if not isinstance(df.index, pd.DatetimeIndex):
+        raise IndexError("Given DataFrame has no DatetimeIndex, conversion not possible")
+
+    new_index = pd.to_timedelta(df.index - df.index[0]).total_seconds()
+    df.index = np.round(new_index, 4) + offset
+    return df
+
+
+def time_based_weighted_mean(df):
+    """
+    Creates the weighted mean according to time index that does not need to be equidistant.
+    Further info:
+    https://stackoverflow.com/questions/26343252/create-a-weighted-mean-for-a-irregular-timeseries-in-pandas
+
+    :param pd.DataFrame df:
+        A pandas DataFrame with DatetimeIndex.
+    :return np.array:
+        A numpy array containing weighted means of all columns
+
+    Example:
+
+    >>> from datetime import datetime
+    >>> import numpy as np
+    >>> import pandas as pd
+    >>> time_vec = [datetime(2007,1,1,0,0),
+    >>>             datetime(2007,1,1,0,0),
+    >>>             datetime(2007,1,1,0,5),
+    >>>             datetime(2007,1,1,0,7),
+    >>>             datetime(2007,1,1,0,10)]
+    >>> df = pd.DataFrame({'A': [1,2,4,3,6], 'B': [11,12,14,13,16]}, index=time_vec)
+    >>> print(time_based_weighted_mean(df=df))
+    [  3.55  13.55]
+    """
+
+    if not isinstance(df.index, pd.DatetimeIndex):
+        raise IndexError(f"df.index must be DatetimeIndex, but it is {type(df.index)}.")
+
+    time_delta = [(x-y).total_seconds() for x, y in zip(df.index[1:], df.index[:-1])]
+    weights = [x+y for x, y in zip([0] + time_delta, time_delta + [0])]
+    # Create empty numpy array
+    res = np.empty(len(df.columns))
+    res[:] = np.nan
+    for i, col_name in enumerate(df.columns):
+        res[i] = np.average(df[col_name], weights=weights)
+    return res
+
+
+def clean_and_space_equally_time_series(df, desired_freq, confidence_warning=0.95):
+    """
+    Function for cleaning of the given dataFrame and interpolating
+    based on the the given desired frequency. Linear interpolation
+    is used.
+
+    :param pd.DataFrame df:
+        Unclean DataFrame. Needs to have a pd.DateTimeIndex
+    :param str desired_freq:
+        Frequency to determine number of elements in processed dataframe.
+        Options are for example:
+        - s: second-based
+        - 5s: Every 5 seconds
+        - 6min: Every 6 minutes
+        This also works for h, d, m, y, ms etc.
+    :param float confidence_warning:
+        Value to check the confidence interval of input data without
+        a defined frequency. If the desired frequency is outside of
+        the resulting confidence interval, a warning is issued.
+    :return: pd.DataFrame
+        Cleaned and equally spaced data-frame
+
+    Example:
+    **Note:** The example is for random data. Try out different sampling
+    frequencys. You will be warned if the samping rate is to high or to low.
+
+    >>> df = pd.DataFrame(np.random.randint(0,100,size=(100, 4)),
+    >>>                   columns=list('ABCD')).set_index("A").sort_index()
+    >>> df = convert_index_to_datetime_index(df, origin=datetime(2007, 1, 1))
+    >>> clean_and_space_equally_time_series(df, "30s")
+    >>> import matplotlib.pyplot as plt
+    >>> plt.plot(df["B"], label="Raw data")
+    >>> df = clean_and_space_equally_time_series(df.copy(), "1500ms")
+    >>> plt.plot(df["B"], label="Clead and spaced equally")
+    >>> plt.legend()
+    >>> plt.show()
+
+    .. versionchanged:: 0.1.7
+    """
+    # Convert indexes to datetime_index:
+    if not isinstance(df.index, pd.DatetimeIndex):
+        if isinstance(df, data_types.TimeSeriesData):
+            raise TypeError("DataFrame needs a DateTimeIndex for executing this function. "
+                            "Call to_datetime_index() to convert any index to "
+                            "a DateTimeIndex")
+        # Else
+        raise TypeError("DataFrame needs a DateTimeIndex for executing this function. "
+                        "Call convert_index_to_datetime_index() to convert any index to "
+                        "a DateTimeIndex")
+    #%% Check DataFrame for NANs
+    # Create a pandas Series with number of invalid values for each column of df
+    series_with_na = df.isnull().sum()
+    for name in series_with_na.index:
+        if series_with_na.loc[name] > 0:
+            # Print only columns with invalid values
+            logger.info("%s has following number of invalid "
+                        "values\n %s", name, series_with_na.loc[name])
+    # Drop all rows where at least one NA exists
+    df = df.dropna(how='any')
+
+    # Check if DataFrame still has non-numeric-values:
+    if not all(df.apply(lambda s: pd.to_numeric(s, errors='coerce').notnull().all())):
+        raise ValueError("Given DataFrame contains non-numeric values.")
+
+    # Merge duplicate rows using mean.
+    df = build_average_on_duplicate_rows(df)
+
+    # Make user warning for two cases: Upsampling and data input without a freq:
+    # Check if the frequency differs
+    old_freq, old_freq_std = get_df_index_frequency_mean_and_std(df_index=df.index)
+    if old_freq_std > 0:
+        _ns_to_s = 1e9
+        # Construct a frequency by converting it first to int, then to timedelta back again:
+        _artificial_freq = old_freq / _ns_to_s
+        cfd_int = st.t.interval(confidence_warning,
+                                len(_artificial_freq)-1,
+                                loc=np.mean(_artificial_freq),
+                                scale=st.sem(_artificial_freq))
+        # Convert back to timedelta
+        cfd_int = pd.to_timedelta(cfd_int)
+        _td_freq = pd.to_timedelta(desired_freq)
+        if (_td_freq < cfd_int[0]) or (_td_freq > cfd_int[1]):
+            in_seconds = np.array(cfd_int.values.tolist()) / _ns_to_s  # From nanoseconds
+            warnings.warn(f"Input data has no frequency, but the desired frequency "
+                          f"{_td_freq.value / _ns_to_s} seconds is outside the given "
+                          f"confidence interval {in_seconds} (in seconds). "
+                          "Carefully check the result to see if you "
+                          "introduced errors to the data.")
+
+    #%% Re-sampling to new frequency with linear interpolation
+    # Create new equally spaced DatetimeIndex. Last entry is always < df.index[-1]
+    time_index = pd.date_range(start=df.index[0], end=df.index[-1], freq=desired_freq)
+    new_freq, _ = get_df_index_frequency_mean_and_std(df_index=time_index)
+
+    # Check if the user is trying to upsample the data:
+    if old_freq_std == 0:
+        if new_freq > old_freq:
+            warnings.warn("You are upsampling your data. This may be dangerous. "
+                          "Carefully check the result to see if you introduced errors to the data.")
+
+    # Create an empty data frame
+    # If multi-columns is used, first get the old index and make it empty:
+    multi_cols = df.columns
+    if isinstance(multi_cols, pd.MultiIndex):
+        empty_multi_cols = pd.MultiIndex.from_product([[] for _ in range(multi_cols.nlevels)],
+                                                      names=multi_cols.names)
+        df_time_temp = pd.DataFrame(index=time_index, columns=empty_multi_cols)
+    else:
+        df_time_temp = pd.DataFrame(index=time_index)
+
+    # Insert temporary time_index into df. fill_value = 0 can only be used,
+    # since all NaNs should be eliminated prior
+    df = df.radd(df_time_temp, axis='index', fill_value=0)
+    del df_time_temp
+
+    # Interpolate linearly according to time index
+    df.interpolate(method='time', axis=0, inplace=True)
+    # Determine Timedelta between current first index entry
+    # in df and the first index entry that would be created
+    # when applying df.resample() without loffset
+    delta_time = df.index[0] - df.resample(rule=desired_freq).first().first(desired_freq).index[0]
+    # Resample to equally spaced index.
+    # All fields should already have a value. Thus NaNs and maybe +/- infs
+    # should have been filtered beforehand.
+
+    # Check if given dataframe was a TimeSeriesData object and of so, convert it as such
+    if isinstance(df, data_types.TimeSeriesData):
+        df = df.resample(rule=desired_freq).first()
+        df.index = df.index + to_offset(delta_time)
+        df = data_types.TimeSeriesData(df)
+    else:
+        df = df.resample(rule=desired_freq).first()
+        df.index = df.index + to_offset(delta_time)
+    del delta_time
+
+    return df
+
+
+def low_pass_filter(data, crit_freq, filter_order):
+    """
+    Create a low pass filter with given order and frequency.
+
+    :param numpy.ndarray data:
+        For dataframe e.g. df['a_col_name'].values
+    :param float crit_freq:
+        The critical frequency or frequencies.
+    :param int filter_order:
+        The order of the filter
+    :return: numpy.ndarray
+
+    Example:
+
+    >>> import numpy as np
+    >>> import matplotlib.pyplot as plt
+    >>> rand_series = np.random.rand(100)
+    >>> plt.plot(rand_series, label="reference")
+    >>> plt.plot(low_pass_filter(rand_series, 0.2, 2), label="filtered")
+    >>> plt.legend()
+    >>> plt.show()
+
+    """
+    if len(data.shape) > 1:  # Check if given data has multiple dimensions
+        if data.shape[1] == 1:
+            data = data[:, 0]  # Resize to 1D-Array
+        else:
+            raise ValueError("Given data has multiple dimensions. "
+                             "Only one-dimensional arrays are supported in this function.")
+    _filter_order = int(filter_order)
+    numerator, denominator = signal.butter(N=_filter_order, Wn=crit_freq,
+                                           btype='low', analog=False, output='ba')
+    output = signal.filtfilt(numerator, denominator, data)
+    return output
+
+
+def moving_average(data, window):
+    """
+    Creates a pandas Series as moving average of the input series.
+
+    :param pd.Series values:
+        For dataframe e.g. df['a_col_name'].values
+    :param int window:
+        sample rate of input
+    :return: numpy.array
+        shape has (###,). First and last points of input Series are extrapolated as constant
+        values (hold first and last point).
+
+    Example:
+
+    >>> import numpy as np
+    >>> import matplotlib.pyplot as plt
+    >>> series = np.sin(np.linspace(-30, 30, 1000))
+    >>> plt.plot(series, label="reference")
+    >>> plt.plot(moving_average(series, 10), label="window=10")
+    >>> plt.plot(moving_average(series, 50), label="window=50")
+    >>> plt.plot(moving_average(series, 100), label="window=100")
+    >>> plt.legend()
+    >>> plt.show()
+
+    """
+    if len(data.shape) > 1: # Check if given data has multiple dimensions
+        if data.shape[1] == 1:
+            data = data[:, 0]  # Resize to 1D-Array
+        else:
+            raise ValueError("Given data has multiple dimensions. "
+                             "Only one-dimensional arrays are supported in this function.")
+    window = int(window)
+    weights = np.repeat(1.0, window) / window
+    sma = np.convolve(data, weights, 'valid')
+    # Create array with first entries and window/2 elements
+    fill_start = np.full((int(np.floor(window/2)), 1), sma[0])
+    # Same with last value of -data-
+    fill_end = np.full((int(np.ceil(window/2)) - 1, 1), sma[-1])
+    # Stack the arrays
+    sma = np.concatenate((fill_start[:, 0], sma, fill_end[:, 0]), axis=0)
+    return sma
+
+
+def create_on_off_signal(df, col_names, threshold, col_names_new,
+                         tags="raw", new_tag="converted_signal"):
+    """
+    Create on and off signals based on the given threshold for all column names.
+
+    :param pd.DataFame df:
+        DataFrame with the data to process
+    :param list col_names:
+        Column names of variables to convert to signals
+    :param float,list threshold:
+        Threshold for all column-names (single float) or
+        a list with specific thresholds for specific columns.
+    :param list col_names_new:
+        New name for the signal-column
+    :param str,list tags:
+        If a 2-Level DataFrame for TimeSeriesData is used, one has to
+        specify the tag of the variables. Default value is to use the "raw"
+        tag set in the TimeSeriesClass. However one can specify a list
+        (Different tag for each variable), or on can pass a string
+        (same tags for all given variables)
+    :param str new_tag:
+        The tag the newly created variable will hold. This can be used to
+        indicate where the signal was converted from.
+    :return: pd.DataFrame
+        Now with the created signals.
+
+    Example:
+
+    >>> import matplotlib.pyplot as plt
+    >>> import numpy as np
+    >>> df = pd.DataFrame({"P_el": np.sin(np.linspace(-20, 20, 10000))*100})
+    >>> df = create_on_off_signal(df, col_names=["P_el"],
+    >>>                           threshold=25, col_names_new=["Device On"])
+    >>> plt.plot(df)
+    >>> plt.show()
+    """
+    if len(col_names) != len(col_names_new):
+        raise IndexError(f"Given lists differ in length. col_names: {len(col_names)}, "
+                         f"col_names_new: {len(col_names_new)}")
+    if isinstance(threshold, list):
+        if len(col_names) != len(threshold):
+            raise IndexError(f"Given lists differ in length. col_names: {len(col_names)}, "
+                             f"threshold: {len(threshold)}")
+    else:
+        threshold = [threshold for _ in enumerate(col_names)]
+    # Do on_off signal creation for all desired columns
+    if isinstance(df.columns, pd.MultiIndex):
+        # Convert given tags to a list
+        if isinstance(tags, str):
+            tags = [tags for _ in enumerate(col_names)]
+
+        for i, _ in enumerate(col_names):
+            # Create zero-array
+            df.loc[:, (col_names_new[i], new_tag)] = 0.0
+            # Change all values to 1.0 according to threshold
+            df.loc[df[col_names[i], tags[i]] >= threshold[i], (col_names_new[i], new_tag)] = 1.0
+    else:
+        for i, _ in enumerate(col_names):
+            # Create zero-array
+            df.loc[:, col_names_new[i]] = 0.0
+            # Change all values to 1.0 according to threshold
+            df.loc[df[col_names[i]] >= threshold[i], col_names_new[i]] = 1.0
+    return df
+
+
+def number_lines_totally_na(df):
+    """
+    Returns the number of rows in the given dataframe
+    that are filled with NaN-values.
+
+    :param pd.DataFrame df:
+        Given dataframe to process
+    :return: int
+        Number of NaN-Rows.
+
+    Example:
+
+    >>> import numpy as np
+    >>> import pandas as pd
+    >>> dim = np.random.randint(100) + 10
+    >>> nan_col = [np.NaN for i in range(dim)]
+    >>> col = [i for i in range(dim)]
+    >>> df_nan = pd.DataFrame({"col_1":nan_col, "col_2":nan_col})
+    >>> df_normal = pd.DataFrame({"col_1":nan_col, "col_2":col})
+    >>> print(number_lines_totally_na(df_nan)-dim)
+    0
+    >>> print(number_lines_totally_na(df_normal))
+    0
+    """
+    if not isinstance(df, pd.DataFrame):
+        raise TypeError('Input must be a pandas data frame')
+    counter = 0
+    for _, row in df.iterrows():
+        # Check if the whole row is filled with NaNs.
+        if all(row.isnull()):
+            counter += 1
+    return counter
+
+
+def z_score(x, limit=3):
+    """
+    Calculate the z-score using the mea
+    and standard deviation of the given data.
+
+    :param np.array x:
+        For dataframe e.g. df['a_col_name'].values
+    :param float limit: default 3
+        Lower limit for required z-score
+    :return: np.array iqr:
+        modified z score
+
+    Example:
+
+    >>> import numpy as np
+    >>> normal_dis = np.random.normal(0, 1, 1000)
+    >>> res = z_score(normal_dis, limit=2)
+    >>> values = normal_dis[res]
+
+    """
+    mean = np.mean(x)
+    standard_deviation = np.std(x)
+    z_score_value = (x-mean)/standard_deviation
+    return np.where(np.abs(z_score_value) > limit)[0]
+
+
+def modified_z_score(x, limit=3.5):
+    """
+    Calculate the modified z-score using the median
+    and median average deviation of the given data.
+
+    :param np.array x:
+        For dataframe e.g. df['a_col_name'].values
+    :param float limit: default 3.5
+        Lower limit for required z-score
+    :return: np.array iqr:
+        modified z score
+
+    Example:
+
+    >>> import numpy as np
+    >>> normal_dis = np.random.normal(0, 1, 1000)
+    >>> res = modified_z_score(normal_dis, limit=2)
+    >>> values = normal_dis[res]
+
+    """
+    median = np.median(x)
+    median_average_deviation = np.median(np.abs(x-median))
+    z_score_mod = 0.6745*(x-median)/median_average_deviation
+    return np.where(np.abs(z_score_mod) > limit)[0]
+
+
+def interquartile_range(x):
+    """
+    Calculate interquartile range of given array.
+    Returns the indices of values outside of the interquartile range.
+
+    :param np.array x:
+        For dataframe e.g. df['a_col_name'].values
+    :return: np.array iqr:
+        Array matching the interquartile-range
+
+    Example:
+
+    >>> import numpy as np
+    >>> normal_dis = np.random.normal(0, 1, 1000)
+    >>> res = interquartile_range(normal_dis)
+    >>> values = normal_dis[res]
+
+    """
+    quartile_1, quartile_3 = np.percentile(x, [25, 75])
+    iqr = quartile_3 - quartile_1
+    lower = quartile_1 - (iqr * 1.5)
+    upper = quartile_3 + (iqr * 1.5)
+    return np.where((x > upper) | (x < lower))[0]
+
+
+def cross_validation(x, y, test_size=0.3):
+    """
+    Split data set randomly with test_size
+    (if test_size = 0.30 --> 70 % are training data).
+    You can use this function for segmentation tasks.
+    Time-series-data may not be splitted with this function
+    as the results are not coherent (time-wise).
+
+    :param x:
+        Indexables with same length / shape[0] as y.
+        Allowed inputs are lists, numpy arrays, scipy-sparse
+        matrices or pandas dataframes.
+    :param list,np.ndarray,pd.DataFrame y:
+        Indexables with same length / shape[0] as x.
+        Allowed inputs are lists, numpy arrays, scipy-sparse
+        matrices or pandas dataframes.
+    :param float test_size:
+        Value between 0 and 1 specifying what percentage of the data
+        will be used for testing.
+    :return: list
+        Split data into 4 objects. The order is:
+        x_train, x_test, y_train, y_test
+
+    Example:
+
+    >>> import numpy as np
+    >>> x = np.random.rand(100)
+    >>> y = np.random.rand(100)
+    >>> ret = cross_validation(x, y)
+    >>> len(ret)
+    4
+    """
+    return model_selection.train_test_split(x, y, test_size=test_size)
+
+
+def get_df_index_frequency_mean_and_std(df_index: pd.Index):
+    """
+    Function to get the mean and std of the index-frequency.
+    If the index is a DatetimeIndex, the seconds are converted from nanoseconds
+    to seconds.
+    Else, seconds are assumed as values.
+
+    :returns:
+        float: Mean value
+        float: Standard deviation
+    """
+
+    if isinstance(df_index, pd.DatetimeIndex):
+        index_in_s = df_index.to_series().diff().dropna().values.astype(np.int64) * 1e-9
+    else:
+        index_in_s = df_index.to_series().diff().dropna().values.astype(np.int64)
+    return np.mean(index_in_s), np.std(index_in_s)
```

### Comparing `ebcpy-0.3.2/ebcpy/simulationapi/dymola_api.py` & `ebcpy-0.3.6/ebcpy/simulationapi/dymola_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1157 +1,1168 @@
-"""Module containing the DymolaAPI used for simulation
-of Modelica-Models."""
-
-import sys
-import os
-import shutil
-import pathlib
-import warnings
-import atexit
-import json
-from typing import Union, List
-from pydantic import Field
-import pandas as pd
-from ebcpy import TimeSeriesData
-from ebcpy.modelica import manipulate_ds
-from ebcpy.simulationapi import SimulationSetup, SimulationAPI, \
-    SimulationSetupClass, Variable
-from ebcpy.utils.conversion import convert_tsd_to_modelica_txt
-
-
-class DymolaSimulationSetup(SimulationSetup):
-    """
-    Adds ``tolerance`` to the list of possible
-    setup fields.
-    """
-    tolerance: float = Field(
-        title="tolerance",
-        default=0.0001,
-        description="Tolerance of integration"
-    )
-
-    _default_solver = "Dassl"
-    _allowed_solvers = ["Dassl", "Euler", "Cerk23", "Cerk34", "Cerk45",
-                        "Esdirk23a", "Esdirk34a", "Esdirk45a", "Cvode",
-                        "Rkfix2", "Rkfix3", "Rkfix4", "Lsodar",
-                        "Radau", "Dopri45", "Dopri853", "Sdirk34hw"]
-
-
-class DymolaAPI(SimulationAPI):
-    """
-    API to a Dymola instance.
-
-    :param str,os.path.normpath cd:
-        Dirpath for the current working directory of dymola
-    :param str model_name:
-        Name of the model to be simulated
-    :param list packages:
-        List with path's to the packages needed to simulate the model
-    :keyword Boolean show_window:
-        True to show the Dymola window. Default is False
-    :keyword Boolean modify_structural_parameters:
-        True to automatically set the structural parameters of the
-        simulation model via Modelica modifiers. Default is True.
-        See also the keyword ``structural_parameters``
-        of the ``simulate`` function.
-    :keyword Boolean equidistant_output:
-        If True (Default), Dymola stores variables in an
-        equisdistant output and does not store variables at events.
-    :keyword str dymola_path:
-         Path to the dymola installation on the device. Necessary
-         e.g. on linux, if we can't find the path automatically.
-         Example: ``dymola_path="C://Program Files//Dymola 2020x"``
-    :keyword int n_restart:
-        Number of iterations after which Dymola should restart.
-        This is done to free memory. Default value -1. For values
-        below 1 Dymola does not restart.
-    :keyword bool extract_variables:
-        If True (the default), all variables of the model will be extracted
-        on init of this class.
-        This required translating the model.
-    :keyword bool debug:
-        If True (not the default), the dymola instance is not closed
-        on exit of the python script. This allows further debugging in
-        dymola itself if API-functions cause a python error.
-    :keyword str mos_script_pre:
-        Path to a valid mos-script for Modelica/Dymola.
-        If given, the script is executed **prior** to laoding any
-        package specified in this API.
-        May be relevant for handling version conflicts.
-    :keyword str mos_script_post:
-        Path to a valid mos-script for Modelica/Dymola.
-        If given, the script is executed before closing Dymola.
-    :keyword str dymola_version:
-        Version of Dymola to use.
-        If not given, newest version will be used.
-        If given, the Version needs to be equal to the folder name
-        of your installation.
-
-        **Example:** If you have two version installed at
-
-        - ``C://Program Files//Dymola 2021`` and
-        - ``C://Program Files//Dymola 2020x``
-
-        and you want to use Dymola 2020x, specify
-        ``dymola_version='Dymola 2020x'``.
-
-        This parameter is overwritten if ``dymola_path`` is specified.
-
-    Example:
-
-    >>> import os
-    >>> from ebcpy import DymolaAPI
-    >>> # Specify the model name
-    >>> model_name = "Modelica.Thermal.FluidHeatFlow.Examples.PumpAndValve"
-    >>> dym_api = DymolaAPI(cd=os.getcwd(),
-    >>>                     model_name=model_name,
-    >>>                     packages=[],
-    >>>                     show_window=True)
-    >>> dym_api.sim_setup = {"start_time": 100,
-    >>>                      "stop_time": 200}
-    >>> dym_api.simulate()
-    >>> dym_api.close()
-
-    """
-    _sim_setup_class: SimulationSetupClass = DymolaSimulationSetup
-    _items_to_drop = ["pool", "dymola", "_dummy_dymola_instance"]
-    dymola = None
-    # Default simulation setup
-    _supported_kwargs = [
-        "show_window",
-        "modify_structural_parameters",
-        "dymola_path",
-        "equidistant_output",
-        "n_restart",
-        "debug",
-        "mos_script_pre",
-        "mos_script_post",
-        "dymola_version"
-    ]
-
-    def __init__(self, cd, model_name, packages=None, **kwargs):
-        """Instantiate class objects."""
-        self.dymola = None  # Avoid key-error in get-state. Instance attribute needs to be there.
-        # Update kwargs with regard to what kwargs are supported.
-        self.extract_variables = kwargs.pop("extract_variables", True)
-        self.fully_initialized = False
-        self.debug = kwargs.pop("debug", False)
-        self.show_window = kwargs.pop("show_window", False)
-        self.modify_structural_parameters = kwargs.pop("modify_structural_parameters", True)
-        self.equidistant_output = kwargs.pop("equidistant_output", True)
-        self.mos_script_pre = kwargs.pop("mos_script_pre", None)
-        self.mos_script_post = kwargs.pop("mos_script_post", None)
-        self.dymola_version = kwargs.pop("dymola_version", None)
-        for mos_script in [self.mos_script_pre, self.mos_script_post]:
-            if mos_script is not None:
-                if not os.path.isfile(mos_script):
-                    raise FileNotFoundError(
-                        f"Given mos_script '{mos_script}' does "
-                        f"not exist."
-                    )
-                if not str(mos_script).endswith(".mos"):
-                    raise TypeError(
-                        f"Given mos_script '{mos_script}' "
-                        f"is not a valid .mos file."
-                    )
-
-        # Convert to modelica path
-        if self.mos_script_pre is not None:
-            self.mos_script_pre = self._make_modelica_normpath(self.mos_script_pre)
-        if self.mos_script_post is not None:
-            self.mos_script_post = self._make_modelica_normpath(self.mos_script_post)
-
-        super().__init__(cd=cd,
-                         model_name=model_name,
-                         n_cpu=kwargs.pop("n_cpu", 1))
-
-        # First import the dymola-interface
-        dymola_path = kwargs.pop("dymola_path", None)
-        if dymola_path is not None:
-            if not os.path.exists(dymola_path):
-                raise FileNotFoundError(f"Given path '{dymola_path}' can not be found on "
-                                        "your machine.")
-            _dym_install = dymola_path
-        else:
-            # Get the dymola-install-path:
-            _dym_installations = self.get_dymola_install_paths()
-            if _dym_installations:
-                if self.dymola_version:
-                    _found_version = False
-                    for _dym_install in _dym_installations:
-                        if _dym_install.endswith(self.dymola_version):
-                            _found_version = True
-                            break
-                    if not _found_version:
-                        raise ValueError(
-                            f"Given dymola_version '{self.dymola_version}' not found in "
-                            f"the list of dymola installations {_dym_installations}"
-                        )
-                else:
-                    _dym_install = _dym_installations[0]  # 0 is the newest
-                self.logger.info("Using dymola installation at %s", _dym_install)
-            else:
-                raise FileNotFoundError("Could not find a dymola-interface on your machine.")
-        dymola_exe_path = self.get_dymola_path(_dym_install)
-        self.logger.info("Using dymola.exe: %s", dymola_exe_path)
-        dymola_interface_path = self.get_dymola_interface_path(_dym_install)
-        self.logger.info("Using dymola interface: %s", dymola_interface_path)
-
-        # Set the path variables:
-        self.dymola_interface_path = dymola_interface_path
-        self.dymola_exe_path = dymola_exe_path
-
-        self.packages = []
-        if packages is not None:
-            for package in packages:
-                if isinstance(package, pathlib.Path):
-                    self.packages.append(str(package))
-                elif isinstance(package, str):
-                    self.packages.append(package)
-                else:
-                    raise TypeError(f"Given package is of type {type(package)}"
-                                    f" but should be any valid path.")
-
-        # Import n_restart
-        self.sim_counter = 0
-        self.n_restart = kwargs.pop("n_restart", -1)
-        if not isinstance(self.n_restart, int):
-            raise TypeError(f"n_restart has to be type int but "
-                            f"is of type {type(self.n_restart)}")
-
-        self._dummy_dymola_instance = None  # Ensure self._close_dummy gets the attribute.
-        if self.n_restart > 0:
-            self.logger.info("Open blank placeholder Dymola instance to ensure"
-                             " a licence during Dymola restarts")
-            self._dummy_dymola_instance = self._open_dymola_interface()
-            atexit.register(self._close_dummy)
-
-        # List storing structural parameters for later modifying the simulation-name.
-        # Parameter for raising a warning if to many dymola-instances are running
-        self._critical_number_instances = 10 + self.n_cpu
-        # Register the function now in case of an error.
-        if not self.debug:
-            atexit.register(self.close)
-        if self.use_mp:
-            self.pool.map(self._setup_dymola_interface, [True for _ in range(self.n_cpu)])
-        # For translation etc. always setup a default dymola instance
-        self.dymola = self._setup_dymola_interface(use_mp=False)
-
-        self.fully_initialized = True
-        # Trigger on init.
-        self._update_model()
-        # Set result_names to output variables.
-        self.result_names = list(self.outputs.keys())
-
-        # Check if some kwargs are still present. If so, inform the user about
-        # false usage of kwargs:
-        if kwargs:
-            self.logger.error(
-                "You passed the following kwargs which "
-                "are not part of the supported kwargs and "
-                "have thus no effect: %s.", " ,".join(list(kwargs.keys())))
-
-    def _update_model(self):
-        # Translate the model and extract all variables,
-        # if the user wants to:
-        if self.extract_variables and self.fully_initialized:
-            self.extract_model_variables()
-
-    def simulate(self,
-                 parameters: Union[dict, List[dict]] = None,
-                 return_option: str = "time_series",
-                 **kwargs):
-        """
-        Simulate the given parameters.
-
-        Additional settings:
-
-        :keyword List[str] model_names:
-            List of Dymola model-names to simulate. Should be either the size
-            of parameters or parameters needs to be sized 1.
-            Keep in mind that different models may use different parameters!
-        :keyword Boolean show_eventlog:
-            Default False. True to show evenlog of simulation (advanced)
-        :keyword Boolean squeeze:
-            Default True. If only one set of initialValues is provided,
-            a DataFrame is returned directly instead of a list.
-        :keyword str table_name:
-            If inputs are given, you have to specify the name of the table
-            in the instance of CombiTimeTable. In order for the inputs to
-            work the value should be equal to the value of 'tableName' in Modelica.
-        :keyword str file_name:
-            If inputs are given, you have to specify the file_name of the table
-            in the instance of CombiTimeTable. In order for the inputs to
-            work the value should be equal to the value of 'fileName' in Modelica.
-        :keyword List[str] structural_parameters:
-            A list containing all parameter names which are structural in Modelica.
-            This means a modifier has to be created in order to change
-            the value of this parameter. Internally, the given list
-            is added to the known states of the model. Hence, you only have to
-            specify this keyword argument if your structural parameter
-            does not appear in the dsin.txt file created during translation.
-
-            Example:
-            Changing a record in a model:
-
-            >>> sim_api.simulate(
-            >>>     parameters={"parameterPipe": "AixLib.DataBase.Pipes.PE_X.DIN_16893_SDR11_d160()"},
-            >>>     structural_parameters=["parameterPipe"])
-
-        """
-        # Handle special case for structural_parameters
-        if "structural_parameters" in kwargs:
-            _struc_params = kwargs["structural_parameters"]
-            # Check if input is 2-dimensional for multiprocessing.
-            # If not, make it 2-dimensional to avoid list flattening in
-            # the super method.
-            if not isinstance(_struc_params[0], list):
-                kwargs["structural_parameters"] = [_struc_params]
-        if "model_names" in kwargs:
-            model_names = kwargs["model_names"]
-            if not isinstance(model_names, list):
-                raise TypeError("model_names needs to be a list.")
-            if isinstance(parameters, dict):
-                # Make an array of parameters to enable correct use of super function.
-                parameters = [parameters] * len(model_names)
-            if parameters is None:
-                parameters = [{}] * len(model_names)
-        return super().simulate(parameters=parameters, return_option=return_option, **kwargs)
-
-    def _single_simulation(self, kwargs):
-        # Unpack kwargs
-        show_eventlog = kwargs.get("show_eventlog", False)
-        squeeze = kwargs.get("squeeze", True)
-        result_file_name = kwargs.get("result_file_name", 'resultFile')
-        parameters = kwargs.get("parameters")
-        return_option = kwargs.get("return_option")
-        model_names = kwargs.get("model_names")
-        inputs = kwargs.get("inputs", None)
-        fail_on_error = kwargs.get("fail_on_error", True)
-        structural_parameters = kwargs.get("structural_parameters", [])
-
-        # Handle multiprocessing
-        if self.use_mp:
-            idx_worker = self.worker_idx
-            if self.dymola is None:
-                self._setup_dymola_interface(use_mp=True)
-
-        # Handle eventlog
-        if show_eventlog:
-            self.dymola.experimentSetupOutput(events=True)
-            self.dymola.ExecuteCommand("Advanced.Debug.LogEvents = true")
-            self.dymola.ExecuteCommand("Advanced.Debug.LogEventsInitialization = true")
-
-        # Restart Dymola after n_restart iterations
-        self._check_restart()
-
-        # Handle custom model_names
-        if model_names is not None:
-            # Custom model_name setting
-            _res_names = self.result_names.copy()
-            self._model_name = model_names
-            self._update_model_variables()
-            if _res_names != self.result_names:
-                self.logger.info(
-                    "Result names changed due to setting the new model. "
-                    "If you do not expect custom result names, ignore this warning."
-                    "If you do expect them, please raise an issue to add the "
-                    "option when using the model_names keyword.")
-                self.logger.info(
-                    "Difference: %s",
-                    " ,".join(list(set(_res_names).difference(self.result_names)))
-                )
-
-        # Handle parameters:
-        if parameters is None:
-            parameters = {}
-            unsupported_parameters = False
-        else:
-            unsupported_parameters = self.check_unsupported_variables(
-                variables=list(parameters.keys()),
-                type_of_var="parameters"
-            )
-
-        # Handle structural parameters
-
-        if (unsupported_parameters and
-                (self.modify_structural_parameters or
-                 structural_parameters)):
-            # Alter the model_name for the next simulation
-            model_name, parameters_new = self._alter_model_name(
-                parameters=parameters,
-                model_name=self.model_name,
-                structural_params=list(self.states.keys()) + structural_parameters
-            )
-            # Trigger translation only if something changed
-            if model_name != self.model_name:
-                _res_names = self.result_names.copy()
-                self.model_name = model_name
-                self.result_names = _res_names  # Restore previous result names
-                self.logger.warning(
-                    "Warning: Currently, the model is re-translating "
-                    "for each simulation. You should add to your Modelica "
-                    "parameters \"annotation(Evaluate=false)\".\n "
-                    "Check for these parameters: %s",
-                    ', '.join(set(parameters.keys()).difference(parameters_new.keys()))
-                )
-            parameters = parameters_new
-            # Check again
-            unsupported_parameters = self.check_unsupported_variables(
-                variables=list(parameters.keys()),
-                type_of_var="parameters"
-            )
-
-        initial_names = list(parameters.keys())
-        initial_values = list(parameters.values())
-        # Convert to float for Boolean and integer types:
-        try:
-            initial_values = [float(v) for v in initial_values]
-        except (ValueError, TypeError) as err:
-            raise TypeError("Dymola only accepts float values. "
-                            "Could bot automatically convert the given "
-                            "parameter values to float.") from err
-
-        # Handle inputs
-        if inputs is not None:
-            # Unpack additional kwargs
-            try:
-                table_name = kwargs["table_name"]
-                file_name = kwargs["file_name"]
-            except KeyError as err:
-                raise KeyError("For inputs to be used by DymolaAPI.simulate, you "
-                               "have to specify the 'table_name' and the 'file_name' "
-                               "as keyword arguments of the function. These must match"
-                               "the values 'tableName' and 'fileName' in the CombiTimeTable"
-                               " model in your modelica code.") from err
-            # Generate the input in the correct format
-            offset = self.sim_setup.start_time - inputs.index[0]
-            filepath = convert_tsd_to_modelica_txt(
-                tsd=inputs,
-                table_name=table_name,
-                save_path_file=file_name,
-                offset=offset
-            )
-            self.logger.info("Successfully created Dymola input file at %s", filepath)
-
-        if return_option == "savepath":
-            if unsupported_parameters:
-                raise KeyError("Dymola does not accept invalid parameter "
-                               "names for option return_type='savepath'. "
-                               "To use this option, delete unsupported "
-                               "parameters from your setup.")
-            res = self.dymola.simulateExtendedModel(
-                self.model_name,
-                startTime=self.sim_setup.start_time,
-                stopTime=self.sim_setup.stop_time,
-                numberOfIntervals=0,
-                outputInterval=self.sim_setup.output_interval,
-                method=self.sim_setup.solver,
-                tolerance=self.sim_setup.tolerance,
-                fixedstepsize=self.sim_setup.fixedstepsize,
-                resultFile=result_file_name,
-                initialNames=initial_names,
-                initialValues=initial_values)
-        else:
-            if not parameters and not self.parameters:
-                raise ValueError(
-                    "Sadly, simulating a model in Dymola "
-                    "with no parameters returns no result. "
-                    "Call this function using return_option='savepath' to get the results."
-                )
-            if not parameters:
-                random_name = list(self.parameters.keys())[0]
-                initial_values = [self.parameters[random_name].value]
-                initial_names = [random_name]
-
-            # Handle 1 and 2 D initial names:
-            # Convert a 1D list to 2D list
-            if initial_values and isinstance(initial_values[0], (float, int)):
-                initial_values = [initial_values]
-
-            # Handle the time of the simulation:
-            res_names = self.result_names.copy()
-            if "Time" not in res_names:
-                res_names.append("Time")
-
-            # Internally convert output Interval to number of intervals
-            # (Required by function simulateMultiResultsModel
-            number_of_intervals = (self.sim_setup.stop_time - self.sim_setup.start_time) / \
-                                  self.sim_setup.output_interval
-            if int(number_of_intervals) != number_of_intervals:
-                raise ValueError(
-                    "Given output_interval and time interval did not yield "
-                    "an integer numberOfIntervals. To use this functions "
-                    "without savepaths, you have to provide either a "
-                    "numberOfIntervals or a value for output_interval "
-                    "which can be converted to numberOfIntervals.")
-
-            res = self.dymola.simulateMultiResultsModel(
-                self.model_name,
-                startTime=self.sim_setup.start_time,
-                stopTime=self.sim_setup.stop_time,
-                numberOfIntervals=int(number_of_intervals),
-                method=self.sim_setup.solver,
-                tolerance=self.sim_setup.tolerance,
-                fixedstepsize=self.sim_setup.fixedstepsize,
-                resultFile=None,
-                initialNames=initial_names,
-                initialValues=initial_values,
-                resultNames=res_names)
-
-        if not res[0]:
-            self.logger.error("Simulation failed!")
-            self.logger.error("The last error log from Dymola:")
-            log = self.dymola.getLastErrorLog()
-            # Only print first part as output is sometimes to verbose.
-            self.logger.error(log[:10000])
-            dslog_path = os.path.join(self.cd, 'dslog.txt')
-            try:
-                with open(dslog_path, "r") as dslog_file:
-                    dslog_content = dslog_file.read()
-                    self.logger.error(dslog_content)
-            except Exception:
-                dslog_content = "Not retreivable. Open it yourself."
-            msg = f"Simulation failed: Reason according " \
-                  f"to dslog, located at '{dslog_path}': {dslog_content}"
-            if fail_on_error:
-                raise Exception(msg)
-            # Don't raise and return None
-            self.logger.error(msg)
-            return None
-
-        if return_option == "savepath":
-            _save_name_dsres = f"{result_file_name}.mat"
-            savepath = kwargs.pop("savepath", None)
-            # Get the cd of the current dymola instance
-            self.dymola.cd()
-            # Get the value and convert it to a 100 % fitting str-path
-            dymola_cd = str(pathlib.Path(self.dymola.getLastErrorLog().replace("\n", "")))
-            if savepath is None or str(savepath) == dymola_cd:
-                return os.path.join(dymola_cd, _save_name_dsres)
-            os.makedirs(savepath, exist_ok=True)
-            for filename in [_save_name_dsres, "dslog.txt", "dsfinal.txt"]:
-                # Delete existing files
-                try:
-                    os.remove(os.path.join(savepath, filename))
-                except OSError:
-                    pass
-                # Move files
-                shutil.copy(os.path.join(dymola_cd, filename),
-                            os.path.join(savepath, filename))
-                os.remove(os.path.join(dymola_cd, filename))
-            return os.path.join(savepath, _save_name_dsres)
-
-        data = res[1]  # Get data
-        if return_option == "last_point":
-            results = []
-            for ini_val_set in data:
-                results.append({result_name: ini_val_set[idx][-1] for idx, result_name
-                                in enumerate(res_names)})
-            if len(results) == 1 and squeeze:
-                return results[0]
-            return results
-        # Else return as dataframe.
-        dfs = []
-        for ini_val_set in data:
-            df = pd.DataFrame({result_name: ini_val_set[idx] for idx, result_name
-                               in enumerate(res_names)})
-            # Set time index
-            df = df.set_index("Time")
-            # Convert it to float
-            df.index = df.index.astype("float64")
-            dfs.append(df)
-        # Most of the cases, only one set is provided. In that case, avoid
-        if len(dfs) == 1 and squeeze:
-            return TimeSeriesData(dfs[0], default_tag="sim")
-        return [TimeSeriesData(df, default_tag="sim") for df in dfs]
-
-    def translate(self):
-        """
-        Translates the current model using dymola.translateModel()
-        and checks if erros occur.
-        """
-        res = self.dymola.translateModel(self.model_name)
-        if not res:
-            self.logger.error("Translation failed!")
-            self.logger.error("The last error log from Dymola:")
-            self.logger.error(self.dymola.getLastErrorLog())
-            raise Exception("Translation failed - Aborting")
-
-    def set_compiler(self, name, path, dll=False, dde=False, opc=False):
-        """
-        Set up the compiler and compiler options on Windows.
-        Optional: Specify if you want to enable dll, dde or opc.
-
-        :param str name:
-            Name of the compiler, avaiable options:
-            - 'vs': Visual Studio
-            - 'gcc': GCC
-        :param str,os.path.normpath path:
-            Path to the compiler files.
-            Example for name='vs': path='C:/Program Files (x86)/Microsoft Visual Studio 10.0/Vc'
-            Example for name='gcc': path='C:/MinGW/bin/gcc'
-        :param Boolean dll:
-            Set option for dll support. Check Dymolas Manual on what this exactly does.
-        :param Boolean dde:
-            Set option for dde support. Check Dymolas Manual on what this exactly does.
-        :param Boolean opc:
-            Set option for opc support. Check Dymolas Manual on what this exactly does.
-        :return: True, on success.
-        """
-        # Lookup dict for internal name of CCompiler-Variable
-        _name_int = {"vs": "MSVC",
-                     "gcc": "GCC"}
-
-        if "win" not in sys.platform:
-            raise OSError(f"set_compiler function only implemented "
-                          f"for windows systems, you are using {sys.platform}")
-        # Manually check correct input as Dymola's error are not a help
-        name = name.lower()
-        if name not in ["vs", "gcc"]:
-            raise ValueError(f"Given compiler name {name} not supported.")
-        if not os.path.exists(path):
-            raise FileNotFoundError(f"Given compiler path {path} does not exist on your machine.")
-        # Convert path for correct input
-        path = self._make_modelica_normpath(path)
-        if self.use_mp:
-            raise ValueError("Given function is not yet supported for multiprocessing")
-
-        res = self.dymola.SetDymolaCompiler(name.lower(),
-                                            [f"CCompiler={_name_int[name]}",
-                                             f"{_name_int[name]}DIR={path}",
-                                             f"DLL={int(dll)}",
-                                             f"DDE={int(dde)}",
-                                             f"OPC={int(opc)}"])
-
-        return res
-
-    def import_initial(self, filepath):
-        """
-        Load given dsfinal.txt into dymola
-
-        :param str,os.path.normpath filepath:
-            Path to the dsfinal.txt to be loaded
-        """
-        if not os.path.isfile(filepath):
-            raise FileNotFoundError(f"Given filepath {filepath} does not exist")
-        if not os.path.splitext(filepath)[1] == ".txt":
-            raise TypeError('File is not of type .txt')
-        if self.use_mp:
-            raise ValueError("Given function is not yet supported for multiprocessing")
-        res = self.dymola.importInitial(dsName=filepath)
-        if res:
-            self.logger.info("Successfully loaded dsfinal.txt")
-        else:
-            raise Exception("Could not load dsfinal into Dymola.")
-
-    @SimulationAPI.cd.setter
-    def cd(self, cd):
-        """Set the working directory to the given path"""
-        self._cd = cd
-        if self.dymola is None:  # Not yet started
-            return
-        # Also set the cd in the dymola api
-        self.set_dymola_cd(dymola=self.dymola,
-                           cd=cd)
-        if self.use_mp:
-            self.logger.warning("Won't set the cd for all workers, "
-                                "not yet implemented.")
-
-    def set_dymola_cd(self, dymola, cd):
-        """
-        Set the cd of the Dymola Instance.
-        Before calling the Function, create the path and
-        convert to a modelica-normpath.
-        """
-        os.makedirs(cd, exist_ok=True)
-        cd_modelica = self._make_modelica_normpath(path=cd)
-        res = dymola.cd(cd_modelica)
-        if not res:
-            raise OSError(f"Could not change working directory to {cd}")
-
-    def close(self):
-        """Closes dymola."""
-        # Close MP of super class
-        super().close()
-        # Always close main instance
-        self._single_close(dymola=self.dymola)
-
-    def _close_multiprocessing(self, _):
-        self._single_close()
-        DymolaAPI.dymola = None
-
-    def _single_close(self, **kwargs):
-        """Closes a single dymola instance"""
-        if self.dymola is None:
-            return  # Already closed prior
-        # Execute the mos-script if given:
-        if self.mos_script_post is not None:
-            self.logger.info("Executing given mos_script_post "
-                             "prior to closing.")
-            self.dymola.RunScript(self.mos_script_post)
-            self.logger.info("Output of mos_script_post: %s", self.dymola.getLastErrorLog())
-        self.logger.info('Closing Dymola')
-        self.dymola.close()
-        self.logger.info('Successfully closed Dymola')
-        self.dymola = None
-
-    def _close_dummy(self):
-        """
-        Closes dummy instance at the end of the execution
-        """
-        if self._dummy_dymola_instance is not None:
-            self.logger.info('Closing dummy Dymola instance')
-            self._dummy_dymola_instance.close()
-            self.logger.info('Successfully closed dummy Dymola instance')
-
-    def extract_model_variables(self):
-        """
-        Extract all variables of the model by
-        translating it and then processing the dsin
-        using the manipulate_ds module.
-        """
-        # Translate model
-        self.logger.info("Translating model '%s' to extract model variables ",
-                         self.model_name)
-        self.translate()
-        # Get path to dsin:
-        dsin_path = os.path.join(self.cd, "dsin.txt")
-        df = manipulate_ds.convert_ds_file_to_dataframe(dsin_path)
-        # Convert and return all parameters of dsin to initial values and names
-        for idx, row in df.iterrows():
-            _max = float(row["4"])
-            _min = float(row["3"])
-            if _min >= _max:
-                _var_ebcpy = Variable(value=float(row["2"]))
-            else:
-                _var_ebcpy = Variable(
-                    min=_min,
-                    max=_max,
-                    value=float(row["2"])
-                )
-            if row["5"] == "1":
-                self.parameters[idx] = _var_ebcpy
-            elif row["5"] == "5":
-                self.inputs[idx] = _var_ebcpy
-            elif row["5"] == "4":
-                self.outputs[idx] = _var_ebcpy
-            else:
-                self.states[idx] = _var_ebcpy
-
-    def _setup_dymola_interface(self, use_mp):
-        """Load all packages and change the current working directory"""
-        dymola = self._open_dymola_interface()
-        self._check_dymola_instances()
-        if use_mp:
-            cd = os.path.join(self.cd, f"worker_{self.worker_idx}")
-        else:
-            cd = self.cd
-        # Execute the mos-script if given:
-        if self.mos_script_pre is not None:
-            self.logger.info("Executing given mos_script_pre "
-                             "prior to loading packages.")
-            dymola.RunScript(self.mos_script_pre)
-            self.logger.info("Output of mos_script_pre: %s", dymola.getLastErrorLog())
-
-        # Set the cd in the dymola api
-        self.set_dymola_cd(dymola=dymola, cd=cd)
-
-        for package in self.packages:
-            self.logger.info("Loading Model %s", os.path.dirname(package).split("\\")[-1])
-            res = dymola.openModel(package, changeDirectory=False)
-            if not res:
-                raise ImportError(dymola.getLastErrorLog())
-        self.logger.info("Loaded modules")
-        if self.equidistant_output:
-            # Change the Simulation Output, to ensure all
-            # simulation results have the same array shape.
-            # Events can also cause errors in the shape.
-            dymola.experimentSetupOutput(equidistant=True,
-                                         events=False)
-        if not dymola.RequestOption("Standard"):
-            warnings.warn("You have no licence to use Dymola. "
-                          "Hence you can only simulate models with 8 or less equations.")
-        if use_mp:
-            DymolaAPI.dymola = dymola
-            return None
-        return dymola
-
-    def _open_dymola_interface(self):
-        """Open an instance of dymola and return the API-Object"""
-        if self.dymola_interface_path not in sys.path:
-            sys.path.insert(0, self.dymola_interface_path)
-        try:
-            from dymola.dymola_interface import DymolaInterface
-            from dymola.dymola_exception import DymolaConnectionException
-            return DymolaInterface(showwindow=self.show_window,
-                                   dymolapath=self.dymola_exe_path)
-        except ImportError as error:
-            raise ImportError("Given dymola-interface could not be "
-                              "loaded:\n %s" % self.dymola_interface_path) from error
-        except DymolaConnectionException as error:
-            raise ConnectionError(error) from error
-
-    def to_dict(self):
-        """
-        Store the most relevant information of this class
-        into a dictionary. This may be used for future configuration.
-
-        :return: dict config:
-            Dictionary with keys to re-init this class.
-        """
-        # Convert Path to str to enable json-dumping
-        config = {"cd": str(self.cd),
-                  "packages": [str(pack) for pack in self.packages],
-                  "model_name": self.model_name,
-                  "type": "DymolaAPI",
-                  }
-        # Update kwargs
-        config.update({kwarg: self.__dict__.get(kwarg, None)
-                       for kwarg in self._supported_kwargs})
-
-        return config
-
-    def get_packages(self):
-        """
-        Get the currently loaded packages of Dymola
-        """
-        packages = self.dymola.ExecuteCommand(
-            'ModelManagement.Structure.AST.Misc.ClassesInPackage("")'
-        )
-        valid_packages = []
-        for pack in packages:
-            current_package = f"modelica://{pack}/package.order"
-            pack_path = self.dymola.ExecuteCommand(
-                f'Modelica.Utilities.Files.loadResource("{current_package}")'
-            )
-            if not isinstance(pack_path, str):
-                self.logger.error("Could not load model resource for package %s", pack)
-            if os.path.isfile(pack_path):
-                valid_packages.append(pathlib.Path(pack_path).parent)
-        return valid_packages
-
-    def save_for_reproduction(
-            self,
-            title: str,
-            path: pathlib.Path = None,
-            files: list = None,
-            save_total_model: bool = True,
-            export_fmu: bool = True
-    ):
-        """
-        Additionally to the basic reproduction, add info
-        for Dymola packages.
-
-        Content which is saved:
-        - DymolaAPI configuration
-        - Information on Dymola: Version, flags
-        - All loaded packages
-        - Total model, if save_total_model = True
-        - FMU, if export_fmu = True
-
-        :param bool save_total_model:
-            True to save the total model
-        :param bool export_fmu:
-            True to export the FMU of the current model.
-        """
-        # Local import to require git-package only when called
-        from ebcpy.utils.reproduction import ReproductionFile, CopyFile, get_git_information
-
-        if files is None:
-            files = []
-        # DymolaAPI Info:
-        files.append(ReproductionFile(
-            filename="Dymola/DymolaAPI_config.json",
-            content=json.dumps(self.to_dict(), indent=2)
-        ))
-        # Dymola info:
-        self.dymola.ExecuteCommand("list();")
-        _flags = self.dymola.getLastErrorLog()
-        dymola_info = [
-            self.dymola.ExecuteCommand("DymolaVersion()"),
-            str(self.dymola.ExecuteCommand("DymolaVersionNumber()")),
-            "\n\n"
-        ]
-        files.append(ReproductionFile(
-            filename="Dymola/DymolaInfo.txt",
-            content="\n".join(dymola_info) + _flags
-        ))
-
-        # Packages
-        packages = self.get_packages()
-        package_infos = []
-        for pack_path in packages:
-
-            for pack_dir_parent in [pack_path] + list(pack_path.parents):
-                repo_info = get_git_information(
-                    path=pack_dir_parent,
-                    zip_folder_path="Dymola"
-                )
-                if not repo_info:
-                    continue
-
-                files.extend(repo_info.pop("difference_files"))
-                pack_path = str(pack_path) + "; " + "; ".join([f"{key}: {value}" for key, value in repo_info.items()])
-                break
-            package_infos.append(str(pack_path))
-        files.append(ReproductionFile(
-            filename="Dymola/Modelica_packages.txt",
-            content="\n".join(package_infos)
-        ))
-        # Total model
-        if save_total_model:
-            _total_model_name = f"Dymola/{self.model_name.replace('.', '_')}_total.mo"
-            _total_model = pathlib.Path(self.cd).joinpath(_total_model_name)
-            os.makedirs(_total_model.parent, exist_ok=True)  # Create to ensure model can be saved.
-            res = self.dymola.saveTotalModel(
-                fileName=str(_total_model),
-                modelName=self.model_name
-            )
-            if res:
-                files.append(ReproductionFile(
-                    filename=_total_model_name,
-                    content=_total_model.read_text()
-                ))
-                os.remove(_total_model)
-            else:
-                self.logger.error("Could not save total model: %s",
-                                  self.dymola.getLastErrorLog())
-        # FMU
-        if export_fmu:
-            _fmu_path = self._save_to_fmu(fail_on_error=False)
-            if _fmu_path is not None:
-                files.append(CopyFile(
-                    sourcepath=_fmu_path,
-                    filename="Dymola/" + _fmu_path.name,
-                    remove=True
-                ))
-
-        return super().save_for_reproduction(
-            title=title,
-            path=path,
-            files=files
-        )
-
-    def _save_to_fmu(self, fail_on_error):
-        """Save model as an FMU"""
-        res = self.dymola.translateModelFMU(
-            modelToOpen=self.model_name,
-            storeResult=False,
-            modelName='',
-            fmiVersion='2',
-            fmiType='all',
-            includeSource=False,
-            includeImage=0
-        )
-        if not res:
-            msg = "Could not export fmu: %s" % self.dymola.getLastErrorLog()
-            self.logger.error(msg)
-            if fail_on_error:
-                raise Exception(msg)
-        else:
-            path = pathlib.Path(self.cd).joinpath(res + ".fmu")
-            return path
-
-    @staticmethod
-    def _make_modelica_normpath(path):
-        """
-        Convert given path to a path readable in dymola.
-        If the base path does not exist, create it.
-
-        :param str,os.path.normpath path:
-            Either a file or a folder path. The base to this
-            path is created in non existent.
-        :return: str
-            Path readable in dymola
-        """
-        if isinstance(path, pathlib.Path):
-            path = str(path)
-
-        path = path.replace("\\", "/")
-        # Search for e.g. "D:testzone" and replace it with D:/testzone
-        loc = path.find(":")
-        if path[loc + 1] != "/" and loc != -1:
-            path = path.replace(":", ":/")
-        return path
-
-    @staticmethod
-    def get_dymola_interface_path(dymola_install_dir):
-        """
-        Function to get the path of the newest dymola interface
-        installment on the used machine
-
-        :param str dymola_install_dir:
-            The dymola installation folder. Example:
-            "C://Program Files//Dymola 2020"
-        :return: str
-            Path to the dymola.egg-file
-        """
-        path_to_egg_file = os.path.normpath("Modelica/Library/python_interface/dymola.egg")
-        egg_file = os.path.join(dymola_install_dir, path_to_egg_file)
-        if not os.path.isfile(egg_file):
-            raise FileNotFoundError(f"The given dymola installation directory "
-                                    f"'{dymola_install_dir}' has no "
-                                    f"dymola-interface egg-file.")
-        return egg_file
-
-    @staticmethod
-    def get_dymola_path(dymola_install_dir, dymola_name=None):
-        """
-        Function to get the path of the dymola exe-file
-        on the current used machine.
-
-        :param str dymola_install_dir:
-            The dymola installation folder. Example:
-            "C://Program Files//Dymola 2020"
-        :param str dymola_name:
-            Name of the executable. On Windows it is always Dymola.exe, on
-            linux just dymola.
-        :return: str
-            Path to the dymola-exe-file.
-        """
-        if dymola_name is None:
-            if "linux" in sys.platform:
-                dymola_name = "dymola"
-            elif "win" in sys.platform:
-                dymola_name = "Dymola.exe"
-            else:
-                raise OSError(f"Your operating system {sys.platform} has no default dymola-name."
-                              f"Please provide one.")
-
-        bin_64 = os.path.join(dymola_install_dir, "bin64", dymola_name)
-        bin_32 = os.path.join(dymola_install_dir, "bin", dymola_name)
-        if os.path.isfile(bin_64):  # First check for 64bit installation
-            dym_file = bin_64
-        elif os.path.isfile(bin_32):  # Else use the 32bit version
-            dym_file = bin_32
-        else:
-            raise FileNotFoundError(
-                f"The given dymola installation has not executable at '{bin_32}'. "
-                f"If your dymola_path exists, please raise an issue."
-            )
-
-        return dym_file
-
-    @staticmethod
-    def get_dymola_install_paths(basedir=None):
-        """
-        Function to get all paths of dymola installations
-        on the used machine. Supported platforms are:
-        * Windows
-        * Linux
-        * Mac OS X
-        If multiple installation of Dymola are found, the newest version will be returned.
-        This assumes the names are sortable, e.g. Dymola 2020, Dymola 2019 etc.
-
-        :param str basedir:
-            The base-directory to search for the dymola-installation.
-            The default value depends on the platform one is using.
-            On Windows it is "C://Program Files" or "C://Program Files (x86)" (for 64 bit)
-            On Linux it is "/opt" (based on our ci-Docker configuration
-            On Mac OS X "/Application" (based on the default)
-        :return: str
-            Path to the dymola-installation
-        """
-
-        if basedir is None:
-            if "linux" in sys.platform:
-                basedir = os.path.normpath("/opt")
-            elif "win" in sys.platform:
-                basedir = os.path.normpath("C:/Program Files")
-            elif "darwin" in sys.platform:
-                basedir = os.path.normpath("/Applications")
-            else:
-                raise OSError(f"Your operating system ({sys.platform})does not support "
-                              f"a default basedir. Please provide one.")
-
-        syspaths = [basedir]
-        # Check if 64bit is installed (Windows only)
-        systempath_64 = os.path.normpath("C://Program Files (x86)")
-        if os.path.exists(systempath_64):
-            syspaths.append(systempath_64)
-        # Get all folders in both path's
-        temp_list = []
-        for systempath in syspaths:
-            temp_list += os.listdir(systempath)
-        # Filter programs that are not Dymola
-        dym_versions = []
-        for folder_name in temp_list:
-            # Catch both Dymola and dymola folder-names
-            if "dymola" in folder_name.lower():
-                dym_versions.append(folder_name)
-        del temp_list
-        # Find the newest version and return the egg-file
-        # This sorting only works with a good Folder structure, eg. Dymola 2020, Dymola 2019 etc.
-        dym_versions.sort()
-        valid_paths = []
-        for dym_version in reversed(dym_versions):
-            for system_path in syspaths:
-                full_path = os.path.join(system_path, dym_version)
-                if os.path.isdir(full_path):
-                    valid_paths.append(full_path)
-        return valid_paths
-
-    def _check_dymola_instances(self):
-        """
-        Check how many dymola instances are running on the machine.
-        Raise a warning if the number exceeds a certain amount.
-        """
-        # The option may be useful. However the explicit requirement leads to
-        # Problems on linux, therefore the feature is not worth the trouble.
-        # pylint: disable=import-outside-toplevel
-        try:
-            import psutil
-        except ImportError:
-            return
-        counter = 0
-        for proc in psutil.process_iter():
-            try:
-                if "Dymola" in proc.name():
-                    counter += 1
-            except psutil.AccessDenied:
-                continue
-        if counter >= self._critical_number_instances:
-            warnings.warn("There are currently %s Dymola-Instances "
-                          "running on your machine!" % counter)
-
-    @staticmethod
-    def _alter_model_name(parameters, model_name, structural_params):
-        """
-        Creates a modifier for all structural parameters,
-        based on the modelname and the initalNames and values.
-
-        :param dict parameters:
-            Parameters of the simulation
-        :param str model_name:
-            Name of the model to be modified
-        :param list structural_params:
-            List of strings with structural parameters
-        :return: str altered_modelName:
-            modified model name
-        """
-        # the structural parameter needs to be removed from paramters dict
-        new_parameters = parameters.copy()
-        model_name = model_name.split("(")[0]  # Trim old modifier
-        if parameters == {}:
-            return model_name
-        all_modifiers = []
-        for var_name, value in parameters.items():
-            # Check if the variable is in the
-            # given list of structural parameters
-            if var_name in structural_params:
-                all_modifiers.append(f"{var_name}={value}")
-                # removal of the structural parameter
-                new_parameters.pop(var_name)
-        altered_model_name = f"{model_name}({','.join(all_modifiers)})"
-        return altered_model_name, new_parameters
-
-    def _check_restart(self):
-        """Restart Dymola every n_restart iterations in order to free memory"""
-
-        if self.sim_counter == self.n_restart:
-            self.logger.info("Closing and restarting Dymola to free memory")
-            self.close()
-            self._dummy_dymola_instance = self._setup_dymola_interface(use_mp=False)
-            self.sim_counter = 1
-        else:
-            self.sim_counter += 1
+"""Module containing the DymolaAPI used for simulation
+of Modelica-Models."""
+
+import sys
+import os
+import shutil
+import pathlib
+import warnings
+import atexit
+import json
+from typing import Union, List
+from pydantic import Field
+import pandas as pd
+from ebcpy import TimeSeriesData
+from ebcpy.modelica import manipulate_ds
+from ebcpy.simulationapi import SimulationSetup, SimulationAPI, \
+    SimulationSetupClass, Variable
+from ebcpy.utils.conversion import convert_tsd_to_modelica_txt
+
+
+class DymolaSimulationSetup(SimulationSetup):
+    """
+    Adds ``tolerance`` to the list of possible
+    setup fields.
+    """
+    tolerance: float = Field(
+        title="tolerance",
+        default=0.0001,
+        description="Tolerance of integration"
+    )
+
+    _default_solver = "Dassl"
+    _allowed_solvers = ["Dassl", "Euler", "Cerk23", "Cerk34", "Cerk45",
+                        "Esdirk23a", "Esdirk34a", "Esdirk45a", "Cvode",
+                        "Rkfix2", "Rkfix3", "Rkfix4", "Lsodar",
+                        "Radau", "Dopri45", "Dopri853", "Sdirk34hw"]
+
+
+class DymolaAPI(SimulationAPI):
+    """
+    API to a Dymola instance.
+
+    :param str,os.path.normpath cd:
+        Dirpath for the current working directory of dymola
+    :param str model_name:
+        Name of the model to be simulated
+    :param list packages:
+        List with path's to the packages needed to simulate the model
+    :keyword Boolean show_window:
+        True to show the Dymola window. Default is False
+    :keyword Boolean modify_structural_parameters:
+        True to automatically set the structural parameters of the
+        simulation model via Modelica modifiers. Default is True.
+        See also the keyword ``structural_parameters``
+        of the ``simulate`` function.
+    :keyword Boolean equidistant_output:
+        If True (Default), Dymola stores variables in an
+        equisdistant output and does not store variables at events.
+    :keyword str dymola_path:
+         Path to the dymola installation on the device. Necessary
+         e.g. on linux, if we can't find the path automatically.
+         Example: ``dymola_path="C://Program Files//Dymola 2020x"``
+    :keyword int n_restart:
+        Number of iterations after which Dymola should restart.
+        This is done to free memory. Default value -1. For values
+        below 1 Dymola does not restart.
+    :keyword bool extract_variables:
+        If True (the default), all variables of the model will be extracted
+        on init of this class.
+        This required translating the model.
+    :keyword bool debug:
+        If True (not the default), the dymola instance is not closed
+        on exit of the python script. This allows further debugging in
+        dymola itself if API-functions cause a python error.
+    :keyword str mos_script_pre:
+        Path to a valid mos-script for Modelica/Dymola.
+        If given, the script is executed **prior** to laoding any
+        package specified in this API.
+        May be relevant for handling version conflicts.
+    :keyword str mos_script_post:
+        Path to a valid mos-script for Modelica/Dymola.
+        If given, the script is executed before closing Dymola.
+    :keyword str dymola_version:
+        Version of Dymola to use.
+        If not given, newest version will be used.
+        If given, the Version needs to be equal to the folder name
+        of your installation.
+
+        **Example:** If you have two version installed at
+
+        - ``C://Program Files//Dymola 2021`` and
+        - ``C://Program Files//Dymola 2020x``
+
+        and you want to use Dymola 2020x, specify
+        ``dymola_version='Dymola 2020x'``.
+
+        This parameter is overwritten if ``dymola_path`` is specified.
+    :keyword str dymola_interface_path:
+        Only relevant for the case when the dymola-exe path
+        differs from the interface path.
+
+    Example:
+
+    >>> import os
+    >>> from ebcpy import DymolaAPI
+    >>> # Specify the model name
+    >>> model_name = "Modelica.Thermal.FluidHeatFlow.Examples.PumpAndValve"
+    >>> dym_api = DymolaAPI(cd=os.getcwd(),
+    >>>                     model_name=model_name,
+    >>>                     packages=[],
+    >>>                     show_window=True)
+    >>> dym_api.sim_setup = {"start_time": 100,
+    >>>                      "stop_time": 200}
+    >>> dym_api.simulate()
+    >>> dym_api.close()
+
+    """
+    _sim_setup_class: SimulationSetupClass = DymolaSimulationSetup
+    _items_to_drop = ["pool", "dymola", "_dummy_dymola_instance"]
+    dymola = None
+    # Default simulation setup
+    _supported_kwargs = [
+        "show_window",
+        "modify_structural_parameters",
+        "dymola_path",
+        "equidistant_output",
+        "n_restart",
+        "debug",
+        "mos_script_pre",
+        "mos_script_post",
+        "dymola_version",
+        "dymola_interface_path"
+    ]
+
+    def __init__(self, cd, model_name, packages=None, **kwargs):
+        """Instantiate class objects."""
+        self.dymola = None  # Avoid key-error in get-state. Instance attribute needs to be there.
+        # Update kwargs with regard to what kwargs are supported.
+        self.extract_variables = kwargs.pop("extract_variables", True)
+        self.fully_initialized = False
+        self.debug = kwargs.pop("debug", False)
+        self.show_window = kwargs.pop("show_window", False)
+        self.modify_structural_parameters = kwargs.pop("modify_structural_parameters", True)
+        self.equidistant_output = kwargs.pop("equidistant_output", True)
+        self.mos_script_pre = kwargs.pop("mos_script_pre", None)
+        self.mos_script_post = kwargs.pop("mos_script_post", None)
+        self.dymola_version = kwargs.pop("dymola_version", None)
+        self.dymola_interface_path = kwargs.pop("dymola_interface_path", None)
+        for mos_script in [self.mos_script_pre, self.mos_script_post]:
+            if mos_script is not None:
+                if not os.path.isfile(mos_script):
+                    raise FileNotFoundError(
+                        f"Given mos_script '{mos_script}' does "
+                        f"not exist."
+                    )
+                if not str(mos_script).endswith(".mos"):
+                    raise TypeError(
+                        f"Given mos_script '{mos_script}' "
+                        f"is not a valid .mos file."
+                    )
+
+        # Convert to modelica path
+        if self.mos_script_pre is not None:
+            self.mos_script_pre = self._make_modelica_normpath(self.mos_script_pre)
+        if self.mos_script_post is not None:
+            self.mos_script_post = self._make_modelica_normpath(self.mos_script_post)
+
+        super().__init__(cd=cd,
+                         model_name=model_name,
+                         n_cpu=kwargs.pop("n_cpu", 1))
+
+        # First import the dymola-interface
+        dymola_path = kwargs.pop("dymola_path", None)
+        if dymola_path is not None:
+            if not os.path.exists(dymola_path):
+                raise FileNotFoundError(f"Given path '{dymola_path}' can not be found on "
+                                        "your machine.")
+            _dym_install = dymola_path
+        else:
+            # Get the dymola-install-path:
+            _dym_installations = self.get_dymola_install_paths()
+            if _dym_installations:
+                if self.dymola_version:
+                    _found_version = False
+                    for _dym_install in _dym_installations:
+                        if _dym_install.endswith(self.dymola_version):
+                            _found_version = True
+                            break
+                    if not _found_version:
+                        raise ValueError(
+                            f"Given dymola_version '{self.dymola_version}' not found in "
+                            f"the list of dymola installations {_dym_installations}"
+                        )
+                else:
+                    _dym_install = _dym_installations[0]  # 0 is the newest
+                self.logger.info("Using dymola installation at %s", _dym_install)
+            else:
+                raise FileNotFoundError("Could not find a dymola-interface on your machine.")
+        self.dymola_exe_path = self.get_dymola_path(_dym_install)
+        self.logger.info("Using dymola.exe: %s", self.dymola_exe_path)
+        if self.dymola_interface_path is None:
+            self.dymola_interface_path = self.get_dymola_interface_path(_dym_install)
+        self.logger.info("Using dymola interface: %s", self.dymola_interface_path)
+
+        self.packages = []
+        if packages is not None:
+            for package in packages:
+                if isinstance(package, pathlib.Path):
+                    self.packages.append(str(package))
+                elif isinstance(package, str):
+                    self.packages.append(package)
+                else:
+                    raise TypeError(f"Given package is of type {type(package)}"
+                                    f" but should be any valid path.")
+
+        # Import n_restart
+        self.sim_counter = 0
+        self.n_restart = kwargs.pop("n_restart", -1)
+        if not isinstance(self.n_restart, int):
+            raise TypeError(f"n_restart has to be type int but "
+                            f"is of type {type(self.n_restart)}")
+
+        self._dummy_dymola_instance = None  # Ensure self._close_dummy gets the attribute.
+        if self.n_restart > 0:
+            self.logger.info("Open blank placeholder Dymola instance to ensure"
+                             " a licence during Dymola restarts")
+            self._dummy_dymola_instance = self._open_dymola_interface()
+            atexit.register(self._close_dummy)
+
+        # List storing structural parameters for later modifying the simulation-name.
+        # Parameter for raising a warning if to many dymola-instances are running
+        self._critical_number_instances = 10 + self.n_cpu
+        # Register the function now in case of an error.
+        if not self.debug:
+            atexit.register(self.close)
+        if self.use_mp:
+            self.pool.map(self._setup_dymola_interface, [True for _ in range(self.n_cpu)])
+        # For translation etc. always setup a default dymola instance
+        self.dymola = self._setup_dymola_interface(use_mp=False)
+
+        self.fully_initialized = True
+        # Trigger on init.
+        self._update_model()
+        # Set result_names to output variables.
+        self.result_names = list(self.outputs.keys())
+
+        # Check if some kwargs are still present. If so, inform the user about
+        # false usage of kwargs:
+        if kwargs:
+            self.logger.error(
+                "You passed the following kwargs which "
+                "are not part of the supported kwargs and "
+                "have thus no effect: %s.", " ,".join(list(kwargs.keys())))
+
+    def _update_model(self):
+        # Translate the model and extract all variables,
+        # if the user wants to:
+        if self.extract_variables and self.fully_initialized:
+            self.extract_model_variables()
+
+    def simulate(self,
+                 parameters: Union[dict, List[dict]] = None,
+                 return_option: str = "time_series",
+                 **kwargs):
+        """
+        Simulate the given parameters.
+
+        Additional settings:
+
+        :keyword List[str] model_names:
+            List of Dymola model-names to simulate. Should be either the size
+            of parameters or parameters needs to be sized 1.
+            Keep in mind that different models may use different parameters!
+        :keyword Boolean show_eventlog:
+            Default False. True to show evenlog of simulation (advanced)
+        :keyword Boolean squeeze:
+            Default True. If only one set of initialValues is provided,
+            a DataFrame is returned directly instead of a list.
+        :keyword str table_name:
+            If inputs are given, you have to specify the name of the table
+            in the instance of CombiTimeTable. In order for the inputs to
+            work the value should be equal to the value of 'tableName' in Modelica.
+        :keyword str file_name:
+            If inputs are given, you have to specify the file_name of the table
+            in the instance of CombiTimeTable. In order for the inputs to
+            work the value should be equal to the value of 'fileName' in Modelica.
+        :keyword List[str] structural_parameters:
+            A list containing all parameter names which are structural in Modelica.
+            This means a modifier has to be created in order to change
+            the value of this parameter. Internally, the given list
+            is added to the known states of the model. Hence, you only have to
+            specify this keyword argument if your structural parameter
+            does not appear in the dsin.txt file created during translation.
+
+            Example:
+            Changing a record in a model:
+
+            >>> sim_api.simulate(
+            >>>     parameters={"parameterPipe": "AixLib.DataBase.Pipes.PE_X.DIN_16893_SDR11_d160()"},
+            >>>     structural_parameters=["parameterPipe"])
+
+        """
+        # Handle special case for structural_parameters
+        if "structural_parameters" in kwargs:
+            _struc_params = kwargs["structural_parameters"]
+            # Check if input is 2-dimensional for multiprocessing.
+            # If not, make it 2-dimensional to avoid list flattening in
+            # the super method.
+            if not isinstance(_struc_params[0], list):
+                kwargs["structural_parameters"] = [_struc_params]
+        if "model_names" in kwargs:
+            model_names = kwargs["model_names"]
+            if not isinstance(model_names, list):
+                raise TypeError("model_names needs to be a list.")
+            if isinstance(parameters, dict):
+                # Make an array of parameters to enable correct use of super function.
+                parameters = [parameters] * len(model_names)
+            if parameters is None:
+                parameters = [{}] * len(model_names)
+        return super().simulate(parameters=parameters, return_option=return_option, **kwargs)
+
+    def _single_simulation(self, kwargs):
+        # Unpack kwargs
+        show_eventlog = kwargs.get("show_eventlog", False)
+        squeeze = kwargs.get("squeeze", True)
+        result_file_name = kwargs.get("result_file_name", 'resultFile')
+        parameters = kwargs.get("parameters")
+        return_option = kwargs.get("return_option")
+        model_names = kwargs.get("model_names")
+        inputs = kwargs.get("inputs", None)
+        fail_on_error = kwargs.get("fail_on_error", True)
+        structural_parameters = kwargs.get("structural_parameters", [])
+
+        # Handle multiprocessing
+        if self.use_mp:
+            idx_worker = self.worker_idx
+            if self.dymola is None:
+                self._setup_dymola_interface(use_mp=True)
+
+        # Handle eventlog
+        if show_eventlog:
+            self.dymola.experimentSetupOutput(events=True)
+            self.dymola.ExecuteCommand("Advanced.Debug.LogEvents = true")
+            self.dymola.ExecuteCommand("Advanced.Debug.LogEventsInitialization = true")
+
+        # Restart Dymola after n_restart iterations
+        self._check_restart()
+
+        # Handle custom model_names
+        if model_names is not None:
+            # Custom model_name setting
+            _res_names = self.result_names.copy()
+            self._model_name = model_names
+            self._update_model_variables()
+            if _res_names != self.result_names:
+                self.logger.info(
+                    "Result names changed due to setting the new model. "
+                    "If you do not expect custom result names, ignore this warning."
+                    "If you do expect them, please raise an issue to add the "
+                    "option when using the model_names keyword.")
+                self.logger.info(
+                    "Difference: %s",
+                    " ,".join(list(set(_res_names).difference(self.result_names)))
+                )
+
+        # Handle parameters:
+        if parameters is None:
+            parameters = {}
+            unsupported_parameters = False
+        else:
+            unsupported_parameters = self.check_unsupported_variables(
+                variables=list(parameters.keys()),
+                type_of_var="parameters"
+            )
+
+        # Handle structural parameters
+
+        if (unsupported_parameters and
+                (self.modify_structural_parameters or
+                 structural_parameters)):
+            # Alter the model_name for the next simulation
+            model_name, parameters_new = self._alter_model_name(
+                parameters=parameters,
+                model_name=self.model_name,
+                structural_params=list(self.states.keys()) + structural_parameters
+            )
+            # Trigger translation only if something changed
+            if model_name != self.model_name:
+                _res_names = self.result_names.copy()
+                self.model_name = model_name
+                self.result_names = _res_names  # Restore previous result names
+                self.logger.warning(
+                    "Warning: Currently, the model is re-translating "
+                    "for each simulation. You should add to your Modelica "
+                    "parameters \"annotation(Evaluate=false)\".\n "
+                    "Check for these parameters: %s",
+                    ', '.join(set(parameters.keys()).difference(parameters_new.keys()))
+                )
+            parameters = parameters_new
+            # Check again
+            unsupported_parameters = self.check_unsupported_variables(
+                variables=list(parameters.keys()),
+                type_of_var="parameters"
+            )
+
+        initial_names = list(parameters.keys())
+        initial_values = list(parameters.values())
+        # Convert to float for Boolean and integer types:
+        try:
+            initial_values = [float(v) for v in initial_values]
+        except (ValueError, TypeError) as err:
+            raise TypeError("Dymola only accepts float values. "
+                            "Could bot automatically convert the given "
+                            "parameter values to float.") from err
+
+        # Handle inputs
+        if inputs is not None:
+            # Unpack additional kwargs
+            try:
+                table_name = kwargs["table_name"]
+                file_name = kwargs["file_name"]
+            except KeyError as err:
+                raise KeyError("For inputs to be used by DymolaAPI.simulate, you "
+                               "have to specify the 'table_name' and the 'file_name' "
+                               "as keyword arguments of the function. These must match"
+                               "the values 'tableName' and 'fileName' in the CombiTimeTable"
+                               " model in your modelica code.") from err
+            # Generate the input in the correct format
+            offset = self.sim_setup.start_time - inputs.index[0]
+            filepath = convert_tsd_to_modelica_txt(
+                tsd=inputs,
+                table_name=table_name,
+                save_path_file=file_name,
+                offset=offset
+            )
+            self.logger.info("Successfully created Dymola input file at %s", filepath)
+
+        if return_option == "savepath":
+            if unsupported_parameters:
+                raise KeyError("Dymola does not accept invalid parameter "
+                               "names for option return_type='savepath'. "
+                               "To use this option, delete unsupported "
+                               "parameters from your setup.")
+            res = self.dymola.simulateExtendedModel(
+                self.model_name,
+                startTime=self.sim_setup.start_time,
+                stopTime=self.sim_setup.stop_time,
+                numberOfIntervals=0,
+                outputInterval=self.sim_setup.output_interval,
+                method=self.sim_setup.solver,
+                tolerance=self.sim_setup.tolerance,
+                fixedstepsize=self.sim_setup.fixedstepsize,
+                resultFile=result_file_name,
+                initialNames=initial_names,
+                initialValues=initial_values)
+        else:
+            if not parameters and not self.parameters:
+                raise ValueError(
+                    "Sadly, simulating a model in Dymola "
+                    "with no parameters returns no result. "
+                    "Call this function using return_option='savepath' to get the results."
+                )
+            if not parameters:
+                random_name = list(self.parameters.keys())[0]
+                initial_values = [self.parameters[random_name].value]
+                initial_names = [random_name]
+
+            # Handle 1 and 2 D initial names:
+            # Convert a 1D list to 2D list
+            if initial_values and isinstance(initial_values[0], (float, int)):
+                initial_values = [initial_values]
+
+            # Handle the time of the simulation:
+            res_names = self.result_names.copy()
+            if "Time" not in res_names:
+                res_names.append("Time")
+
+            # Internally convert output Interval to number of intervals
+            # (Required by function simulateMultiResultsModel
+            number_of_intervals = (self.sim_setup.stop_time - self.sim_setup.start_time) / \
+                                  self.sim_setup.output_interval
+            if int(number_of_intervals) != number_of_intervals:
+                raise ValueError(
+                    "Given output_interval and time interval did not yield "
+                    "an integer numberOfIntervals. To use this functions "
+                    "without savepaths, you have to provide either a "
+                    "numberOfIntervals or a value for output_interval "
+                    "which can be converted to numberOfIntervals.")
+
+            res = self.dymola.simulateMultiResultsModel(
+                self.model_name,
+                startTime=self.sim_setup.start_time,
+                stopTime=self.sim_setup.stop_time,
+                numberOfIntervals=int(number_of_intervals),
+                method=self.sim_setup.solver,
+                tolerance=self.sim_setup.tolerance,
+                fixedstepsize=self.sim_setup.fixedstepsize,
+                resultFile=None,
+                initialNames=initial_names,
+                initialValues=initial_values,
+                resultNames=res_names)
+
+        if not res[0]:
+            self.logger.error("Simulation failed!")
+            self.logger.error("The last error log from Dymola:")
+            log = self.dymola.getLastErrorLog()
+            # Only print first part as output is sometimes to verbose.
+            self.logger.error(log[:10000])
+            dslog_path = os.path.join(self.cd, 'dslog.txt')
+            try:
+                with open(dslog_path, "r") as dslog_file:
+                    dslog_content = dslog_file.read()
+                    self.logger.error(dslog_content)
+            except Exception:
+                dslog_content = "Not retreivable. Open it yourself."
+            msg = f"Simulation failed: Reason according " \
+                  f"to dslog, located at '{dslog_path}': {dslog_content}"
+            if fail_on_error:
+                raise Exception(msg)
+            # Don't raise and return None
+            self.logger.error(msg)
+            return None
+
+        if return_option == "savepath":
+            _save_name_dsres = f"{result_file_name}.mat"
+            savepath = kwargs.pop("savepath", None)
+            # Get the cd of the current dymola instance
+            self.dymola.cd()
+            # Get the value and convert it to a 100 % fitting str-path
+            dymola_cd = str(pathlib.Path(self.dymola.getLastErrorLog().replace("\n", "")))
+            if savepath is None or str(savepath) == dymola_cd:
+                return os.path.join(dymola_cd, _save_name_dsres)
+            os.makedirs(savepath, exist_ok=True)
+            for filename in [_save_name_dsres, "dslog.txt", "dsfinal.txt"]:
+                # Delete existing files
+                try:
+                    os.remove(os.path.join(savepath, filename))
+                except OSError:
+                    pass
+                # Move files
+                shutil.copy(os.path.join(dymola_cd, filename),
+                            os.path.join(savepath, filename))
+                os.remove(os.path.join(dymola_cd, filename))
+            return os.path.join(savepath, _save_name_dsres)
+
+        data = res[1]  # Get data
+        if return_option == "last_point":
+            results = []
+            for ini_val_set in data:
+                results.append({result_name: ini_val_set[idx][-1] for idx, result_name
+                                in enumerate(res_names)})
+            if len(results) == 1 and squeeze:
+                return results[0]
+            return results
+        # Else return as dataframe.
+        dfs = []
+        for ini_val_set in data:
+            df = pd.DataFrame({result_name: ini_val_set[idx] for idx, result_name
+                               in enumerate(res_names)})
+            # Set time index
+            df = df.set_index("Time")
+            # Convert it to float
+            df.index = df.index.astype("float64")
+            dfs.append(df)
+        # Most of the cases, only one set is provided. In that case, avoid
+        if len(dfs) == 1 and squeeze:
+            return TimeSeriesData(dfs[0], default_tag="sim")
+        return [TimeSeriesData(df, default_tag="sim") for df in dfs]
+
+    def translate(self):
+        """
+        Translates the current model using dymola.translateModel()
+        and checks if erros occur.
+        """
+        res = self.dymola.translateModel(self.model_name)
+        if not res:
+            self.logger.error("Translation failed!")
+            self.logger.error("The last error log from Dymola:")
+            self.logger.error(self.dymola.getLastErrorLog())
+            raise Exception("Translation failed - Aborting")
+
+    def set_compiler(self, name, path, dll=False, dde=False, opc=False):
+        """
+        Set up the compiler and compiler options on Windows.
+        Optional: Specify if you want to enable dll, dde or opc.
+
+        :param str name:
+            Name of the compiler, avaiable options:
+            - 'vs': Visual Studio
+            - 'gcc': GCC
+        :param str,os.path.normpath path:
+            Path to the compiler files.
+            Example for name='vs': path='C:/Program Files (x86)/Microsoft Visual Studio 10.0/Vc'
+            Example for name='gcc': path='C:/MinGW/bin/gcc'
+        :param Boolean dll:
+            Set option for dll support. Check Dymolas Manual on what this exactly does.
+        :param Boolean dde:
+            Set option for dde support. Check Dymolas Manual on what this exactly does.
+        :param Boolean opc:
+            Set option for opc support. Check Dymolas Manual on what this exactly does.
+        :return: True, on success.
+        """
+        # Lookup dict for internal name of CCompiler-Variable
+        _name_int = {"vs": "MSVC",
+                     "gcc": "GCC"}
+
+        if "win" not in sys.platform:
+            raise OSError(f"set_compiler function only implemented "
+                          f"for windows systems, you are using {sys.platform}")
+        # Manually check correct input as Dymola's error are not a help
+        name = name.lower()
+        if name not in ["vs", "gcc"]:
+            raise ValueError(f"Given compiler name {name} not supported.")
+        if not os.path.exists(path):
+            raise FileNotFoundError(f"Given compiler path {path} does not exist on your machine.")
+        # Convert path for correct input
+        path = self._make_modelica_normpath(path)
+        if self.use_mp:
+            raise ValueError("Given function is not yet supported for multiprocessing")
+
+        res = self.dymola.SetDymolaCompiler(name.lower(),
+                                            [f"CCompiler={_name_int[name]}",
+                                             f"{_name_int[name]}DIR={path}",
+                                             f"DLL={int(dll)}",
+                                             f"DDE={int(dde)}",
+                                             f"OPC={int(opc)}"])
+
+        return res
+
+    def import_initial(self, filepath):
+        """
+        Load given dsfinal.txt into dymola
+
+        :param str,os.path.normpath filepath:
+            Path to the dsfinal.txt to be loaded
+        """
+        if not os.path.isfile(filepath):
+            raise FileNotFoundError(f"Given filepath {filepath} does not exist")
+        if not os.path.splitext(filepath)[1] == ".txt":
+            raise TypeError('File is not of type .txt')
+        if self.use_mp:
+            raise ValueError("Given function is not yet supported for multiprocessing")
+        res = self.dymola.importInitial(dsName=filepath)
+        if res:
+            self.logger.info("Successfully loaded dsfinal.txt")
+        else:
+            raise Exception("Could not load dsfinal into Dymola.")
+
+    @SimulationAPI.cd.setter
+    def cd(self, cd):
+        """Set the working directory to the given path"""
+        self._cd = cd
+        if self.dymola is None:  # Not yet started
+            return
+        # Also set the cd in the dymola api
+        self.set_dymola_cd(dymola=self.dymola,
+                           cd=cd)
+        if self.use_mp:
+            self.logger.warning("Won't set the cd for all workers, "
+                                "not yet implemented.")
+
+    def set_dymola_cd(self, dymola, cd):
+        """
+        Set the cd of the Dymola Instance.
+        Before calling the Function, create the path and
+        convert to a modelica-normpath.
+        """
+        os.makedirs(cd, exist_ok=True)
+        cd_modelica = self._make_modelica_normpath(path=cd)
+        res = dymola.cd(cd_modelica)
+        if not res:
+            raise OSError(f"Could not change working directory to {cd}")
+
+    def close(self):
+        """Closes dymola."""
+        # Close MP of super class
+        super().close()
+        # Always close main instance
+        self._single_close(dymola=self.dymola)
+
+    def _close_multiprocessing(self, _):
+        self._single_close()
+        DymolaAPI.dymola = None
+
+    def _single_close(self, **kwargs):
+        """Closes a single dymola instance"""
+        if self.dymola is None:
+            return  # Already closed prior
+        # Execute the mos-script if given:
+        if self.mos_script_post is not None:
+            self.logger.info("Executing given mos_script_post "
+                             "prior to closing.")
+            self.dymola.RunScript(self.mos_script_post)
+            self.logger.info("Output of mos_script_post: %s", self.dymola.getLastErrorLog())
+        self.logger.info('Closing Dymola')
+        self.dymola.close()
+        self.logger.info('Successfully closed Dymola')
+        self.dymola = None
+
+    def _close_dummy(self):
+        """
+        Closes dummy instance at the end of the execution
+        """
+        if self._dummy_dymola_instance is not None:
+            self.logger.info('Closing dummy Dymola instance')
+            self._dummy_dymola_instance.close()
+            self.logger.info('Successfully closed dummy Dymola instance')
+
+    def extract_model_variables(self):
+        """
+        Extract all variables of the model by
+        translating it and then processing the dsin
+        using the manipulate_ds module.
+        """
+        # Translate model
+        self.logger.info("Translating model '%s' to extract model variables ",
+                         self.model_name)
+        self.translate()
+        # Get path to dsin:
+        dsin_path = os.path.join(self.cd, "dsin.txt")
+        df = manipulate_ds.convert_ds_file_to_dataframe(dsin_path)
+        # Convert and return all parameters of dsin to initial values and names
+        for idx, row in df.iterrows():
+            _max = float(row["4"])
+            _min = float(row["3"])
+            if _min >= _max:
+                _var_ebcpy = Variable(value=float(row["2"]))
+            else:
+                _var_ebcpy = Variable(
+                    min=_min,
+                    max=_max,
+                    value=float(row["2"])
+                )
+            if row["5"] == "1":
+                self.parameters[idx] = _var_ebcpy
+            elif row["5"] == "5":
+                self.inputs[idx] = _var_ebcpy
+            elif row["5"] == "4":
+                self.outputs[idx] = _var_ebcpy
+            else:
+                self.states[idx] = _var_ebcpy
+
+    def _setup_dymola_interface(self, use_mp):
+        """Load all packages and change the current working directory"""
+        dymola = self._open_dymola_interface()
+        self._check_dymola_instances()
+        if use_mp:
+            cd = os.path.join(self.cd, f"worker_{self.worker_idx}")
+        else:
+            cd = self.cd
+        # Execute the mos-script if given:
+        if self.mos_script_pre is not None:
+            self.logger.info("Executing given mos_script_pre "
+                             "prior to loading packages.")
+            dymola.RunScript(self.mos_script_pre)
+            self.logger.info("Output of mos_script_pre: %s", dymola.getLastErrorLog())
+
+        # Set the cd in the dymola api
+        self.set_dymola_cd(dymola=dymola, cd=cd)
+
+        for package in self.packages:
+            self.logger.info("Loading Model %s", os.path.dirname(package).split("\\")[-1])
+            res = dymola.openModel(package, changeDirectory=False)
+            if not res:
+                raise ImportError(dymola.getLastErrorLog())
+        self.logger.info("Loaded modules")
+        if self.equidistant_output:
+            # Change the Simulation Output, to ensure all
+            # simulation results have the same array shape.
+            # Events can also cause errors in the shape.
+            dymola.experimentSetupOutput(equidistant=True,
+                                         events=False)
+        if not dymola.RequestOption("Standard"):
+            warnings.warn("You have no licence to use Dymola. "
+                          "Hence you can only simulate models with 8 or less equations.")
+        if use_mp:
+            DymolaAPI.dymola = dymola
+            return None
+        return dymola
+
+    def _open_dymola_interface(self):
+        """Open an instance of dymola and return the API-Object"""
+        if self.dymola_interface_path not in sys.path:
+            sys.path.insert(0, self.dymola_interface_path)
+        try:
+            from dymola.dymola_interface import DymolaInterface
+            from dymola.dymola_exception import DymolaConnectionException
+            return DymolaInterface(showwindow=self.show_window,
+                                   dymolapath=self.dymola_exe_path)
+        except ImportError as error:
+            raise ImportError("Given dymola-interface could not be "
+                              "loaded:\n %s" % self.dymola_interface_path) from error
+        except DymolaConnectionException as error:
+            raise ConnectionError(error) from error
+
+    def to_dict(self):
+        """
+        Store the most relevant information of this class
+        into a dictionary. This may be used for future configuration.
+
+        :return: dict config:
+            Dictionary with keys to re-init this class.
+        """
+        # Convert Path to str to enable json-dumping
+        config = {"cd": str(self.cd),
+                  "packages": [str(pack) for pack in self.packages],
+                  "model_name": self.model_name,
+                  "type": "DymolaAPI",
+                  }
+        # Update kwargs
+        config.update({kwarg: self.__dict__.get(kwarg, None)
+                       for kwarg in self._supported_kwargs})
+
+        return config
+
+    def get_packages(self):
+        """
+        Get the currently loaded packages of Dymola
+        """
+        packages = self.dymola.ExecuteCommand(
+            'ModelManagement.Structure.AST.Misc.ClassesInPackage("")'
+        )
+        if packages is None:
+            self.logger.error("Could not load packages from Dymola, using self.packages")
+            packages = []
+            for pack in self.packages:
+                pack = pathlib.Path(pack)
+                if pack.name == "package.mo":
+                    packages.append(pack.parent.name)
+        valid_packages = []
+        for pack in packages:
+            current_package = f"modelica://{pack}/package.order"
+            pack_path = self.dymola.ExecuteCommand(
+                f'Modelica.Utilities.Files.loadResource("{current_package}")'
+            )
+            if not isinstance(pack_path, str):
+                self.logger.error("Could not load model resource for package %s", pack)
+            if os.path.isfile(pack_path):
+                valid_packages.append(pathlib.Path(pack_path).parent)
+        return valid_packages
+
+    def save_for_reproduction(
+            self,
+            title: str,
+            path: pathlib.Path = None,
+            files: list = None,
+            save_total_model: bool = True,
+            export_fmu: bool = True,
+            **kwargs
+    ):
+        """
+        Additionally to the basic reproduction, add info
+        for Dymola packages.
+
+        Content which is saved:
+        - DymolaAPI configuration
+        - Information on Dymola: Version, flags
+        - All loaded packages
+        - Total model, if save_total_model = True
+        - FMU, if export_fmu = True
+
+        :param bool save_total_model:
+            True to save the total model
+        :param bool export_fmu:
+            True to export the FMU of the current model.
+        """
+        # Local import to require git-package only when called
+        from ebcpy.utils.reproduction import ReproductionFile, CopyFile, get_git_information
+
+        if files is None:
+            files = []
+        # DymolaAPI Info:
+        files.append(ReproductionFile(
+            filename="Dymola/DymolaAPI_config.json",
+            content=json.dumps(self.to_dict(), indent=2)
+        ))
+        # Dymola info:
+        self.dymola.ExecuteCommand("list();")
+        _flags = self.dymola.getLastErrorLog()
+        dymola_info = [
+            self.dymola.ExecuteCommand("DymolaVersion()"),
+            str(self.dymola.ExecuteCommand("DymolaVersionNumber()")),
+            "\n\n"
+        ]
+        files.append(ReproductionFile(
+            filename="Dymola/DymolaInfo.txt",
+            content="\n".join(dymola_info) + _flags
+        ))
+
+        # Packages
+        packages = self.get_packages()
+        package_infos = []
+        for pack_path in packages:
+
+            for pack_dir_parent in [pack_path] + list(pack_path.parents):
+                repo_info = get_git_information(
+                    path=pack_dir_parent,
+                    zip_folder_path="Dymola"
+                )
+                if not repo_info:
+                    continue
+
+                files.extend(repo_info.pop("difference_files"))
+                pack_path = str(pack_path) + "; " + "; ".join([f"{key}: {value}" for key, value in repo_info.items()])
+                break
+            package_infos.append(str(pack_path))
+        files.append(ReproductionFile(
+            filename="Dymola/Modelica_packages.txt",
+            content="\n".join(package_infos)
+        ))
+        # Total model
+        if save_total_model:
+            _total_model_name = f"Dymola/{self.model_name.replace('.', '_')}_total.mo"
+            _total_model = pathlib.Path(self.cd).joinpath(_total_model_name)
+            os.makedirs(_total_model.parent, exist_ok=True)  # Create to ensure model can be saved.
+            res = self.dymola.saveTotalModel(
+                fileName=str(_total_model),
+                modelName=self.model_name
+            )
+            if res:
+                files.append(ReproductionFile(
+                    filename=_total_model_name,
+                    content=_total_model.read_text()
+                ))
+                os.remove(_total_model)
+            else:
+                self.logger.error("Could not save total model: %s",
+                                  self.dymola.getLastErrorLog())
+        # FMU
+        if export_fmu:
+            _fmu_path = self._save_to_fmu(fail_on_error=False)
+            if _fmu_path is not None:
+                files.append(CopyFile(
+                    sourcepath=_fmu_path,
+                    filename="Dymola/" + _fmu_path.name,
+                    remove=True
+                ))
+
+        return super().save_for_reproduction(
+            title=title,
+            path=path,
+            files=files,
+            **kwargs
+        )
+
+    def _save_to_fmu(self, fail_on_error):
+        """Save model as an FMU"""
+        res = self.dymola.translateModelFMU(
+            modelToOpen=self.model_name,
+            storeResult=False,
+            modelName='',
+            fmiVersion='2',
+            fmiType='all',
+            includeSource=False,
+            includeImage=0
+        )
+        if not res:
+            msg = "Could not export fmu: %s" % self.dymola.getLastErrorLog()
+            self.logger.error(msg)
+            if fail_on_error:
+                raise Exception(msg)
+        else:
+            path = pathlib.Path(self.cd).joinpath(res + ".fmu")
+            return path
+
+    @staticmethod
+    def _make_modelica_normpath(path):
+        """
+        Convert given path to a path readable in dymola.
+        If the base path does not exist, create it.
+
+        :param str,os.path.normpath path:
+            Either a file or a folder path. The base to this
+            path is created in non existent.
+        :return: str
+            Path readable in dymola
+        """
+        if isinstance(path, pathlib.Path):
+            path = str(path)
+
+        path = path.replace("\\", "/")
+        # Search for e.g. "D:testzone" and replace it with D:/testzone
+        loc = path.find(":")
+        if path[loc + 1] != "/" and loc != -1:
+            path = path.replace(":", ":/")
+        return path
+
+    @staticmethod
+    def get_dymola_interface_path(dymola_install_dir):
+        """
+        Function to get the path of the newest dymola interface
+        installment on the used machine
+
+        :param str dymola_install_dir:
+            The dymola installation folder. Example:
+            "C://Program Files//Dymola 2020"
+        :return: str
+            Path to the dymola.egg-file
+        """
+        path_to_egg_file = os.path.normpath("Modelica/Library/python_interface/dymola.egg")
+        egg_file = os.path.join(dymola_install_dir, path_to_egg_file)
+        if not os.path.isfile(egg_file):
+            raise FileNotFoundError(f"The given dymola installation directory "
+                                    f"'{dymola_install_dir}' has no "
+                                    f"dymola-interface egg-file.")
+        return egg_file
+
+    @staticmethod
+    def get_dymola_path(dymola_install_dir, dymola_name=None):
+        """
+        Function to get the path of the dymola exe-file
+        on the current used machine.
+
+        :param str dymola_install_dir:
+            The dymola installation folder. Example:
+            "C://Program Files//Dymola 2020"
+        :param str dymola_name:
+            Name of the executable. On Windows it is always Dymola.exe, on
+            linux just dymola.
+        :return: str
+            Path to the dymola-exe-file.
+        """
+        if dymola_name is None:
+            if "linux" in sys.platform:
+                dymola_name = "dymola"
+            elif "win" in sys.platform:
+                dymola_name = "Dymola.exe"
+            else:
+                raise OSError(f"Your operating system {sys.platform} has no default dymola-name."
+                              f"Please provide one.")
+
+        bin_64 = os.path.join(dymola_install_dir, "bin64", dymola_name)
+        bin_32 = os.path.join(dymola_install_dir, "bin", dymola_name)
+        if os.path.isfile(bin_64):  # First check for 64bit installation
+            dym_file = bin_64
+        elif os.path.isfile(bin_32):  # Else use the 32bit version
+            dym_file = bin_32
+        else:
+            raise FileNotFoundError(
+                f"The given dymola installation has not executable at '{bin_32}'. "
+                f"If your dymola_path exists, please raise an issue."
+            )
+
+        return dym_file
+
+    @staticmethod
+    def get_dymola_install_paths(basedir=None):
+        """
+        Function to get all paths of dymola installations
+        on the used machine. Supported platforms are:
+        * Windows
+        * Linux
+        * Mac OS X
+        If multiple installation of Dymola are found, the newest version will be returned.
+        This assumes the names are sortable, e.g. Dymola 2020, Dymola 2019 etc.
+
+        :param str basedir:
+            The base-directory to search for the dymola-installation.
+            The default value depends on the platform one is using.
+            On Windows it is "C://Program Files" or "C://Program Files (x86)" (for 64 bit)
+            On Linux it is "/opt" (based on our ci-Docker configuration
+            On Mac OS X "/Application" (based on the default)
+        :return: str
+            Path to the dymola-installation
+        """
+
+        if basedir is None:
+            if "linux" in sys.platform:
+                basedir = os.path.normpath("/opt")
+            elif "win" in sys.platform:
+                basedir = os.path.normpath("C:/Program Files")
+            elif "darwin" in sys.platform:
+                basedir = os.path.normpath("/Applications")
+            else:
+                raise OSError(f"Your operating system ({sys.platform})does not support "
+                              f"a default basedir. Please provide one.")
+
+        syspaths = [basedir]
+        # Check if 64bit is installed (Windows only)
+        systempath_64 = os.path.normpath("C://Program Files (x86)")
+        if os.path.exists(systempath_64):
+            syspaths.append(systempath_64)
+        # Get all folders in both path's
+        temp_list = []
+        for systempath in syspaths:
+            temp_list += os.listdir(systempath)
+        # Filter programs that are not Dymola
+        dym_versions = []
+        for folder_name in temp_list:
+            # Catch both Dymola and dymola folder-names
+            if "dymola" in folder_name.lower():
+                dym_versions.append(folder_name)
+        del temp_list
+        # Find the newest version and return the egg-file
+        # This sorting only works with a good Folder structure, eg. Dymola 2020, Dymola 2019 etc.
+        dym_versions.sort()
+        valid_paths = []
+        for dym_version in reversed(dym_versions):
+            for system_path in syspaths:
+                full_path = os.path.join(system_path, dym_version)
+                if os.path.isdir(full_path):
+                    valid_paths.append(full_path)
+        return valid_paths
+
+    def _check_dymola_instances(self):
+        """
+        Check how many dymola instances are running on the machine.
+        Raise a warning if the number exceeds a certain amount.
+        """
+        # The option may be useful. However the explicit requirement leads to
+        # Problems on linux, therefore the feature is not worth the trouble.
+        # pylint: disable=import-outside-toplevel
+        try:
+            import psutil
+        except ImportError:
+            return
+        counter = 0
+        for proc in psutil.process_iter():
+            try:
+                if "Dymola" in proc.name():
+                    counter += 1
+            except psutil.AccessDenied:
+                continue
+        if counter >= self._critical_number_instances:
+            warnings.warn("There are currently %s Dymola-Instances "
+                          "running on your machine!" % counter)
+
+    @staticmethod
+    def _alter_model_name(parameters, model_name, structural_params):
+        """
+        Creates a modifier for all structural parameters,
+        based on the modelname and the initalNames and values.
+
+        :param dict parameters:
+            Parameters of the simulation
+        :param str model_name:
+            Name of the model to be modified
+        :param list structural_params:
+            List of strings with structural parameters
+        :return: str altered_modelName:
+            modified model name
+        """
+        # the structural parameter needs to be removed from paramters dict
+        new_parameters = parameters.copy()
+        model_name = model_name.split("(")[0]  # Trim old modifier
+        if parameters == {}:
+            return model_name
+        all_modifiers = []
+        for var_name, value in parameters.items():
+            # Check if the variable is in the
+            # given list of structural parameters
+            if var_name in structural_params:
+                all_modifiers.append(f"{var_name}={value}")
+                # removal of the structural parameter
+                new_parameters.pop(var_name)
+        altered_model_name = f"{model_name}({','.join(all_modifiers)})"
+        return altered_model_name, new_parameters
+
+    def _check_restart(self):
+        """Restart Dymola every n_restart iterations in order to free memory"""
+
+        if self.sim_counter == self.n_restart:
+            self.logger.info("Closing and restarting Dymola to free memory")
+            self.close()
+            self._dummy_dymola_instance = self._setup_dymola_interface(use_mp=False)
+            self.sim_counter = 1
+        else:
+            self.sim_counter += 1
```

### Comparing `ebcpy-0.3.2/ebcpy/simulationapi/fmu.py` & `ebcpy-0.3.6/ebcpy/simulationapi/fmu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,398 +1,406 @@
-"""Module for classes using a fmu to
-simulate models."""
-
-import os
-import logging
-import pathlib
-import atexit
-import shutil
-from typing import List, Union
-
-import fmpy
-from fmpy.model_description import read_model_description
-from pydantic import Field
-import pandas as pd
-import numpy as np
-
-from ebcpy import simulationapi, TimeSeriesData
-from ebcpy.simulationapi import SimulationSetup, SimulationSetupClass, Variable
-from ebcpy.utils.reproduction import CopyFile
-
-# pylint: disable=broad-except
-
-
-class FMU_Setup(SimulationSetup):
-    """
-    Add's custom setup parameters for simulating FMU's
-    to the basic `SimulationSetup`
-    """
-
-    timeout: float = Field(
-        title="timeout",
-        default=np.inf,
-        description="Timeout after which the simulation stops."
-    )
-
-    _default_solver = "CVode"
-    _allowed_solvers = ["CVode", "Euler"]
-
-
-class FMU_API(simulationapi.SimulationAPI):
-    """
-    Class for simulation using the fmpy library and
-    a functional mockup interface as a model input.
-
-    :keyword bool log_fmu:
-        Whether to print fmu messages or not.
-
-    Example:
-
-    >>> import matplotlib.pyplot as plt
-    >>> from ebcpy import FMU_API
-    >>> # Select any valid fmu. Replace the line below if
-    >>> # you don't have this file on your device.
-    >>> model_name = "Path to your fmu"
-    >>> fmu_api = FMU_API(model_name)
-    >>> fmu_api.sim_setup = {"stop_time": 3600}
-    >>> result_df = fmu_api.simulate()
-    >>> fmu_api.close()
-    >>> # Select an exemplary column
-    >>> col = result_df.columns[0]
-    >>> plt.plot(result_df[col], label=col)
-    >>> _ = plt.legend()
-    >>> _ = plt.show()
-
-    .. versionadded:: 0.1.7
-    """
-    _items_to_drop = ["pool", "_fmu_instance", "_unzip_dir"]
-    _fmu_instance = None
-    _unzip_dir: str = None
-    _sim_setup_class: SimulationSetupClass = FMU_Setup
-    _type_map = {
-        float: np.double,
-        bool: np.bool_,
-        int: np.int_
-    }
-
-    def __init__(self, cd, model_name, **kwargs):
-        """Instantiate class parameters"""
-        # Init instance attributes
-        self._model_description = None
-        self._fmi_type = None
-        self._unzip_dir = None
-        self._fmu_instance = None
-        self.log_fmu = kwargs.get("log_fmu", True)
-        self._single_unzip_dir: str = None
-
-        if isinstance(model_name, pathlib.Path):
-            model_name = str(model_name)
-        if not model_name.lower().endswith(".fmu"):
-            raise ValueError(f"{model_name} is not a valid fmu file!")
-        if cd is None:
-            cd = os.path.dirname(model_name)
-        super().__init__(cd, model_name, **kwargs)
-        # Register exit option
-        atexit.register(self.close)
-
-    def _update_model(self):
-        # Setup the fmu instance
-        self.setup_fmu_instance()
-
-    def close(self):
-        """
-        Closes the fmu.
-
-        :return: bool
-            True on success
-        """
-        # Close MP of super class
-        super().close()
-        # Close if single process
-        if not self.use_mp:
-            if not self._fmu_instance:
-                return  # Already closed
-            self._single_close(fmu_instance=self._fmu_instance,
-                               unzip_dir=self._unzip_dir)
-            self._unzip_dir = None
-            self._fmu_instance = None
-
-    def _single_close(self, **kwargs):
-        fmu_instance = kwargs["fmu_instance"]
-        unzip_dir = kwargs["unzip_dir"]
-        try:
-            fmu_instance.terminate()
-        except Exception as error:  # This is due to fmpy which does not yield a narrow error
-            self.logger.error(f"Could not terminate fmu instance: {error}")
-        try:
-            fmu_instance.freeInstance()
-        except OSError as error:
-            self.logger.error(f"Could not free fmu instance: {error}")
-        # Remove the extracted files
-        if unzip_dir is not None:
-            try:
-                shutil.rmtree(unzip_dir)
-            except FileNotFoundError:
-                pass  # Nothing to delete
-            except PermissionError:
-                self.logger.error("Could not delete unzipped fmu "
-                                  "in location %s. Delete it yourself.", unzip_dir)
-
-    def _close_multiprocessing(self, _):
-        """Small helper function"""
-        idx_worker = self.worker_idx
-        if self._fmu_instance is None:
-            return  # Already closed
-        self.logger.error(f"Closing fmu for worker {idx_worker}")
-        self._single_close(fmu_instance=self._fmu_instance,
-                           unzip_dir=self._unzip_dir)
-        self._unzip_dir = None
-        self._fmu_instance = None
-        FMU_API._unzip_dir = None
-        FMU_API._fmu_instance = None
-
-    def simulate(self,
-                 parameters: Union[dict, List[dict]] = None,
-                 return_option: str = "time_series",
-                 **kwargs):
-        """
-        Perform the single simulation for the given
-        unzip directory and fmu_instance.
-        See the docstring of simulate() for information on kwargs.
-
-        Additional kwargs:
-        :keyword str result_file_suffix:
-            Suffix of the result file. Supported options can be extracted
-            from the TimeSeriesData.save() function.
-            Default is 'csv'.
-        """
-        return super().simulate(parameters=parameters, return_option=return_option, **kwargs)
-
-    def _single_simulation(self, kwargs):
-        """
-        Perform the single simulation for the given
-        unzip directory and fmu_instance.
-        See the docstring of simulate() for information on kwargs.
-
-        The single argument kwarg is to make this
-        function accessible by multiprocessing pool.map.
-        """
-        # Unpack kwargs:
-        parameters = kwargs.pop("parameters", None)
-        return_option = kwargs.pop("return_option", "time_series")
-        inputs = kwargs.get("inputs", None)
-        fail_on_error = kwargs.get("fail_on_error", True)
-
-        if self.use_mp:
-            if self._fmu_instance is None:
-                self._setup_single_fmu_instance(use_mp=True)
-
-        if inputs is not None:
-            if not isinstance(inputs, (TimeSeriesData, pd.DataFrame)):
-                raise TypeError("DataFrame or TimeSeriesData object expected for inputs.")
-            inputs = inputs.copy()  # Create save copy
-            if isinstance(inputs, TimeSeriesData):
-                inputs = inputs.to_df(force_single_index=True)
-            if "time" in inputs.columns:
-                raise IndexError(
-                    "Given inputs contain a column named 'time'. "
-                    "The index is assumed to contain the time-information."
-                )
-            # Convert df to structured numpy array for fmpy: simulate_fmu
-            inputs.insert(0, column="time", value=inputs.index)
-            inputs_tuple = [tuple(columns) for columns in inputs.to_numpy()]
-            # Try to match the type, default is np.double.
-            # 'time' is not in inputs and thus handled separately.
-            dtype = [(inputs.columns[0], np.double)] + \
-                    [(col,
-                      self._type_map.get(self.inputs[col].type, np.double)
-                      ) for col in inputs.columns[1:]]
-            inputs = np.array(inputs_tuple, dtype=dtype)
-        if parameters is None:
-            parameters = {}
-        else:
-            self.check_unsupported_variables(variables=list(parameters.keys()),
-                                             type_of_var="parameters")
-        try:
-            # reset the FMU instance instead of creating a new one
-            self._fmu_instance.reset()
-            # Simulate
-            res = fmpy.simulate_fmu(
-                filename=self._unzip_dir,
-                start_time=self.sim_setup.start_time,
-                stop_time=self.sim_setup.stop_time,
-                solver=self.sim_setup.solver,
-                step_size=self.sim_setup.fixedstepsize,
-                relative_tolerance=None,
-                output_interval=self.sim_setup.output_interval,
-                record_events=False,  # Used for an equidistant output
-                start_values=parameters,
-                apply_default_start_values=False,  # As we pass start_values already
-                input=inputs,
-                output=self.result_names,
-                timeout=self.sim_setup.timeout,
-                step_finished=None,
-                model_description=self._model_description,
-                fmu_instance=self._fmu_instance,
-                fmi_type=self._fmi_type,
-            )
-
-        except Exception as error:
-            self.logger.error(f"[SIMULATION ERROR] Error occurred while running FMU: \n {error}")
-            if fail_on_error:
-                raise error
-            return None
-
-        # Reshape result:
-        df = pd.DataFrame(res).set_index("time")
-        df.index = np.round(df.index.astype("float64"),
-                            str(self.sim_setup.output_interval)[::-1].find('.'))
-
-        if return_option == "savepath":
-            result_file_name = kwargs.get("result_file_name", "resultFile")
-            result_file_suffix = kwargs.get("result_file_suffix", "csv")
-            savepath = kwargs.get("savepath", None)
-
-            if savepath is None:
-                savepath = self.cd
-
-            os.makedirs(savepath, exist_ok=True)
-            filepath = os.path.join(savepath, f"{result_file_name}.{result_file_suffix}")
-            TimeSeriesData(df).droplevel(1, axis=1).save(
-                filepath=filepath,
-                key="simulation"
-            )
-
-            return filepath
-        if return_option == "last_point":
-            return df.iloc[-1].to_dict()
-        # Else return time series data
-        tsd = TimeSeriesData(df, default_tag="sim")
-        return tsd
-
-    def setup_fmu_instance(self):
-        """
-        Manually set up and extract the data to
-        avoid this step in the simulate function.
-        """
-        self.logger.info("Extracting fmu and reading fmu model description")
-        # First load model description and extract variables
-        self._single_unzip_dir = os.path.join(self.cd,
-                                              os.path.basename(self.model_name)[:-4] + "_extracted")
-        os.makedirs(self._single_unzip_dir, exist_ok=True)
-        self._single_unzip_dir = fmpy.extract(self.model_name,
-                                              unzipdir=self._single_unzip_dir)
-        self._model_description = read_model_description(self._single_unzip_dir,
-                                                         validate=True)
-
-        if self._model_description.coSimulation is None:
-            self._fmi_type = 'ModelExchange'
-        else:
-            self._fmi_type = 'CoSimulation'
-
-        self.logger.info("Reading model variables")
-
-        _types = {
-            "Enumeration": int,
-            "Integer": int,
-            "Real": float,
-            "Boolean": bool,
-            "String": str
-        }
-        # Extract inputs, outputs & tuner (lists from parent classes will be appended)
-        for var in self._model_description.modelVariables:
-            if var.start is not None:
-                var.start = _types[var.type](var.start)
-
-            _var_ebcpy = Variable(
-                min=var.min,
-                max=var.max,
-                value=var.start,
-                type=_types[var.type]
-            )
-            if var.causality == 'input':
-                self.inputs[var.name] = _var_ebcpy
-            elif var.causality == 'output':
-                self.outputs[var.name] = _var_ebcpy
-            elif var.causality == 'parameter' or var.causality == 'calculatedParameter':
-                self.parameters[var.name] = _var_ebcpy
-            elif var.causality == 'local':
-                self.states[var.name] = _var_ebcpy
-            else:
-                self.logger.error(f"Could not map causality {var.causality}"
-                                  f" to any variable type.")
-
-        if self.use_mp:
-            self.logger.info("Extracting fmu %s times for "
-                             "multiprocessing on %s processes",
-                             self.n_cpu, self.n_cpu)
-            self.pool.map(
-                self._setup_single_fmu_instance,
-                [True for _ in range(self.n_cpu)]
-            )
-            self.logger.info("Instantiated fmu's on all processes.")
-        else:
-            self._setup_single_fmu_instance(use_mp=False)
-
-    def _setup_single_fmu_instance(self, use_mp):
-        if use_mp:
-            wrk_idx = self.worker_idx
-            if self._fmu_instance is not None:
-                return True
-            unzip_dir = self._single_unzip_dir + f"_worker_{wrk_idx}"
-            fmpy.extract(self.model_name,
-                         unzipdir=unzip_dir)
-        else:
-            wrk_idx = 0
-            unzip_dir = self._single_unzip_dir
-
-        self.logger.info("Instantiating fmu for worker %s", wrk_idx)
-        fmu_instance = fmpy.instantiate_fmu(
-            unzipdir=unzip_dir,
-            model_description=self._model_description,
-            fmi_type=self._fmi_type,
-            visible=False,
-            debug_logging=False,
-            logger=self._custom_logger,
-            fmi_call_logger=None)
-        if use_mp:
-            FMU_API._fmu_instance = fmu_instance
-            FMU_API._unzip_dir = unzip_dir
-        else:
-            self._fmu_instance = fmu_instance
-            self._unzip_dir = unzip_dir
-        return True
-
-    def _custom_logger(self, component, instanceName, status, category, message):
-        """ Print the FMU's log messages to the command line (works for both FMI 1.0 and 2.0) """
-        # pylint: disable=unused-argument, invalid-name
-        label = ['OK', 'WARNING', 'DISCARD', 'ERROR', 'FATAL', 'PENDING'][status]
-        _level_map = {'OK': logging.INFO,
-                      'WARNING': logging.WARNING,
-                      'DISCARD': logging.WARNING,
-                      'ERROR': logging.ERROR,
-                      'FATAL': logging.FATAL,
-                      'PENDING': logging.FATAL}
-        if self.log_fmu:
-            self.logger.log(level=_level_map[label], msg=message.decode("utf-8"))
-
-    def save_for_reproduction(self,
-                              title: str,
-                              path: pathlib.Path = None,
-                              files: list = None,
-                              **kwargs):
-        """
-        Additionally to the basic reproduction, add info
-        for FMU files.
-        """
-        if files is None:
-            files = []
-        files.append(CopyFile(
-            filename="FMU/" + pathlib.Path(self.model_name).name,
-            sourcepath=pathlib.Path(self.model_name),
-            remove=False
-        ))
-        return super().save_for_reproduction(
-            title=title,
-            path=path,
-            files=files
-        )
+"""Module for classes using a fmu to
+simulate models."""
+
+import os
+import logging
+import pathlib
+import atexit
+import shutil
+from typing import List, Union
+
+import fmpy
+from fmpy.model_description import read_model_description
+from pydantic import Field
+import pandas as pd
+import numpy as np
+
+from ebcpy import simulationapi, TimeSeriesData
+from ebcpy.simulationapi import SimulationSetup, SimulationSetupClass, Variable
+from ebcpy.utils.reproduction import CopyFile
+
+# pylint: disable=broad-except
+
+
+class FMU_Setup(SimulationSetup):
+    """
+    Add's custom setup parameters for simulating FMU's
+    to the basic `SimulationSetup`
+    """
+
+    timeout: float = Field(
+        title="timeout",
+        default=np.inf,
+        description="Timeout after which the simulation stops."
+    )
+
+    _default_solver = "CVode"
+    _allowed_solvers = ["CVode", "Euler"]
+
+
+class FMU_API(simulationapi.SimulationAPI):
+    """
+    Class for simulation using the fmpy library and
+    a functional mockup interface as a model input.
+
+    :keyword bool log_fmu:
+        Whether to print fmu messages or not.
+
+    Example:
+
+    >>> import matplotlib.pyplot as plt
+    >>> from ebcpy import FMU_API
+    >>> # Select any valid fmu. Replace the line below if
+    >>> # you don't have this file on your device.
+    >>> model_name = "Path to your fmu"
+    >>> fmu_api = FMU_API(model_name)
+    >>> fmu_api.sim_setup = {"stop_time": 3600}
+    >>> result_df = fmu_api.simulate()
+    >>> fmu_api.close()
+    >>> # Select an exemplary column
+    >>> col = result_df.columns[0]
+    >>> plt.plot(result_df[col], label=col)
+    >>> _ = plt.legend()
+    >>> _ = plt.show()
+
+    .. versionadded:: 0.1.7
+    """
+    _items_to_drop = ["pool", "_fmu_instance", "_unzip_dir"]
+    _fmu_instance = None
+    _unzip_dir: str = None
+    _sim_setup_class: SimulationSetupClass = FMU_Setup
+    _type_map = {
+        float: np.double,
+        bool: np.bool_,
+        int: np.int_
+    }
+
+    def __init__(self, cd, model_name, **kwargs):
+        """Instantiate class parameters"""
+        # Init instance attributes
+        self._model_description = None
+        self._fmi_type = None
+        self._unzip_dir = None
+        self._fmu_instance = None
+        self.log_fmu = kwargs.get("log_fmu", True)
+        self._single_unzip_dir: str = None
+
+        if isinstance(model_name, pathlib.Path):
+            model_name = str(model_name)
+        if not model_name.lower().endswith(".fmu"):
+            raise ValueError(f"{model_name} is not a valid fmu file!")
+        if cd is None:
+            cd = os.path.dirname(model_name)
+        super().__init__(cd, model_name, **kwargs)
+        # Register exit option
+        atexit.register(self.close)
+
+    def _update_model(self):
+        # Setup the fmu instance
+        self.setup_fmu_instance()
+
+    def close(self):
+        """
+        Closes the fmu.
+
+        :return: bool
+            True on success
+        """
+        # Close MP of super class
+        super().close()
+        # Close if single process
+        if not self.use_mp:
+            if not self._fmu_instance:
+                return  # Already closed
+            self._single_close(fmu_instance=self._fmu_instance,
+                               unzip_dir=self._unzip_dir)
+            self._unzip_dir = None
+            self._fmu_instance = None
+
+    def _single_close(self, **kwargs):
+        fmu_instance = kwargs["fmu_instance"]
+        unzip_dir = kwargs["unzip_dir"]
+        try:
+            fmu_instance.terminate()
+        except Exception as error:  # This is due to fmpy which does not yield a narrow error
+            self.logger.error(f"Could not terminate fmu instance: {error}")
+        try:
+            fmu_instance.freeInstance()
+        except OSError as error:
+            self.logger.error(f"Could not free fmu instance: {error}")
+        # Remove the extracted files
+        if unzip_dir is not None:
+            try:
+                shutil.rmtree(unzip_dir)
+            except FileNotFoundError:
+                pass  # Nothing to delete
+            except PermissionError:
+                self.logger.error("Could not delete unzipped fmu "
+                                  "in location %s. Delete it yourself.", unzip_dir)
+
+    def _close_multiprocessing(self, _):
+        """Small helper function"""
+        idx_worker = self.worker_idx
+        if self._fmu_instance is None:
+            return  # Already closed
+        self.logger.error(f"Closing fmu for worker {idx_worker}")
+        self._single_close(fmu_instance=self._fmu_instance,
+                           unzip_dir=self._unzip_dir)
+        self._unzip_dir = None
+        self._fmu_instance = None
+        FMU_API._unzip_dir = None
+        FMU_API._fmu_instance = None
+
+    def simulate(self,
+                 parameters: Union[dict, List[dict]] = None,
+                 return_option: str = "time_series",
+                 **kwargs):
+        """
+        Perform the single simulation for the given
+        unzip directory and fmu_instance.
+        See the docstring of simulate() for information on kwargs.
+
+        Additional kwargs:
+        :keyword str result_file_suffix:
+            Suffix of the result file. Supported options can be extracted
+            from the TimeSeriesData.save() function.
+            Default is 'csv'.
+        :keyword str parquet_engine:
+            The engine to use for the data format parquet.
+            Supported options can be extracted
+            from the TimeSeriesData.save() function.
+            Default is 'pyarrow'.
+        """
+        return super().simulate(parameters=parameters, return_option=return_option, **kwargs)
+
+    def _single_simulation(self, kwargs):
+        """
+        Perform the single simulation for the given
+        unzip directory and fmu_instance.
+        See the docstring of simulate() for information on kwargs.
+
+        The single argument kwarg is to make this
+        function accessible by multiprocessing pool.map.
+        """
+        # Unpack kwargs:
+        parameters = kwargs.pop("parameters", None)
+        return_option = kwargs.pop("return_option", "time_series")
+        inputs = kwargs.get("inputs", None)
+        fail_on_error = kwargs.get("fail_on_error", True)
+
+        if self.use_mp:
+            if self._fmu_instance is None:
+                self._setup_single_fmu_instance(use_mp=True)
+
+        if inputs is not None:
+            if not isinstance(inputs, (TimeSeriesData, pd.DataFrame)):
+                raise TypeError("DataFrame or TimeSeriesData object expected for inputs.")
+            inputs = inputs.copy()  # Create save copy
+            if isinstance(inputs, TimeSeriesData):
+                inputs = inputs.to_df(force_single_index=True)
+            if "time" in inputs.columns:
+                raise IndexError(
+                    "Given inputs contain a column named 'time'. "
+                    "The index is assumed to contain the time-information."
+                )
+            # Convert df to structured numpy array for fmpy: simulate_fmu
+            inputs.insert(0, column="time", value=inputs.index)
+            inputs_tuple = [tuple(columns) for columns in inputs.to_numpy()]
+            # Try to match the type, default is np.double.
+            # 'time' is not in inputs and thus handled separately.
+            dtype = [(inputs.columns[0], np.double)] + \
+                    [(col,
+                      self._type_map.get(self.inputs[col].type, np.double)
+                      ) for col in inputs.columns[1:]]
+            inputs = np.array(inputs_tuple, dtype=dtype)
+        if parameters is None:
+            parameters = {}
+        else:
+            self.check_unsupported_variables(variables=list(parameters.keys()),
+                                             type_of_var="parameters")
+        try:
+            # reset the FMU instance instead of creating a new one
+            self._fmu_instance.reset()
+            # Simulate
+            res = fmpy.simulate_fmu(
+                filename=self._unzip_dir,
+                start_time=self.sim_setup.start_time,
+                stop_time=self.sim_setup.stop_time,
+                solver=self.sim_setup.solver,
+                step_size=self.sim_setup.fixedstepsize,
+                relative_tolerance=None,
+                output_interval=self.sim_setup.output_interval,
+                record_events=False,  # Used for an equidistant output
+                start_values=parameters,
+                apply_default_start_values=False,  # As we pass start_values already
+                input=inputs,
+                output=self.result_names,
+                timeout=self.sim_setup.timeout,
+                step_finished=None,
+                model_description=self._model_description,
+                fmu_instance=self._fmu_instance,
+                fmi_type=self._fmi_type,
+            )
+
+        except Exception as error:
+            self.logger.error(f"[SIMULATION ERROR] Error occurred while running FMU: \n {error}")
+            if fail_on_error:
+                raise error
+            return None
+
+        # Reshape result:
+        df = pd.DataFrame(res).set_index("time")
+        df.index = np.round(df.index.astype("float64"),
+                            str(self.sim_setup.output_interval)[::-1].find('.'))
+
+        if return_option == "savepath":
+            result_file_name = kwargs.get("result_file_name", "resultFile")
+            result_file_suffix = kwargs.get("result_file_suffix", "csv")
+            parquet_engine = kwargs.get('parquet_engine', 'pyarrow')
+            savepath = kwargs.get("savepath", None)
+
+            if savepath is None:
+                savepath = self.cd
+
+            os.makedirs(savepath, exist_ok=True)
+            filepath = os.path.join(savepath, f"{result_file_name}.{result_file_suffix}")
+            TimeSeriesData(df).droplevel(1, axis=1).save(
+                filepath=filepath,
+                key="simulation",
+                engine=parquet_engine
+            )
+
+            return filepath
+        if return_option == "last_point":
+            return df.iloc[-1].to_dict()
+        # Else return time series data
+        tsd = TimeSeriesData(df, default_tag="sim")
+        return tsd
+
+    def setup_fmu_instance(self):
+        """
+        Manually set up and extract the data to
+        avoid this step in the simulate function.
+        """
+        self.logger.info("Extracting fmu and reading fmu model description")
+        # First load model description and extract variables
+        self._single_unzip_dir = os.path.join(self.cd,
+                                              os.path.basename(self.model_name)[:-4] + "_extracted")
+        os.makedirs(self._single_unzip_dir, exist_ok=True)
+        self._single_unzip_dir = fmpy.extract(self.model_name,
+                                              unzipdir=self._single_unzip_dir)
+        self._model_description = read_model_description(self._single_unzip_dir,
+                                                         validate=True)
+
+        if self._model_description.coSimulation is None:
+            self._fmi_type = 'ModelExchange'
+        else:
+            self._fmi_type = 'CoSimulation'
+
+        self.logger.info("Reading model variables")
+
+        _types = {
+            "Enumeration": int,
+            "Integer": int,
+            "Real": float,
+            "Boolean": bool,
+            "String": str
+        }
+        # Extract inputs, outputs & tuner (lists from parent classes will be appended)
+        for var in self._model_description.modelVariables:
+            if var.start is not None:
+                var.start = _types[var.type](var.start)
+
+            _var_ebcpy = Variable(
+                min=var.min,
+                max=var.max,
+                value=var.start,
+                type=_types[var.type]
+            )
+            if var.causality == 'input':
+                self.inputs[var.name] = _var_ebcpy
+            elif var.causality == 'output':
+                self.outputs[var.name] = _var_ebcpy
+            elif var.causality == 'parameter' or var.causality == 'calculatedParameter':
+                self.parameters[var.name] = _var_ebcpy
+            elif var.causality == 'local':
+                self.states[var.name] = _var_ebcpy
+            else:
+                self.logger.error(f"Could not map causality {var.causality}"
+                                  f" to any variable type.")
+
+        if self.use_mp:
+            self.logger.info("Extracting fmu %s times for "
+                             "multiprocessing on %s processes",
+                             self.n_cpu, self.n_cpu)
+            self.pool.map(
+                self._setup_single_fmu_instance,
+                [True for _ in range(self.n_cpu)]
+            )
+            self.logger.info("Instantiated fmu's on all processes.")
+        else:
+            self._setup_single_fmu_instance(use_mp=False)
+
+    def _setup_single_fmu_instance(self, use_mp):
+        if use_mp:
+            wrk_idx = self.worker_idx
+            if self._fmu_instance is not None:
+                return True
+            unzip_dir = self._single_unzip_dir + f"_worker_{wrk_idx}"
+            fmpy.extract(self.model_name,
+                         unzipdir=unzip_dir)
+        else:
+            wrk_idx = 0
+            unzip_dir = self._single_unzip_dir
+
+        self.logger.info("Instantiating fmu for worker %s", wrk_idx)
+        fmu_instance = fmpy.instantiate_fmu(
+            unzipdir=unzip_dir,
+            model_description=self._model_description,
+            fmi_type=self._fmi_type,
+            visible=False,
+            debug_logging=False,
+            logger=self._custom_logger,
+            fmi_call_logger=None)
+        if use_mp:
+            FMU_API._fmu_instance = fmu_instance
+            FMU_API._unzip_dir = unzip_dir
+        else:
+            self._fmu_instance = fmu_instance
+            self._unzip_dir = unzip_dir
+        return True
+
+    def _custom_logger(self, component, instanceName, status, category, message):
+        """ Print the FMU's log messages to the command line (works for both FMI 1.0 and 2.0) """
+        # pylint: disable=unused-argument, invalid-name
+        label = ['OK', 'WARNING', 'DISCARD', 'ERROR', 'FATAL', 'PENDING'][status]
+        _level_map = {'OK': logging.INFO,
+                      'WARNING': logging.WARNING,
+                      'DISCARD': logging.WARNING,
+                      'ERROR': logging.ERROR,
+                      'FATAL': logging.FATAL,
+                      'PENDING': logging.FATAL}
+        if self.log_fmu:
+            self.logger.log(level=_level_map[label], msg=message.decode("utf-8"))
+
+    def save_for_reproduction(self,
+                              title: str,
+                              path: pathlib.Path = None,
+                              files: list = None,
+                              **kwargs):
+        """
+        Additionally to the basic reproduction, add info
+        for FMU files.
+        """
+        if files is None:
+            files = []
+        files.append(CopyFile(
+            filename="FMU/" + pathlib.Path(self.model_name).name,
+            sourcepath=pathlib.Path(self.model_name),
+            remove=False
+        ))
+        return super().save_for_reproduction(
+            title=title,
+            path=path,
+            files=files,
+            **kwargs
+        )
```

### Comparing `ebcpy-0.3.2/ebcpy/utils/__init__.py` & `ebcpy-0.3.6/ebcpy/utils/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-Package containing utility functions used in different packages.
-Contains a statistics analyzer and a visualizer.
-"""
-import logging
-import os
-
-
-def setup_logger(name: str,
-                 cd: str = None,
-                 level=logging.DEBUG):
-    """
-    Setup an class or module specific logger instance
-    to ensure readable output for users.
-
-    :param str name:
-        The name of the logger instance
-    :param str cd:
-        The path where to store the logfile.
-        If None is given, logs are not stored.
-    :param str level:
-        The logging level, default is DEBUG
-
-    .. versionadded:: 0.1.7
-    """
-    logger = logging.getLogger(name=name)
-    # Set log-level
-    logger.setLevel(level=level)
-    # Check if logger was already instantiated. If so, return already.
-    if logger.handlers:
-        return logger
-    # Add handlers
-    formatter = logging.Formatter(fmt='%(asctime)s %(levelname)s %(name)s: %(message)s',
-                                  datefmt='%d.%m.%Y-%H:%M:%S')
-    console = logging.StreamHandler()
-    console.setFormatter(fmt=formatter)
-    logger.addHandler(hdlr=console)
-    if cd is not None:
-        os.makedirs(cd, exist_ok=True)
-        file_handler = logging.FileHandler(filename=os.path.join(cd, f"{name}.log"))
-        file_handler.setFormatter(fmt=formatter)
-        logger.addHandler(hdlr=file_handler)
-    return logger
+"""
+Package containing utility functions used in different packages.
+Contains a statistics analyzer and a visualizer.
+"""
+import logging
+import os
+
+
+def setup_logger(name: str,
+                 cd: str = None,
+                 level=logging.DEBUG):
+    """
+    Setup an class or module specific logger instance
+    to ensure readable output for users.
+
+    :param str name:
+        The name of the logger instance
+    :param str cd:
+        The path where to store the logfile.
+        If None is given, logs are not stored.
+    :param str level:
+        The logging level, default is DEBUG
+
+    .. versionadded:: 0.1.7
+    """
+    logger = logging.getLogger(name=name)
+    # Set log-level
+    logger.setLevel(level=level)
+    # Check if logger was already instantiated. If so, return already.
+    if logger.handlers:
+        return logger
+    # Add handlers
+    formatter = logging.Formatter(fmt='%(asctime)s %(levelname)s %(name)s: %(message)s',
+                                  datefmt='%d.%m.%Y-%H:%M:%S')
+    console = logging.StreamHandler()
+    console.setFormatter(fmt=formatter)
+    logger.addHandler(hdlr=console)
+    if cd is not None:
+        os.makedirs(cd, exist_ok=True)
+        file_handler = logging.FileHandler(filename=os.path.join(cd, f"{name}.log"))
+        file_handler.setFormatter(fmt=formatter)
+        logger.addHandler(hdlr=file_handler)
+    return logger
```

### Comparing `ebcpy-0.3.2/ebcpy/utils/conversion.py` & `ebcpy-0.3.6/ebcpy/utils/conversion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,226 +1,226 @@
-"""
-Module with functions to convert
-certain format into other formats.
-"""
-import pathlib
-import scipy.io as spio
-import numpy as np
-import pandas as pd
-
-from ebcpy.data_types import numeric_indexes, datetime_indexes
-
-
-def convert_tsd_to_modelica_mat(tsd, save_path_file, **kwargs):
-    """
-    Function to convert a tsd to a mat-file readable within Dymola.
-
-    :param TimeSeriesData tsd:
-        TimeSeriesData object
-    :param str,os.path.normpath save_path_file:
-        File path and name where to store the output .mat file.
-    :keyword list columns:
-        A list with names of columns that should be saved to .mat file.
-        If no list is provided, all columns are converted.
-    :keyword float offset:
-        Offset for time in seconds, default 0
-    :returns mat_file:
-        Returns the version 4 mat-file
-
-    :return:
-        str,os.path.normpath:
-            Path where the data is saved.
-            Equal to save_path_file
-
-    Examples:
-
-    >>> import os
-    >>> from ebcpy import TimeSeriesData
-    >>> project_dir = os.path.dirname(os.path.dirname(__file__))
-    >>> example_file = os.path.normpath(project_dir + "//tests//data//example_data.csv")
-    >>> save_path = os.path.normpath(project_dir + "//tests//data//example_data_converted.mat")
-    >>> cols = ["sine.freqHz / Hz"]
-    >>> tsd = TimeSeriesData(example_file, sep=";")
-    >>> filepath = convert_tsd_to_modelica_mat(tsd,
-    >>>                                        save_path, columns=cols)
-    >>> os.remove(filepath)
-    """
-    if isinstance(save_path_file, pathlib.Path):
-        save_path_file = str(save_path_file)
-
-    if not save_path_file.endswith(".mat"):
-        raise ValueError("Given savepath for txt-file is not a .mat file!")
-
-    # Load the relevant part of the df
-    df_sub, _ = _convert_to_subset(
-        df=tsd,
-        columns=kwargs.get("columns", None),
-        offset=kwargs.get("offset", 0)
-    )
-
-    # Convert np.array into a list and create a dict with 'table' as matrix name
-    new_mat = {'table': df_sub.values.tolist()}
-    # Save matrix as a MATLAB *.mat file, which is readable by Modelica.
-    spio.savemat(save_path_file, new_mat, format="4")
-    # Provide user feedback whether the conversion was successful.
-    return save_path_file
-
-
-def convert_tsd_to_clustering_txt(tsd, save_path_file, columns=None):
-    """
-    Function to convert a TimeSeriesData object
-    to a txt-file readable within the TICC-module.
-
-    :param TimeSeriesData tsd:
-        TimeSeriesData object
-    :param str,os.path.normpath save_path_file:
-        File path and name where to store the output .mat file.
-    :param list columns:
-        A list with names of columns that should be saved to .mat file.
-        If no list is provided, all columns are converted.
-    :returns True on Success, savepath of txt-file:
-        Returns the version 4 mat-file
-
-    :return:
-        str,os.path.normpath:
-            Path where the data is saved.
-            Equal to save_path_file
-
-    Examples:
-
-    >>> import os
-    >>> project_dir = os.path.dirname(os.path.dirname(__file__))
-    >>> example_file = os.path.normpath(project_dir + "//tests//data//example_data.csv")
-    >>> save_path = os.path.normpath(project_dir + "//tests//data//example_data_converted.txt")
-    >>> cols = ["sine.freqHz / Hz"]
-    >>> tsd = TimeSeriesData(example_file, sep=";")
-    >>> filepath = convert_tsd_to_clustering_txt(tsd,
-    >>>                                          save_path, columns=cols)
-    >>> os.remove(filepath)
-    """
-    # Get the subset of the dataFrame
-    df_sub, _ = _convert_to_subset(df=tsd, columns=columns, offset=0)
-
-    # Convert np.array into a list and create a list as matrix name
-    df_sub.values.tolist()
-    # Save matrix as a *.txt file, which is readable by TICC.
-    np.savetxt(save_path_file, df_sub, delimiter=',', fmt='%.4f')
-    # Provide user feedback whether the conversion was successful.
-    return save_path_file
-
-
-def convert_tsd_to_modelica_txt(tsd, table_name, save_path_file, **kwargs):
-    """
-    Convert a TimeSeriesData object to modelica readable text. This is especially useful
-    for generating input data for a modelica simulation.
-
-    :param TimeSeriesData tsd:
-        TimeSeriesData object
-    :param str table_name:
-        Name of the table for modelica.
-        Needed in Modelica to correctly load the file.
-    :param str,os.path.normpath save_path_file:
-        File path and name where to store the output .txt file.
-    :keyword list columns:
-        A list with names of columns that should be saved to .mat file.
-        If no list is provided, all columns are converted.
-    :keyword float offset:
-        Offset for time in seconds, default 0
-    :keyword str sep:
-        Separator used to separate values between columns
-    :keyword Boolean with_tag:
-        Use True each variable and tag is written to the file
-        If False, only the variable name is written to the file.
-
-    :return:
-        str,os.path.normpath:
-            Path where the data is saved.
-            Equal to save_path_file
-
-    Examples:
-
-    >>> import os
-    >>> from ebcpy import TimeSeriesData
-    >>> project_dir = os.path.dirname(os.path.dirname(__file__))
-    >>> example_file = os.path.normpath(project_dir + "//tests//data//example_data.csv")
-    >>> save_path = os.path.normpath(project_dir + "//tests//data//example_data_converted.txt")
-    >>> cols = ["sine.freqHz / Hz"]
-    >>> tsd = TimeSeriesData(example_file, sep=";")
-    >>> filepath = convert_tsd_to_modelica_txt(tsd, "dummy_input_data", columns=cols)
-    >>> os.remove(filepath)
-    """
-    if isinstance(save_path_file, pathlib.Path):
-        save_path_file = str(save_path_file)
-    if not save_path_file.endswith(".txt"):
-        raise ValueError("Given savepath for txt-file is not a .txt file!")
-
-    # Load the relavant part of the df
-    df_sub, headers = _convert_to_subset(
-        df=tsd,
-        columns=kwargs.get("columns", None),
-        offset=kwargs.get("offset", 0)
-    )
-
-    # Unpack kwargs
-    sep = kwargs.get("sep", "\t")
-
-    n_cols = len(headers)
-    n_rows = len(df_sub.index)
-    # Comment header line
-    _temp_str = ""
-    if kwargs.get("with_tag", True):
-        # Convert ("variable", "tag") to "variable_tag"
-        _temp_str = sep.join(["_".join(variable_tag) for variable_tag in headers])
-    else:
-        for idx, var in enumerate(headers):
-            if idx == 0:
-                # Convert time with tag to one string as unit is important
-                _temp_str += "_".join(var)
-            else:
-                # Convert ("variable", "tag") to "variable"
-                _temp_str += sep + var[0]
-    content_as_lines = [f"#{_temp_str}\n"]
-    content_as_lines.insert(0, f"double {table_name}({n_rows}, {n_cols})\n")
-    content_as_lines.insert(0, "#1\n")  # Print Modelica table no
-
-    # Open file and write the header
-    with open(file=save_path_file, mode="a+", encoding="utf-8") as file:
-        file.seek(0)
-        file.truncate()  # Delete possible old content
-        file.writelines(content_as_lines)
-
-    # Append the data directly using to_csv from pandas
-    df_sub.to_csv(save_path_file, header=None, index=None, sep=sep, mode="a")
-
-    return save_path_file
-
-
-def _convert_to_subset(df, columns, offset):
-    """
-    Private function to ensure lean conversion to either mat or txt.
-    """
-    df = df.copy()
-    if columns:
-        headers = df[columns].columns.values.tolist()
-    else:
-        headers = df.columns.values.tolist()
-
-    _time_header = ('time', 'in_s')
-    headers.insert(0, _time_header)  # Ensure time will be at first place
-
-    if isinstance(df.index, tuple(datetime_indexes)):
-        df.index = df.index - df.iloc[0].name.to_datetime64()  # Make index zero based
-        df[_time_header] = df.index.total_seconds() + offset
-    elif isinstance(df.index, tuple(numeric_indexes)):
-        df[_time_header] = df.index - df.iloc[0].name + offset
-    else:
-        # Should not happen as error is raised in data_types. But just to be sure:
-        raise IndexError(f"Given index of type {type(df.index)} is not supported.")
-    # Avoid 1e-8 errors in timedelta calculation.
-    df[_time_header] = df[_time_header].round(4)
-
-    # Check if nan values occur
-    if df.loc[:, headers].isnull().values.sum() > 0:
-        raise ValueError("Selected columns contain NaN values. This would lead to errors"
-                         "in the simulation environment.")
-
-    return df.loc[:, headers], headers
+"""
+Module with functions to convert
+certain format into other formats.
+"""
+import pathlib
+import scipy.io as spio
+import numpy as np
+import pandas as pd
+
+from ebcpy.data_types import index_is_numeric, datetime_indexes
+
+
+def convert_tsd_to_modelica_mat(tsd, save_path_file, **kwargs):
+    """
+    Function to convert a tsd to a mat-file readable within Dymola.
+
+    :param TimeSeriesData tsd:
+        TimeSeriesData object
+    :param str,os.path.normpath save_path_file:
+        File path and name where to store the output .mat file.
+    :keyword list columns:
+        A list with names of columns that should be saved to .mat file.
+        If no list is provided, all columns are converted.
+    :keyword float offset:
+        Offset for time in seconds, default 0
+    :returns mat_file:
+        Returns the version 4 mat-file
+
+    :return:
+        str,os.path.normpath:
+            Path where the data is saved.
+            Equal to save_path_file
+
+    Examples:
+
+    >>> import os
+    >>> from ebcpy import TimeSeriesData
+    >>> project_dir = os.path.dirname(os.path.dirname(__file__))
+    >>> example_file = os.path.normpath(project_dir + "//tests//data//example_data.csv")
+    >>> save_path = os.path.normpath(project_dir + "//tests//data//example_data_converted.mat")
+    >>> cols = ["sine.freqHz / Hz"]
+    >>> tsd = TimeSeriesData(example_file, sep=";")
+    >>> filepath = convert_tsd_to_modelica_mat(tsd,
+    >>>                                        save_path, columns=cols)
+    >>> os.remove(filepath)
+    """
+    if isinstance(save_path_file, pathlib.Path):
+        save_path_file = str(save_path_file)
+
+    if not save_path_file.endswith(".mat"):
+        raise ValueError("Given savepath for txt-file is not a .mat file!")
+
+    # Load the relevant part of the df
+    df_sub, _ = _convert_to_subset(
+        df=tsd,
+        columns=kwargs.get("columns", None),
+        offset=kwargs.get("offset", 0)
+    )
+
+    # Convert np.array into a list and create a dict with 'table' as matrix name
+    new_mat = {'table': df_sub.values.tolist()}
+    # Save matrix as a MATLAB *.mat file, which is readable by Modelica.
+    spio.savemat(save_path_file, new_mat, format="4")
+    # Provide user feedback whether the conversion was successful.
+    return save_path_file
+
+
+def convert_tsd_to_clustering_txt(tsd, save_path_file, columns=None):
+    """
+    Function to convert a TimeSeriesData object
+    to a txt-file readable within the TICC-module.
+
+    :param TimeSeriesData tsd:
+        TimeSeriesData object
+    :param str,os.path.normpath save_path_file:
+        File path and name where to store the output .mat file.
+    :param list columns:
+        A list with names of columns that should be saved to .mat file.
+        If no list is provided, all columns are converted.
+    :returns True on Success, savepath of txt-file:
+        Returns the version 4 mat-file
+
+    :return:
+        str,os.path.normpath:
+            Path where the data is saved.
+            Equal to save_path_file
+
+    Examples:
+
+    >>> import os
+    >>> project_dir = os.path.dirname(os.path.dirname(__file__))
+    >>> example_file = os.path.normpath(project_dir + "//tests//data//example_data.csv")
+    >>> save_path = os.path.normpath(project_dir + "//tests//data//example_data_converted.txt")
+    >>> cols = ["sine.freqHz / Hz"]
+    >>> tsd = TimeSeriesData(example_file, sep=";")
+    >>> filepath = convert_tsd_to_clustering_txt(tsd,
+    >>>                                          save_path, columns=cols)
+    >>> os.remove(filepath)
+    """
+    # Get the subset of the dataFrame
+    df_sub, _ = _convert_to_subset(df=tsd, columns=columns, offset=0)
+
+    # Convert np.array into a list and create a list as matrix name
+    df_sub.values.tolist()
+    # Save matrix as a *.txt file, which is readable by TICC.
+    np.savetxt(save_path_file, df_sub, delimiter=',', fmt='%.4f')
+    # Provide user feedback whether the conversion was successful.
+    return save_path_file
+
+
+def convert_tsd_to_modelica_txt(tsd, table_name, save_path_file, **kwargs):
+    """
+    Convert a TimeSeriesData object to modelica readable text. This is especially useful
+    for generating input data for a modelica simulation.
+
+    :param TimeSeriesData tsd:
+        TimeSeriesData object
+    :param str table_name:
+        Name of the table for modelica.
+        Needed in Modelica to correctly load the file.
+    :param str,os.path.normpath save_path_file:
+        File path and name where to store the output .txt file.
+    :keyword list columns:
+        A list with names of columns that should be saved to .mat file.
+        If no list is provided, all columns are converted.
+    :keyword float offset:
+        Offset for time in seconds, default 0
+    :keyword str sep:
+        Separator used to separate values between columns
+    :keyword Boolean with_tag:
+        Use True each variable and tag is written to the file
+        If False, only the variable name is written to the file.
+
+    :return:
+        str,os.path.normpath:
+            Path where the data is saved.
+            Equal to save_path_file
+
+    Examples:
+
+    >>> import os
+    >>> from ebcpy import TimeSeriesData
+    >>> project_dir = os.path.dirname(os.path.dirname(__file__))
+    >>> example_file = os.path.normpath(project_dir + "//tests//data//example_data.csv")
+    >>> save_path = os.path.normpath(project_dir + "//tests//data//example_data_converted.txt")
+    >>> cols = ["sine.freqHz / Hz"]
+    >>> tsd = TimeSeriesData(example_file, sep=";")
+    >>> filepath = convert_tsd_to_modelica_txt(tsd, "dummy_input_data", columns=cols)
+    >>> os.remove(filepath)
+    """
+    if isinstance(save_path_file, pathlib.Path):
+        save_path_file = str(save_path_file)
+    if not save_path_file.endswith(".txt"):
+        raise ValueError("Given savepath for txt-file is not a .txt file!")
+
+    # Load the relavant part of the df
+    df_sub, headers = _convert_to_subset(
+        df=tsd,
+        columns=kwargs.get("columns", None),
+        offset=kwargs.get("offset", 0)
+    )
+
+    # Unpack kwargs
+    sep = kwargs.get("sep", "\t")
+
+    n_cols = len(headers)
+    n_rows = len(df_sub.index)
+    # Comment header line
+    _temp_str = ""
+    if kwargs.get("with_tag", True):
+        # Convert ("variable", "tag") to "variable_tag"
+        _temp_str = sep.join(["_".join(variable_tag) for variable_tag in headers])
+    else:
+        for idx, var in enumerate(headers):
+            if idx == 0:
+                # Convert time with tag to one string as unit is important
+                _temp_str += "_".join(var)
+            else:
+                # Convert ("variable", "tag") to "variable"
+                _temp_str += sep + var[0]
+    content_as_lines = [f"#{_temp_str}\n"]
+    content_as_lines.insert(0, f"double {table_name}({n_rows}, {n_cols})\n")
+    content_as_lines.insert(0, "#1\n")  # Print Modelica table no
+
+    # Open file and write the header
+    with open(file=save_path_file, mode="a+", encoding="utf-8") as file:
+        file.seek(0)
+        file.truncate()  # Delete possible old content
+        file.writelines(content_as_lines)
+
+    # Append the data directly using to_csv from pandas
+    df_sub.to_csv(save_path_file, header=None, index=None, sep=sep, mode="a")
+
+    return save_path_file
+
+
+def _convert_to_subset(df, columns, offset):
+    """
+    Private function to ensure lean conversion to either mat or txt.
+    """
+    df = df.copy()
+    if columns:
+        headers = df[columns].columns.values.tolist()
+    else:
+        headers = df.columns.values.tolist()
+
+    _time_header = ('time', 'in_s')
+    headers.insert(0, _time_header)  # Ensure time will be at first place
+
+    if isinstance(df.index, tuple(datetime_indexes)):
+        df.index = df.index - df.iloc[0].name.to_datetime64()  # Make index zero based
+        df[_time_header] = df.index.total_seconds() + offset
+    elif index_is_numeric(df.index):
+        df[_time_header] = df.index - df.iloc[0].name + offset
+    else:
+        # Should not happen as error is raised in data_types. But just to be sure:
+        raise IndexError(f"Given index of type {type(df.index)} is not supported.")
+    # Avoid 1e-8 errors in timedelta calculation.
+    df[_time_header] = df[_time_header].round(4)
+
+    # Check if nan values occur
+    if df.loc[:, headers].isnull().values.sum() > 0:
+        raise ValueError("Selected columns contain NaN values. This would lead to errors"
+                         "in the simulation environment.")
+
+    return df.loc[:, headers], headers
```

### Comparing `ebcpy-0.3.2/ebcpy.egg-info/SOURCES.txt` & `ebcpy-0.3.6/ebcpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.2/setup.py` & `ebcpy-0.3.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,78 @@
-"""Setup.py script for the ebcpy-framework"""
-
-import setuptools
-import sys
-
-# read the contents of your README file
-from pathlib import Path
-readme_path = Path(__file__).parent.joinpath("README.md")
-long_description = readme_path.read_text()
-
-EXTRAS_REQUIRE = {
-    'full': [
-        'openpyxl>=3.0.5',
-        'xlrd>=2.0.1',
-        'pymoo==0.4.2',
-        'GitPython>=3.1.27'
-    ]
-}
-
-INSTALL_REQUIRES = [
-    'numpy>=1.19.5',
-    'matplotlib>=3.3.4',
-    'scipy>=1.5.4',
-    'pandas>=1.1.5',
-    'scikit-learn>=0.24.2',
-    'fmpy>=0.2.27',
-    'pydantic>=1.8.2',
-    'h5py>=3.1.0'
-]
-# TODO: Remove once tables in enables for python >3.9
-if sys.version_info.minor < 9 and sys.version_info.major == 3:
-    INSTALL_REQUIRES.append('tables>=3.6.1')
-# Add all open-source packages to setup-requires
-SETUP_REQUIRES = INSTALL_REQUIRES.copy()
-
-VERSION = "0.3.2"
-
-setuptools.setup(
-    name='ebcpy',
-    version=VERSION,
-    description='Python Library used for different python modules'
-                ' for the analysis and optimization of energy systems, '
-                'buildings and indoor climate ',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/RWTH-EBC/ebcpy',
-    download_url=f'https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/{VERSION}.tar.gz',
-    license='BSD 3-Clause',
-    author='RWTH Aachen University, E.ON Energy Research Center, Institute '
-           'of Energy Efficient Buildings and Indoor Climate',
-    author_email='fabian.wuellhorst@eonerc.rwth-aachen.de',
-    # Specify the Python versions you support here. In particular, ensure
-    # that you indicate whether you support Python 2, Python 3 or both.
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'License :: OSI Approved :: BSD License',
-        'Topic :: Scientific/Engineering',
-        'Intended Audience :: Science/Research',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
-    ],
-    keywords=[
-        'simulation', 'building', 'energy',
-        'time-series-data', 'comfort',
-        'black-box optimization'
-    ],
-    packages=setuptools.find_packages(exclude=['tests', 'tests.*', 'img']),
-    extras_require=EXTRAS_REQUIRE,
-    setup_requires=SETUP_REQUIRES,
-    install_requires=INSTALL_REQUIRES,
-)
+"""Setup.py script for the ebcpy-framework"""
+
+import setuptools
+import sys
+
+# read the contents of your README file
+from pathlib import Path
+readme_path = Path(__file__).parent.joinpath("README.md")
+long_description = readme_path.read_text()
+
+EXTRAS_REQUIRE = {
+    'full': [
+        'openpyxl>=3.0.5',
+        'xlrd>=2.0.1',
+        'pymoo==0.5.0',
+        'GitPython>=3.1.27',
+        'pyarrow>=11.0.0'
+    ]
+}
+
+INSTALL_REQUIRES = [
+    'numpy>=1.19.5',
+    'matplotlib>=3.3.4',
+    'scipy>=1.5.4',
+    'pandas>=1.1.5',
+    'scikit-learn>=0.24.2',
+    'fmpy>=0.2.27',
+    'pydantic>=1.8.2',
+    'h5py>=3.1.0',
+    'tables>=3.6.1'
+]
+    
+if sys.version_info.minor >= 9 and sys.version_info.major == 3:
+    EXTRAS_REQUIRE['full'].append('fastparquet>=2023.1.0')
+
+# Add all open-source packages to setup-requires
+SETUP_REQUIRES = INSTALL_REQUIRES.copy()
+
+with open(Path(__file__).parent.joinpath("ebcpy", "__init__.py"), "r") as file:
+    for line in file.readlines():
+        if line.startswith("__version__"):
+            VERSION = line.replace("__version__", "").split("=")[1].strip().replace("'", "").replace('"', '')
+
+setuptools.setup(
+    name='ebcpy',
+    version=VERSION,
+    description='Python Library used for different python modules'
+                ' for the analysis and optimization of energy systems, '
+                'buildings and indoor climate ',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/RWTH-EBC/ebcpy',
+    download_url=f'https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/{VERSION}.tar.gz',
+    license='BSD 3-Clause',
+    author='RWTH Aachen University, E.ON Energy Research Center, Institute '
+           'of Energy Efficient Buildings and Indoor Climate',
+    author_email='fabian.wuellhorst@eonerc.rwth-aachen.de',
+    # Specify the Python versions you support here. In particular, ensure
+    # that you indicate whether you support Python 2, Python 3 or both.
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'License :: OSI Approved :: BSD License',
+        'Topic :: Scientific/Engineering',
+        'Intended Audience :: Science/Research',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9'
+    ],
+    keywords=[
+        'simulation', 'building', 'energy',
+        'time-series-data', 'comfort',
+        'black-box optimization'
+    ],
+    packages=setuptools.find_packages(exclude=['tests', 'tests.*', 'img']),
+    extras_require=EXTRAS_REQUIRE,
+    setup_requires=SETUP_REQUIRES,
+    install_requires=INSTALL_REQUIRES,
+)
```

