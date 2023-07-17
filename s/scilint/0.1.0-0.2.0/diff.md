# Comparing `tmp/scilint-0.1.0.tar.gz` & `tmp/scilint-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scilint-0.1.0.tar", last modified: Fri Jul 14 15:42:38 2023, max compression
+gzip compressed data, was "scilint-0.2.0.tar", last modified: Mon Jul 17 09:55:11 2023, max compression
```

## Comparing `scilint-0.1.0.tar` & `scilint-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-14 15:41:07.000000 scilint-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-14 15:41:07.000000 scilint-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-07-14 15:42:38.072636 scilint-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17401 2023-07-14 15:42:22.000000 scilint-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-14 15:41:07.000000 scilint-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.068636 scilint-0.1.0/scilint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25902 2023-07-14 15:42:22.000000 scilint-0.1.0/scilint/_modidx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/experimental/test_nbdev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/exploratory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/exploratory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/exploratory/test_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (123)    22180 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/scilint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/test/test_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/test/test_nbdev_high_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/validated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/validated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/validated/test_nbdev_high_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:41:20.000000 scilint-0.1.0/scilint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:42:38.072636 scilint-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-14 15:41:07.000000 scilint-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-17 09:53:13.000000 scilint-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 09:53:13.000000 scilint-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-17 09:55:11.653639 scilint-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17398 2023-07-17 09:54:49.000000 scilint-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 09:53:13.000000 scilint-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.649639 scilint-0.2.0/scilint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28316 2023-07-17 09:54:49.000000 scilint-0.2.0/scilint/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/experimental/test_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/exploratory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/exploratory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/exploratory/test_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/scilint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/test/test_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/test/test_nbdev_high_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/validated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/validated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/validated/test_nbdev_high_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:53:31.000000 scilint-0.2.0/scilint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:55:11.653639 scilint-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-17 09:53:13.000000 scilint-0.2.0/setup.py
```

### Comparing `scilint-0.1.0/LICENSE` & `scilint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scilint-0.1.0/NOTICE` & `scilint-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `scilint-0.1.0/PKG-INFO` & `scilint-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilint
-Version: 0.1.0
+Version: 0.2.0
 Summary: infuse quality into notebook based workflows with a new type of build tool.
 Home-page: https://github.com/newday-data/scilint/tree/{branch}/
 Author: Donal Simmie
 Author-email: oss@newday.co.uk
 License: Apache Software License 2.0
 Project-URL: Documentation, https://newday-data.github.io/scilint/
 Keywords: research,production,exploration,CI/CD
@@ -196,32 +196,33 @@
 
 The below are potential quality indicators that you can use to set a
 minimum bar for quality and comprehensibility within your projects.
 These are not exhaustive or definite quality indicators - they are a
 starting point to open the conversation about what it means to have a
 high quality notebook in practice.
 
-1.  **Calls-Per-Function (CPF):** compares the amount of calls to the
-    amount of functions. Looks for possible relationship between
-    function definitions and usage.
-2.  **In-Function-Percent (IFP):** the percentage of code that is within
-    a function rather than outside function scope.
-3.  **Asserts-Per-Function (APF):** looks at how many tests (where
-    assert = test) there are compared to the total function count.
-4.  **InlineAssertsPerFunction (IAF):** examines how many times a
-    function is called within an assert statement - this aims to see
-    testing of functions not just usage.
-5.  **MarkdownToCodeRatio (MCP):** what is the ratio of markdown cells
-    to code cells.
-6.  **TotalCodeLen (TCL):** the total line length of the notebook code
+1.  Calls-Per-Function (CPF):\*\* compares the **amount of calls to the
+    amount of functions**. *Looks for possible relationship between
+    function definitions and usage.*
+2.  In-Function-Percent (IFP): the **percentage of code that is within a
+    function** rather than outside function scope.
+3.  Tests-Per-Function-Mean (TPF: the **average number of tests (where
+    test==assert) for all functions**. *Mean value so may be dominated
+    by outliers.*
+4.  Tests-Function-Coverage-Pct (TFC): what **percentage of all
+    functions have at least one test**. *Note: this is coverage at
+    function-level not line-based coverage.*
+5.  MarkdownToCodeRatio (MCP): what is the **ratio of markdown cells to
+    code cells**.
+6.  TotalCodeLen (TCL): the **total line length** of the notebook code
     cells.
-7.  **Loc-Per-MD-Section:** the lines of code per Markdown section
+7.  Loc-Per-MD-Section (LPS): the **lines of code per Markdown section**
     header.
-8.  **SyntaxErrors**: if the code within the notebook has invalid Python
-    syntax.
+8.  SyntaxErrors (SYN): if the code within the notebook has **invalid
+    Python syntax**.
 
 > *as already stated there is no definitive answer as to whether any of
 > these are low or high quality. However there are reasons to believe
 > inituitively that higher or lower values of the above will produce
 > higher quality notebooks. There are many questions left to answer,
 > like the role of docstrings, comments and type annotations; their
 > effectiveness may warrant inclusion but that is an open question at
@@ -306,17 +307,16 @@
       print_syntax_errors: false
       evaluate: true
       warnings:
         lt:
           calls_per_func_median: 1
           calls_per_func_mean: 1
           in_func_pct: 20
-          asserts_func_ratio: 1
-          inline_asserts_per_func_median: 0
-          inline_asserts_per_func_mean: 0.5
+          tests_func_coverage_pct: 20
+          tests_per_func_mean: 0.5
           markdown_code_pct: 5
         gt:
           total_code_len: 50000
           loc_per_md_section: 2000
         equals:
           has_syntax_error: true
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scilint Version: 0.1.0 Summary: infuse quality into
+Metadata-Version: 2.1 Name: scilint Version: 0.2.0 Summary: infuse quality into
 notebook based workflows with a new type of build tool. Home-page: https://
 github.com/newday-data/scilint/tree/{branch}/ Author: Donal Simmie Author-
 email: oss@newday.co.uk License: Apache Software License 2.0 Project-URL:
 Documentation, https://newday-data.github.io/scilint/ Keywords:
 research,production,exploration,CI/CD Platform: UNKNOWN Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Programming Language ::
@@ -101,57 +101,58 @@
 quarto build. Quarto is a core part of the nbdev system, if you are having
 trouble installing it, check out the `nbdev` Github [page](https://github.com/
 fastai/nbdev). For more details on the Quarto project, check out their home
 [page](https://quarto.org/). # ð Quality Indicators The below are potential
 quality indicators that you can use to set a minimum bar for quality and
 comprehensibility within your projects. These are not exhaustive or definite
 quality indicators - they are a starting point to open the conversation about
-what it means to have a high quality notebook in practice. 1. **Calls-Per-
-Function (CPF):** compares the amount of calls to the amount of functions.
-Looks for possible relationship between function definitions and usage. 2.
-**In-Function-Percent (IFP):** the percentage of code that is within a function
-rather than outside function scope. 3. **Asserts-Per-Function (APF):** looks at
-how many tests (where assert = test) there are compared to the total function
-count. 4. **InlineAssertsPerFunction (IAF):** examines how many times a
-function is called within an assert statement - this aims to see testing of
-functions not just usage. 5. **MarkdownToCodeRatio (MCP):** what is the ratio
-of markdown cells to code cells. 6. **TotalCodeLen (TCL):** the total line
-length of the notebook code cells. 7. **Loc-Per-MD-Section:** the lines of code
-per Markdown section header. 8. **SyntaxErrors**: if the code within the
-notebook has invalid Python syntax. > *as already stated there is no definitive
-answer as to whether any of > these are low or high quality. However there are
-reasons to believe > inituitively that higher or lower values of the above will
-produce > higher quality notebooks. There are many questions left to answer, >
-like the role of docstrings, comments and type annotations; their >
-effectiveness may warrant inclusion but that is an open question at > the
-moment. As this library is used and refined with more projects and > more
-experimental metrics then these intuitions can evaluated more > rigorously.* ##
-â Adding New Indicators For now post your ideas as a feature request and we
-can discuss, if accepted you can provide a PR. We are looking for a more
-rigorous way link indicator and effectivess, until that is found discussion is
-the best we can do! # ð Quality Specs (& a Quality Standard) Often in
-Software Engineering code is both likely to go into production and likely to
-continue to be used once it does. In this enviroment it makes sense for
-codebases to have a single quality standard. In the **explore vs exploit**
-decision making [trade-off](https://en.wikipedia.org/wiki/Exploration-
-exploitation_dilemma) this environment could be classified as **high exploit**.
-For problems that are **high explore**, like most Data Science work, we argue
-that **a single quality bar is not sufficient**. `scilint` promotes adopting a
-*progressive consolidation*\* approach where exploration code starts with a
-speed of exploration goal and this may gradually shift to increase the emphasis
-on quality and reuse as the utility of the workflow becomes proven. This
-feature is known as âQuality Specsâ and it allows multiple different
-specifications of quality to exist within a project. The standard can be a
-relatively low bar for exploration work but can become more demanding as you
-are closer to the productionisation of your work. \**(term first used by [GaÃ«l
-Varoqouax](https://gael-varoquaux.info/); see [here](https://gael-
-varoquaux.info/programming/software-for-reproducible-science-lets-not-have-a-
-misunderstanding.html) for argument expansion).* ## Reference Quality Standard
-> The progressive consolidation workflow that we use on projects is the >
-reference implementation for `scilint` and is summarised in the below > image:
+what it means to have a high quality notebook in practice. 1. Calls-Per-
+Function (CPF):\*\* compares the **amount of calls to the amount of
+functions**. *Looks for possible relationship between function definitions and
+usage.* 2. In-Function-Percent (IFP): the **percentage of code that is within a
+function** rather than outside function scope. 3. Tests-Per-Function-Mean (TPF:
+the **average number of tests (where test==assert) for all functions**. *Mean
+value so may be dominated by outliers.* 4. Tests-Function-Coverage-Pct (TFC):
+what **percentage of all functions have at least one test**. *Note: this is
+coverage at function-level not line-based coverage.* 5. MarkdownToCodeRatio
+(MCP): what is the **ratio of markdown cells to code cells**. 6. TotalCodeLen
+(TCL): the **total line length** of the notebook code cells. 7. Loc-Per-MD-
+Section (LPS): the **lines of code per Markdown section** header. 8.
+SyntaxErrors (SYN): if the code within the notebook has **invalid Python
+syntax**. > *as already stated there is no definitive answer as to whether any
+of > these are low or high quality. However there are reasons to believe >
+inituitively that higher or lower values of the above will produce > higher
+quality notebooks. There are many questions left to answer, > like the role of
+docstrings, comments and type annotations; their > effectiveness may warrant
+inclusion but that is an open question at > the moment. As this library is used
+and refined with more projects and > more experimental metrics then these
+intuitions can evaluated more > rigorously.* ## â Adding New Indicators For
+now post your ideas as a feature request and we can discuss, if accepted you
+can provide a PR. We are looking for a more rigorous way link indicator and
+effectivess, until that is found discussion is the best we can do! # ð
+Quality Specs (& a Quality Standard) Often in Software Engineering code is both
+likely to go into production and likely to continue to be used once it does. In
+this enviroment it makes sense for codebases to have a single quality standard.
+In the **explore vs exploit** decision making [trade-off](https://
+en.wikipedia.org/wiki/Exploration-exploitation_dilemma) this environment could
+be classified as **high exploit**. For problems that are **high explore**, like
+most Data Science work, we argue that **a single quality bar is not
+sufficient**. `scilint` promotes adopting a *progressive consolidation*\*
+approach where exploration code starts with a speed of exploration goal and
+this may gradually shift to increase the emphasis on quality and reuse as the
+utility of the workflow becomes proven. This feature is known as âQuality
+Specsâ and it allows multiple different specifications of quality to exist
+within a project. The standard can be a relatively low bar for exploration work
+but can become more demanding as you are closer to the productionisation of
+your work. \**(term first used by [GaÃ«l Varoqouax](https://gael-
+varoquaux.info/); see [here](https://gael-varoquaux.info/programming/software-
+for-reproducible-science-lets-not-have-a-misunderstanding.html) for argument
+expansion).* ## Reference Quality Standard > The progressive consolidation
+workflow that we use on projects is the > reference implementation for
+`scilint` and is summarised in the below > image:
                               [Quality Standard]
 - **Legacy:** especially on larger projects there may be a large number of
 legacy notebooks that are not in use and no there is no obvious value in
 improving their quality. This could be removed from the workflow if you have
 enforced a quality standard from the outset. - **Exploratory:** exploratory
 workflows are typically off-line and involve much iteration. The benefit of
 some quality bar here is that it aids collaboration, review and generally helps
@@ -166,19 +167,19 @@
 is just a yaml configuration file of the properties of the quality spec. It
 contains threshold values for warning along with some other settings. To adopt
 a multi-spec standard place a spec file into each directory that you want to
 have different standards for. Look at `nbs/examples/nbs` to see an example of a
 multi-spec standard. --- exclusions: ~ fail_over: 1 out_dir: "/tmp/scilint/
 " precision: 3 print_syntax_errors: false evaluate: true warnings: lt:
 calls_per_func_median: 1 calls_per_func_mean: 1 in_func_pct: 20
-asserts_func_ratio: 1 inline_asserts_per_func_median: 0
-inline_asserts_per_func_mean: 0.5 markdown_code_pct: 5 gt: total_code_len:
-50000 loc_per_md_section: 2000 equals: has_syntax_error: true ## What does a
-lint report look like? The lint warnings are printed to the console and a more
-thorough report is generated and saved as a CSV file which looks like this:
+tests_func_coverage_pct: 20 tests_per_func_mean: 0.5 markdown_code_pct: 5 gt:
+total_code_len: 50000 loc_per_md_section: 2000 equals: has_syntax_error: true
+## What does a lint report look like? The lint warnings are printed to the
+console and a more thorough report is generated and saved as a CSV file which
+looks like this:
                                 [Sample Report]
 # ð Changing Behaviour - Recommended Usage Infusing quality into workflows
 is aided by having timely, short-cycle feedback of issues. Addtionally whatever
 quality bar you choose as a team, it should be non-negotiable that way you can
 spend time thinking about what matters like the problem you are trying to solve
 not nitpicking on small details repeatedly. We recommend using `scilint` in the
 following way to maximise benefit: 1. Decide upon a quality standard including
```

