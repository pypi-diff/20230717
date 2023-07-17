# Comparing `tmp/bowtie_json_schema-2023.7.7.tar.gz` & `tmp/bowtie_json_schema-2023.7.8.tar.gz`

## Comparing `bowtie_json_schema-2023.7.7.tar` & `bowtie_json_schema-2023.7.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.flake8
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.readthedocs.yml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/test-requirements.in
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/SECURITY.md
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/release.yml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/workflows/build-frontend.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/workflows/deploy-frontend.yml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/workflows/images.yml
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/__main__.py
--rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/cli.rst
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/conf.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/requirements.in
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/requirements.txt
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/docs/_static/dreamed.png
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/.eslintrc.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/index.html
--rw-r--r--   0        0        0   165159 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/package-lock.json
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/package.json
--rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/tsconfig.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/vite.config.js
--rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/public/favicon.ico
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/MainContainer.jsx
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/ReportDataHandler.jsx
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/ReportView.jsx
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/index.jsx
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/CopyToClipboard.jsx
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/LoadingAnimation.jsx
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/NavBar.jsx
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Cases/AccordionItem.jsx
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Cases/AccordionSvg.jsx
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Cases/CasesSection.jsx
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Cases/SchemaDisplay.jsx
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/DragAndDrop/DragAndDrop.jsx
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Modals/DetailsButtonModal.jsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Modals/RunTimeInfoModal.jsx
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/RunInfo/RunInfoSection.jsx
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Summary/ImplementationRow.jsx
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Summary/SummarySection.jsx
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/components/Summary/SummaryTable.jsx
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/context/BowtieVersionContext.jsx
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/context/ThemeContext.jsx
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/LICENSE
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/README.rst
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/pyproject.toml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.7/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.flake8
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.readthedocs.yml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/test-requirements.in
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/SECURITY.md
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/release.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/build-frontend.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/deploy-frontend.yml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/images.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/__main__.py
+-rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/cli.rst
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/conf.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/requirements.in
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/requirements.txt
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/_static/dreamed.png
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/.eslintrc.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/index.html
+-rw-r--r--   0        0        0   165159 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/package-lock.json
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/package.json
+-rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/tsconfig.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/vite.config.js
+-rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/public/favicon.ico
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/MainContainer.jsx
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/ReportDataHandler.jsx
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/ReportView.jsx
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/index.jsx
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/CopyToClipboard.jsx
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/LoadingAnimation.jsx
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/NavBar.jsx
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionItem.jsx
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionSvg.jsx
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/CasesSection.jsx
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/SchemaDisplay.jsx
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/DragAndDrop/DragAndDrop.jsx
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Modals/DetailsButtonModal.jsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Modals/RunTimeInfoModal.jsx
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/RunInfo/RunInfoSection.jsx
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.jsx
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummarySection.jsx
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummaryTable.jsx
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/context/BowtieVersionContext.jsx
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/context/ThemeContext.jsx
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/README.rst
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/pyproject.toml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.7.7/.flake8` & `bowtie_json_schema-2023.7.8/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.pre-commit-config.yaml` & `bowtie_json_schema-2023.7.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/noxfile.py` & `bowtie_json_schema-2023.7.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/test-requirements.txt` & `bowtie_json_schema-2023.7.8/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.github/SECURITY.md` & `bowtie_json_schema-2023.7.8/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.github/dependabot.yml` & `bowtie_json_schema-2023.7.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.github/workflows/build-frontend.yml` & `bowtie_json_schema-2023.7.8/.github/workflows/build-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.github/workflows/ci.yml` & `bowtie_json_schema-2023.7.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.7.8/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.github/workflows/deploy-frontend.yml` & `bowtie_json_schema-2023.7.8/.github/workflows/deploy-frontend.yml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         with:
           workflow: report.yml
           branch: main
           name: report
           path: _site
 
       - name: Upload artifact
-        uses: actions/upload-pages-artifact@v1
+        uses: actions/upload-pages-artifact@v2
 
   deploy:
     permissions:
       pages: write
       id-token: write
     environment:
       name: github-pages
```

### Comparing `bowtie_json_schema-2023.7.7/.github/workflows/images.yml` & `bowtie_json_schema-2023.7.8/.github/workflows/images.yml`

 * *Files 0% similar despite different names*

```diff
@@ -83,13 +83,13 @@
           tags: ${{ steps.build_image.outputs.tags }}
           registry: ghcr.io/${{ github.repository_owner }}
           username: ${{ github.actor }}
           password: ${{ github.token }}
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
 
       - name: Install Bowtie
-        uses: bowtie-json-schema/bowtie@v2023.07.2
+        uses: bowtie-json-schema/bowtie@v2023.07.7
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
 
       - name: Smoke Test
         run: bowtie smoke -i "${{ steps.build_image.outputs.image-with-tag }}"
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
```

### Comparing `bowtie_json_schema-2023.7.7/.github/workflows/report.yml` & `bowtie_json_schema-2023.7.8/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/bowtie/_cli.py` & `bowtie_json_schema-2023.7.8/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/bowtie/_commands.py` & `bowtie_json_schema-2023.7.8/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/bowtie/_core.py` & `bowtie_json_schema-2023.7.8/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/bowtie/_report.py` & `bowtie_json_schema-2023.7.8/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/bowtie/exceptions.py` & `bowtie_json_schema-2023.7.8/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/Makefile` & `bowtie_json_schema-2023.7.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/cli.rst` & `bowtie_json_schema-2023.7.8/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/conf.py` & `bowtie_json_schema-2023.7.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/contributing.rst` & `bowtie_json_schema-2023.7.8/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/implementers.rst` & `bowtie_json_schema-2023.7.8/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/index.rst` & `bowtie_json_schema-2023.7.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/requirements.txt` & `bowtie_json_schema-2023.7.8/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/docs/_static/dreamed.png` & `bowtie_json_schema-2023.7.8/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/package-lock.json` & `bowtie_json_schema-2023.7.8/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/package.json` & `bowtie_json_schema-2023.7.8/frontend/package.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2023.7.8/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/public/favicon.ico` & `bowtie_json_schema-2023.7.8/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/ReportDataHandler.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/ReportDataHandler.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/index.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/index.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/CopyToClipboard.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/CopyToClipboard.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/LoadingAnimation.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/LoadingAnimation.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/NavBar.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/NavBar.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Cases/AccordionItem.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionItem.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Cases/AccordionSvg.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionSvg.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Cases/CasesSection.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/CasesSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Cases/SchemaDisplay.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/SchemaDisplay.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/DragAndDrop/DragAndDrop.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/DragAndDrop/DragAndDrop.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Modals/DetailsButtonModal.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Modals/DetailsButtonModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Modals/RunTimeInfoModal.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Modals/RunTimeInfoModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/RunInfo/RunInfoSection.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/RunInfo/RunInfoSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Summary/ImplementationRow.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Summary/SummarySection.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummarySection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/components/Summary/SummaryTable.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummaryTable.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/context/ThemeContext.jsx` & `bowtie_json_schema-2023.7.8/frontend/src/context/ThemeContext.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2023.7.8/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/tests/test_integration.py` & `bowtie_json_schema-2023.7.8/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.7.8/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.7.8/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.7.8/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.7.8/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/.gitignore` & `bowtie_json_schema-2023.7.8/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/LICENSE` & `bowtie_json_schema-2023.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/README.rst` & `bowtie_json_schema-2023.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/pyproject.toml` & `bowtie_json_schema-2023.7.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.7/PKG-INFO` & `bowtie_json_schema-2023.7.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.7.7
+Version: 2023.7.8
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