### Comparing `scilint-0.1.0/README.md` & `scilint-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -172,32 +172,33 @@
 
 The below are potential quality indicators that you can use to set a
 minimum bar for quality and comprehensibility within your projects.
 These are not exhaustive or definite quality indicators - they are a
 starting point to open the conversation about what it means to have a
 high quality notebook in practice.
 
-1.  **Calls-Per-Function (CPF):** compares the amount of calls to the
-    amount of functions. Looks for possible relationship between
-    function definitions and usage.
-2.  **In-Function-Percent (IFP):** the percentage of code that is within
-    a function rather than outside function scope.
-3.  **Asserts-Per-Function (APF):** looks at how many tests (where
-    assert = test) there are compared to the total function count.
-4.  **InlineAssertsPerFunction (IAF):** examines how many times a
-    function is called within an assert statement - this aims to see
-    testing of functions not just usage.
-5.  **MarkdownToCodeRatio (MCP):** what is the ratio of markdown cells
-    to code cells.
-6.  **TotalCodeLen (TCL):** the total line length of the notebook code
+1.  Calls-Per-Function (CPF):\*\* compares the **amount of calls to the
+    amount of functions**. *Looks for possible relationship between
+    function definitions and usage.*
+2.  In-Function-Percent (IFP): the **percentage of code that is within a
+    function** rather than outside function scope.
+3.  Tests-Per-Function-Mean (TPF: the **average number of tests (where
+    test==assert) for all functions**. *Mean value so may be dominated
+    by outliers.*
+4.  Tests-Function-Coverage-Pct (TFC): what **percentage of all
+    functions have at least one test**. *Note: this is coverage at
+    function-level not line-based coverage.*
+5.  MarkdownToCodeRatio (MCP): what is the **ratio of markdown cells to
+    code cells**.
+6.  TotalCodeLen (TCL): the **total line length** of the notebook code
     cells.
-7.  **Loc-Per-MD-Section:** the lines of code per Markdown section
+7.  Loc-Per-MD-Section (LPS): the **lines of code per Markdown section**
     header.
-8.  **SyntaxErrors**: if the code within the notebook has invalid Python
-    syntax.
+8.  SyntaxErrors (SYN): if the code within the notebook has **invalid
+    Python syntax**.
 
 > *as already stated there is no definitive answer as to whether any of
 > these are low or high quality. However there are reasons to believe
 > inituitively that higher or lower values of the above will produce
 > higher quality notebooks. There are many questions left to answer,
 > like the role of docstrings, comments and type annotations; their
 > effectiveness may warrant inclusion but that is an open question at
@@ -282,17 +283,16 @@
       print_syntax_errors: false
       evaluate: true
       warnings:
         lt:
           calls_per_func_median: 1
           calls_per_func_mean: 1
           in_func_pct: 20
-          asserts_func_ratio: 1
-          inline_asserts_per_func_median: 0
-          inline_asserts_per_func_mean: 0.5
+          tests_func_coverage_pct: 20
+          tests_per_func_mean: 0.5
           markdown_code_pct: 5
         gt:
           total_code_len: 50000
           loc_per_md_section: 2000
         equals:
           has_syntax_error: true
```

#### html2text {}

```diff
@@ -89,57 +89,58 @@
 quarto build. Quarto is a core part of the nbdev system, if you are having
 trouble installing it, check out the `nbdev` Github [page](https://github.com/
 fastai/nbdev). For more details on the Quarto project, check out their home
 [page](https://quarto.org/). # ð Quality Indicators The below are potential
 quality indicators that you can use to set a minimum bar for quality and
 comprehensibility within your projects. These are not exhaustive or definite
 quality indicators - they are a starting point to open the conversation about
-what it means to have a high quality notebook in practice. 1. **Calls-Per-
-Function (CPF):** compares the amount of calls to the amount of functions.
-Looks for possible relationship between function definitions and usage. 2.
-**In-Function-Percent (IFP):** the percentage of code that is within a function
-rather than outside function scope. 3. **Asserts-Per-Function (APF):** looks at
-how many tests (where assert = test) there are compared to the total function
-count. 4. **InlineAssertsPerFunction (IAF):** examines how many times a
-function is called within an assert statement - this aims to see testing of
-functions not just usage. 5. **MarkdownToCodeRatio (MCP):** what is the ratio
-of markdown cells to code cells. 6. **TotalCodeLen (TCL):** the total line
-length of the notebook code cells. 7. **Loc-Per-MD-Section:** the lines of code
-per Markdown section header. 8. **SyntaxErrors**: if the code within the
-notebook has invalid Python syntax. > *as already stated there is no definitive
-answer as to whether any of > these are low or high quality. However there are
-reasons to believe > inituitively that higher or lower values of the above will
-produce > higher quality notebooks. There are many questions left to answer, >
-like the role of docstrings, comments and type annotations; their >
-effectiveness may warrant inclusion but that is an open question at > the
-moment. As this library is used and refined with more projects and > more
-experimental metrics then these intuitions can evaluated more > rigorously.* ##
-â Adding New Indicators For now post your ideas as a feature request and we
-can discuss, if accepted you can provide a PR. We are looking for a more
-rigorous way link indicator and effectivess, until that is found discussion is
-the best we can do! # ð Quality Specs (& a Quality Standard) Often in
-Software Engineering code is both likely to go into production and likely to
-continue to be used once it does. In this enviroment it makes sense for
-codebases to have a single quality standard. In the **explore vs exploit**
-decision making [trade-off](https://en.wikipedia.org/wiki/Exploration-
-exploitation_dilemma) this environment could be classified as **high exploit**.
-For problems that are **high explore**, like most Data Science work, we argue
-that **a single quality bar is not sufficient**. `scilint` promotes adopting a
-*progressive consolidation*\* approach where exploration code starts with a
-speed of exploration goal and this may gradually shift to increase the emphasis
-on quality and reuse as the utility of the workflow becomes proven. This
-feature is known as âQuality Specsâ and it allows multiple different
-specifications of quality to exist within a project. The standard can be a
-relatively low bar for exploration work but can become more demanding as you
-are closer to the productionisation of your work. \**(term first used by [GaÃ«l
-Varoqouax](https://gael-varoquaux.info/); see [here](https://gael-
-varoquaux.info/programming/software-for-reproducible-science-lets-not-have-a-
-misunderstanding.html) for argument expansion).* ## Reference Quality Standard
-> The progressive consolidation workflow that we use on projects is the >
-reference implementation for `scilint` and is summarised in the below > image:
+what it means to have a high quality notebook in practice. 1. Calls-Per-
+Function (CPF):\*\* compares the **amount of calls to the amount of
+functions**. *Looks for possible relationship between function definitions and
+usage.* 2. In-Function-Percent (IFP): the **percentage of code that is within a
+function** rather than outside function scope. 3. Tests-Per-Function-Mean (TPF:
+the **average number of tests (where test==assert) for all functions**. *Mean
+value so may be dominated by outliers.* 4. Tests-Function-Coverage-Pct (TFC):
+what **percentage of all functions have at least one test**. *Note: this is
+coverage at function-level not line-based coverage.* 5. MarkdownToCodeRatio
+(MCP): what is the **ratio of markdown cells to code cells**. 6. TotalCodeLen
+(TCL): the **total line length** of the notebook code cells. 7. Loc-Per-MD-
+Section (LPS): the **lines of code per Markdown section** header. 8.
+SyntaxErrors (SYN): if the code within the notebook has **invalid Python
+syntax**. > *as already stated there is no definitive answer as to whether any
+of > these are low or high quality. However there are reasons to believe >
+inituitively that higher or lower values of the above will produce > higher
+quality notebooks. There are many questions left to answer, > like the role of
+docstrings, comments and type annotations; their > effectiveness may warrant
+inclusion but that is an open question at > the moment. As this library is used
+and refined with more projects and > more experimental metrics then these
+intuitions can evaluated more > rigorously.* ## â Adding New Indicators For
+now post your ideas as a feature request and we can discuss, if accepted you
+can provide a PR. We are looking for a more rigorous way link indicator and
+effectivess, until that is found discussion is the best we can do! # ð
+Quality Specs (& a Quality Standard) Often in Software Engineering code is both
+likely to go into production and likely to continue to be used once it does. In
+this enviroment it makes sense for codebases to have a single quality standard.
+In the **explore vs exploit** decision making [trade-off](https://
+en.wikipedia.org/wiki/Exploration-exploitation_dilemma) this environment could
+be classified as **high exploit**. For problems that are **high explore**, like
+most Data Science work, we argue that **a single quality bar is not
+sufficient**. `scilint` promotes adopting a *progressive consolidation*\*
+approach where exploration code starts with a speed of exploration goal and
+this may gradually shift to increase the emphasis on quality and reuse as the
+utility of the workflow becomes proven. This feature is known as âQuality
+Specsâ and it allows multiple different specifications of quality to exist
+within a project. The standard can be a relatively low bar for exploration work
+but can become more demanding as you are closer to the productionisation of
+your work. \**(term first used by [GaÃ«l Varoqouax](https://gael-
+varoquaux.info/); see [here](https://gael-varoquaux.info/programming/software-
+for-reproducible-science-lets-not-have-a-misunderstanding.html) for argument
+expansion).* ## Reference Quality Standard > The progressive consolidation
+workflow that we use on projects is the > reference implementation for
+`scilint` and is summarised in the below > image:
                               [Quality Standard]
 - **Legacy:** especially on larger projects there may be a large number of
 legacy notebooks that are not in use and no there is no obvious value in
 improving their quality. This could be removed from the workflow if you have
 enforced a quality standard from the outset. - **Exploratory:** exploratory
 workflows are typically off-line and involve much iteration. The benefit of
 some quality bar here is that it aids collaboration, review and generally helps
@@ -154,19 +155,19 @@
 is just a yaml configuration file of the properties of the quality spec. It
 contains threshold values for warning along with some other settings. To adopt
 a multi-spec standard place a spec file into each directory that you want to
 have different standards for. Look at `nbs/examples/nbs` to see an example of a
 multi-spec standard. --- exclusions: ~ fail_over: 1 out_dir: "/tmp/scilint/
 " precision: 3 print_syntax_errors: false evaluate: true warnings: lt:
 calls_per_func_median: 1 calls_per_func_mean: 1 in_func_pct: 20
-asserts_func_ratio: 1 inline_asserts_per_func_median: 0
-inline_asserts_per_func_mean: 0.5 markdown_code_pct: 5 gt: total_code_len:
-50000 loc_per_md_section: 2000 equals: has_syntax_error: true ## What does a
-lint report look like? The lint warnings are printed to the console and a more
-thorough report is generated and saved as a CSV file which looks like this:
+tests_func_coverage_pct: 20 tests_per_func_mean: 0.5 markdown_code_pct: 5 gt:
+total_code_len: 50000 loc_per_md_section: 2000 equals: has_syntax_error: true
+## What does a lint report look like? The lint warnings are printed to the
+console and a more thorough report is generated and saved as a CSV file which
+looks like this:
                                 [Sample Report]
 # ð Changing Behaviour - Recommended Usage Infusing quality into workflows
 is aided by having timely, short-cycle feedback of issues. Addtionally whatever
 quality bar you choose as a team, it should be non-negotiable that way you can
 spend time thinking about what matters like the problem you are trying to solve
 not nitpicking on small details repeatedly. We recommend using `scilint` in the
 following way to maximise benefit: 1. Decide upon a quality standard including
```

### Comparing `scilint-0.1.0/scilint/_modidx.py` & `scilint-0.2.0/scilint/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,50 +57,69 @@
                                                                                                    'scilint/exploratory/test_nbdev.py'),
                                                 'scilint.exploratory.test_nbdev.preprocess': ( 'example_nbs/exploratory/nbdev.html#preprocess',
                                                                                                'scilint/exploratory/test_nbdev.py'),
                                                 'scilint.exploratory.test_nbdev.serve_num_topics': ( 'example_nbs/exploratory/nbdev.html#serve_num_topics',
                                                                                                      'scilint/exploratory/test_nbdev.py'),
                                                 'scilint.exploratory.test_nbdev.something': ( 'example_nbs/exploratory/nbdev.html#something',
                                                                                               'scilint/exploratory/test_nbdev.py')},
+            'scilint.indicators': { 'scilint.indicators._check_for_function_asserts': ( 'indicators.html#_check_for_function_asserts',
+                                                                                        'scilint/indicators.py'),
+                                    'scilint.indicators._count_func_ret_asserts': ( 'indicators.html#_count_func_ret_asserts',
+                                                                                    'scilint/indicators.py'),
+                                    'scilint.indicators._count_inline_asserts': ( 'indicators.html#_count_inline_asserts',
+                                                                                  'scilint/indicators.py'),
+                                    'scilint.indicators._incr_assert_count': ( 'indicators.html#_incr_assert_count',
+                                                                               'scilint/indicators.py'),
+                                    'scilint.indicators._tests_per_function_code': ( 'indicators.html#_tests_per_function_code',
+                                                                                     'scilint/indicators.py'),
+                                    'scilint.indicators._update_ret_vals': ('indicators.html#_update_ret_vals', 'scilint/indicators.py'),
+                                    'scilint.indicators.calc_ifp': ('indicators.html#calc_ifp', 'scilint/indicators.py'),
+                                    'scilint.indicators.calls_per_func': ('indicators.html#calls_per_func', 'scilint/indicators.py'),
+                                    'scilint.indicators.calls_per_func_mean': ( 'indicators.html#calls_per_func_mean',
+                                                                                'scilint/indicators.py'),
+                                    'scilint.indicators.calls_per_func_median': ( 'indicators.html#calls_per_func_median',
+                                                                                  'scilint/indicators.py'),
+                                    'scilint.indicators.count_func_calls': ('indicators.html#count_func_calls', 'scilint/indicators.py'),
+                                    'scilint.indicators.get_cell_code': ('indicators.html#get_cell_code', 'scilint/indicators.py'),
+                                    'scilint.indicators.get_func_defs': ('indicators.html#get_func_defs', 'scilint/indicators.py'),
+                                    'scilint.indicators.get_project_root': ('indicators.html#get_project_root', 'scilint/indicators.py'),
+                                    'scilint.indicators.iaf': ('indicators.html#iaf', 'scilint/indicators.py'),
+                                    'scilint.indicators.in_func_pct': ('indicators.html#in_func_pct', 'scilint/indicators.py'),
+                                    'scilint.indicators.loc_per_md_section': ( 'indicators.html#loc_per_md_section',
+                                                                               'scilint/indicators.py'),
+                                    'scilint.indicators.markdown_code_pct': ('indicators.html#markdown_code_pct', 'scilint/indicators.py'),
+                                    'scilint.indicators.replace_ipython_magics': ( 'indicators.html#replace_ipython_magics',
+                                                                                   'scilint/indicators.py'),
+                                    'scilint.indicators.safe_div': ('indicators.html#safe_div', 'scilint/indicators.py'),
+                                    'scilint.indicators.tests_func_coverage_pct': ( 'indicators.html#tests_func_coverage_pct',
+                                                                                    'scilint/indicators.py'),
+                                    'scilint.indicators.tests_per_func_mean': ( 'indicators.html#tests_per_func_mean',
+                                                                                'scilint/indicators.py'),
+                                    'scilint.indicators.tests_per_function': ( 'indicators.html#tests_per_function',
+                                                                               'scilint/indicators.py'),
+                                    'scilint.indicators.total_code_len': ('indicators.html#total_code_len', 'scilint/indicators.py')},
             'scilint.scilint': { 'scilint.scilint._calculate_warnings': ('scilint.html#_calculate_warnings', 'scilint/scilint.py'),
                                  'scilint.scilint._get_excluded_paths': ('scilint.html#_get_excluded_paths', 'scilint/scilint.py'),
                                  'scilint.scilint._load_conf': ('scilint.html#_load_conf', 'scilint/scilint.py'),
                                  'scilint.scilint._map_paths_specs': ('scilint.html#_map_paths_specs', 'scilint/scilint.py'),
                                  'scilint.scilint._persist_results': ('scilint.html#_persist_results', 'scilint/scilint.py'),
                                  'scilint.scilint._reshape_warnings': ('scilint.html#_reshape_warnings', 'scilint/scilint.py'),
-                                 'scilint.scilint.afr': ('scilint.html#afr', 'scilint/scilint.py'),
                                  'scilint.scilint.build': ('scilint.html#build', 'scilint/scilint.py'),
-                                 'scilint.scilint.calc_ifp': ('scilint.html#calc_ifp', 'scilint/scilint.py'),
-                                 'scilint.scilint.calls_per_func': ('scilint.html#calls_per_func', 'scilint/scilint.py'),
-                                 'scilint.scilint.count_func_calls': ('scilint.html#count_func_calls', 'scilint/scilint.py'),
-                                 'scilint.scilint.count_inline_asserts': ('scilint.html#count_inline_asserts', 'scilint/scilint.py'),
                                  'scilint.scilint.display_warning_report': ('scilint.html#display_warning_report', 'scilint/scilint.py'),
-                                 'scilint.scilint.get_cell_code': ('scilint.html#get_cell_code', 'scilint/scilint.py'),
-                                 'scilint.scilint.get_func_defs': ('scilint.html#get_func_defs', 'scilint/scilint.py'),
+                                 'scilint.scilint.get_default_spec': ('scilint.html#get_default_spec', 'scilint/scilint.py'),
                                  'scilint.scilint.get_project_root': ('scilint.html#get_project_root', 'scilint/scilint.py'),
-                                 'scilint.scilint.iaf': ('scilint.html#iaf', 'scilint/scilint.py'),
-                                 'scilint.scilint.ifp': ('scilint.html#ifp', 'scilint/scilint.py'),
                                  'scilint.scilint.is_nbdev_project': ('scilint.html#is_nbdev_project', 'scilint/scilint.py'),
                                  'scilint.scilint.lint': ('scilint.html#lint', 'scilint/scilint.py'),
                                  'scilint.scilint.lint_nb': ('scilint.html#lint_nb', 'scilint/scilint.py'),
                                  'scilint.scilint.lint_nbs': ('scilint.html#lint_nbs', 'scilint/scilint.py'),
-                                 'scilint.scilint.loc_per_md_section': ('scilint.html#loc_per_md_section', 'scilint/scilint.py'),
-                                 'scilint.scilint.mcp': ('scilint.html#mcp', 'scilint/scilint.py'),
-                                 'scilint.scilint.mean_cpf': ('scilint.html#mean_cpf', 'scilint/scilint.py'),
-                                 'scilint.scilint.mean_iaf': ('scilint.html#mean_iaf', 'scilint/scilint.py'),
-                                 'scilint.scilint.median_cpf': ('scilint.html#median_cpf', 'scilint/scilint.py'),
-                                 'scilint.scilint.median_iaf': ('scilint.html#median_iaf', 'scilint/scilint.py'),
-                                 'scilint.scilint.replace_ipython_magics': ('scilint.html#replace_ipython_magics', 'scilint/scilint.py'),
                                  'scilint.scilint.run_nbqa_cmd': ('scilint.html#run_nbqa_cmd', 'scilint/scilint.py'),
-                                 'scilint.scilint.safe_div': ('scilint.html#safe_div', 'scilint/scilint.py'),
                                  'scilint.scilint.scilint_build': ('scilint.html#scilint_build', 'scilint/scilint.py'),
                                  'scilint.scilint.scilint_ci': ('scilint.html#scilint_ci', 'scilint/scilint.py'),
                                  'scilint.scilint.scilint_lint': ('scilint.html#scilint_lint', 'scilint/scilint.py'),
                                  'scilint.scilint.scilint_tidy': ('scilint.html#scilint_tidy', 'scilint/scilint.py'),
-                                 'scilint.scilint.tcl': ('scilint.html#tcl', 'scilint/scilint.py'),
                                  'scilint.scilint.tidy': ('scilint.html#tidy', 'scilint/scilint.py')},
             'scilint.test.test_nbdev': { 'scilint.test.test_nbdev.Topics': ( 'example_nbs/no_spec_provided/nbdev.html#topics',
                                                                              'scilint/test/test_nbdev.py'),
                                          'scilint.test.test_nbdev.Topics.__init__': ( 'example_nbs/no_spec_provided/nbdev.html#topics.__init__',
                                                                                       'scilint/test/test_nbdev.py'),
                                          'scilint.test.test_nbdev.Topics.get_num_topics': ( 'example_nbs/no_spec_provided/nbdev.html#topics.get_num_topics',
                                                                                             'scilint/test/test_nbdev.py'),
```

### Comparing `scilint-0.1.0/scilint/experimental/test_nbdev.py` & `scilint-0.2.0/scilint/experimental/test_nbdev.py`

 * *Files identical despite different names*

### Comparing `scilint-0.1.0/scilint/exploratory/test_nbdev.py` & `scilint-0.2.0/scilint/exploratory/test_nbdev.py`

 * *Files identical despite different names*

### Comparing `scilint-0.1.0/scilint/scilint.py` & `scilint-0.2.0/scilint/scilint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/scilint.ipynb.
 
 # %% auto 0
-__all__ = ['indicator_funcs', 'run_nbqa_cmd', 'tidy', 'get_project_root', 'is_nbdev_project', 'get_func_defs', 'count_func_calls',
-           'replace_ipython_magics', 'safe_div', 'get_cell_code', 'calls_per_func', 'mean_cpf', 'median_cpf', 'afr',
-           'count_inline_asserts', 'iaf', 'mean_iaf', 'median_iaf', 'calc_ifp', 'ifp', 'mcp', 'tcl',
-           'loc_per_md_section', 'lint_nb', 'lint_nbs', 'display_warning_report', 'lint', 'build', 'scilint_tidy',
-           'scilint_lint', 'scilint_build', 'scilint_ci']
+__all__ = ['run_nbqa_cmd', 'tidy', 'get_project_root', 'is_nbdev_project', 'get_default_spec', 'lint_nb', 'lint_nbs',
+           'display_warning_report', 'lint', 'build', 'scilint_tidy', 'scilint_lint', 'scilint_build', 'scilint_ci']
 
 # %% ../nbs/scilint.ipynb 2
-import ast
 import json
 import operator
 import os
-import re
 import shutil
 import sys
-import warnings
-from collections import Counter
 from configparser import InterpolationMissingOptionError
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, Tuple
 
-import nbformat
 import numpy as np
 import pandas as pd
 import yaml
 from execnb.nbio import read_nb
 from fastcore.script import Param, call_parse, store_false
 from fastcore.xtras import globtastic
 from nbdev.clean import nbdev_clean
@@ -33,14 +25,16 @@
 from nbdev.doclinks import nbdev_export, nbglob
 from nbdev.quarto import nbdev_docs, nbdev_readme
 from nbdev.test import nbdev_test
 from nbqa.__main__ import _get_configs, _main
 from nbqa.cmdline import CLIArgs
 from nbqa.find_root import find_project_root
 
+from .indicators import indicator_funcs
+
 # %% ../nbs/scilint.ipynb 7
 def run_nbqa_cmd(cmd):
     print(f"Running {cmd}")
     project_root: Path = find_project_root(tuple([str(Path(".").resolve())]))
     args = CLIArgs.parse_args([cmd, str(project_root)])
     configs = _get_configs(args, project_root)
     output_code = _main(args, configs)
@@ -66,210 +60,38 @@
         get_config().lib_name
     except InterpolationMissingOptionError:
         is_nbdev = False
 
     return is_nbdev
 
 # %% ../nbs/scilint.ipynb 15
-def get_func_defs(code, ignore_private_prefix=True):
-    func_names = []
-    for stmt in ast.walk(ast.parse(code)):
-        if isinstance(stmt, ast.FunctionDef):
-            inner_cond = (
-                False if ignore_private_prefix and stmt.name.startswith("_") else True
-            )
-            if inner_cond:
-                func_names.append(stmt.name)
-    return func_names
-
-# %% ../nbs/scilint.ipynb 17
-def count_func_calls(code, func_defs):
-    func_calls = Counter({k: 0 for k in func_defs})
-    for stmt in ast.walk(ast.parse(code)):
-        if isinstance(stmt, ast.Call):
-            if type(stmt.func) == ast.Subscript:
-                func_name = stmt.func.value.id
-            else:
-                func_name = (
-                    stmt.func.id if "id" in stmt.func.__dict__ else stmt.func.attr
-                )
-            if func_name in func_defs:
-                if func_name in func_calls:
-                    func_calls[func_name] += 1
-    return func_calls
-
-# %% ../nbs/scilint.ipynb 21
-def replace_ipython_magics(code):
-    # Replace Ipython magic and shell command symbol with comment
-    code = code.replace("%", "#")
-    code = re.sub(r"^!", "#", code)
-    return re.sub(r"\n\W?!", "\n#", code)
-
-# %% ../nbs/scilint.ipynb 23
-def safe_div(numer, denom):
-    return 0 if denom == 0 else numer / denom
-
-# %% ../nbs/scilint.ipynb 25
-def get_cell_code(nb):
-    pnb = nbformat.from_dict(nb)
-    nb_cell_code = "\n".join(
-        [
-            replace_ipython_magics(c["source"])
-            for c in pnb.cells
-            if c["cell_type"] == "code"
-        ]
-    )
-    return nb_cell_code
-
-# %% ../nbs/scilint.ipynb 28
-def calls_per_func(nb):
-    nb_cell_code = get_cell_code(nb)
-    func_defs = get_func_defs(nb_cell_code)
-    func_calls = count_func_calls(nb_cell_code, func_defs)
-    return func_calls
-
-# %% ../nbs/scilint.ipynb 29
-def mean_cpf(nb):
-    return pd.Series(calls_per_func(nb)).mean()
+def get_default_spec():
+    return {
+        "exclusions": None,
+        "fail_over": 1,
+        "out_dir": "/tmp/scilint/",
+        "precision": 3,
+        "print_syntax_errors": False,
+        "evaluate": True,
+        "warnings": {
+            "lt": {
+                "calls_per_func_median": 0,
+                "calls_per_func_mean": 1,
+                "in_func_pct": 20,
+                "asserts_func_ratio": 1,
+                "tests_func_coverage_pct": 20,
+                "tests_per_func_mean": 0.5,
+                "markdown_code_pct": 5,
+            },
+            "gt": {"total_code_len": 50000, "loc_per_md_section": 2000},
+            "equals": {"has_syntax_error": True},
+        },
+    }
 
-# %% ../nbs/scilint.ipynb 30
-def median_cpf(nb):
-    with warnings.catch_warnings():
-        warnings.filterwarnings(action="ignore", message="Mean of empty slice")
-        return pd.Series(calls_per_func(nb)).median()
-
-# %% ../nbs/scilint.ipynb 38
-def afr(nb):
-    nb_cell_code = get_cell_code(nb)
-    if nb_cell_code == "":  # no code cells - metric is not well defined
-        return np.nan
-    func_defs = get_func_defs(nb_cell_code)
-    num_funcs = len(func_defs)
-
-    assert_count = 0
-    for stmt in ast.walk(ast.parse(nb_cell_code)):
-        if isinstance(stmt, ast.Assert):
-            assert_count += 1
-
-    return safe_div(assert_count, num_funcs)
-
-# %% ../nbs/scilint.ipynb 41
-def count_inline_asserts(code, func_defs):
-    inline_func_asserts = Counter({k: 0 for k in func_defs})
-
-    for stmt in ast.walk(ast.parse(code)):
-        if isinstance(stmt, ast.Assert):
-            for assert_st in ast.walk(stmt):
-                if isinstance(assert_st, ast.Call):
-                    func_name = (
-                        assert_st.func.id
-                        if "id" in assert_st.func.__dict__
-                        else assert_st.func.attr
-                    )
-                    if func_name in inline_func_asserts:
-                        inline_func_asserts[func_name] += 1
-    return inline_func_asserts
-
-# %% ../nbs/scilint.ipynb 42
-def iaf(nb):
-    nb_cell_code = get_cell_code(nb)
-    if nb_cell_code == "":
-        return np.nan
-    func_defs = get_func_defs(nb_cell_code)
-    return count_inline_asserts(nb_cell_code, func_defs)
-
-# %% ../nbs/scilint.ipynb 49
-def mean_iaf(nb):
-    return pd.Series(iaf(nb)).mean()
-
-# %% ../nbs/scilint.ipynb 50
-def median_iaf(nb):
-    with warnings.catch_warnings():
-        warnings.filterwarnings(action="ignore", message="Mean of empty slice")
-        return pd.Series(iaf(nb)).median()
-
-# %% ../nbs/scilint.ipynb 53
-def calc_ifp(nb_cell_code):
-    stmts_in_func = 0
-    stmts_outside_func = 0
-    for stmt in ast.walk(ast.parse(replace_ipython_magics(nb_cell_code))):
-        if isinstance(stmt, ast.FunctionDef) and not stmt.name.startswith("_"):
-            for body_item in stmt.body:
-                stmts_in_func += 1
-        elif isinstance(stmt, ast.Module):
-            for body_item in stmt.body:
-                if not isinstance(body_item, ast.FunctionDef):
-                    stmts_outside_func += 1
-    return (
-        0
-        if stmts_outside_func + stmts_in_func == 0
-        else (stmts_in_func / (stmts_outside_func + stmts_in_func)) * 100
-    )
-
-# %% ../nbs/scilint.ipynb 55
-def ifp(nb):
-    nb_cell_code = "\n".join(
-        [
-            replace_ipython_magics(c["source"])
-            for c in nb.cells
-            if c["cell_type"] == "code"
-        ]
-    )
-    if nb_cell_code == "":
-        return np.nan
-    return calc_ifp(nb_cell_code)
-
-# %% ../nbs/scilint.ipynb 58
-def mcp(nb):
-    md_cells = [c for c in nb.cells if c["cell_type"] == "markdown"]
-    code_cells = [c for c in nb.cells if c["cell_type"] == "code"]
-    num_code_cells = len(code_cells)
-    if num_code_cells == 0:
-        return np.nan
-    num_md_cells = len(md_cells)
-    return (
-        100
-        if num_code_cells == 0
-        else (num_md_cells / (num_md_cells + num_code_cells)) * 100
-    )
-
-# %% ../nbs/scilint.ipynb 61
-def tcl(nb):
-    return sum([len(c["source"]) for c in nb.cells if c["cell_type"] == "code"])
-
-# %% ../nbs/scilint.ipynb 64
-def loc_per_md_section(nb):
-    num_md_sections = len(
-        [
-            c["source"]
-            for c in nb.cells
-            if c["cell_type"] == "markdown" and c["source"].strip().startswith("#")
-        ]
-    )
-    total_code_len = tcl(nb)
-    if total_code_len == 0 or num_md_sections == 0:
-        result = np.nan
-    else:
-        result = tcl(nb) / num_md_sections
-    return result
-
-# %% ../nbs/scilint.ipynb 67
-indicator_funcs = {
-    "calls_per_func_mean": mean_cpf,
-    "calls_per_func_median": median_cpf,
-    "asserts_func_ratio": afr,
-    "inline_asserts_per_func_mean": mean_iaf,
-    "inline_asserts_per_func_median": median_iaf,
-    "in_func_pct": ifp,
-    "markdown_code_pct": mcp,
-    "loc_per_md_section": loc_per_md_section,
-    "total_code_len": tcl,
-}
-
-# %% ../nbs/scilint.ipynb 70
+# %% ../nbs/scilint.ipynb 18
 def lint_nb(
     spec_name: str,
     nb_path: Path,
     conf: Dict[str, Any],
     indicators: Dict[str, Callable],
     include_in_scoring: bool,
 ) -> Tuple[float]:
@@ -286,15 +108,15 @@
         has_syntax_error = True
     indic_vals.append(has_syntax_error)
     indic_vals.append(include_in_scoring)
     indic_vals.insert(0, spec_name)
 
     return tuple(indic_vals)
 
-# %% ../nbs/scilint.ipynb 72
+# %% ../nbs/scilint.ipynb 21
 def _get_excluded_paths(paths: Iterable[Path], exclude_pattern: str) -> Iterable[Path]:
     """Excluded paths should either be absolute paths or paths rooted at the project root directory"""
     excl_paths = []
     paths = [p.absolute() for p in paths]
 
     for ex_pattern in exclude_pattern.split(","):
         if Path(ex_pattern).is_absolute():
@@ -308,15 +130,15 @@
             raise ValueError(f"Path component: {ex_path} does not exist")
         else:
             raise ValueError(
                 f"Invalid exclusion pattern: {ex_path} pattern is comma separrated list of 'dir/' for directories and 'name.ipynb' for specific notebook"
             )
     return excl_paths
 
-# %% ../nbs/scilint.ipynb 75
+# %% ../nbs/scilint.ipynb 24
 def _calculate_warnings(
     spec_name: str,
     scoring_report: pd.DataFrame,
     conf: Dict[str, Any],
     include_missing: bool = False,
 ) -> Tuple[Dict[str, Any], int]:
     warning_details = []
@@ -345,15 +167,15 @@
                 )
             warning_details.append(warning_dict)
 
     all_warns = _reshape_warnings(spec_name, scoring_report, warning_details)
     num_warnings = len(all_warns)
     return all_warns, num_warnings
 
-# %% ../nbs/scilint.ipynb 77
+# %% ../nbs/scilint.ipynb 27
 def _reshape_warnings(
     spec_name: str, scoring_report: pd.DataFrame, warning_details: Iterable[Any]
 ) -> Dict[str, Iterable[Tuple]]:
     warnings_by_nb = {nb: [] for nb in scoring_report.index}
     for nb in scoring_report.index:
         for wd in warning_details:
             if nb in wd:
@@ -368,15 +190,15 @@
             "indicator",
             "value",
             "operator",
             "threshold",
         ],
     )
 
-# %% ../nbs/scilint.ipynb 79
+# %% ../nbs/scilint.ipynb 30
 def lint_nbs(
     spec_name: str,
     conf: Dict[str, Any],
     indicators: Dict[str, Callable],
     nb_paths: Iterable[Path] = None,
     nb_glob: Path = None,
 ):
@@ -412,15 +234,15 @@
         + ["has_syntax_error", "include_in_scoring"],
     ).sort_values(["in_func_pct", "markdown_code_pct"], ascending=False)
 
     scoring_report = lint_report[lint_report.include_in_scoring].copy()
     all_warns, num_warnings = _calculate_warnings(spec_name, scoring_report, conf)
     return lint_report, all_warns, num_warnings
 
-# %% ../nbs/scilint.ipynb 81
+# %% ../nbs/scilint.ipynb 32
 def _map_paths_specs(nb_glob: Path = None, specs_glob: Path = Path(".").resolve()):
     nbs = nbglob(nb_glob)
     spec_files = [
         Path(p)
         for p in globtastic(
             specs_glob,
             file_glob="scilint-*.yaml",
@@ -446,38 +268,38 @@
                 fallback_path = Path("scilint-default")
                 if fallback_path not in spec_nbs:
                     spec_nbs[fallback_path] = []
                 spec_nbs[fallback_path].append(nb)
 
     return spec_nbs
 
-# %% ../nbs/scilint.ipynb 96
+# %% ../nbs/scilint.ipynb 47
 def display_warning_report(all_warns: pd.DataFrame):
     print(
         "\n******************************************Begin Scilint Warning Report*****************************************"
     )
     print(all_warns.to_markdown(tablefmt="grid", index=False))
     print(
         "\n******************************************End Scilint Warning Report*******************************************\n"
     )
 
-# %% ../nbs/scilint.ipynb 98
+# %% ../nbs/scilint.ipynb 49
 def _persist_results(
     lint_report: pd.DataFrame, all_warns: pd.DataFrame, conf: Dict[str, Any]
 ):
     out_dir = Path(conf["out_dir"])
     conf_to_persist = {k: v for k, v in conf.items() if k != "indicators"}
     if not out_dir.exists():
         Path(out_dir).mkdir()
     with open(Path(out_dir, "scilint_config.json"), "w") as outfile:
         json.dump(conf_to_persist, outfile)
     all_warns.to_csv(Path(out_dir, "scilint_warnings.csv"), index=False)
     lint_report.to_csv(Path(out_dir, "scilint_report.csv"))
 
-# %% ../nbs/scilint.ipynb 101
+# %% ../nbs/scilint.ipynb 52
 def _load_conf(
     conf_path: str = None,
     exclusions: str = None,
     fail_over: int = None,
     out_dir: int = None,
     precision: int = None,
     print_syntax_errors: bool = None,
@@ -499,15 +321,15 @@
     )
     overrides = (exclusions, fail_over, out_dir, precision, print_syntax_errors)
     for override in zip(override_names, overrides):
         if override[1] is not None:
             conf[override[0]] = override[1]
     return conf
 
-# %% ../nbs/scilint.ipynb 105
+# %% ../nbs/scilint.ipynb 56
 def lint(
     display_report: bool = True,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
     out_dir: int = None,
@@ -562,15 +384,15 @@
             display_warning_report(all_warns)
     elif num_warnings == 0:
         print("No issues found during linting")
 
     _persist_results(lint_report, all_warns, conf)
     print("Linting completed")
 
-# %% ../nbs/scilint.ipynb 108
+# %% ../nbs/scilint.ipynb 59
 def build(
     display_report: bool = True,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
     out_dir: int = None,
@@ -595,20 +417,20 @@
         precision,
         print_syntax_errors,
     )
     if is_nbdev_project():
         nbdev_clean.__wrapped__()
         print("Cleaned notebooks")
 
-# %% ../nbs/scilint.ipynb 111
+# %% ../nbs/scilint.ipynb 62
 @call_parse
 def scilint_tidy():
     tidy()
 
-# %% ../nbs/scilint.ipynb 113
+# %% ../nbs/scilint.ipynb 64
 @call_parse
 def scilint_lint(
     display_report: Param("Print the lint report", store_false) = False,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
@@ -623,15 +445,15 @@
         exclusions,
         fail_over,
         out_dir,
         precision,
         print_syntax_errors,
     )
 
-# %% ../nbs/scilint.ipynb 116
+# %% ../nbs/scilint.ipynb 67
 @call_parse
 def scilint_build(
     display_report: Param("Print the lint report", store_false) = False,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
@@ -646,15 +468,15 @@
         exclusions,
         fail_over,
         out_dir,
         precision,
         print_syntax_errors,
     )
 
-# %% ../nbs/scilint.ipynb 118
+# %% ../nbs/scilint.ipynb 69
 @call_parse
 def scilint_ci(
     display_report: Param("Print the lint report", store_false) = False,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
```

### Comparing `scilint-0.1.0/scilint/test/test_nbdev.py` & `scilint-0.2.0/scilint/test/test_nbdev.py`

 * *Files identical despite different names*

### Comparing `scilint-0.1.0/scilint/test/test_nbdev_high_quality.py` & `scilint-0.2.0/scilint/test/test_nbdev_high_quality.py`

 * *Files identical despite different names*

### Comparing `scilint-0.1.0/scilint/validated/test_nbdev_high_quality.py` & `scilint-0.2.0/scilint/validated/test_nbdev_high_quality.py`

 * *Files identical despite different names*

### Comparing `scilint-0.1.0/scilint.egg-info/PKG-INFO` & `scilint-0.2.0/scilint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilint
-Version: 0.1.0
+Version: 0.2.0
 Summary: infuse quality into notebook based workflows with a new type of build tool.
 Home-page: https://github.com/newday-data/scilint/tree/{branch}/
 Author: Donal Simmie
 Author-email: oss@newday.co.uk
 License: Apache Software License 2.0
 Project-URL: Documentation, https://newday-data.github.io/scilint/
 Keywords: research,production,exploration,CI/CD
@@ -196,32 +196,33 @@
 
 The below are potential quality indicators that you can use to set a
 minimum bar for quality and comprehensibility within your projects.
 These are not exhaustive or definite quality indicators - they are a
 starting point to open the conversation about what it means to have a
 high quality notebook in practice.
 
-1.  **Calls-Per-Function (CPF):** compares the amount of calls to the
-    amount of functions. Looks for possible relationship between
-    function definitions and usage.
-2.  **In-Function-Percent (IFP):** the percentage of code that is within
-    a function rather than outside function scope.
-3.  **Asserts-Per-Function (APF):** looks at how many tests (where
-    assert = test) there are compared to the total function count.
-4.  **InlineAssertsPerFunction (IAF):** examines how many times a
-    function is called within an assert statement - this aims to see
-    testing of functions not just usage.
-5.  **MarkdownToCodeRatio (MCP):** what is the ratio of markdown cells
-    to code cells.
-6.  **TotalCodeLen (TCL):** the total line length of the notebook code
+1.  Calls-Per-Function (CPF):\*\* compares the **amount of calls to the
+    amount of functions**. *Looks for possible relationship between
+    function definitions and usage.*
+2.  In-Function-Percent (IFP): the **percentage of code that is within a
+    function** rather than outside function scope.
+3.  Tests-Per-Function-Mean (TPF: the **average number of tests (where
+    test==assert) for all functions**. *Mean value so may be dominated
+    by outliers.*
+4.  Tests-Function-Coverage-Pct (TFC): what **percentage of all
+    functions have at least one test**. *Note: this is coverage at
+    function-level not line-based coverage.*
+5.  MarkdownToCodeRatio (MCP): what is the **ratio of markdown cells to
+    code cells**.
+6.  TotalCodeLen (TCL): the **total line length** of the notebook code
     cells.
-7.  **Loc-Per-MD-Section:** the lines of code per Markdown section
+7.  Loc-Per-MD-Section (LPS): the **lines of code per Markdown section**
     header.
-8.  **SyntaxErrors**: if the code within the notebook has invalid Python
-    syntax.
+8.  SyntaxErrors (SYN): if the code within the notebook has **invalid
+    Python syntax**.
 
 > *as already stated there is no definitive answer as to whether any of
 > these are low or high quality. However there are reasons to believe
 > inituitively that higher or lower values of the above will produce
 > higher quality notebooks. There are many questions left to answer,
 > like the role of docstrings, comments and type annotations; their
 > effectiveness may warrant inclusion but that is an open question at
@@ -306,17 +307,16 @@
       print_syntax_errors: false
       evaluate: true
       warnings:
         lt:
           calls_per_func_median: 1
           calls_per_func_mean: 1
           in_func_pct: 20
-          asserts_func_ratio: 1
-          inline_asserts_per_func_median: 0
-          inline_asserts_per_func_mean: 0.5
+          tests_func_coverage_pct: 20
+          tests_per_func_mean: 0.5
           markdown_code_pct: 5
         gt:
           total_code_len: 50000
           loc_per_md_section: 2000
         equals:
           has_syntax_error: true
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scilint Version: 0.1.0 Summary: infuse quality into
+Metadata-Version: 2.1 Name: scilint Version: 0.2.0 Summary: infuse quality into
 notebook based workflows with a new type of build tool. Home-page: https://
 github.com/newday-data/scilint/tree/{branch}/ Author: Donal Simmie Author-
 email: oss@newday.co.uk License: Apache Software License 2.0 Project-URL:
 Documentation, https://newday-data.github.io/scilint/ Keywords:
 research,production,exploration,CI/CD Platform: UNKNOWN Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Programming Language ::
@@ -101,57 +101,58 @@
 quarto build. Quarto is a core part of the nbdev system, if you are having
 trouble installing it, check out the `nbdev` Github [page](https://github.com/
 fastai/nbdev). For more details on the Quarto project, check out their home
 [page](https://quarto.org/). # ð Quality Indicators The below are potential
 quality indicators that you can use to set a minimum bar for quality and
 comprehensibility within your projects. These are not exhaustive or definite
 quality indicators - they are a starting point to open the conversation about
-what it means to have a high quality notebook in practice. 1. **Calls-Per-
-Function (CPF):** compares the amount of calls to the amount of functions.
-Looks for possible relationship between function definitions and usage. 2.
-**In-Function-Percent (IFP):** the percentage of code that is within a function
-rather than outside function scope. 3. **Asserts-Per-Function (APF):** looks at
-how many tests (where assert = test) there are compared to the total function
-count. 4. **InlineAssertsPerFunction (IAF):** examines how many times a
-function is called within an assert statement - this aims to see testing of
-functions not just usage. 5. **MarkdownToCodeRatio (MCP):** what is the ratio
-of markdown cells to code cells. 6. **TotalCodeLen (TCL):** the total line
-length of the notebook code cells. 7. **Loc-Per-MD-Section:** the lines of code
-per Markdown section header. 8. **SyntaxErrors**: if the code within the
-notebook has invalid Python syntax. > *as already stated there is no definitive
-answer as to whether any of > these are low or high quality. However there are
-reasons to believe > inituitively that higher or lower values of the above will
-produce > higher quality notebooks. There are many questions left to answer, >
-like the role of docstrings, comments and type annotations; their >
-effectiveness may warrant inclusion but that is an open question at > the
-moment. As this library is used and refined with more projects and > more
-experimental metrics then these intuitions can evaluated more > rigorously.* ##
-â Adding New Indicators For now post your ideas as a feature request and we
-can discuss, if accepted you can provide a PR. We are looking for a more
-rigorous way link indicator and effectivess, until that is found discussion is
-the best we can do! # ð Quality Specs (& a Quality Standard) Often in
-Software Engineering code is both likely to go into production and likely to
-continue to be used once it does. In this enviroment it makes sense for
-codebases to have a single quality standard. In the **explore vs exploit**
-decision making [trade-off](https://en.wikipedia.org/wiki/Exploration-
-exploitation_dilemma) this environment could be classified as **high exploit**.
-For problems that are **high explore**, like most Data Science work, we argue
-that **a single quality bar is not sufficient**. `scilint` promotes adopting a
-*progressive consolidation*\* approach where exploration code starts with a
-speed of exploration goal and this may gradually shift to increase the emphasis
-on quality and reuse as the utility of the workflow becomes proven. This
-feature is known as âQuality Specsâ and it allows multiple different
-specifications of quality to exist within a project. The standard can be a
-relatively low bar for exploration work but can become more demanding as you
-are closer to the productionisation of your work. \**(term first used by [GaÃ«l
-Varoqouax](https://gael-varoquaux.info/); see [here](https://gael-
-varoquaux.info/programming/software-for-reproducible-science-lets-not-have-a-
-misunderstanding.html) for argument expansion).* ## Reference Quality Standard
-> The progressive consolidation workflow that we use on projects is the >
-reference implementation for `scilint` and is summarised in the below > image:
+what it means to have a high quality notebook in practice. 1. Calls-Per-
+Function (CPF):\*\* compares the **amount of calls to the amount of
+functions**. *Looks for possible relationship between function definitions and
+usage.* 2. In-Function-Percent (IFP): the **percentage of code that is within a
+function** rather than outside function scope. 3. Tests-Per-Function-Mean (TPF:
+the **average number of tests (where test==assert) for all functions**. *Mean
+value so may be dominated by outliers.* 4. Tests-Function-Coverage-Pct (TFC):
+what **percentage of all functions have at least one test**. *Note: this is
+coverage at function-level not line-based coverage.* 5. MarkdownToCodeRatio
+(MCP): what is the **ratio of markdown cells to code cells**. 6. TotalCodeLen
+(TCL): the **total line length** of the notebook code cells. 7. Loc-Per-MD-
+Section (LPS): the **lines of code per Markdown section** header. 8.
+SyntaxErrors (SYN): if the code within the notebook has **invalid Python
+syntax**. > *as already stated there is no definitive answer as to whether any
+of > these are low or high quality. However there are reasons to believe >
+inituitively that higher or lower values of the above will produce > higher
+quality notebooks. There are many questions left to answer, > like the role of
+docstrings, comments and type annotations; their > effectiveness may warrant
+inclusion but that is an open question at > the moment. As this library is used
+and refined with more projects and > more experimental metrics then these
+intuitions can evaluated more > rigorously.* ## â Adding New Indicators For
+now post your ideas as a feature request and we can discuss, if accepted you
+can provide a PR. We are looking for a more rigorous way link indicator and
+effectivess, until that is found discussion is the best we can do! # ð
+Quality Specs (& a Quality Standard) Often in Software Engineering code is both
+likely to go into production and likely to continue to be used once it does. In
+this enviroment it makes sense for codebases to have a single quality standard.
+In the **explore vs exploit** decision making [trade-off](https://
+en.wikipedia.org/wiki/Exploration-exploitation_dilemma) this environment could
+be classified as **high exploit**. For problems that are **high explore**, like
+most Data Science work, we argue that **a single quality bar is not
+sufficient**. `scilint` promotes adopting a *progressive consolidation*\*
+approach where exploration code starts with a speed of exploration goal and
+this may gradually shift to increase the emphasis on quality and reuse as the
+utility of the workflow becomes proven. This feature is known as âQuality
+Specsâ and it allows multiple different specifications of quality to exist
+within a project. The standard can be a relatively low bar for exploration work
+but can become more demanding as you are closer to the productionisation of
+your work. \**(term first used by [GaÃ«l Varoqouax](https://gael-
+varoquaux.info/); see [here](https://gael-varoquaux.info/programming/software-
+for-reproducible-science-lets-not-have-a-misunderstanding.html) for argument
+expansion).* ## Reference Quality Standard > The progressive consolidation
+workflow that we use on projects is the > reference implementation for
+`scilint` and is summarised in the below > image:
                               [Quality Standard]
 - **Legacy:** especially on larger projects there may be a large number of
 legacy notebooks that are not in use and no there is no obvious value in
 improving their quality. This could be removed from the workflow if you have
 enforced a quality standard from the outset. - **Exploratory:** exploratory
 workflows are typically off-line and involve much iteration. The benefit of
 some quality bar here is that it aids collaboration, review and generally helps
@@ -166,19 +167,19 @@
 is just a yaml configuration file of the properties of the quality spec. It
 contains threshold values for warning along with some other settings. To adopt
 a multi-spec standard place a spec file into each directory that you want to
 have different standards for. Look at `nbs/examples/nbs` to see an example of a
 multi-spec standard. --- exclusions: ~ fail_over: 1 out_dir: "/tmp/scilint/
 " precision: 3 print_syntax_errors: false evaluate: true warnings: lt:
 calls_per_func_median: 1 calls_per_func_mean: 1 in_func_pct: 20
-asserts_func_ratio: 1 inline_asserts_per_func_median: 0
-inline_asserts_per_func_mean: 0.5 markdown_code_pct: 5 gt: total_code_len:
-50000 loc_per_md_section: 2000 equals: has_syntax_error: true ## What does a
-lint report look like? The lint warnings are printed to the console and a more
-thorough report is generated and saved as a CSV file which looks like this:
+tests_func_coverage_pct: 20 tests_per_func_mean: 0.5 markdown_code_pct: 5 gt:
+total_code_len: 50000 loc_per_md_section: 2000 equals: has_syntax_error: true
+## What does a lint report look like? The lint warnings are printed to the
+console and a more thorough report is generated and saved as a CSV file which
+looks like this:
                                 [Sample Report]
 # ð Changing Behaviour - Recommended Usage Infusing quality into workflows
 is aided by having timely, short-cycle feedback of issues. Addtionally whatever
 quality bar you choose as a team, it should be non-negotiable that way you can
 spend time thinking about what matters like the problem you are trying to solve
 not nitpicking on small details repeatedly. We recommend using `scilint` in the
 following way to maximise benefit: 1. Decide upon a quality standard including
```

### Comparing `scilint-0.1.0/scilint.egg-info/SOURCES.txt` & `scilint-0.2.0/scilint.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 NOTICE
 README.md
 pyproject.toml
 setup.py
 scilint/__init__.py
 scilint/_modidx.py
+scilint/indicators.py
 scilint/scilint.py
 scilint.egg-info/PKG-INFO
 scilint.egg-info/SOURCES.txt
 scilint.egg-info/dependency_links.txt
 scilint.egg-info/entry_points.txt
 scilint.egg-info/not-zip-safe
 scilint.egg-info/requires.txt
```

### Comparing `scilint-0.1.0/setup.py` & `scilint-0.2.0/setup.py`

 * *Files identical despite different names*

