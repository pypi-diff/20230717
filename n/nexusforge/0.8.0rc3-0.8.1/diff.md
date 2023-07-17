# Comparing `tmp/nexusforge-0.8.0rc3.tar.gz` & `tmp/nexusforge-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nexusforge-0.8.0rc3.tar", last modified: Thu Dec 15 15:28:10 2022, max compression
+gzip compressed data, was "nexusforge-0.8.1.tar", last modified: Mon Jul 17 16:09:14 2023, max compression
```

## Comparing `nexusforge-0.8.0rc3.tar` & `nexusforge-0.8.1.tar`

### file list

```diff
@@ -1,300 +1,301 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/.gitreview
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      365 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/Contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/binder/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/binder/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/archetypes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      409 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/docs/source/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   158851 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/assets/bbnforge
--rw-r--r--   0 runner    (1001) docker     (123)   187793 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/assets/nexus-forge-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    31220 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/interaction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/docs/source/releases/
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.3-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.3.3-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.4.0-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.5.0-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      748 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.5.1-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.5.2-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.6.0-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.6.1-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.6.2-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.6.3-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releases/v0.7.0-release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/releasesfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/specializations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/docs/source/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/configurations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/configurations/demo-resolver/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/demo-resolver/entity-to-resource-mapping.hjson
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/demo-resolver/term-to-resource-mapping.hjson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/configurations/demo-store/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/demo-store/demo-config-with-resolvers.yml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/demo-store/file-to-resource-mapping.hjson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/configurations/entitylinking-resolver/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/entitylinking-resolver/entitylinking-mapper-encoder.hjson
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/entitylinking-resolver/entitylinking-mapper-es.hjson
--rw-r--r--   0 runner    (1001) docker     (123)      297 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/entitylinking-resolver/entitylinking-mapper.hjson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/configurations/nexus-resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/nexus-resolver/agent-to-resource-mapping.hjson
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/nexus-resolver/term-to-resource-mapping.hjson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/configurations/nexus-store/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/nexus-store/file-to-resource-mapping.hjson
--rw-r--r--   0 runner    (1001) docker     (123)      282 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/configurations/nexus-store/publishing-file-to-resource-mapping.hjson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/associations.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/my_data.xwz
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/my_data_derived.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/persons-with-id.csv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/persons.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/data/scientists-database/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/scientists-database/albert_einstein.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/scientists-database/marie_curie.txt
--rw-r--r--   0 runner    (1001) docker     (123)   204848 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/data/tfidfvectorizer_model_schemaorg_linking
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/mappings/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/models/
--rw-r--r--   0 runner    (1001) docker     (123)    35789 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/models/neuroshapes_context.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)    18111 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/00 - Initialization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/01 - Resources.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    28764 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/02 - Datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/03 - Storing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   114758 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/04 - Querying.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/05 - Versioning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/06 - JSON IO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31087 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/07 - DataFrame IO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/08 - Formatting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   108947 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/09 - Resolving-test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26195 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/09 - Resolving.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/10 - Reshaping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15770 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/11 - Modeling.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/12 - Mapping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/13 - JSON-LD IO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/14 - RDF IO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/15 - SQL IO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/16 - Debugging.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/getting-started/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/
--rw-r--r--   0 runner    (1001) docker     (123)    63827 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Create Datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    65632 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Ontology Brain Building Workflow Search and Exploration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    55291 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Ontology types Search and Exploration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24563 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Search and Download.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP-KG-Search-and-Download-Data-at-a-given-tag.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/EntityLinkerElastic-forge-demo-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/EntityLinkerSkLearn-forge-demo-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25841 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/MOOC_Content_based_Recommender_System_using_Blue_Brain_Nexus.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/ResolvingStrategies.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/bbp-staging-forge.yml
--rw-r--r--   0 runner    (1001) docker     (123)    52783 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/copy-token.png
--rw-r--r--   0 runner    (1001) docker     (123)    23191 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/dataset_from_different_sources.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      929 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/forge.yml
--rw-r--r--   0 runner    (1001) docker     (123)    52041 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/login-ui.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/mappings/allen_ephys_dataset.hjson
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/mappings/allen_morphology_dataset.hjson
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/mappings/mouselight_dataset.hjson
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/one_cell_minds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/prod-forge-nexus.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/rdfmodel/
--rw-r--r--   0 runner    (1001) docker     (123)    32325 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/examples/notebooks/use-cases/rdfmodel/jsonldcontext.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgentitylinkingsklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgentitylinkingsklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgentitylinkingsklearn/entity_linking_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgentitylinkingsklearn/entity_linking_sklearn_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/core/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/core/archetypes/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/archetypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/archetypes/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/archetypes/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/archetypes/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/archetypes/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/archetypes/store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/core/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/es_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/commons/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/core/conversions/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/conversions/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/conversions/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/conversions/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    35400 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/forge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/reshaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/core/wrappings/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/wrappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/wrappings/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/core/wrappings/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappers/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappers/r2rml.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappers/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappers/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/mappings/dictionaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/demo_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19162 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/directory_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/store_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/models/rdf_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/agent_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/demo_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/entity_linker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/entity_linker_elastic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/service/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/service/entity_linking_elastic_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/service/entity_linking_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/ontology_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resolvers/store_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resources/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/resources/entity_linking_candidate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42715 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/bluebrain_nexus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/demo_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/nexus/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/nexus/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/kgforge/specializations/stores/rdflib_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/kgforge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/nexusforge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/nexusforge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/nexusforge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/nexusforge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/nexusforge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/nexusforge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/KGForge Setup.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/core/archetypes/
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/archetypes/test_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/core/commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/commons/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/commons/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/commons/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/commons/test_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    28673 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/commons/test_es_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/commons/test_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/core/conversions/
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/conversions/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/conversions/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/conversions/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/conversions/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/resource.feature
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/test_forge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/test_reshaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/test_resolving.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/core/wrappings/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/wrappings/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/core/wrappings/test_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/demo-model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/allen-cell-types-database/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/NeuronMorphology.hjson
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/PatchedCell.hjson
--rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/Subject.hjson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/scientists-database/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/scientists-database/DictionaryMapping/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/scientists-database/DictionaryMapping/Association.hjson
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/mappings/scientists-database/DictionaryMapping/Contribution.hjson
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/namespaces.json
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/schemas.json
--rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-model/vocabulary.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/demo-resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-resolver/agents.json
--rw-r--r--   0 runner    (1001) docker     (123)      621 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-resolver/cell_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-resolver/sex.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-resolver/species.json
--rw-r--r--   0 runner    (1001) docker     (123)      548 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/demo-resolver/structure_layer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/shacl-model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/data/shacl-model/commons/
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/shacl-model/commons/shapes-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/shacl-model/commons/shapes-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/shacl-model/commons/shapes-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/data/shacl-model/context.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/specializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/specializations/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/mappers/test_mappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/specializations/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/mappings/test_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/specializations/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/models/demo_model.feature
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/models/test_demo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/models/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/models/test_rdf_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/specializations/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/resolvers/test_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/specializations/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/resources/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/resources/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:28:10.000000 nexusforge-0.8.0rc3/tests/specializations/stores/
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/stores/demo_store.feature
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/stores/test_bluebrain_nexus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/stores/test_demo_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tests/specializations/stores/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-15 15:27:56.000000 nexusforge-0.8.0rc3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.019566 nexusforge-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-17 16:09:09.000000 nexusforge-0.8.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-17 16:09:09.000000 nexusforge-0.8.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 16:09:09.000000 nexusforge-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 16:09:09.000000 nexusforge-0.8.1/.gitreview
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-17 16:09:09.000000 nexusforge-0.8.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-17 16:09:09.000000 nexusforge-0.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-17 16:09:09.000000 nexusforge-0.8.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-17 16:09:09.000000 nexusforge-0.8.1/Contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-17 16:09:09.000000 nexusforge-0.8.1/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-17 16:09:09.000000 nexusforge-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-17 16:09:14.051566 nexusforge-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-17 16:09:09.000000 nexusforge-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 16:09:09.000000 nexusforge-0.8.1/binder/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.027566 nexusforge-0.8.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/archetypes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.027566 nexusforge-0.8.1/docs/source/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   158851 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/assets/bbnforge
+-rw-r--r--   0 runner    (1001) docker     (123)   187793 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/assets/nexus-forge-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34209 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/interaction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.027566 nexusforge-0.8.1/docs/source/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.3-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.3.3-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.4.0-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.5.0-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.5.1-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.5.2-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.6.0-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.6.1-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.6.2-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.6.3-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releases/v0.7.0-release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/releasesfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/specializations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-17 16:09:09.000000 nexusforge-0.8.1/docs/source/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.019566 nexusforge-0.8.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.019566 nexusforge-0.8.1/examples/configurations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.027566 nexusforge-0.8.1/examples/configurations/demo-resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/demo-resolver/entity-to-resource-mapping.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/demo-resolver/term-to-resource-mapping.hjson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.027566 nexusforge-0.8.1/examples/configurations/demo-store/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/demo-store/demo-config-with-resolvers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/demo-store/file-to-resource-mapping.hjson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.027566 nexusforge-0.8.1/examples/configurations/entitylinking-resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/entitylinking-resolver/entitylinking-mapper-encoder.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/entitylinking-resolver/entitylinking-mapper-es.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/entitylinking-resolver/entitylinking-mapper.hjson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.031566 nexusforge-0.8.1/examples/configurations/nexus-resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/nexus-resolver/agent-to-resource-mapping.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/nexus-resolver/term-to-resource-mapping.hjson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.031566 nexusforge-0.8.1/examples/configurations/nexus-store/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/nexus-store/file-to-resource-mapping.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/configurations/nexus-store/publishing-file-to-resource-mapping.hjson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.031566 nexusforge-0.8.1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/associations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/my_data.xwz
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/my_data_derived.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/persons-with-id.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/persons.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.031566 nexusforge-0.8.1/examples/data/scientists-database/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/scientists-database/albert_einstein.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/scientists-database/marie_curie.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   204848 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/data/tfidfvectorizer_model_schemaorg_linking
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.031566 nexusforge-0.8.1/examples/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/mappings/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.031566 nexusforge-0.8.1/examples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    35789 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/models/neuroshapes_context.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.019566 nexusforge-0.8.1/examples/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.035566 nexusforge-0.8.1/examples/notebooks/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/00 - Initialization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/01 - Resources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/02 - Datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/03 - Storing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   136033 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/04 - Querying.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/05 - Versioning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/06 - JSON IO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31087 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/07 - DataFrame IO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/08 - Formatting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26195 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/09 - Resolving.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/10 - Reshaping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/11 - Modeling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/12 - Mapping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/13 - JSON-LD IO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/14 - RDF IO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/15 - SQL IO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/16 - Debugging.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/getting-started/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.035566 nexusforge-0.8.1/examples/notebooks/use-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)    63827 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Create Datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    65632 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Ontology Brain Building Workflow Search and Exploration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Ontology types Search and Exploration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24563 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Search and Download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/BBP-KG-Search-and-Download-Data-at-a-given-tag.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/EntityLinkerElastic-forge-demo-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/EntityLinkerSkLearn-forge-demo-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25841 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/MOOC_Content_based_Recommender_System_using_Blue_Brain_Nexus.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/ResolvingStrategies.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/bbp-staging-forge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    52783 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/copy-token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/dataset_from_different_sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/forge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    52041 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/login-ui.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.035566 nexusforge-0.8.1/examples/notebooks/use-cases/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/mappings/allen_ephys_dataset.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/mappings/allen_morphology_dataset.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/mappings/mouselight_dataset.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/one_cell_minds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/prod-forge-nexus.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.035566 nexusforge-0.8.1/examples/notebooks/use-cases/rdfmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)    32325 2023-07-17 16:09:09.000000 nexusforge-0.8.1/examples/notebooks/use-cases/rdfmodel/jsonldcontext.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.035566 nexusforge-0.8.1/kgentitylinkingsklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgentitylinkingsklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgentitylinkingsklearn/entity_linking_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgentitylinkingsklearn/entity_linking_sklearn_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.035566 nexusforge-0.8.1/kgforge/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.039566 nexusforge-0.8.1/kgforge/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.039566 nexusforge-0.8.1/kgforge/core/archetypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/archetypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/archetypes/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/archetypes/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/archetypes/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/archetypes/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/archetypes/store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.039566 nexusforge-0.8.1/kgforge/core/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/es_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/sparql_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/commons/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.039566 nexusforge-0.8.1/kgforge/core/conversions/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/conversions/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/conversions/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/conversions/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38798 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/forge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/reshaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.039566 nexusforge-0.8.1/kgforge/core/wrappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/wrappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/wrappings/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/core/wrappings/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.039566 nexusforge-0.8.1/kgforge/specializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.039566 nexusforge-0.8.1/kgforge/specializations/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/mappers/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/mappers/r2rml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/mappers/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/mappers/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/mappings/dictionaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/demo_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/models/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19162 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf/directory_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf/store_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/models/rdf_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/agent_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/demo_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/entity_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/entity_linker_elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/service/entity_linking_elastic_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/service/entity_linking_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/ontology_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resolvers/store_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resources/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/resources/entity_linking_candidate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44034 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/stores/bluebrain_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/stores/demo_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/kgforge/specializations/stores/nexus/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/stores/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22422 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/stores/nexus/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 16:09:09.000000 nexusforge-0.8.1/kgforge/specializations/stores/rdflib_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 16:09:13.000000 nexusforge-0.8.1/kgforge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/nexusforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-17 16:09:13.000000 nexusforge-0.8.1/nexusforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-17 16:09:13.000000 nexusforge-0.8.1/nexusforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:09:13.000000 nexusforge-0.8.1/nexusforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-17 16:09:13.000000 nexusforge-0.8.1/nexusforge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 16:09:13.000000 nexusforge-0.8.1/nexusforge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:09:14.051566 nexusforge-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-17 16:09:09.000000 nexusforge-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.043566 nexusforge-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/KGForge Setup.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21574 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/core/archetypes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/archetypes/test_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/core/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/commons/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/commons/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/commons/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/commons/test_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29684 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/commons/test_es_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/commons/test_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/core/conversions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/conversions/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/conversions/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/conversions/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/conversions/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/resource.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/test_forge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/test_reshaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/test_resolving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/core/wrappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/wrappings/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/core/wrappings/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/data/demo-model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/tests/data/demo-model/mappings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/tests/data/demo-model/mappings/allen-cell-types-database/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/NeuronMorphology.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/PatchedCell.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/Subject.hjson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/tests/data/demo-model/mappings/scientists-database/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.047566 nexusforge-0.8.1/tests/data/demo-model/mappings/scientists-database/DictionaryMapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/mappings/scientists-database/DictionaryMapping/Association.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/mappings/scientists-database/DictionaryMapping/Contribution.hjson
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/namespaces.json
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/schemas.json
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-model/vocabulary.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/data/demo-resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-resolver/agents.json
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-resolver/cell_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-resolver/sex.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-resolver/species.json
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/demo-resolver/structure_layer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/data/shacl-model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/data/shacl-model/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/shacl-model/commons/shapes-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/shacl-model/commons/shapes-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/shacl-model/commons/shapes-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/data/shacl-model/context.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.023566 nexusforge-0.8.1/tests/specializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/specializations/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/mappers/test_mappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/specializations/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/mappings/test_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/specializations/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/models/demo_model.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/models/test_demo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/models/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/models/test_rdf_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/specializations/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/resolvers/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/specializations/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/resources/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/resources/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:09:14.051566 nexusforge-0.8.1/tests/specializations/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/stores/demo_store.feature
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/stores/test_bluebrain_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/stores/test_demo_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tests/specializations/stores/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-17 16:09:09.000000 nexusforge-0.8.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nexusforge-0.8.0rc3/.github/workflows/publish.yml` & `nexusforge-0.8.1/.github/workflows/publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Publish sdist tarball to PyPi
 
 on:
   push:
     tags:
-      - 'v[0-9]+.[0-9]+.[0-9]+-rc.[0-9]+'
+      - 'v[0-9]+.[0-9]+.[0-9]+'
 
 jobs:
   build-n-publish:
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@master
-      - name: Set up Python 3.7
+      - name: Set up Python 3.8
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: 3.8
       - name: Build a source tarball
         run: python setup.py sdist
       - name: Publish distribution package to PyPI
         uses: pypa/gh-action-pypi-publish@master
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `nexusforge-0.8.0rc3/.pylintrc` & `nexusforge-0.8.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/Contributing.rst` & `nexusforge-0.8.1/Contributing.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/LICENSE-3RD-PARTY.txt` & `nexusforge-0.8.1/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/LICENSE.txt` & `nexusforge-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/PKG-INFO` & `nexusforge-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusforge
-Version: 0.8.0rc3
+Version: 0.8.1
 Summary: Building and Using Knowledge Graphs made easy.
 Home-page: https://github.com/BlueBrain/nexus-forge
 Author: Blue Brain Project, EPFL
 License: UNKNOWN
 Description: Blue Brain Nexus Forge
         ======================
         
@@ -97,12 +97,12 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: linking_sklearn
```

### Comparing `nexusforge-0.8.0rc3/README.rst` & `nexusforge-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/Makefile` & `nexusforge-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/archetypes.rst` & `nexusforge-0.8.1/docs/source/archetypes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/assets/bbnforge` & `nexusforge-0.8.1/docs/source/assets/bbnforge`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/assets/nexus-forge-architecture.png` & `nexusforge-0.8.1/docs/source/assets/nexus-forge-architecture.png`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/conf.py` & `nexusforge-0.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/configuration.rst` & `nexusforge-0.8.1/docs/source/configuration.rst`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,20 @@
      <scope>:
        - resolver: <a class name of a Resolver>
          origin: <'directory', 'web_service', or 'store'>
          source: <a directory path, a web service endpoint, or the class name of a Store>
          targets:
            - identifier: <a name, or an IRI>
              bucket: <a file name, an URL path, or a Store bucket>
+             filters:
+               - path: <a resource property path>
+               - value: <a resource property value to filter with>
+         searchendpoints:
+           sparql:
+             endpoint: <A SPARQL endpoint to send resolving query to. Only used for resolvers based on SPARQL>
          resolve_with_properties: <a list of str currently only supported by DemoResolver>
          result_resource_mapping: <an Hjson string, a file path, or an URL>
          endpoint: <when 'origin' is 'store', a Store endpoint, default to Store:endpoint>
          token: <when 'origin' is 'store', a Store token, default to Store:token>
    Formatters:
      <identifier>: <a string template with replacement fields delimited by braces, i.e. '{}'>
 
@@ -93,17 +99,28 @@
                    "resolver": <str>,
                    "origin": <str>,
                    "source": <str>,
                    "targets": [
                        {
                            "identifier": <str>,
                            "bucket": <str>,
+                           "filter":[
+                                {
+                                    "path": <str>,
+                                    "value": <str>
+                                }
+                            ]
                        },
                        ...,
                    ],
+                   "searchendpoints":{
+                        "sparql":{
+                            "endpoint": <str>
+                        }
+                    },
                    "resolve_with_properties":[str],
                    "result_resource_mapping": <str>,
                    "endpoint": <str>,
                    "token": <str>,
                },
                ...,
            ],
```

### Comparing `nexusforge-0.8.0rc3/docs/source/interaction.rst` & `nexusforge-0.8.1/docs/source/interaction.rst`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
           name: BlueBrainNexus,
           "endpoint":"https://bluebrainnexus_deployment_address"
           bucket: <org/project> # A Blue Brain Nexus organisation and project can be provided as bucket
 
     """
    forge = KnowledgeGraphForge(configuration=config)
 
-See the `configuration documentation page section <https://nexus-forge.readthedocs.io/en/latest/configuration.html>`__ for a full list of forge configuration and see the `examples/notebooks/use-cases/ <https://github.com/BlueBrain/nexus-forge/tree/master/examples/notebooks/use-cases>`__ folder
+See the `configuration documentation page section <https://nexus-forge.readthedocs.io/en/v0.8.1/configuration.html>`__ for a full list of forge configuration and see the `examples/notebooks/use-cases/ <https://github.com/BlueBrain/nexus-forge/tree/master/examples/notebooks/use-cases>`__ folder
 for more real world YAML examples.
 
 |Binder_Init| for more details about how to create forge configurations files.
 
 Resource
 --------
 
@@ -317,19 +317,32 @@
 * Convert a `Resource` to RDF Graph and vice-versa: |Binder_RDF|
 
 Formatting
 ----------
 
 |Binder_Formatting| to explore more about forge formatting capabilities.
 
-A preconfigured set of string formats can be provided to ensure the consistency of data.
+.. code-block:: python
+   
+   forge.format(what: str = None, *args, formatter: Union[Formatter, str] = Formatter.STR, uri: str = None, **kwargs) -> str
+
+Two type of formatters are supported:
+
+* Formatter.STR: Default formatter. A preconfigured set of string formatters implemented as `str.format(*args, **kwargs)`. See the Formatter section of the `configuration documentation page section <https://nexus-forge.readthedocs.io/en/v0.8.1/configuration.html>`__ .
 
 .. code-block:: python
+   
+   forge.format(what="formatter_configured_name", "str1", "str2") -> str
+
+* Formatter.URI_REWRITER: URI rewriter delegated to the configured Store. For example, the BlueBrainNexus store can fully expand a provided URI using its json-ld context.
+
+.. code-block:: python
+   
+   forge.format(uri="http://uri", formatter = Formatter.URI_REWRITER, **kwargs) -> str
 
-   forge.format(what: str, *args) -> str
 
 Next is an example of formatting a resource identifier with a namespace. This make all resources identifiers
 fall under the same namespace.
 
 .. code-block:: python
 
    from kgforge.core import KnowledgeGraphForge
@@ -422,26 +435,59 @@
                     - resolver: EntityLinkerSkLearn from kgentitylinkingsklearn
                       origin: directory
                       source: "../../data/"
                       targets:
                         - identifier: terms
                           bucket: tfidfvectorizer_model_schemaorg_linking
                       result_resource_mapping: ../../configurations/entitylinking-resolver/entitylinking-mapper.hjson
+                  schemaorg_CreativeWork:
+                    - resolver: OntologyResolver
+                      origin: directory
+                      source: "../../data/"
+                      targets:
+                        - identifier: CreativeWork
+                          bucket: schemaorg_ontology_file_path
+                          filters:
+                            - path: subClassOf*.id
+                              value: CreativeWork
+                      result_resource_mapping: ../../configurations/nexus-resolver/term-to-resource-mapping.hjson
 
             """
    forge = KnowledgeGraphForge(configuration= config)
    forge.resolve(text="person", scope="schemaorg", target="terms", strategy=ResolvingStrategy.BEST_MATCH)
+   forge.resolve(text="Chapter", scope="schemaorg_CreativeWork", target="CreativeWork", strategy=ResolvingStrategy.EXACT_MATCH)
 
 A `scope` is a convenient way to name (any name can be provided) a given `Resolver` along with a set of sources of data
 (the `targets`) to resolve against.
 
+Here is the complete configuration of a Resolver:
+
+.. code-block:: python
+
+   Resolvers:
+     <scope>:
+       - resolver: <a class name of a Resolver>
+         origin: <'directory', 'web_service', or 'store'>
+         source: <a directory path, a web service endpoint, or the class name of a Store>
+         targets:
+           - identifier: <a name, or an IRI>
+             bucket: <a file name, an URL path, or a Store bucket>
+             filters:
+               - path: <a resource property path>
+               - value: <a resource property value to filter with>
+         resolve_with_properties: <a list of str currently only supported by DemoResolver>
+         result_resource_mapping: <an Hjson string, a file path, or an URL>
+         endpoint: <when 'origin' is 'store', a Store endpoint, default to Store:endpoint>
+         token: <when 'origin' is 'store', a Store token, default to the token provided in the configured Store>
+
 Nexus Forge comes with the support of 5 types Resolvers:
 
-* **OntologyResolver**: based on type, label and notation (ie. acronym) filtering using a SPARQL query to generate candidates.
-  An example of configuration is available at `examples/notebooks/use-cases/prod-forge-nexus.yml`.
+* **OntologyResolver**: based on type (rdf:type), label (rdfs:label), prefLabel (skos:prefLabel), altLabel (skos:altLabel) and notation (skos:notation) properties to filter with using a SPARQL query to generate candidates. 
+  Extra property path based filters can be provided as part of the resolver configuration to further narrow the results.
+  An example of ontology resolving configuration is available at `examples/notebooks/use-cases/prod-forge-nexus.yml <https://github.com/BlueBrain/nexus-forge/blob/master/examples/notebooks/use-cases/prod-forge-nexus.yml>`__ .
 
 * **EntityLinkerSkLearn**: based on a pretrained model and using `scikit-learn <https://scikit-learn.org/stable/>`__.
   to generate and rank candidates. To customise the configuration of this resolver
   (as shown in the resolving example above):
 
   * Nexus Forge should be installed as follows `pip install nexusforge[linking_sklearn]`
 
@@ -458,16 +504,17 @@
   An example of configuration for `EntityLinkerSkLearn` is available at
   `examples/notebooks/use-cases/EntityLinkerSkLearn-forge-demo-config.yml`.
 
 * **EntityLinkerElastic**: based on `ElasticSearch text similarity search <https://www.elastic.co/blog/text-similarity-search-with-vectors-in-elasticsearch>`__
   to generate and rank candidates but require a text embedding or encoding service to compute embeddings of items.
   An example of configuration is available at `examples/notebooks/use-cases/EntityLinkerElastic-forge-demo-config.yml`. .
 
-* **AgentResolver**: based on type, full, given or family names filtering using a SPARQL query to generate candidates.
-  An example of configuration is available at `examples/notebooks/use-cases/prod-forge-nexus.yml`.
+* **AgentResolver**: based on type (rdf:type), name (schema:name), givenName (schema:givenName) or familyName (schema:familyName) properties to filter with using a SPARQL query to generate candidates.
+  Extra property path based filters can be provided as part of the resolver configuration to further narrow the results.
+  An example of configuration is available at `examples/notebooks/use-cases/prod-forge-nexus.yml <https://github.com/BlueBrain/nexus-forge/blob/master/examples/notebooks/use-cases/prod-forge-nexus.yml>`__ .
 
 * **DemoResolver**: an example resolver based on filtering by configurable properties and looking up candidates from a json file.
   An example of configuration is available at `examples/notebooks/use-cases/EntityLinkerSkLearn-forge-demo-config.yml`.
 
 Reshaping
 ---------
```

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.4.0-release-notes.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,122 @@
-=============
-Release Notes
-=============
+====================
+vO.4.0 Release Notes
+====================
 
-This release adds new features and enhancements to Nexus Forge as well as bug fixes.
+This release adds incremental features to both Nexus Forge core and specializations modules. This release also implemented many fixes to various issues raised by users.
 
 New Features
 ============
 
-Resolving
----------
+Querying
+--------
 
-* Added ontology resource resolving based on skos:prefLabel and skos:altLabel in addition to label and skos:notation. `#245 <https://github.com/BlueBrain/nexus-forge/pull/245>`__ (|Binder_Resolving| to try it)
+* Add cross-bucket search feature `#71 <https://github.com/BlueBrain/nexus-forge/pull/71>`__ `#74 <https://github.com/BlueBrain/nexus-forge/pull/74>`__ (issue:`#63 <https://github.com/BlueBrain/nexus-forge/pull/63>`__)(usage: 04 - Querying notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/04%20-%20Querying.ipynb>`__ or on |Binder|)
 
-Modeling
---------
+If cross_bucket is set to True, resources could be retrieved by identifier from multiple buckets. In such case, a specific bucket can be target using the `bucket` argument.
 
-* Add support for validation against a schema. `#217 <https://github.com/BlueBrain/nexus-forge/pull/217>`__ (|Binder_Modeling| to try it)
+Usage:
 
 .. code-block:: python
 
-    from kgforge.core import KnowledgeGraphForge
-    # see https://github.com/BlueBrain/nexus-forge/blob/master/examples/notebooks/use-cases/prod-forge-nexus.yml for a full forge config example.
-    forge = KnowledgeGraphForge(configuration="./config.yml", **kwargs)
-    person = Resource(type="Person", name="Jane Doe")
-    # By default the schema associated with the resource type is picked for validation. A different type can be set using the type_ argument.
-    forge.validate(person, type_="Agent")
+   resource = forge.search(<resource_id>, cross_bucket=True, bucket=<str>)
 
+.. note::
+
+   The configured store should support cross bucket search.
+
+* Add support for targeting specific search endpoint when searching data. Currently only SPARQL endpoints are supported `#71 <https://github.com/BlueBrain/nexus-forge/pull/71>`__ (issue:`#63 <https://github.com/BlueBrain/nexus-forge/pull/63>`__)(usage: 04 - Querying notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/04%20-%20Querying.ipynb>`__ or on |Binder|)
+
+A `searchendpoints` configuration can be added to the `Store` configuration.
+
+.. code-block:: python
+
+   "Store": {
+           "name": <str>,
+           "endpoint": <str>,
+           "bucket": <str>,
+           "token": <str>,
+           "searchendpoints": {
+                "<querytype>": { # <a query paradigm supported by the store (e.g. sparql)>
+                "endpoint": <str> #<an IRI of a query endpoint>
+            }
+           },
+           "versioned_id_template": <str>,
+           "file_resource_mapping": <str>
+   }
 
 Enhancements
 ============
 
+Forge
+-----
+
+* Add creating a forge session from a configuration URL `#91 <https://github.com/BlueBrain/nexus-forge/pull/91>`__ (issue:`#65 <https://github.com/BlueBrain/nexus-forge/pull/65>`__)
+
+.. code-block:: python
+
+   forge = KnowledgeGraphForge(configuration="https://...config.json") # or config.yml
+
 Querying
 --------
 
-|Binder_Querying| to try the querying enhancements.
+* Add query param support when retrieving a resource `#79 <https://github.com/BlueBrain/nexus-forge/pull/79>`__
+
+.. code-block:: python
+
+   resource = forge.retrieve(id="https://..?rev=1&p=aparam")
 
-* Added support for searching using filters (except when Paths syntax is used) from _store_metadata properties (i.e _createdAt, _updatedAt,...) `#224 <https://github.com/BlueBrain/nexus-forge/pull/224>`__ `#240 <https://github.com/BlueBrain/nexus-forge/pull/240>`__ (issue `#209 <https://github.com/BlueBrain/nexus-forge/pull/209>`__)
-* Added support for searching using datetime filters which can be specify as string suffixed with `^^xsd:dateTime` `#224 <https://github.com/BlueBrain/nexus-forge/pull/224>`__
+Specifically, when the version argument is provided like in:
 
 .. code-block:: python
 
-    from kgforge.core import KnowledgeGraphForge
-    # see https://github.com/BlueBrain/nexus-forge/blob/master/examples/notebooks/use-cases/prod-forge-nexus.yml for a full forge config example.
-    forge = KnowledgeGraphForge(configuration="./config.yml", **kwargs)
-    filters = {
-           "type": "Dataset",
-           "_createdAt":'"2022-04-12T21:29:14.410Z"^^xsd:dateTime'
-          }
-    forge.search(filters)
-
-
-* Added support for disabling SPARQL rewriting when a correct SPARQL is provided `#224 <https://github.com/BlueBrain/nexus-forge/pull/224>`__ (issue `#218 <https://github.com/BlueBrain/nexus-forge/pull/218>`__)
-* Inline query limit/offset arguments are now superseded by limit/offset provided as argument for `forge.search()` `#224 <https://github.com/BlueBrain/nexus-forge/pull/224>`__ (issue `#189 <https://github.com/BlueBrain/nexus-forge/pull/189>`__)
-* Added support for `IN` SPARQL clause when rewriting SPARQL queries in `forge.search()` `#240 <https://github.com/BlueBrain/nexus-forge/pull/240>`__ (issue `#242 <https://github.com/BlueBrain/nexus-forge/pull/242>`__)
-* Using filters as argument when calling `forge.search(*filters, **params)` now raises an exception `#240 <https://github.com/BlueBrain/nexus-forge/pull/240>`__
-* When using BlueBrainNexusStore, `forge.retrieve()` and `forge.search()` now get the `original registered JSON payload <https://bluebrainnexus.io/docs/delta/api/resources-api.html#fetch-original-payload>`__ to avoid any JSON transformation `#232 <https://github.com/BlueBrain/nexus-forge/pull/232>`__
-* `forge.search()` returns resources at the exact revision they are stored in the configured searchendpoint and no longer at the latest revision. As a consequence search results are no longer `_sychronized` `#232 <https://github.com/BlueBrain/nexus-forge/pull/232>`__
-* `_last_action` property is now added to resources obtained from `forge.retrieve()` `#232 <https://github.com/BlueBrain/nexus-forge/pull/232>`__
-* Added the property distribution.atLocation.store.type and distribution.atLocation.store.type._rev to BlueBrainNexusStore file metadata mapping file `#232 <https://github.com/BlueBrain/nexus-forge/pull/232>`__
-* When using BlueBrainNexusStore, it is possible to set (in the forge config file) GET params when calling `forge.retrieve() `#232 <https://github.com/BlueBrain/nexus-forge/pull/232>`__
+   resource = forge.retrieve(id="https://..?rev=1&p=aparam, version=2")
 
-Converting
-----------
 
-|Binder_JSON-LD-IO| to try the JSON-LD enhancements.
+then it supersedes the `rev` query param while the other query params (e.g `p=aparam`) are kept as they are.
 
-* `forge.as_jsonld(r, form="expanded")` now outputs expanded JSON-LD with @value added for literals. `#244 <https://github.com/BlueBrain/nexus-forge/pull/244>`__
-* `forge.as_jsonld(r, form="compacted")` keeps unchanged JSON null values and arrays. The param `array_as_set` is no longer needed and is thus removed along with the `na` argument `#244 <https://github.com/BlueBrain/nexus-forge/pull/244>`__
 
+Dataset
+-------
 
-Resolving
----------
+* Dataset provenance assertion methods are now all aligned to accept either a `Resource` object of identifier. `#88 <https://github.com/BlueBrain/nexus-forge/pull/88>`__ (usage: 02 - Dataset notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/02%20-%20Datasets.ipynb>`__ or on |Binder|)
 
-|Binder_Resolving| to try the resolving enhancements.
+.. code-block:: python
 
-* Added `searchendpoints` config in the `forge config Resolvers section <https://github.com/BlueBrain/nexus-forge/blob/v0.7.1/examples/notebooks/use-cases/prod-forge-nexus.yml#L30>`__ `#226 <https://github.com/BlueBrain/nexus-forge/pull/226>`__
+   Dataset(forge: KnowledgeGraphForge, type: str = "Dataset", **properties)
+     add_contribution(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
+     add_generation(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
+     add_derivation(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
+     add_invalidation(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
 
+When a `Resourcce` is provided, `forge.freeze` will add the resource's version to its reference within the dataset enabling immutable identifier. `forge.freeze` is not supported when a resource identifier (str) is provided.
 
 Bug Fixes
 =========
 
-* Added an identifier and the forge model configured JSON-LD context to resources obtained from an ElasticSearch query `#238 <https://github.com/BlueBrain/nexus-forge/pull/238>`__ (issue `#230 <https://github.com/BlueBrain/nexus-forge/pull/230>`__) (|Binder_Querying| to try it)
-* Fixed failing SPARQL query rewriting when a used JSON-LD context term does not have `@id` `#231 <https://github.com/BlueBrain/nexus-forge/pull/231>`__
+Forge
+-----
+
+* Fix `has no attribute '_rev'` error when calling `forge.freeze` on a `Dataset` object. `#81 <https://github.com/BlueBrain/nexus-forge/pull/81>`__ `#88 <https://github.com/BlueBrain/nexus-forge/pull/88>`__ (issue:`#80 <https://github.com/BlueBrain/nexus-forge/pull/80>`__)
+* Fix `RuntimeError` occuring when calling `nest_asyncio.apply()` outside a Jupyter notebook session `#62 <https://github.com/BlueBrain/nexus-forge/pull/62>`__ (issue:`#60 <https://github.com/BlueBrain/nexus-forge/pull/60>`__)
+* Fix failing `forge.download` when the provided path (e.g. distribution.contentUrl) is no longer present in all distributions json objects `#85 <https://github.com/BlueBrain/nexus-forge/pull/85>`__ (issue:`#84 <https://github.com/BlueBrain/nexus-forge/pull/84>`__)(usage: 02 - Dataset notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/02%20-%20Datasets.ipynb>`__ or on |Binder|). This is to cope with `schema.org/distribution <https://schema.org/distribution>`__ specification which supports `distribution.contentUrl` or `distribution.url` when recording the location of a dataset.
+
+Resolving
+---------
+
+* Fix `OntologyResolver` to resolve ontology terms when notation and prefLabel properties are missing `#76 <https://github.com/BlueBrain/nexus-forge/pull/76>`__ (issue:`#69 <https://github.com/BlueBrain/nexus-forge/pull/69>`__)(usage: 09 - Resolving notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/09%20-%20Resolving.ipynb>`__ or on |Binder|)
+
+Querying
+--------
+
+* Fix `BlueBrainNexus` store file retrieval support `#75 <https://github.com/BlueBrain/nexus-forge/pull/75>`__ (issue:`#64 <https://github.com/BlueBrain/nexus-forge/pull/64>`__)
+
+Converting
+----------
+
+*  Fix turning a list of `Resource` elements to `RDFlib Graph` using `forge.as_graph` while avoiding graph merge resulting from using graph set operation (such as +) `#87 <https://github.com/BlueBrain/nexus-forge/pull/87>`__
 
-Changelog
-=========
 
-`Full changelog <https://github.com/BlueBrain/nexus-forge/compare/v0.7.0...v0.7.1>`__
 
-.. |Binder_Resolving| image:: https://mybinder.org/badge_logo.svg
-    :alt: Binder_Querying
-    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.1?filepath=examples%2Fnotebooks%2Fgetting-started%2F09%20-%20Resolving.ipynb
-
-.. |Binder_Modeling| image:: https://mybinder.org/badge_logo.svg
-    :alt: Binder_Modeling
-    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.1?filepath=examples%2Fnotebooks%2Fgetting-started%2F09%20-%20Modeling.ipynb
-
-.. |Binder_JSON-LD-IO| image:: https://mybinder.org/badge_logo.svg
-    :alt: Binder_JSON-LD-IO
-    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.1?filepath=examples%2Fnotebooks%2Fgetting-started%2F13%20-%20JSON-LD%20IO.ipynb
-
-.. |Binder_Querying| image:: https://mybinder.org/badge_logo.svg
-    :alt: Binder_Querying
-    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.1?filepath=examples%2Fnotebooks%2Fgetting-started%2F04%20-%20Querying.ipynb
+.. |Binder| image:: https://mybinder.org/badge_logo.svg
+    :alt: Binder
+    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.4.0?filepath=examples%2Fnotebooks%2Fgetting-started
```

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.3-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.3-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.3.3-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.3.3-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.4.0-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.7.0-release-notes.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,116 @@
 ====================
-vO.4.0 Release Notes
+vO.7.0 Release Notes
 ====================
 
-This release adds incremental features to both Nexus Forge core and specializations modules. This release also implemented many fixes to various issues raised by users.
+Welcome to two new contributors @Nabil-AL and @kplatis.
+
+This release adds new features and enhancements to Nexus Forge as well as bug fixes.
+
+New Contributors
+================
+
+The following people made their first contributions:
+
+* Alibou Nabil William (@Nabil-AL): `#196 <https://github.com/BlueBrain/nexus-forge/pull/196>`__
+* Platis Konstantinos (@kplatis): `#210 <https://github.com/BlueBrain/nexus-forge/pull/210>`__
 
 New Features
 ============
 
 Querying
 --------
 
-* Add cross-bucket search feature `#71 <https://github.com/BlueBrain/nexus-forge/pull/71>`__ `#74 <https://github.com/BlueBrain/nexus-forge/pull/74>`__ (issue:`#63 <https://github.com/BlueBrain/nexus-forge/pull/63>`__)(usage: 04 - Querying notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/04%20-%20Querying.ipynb>`__ or on |Binder|)
+* Added support for running forge search queries against ElasticSearch indices and not just SPARQL endpoints. `#192 <https://github.com/BlueBrain/nexus-forge/pull/192>`__, `#221 <https://github.com/BlueBrain/nexus-forge/pull/221>`__ (Try it using the `Querying` notebook |Binder_Querying|)
+  When calling `forge.search(...)`, a `search_endpoint` argument can be set to:
 
-If cross_bucket is set to True, resources could be retrieved by identifier from multiple buckets. In such case, a specific bucket can be target using the `bucket` argument.
+  * `elastic` to search a configured ElasticSearch search endpoint
 
-Usage:
+  * `sparql` to search a configured SPARQL endpoint (which is also the default search endpoint when no `search_endpoint` value is provided).
 
 .. code-block:: python
 
-   resource = forge.search(<resource_id>, cross_bucket=True, bucket=<str>)
-
-.. note::
-
-   The configured store should support cross bucket search.
+    from kgforge.core import KnowledgeGraphForge
+    # see https://github.com/BlueBrain/nexus-forge/blob/master/examples/notebooks/use-cases/prod-forge-nexus.yml for a full forge config example.
+    forge = KnowledgeGraphForge(configuration="./config.yml", **kwargs)
+    # Search for resources  by type using a dictionary
+    filters = {"type":"Dataset"} # any supported forge filter syntax can be provided: https://nexus-forge.readthedocs.io/en/latest/interaction.html#querying
+    results_filters = forge.search(filters, search_endpoint="elastic")
 
-* Add support for targeting specific search endpoint when searching data. Currently only SPARQL endpoints are supported `#71 <https://github.com/BlueBrain/nexus-forge/pull/71>`__ (issue:`#63 <https://github.com/BlueBrain/nexus-forge/pull/63>`__)(usage: 04 - Querying notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/04%20-%20Querying.ipynb>`__ or on |Binder|)
+ElasticSearch support in `forge.search(...)` is based on a `kgforge.core.wrappings.Filter` to ElasticSearch DSL
+rewriting strategy completely driven by either a user provided ElasticSearch mapping or by ElasticSearch dynamic field mapping.
 
-A `searchendpoints` configuration can be added to the `Store` configuration.
+When using the `BlueBrainNexus` store, the ElasticSearch endpoint (an actual ElasticSearch View) to query as well as the
+(optional) mapping to use can be configured as follows:
 
 .. code-block:: python
 
-   "Store": {
-           "name": <str>,
-           "endpoint": <str>,
-           "bucket": <str>,
-           "token": <str>,
-           "searchendpoints": {
-                "<querytype>": { # <a query paradigm supported by the store (e.g. sparql)>
-                "endpoint": <str> #<an IRI of a query endpoint>
-            }
-           },
-           "versioned_id_template": <str>,
-           "file_resource_mapping": <str>
-   }
+    Store:
+      name: BlueBrainNexus
+      endpoint: https://sandbox.bluebrainnexus.io/v1
+      searchendpoints:
+        sparql:
+          endpoint: "https://bluebrain.github.io/nexus/vocabulary/defaultSparqlIndex"
+        elastic:
+          endpoint: "https://bluebrain.github.io/nexus/vocabulary/defaultElasticSearchIndex"
+          mapping: "https://bluebrain.github.io/nexus/vocabulary/defaultElasticSearchIndex"
+          default_str_keyword_field: "keyword"
+
+For a more detailed forge configuration, see an example `available from github <https://github.com/BlueBrain/nexus-forge/blob/master/examples/notebooks/use-cases/prod-forge-nexus.yml>`__.
 
 Enhancements
 ============
 
-Forge
------
-
-* Add creating a forge session from a configuration URL `#91 <https://github.com/BlueBrain/nexus-forge/pull/91>`__ (issue:`#65 <https://github.com/BlueBrain/nexus-forge/pull/65>`__)
-
-.. code-block:: python
-
-   forge = KnowledgeGraphForge(configuration="https://...config.json") # or config.yml
-
 Querying
 --------
+* Applied user provided limit and offset arguments with higher priority than:
 
-* Add query param support when retrieving a resource `#79 <https://github.com/BlueBrain/nexus-forge/pull/79>`__
-
-.. code-block:: python
-
-   resource = forge.retrieve(id="https://..?rev=1&p=aparam")
-
-Specifically, when the version argument is provided like in:
-
-.. code-block:: python
-
-   resource = forge.retrieve(id="https://..?rev=1&p=aparam, version=2")
-
+  * `size` and `from` set in a ElasticSearch query when using `forge.elastic(...)`  `#192 <https://github.com/BlueBrain/nexus-forge/pull/192>`__ (issue `#176 <https://github.com/BlueBrain/nexus-forge/pull/176>`__) (Try it using the `Querying` notebook |Binder_Querying|)
 
-then it supersedes the `rev` query param while the other query params (e.g `p=aparam`) are kept as they are.
-
-
-Dataset
--------
-
-* Dataset provenance assertion methods are now all aligned to accept either a `Resource` object of identifier. `#88 <https://github.com/BlueBrain/nexus-forge/pull/88>`__ (usage: 02 - Dataset notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/02%20-%20Datasets.ipynb>`__ or on |Binder|)
-
-.. code-block:: python
-
-   Dataset(forge: KnowledgeGraphForge, type: str = "Dataset", **properties)
-     add_contribution(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
-     add_generation(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
-     add_derivation(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
-     add_invalidation(resource: Union[str, Resource], versioned: bool = True, **kwargs) -> None
-
-When a `Resourcce` is provided, `forge.freeze` will add the resource's version to its reference within the dataset enabling immutable identifier. `forge.freeze` is not supported when a resource identifier (str) is provided.
-
-Bug Fixes
-=========
-
-Forge
------
-
-* Fix `has no attribute '_rev'` error when calling `forge.freeze` on a `Dataset` object. `#81 <https://github.com/BlueBrain/nexus-forge/pull/81>`__ `#88 <https://github.com/BlueBrain/nexus-forge/pull/88>`__ (issue:`#80 <https://github.com/BlueBrain/nexus-forge/pull/80>`__)
-* Fix `RuntimeError` occuring when calling `nest_asyncio.apply()` outside a Jupyter notebook session `#62 <https://github.com/BlueBrain/nexus-forge/pull/62>`__ (issue:`#60 <https://github.com/BlueBrain/nexus-forge/pull/60>`__)
-* Fix failing `forge.download` when the provided path (e.g. distribution.contentUrl) is no longer present in all distributions json objects `#85 <https://github.com/BlueBrain/nexus-forge/pull/85>`__ (issue:`#84 <https://github.com/BlueBrain/nexus-forge/pull/84>`__)(usage: 02 - Dataset notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/02%20-%20Datasets.ipynb>`__ or on |Binder|). This is to cope with `schema.org/distribution <https://schema.org/distribution>`__ specification which supports `distribution.contentUrl` or `distribution.url` when recording the location of a dataset.
+* Returned a set of Resource objects as result of a forge.elastic(..) call instead of raw ES hits. ES metadata (_index, _score) are added in _store_metadata. `#192 <https://github.com/BlueBrain/nexus-forge/pull/192>`__ (issue `#177 <https://github.com/BlueBrain/nexus-forge/pull/177>`__) (Try it using the `Querying` notebook |Binder_Querying|)
 
 Resolving
 ---------
+* Added support for returning resolvers as dictionary. `#210 <https://github.com/BlueBrain/nexus-forge/pull/210>`__ (issue `#208 <https://github.com/BlueBrain/nexus-forge/pull/208>`__) (Try it using the `Resolving` notebook |Binder_Resolving|)
 
-* Fix `OntologyResolver` to resolve ontology terms when notation and prefLabel properties are missing `#76 <https://github.com/BlueBrain/nexus-forge/pull/76>`__ (issue:`#69 <https://github.com/BlueBrain/nexus-forge/pull/69>`__)(usage: 09 - Resolving notebook on `Github <https://github.com/BlueBrain/nexus-forge/blob/v0.4.0/examples/notebooks/getting-started/09%20-%20Resolving.ipynb>`__ or on |Binder|)
-
-Querying
+Tutorial
 --------
+* Added a jupyter notebook for accessing data in a BlueBrainNexus Store's view or tag. (|Binder_BBP-KG-Search-and-Download-Data-at-a-given-tag| to try it)
+* Added a jupyter notebook for ontology types search and exploration. (|Binder_BBP-KG-Ontology-types-Search-and-Exploration| to try it)
 
-* Fix `BlueBrainNexus` store file retrieval support `#75 <https://github.com/BlueBrain/nexus-forge/pull/75>`__ (issue:`#64 <https://github.com/BlueBrain/nexus-forge/pull/64>`__)
+Setup
+-----
+* Set `python>=3.7`, `rdflib>=6.0.0`, `pyshacl==v0.17.2` and `pyparsing>=2.0.2`. `#201 <https://github.com/BlueBrain/nexus-forge/pull/201>`__, `#204 <https://github.com/BlueBrain/nexus-forge/pull/204>`__, `#196 <https://github.com/BlueBrain/nexus-forge/pull/196>`__ (issue `#198 <https://github.com/BlueBrain/nexus-forge/pull/198>`__)
+  Releases of `rdflib>=6.0.0` now includes the plugin `rdflib-jsonld`, so there is no need to install it separately.
 
-Converting
-----------
+Bug Fixes
+=========
 
-*  Fix turning a list of `Resource` elements to `RDFlib Graph` using `forge.as_graph` while avoiding graph merge resulting from using graph set operation (such as +) `#87 <https://github.com/BlueBrain/nexus-forge/pull/87>`__
+* Added a fix list of JSONLD keys to JSONify (i.e. to remove the `@` prefix) to avoid removing `@` prefix for JSON-LD literal `@value`. `#200 <https://github.com/BlueBrain/nexus-forge/pull/200>`__ (issue `#194 <https://github.com/BlueBrain/nexus-forge/pull/194>`__) (Try it using the `JSON-LD IO` notebook |Binder_JSON-LD-IO|)
+* Added bucket first resolving of JSON-LD contexts (before attempting to resolve them following their HTTP URI) when using BlueBrainNexus store. This capability avoid failure when initializing a KnowledgeGraphForge session in a closed network such as Openshift pods. `#190 <https://github.com/BlueBrain/nexus-forge/pull/190>`__, `#193 <https://github.com/BlueBrain/nexus-forge/pull/193>`__ (issue `#178 <https://github.com/BlueBrain/nexus-forge/pull/178>`__)
+* Updated BlueBrainNexus store parallel batch requests to avoid tasks parameters overriding. `#191 <https://github.com/BlueBrain/nexus-forge/pull/191>`__
 
 
+Changelog
+=========
+
+`Full changelog <https://github.com/BlueBrain/nexus-forge/compare/v0.6.3...v0.7.0>`__.
 
-.. |Binder| image:: https://mybinder.org/badge_logo.svg
-    :alt: Binder
-    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.4.0?filepath=examples%2Fnotebooks%2Fgetting-started
+.. |Binder_Resolving| image:: https://mybinder.org/badge_logo.svg
+    :alt: Binder_Querying
+    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.0?filepath=examples%2Fnotebooks%2Fgetting-started%2F09%20-%20Resolving.ipynb
+
+.. |Binder_BBP-KG-Search-and-Download-Data-at-a-given-tag| image:: https://mybinder.org/badge_logo.svg
+    :alt: Binder_BBP-KG-Search-and-Download-Data-at-a-given-tag
+    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.0?filepath=examples%2Fnotebooks%2Fuse-cases%2FBBP-KG-Search-and-Download-Data-at-a-given-tag.ipynb
+
+.. |Binder_BBP-KG-Ontology-types-Search-and-Exploration| image:: https://mybinder.org/badge_logo.svg
+    :alt: Binder_BBP-KG-Search-and-Download-Data-at-a-given-tag
+    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.0?filepath=examples%2Fnotebooks%2Fuse-cases%2FBBP%20KG%20Ontology%20types%20Search%20and%20Exploration.ipynb
+
+.. |Binder_JSON-LD-IO| image:: https://mybinder.org/badge_logo.svg
+    :alt: Binder_JSON-LD-IO
+    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.0?filepath=examples%2Fnotebooks%2Fgetting-started%2F13%20-%20JSON-LD%20IO.ipynb
+
+.. |Binder_Querying| image:: https://mybinder.org/badge_logo.svg
+    :alt: Binder_Querying
+    :target: https://mybinder.org/v2/gh/BlueBrain/nexus-forge/v0.7.0?filepath=examples%2Fnotebooks%2Fgetting-started%2F04%20-%20Querying.ipynb
```

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.5.0-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.5.0-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.5.1-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.5.1-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.5.2-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.5.2-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.6.0-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.6.0-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.6.1-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.6.1-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.6.2-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.6.2-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/releases/v0.6.3-release-notes.rst` & `nexusforge-0.8.1/docs/source/releases/v0.6.3-release-notes.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/specializations.rst` & `nexusforge-0.8.1/docs/source/specializations.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/docs/source/tutorials.rst` & `nexusforge-0.8.1/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/configurations/demo-store/demo-config-with-resolvers.yml` & `nexusforge-0.8.1/examples/configurations/demo-store/demo-config-with-resolvers.yml`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/configurations/nexus-store/file-to-resource-mapping.hjson` & `nexusforge-0.8.1/examples/configurations/nexus-store/file-to-resource-mapping.hjson`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     digest:
     {
         algorithm: x._digest._algorithm
         value: x._digest._value
     }
     encodingFormat: x._mediaType
     name: x._filename
-    contentUrl: x._self
+    contentUrl: forge.format(uri=x['@id'], formatter='URI_REWRITER', is_file=True)
     atLocation:
     {
         type: Location
         store: 
         {
             id: x._storage["@id"]
             type: x._storage["@type"] if '@type' in x._storage else None
```

### Comparing `nexusforge-0.8.0rc3/examples/data/tfidfvectorizer_model_schemaorg_linking` & `nexusforge-0.8.1/examples/data/tfidfvectorizer_model_schemaorg_linking`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/models/neuroshapes_context.json` & `nexusforge-0.8.1/examples/models/neuroshapes_context.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/00 - Initialization.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/00 - Initialization.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9887844768092144%*

 * *Differences: {"'cells'": "{4: {'execution_count': 5}, 19: {'execution_count': 13}, 24: {'execution_count': 14}, "*

 * *            "25: {'execution_count': 15}, 34: {'execution_count': 28}, 37: {'execution_count': "*

 * *            "24}, 38: {'execution_count': 25, 'source': {insert: [(13, '        }\\n'), (14, '    "*

 * *            '],\\n\'), (15, \'    "ontology": [\\n\'), (16, \'        {\\n\'), (17, \'            '*

 * *            '"resolver": "OntologyResolver",\\n\'), (18, \'            "origin": "store",\\n\'), '*

 * *            '(1 […]*

```diff
@@ -32,15 +32,15 @@
                 "# Configuration\n",
                 "\n",
                 "This notebook presents a set of configuation options to set up when creating a knowledge graph forge session. Refer to the [Nexus Forge docs](https://nexus-forge.readthedocs.io/en/latest/interaction.html#forge) to learn more about all the possible configuration options."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "config = dict()"
             ]
         },
         {
@@ -210,15 +210,15 @@
             "metadata": {},
             "source": [
                 "#### Set a project name"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "endpoint = \"https://sandbox.bluebrainnexus.io/v1\"\n",
                 "org =\"github-users\"\n",
                 "project =\"mfsy\"  # Provide here the automatically created project name corresponding to your Github login when you logged in the Nexus sandbox instance."
             ]
@@ -249,24 +249,24 @@
             "metadata": {},
             "source": [
                 "##### sourced from BlueBrainNexus store"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "shacl_schema_bucket = \"neurosciencegraph/datamodels\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
                 "config['Model'] = {\n",
                 "    \"name\": \"RdfModel\",\n",
                 "    \"origin\": \"store\",\n",
                 "    \"source\": \"BlueBrainNexus\",\n",
@@ -367,15 +367,15 @@
             "metadata": {},
             "source": [
                 "### Store"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 28,
             "metadata": {},
             "outputs": [],
             "source": [
                 "config[\"Store\"] = {\n",
                 "    \"name\": \"BlueBrainNexus\",\n",
                 "    \"endpoint\": endpoint,\n",
                 "    \"searchendpoints\":{\n",
@@ -415,24 +415,24 @@
             "metadata": {},
             "source": [
                 "#### sourced from a store"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ontology_bucket = \"neurosciencegraph/datamodels\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 25,
             "metadata": {},
             "outputs": [],
             "source": [
                 "config[\"Resolvers\"] = {\n",
                 "    \"terms\": [\n",
                 "        {\n",
                 "            \"resolver\": \"OntologyResolver\",\n",
@@ -443,14 +443,28 @@
                 "                    \"identifier\": \"sexontology\",\n",
                 "                    \"bucket\": ontology_bucket\n",
                 "                }\n",
                 "            ],\n",
                 "            \"result_resource_mapping\": \"../../configurations/nexus-resolver/term-to-resource-mapping.hjson\"\n",
                 "        }\n",
                 "    ],\n",
+                "    \"ontology\": [\n",
+                "        {\n",
+                "            \"resolver\": \"OntologyResolver\",\n",
+                "            \"origin\": \"store\",\n",
+                "            \"source\": \"BlueBrainNexus\",\n",
+                "            \"targets\": [\n",
+                "                {\n",
+                "                    \"identifier\": \"cells\",\n",
+                "                    \"bucket\": ontology_bucket\n",
+                "                }\n",
+                "            ],\n",
+                "            \"result_resource_mapping\": \"../../configurations/demo-resolver/term-to-resource-mapping.hjson\"\n",
+                "        }\n",
+                "    ],\n",
                 "    \"entities\": [\n",
                 "        {\n",
                 "            \"resolver\": \"DemoResolver\",\n",
                 "            \"origin\": \"directory\",\n",
                 "            \"source\": \"../../../tests/data/demo-resolver/\",\n",
                 "            \"targets\": [\n",
                 "                {\n",
@@ -556,15 +570,15 @@
             "metadata": {},
             "source": [
                 "## Configure formatters"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "config[\"Formatters\"] = {\n",
                 "    \"identifier\": \"https://kg.example.ch/{}/{}\",\n",
                 "}"
             ]
@@ -574,49 +588,49 @@
             "metadata": {},
             "source": [
                 "## Save configuration"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import yaml"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 29,
             "metadata": {},
             "outputs": [],
             "source": [
                 "with open(\"../../configurations/forge.yml\", \"w\") as f:\n",
                 "    yaml.dump(config, f)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.7.13 ('kgforge')",
+            "display_name": "Python 3.7 (nexusforgelatest)",
             "language": "python",
-            "name": "python3"
+            "name": "nexusforgelatest"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.13"
+            "version": "3.7.10"
         },
         "vscode": {
             "interpreter": {
                 "hash": "9ac393a5ddd595f2c78ea58b15bf8d269850a4413729cbea5c5fae9013762763"
             }
         }
     },
```

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/01 - Resources.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/01 - Resources.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9773320333880678%*

 * *Differences: {"'cells'": "{13: {'execution_count': 14, 'outputs': {0: {'text': {insert: [(1, '    id: "*

 * *            "https://id\\n'), (6, '        email: jane.doe@epfl.ch\\n')]}}}, 'source': {insert: "*

 * *            '[(2, \'    "id": "https://id",\\n\')]}}, 15: {\'execution_count\': 15}, 18: '*

 * *            "{'execution_count': 16}, 20: {'execution_count': 17, 'outputs': {0: "*

 * *            "{'execution_count': 17}}}, 21: {'execution_count': 18, 'outputs': {0: "*

 * *            "{'execution_count': 18}}}, 27: {'execution_count':  […]*

```diff
@@ -166,35 +166,38 @@
             "metadata": {},
             "source": [
                 "#### JSON keys with specific values can be excluded"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "{\n",
+                        "    id: https://id\n",
                         "    type: Association\n",
                         "    agent:\n",
                         "    {\n",
                         "        type: Person\n",
+                        "        email: jane.doe@epfl.ch\n",
                         "        name: Jane Doe\n",
                         "    }\n",
                         "}\n"
                     ]
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "association_json = {\n",
+                "    \"id\": \"https://id\",\n",
                 "    \"type\" : \"Association\",\n",
                 "    \"nanValue\": np.nan,\n",
                 "    \"agent\": jane\n",
                 "}\n",
                 "association = Resource.from_json(association_json, na=np.nan)\n",
                 "print(association)"
             ]
@@ -204,15 +207,15 @@
             "metadata": {},
             "source": [
                 "### from pandas.DataFrame"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -295,15 +298,15 @@
             "metadata": {},
             "source": [
                 "### modification"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 16,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2019-09-23T18:50:20.261616Z",
                     "start_time": "2019-09-23T18:50:20.255355Z"
                 }
             },
             "outputs": [],
@@ -316,72 +319,152 @@
             "metadata": {},
             "source": [
                 "### access"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 17,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2019-09-23T18:50:20.187035Z",
                     "start_time": "2019-09-23T18:50:20.165715Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "'jane.doe@epfl.ch'"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "jane.email"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 18,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2019-09-23T18:50:20.207733Z",
                     "start_time": "2019-09-23T18:50:20.199854Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "'jane.doe@epfl.ch'"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "association.agent.email"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 23,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(True, 'id')"
+                        ]
+                    },
+                    "execution_count": 23,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "association.has_identifier(return_attribute=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 24,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'https://id'"
+                        ]
+                    },
+                    "execution_count": 24,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "association.get_identifier()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 26,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(True, 'type')"
+                        ]
+                    },
+                    "execution_count": 26,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "association.has_type(return_attribute=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 25,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'Association'"
+                        ]
+                    },
+                    "execution_count": 25,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "association.get_type()"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Display"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "{\n",
@@ -394,27 +477,28 @@
             ],
             "source": [
                 "print(jane)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 20,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2019-09-23T18:50:20.332705Z",
                     "start_time": "2019-09-23T18:50:20.325401Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "{\n",
+                        "    id: https://id\n",
                         "    type: Association\n",
                         "    agent:\n",
                         "    {\n",
                         "        type: Person\n",
                         "        email: jane.doe@epfl.ch\n",
                         "        name: Jane Doe\n",
                         "    }\n",
@@ -439,13 +523,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.10"
+            "version": "3.8.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/02 - Datasets.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/02 - Datasets.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994327731092437%*

 * *Differences: {"'cells'": "{20: {'source': {insert: [(0, '# A specific path can be provided.\\n')], delete: [4, "*

 * *            "3, 2, 1, 0]}}, insert: [(19, OrderedDict([('cell_type', 'code'), ('execution_count', "*

 * *            "None), ('metadata', OrderedDict()), ('outputs', []), ('source', ['# By default the "*

 * *            'files are downloaded in the current path (path="."). The urls or the files to '*

 * *            'download can be collected from a different json path (by setting a value for '*

 * *            '"follow") and \\ […]*

```diff
@@ -262,28 +262,49 @@
             ],
             "source": [
                 "forge.as_json(associations)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# By default the files are downloaded in the current path (path=\".\"). The urls or the files to download can be collected from a different json path (by setting a value for \"follow\") and \n",
+                "# the files downloaded to a different path (by setting a value for \"path\")\n",
                 "# The argument overwrite: bool can be provided to decide whether to overwrite (True) existing files with the same name or\n",
                 "# to create new ones (False) with their names suffixed with a timestamp.\n",
-                "\n",
                 "# A cross_bucket argument can be provided to download data from the configured bucket (cross_bucket=False - the default value) \n",
                 "# or from a bucket different than the configured one (cross_bucket=True). The configured store should support crossing buckets for this to work.\n",
+                "associations.download(source=\"parts\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 19,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# A specific path can be provided.\n",
                 "associations.download(path=\"./downloaded/\", source=\"parts\")"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# A specific content type can be downloded.\n",
+                "associations.download(path=\"./downloaded/\", source=\"parts\", content_type=\"text/tab-separated-values\")"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -378,14 +399,25 @@
                 }
             ],
             "source": [
                 "forge.as_json(persons)"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# When files are added as distributions, they can be directly downloaded without specifying which json path to use to collect the downlodable urls. In addition, content type and path arguments\n",
+                "# can still be provided\n",
+                "persons.download()"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creation with resources added as parts"
             ]
         },
         {
```

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/03 - Storing.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/03 - Storing.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/05 - Versioning.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/05 - Versioning.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/06 - JSON IO.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/06 - JSON IO.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/07 - DataFrame IO.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/07 - DataFrame IO.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/08 - Formatting.ipynb` & `nexusforge-0.8.1/tests/KGForge Setup.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9436011904761905%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}, 'source': {insert: [(0, '# Chcek "*

 * *            "requirements\\n'), (2, 'Your python version should be >=3.6')], delete: [2, 0]}}, 1: "*

 * *            "{'execution_count': None, 'metadata': {replace: OrderedDict()}, 'source': ['! python "*

 * *            "--version']}, 2: {'source': ['# First time insatall\\n', '\\n', 'This will create a "*

 * *            "kgforge directory where the project will be cloned.']}, 3: {'execution_count': None, "*

 * *            "'source': […]*

```diff
@@ -1,149 +1,120 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2019-09-23T18:50:19.036357Z",
-                    "start_time": "2019-09-23T18:50:19.031896Z"
-                }
-            },
+            "metadata": {},
             "source": [
-                "# Formatting\n",
+                "# Chcek requirements\n",
                 "\n",
-                "This notebooks demonstrates how to use configured [Formatting](https://nexus-forge.readthedocs.io/en/latest/interaction.html#formatting) string patterns to normalise resource identifiers."
+                "Your python version should be >=3.6"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2019-09-23T18:50:20.068658Z",
-                    "start_time": "2019-09-23T18:50:19.054054Z"
-                }
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from kgforge.core import KnowledgeGraphForge"
+                "! python --version"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A configuration file is needed in order to create a KnowledgeGraphForge session. A configuration can be generated using the notebook [00-Initialization.ipynb](00%20-%20Initialization.ipynb)."
+                "# First time insatall\n",
+                "\n",
+                "This will create a kgforge directory where the project will be cloned."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "forge = KnowledgeGraphForge(\"../../configurations/forge.yml\")"
+                "! git clone https://bbpcode.epfl.ch/code/a/dke/kgforge"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Imports"
+                "Install kgforge in the current kernel."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from kgforge.core import Resource"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from uuid import uuid4"
+                "! pip install ./kgforge"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Using a formatter named 'identifier'"
+                "# Update\n",
+                "\n",
+                "If you already have kgforge, get the latest version."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "uuid = str(uuid4())"
+                "! cd kgforge && git pull && pip install --upgrade ."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 6,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "uid = forge.format(\"identifier\", \"persons\", uuid) # here \"identifier\" is the formatter name as configured while \"persons\" can be seen as a type"
+                "# Setup Neuroshapes localy"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 7,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "resource = Resource(id=uid, type=\"Person\", name=\"Jane Doe\")"
+                "This will allow to use Neuroshapes as a RDF Model for the kgForge.\n",
+                "\n",
+                "Clone the neuroshapes repository."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{\n",
-                        "    id: https://kg.example.ch/persons/25893e86-c363-4943-82c4-d4edbcf71fce\n",
-                        "    type: Person\n",
-                        "    name: Jane Doe\n",
-                        "}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "print(resource)"
+                "! git clone https://github.com/INCF/neuroshapes.git"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.7 (nexusforgelatest)",
+            "display_name": "shacl-tests",
             "language": "python",
-            "name": "nexusforgelatest"
+            "name": "shacl-tests"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.10"
+            "version": "3.7.4"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/09 - Resolving.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/09 - Resolving.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/10 - Reshaping.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/10 - Reshaping.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/11 - Modeling.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/11 - Modeling.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/12 - Mapping.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/12 - Mapping.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/13 - JSON-LD IO.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/13 - JSON-LD IO.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/14 - RDF IO.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/14 - RDF IO.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/15 - SQL IO.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/15 - SQL IO.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/getting-started/16 - Debugging.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/16 - Debugging.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Create Datasets.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Create Datasets.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Ontology Brain Building Workflow Search and Exploration.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Ontology Brain Building Workflow Search and Exploration.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Ontology types Search and Exploration.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Ontology types Search and Exploration.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP KG Search and Download.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/BBP KG Search and Download.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/BBP-KG-Search-and-Download-Data-at-a-given-tag.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/BBP-KG-Search-and-Download-Data-at-a-given-tag.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/EntityLinkerElastic-forge-demo-config.yml` & `nexusforge-0.8.1/examples/notebooks/use-cases/EntityLinkerElastic-forge-demo-config.yml`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/EntityLinkerSkLearn-forge-demo-config.yml` & `nexusforge-0.8.1/examples/notebooks/use-cases/EntityLinkerSkLearn-forge-demo-config.yml`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/MOOC_Content_based_Recommender_System_using_Blue_Brain_Nexus.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/MOOC_Content_based_Recommender_System_using_Blue_Brain_Nexus.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/ResolvingStrategies.ipynb` & `nexusforge-0.8.1/examples/notebooks/getting-started/08 - Formatting.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.904962642609127%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('ExecuteTime', OrderedDict([('end_time', "*

 * *            "'2019-09-23T18:50:19.036357Z'), ('start_time', '2019-09-23T18:50:19.031896Z')]))])}, "*

 * *            "'source': {insert: [(0, '# Formatting\\n'), (2, 'This notebooks demonstrates how to "*

 * *            'use configured '*

 * *            '[Formatting](https://nexus-forge.readthedocs.io/en/latest/interaction.html#formatting) '*

 * *            "string patterns to normalise resource identifiers.')], delete: [2, 0]}} […]*

```diff
@@ -1,191 +1,200 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2019-09-23T18:50:19.036357Z",
+                    "start_time": "2019-09-23T18:50:19.031896Z"
+                }
+            },
             "source": [
-                "# Resolving Strategies\n",
+                "# Formatting\n",
                 "\n",
-                "* Example on how to use resolving strategies\n"
+                "This notebooks demonstrates how to use configured [Formatting](https://nexus-forge.readthedocs.io/en/latest/interaction.html#formatting) string patterns to normalise resource identifiers."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 13,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2019-09-23T18:50:20.068658Z",
                     "start_time": "2019-09-23T18:50:19.054054Z"
                 }
             },
             "outputs": [],
             "source": [
-                "import os\n",
-                "import json\n",
-                "\n",
-                "from kgforge.core import KnowledgeGraphForge\n",
-                "from kgforge.specializations.resources import Dataset"
+                "from kgforge.core import KnowledgeGraphForge"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 2,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "import getpass\n",
-                "TOKEN = getpass.getpass()"
+                "A configuration file is needed in order to create a KnowledgeGraphForge session. A configuration can be generated using the notebook [00-Initialization.ipynb](00%20-%20Initialization.ipynb)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
-                "endpoint = \"https://staging.nise.bbp.epfl.ch/nexus/v1\"\n",
-                "BUCKET = \"dke/kgforge\"\n",
-                "forge = KnowledgeGraphForge(\"../use-cases/prod-forge-nexus.yml\",\n",
-                " endpoint=endpoint, \n",
-                " bucket=BUCKET,\n",
-                " token=TOKEN\n",
-                " )"
+                "forge = KnowledgeGraphForge(\"../../configurations/forge.yml\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 4,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "case_insensitive = forge.resolve('Pv+', scope='ontology', strategy='EXACT_CASEINSENSITIVE_MATCH')"
+                "## Imports"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
-                "exact = forge.resolve('PV+', scope='ontology', strategy='EXACT_MATCH')"
+                "from kgforge.core import Resource"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert case_insensitive == exact"
+                "from uuid import uuid4"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Try with a similar string, but other characters"
+                "## Using a str formatter named 'identifier'"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [],
             "source": [
-                "similar = forge.resolve('pv-', scope='ontology', strategy='EXACT_CASEINSENSITIVE_MATCH')"
+                "uuid = str(uuid4())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [],
             "source": [
-                "similar1 = forge.resolve('pv:', scope='ontology', strategy='EXACT_CASEINSENSITIVE_MATCH')"
+                "# here \"identifier\" is the formatter name as configured while \"persons\" can be seen as a type\n",
+                "# by default, the type of formatter is str.format()\n",
+                "uid = forge.format(\"identifier\", \"persons\", uuid) "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert similar is None\n",
-                "assert similar1 is None"
+                "resource = Resource(id=uid, type=\"Person\", name=\"Jane Doe\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 21,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "{\n",
+                        "    id: https://kg.example.ch/persons/9be10b3c-470c-4a1c-b212-5c118934e055\n",
+                        "    type: Person\n",
+                        "    name: Jane Doe\n",
+                        "}\n"
+                    ]
+                }
+            ],
+            "source": [
+                "print(resource)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Combine spaces and other characters"
+                "## Using a URI_REWRITER formatter\n",
+                "This is a store based URI formatter. Using BlueBrainNexus store, this formatter will output a fully expanded resource._store_metadata._self url value"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 29,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "Resource(_last_action=None, _validated=False, _synchronized=False, _store_metadata=None, id='https://bbp.epfl.ch/ontologies/core/ttypes/229_L6_IT_CTX', type=['Entity', 'Class'], label='229_L6 IT CTX', _inner_sync=False, subClassOf=['https://bbp.epfl.ch/ontologies/core/ttypes/L4_5_6_IT_Car3', 'https://bbp.epfl.ch/ontologies/core/celltypes/NeuronTranscriptomicType'])"
-                        ]
-                    },
-                    "execution_count": 10,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "forge.resolve('229_l6 it ctx', scope='ontology', strategy='EXACT_CASEINSENSITIVE_MATCH')"
+                "from kgforge.core.commons.formatter import Formatter"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 30,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "Resource(_last_action=None, _validated=False, _synchronized=False, _store_metadata=None, id='https://bbp.epfl.ch/ontologies/core/ttypes/264_L5_6_NP_CTX', type=['Entity', 'Class'], label='264_L5/6 NP CTX', _inner_sync=False, subClassOf=['https://bbp.epfl.ch/ontologies/core/ttypes/L5_6_NP_CTX', 'https://bbp.epfl.ch/ontologies/core/celltypes/NeuronTranscriptomicType'])"
+                            "['STR', 'URI_REWRITER']"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 30,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "forge.resolve('264_L5/6 np CTX', scope='ontology', strategy='EXACT_CASEINSENSITIVE_MATCH')"
+                "# List the supported formatter types\n",
+                "[f\"{fm.name}\" for fm in Formatter] "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# When using BlueBrainNexus store, set is_file to True to rewrite a file id or _self \n",
+                "\n",
+                "forge.format(uri=resource.id, formatter=Formatter.URI_REWRITER, is_file=False) "
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.7.13 ('kgforge')",
+            "display_name": "Python 3.7 (nexusforgelatest)",
             "language": "python",
-            "name": "python3"
+            "name": "nexusforgelatest"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.13"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "9ac393a5ddd595f2c78ea58b15bf8d269850a4413729cbea5c5fae9013762763"
-            }
+            "version": "3.8.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/bbp-staging-forge.yml` & `nexusforge-0.8.1/examples/notebooks/use-cases/bbp-staging-forge.yml`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/copy-token.png` & `nexusforge-0.8.1/examples/notebooks/use-cases/copy-token.png`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/dataset_from_different_sources.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/dataset_from_different_sources.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/forge.yml` & `nexusforge-0.8.1/examples/notebooks/use-cases/forge.yml`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/login-ui.png` & `nexusforge-0.8.1/examples/notebooks/use-cases/login-ui.png`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/mappings/allen_ephys_dataset.hjson` & `nexusforge-0.8.1/examples/notebooks/use-cases/mappings/allen_ephys_dataset.hjson`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/mappings/allen_morphology_dataset.hjson` & `nexusforge-0.8.1/examples/notebooks/use-cases/mappings/allen_morphology_dataset.hjson`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/mappings/mouselight_dataset.hjson` & `nexusforge-0.8.1/examples/notebooks/use-cases/mappings/mouselight_dataset.hjson`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/one_cell_minds.ipynb` & `nexusforge-0.8.1/examples/notebooks/use-cases/one_cell_minds.ipynb`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/prod-forge-nexus.yml` & `nexusforge-0.8.1/examples/notebooks/use-cases/prod-forge-nexus.yml`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,29 @@
   ontology:
     - resolver: OntologyResolver
       origin: store
       source: BlueBrainNexus
       targets:
         - identifier: terms
           bucket: neurosciencegraph/datamodels
+        - identifier: CellType
+          bucket: neurosciencegraph/datamodels
+          filters:
+            - path: subClassOf*.id
+              value: BrainCellType
+        - identifier: BrainRegion
+          bucket: neurosciencegraph/datamodels
+          filters:
+            - path: subClassOf*.id
+              value: BrainRegion
+        - identifier: Species
+          bucket: neurosciencegraph/datamodels
+          filters:
+            - path: subClassOf*.id
+              value: Species
       searchendpoints:
         sparql:
           endpoint: "https://bluebrain.github.io/nexus/vocabulary/defaultSparqlIndex"
       result_resource_mapping: https://raw.githubusercontent.com/BlueBrain/nexus-forge/master/examples/configurations/nexus-resolver/term-to-resource-mapping.hjson
   agent:
     - resolver: AgentResolver
       origin: store
```

### Comparing `nexusforge-0.8.0rc3/examples/notebooks/use-cases/rdfmodel/jsonldcontext.json` & `nexusforge-0.8.1/examples/notebooks/use-cases/rdfmodel/jsonldcontext.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgentitylinkingsklearn/__init__.py` & `nexusforge-0.8.1/kgentitylinkingsklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgentitylinkingsklearn/entity_linking_sklearn.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/entity_linker.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,36 +7,42 @@
 # Blue Brain Nexus Forge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
 # 
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
-from pathlib import Path
-from typing import Dict, List, Callable
+from abc import ABCMeta
+from typing import Dict, List, Optional, Tuple, Union, Any
 
-from kgentitylinkingsklearn import EntityLinkerServiceSkLearn
+from kgforge.core import Resource
+from kgforge.core.archetypes import Resolver
 from kgforge.core.commons.actions import LazyAction
-from kgforge.specializations.mappers import DictionaryMapper
-from kgforge.specializations.mappings import DictionaryMapping
-from kgforge.specializations.resolvers import EntityLinker
+from kgforge.core.commons.exceptions import ResolvingError
+from kgforge.core.commons.execution import not_supported
+from kgforge.core.commons.strategies import ResolvingStrategy
 
 
-class EntityLinkerSkLearn(EntityLinker):
+class EntityLinker(Resolver, metaclass=ABCMeta):
 
-    def __init__(self, source: str, targets: List[Dict[str, str]], result_resource_mapping: str,
+    def __init__(self, source: str, targets: List[Dict[str, Any]], result_resource_mapping: str,
                  **source_config) -> None:
         super().__init__(source, targets, result_resource_mapping, **source_config)
 
-    @property
-    def mapping(self) -> Callable:
-        return DictionaryMapping
-
-    @property
-    def mapper(self) -> Callable:
-        return DictionaryMapper
-
-    @staticmethod
-    def _service_from_directory(dirpath: Path, targets: Dict[str, str], ** source_config) -> Dict[str, LazyAction]:
-        # FIXME: the same model is loaded multiple times if provided for multiple targets
-        return {target: LazyAction(EntityLinkerServiceSkLearn.from_pretrained, dirpath, filename) for target, filename in
-                targets.items()}
+    def _resolve(self, text: Union[str, List[str]], target: str, type: str,
+                 strategy: ResolvingStrategy, resolving_context: Any, limit: Optional[int],
+                 threshold: Optional[float]) -> Optional[List[Tuple[str, List[Dict]]]]:
+        if target is not None:
+            if isinstance(self.service, dict):
+                entity_linker_service = self.service[target]
+            else:
+                entity_linker_service = self.service
+        else:
+            raise ResolvingError("A target is required for Entity Linker.")
+        if isinstance(entity_linker_service, LazyAction):
+            entity_linker_service = entity_linker_service.execute()
+            self.service[target] = entity_linker_service
+        mentions = [text] if isinstance(text, str) else text
+        candidates = entity_linker_service.generate_candidates(mentions=mentions, target=target, mention_context=resolving_context,
+                                                               limit=limit, bulk=False)
+        return [(m, entity_linker_service.rank_candidates(candidates=cl, strategy=strategy, threshold=threshold,
+                                                          mention=m, mention_context=resolving_context)) for m, cl in candidates]
```

### Comparing `nexusforge-0.8.0rc3/kgentitylinkingsklearn/entity_linking_sklearn_service.py` & `nexusforge-0.8.1/kgentitylinkingsklearn/entity_linking_sklearn_service.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/__init__.py` & `nexusforge-0.8.1/kgforge/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/__init__.py` & `nexusforge-0.8.1/kgforge/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/archetypes/__init__.py` & `nexusforge-0.8.1/kgforge/core/archetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/archetypes/mapper.py` & `nexusforge-0.8.1/kgforge/core/archetypes/mapper.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/archetypes/mapping.py` & `nexusforge-0.8.1/kgforge/core/archetypes/mapping.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/archetypes/model.py` & `nexusforge-0.8.1/kgforge/core/archetypes/model.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/archetypes/resolver.py` & `nexusforge-0.8.1/kgforge/core/archetypes/resolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,33 +17,42 @@
 from typing import Any, Callable, Dict, List, Optional, Union, Tuple
 
 from kgforge.core import Resource
 from kgforge.core.commons.attributes import repr_class
 from kgforge.core.commons.exceptions import ConfigurationError, ResolvingError
 from kgforge.core.commons.execution import not_supported
 from kgforge.core.commons.imports import import_class
+from kgforge.core.commons.query_builder import QueryBuilder
 from kgforge.core.commons.strategies import ResolvingStrategy
+from kgforge.core.wrappings.paths import Filter, FilterOperator
 
 class Resolver(ABC):
 
     # See demo_resolver.py in kgforge/specializations/resolvers/ for a reference implementation.
 
     # POLICY Methods of archetypes, except __init__, should not have optional arguments.
 
     # POLICY Implementations should be declared in kgforge/specializations/resolvers/__init__.py.
     # POLICY Implementations should not add methods but private functions in the file.
     # TODO Create a generic parameterizable test suite for resolvers. DKE-135.
     # POLICY Implementations should pass tests/specializations/resolvers/test_resolvers.py.
 
-    def __init__(self, source: str, targets: List[Dict[str, str]], result_resource_mapping: str,
+    def __init__(self, source: str, targets: List[Dict[str, Any]], result_resource_mapping: str,
                  **source_config) -> None:
         # POLICY Resolver data access should be lazy, unless it takes less than a second.
         # POLICY There could be data caching but it should be aware of changes made in the source.
         self.source: str = source
-        self.targets: Dict[str, str] = {x["identifier"]: x["bucket"] for x in targets}
+        self.targets: Dict[str, Tuple[str, Dict[str, str]]] = {}
+        for target in targets:
+            if "filters" in target:
+                # reshape filters to match query filters
+                filters = {f["path"]: f["value"] for f in target["filters"]}
+            else:
+                filters = None
+            self.targets[target["identifier"]] = {"bucket": target["bucket"], "filters": filters}
         self.result_mapping: Any = self.mapping.load(result_resource_mapping)
         self.service: Any = self._initialize_service(self.source, self.targets, **source_config)
 
     def __repr__(self) -> str:
         return repr_class(self)
 
     @property
@@ -76,14 +85,15 @@
                     "When resolving a Resource, a property_to_resolve of type str or List[str] should be provided")
 
         elif property_to_resolve is not None or merge_inplace_as is not None:
             not_supported(("property_to_resolve or merge_inplace_as", str))
         else:
             text_to_resolve = text
         # The resolving strategy cannot be abstracted as it should be managed by the service.
+        self._is_target_valid(target)
         resolved = self._resolve(text_to_resolve, target, type, strategy, resolving_context, limit, threshold)
         if resolved is None or len(resolved) == 0:
             return None
         resolved = resolved[0] if len(resolved) == 1 else resolved
         if isinstance(resolved, tuple):
             # Case Tuple[str,List[Dict]]
             resolved_mapped = self.mapper().map(resolved[1], self.result_mapping, None) if resolved[1] is not None else None
@@ -103,17 +113,23 @@
     @abstractmethod
     def _resolve(self, text: Union[str, List[str], Resource], target: str, type: str,
                  strategy: ResolvingStrategy, resolving_context: Any, limit: int, threshold: float) -> Optional[
         List[Any]]:
         # POLICY Should notify of failures with exception ResolvingError including a message.
         pass
 
+    @abstractmethod
+    def _is_target_valid(self, target: str) -> Optional[bool]:
+        # POLICY Should notify of failures with exception ValueError including a message.
+        pass
+
+
     # Utils.
 
-    def _initialize_service(self, source: str, targets: Dict[str, str], **source_config) -> Any:
+    def _initialize_service(self, source: str, targets: Dict[str, Dict[str, Dict[str, str]]], **source_config) -> Any:
         # Resolver data could be accessed from a directory, a web service, or a Store.
         # Initialize the access to the resolver data according to the source type.
         # POLICY Should not use 'self'. This is not a function only for the specialization to work.
         origin = source_config.pop("origin")
         if origin == "directory":
             dirpath = Path(source)
             return self._service_from_directory(dirpath, targets, **source_config)
@@ -123,23 +139,23 @@
             store = import_class(source, "stores")
             return self._service_from_store(store, targets, **source_config)
         else:
             raise ConfigurationError(f"unrecognized Resolver origin '{origin}'")
 
     @staticmethod
     @abstractmethod
-    def _service_from_directory(dirpath: Path, targets: Dict[str, str], **source_config) -> Any:
+    def _service_from_directory(dirpath: Path, targets: Dict[str, Dict[str, Dict[str, str]]], **source_config) -> Any:
         pass
 
     @staticmethod
-    def _service_from_web_service(endpoint: str, targets: Dict[str, str]) -> Any:
+    def _service_from_web_service(endpoint: str, targets: Dict[str,  Dict[str, Dict[str, str]]]) -> Any:
         not_supported()
 
     @staticmethod
-    def _service_from_store(store: Callable, targets: Dict[str, str], **store_config) -> Any:
+    def _service_from_store(store: Callable, targets: Dict[str,  Dict[str, Dict[str, str]]], **store_config) -> Any:
         not_supported()
 
 
 def escape_punctuation(text):
     if not isinstance(text, str):
         raise TypeError('Only accepting strings.')
     punctuation = "-()\"#/@;:<>{}`+=~|.!?,"
@@ -158,7 +174,48 @@
     for property in properties:
         if regex:
             full_str = start_str + f"?{property}, \"{text}\"" + end_str
         else:
             full_str = start_str + f"?{property} = \"{text}\"" + end_str
         filters.append(full_str)
     return filters
+
+
+def _build_resolving_query(text, query_template, deprecated_property, filters, strategy, _type, properties_to_filter_with, resolving_context: Any, query_builder: QueryBuilder, limit: Optional[int]):
+    first_filters = f"?id <{deprecated_property}> \"false\"^^xsd:boolean"
+    if _type:
+        first_filters = f"{first_filters} ; a {_type}"
+
+    if strategy == strategy.EXACT_MATCH:
+        regex = False
+        case_insensitive = False
+        limit = 1
+    elif strategy == strategy.EXACT_CASEINSENSITIVE_MATCH:
+        regex = True
+        case_insensitive = True
+        text = f"^{escape_punctuation(text)}$"
+        limit = 1
+    else:
+        regex = True
+        case_insensitive = True
+        if strategy == strategy.BEST_MATCH:
+            limit = 1
+
+    properties_filters = write_sparql_filters(text, properties_to_filter_with,
+                                            regex, case_insensitive)
+    
+    configured_target_filters = []
+    if filters:
+        for path, value in filters.items():
+            path = path.split(".") if '.' in path else [path]
+            configured_target_filters.append(Filter(operator=FilterOperator.EQUAL, path=path, value=value))
+        target_query_statements, target_query_filters = query_builder.build(None,
+                                                            None,
+                                                            resolving_context,
+                                                            *configured_target_filters)
+        
+        target_query_statements = ";\n ".join(target_query_statements)
+        target_query_filters = "\n ".join(target_query_filters)
+        first_filters = f"{first_filters} ; \n {target_query_statements}"
+        first_filters = f"{first_filters} . \n {target_query_filters}" if len(target_query_filters) > 0 else first_filters
+    query = query_template.format(first_filters, *properties_filters, limit)
+    return query, limit
```

### Comparing `nexusforge-0.8.0rc3/kgforge/core/archetypes/store.py` & `nexusforge-0.8.1/kgforge/core/archetypes/store.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
 import json
 
 import re
 import time
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Match, Optional, Union
+from typing import Any, Callable, Dict, List, Match, Optional, Tuple, Union
 
 from kgforge.core import Resource
 from kgforge.core.commons.attributes import repr_class
+from kgforge.specializations.mappers import DictionaryMapper
 from kgforge.core.commons.context import Context
 from kgforge.core.commons.exceptions import (
     DeprecationError,
     DownloadingError,
     FreezingError,
     RegistrationError,
     TaggingError,
@@ -37,14 +38,16 @@
 
 
 # NB: Do not 'from kgforge.core.archetypes import Resolver' to avoid cyclic dependency.
 
 # FIXME: need to find a comprehensive way (different than list) to get all SPARQL reserved clauses
 from kgforge.core.wrappings.dict import DictWrapper
 
+DEFAULT_LIMIT = 100
+DEFAULT_OFFSET = 0
 SPARQL_CLAUSES = [
     "where",
     "filter",
     "select",
     "union",
     "limit",
     "construct",
@@ -52,15 +55,45 @@
     "bind",
     "values",
     "offset",
     "order by",
     "prefix",
     "graph",
     "distinct",
-    "in"
+    "in",
+    "as",
+    "base",
+    "prefix",
+    "reduced",
+    "describe",
+    "ask",
+    "named",
+    "asc",
+    "desc",
+    "from",
+    "optional",
+    "graph",
+    "regex",
+    "union",
+    "str",
+    "lang",
+    "langmatches",
+    "datatype",
+    "bound",
+    "sameTerm",
+    "isIRI",
+    "isURI",
+    "isBLANK",
+    "isLITERAL",
+    "group",
+    "by",
+    "order",
+    "minus",
+    "not",
+    "exists"
 ]
 
 
 class Store(ABC):
 
     # See demo_store.py in kgforge/specializations/stores/ for a reference implementation.
 
@@ -113,15 +146,15 @@
         """Mapping class to load file_resource_mapping."""
         return None
 
     @property
     def mapper(self) -> Optional[Callable]:
         """Mapper class to map file metadata to a Resource with file_resource_mapping."""
         return None
-
+    
     # [C]RUD.
 
     def register(
         self, data: Union[Resource, List[Resource]], schema_id: str = None
     ) -> None:
         # Replace None by self._register_many to switch to optimized bulk registration.
         run(
@@ -144,20 +177,20 @@
     def _register_one(self, resource: Resource, schema_id: str) -> None:
         # POLICY Should notify of failures with exception RegistrationError including a message.
         # POLICY Resource _store_metadata should be set using wrappers.dict.wrap_dict().
         # TODO This operation might be abstracted here when other stores will be implemented.
         pass
 
     # This expected that '@catch' is not used here. This is for actions.execute_lazy_actions().
-    def upload(self, path: str, content_type: str) -> Union[Resource, List[Resource]]:
+    def upload(self, path: str, content_type: str, forge: Optional['KnowledgeGraphForge']) -> Union[Resource, List[Resource]]:
         # path: Union[FilePath, DirPath].
         if self.file_mapping is not None:
             p = Path(path)
             uploaded = self._upload(p, content_type)
-            return self.mapper().map(uploaded, self.file_mapping, None)
+            return self.mapper(forge).map(uploaded, self.file_mapping, None)
         else:
             raise UploadingError("no file_resource_mapping has been configured")
 
     def _upload(self, path: Path, content_type: str) -> Union[Any, List[Any]]:
         # path: Union[FilePath, DirPath].
         if path.is_dir():
             filepaths = [
@@ -185,76 +218,100 @@
     ) -> Resource:
         # POLICY Should notify of failures with exception RetrievalError including a message.
         # POLICY Resource _store_metadata should be set using wrappers.dict.wrap_dict().
         # POLICY Resource _synchronized should be set to True.
         # TODO These two operations might be abstracted here when other stores will be implemented.
         pass
 
-    def _retrieve_filename(self, id: str) -> str:
+    def _retrieve_filename(self, id: str) -> Tuple[str, str]:
         # TODO This operation might be adapted if other file metadata are needed.
         not_supported()
+    
+    def _prepare_download_one(self,
+        url: str,
+        store_metadata: Optional[DictWrapper],
+        cross_bucket: bool
+    ) -> Tuple[str, str]:
+        # Prepare download url and download bucket
+        not_supported()
 
     def download(
         self,
         data: Union[Resource, List[Resource]],
         follow: str,
         path: str,
         overwrite: bool,
         cross_bucket: bool,
+        content_type: str = None
     ) -> None:
         # path: DirPath.
         urls = []
         store_metadata = []
         to_download = [data] if isinstance(data, Resource) else data
         for d in to_download:
             collected_values = collect_values(d, follow, DownloadingError)
             urls.extend(collected_values)
             store_metadata.extend(
                 [d._store_metadata for _ in range(len(collected_values))]
             )
-        count = len(urls)
-        if count == 0:
+        if len(urls) == 0:
             raise DownloadingError(
                 f"path to follow '{follow}' was not found in any provided resource."
             )
         dirpath = Path(path)
         dirpath.mkdir(parents=True, exist_ok=True)
         timestamp = time.strftime("%Y%m%d%H%M%S")
         filepaths = []
-        for x in urls:
-            filename = self._retrieve_filename(x)
-            filepath = dirpath / filename
-            if not overwrite and filepath.exists():
-                filepaths.append(f"{filepath}.{timestamp}")
-            else:
-                filepaths.append(str(filepath))
-        if count > 1:
-            self._download_many(urls, filepaths, store_metadata, cross_bucket)
+        buckets = []
+        download_urls = []
+        download_store_metadata = []
+        for i, x in enumerate(urls):
+            x_download_url, x_bucket = self._prepare_download_one(x, store_metadata[i], cross_bucket)
+            filename, store_content_type = self._retrieve_filename(x_download_url)
+            if not content_type or (content_type and store_content_type == content_type):
+                filepath = dirpath / filename
+                if not overwrite and filepath.exists():
+                    filepaths.append(f"{filepath}.{timestamp}")
+                else:
+                    filepaths.append(str(filepath))
+                download_urls.append(x_download_url)
+                buckets.append(x_bucket)
+                download_store_metadata.append(store_metadata[i])
+        if len(download_urls) > 1:
+            self._download_many(download_urls, filepaths, download_store_metadata, cross_bucket, content_type, buckets)
+        elif len(download_urls) == 1 :
+            self._download_one(download_urls[0], filepaths[0], download_store_metadata[0], cross_bucket, content_type, buckets[0])
         else:
-            self._download_one(urls[0], filepaths[0], store_metadata[0], cross_bucket)
+            raise DownloadingError(
+                f"No resource with content_type {content_type} was found when following the resource path '{follow}'."
+            )
 
     def _download_many(
         self,
         urls: List[str],
         paths: List[str],
         store_metadata: Optional[List[DictWrapper]],
         cross_bucket: bool,
+        content_type: str,
+        buckets: List[str]
     ) -> None:
         # paths: List[FilePath].
         # Bulk downloading could be optimized by overriding this method in the specialization.
         # POLICY Should follow self._download_one() policies.
-        for url, path in zip(urls, paths):
-            self._download_one(url, path)
+        for url, path, store_m in zip(urls, paths, store_metadata):
+            self._download_one(url, path, store_m, cross_bucket, content_type)
 
     def _download_one(
         self,
         url: str,
         path: str,
         store_metadata: Optional[DictWrapper],
         cross_bucket: bool,
+        content_type: str,
+        bucket: str
     ) -> None:
         # path: FilePath.
         # POLICY Should notify of failures with exception DownloadingError including a message.
         not_supported()
 
     # CR[U]D.
 
@@ -350,52 +407,57 @@
         #   - limit: int,
         #   - offset: int,
         #   - deprecated: bool,
         #   - resolving: str, with values in ('exact', 'fuzzy'),
         #   - lookup: str, with values in ('current', 'children').
         # POLICY Should use sparql() when 'sparql' is chosen as value  for the param 'search_endpoint'.
         # POLICY Should use elastic() when 'elastic' is chosen as value  for the param 'search_endpoint'.
+        # POLICY Given parameters for limit and offset override the input query.
         # POLICY Should notify of failures with exception QueryingError including a message.
         # POLICY Resource _store_metadata should be set using wrappers.dict.wrap_dict().
         # POLICY Resource _synchronized should be set to True.
         # TODO These two operations might be abstracted here when other stores will be implemented.
         not_supported()
 
     def sparql(
-        self, query: str, debug: bool, limit: int = None, offset: int = None, **params
+        self, query: str, debug: bool, limit: int = DEFAULT_LIMIT, offset: int = DEFAULT_OFFSET, **params
     ) -> List[Resource]:
         rewrite = params.get("rewrite", True)
         qr = (
             rewrite_sparql(query, self.model_context, self.service.metadata_context)
             if self.model_context is not None and rewrite
             else query
         )
-        qr = _replace_in_sparql(qr, "LIMIT", limit, 100, r" LIMIT \d+")
-        qr = _replace_in_sparql(qr, "OFFSET", offset, 0, r" OFFSET \d+")
+        if limit:
+            qr = _replace_in_sparql(qr, "LIMIT", limit, DEFAULT_LIMIT, r" LIMIT \d+")
+        if offset:
+            qr = _replace_in_sparql(qr, "OFFSET", offset, DEFAULT_OFFSET, r" OFFSET \d+")
         if debug:
             self._debug_query(qr)
-        return self._sparql(qr, limit, offset, **params)
+        return self._sparql(qr)
 
-    def _sparql(self, query: str, limit: int, offset: int, **params) -> List[Resource]:
+    def _sparql(self, query: str) -> List[Resource]:
         # POLICY Should notify of failures with exception QueryingError including a message.
         # POLICY Resource _store_metadata should not be set (default is None).
         # POLICY Resource _synchronized should not be set (default is False).
         not_supported()
 
     def elastic(
-        self, query: str, debug: bool, limit: int, offset: int
+        self, query: str, debug: bool, limit: int = DEFAULT_LIMIT, offset: int = DEFAULT_OFFSET
     ) -> List[Resource]:
         query_dict = json.loads(query)
-        query_dict["size"] = limit if limit else query_dict.get("size", 100)
-        query_dict["from"] = offset if offset else query_dict.get("from", 0)
+        if limit:
+            query_dict["size"] = limit
+        if offset:
+            query_dict["from"] = offset 
         if debug:
             self._debug_query(query_dict)
-        return self._elastic(json.dumps(query_dict), limit, offset)
+        return self._elastic(json.dumps(query_dict))
 
-    def _elastic(self, query: str, limit: int, offset: int) -> List[Resource]:
+    def _elastic(self, query: str) -> List[Resource]:
         # POLICY Should notify of failures with exception QueryingError including a message.
         # POLICY Resource _store_metadata should not be set (default is None).
         # POLICY Resource _synchronized should not be set (default is False).
         not_supported()
 
     # Versioning.
 
@@ -445,14 +507,22 @@
     @staticmethod
     def _debug_query(query):
         if isinstance(query, Dict):
             print("Submitted query:", query)
         else:
             print(*["Submitted query:", *query.splitlines()], sep="\n   ")
         print()
+    
+    def rewrite_uri(self, uri: str, context: Context, **kwargs) -> str:
+        """Rewrite a given uri using the store Context
+        :param uri: a URI to rewrite.
+        :param context: a Store Context object
+        :return: str
+        """
+        pass
 
 
 def _replace_in_sparql(qr, what, value, default_value, search_regex, replace_if_in_query=True):
 
     is_what_in_query = bool(re.search(f"{search_regex}", qr, flags=re.IGNORECASE))
     if is_what_in_query and value and not replace_if_in_query:
         raise QueryingError(f"Value for '{what}' is present in the provided query and set as argument: set 'replace_if_in_query' to True to replace '{what}' when present in the query.")
@@ -512,15 +582,15 @@
                 return f"{v}{m5}"
 
     g4 = r"([a-zA-Z_]+)"
     g5 = r"([.;]?)"
     g0 = rf"((?<=[\s,[(/|!^])((a|true|false)|{g4}){g5}(?=[\s,\])/|?*+]))"
     g6 = r"(('[^']+')|('''[^\n\r]+''')|(\"[^\"]+\")|(\"\"\"[^\n\r]+\"\"\"))"
     rx = rf"{g0}|{g6}|(?<=< )(.*)(?= >)"
-    qr = re.sub(rx, replace, query, flags=re.VERBOSE)
+    qr = re.sub(rx, replace, query, flags=re.VERBOSE | re.MULTILINE)
 
     if not has_prefixes or "prefix" in str(qr).lower():
         return qr
     else:
         pfx = "\n".join(f"PREFIX {k}: <{v}>" for k, v in prefixes.items())
     if context.has_vocab():
         pfx = "\n".join([pfx, f"PREFIX : <{context.vocab}>"])
```

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/__init__.py` & `nexusforge-0.8.1/kgforge/core/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/actions.py` & `nexusforge-0.8.1/kgforge/core/commons/actions.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/attributes.py` & `nexusforge-0.8.1/kgforge/core/commons/attributes.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/context.py` & `nexusforge-0.8.1/kgforge/core/commons/context.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/dictionaries.py` & `nexusforge-0.8.1/kgforge/core/commons/dictionaries.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,26 @@
 # Blue Brain Nexus Forge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
+import copy
 
 from typing import Dict, List
 
 
 def with_defaults(original: Dict, other: Dict, original_key: str, other_key: str,
                   keys: List[str]) -> None:
     """Update 'original' with 'other' 'keys' unless keys value is different in both dictionaries."""
 
     if original[original_key] == other[other_key]:
         for x in keys:
             if x not in original and x in other:
                 original[x] = other[x]
+
+
+def update_dict(original: Dict, other:Dict) -> Dict:
+    original_copy = copy.deepcopy(original)
+    original_copy.update(other)
+    return original_copy
```

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/es_query_builder.py` & `nexusforge-0.8.1/kgforge/core/commons/es_query_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 if keyword_path:
                     filter_or_must_or_must_not = (
                         "filter"
                         if f.operator == FilterOperator.EQUAL.value
                         else "must_not"
                     )
                     k_path = keyword_path
-                    term_or_match = "term"
+                    term_or_match = "terms" if isinstance(f.value, list) else "term"
                 else:
                     filter_or_must_or_must_not = (
                         "must"
                         if f.operator == FilterOperator.EQUAL.value
                         else "must_not"
                     )
                     k_path = property_path
@@ -132,15 +132,15 @@
                 if keyword_path:
                     filter_or_must_or_must_not = (
                         "filter"
                         if f.operator == FilterOperator.EQUAL.value
                         else "must_not"
                     )
                     k_path = keyword_path
-                    term_or_match = "term"
+                    term_or_match = "terms" if isinstance(f.value, list) else "term"
                 else:
                     filter_or_must_or_must_not = (
                         "must"
                         if f.operator == FilterOperator.EQUAL.value
                         else "must_not"
                     )
                     k_path = property_path
```

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/exceptions.py` & `nexusforge-0.8.1/kgforge/core/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/execution.py` & `nexusforge-0.8.1/kgforge/core/commons/execution.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/files.py` & `nexusforge-0.8.1/kgforge/core/commons/files.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/imports.py` & `nexusforge-0.8.1/kgforge/core/commons/imports.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/parser.py` & `nexusforge-0.8.1/kgforge/core/commons/parser.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/query_builder.py` & `nexusforge-0.8.1/kgforge/core/commons/query_builder.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/commons/strategies.py` & `nexusforge-0.8.1/kgforge/core/commons/strategies.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/conversions/__init__.py` & `nexusforge-0.8.1/kgforge/core/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/conversions/dataframe.py` & `nexusforge-0.8.1/kgforge/core/conversions/dataframe.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/conversions/json.py` & `nexusforge-0.8.1/kgforge/core/conversions/json.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/conversions/rdf.py` & `nexusforge-0.8.1/kgforge/core/conversions/rdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,17 @@
     local_attrs = dict()
     for k, v in dictionary.items():
         if k == "@context":
             if v != context:
                 local_attrs["context"] = v
         else:
             if k == "@id":
+                if not isinstance(v, str):
+                    raise ValueError(f"Invalid value found in data: value of type {type(v)} "
+                                     f"found associated to a \"@id\" key. Only strings are valid")
                 local_attrs["id"] = context.resolve(v)
             elif k.startswith("@") and k in LD_KEYS.values():
                 local_attrs[k[1:]] = v
             else:
                 if isinstance(v, dict):
                     local_attrs[k] = _remove_ld_keys(v, context, to_resource)
                 elif isinstance(v, list):
```

### Comparing `nexusforge-0.8.0rc3/kgforge/core/forge.py` & `nexusforge-0.8.1/kgforge/core/forge.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
 
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+import re
 import numpy as np
 import yaml
 from kgforge.core.commons.files import load_file_as_byte
 from pandas import DataFrame
 from rdflib import Graph
+from urllib.parse import quote_plus, urlparse
 
 from kgforge.core import Resource
 from kgforge.core.archetypes import Mapping, Model, Resolver, Store
+from kgforge.core.commons.context import Context
 from kgforge.core.commons.actions import LazyAction
 from kgforge.core.commons.dictionaries import with_defaults
 from kgforge.core.commons.exceptions import ResolvingError
 from kgforge.core.commons.execution import catch
 from kgforge.core.commons.imports import import_class
 from kgforge.core.commons.strategies import ResolvingStrategy
+from kgforge.core.commons.formatter import Formatter
 from kgforge.core.conversions.dataframe import as_dataframe, from_dataframe
 from kgforge.core.conversions.json import as_json, from_json
 from kgforge.core.conversions.rdf import (
     as_jsonld,
     from_jsonld,
     as_graph,
     from_graph,
@@ -94,14 +98,21 @@
            <scope>:
              - resolver: <a class name of a Resolver>
                origin: <'directory', 'web_service', or 'store'>
                source: <a directory path, a web service endpoint, or the class name of a Store>
                targets:
                  - identifier: <a name, or an IRI>
                    bucket: <a file name, an URL path, or a Store bucket>
+                   filters:
+                     - path: <a resource property path>
+                     - value: <a resource property value to filter with>
+               searchendpoints:
+                 sparql:
+                   endpoint: <A SPARQL endpoint to send resolving query to. Only used for resolvers based on SPARQL>
+               resolve_with_properties: <a list of str currently only supported by DemoResolver>
                result_resource_mapping: <an Hjson string, a file path, or an URL>
                endpoint: <when 'origin' is 'store', a Store endpoint, default to Store:endpoint>
                token: <when 'origin' is 'store', a Store token, default to Store:token>
 
          Formatters:
            <identifier>: <a string template with replacement fields delimited by braces, i.e. '{}'>
 
@@ -146,17 +157,29 @@
                          "resolver": <str>,
                          "origin": <str>,
                          "source": <str>,
                          "targets": [
                              {
                                  "identifier": <str>,
                                  "bucket": <str>,
+                                 "filter":[
+                                    {
+                                        "path": <str>,
+                                        "value": <str>
+                                    }
+                                 ]
                              },
                              ...,
                          ],
+                         "searchendpoints":{
+                            "sparql":{
+                                "endpoint": <str>
+                            }
+                         },
+                         "resolve_with_properties": [str]
                          "result_resource_mapping": <str>,
                          "endpoint": <str>,
                          "token": <str>,
                      },
                      ...,
                  ],
              },
@@ -202,15 +225,14 @@
                 ["endpoint", "token", "bucket", "vocabulary"],
             )
         model_name = model_config.pop("name")
         model = import_class(model_name, "models")
         self._model: Model = model(**model_config)
 
         # Store.
-
         store_config.update(model_context=self._model.context())
         store_name = store_config.pop("name")
         store = import_class(store_name, "stores")
         self._store: Store = store(**store_config)
         store_config.update(name=store_name)
 
         # Resolvers.
@@ -221,16 +243,14 @@
             if resolvers_config
             else None
         )
 
         # Formatters.
         self._formatters: Optional[Dict[str, str]] = config.pop("Formatters", None)
 
-    # Modeling User Interface.
-
     @catch
     def prefixes(self, pretty: bool = True) -> Optional[Dict[str, str]]:
         """
         Print (pretty=True) prefix mappings:
             Used prefixes:
             rdf          http://www.w3.org/1999/02/22-rdf-syntax-ns#
             prov         http://www.w3.org/ns/prov#
@@ -306,14 +326,20 @@
         Print (output='print') the available resolvers or return them based as dictionary (output='dict').
 
         The dictionary returned has the following format:
         {
             "firstResolver": {
                 "firstTarget": {
                     "bucket": "firstSource",
+                    "filters":[
+                        {
+                            "path": "path",
+                            "value": "value"
+                        }
+                    ]
                 },
                 "secondTarget": {
                     "bucket": "secondSource",
                 }
             }
         }
 
@@ -327,20 +353,20 @@
                 for resolver_key, resolver_value in scope_value.items():
                     print("     - resolver: ", resolver_key)
                     print(
                         "         - targets: ", ",".join(resolver_value.targets.keys())
                     )
         elif output == "dict":
             resolvers_dict = dict()
-            # iterate over resolvers and fill dictionary with targets
+            # iterate over target_key, target_value and fill dictionary with targets
             for scope, scope_value in sorted(self._resolvers.items()):
                 individual_dict = dict()
                 for resolver_key, resolver_value in scope_value.items():
                     for target_key, target_value in resolver_value.targets.items():
-                        individual_dict[target_key] = {"bucket": target_value}
+                        individual_dict[target_key] = target_value
                 resolvers_dict[scope] = individual_dict
             return resolvers_dict
         else:
             raise ValueError("unrecognized output")
 
     @catch
     def resolve(
@@ -428,22 +454,57 @@
             )
         else:
             raise ResolvingError("no resolvers have been configured")
 
     # Formatting User Interface.
 
     @catch
-    def format(self, what: str, *args) -> str:
+    def format(self, what: str = None, *args, formatter: Union[Formatter, str] = Formatter.STR, uri: str = None, **kwargs) -> str:
         """
         Select a configured formatter (see https://nexus-forge.readthedocs.io/en/latest/interaction.html#formatting) string (identified by 'what') and format it using provided '*args'
-        :param what: a configured formatter
+        :param what: a configured str format name. Required formatter:str = Formatter.STR
         :param args: a list of string to use for formatting
+        :param formatter: the type of formatter to use. STR (default, corresponds to str.format(*args, **kwargs)), URI_REWRITER (Store based URI rewritter)  
+        :param uri: a URI to rewrite. Required formatter:str = Formatter.URI_REWRITER
         :return: str
         """
-        return self._formatters[what].format(*args)
+        
+        if what and uri:
+            raise AttributeError(
+                    f"both 'what': {what} and 'uri': {uri} arguments are provided. One of them should be provided."
+            )
+
+        try:
+            formatter = (
+                formatter
+                if isinstance(formatter, Formatter)
+                else Formatter[formatter]
+            )
+        except Exception as e:
+            raise AttributeError(
+                f"Invalid Formatter value '{formatter}'. Allowed names are {[name for name, member in Formatter.__members__.items()]} and allowed members are {[member for name, member in Formatter.__members__.items()]}"
+            )
+        
+        if formatter == Formatter.STR:
+            if what is None:
+                raise AttributeError(
+                        f"A non None 'what' value is required when formatter == Formatter.STR"
+                )
+            return self._formatters[what].format(*args, **kwargs)
+        elif formatter == Formatter.URI_REWRITER:
+            if uri is None:
+                raise AttributeError(
+                            f"A non None 'uri' value is required when formatter == Formatter.URI_REWRITER"
+                    )
+            return self._store.rewrite_uri(uri, self.get_store_context(), **kwargs)
+        else:
+            raise AttributeError(
+                    f"{formatter} is not a valid formatter. Valid formatters are {[fm.value for fm in Formatter]}"
+            )
+
 
     # Mapping User Interface.
 
     @catch
     def sources(self, pretty: bool = True) -> Optional[List[str]]:
         """
         Print(pretty=True) or return (pretty=False) configured data sources.
@@ -608,43 +669,46 @@
         """
         return self._store.elastic(query, debug, limit, offset)
 
     @catch
     def download(
         self,
         data: Union[Resource, List[Resource]],
-        follow: str,
-        path: str,
+        follow: str = "distribution.contentUrl",
+        path: str = ".",
         overwrite: bool = False,
         cross_bucket: bool = False,
+        content_type: str = None
     ) -> None:
         """
         Download files attached to a resource or a list of resources.
 
         :param data: the resources whose attached files to download
         :param follow: the property path holding a URL to download the files
         :param path: where to output the downloaded files
         :param overwrite: whether to replace (True) and existing file with the same name or not (False)
         :param cross_bucket: instructs the configured store to whether download files beyond the configured bucket (True) or not (False)
+        :param content_type: the content_type of the files to download
         """
         # path: DirPath.
-        self._store.download(data, follow, path, overwrite, cross_bucket)
+        self._store.download(data, follow, path, overwrite, cross_bucket, content_type)
 
     # Storing User Interface.
 
     # No @catch because the error handling is done by execution.run().
     def register(
         self, data: Union[Resource, List[Resource]], schema_id: Optional[str] = None
     ) -> None:
         """
         Store a resource or list of resources in the configured Store.
 
         :param data: the resources to register
         :param schema_id: an identifier of the schema the registered resources should conform to
         """
+        #self._store.mapper = self._store.mapper(self)
         self._store.register(data, schema_id)
 
     # No @catch because the error handling is done by execution.run().
     def update(
         self, data: Union[Resource, List[Resource]], schema_id: Optional[str] = None
     ) -> None:
         """
@@ -691,19 +755,19 @@
     @catch
     def attach(self, path: str, content_type: str = None) -> LazyAction:
         """
         Return a LazyAction for future upload  of files located in a provided path.
         The output of this method can be used to attach files to a resource: https://nexus-forge.readthedocs.io/en/latest/interaction.html#resource.
 
         :param path: path to upload files from
-        :param content_type: the content_type of the fiels to upload
+        :param content_type: the content_type of the files to upload
         :return: LazyAction
         """
         # path: Union[FilePath, DirPath].
-        return LazyAction(self._store.upload, path, content_type)
+        return LazyAction(self._store.upload, path, content_type, self)
 
     # Converting User Interface.
 
     @catch
     def as_json(
         self,
         data: Union[Resource, List[Resource]],
@@ -724,30 +788,28 @@
             store_metadata,
             self._model.context(),
             self._store.metadata_context,
             self._model.resolve_context,
         )
 
     @catch
-    @catch
     def as_jsonld(
         self,
         data: Union[Resource, List[Resource]],
         form: str = Form.COMPACTED.value,
         store_metadata: bool = False,
         **params
     ) -> Union[Dict, List[Dict]]:
         """
         Convert a resource or a list of resources to JSON-LD.
 
         :param data: the resources to convert
         :param form: whether to expand ('expanded') or compact ('compacted') the JSON-LD output
         :param store_metadata: whether to add (True) store related metadata (e.g rev) to the output or not (False)
-        :param params: a dictionary of parameters. Supported parameters are:
-              [array_as_set] whether to consider JSON arrays as RDF set (default: False)
+        :param params: a dictionary of parameters.
         :return: Union[Dict, List[Dict]]
         """
         return as_jsonld(
             data,
             form,
             store_metadata,
             self._model.context(),
@@ -860,16 +922,23 @@
 
         :param data: the pandas.DataFrame to convert
         :param na: represents missing values
         :param nesting: str to use to detect nested nested properties
         :return: Union[Resource, List[Resource]]
         """
         return from_dataframe(data, na, nesting)
-
-
+    
+    def get_store_context(self):
+        """Expose the context used in the store."""
+        return self._store.context
+
+    def get_model_context(self):
+        """Expose the context used in the model."""
+        return self._model.context()
+    
 def prepare_resolvers(
     config: Dict, store_config: Dict
 ) -> Dict[str, Dict[str, Resolver]]:
     return {
         scope: dict(prepare_resolver(x, store_config) for x in configs)
         for scope, configs in config.items()
     }
```

### Comparing `nexusforge-0.8.0rc3/kgforge/core/reshaping.py` & `nexusforge-0.8.1/kgforge/core/reshaping.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/resource.py` & `nexusforge-0.8.1/kgforge/specializations/models/demo_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,145 @@
-#
+# 
 # Blue Brain Nexus Forge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-#
+# 
 # Blue Brain Nexus Forge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
-#
+# 
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
-from typing import Any, Dict, Optional, Union, List
 
-import hjson
-
-from kgforge.core.commons.attributes import check_collisions, repr_class, sort_attrs
-from kgforge.core.wrappings.dict import DictWrapper
-
-
-# NB: Do not 'from kgforge.core.commons.actions import Action' to avoid cyclic dependency.
-
-
-class Resource:
-
-    # See datasets.py in kgforge/specializations/resources/ for a reference specialization.
-
-    # POLICY Specializations could add methods and attributes if they are added to _RESERVED.
-    # TODO Move from BDD to classical testing to have a more parameterizable test suite. DKE-135.
-    # POLICY Specializations should pass tests/core/resources/resource.feature tests.
-
-    # FIXME remove "_forge" from _RESERVED and implement a "cast" of derived classes to Resource
-    _RESERVED = {"_last_action", "_validated", "_synchronized", "_store_metadata", "_forge", "_inner_sync"}
-
-    def __init__(self, **properties) -> None:
-        check_collisions(self._RESERVED, properties.keys())
-        self.__dict__.update(properties)
-        # Status of the last modifying action performed on the resource.
-        self._last_action: Optional["Action"] = None
-        # True if the resource has been validated.
-        # False if the resource has not been validated yet or a modification has been done since
-        # the last validation.
-        self._validated: bool = False
-        # True if the resource is synchronized with the store.
-        # False if the resource has not been registered yet or a modification has been done since
-        # the synchronization.
-        self._synchronized: bool = False
-        self._inner_sync: bool = False
-        # None until synchronized.
-        # Otherwise, holds the metadata the store returns at synchronization.
-        self._store_metadata: Optional[DictWrapper] = None
-
-    def __repr__(self) -> str:
-        return repr_class(self)
-
-    def __str__(self) -> str:
-        return hjson.dumps(self, indent=4, default=encode, item_sort_key=sort_attrs)
-
-    def __eq__(self, other: object) -> bool:
-        def _data(resource: Resource) -> Dict:
-            return {k: _data(v) if isinstance(v, Resource) else v
-                    for k, v in resource.__dict__.items()
-                    if k not in resource._RESERVED}
-        if type(other) is type(self):
-            sdict = _data(self)
-            odict = _data(other)
-            return sdict == odict
+import json
+import re
+from pathlib import Path
+from typing import Callable, Dict, List, Optional, Tuple, Union
+
+from kgforge.core import Resource
+from kgforge.core.archetypes import Mapping, Model
+from kgforge.core.commons.context import Context
+from kgforge.core.commons.exceptions import ValidationError
+
+
+class DemoModel(Model):
+    """An example to show how to implement a Model and to demonstrate how it is used."""
+
+    def __init__(self, source: str, **source_config) -> None:
+        super().__init__(source, **source_config)
+
+    # Vocabulary.
+
+    def _prefixes(self) -> Dict[str, str]:
+        return self.service.namespaces
+
+    def _types(self) -> List[str]:
+        return [x["label"] for x in self.service.vocabulary["Class"]]
+
+    def context(self) -> Context:
+        ctx = {x["label"]: x["id"] for k, v in self.service.vocabulary.items() for x in v}
+        return Context({"@context": ctx})
+
+    # Templates.
+
+    def _template(self, type: str, only_required: bool) -> Dict:
+        # TODO DKE-148.
+        print("<info> DemoModel does not distinguish values and constraints in templates for now.")
+        # TODO DKE-148.
+        print("<info> DemoModel does not automatically include nested schemas for now.")
+        if only_required:
+            # TODO DKE-148.
+            print("<info> DemoModel does not support keeping only required properties for now.")
+        type_expanded = self.service.expand(type)
+        schema = self.service.schema(type_expanded)
+        return self.service.compact(schema)
+
+    # Mappings.
+
+    def _sources(self) -> List[str]:
+        dirpath = Path(self.source, "mappings")
+        return [x.stem for x in dirpath.iterdir() if x.is_dir()]
+
+    def _mappings(self, source: str) -> Dict[str, List[str]]:
+        dirpath = Path(self.source, "mappings", source)
+        mappings = {}
+        if dirpath.is_dir():
+            for x in dirpath.glob("*/*.hjson"):
+                mappings.setdefault(x.stem, []).append(x.parent.name)
         else:
-            return False
+            raise ValueError("unrecognized source")
+        return mappings
 
-    def __setattr__(self, key, value) -> None:
-        if key not in self._RESERVED:
-            self.__dict__["_validated"] = False
-            self.__dict__["_synchronized"] = False
-        elif key == "_synchronized":
-            self._set_synchronized(value)
-        self.__dict__[key] = value
-
-    def _get_synchronized(self) -> bool:
-        inner = [v._synchronized for v in self.__dict__.values() if isinstance(v, Resource)]
-        if inner:
-            self._inner_sync = (all(inner))
-        if self._inner_sync is False:    
-            return False
+    def mapping(self, entity: str, source: str, type: Callable) -> Mapping:
+        filename = f"{entity}.hjson"
+        filepath = Path(self.source, "mappings", source, type.__name__, filename)
+        if filepath.is_file():
+            return type.load(filepath)
         else:
-            return self.__dict__["_synchronized"]
-    
-    def _set_synchronized(self, sync: bool) -> None:
-        inner = [v for v in self.__dict__.values() if isinstance(v, Resource)]
-        if inner:
-            for iresource in inner:
-                iresource._synchronized = sync
-        self.__dict__["_inner_sync"] = sync
-    
-    _synchronized = property(_get_synchronized, _set_synchronized)
-
-    @classmethod
-    def from_json(cls, data: Union[Dict, List[Dict]], na: Union[Any, List[Any]] = None):
-
-        def _(d: Union[Dict, List[Dict]], nas: List[Any]) -> Resource:
-            if isinstance(d, List):
-                return [_(x,  nas) for x in d]
-            elif isinstance(d, Dict):
-                properties = {k: _(v, nas) for k, v in d.items() if v not in nas}
-                return Resource(**properties)
-            else:
-                return d
+            raise ValueError("unrecognized entity type or source")
 
-        nas = na if isinstance(na, List) else [na]
-        return [_(d, nas) for d in data] if isinstance(data, List) else _(data, nas)
+    # Validation.
 
+    def _validate_one(self, resource: Resource, type_: str) -> None:
+        """
+        Validates the model against a given type provided by type_ parameter.
+        If type_ is None then it looks for type attribute in resource.
+        If the resource is not typed, AttributeError is raised
+        """
+        type_expanded = self.service.expand(type_)
+        schema = self.service.schema(type_expanded)
+        result, reason = self.service.check(resource, schema)
+        if reason is not None:
+            raise ValidationError(reason)
+
+    # Utils.
+
+    @staticmethod
+    def _service_from_directory(dirpath: Path, context_iri: str, **dir_config):
+        return ModelLibrary(dirpath)
+
+
+class ModelLibrary:
+    """Simulate a third-party library handling interactions with the data used by the model."""
+
+    def __init__(self, dirpath: Path):
+        with (dirpath / "namespaces.json").open() as f:
+            self.namespaces: Dict[str, str] = json.load(f)
+        with (dirpath / "vocabulary.json").open() as f:
+            self.vocabulary: Dict = json.load(f)
+        with (dirpath / "schemas.json").open() as f:
+            self.schemas: Dict = json.load(f)
+
+    def expand(self, value: str) -> str:
+        return next(x["id"] for x in self.vocabulary["Class"] if x["label"] == value)
+
+    def compact(self, value: Union[str, Dict]) -> Union[str, Dict]:
+        if isinstance(value, Dict):
+            return {self.compact(k): self.compact(v) for k, v in value.items()}
+        else:
+            return re.sub("[a-z]+:", "", value)
+
+    def schema(self, type_expanded: str) -> Dict:
+        return self.schemas[type_expanded]
 
-def encode(data: Any) -> Union[str, Dict]:
-    if isinstance(data, Resource):
-        return {k: v for k, v in data.__dict__.items() if k not in data._RESERVED}
-    elif type(data).__name__ == "LazyAction":
-        return str(data)
-    elif isinstance(data, set) or isinstance(data, list):
-        return {encode(r) for r in data}
-    else:
-        return data.__dict__
+    def check(self, resource: Resource, schema: Dict) -> Tuple[bool, Optional[str]]:
+        result, reason = (True, None)
+        for k, v in schema.items():
+            compacted = self.compact(k)
+            if isinstance(v, Dict):
+                nested = getattr(resource, compacted)
+                result, reason = self.check(nested, v)
+                if result is False:
+                    return result, reason
+            else:
+                rule = f"{v}(resource, '{compacted}')"
+                try:
+                    checked = eval(rule, {}, {"resource": resource})
+                except (TypeError, NameError, SyntaxError):
+                    pass
+                else:
+                    if not checked:
+                        return False, f"{compacted} is missing"
+        else:
+            return result, reason
```

### Comparing `nexusforge-0.8.0rc3/kgforge/core/wrappings/__init__.py` & `nexusforge-0.8.1/kgforge/core/wrappings/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/wrappings/dict.py` & `nexusforge-0.8.1/kgforge/core/wrappings/dict.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/core/wrappings/paths.py` & `nexusforge-0.8.1/kgforge/core/wrappings/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,16 @@
 
 
 def create_filters_from_dict(filter_dict: Dict, path_prefix=None) -> List[Filter]:
     filters = list()
     if path_prefix is None:
         path_prefix = []
     for k, v in filter_dict.items():
-        path_prefix.append(k)
-        path = list(path_prefix)
+        if '/' in k:
+            path = path_prefix + k.split('/')
+        else:
+            path = path_prefix + [k]
         if isinstance(v, dict):
             filters.extend(create_filters_from_dict(v, path))
         else:
             filters.append(Filter(path, FilterOperator.EQUAL.value, v))
-        path_prefix.remove(k)
     return filters
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/mappers/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/mappers/dictionaries.py` & `nexusforge-0.8.1/kgforge/specializations/mappers/dictionaries.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/mappers/r2rml.py` & `nexusforge-0.8.1/kgforge/specializations/mappers/r2rml.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/mappers/resources.py` & `nexusforge-0.8.1/kgforge/specializations/mappers/resources.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/mappers/tables.py` & `nexusforge-0.8.1/kgforge/specializations/mappers/tables.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/mappings/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/mappings/dictionaries.py` & `nexusforge-0.8.1/kgforge/specializations/mappings/dictionaries.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/demo_model.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/demo_resolver.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,137 +9,103 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
 # 
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
 
 import json
-import re
+from itertools import chain
 from pathlib import Path
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, Iterator, List, Optional, Union, Any
 
-from kgforge.core import Resource
-from kgforge.core.archetypes import Mapping, Model
-from kgforge.core.commons.context import Context
-from kgforge.core.commons.exceptions import ValidationError
-
-
-class DemoModel(Model):
-    """An example to show how to implement a Model and to demonstrate how it is used."""
-
-    def __init__(self, source: str, **source_config) -> None:
-        super().__init__(source, **source_config)
-
-    # Vocabulary.
-
-    def _prefixes(self) -> Dict[str, str]:
-        return self.service.namespaces
-
-    def _types(self) -> List[str]:
-        return [x["label"] for x in self.service.vocabulary["Class"]]
-
-    def context(self) -> Context:
-        ctx = {x["label"]: x["id"] for k, v in self.service.vocabulary.items() for x in v}
-        return Context({"@context": ctx})
-
-    # Templates.
-
-    def _template(self, type: str, only_required: bool) -> Dict:
-        # TODO DKE-148.
-        print("<info> DemoModel does not distinguish values and constraints in templates for now.")
-        # TODO DKE-148.
-        print("<info> DemoModel does not automatically include nested schemas for now.")
-        if only_required:
-            # TODO DKE-148.
-            print("<info> DemoModel does not support keeping only required properties for now.")
-        type_expanded = self.service.expand(type)
-        schema = self.service.schema(type_expanded)
-        return self.service.compact(schema)
-
-    # Mappings.
-
-    def _sources(self) -> List[str]:
-        dirpath = Path(self.source, "mappings")
-        return [x.stem for x in dirpath.iterdir() if x.is_dir()]
-
-    def _mappings(self, source: str) -> Dict[str, List[str]]:
-        dirpath = Path(self.source, "mappings", source)
-        mappings = {}
-        if dirpath.is_dir():
-            for x in dirpath.glob("*/*.hjson"):
-                mappings.setdefault(x.stem, []).append(x.parent.name)
-        else:
-            raise ValueError("unrecognized source")
-        return mappings
+from kgforge.core.archetypes import Resolver
+from kgforge.core.commons.exceptions import ConfigurationError
+from kgforge.core.commons.execution import not_supported
+from kgforge.core.commons.strategies import ResolvingStrategy
+from kgforge.specializations.mappers import DictionaryMapper
+from kgforge.specializations.mappings import DictionaryMapping
 
-    def mapping(self, entity: str, source: str, type: Callable) -> Mapping:
-        filename = f"{entity}.hjson"
-        filepath = Path(self.source, "mappings", source, type.__name__, filename)
-        if filepath.is_file():
-            return type.load(filepath)
-        else:
-            raise ValueError("unrecognized entity type or source")
 
-    # Validation.
+class DemoResolver(Resolver):
+    """An example to show how to implement a Resolver and to demonstrate how it is used."""
 
-    def _validate_one(self, resource: Resource, type_: str) -> None:
-        """
-        Validates the model against a given type provided by type_ parameter.
-        If type_ is None then it looks for type attribute in resource.
-        If the resource is not typed, AttributeError is raised
-        """
-        type_expanded = self.service.expand(type_)
-        schema = self.service.schema(type_expanded)
-        result, reason = self.service.check(resource, schema)
-        if reason is not None:
-            raise ValidationError(reason)
+    def __init__(self, source: str, targets: List[Dict[str, Any]], result_resource_mapping: str,
+                 **source_config) -> None:
+        super().__init__(source, targets, result_resource_mapping, **source_config)
 
-    # Utils.
+    @property
+    def mapping(self) -> Callable:
+        return DictionaryMapping
 
-    @staticmethod
-    def _service_from_directory(dirpath: Path, context_iri: str, **dir_config):
-        return ModelLibrary(dirpath)
+    @property
+    def mapper(self) -> Callable:
+        return DictionaryMapper
 
+    def _resolve(self, text: Union[str, List[str]], target: Optional[str], type: Optional[str],
+                 strategy: ResolvingStrategy, resolving_context: Any, limit: Optional[int], threshold: Optional[float]) -> Optional[List[Dict[str, str]]]:
 
-class ModelLibrary:
-    """Simulate a third-party library handling interactions with the data used by the model."""
+        if isinstance(text, list):
+            not_supported(("text", list))
 
-    def __init__(self, dirpath: Path):
-        with (dirpath / "namespaces.json").open() as f:
-            self.namespaces: Dict[str, str] = json.load(f)
-        with (dirpath / "vocabulary.json").open() as f:
-            self.vocabulary: Dict = json.load(f)
-        with (dirpath / "schemas.json").open() as f:
-            self.schemas: Dict = json.load(f)
-
-    def expand(self, value: str) -> str:
-        return next(x["id"] for x in self.vocabulary["Class"] if x["label"] == value)
-
-    def compact(self, value: Union[str, Dict]) -> Union[str, Dict]:
-        if isinstance(value, Dict):
-            return {self.compact(k): self.compact(v) for k, v in value.items()}
+        resolve_with_properties = None
+        if target is not None:
+            data = self.service[target]["data"]
+            resolve_with_properties = self.service[target]["resolve_with_properties"]
         else:
-            return re.sub("[a-z]+:", "", value)
-
-    def schema(self, type_expanded: str) -> Dict:
-        return self.schemas[type_expanded]
-
-    def check(self, resource: Resource, schema: Dict) -> Tuple[bool, Optional[str]]:
-        result, reason = (True, None)
-        for k, v in schema.items():
-            compacted = self.compact(k)
-            if isinstance(v, Dict):
-                nested = getattr(resource, compacted)
-                result, reason = self.check(nested, v)
-                if result is False:
-                    return result, reason
-            else:
-                rule = f"{v}(resource, '{compacted}')"
-                try:
-                    checked = eval(rule, {}, {"resource": resource})
-                except (TypeError, NameError, SyntaxError):
-                    pass
+            data = chain.from_iterable([self.service[target]["data"] for target in self.targets])
+        resolve_with_properties = ["label", "acronym"] if resolve_with_properties is None else resolve_with_properties
+        if type is not None:
+            data = (x for x in data if x.get("type", None) == type)
+        if strategy == ResolvingStrategy.EXACT_MATCH:
+            try:
+                return next(x for x in data
+                            if text and any([p in x and text == x[p] for p in resolve_with_properties]))
+            except StopIteration:
+                return None
+        elif strategy == ResolvingStrategy.EXACT_CASEINSENSITIVE_MATCH:
+            try:
+                return next(x for x in data
+                            if text and any([p in x and str(text).lower() == str(x[p]).lower() for p in resolve_with_properties]))
+            except StopIteration:
+                return None
+        else:
+            results = [(_dist([str(x[prop]) for prop in resolve_with_properties if prop in x][0], text), x) for x in data
+                       if text and any ([p in x and str(text).lower() in str(x[p]).lower() for p in resolve_with_properties])]
+            if results:
+                ordered = sorted(results, key=lambda x: x[0])
+                if strategy == ResolvingStrategy.BEST_MATCH:
+                    return ordered[0][1]
                 else:
-                    if not checked:
-                        return False, f"{compacted} is missing"
+                    # Case: ResolvingStrategy.ALL_MATCHES.
+                    return [x[1] for x in ordered]
+            else:
+                return None
+
+    def _is_target_valid(self, target: str) -> Optional[bool]:
+        if target and target not in self.service:
+            raise ValueError(f"Unknown target value: {target}. Supported targets are: {self.service.keys()}")
         else:
-            return result, reason
+            return True
+    
+    @staticmethod
+    def _service_from_directory(dirpath: Path, targets: Dict[str,  Dict[str, Dict[str, str]]], **source_config)\
+            -> Dict[str, List[Dict[str, str]]]:
+        resolve_with_properties: List[str] = source_config.pop("resolve_with_properties", None)
+        if isinstance(resolve_with_properties, str):
+            resolve_with_properties = [resolve_with_properties]
+        elif resolve_with_properties is not None and not isinstance(resolve_with_properties, list):
+            raise ConfigurationError(f"The 'resolve_with_properties' should be a list: {resolve_with_properties} provided.")
+        return {target: {"data": list(_load(dirpath, values['bucket'])),
+                         "resolve_with_properties": resolve_with_properties} for target, values in targets.items()}
+
+
+def _dist(x: str, y: str) -> int:
+    return len(x) - len(y)
+
+
+def _load(dirpath: Path, filename: str) -> Iterator[Dict[str, str]]:
+    filepath = dirpath / filename
+    if filepath.is_file():
+        with filepath.open(encoding='utf-8') as f:
+            yield from json.load(f)
+    else:
+        raise ConfigurationError("<source>/<bucket> should be a valid file path")
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/collectors.py` & `nexusforge-0.8.1/kgforge/specializations/models/rdf/collectors.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/directory_service.py` & `nexusforge-0.8.1/kgforge/specializations/models/rdf/directory_service.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/node_properties.py` & `nexusforge-0.8.1/kgforge/specializations/models/rdf/node_properties.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/service.py` & `nexusforge-0.8.1/kgforge/specializations/models/rdf/service.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/store_service.py` & `nexusforge-0.8.1/kgforge/specializations/models/rdf/store_service.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/rdf/utils.py` & `nexusforge-0.8.1/kgforge/specializations/models/rdf/utils.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/models/rdf_model.py` & `nexusforge-0.8.1/kgforge/specializations/models/rdf_model.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resolvers/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resolvers/agent_resolver.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/agent_resolver.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,91 +12,86 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
 import re
 from pathlib import Path
 from typing import List, Dict, Any, Optional, Callable, Union
 
 from kgforge.core.archetypes import Resolver
-from kgforge.core.archetypes.resolver import write_sparql_filters, escape_punctuation
+from kgforge.core.archetypes.resolver import _build_resolving_query
 from kgforge.core.commons.execution import not_supported
+from kgforge.core.commons.sparql_query_builder import SPARQLQueryBuilder
 from kgforge.core.commons.strategies import ResolvingStrategy
 from kgforge.specializations.mappers import DictionaryMapper
 from kgforge.specializations.mappings import DictionaryMapping
 from kgforge.specializations.resolvers.store_service import StoreService
 
 
 class AgentResolver(Resolver):
 
-    def __init__(self, source: str, targets: List[Dict[str, str]], result_resource_mapping: str,
+    def __init__(self, source: str, targets: List[Dict[str, Any]], result_resource_mapping: str,
                  **source_config) -> None:
         super().__init__(source,  targets, result_resource_mapping, **source_config)
 
     @property
     def mapping(self) -> Callable:
         return DictionaryMapping
 
     @property
     def mapper(self) -> Callable:
         return DictionaryMapper
 
     def _resolve(self, text: Union[str, List[str]], target: Optional[str], type: Optional[str],
-                 strategy: ResolvingStrategy, resolving_context: Any, limit: Optional[str], threshold: Optional[float]) -> Optional[List[Dict]]:
+                 strategy: ResolvingStrategy, resolving_context: Any, limit: Optional[int], threshold: Optional[float]) -> Optional[List[Dict]]:
 
         if isinstance(text, list):
             not_supported(("text", list))
-
-        first_filters = f"?id <{self.service.deprecated_property}> \"false\"^^xsd:boolean"
-        if type:
-            first_filters = f"{first_filters} ; a {type}"
-
-        properties = ['name', 'givenName', 'familyName']
-        if strategy == strategy.EXACT_MATCH:
-            regex = False
-            case_insensitive = False
-            limit = 1
-        elif strategy == strategy.EXACT_CASEINSENSITIVE_MATCH:
-            text = f"^{escape_punctuation(text)}$"
-            regex = True
-            case_insensitive = True
-            limit = 1
-        else:
-            regex = True
-            case_insensitive = True
-            if strategy == strategy.BEST_MATCH:
-                limit = 1
-        name_filter, given_name_filter, family_name_filter = write_sparql_filters(text, properties,
-                                                                                  regex, case_insensitive)
-
-        query = """
+        
+        if target and target not in self.service.sources:
+            raise ValueError(f"Unknown target value: {target}. Supported targets for the selected resolvers are: {self.service.sources.keys()}")
+        
+        properties_to_filter_with = ['name', 'givenName', 'familyName']
+        query_template = """
             CONSTRUCT {{
-              ?id a ?type ;
+                ?id a ?type ;
                 name ?name ;
                 givenName ?givenName ;
                 familyName ?familyName
             }} WHERE {{
-              ?id a ?type . 
-              OPTIONAL {{
-                ?id name ?name .
-                ?id givenName ?givenName . 
-                ?id familyName ?familyName .
-              }}
-              {{
-                SELECT * WHERE {{
-                  {{ {0} ; name ?name {1} }} UNION
-                  {{ {0} ; familyName ?familyName; givenName ?givenName {2} }} UNION
-                  {{ {0} ; familyName ?familyName; givenName ?givenName {3} }}
-                }} LIMIT {4}
+              GRAPH ?g {{
+                ?id a ?type .
+                OPTIONAL {{
+                  ?id name ?name .
+                }}
+                OPTIONAL {{
+                  ?id givenName ?givenName .
+                }}
+                OPTIONAL {{
+                  ?id familyName ?familyName .
+                }}
+                {{
+                  SELECT * WHERE {{
+                    {{ {0} ; name ?name {1} }} UNION
+                    {{ {0} ; familyName ?familyName; givenName ?givenName {2} }} UNION
+                    {{ {0} ; familyName ?familyName; givenName ?givenName {3} }}
+                  }} LIMIT {4}
+                }}
               }}
             }}
-            """.format(first_filters, name_filter, given_name_filter, family_name_filter, limit)
-
-        expected_fields = ["type", "name", "familyName", "givenName"]
-        return self.service.perform_query(query, target, expected_fields, None)
+            """
+        filters = self.service.filters[target] if target in self.service.filters else None
+        context = self.service.get_context(resolving_context, target, filters)
+        query, strategy_dependant_limit = _build_resolving_query(text, query_template, self.service.deprecated_property, self.service.filters[target], strategy, type, properties_to_filter_with, context, SPARQLQueryBuilder, limit)
+        expected_fields = properties_to_filter_with+["type"]
+        return self.service.perform_query(query, target, expected_fields, strategy_dependant_limit)
+    
+    def _is_target_valid(self, target) -> Optional[bool]:
+        return self.service.validate_target(target)
 
     @staticmethod
     def _service_from_directory(dirpath: Path, targets: Dict[str, str], **source_config) -> Any:
         not_supported()
 
     @staticmethod
-    def _service_from_store(store: Callable, targets: Dict[str, str], **store_config) -> StoreService:
+    def _service_from_store(store: Callable, targets: Dict[str, Dict[str, Dict[str, str]]], **store_config) -> StoreService:
         return StoreService(store, targets, **store_config)
 
+
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resolvers/demo_resolver.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/ontology_resolver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,110 @@
-# 
+#
 # Blue Brain Nexus Forge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # Blue Brain Nexus Forge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
-
-import json
-from itertools import chain
 from pathlib import Path
-from typing import Callable, Dict, Iterator, List, Optional, Union, Any
+from typing import List, Dict, Any, Optional, Callable, Union
 
 from kgforge.core.archetypes import Resolver
-from kgforge.core.commons.exceptions import ConfigurationError
+from kgforge.core.archetypes.resolver import _build_resolving_query
 from kgforge.core.commons.execution import not_supported
+from kgforge.core.commons.sparql_query_builder import SPARQLQueryBuilder
 from kgforge.core.commons.strategies import ResolvingStrategy
 from kgforge.specializations.mappers import DictionaryMapper
 from kgforge.specializations.mappings import DictionaryMapping
+from kgforge.specializations.resolvers.store_service import StoreService
 
 
-class DemoResolver(Resolver):
-    """An example to show how to implement a Resolver and to demonstrate how it is used."""
+class OntologyResolver(Resolver):
 
-    def __init__(self, source: str, targets: List[Dict[str, str]], result_resource_mapping: str,
+    def __init__(self, source: str, targets: List[Dict[str, Any]], result_resource_mapping: str,
                  **source_config) -> None:
-        super().__init__(source, targets, result_resource_mapping, **source_config)
+        super().__init__(source,  targets, result_resource_mapping, **source_config)
 
     @property
     def mapping(self) -> Callable:
         return DictionaryMapping
 
     @property
     def mapper(self) -> Callable:
         return DictionaryMapper
 
     def _resolve(self, text: Union[str, List[str]], target: Optional[str], type: Optional[str],
-                 strategy: ResolvingStrategy, resolving_context: Any, limit: Optional[str], threshold=Optional[float]) -> Optional[List[Dict[str, str]]]:
+                 strategy: ResolvingStrategy, resolving_context: Any, limit: Optional[int], threshold: Optional[float]) \
+            -> Optional[List[Dict]]:
 
         if isinstance(text, list):
             not_supported(("text", list))
+        # Use as default type owl:Class
+        if type is None:
+            type = "Class"
+
+        properties_to_filter_with = ['label', 'notation', 'prefLabel', 'altLabel']        
+        query_template = """
+        CONSTRUCT {{
+            ?id a ?type ;
+            label ?label ;
+            prefLabel ?prefLabel ;
+            altLabel ?altLabel ;
+            definition ?definition;
+            subClassOf ?subClassOf ;
+            isDefinedBy ?isDefinedBy ;
+            notation ?notation
+        }} WHERE {{
+            GRAPH ?g {{
+                ?id a ?type ;
+                    label ?label ; 
+                OPTIONAL {{
+                ?id subClassOf ?subClassOf ;
+                }}
+                OPTIONAL {{
+                ?id definition ?definition ;
+                }}
+                OPTIONAL {{
+                ?id prefLabel ?prefLabel .
+                }}
+                OPTIONAL {{
+                ?id altLabel ?altLabel .
+                }}
+                OPTIONAL {{
+                ?id isDefinedBy ?isDefinedBy .
+                }}     
+                OPTIONAL {{
+                ?id notation ?notation .
+                }}    
+                {{
+                SELECT * WHERE {{
+                    {{ {0} ; label ?label {1} }} UNION
+                    {{ {0} ; notation ?notation {2} }} UNION
+                    {{ {0} ; prefLabel ?prefLabel {3} }} UNION
+                    {{ {0} ; altLabel ?altLabel {4} }}
+                }} LIMIT {5}
+                }}
+            }}
+        }}
+        """
+        filters = self.service.filters[target] if target in self.service.filters else None
+        context = self.service.get_context(resolving_context, target, filters)
+        query, strategy_dependant_limit = _build_resolving_query(text, query_template, self.service.deprecated_property, filters, strategy, type, properties_to_filter_with, context, SPARQLQueryBuilder, limit)
+        expected_fields = properties_to_filter_with+["type",  "definition", "subClassOf", "isDefinedBy"]
+        return self.service.perform_query(query, target, expected_fields, strategy_dependant_limit)
+
+    def _is_target_valid(self, target) -> Optional[bool]:
+        return self.service.validate_target(target)
 
-        resolve_with_properties = None
-        if target is not None:
-            data = self.service[target]["data"]
-            resolve_with_properties = self.service[target]["resolve_with_properties"]
-        else:
-            data = chain.from_iterable([self.service[target]["data"] for target in self.targets])
-        resolve_with_properties = ["label", "acronym"] if resolve_with_properties is None else resolve_with_properties
-        if type is not None:
-            data = (x for x in data if x.get("type", None) == type)
-        if strategy == ResolvingStrategy.EXACT_MATCH:
-            try:
-                return next(x for x in data
-                            if text and any([p in x and text == x[p] for p in resolve_with_properties]))
-            except StopIteration:
-                return None
-        elif strategy == ResolvingStrategy.EXACT_CASEINSENSITIVE_MATCH:
-            try:
-                return next(x for x in data
-                            if text and any([p in x and str(text).lower() == str(x[p]).lower() for p in resolve_with_properties]))
-            except StopIteration:
-                return None
-        else:
-            results = [(_dist([str(x[prop]) for prop in resolve_with_properties if prop in x][0], text), x) for x in data
-                       if text and any ([p in x and str(text).lower() in str(x[p]).lower() for p in resolve_with_properties])]
-            if results:
-                ordered = sorted(results, key=lambda x: x[0])
-                if strategy == ResolvingStrategy.BEST_MATCH:
-                    return ordered[0][1]
-                else:
-                    # Case: ResolvingStrategy.ALL_MATCHES.
-                    return [x[1] for x in ordered]
-            else:
-                return None
+    @staticmethod
+    def _service_from_directory(dirpath: Path, targets: Dict[str,  Dict[str, Dict[str, str]]], **source_config) -> Any:
+        not_supported()
 
     @staticmethod
-    def _service_from_directory(dirpath: Path, targets: Dict[str, str], **source_config)\
-            -> Dict[str, List[Dict[str, str]]]:
-        resolve_with_properties: List[str] = source_config.pop("resolve_with_properties", None)
-        if isinstance(resolve_with_properties, str):
-            resolve_with_properties = [resolve_with_properties]
-        elif resolve_with_properties is not None and not isinstance(resolve_with_properties, list):
-            raise ConfigurationError(f"The 'resolve_with_properties' should be a list: {resolve_with_properties} provided.")
-        return {target: {"data": list(_load(dirpath, filename)),
-                         "resolve_with_properties": resolve_with_properties} for target, filename in targets.items()}
-
-
-def _dist(x: str, y: str) -> int:
-    return len(x) - len(y)
-
-
-def _load(dirpath: Path, filename: str) -> Iterator[Dict[str, str]]:
-    filepath = dirpath / filename
-    if filepath.is_file():
-        with filepath.open(encoding='utf-8') as f:
-            yield from json.load(f)
-    else:
-        raise ConfigurationError("<source>/<bucket> should be a valid file path")
+    def _service_from_store(store: Callable, targets: Dict[str,  Dict[str, Dict[str, str]]], **store_config) -> StoreService:
+        return StoreService(store, targets, **store_config)
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/service/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/service/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/service/entity_linking_elastic_service.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/service/entity_linking_elastic_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,18 @@
         targets: Dict[str, str],
         encoder,
         result_resource_mapping,
         **store_config
     ):
         super().__init__(is_distance=False)
         self.sources: Dict[str, Store] = dict()
-        for target, bucket in targets.items():
+        for identifier in targets:
+            bucket = targets[identifier]['bucket']
             store_config.update(bucket=bucket)
-            self.sources[target] = store(**store_config)
+            self.sources[identifier] = store(**store_config)
         self.encoder = encoder
         self.result_mapping: Any = self.mapping.load(result_resource_mapping)
 
     @property
     def mapping(self) -> Callable:
         return DictionaryMapping
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resolvers/entity_linking/service/entity_linking_service.py` & `nexusforge-0.8.1/kgforge/specializations/resolvers/entity_linking/service/entity_linking_service.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resources/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resources/datasets.py` & `nexusforge-0.8.1/kgforge/specializations/resources/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
 # 
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
 
 from typing import List, Union
+from warnings import warn
 
 from kgforge.core import Resource
 from kgforge.core.commons.actions import LazyAction
 from kgforge.core.commons.execution import catch, not_supported
 from kgforge.core.forge import KnowledgeGraphForge
 
 
@@ -110,26 +111,53 @@
     @catch
     def add_files(self, path: str, content_type: str = None) -> None:
         # path: DirPath.
         """Add (different) files as parts of the dataset."""
         action = self._forge.attach(path, content_type)
         distribution = Resource(distribution=action)
         _set(self, "hasPart", distribution)
-
+ 
     @catch
-    def download(self, path: str, source: str = "distributions", overwrite: bool = False, cross_bucket: bool = False) -> None:
-        # path: DirPath.
-        """Download the distributions of the dataset or the files part of the dataset."""
-        if source == "distributions":
-            follow = "distribution.contentUrl"
-        elif source == "parts":
-            follow = "hasPart.distribution.contentUrl"
-        else:
-            raise ValueError("unrecognized source")
-        self._forge.download(self, follow, path, overwrite, cross_bucket)
+    def download(self, path: str = ".", source: str = "distributions", follow: str = None, overwrite: bool = False, cross_bucket: bool = False,
+                 content_type: str = None) -> None:
+        """
+        Download the distributions of the dataset or the files part of the dataset.
+        :param path: where to output the downloaded files
+        :param source: [Deprecated] aliases to instruct forge the json path to use to collect downloadable file urls. Supported values are:
+              [distributions] corresponding to the json path "distribution.contentUrl" (default)
+              [parts] corresponding to the json path "hasPart.distribution.contentUrl"
+        :param follow: the json property path holding a URL to download the files. This argument is exclusive to the 'source' argument
+        :param overwrite: whether to replace (True) and existing file with the same name or not (False)
+        :param cross_bucket: instructs the configured store to whether download files beyond the configured bucket (True) or not (False)
+        :param content_type: the content_type of the files to download
+        """
+        if source:
+            warn(
+                DeprecationWarning(
+                    "the source argument is deprecated and will be removed in nexusforge 1.0.0. Use the 'follow' argument instead"
+                )
+            )
+        if source and follow:
+            warn(
+                Warning(
+                    f"both 'source' {source} and 'follow' {follow} arguments are provided. 'follow' argument will be used. Consider providing one of the two arguments."
+                )
+            )
+        if follow is None:
+            if source == "distributions":
+                follow = "distribution.contentUrl"
+            elif source == "parts":
+                follow = "hasPart.distribution.contentUrl"
+            elif source:
+                raise ValueError("unrecognized source. Use 'distributions' if the downloadable url is the value of 'distribution.contentUrl' or 'parts' if the downloadable url is the value of 'hasPart.distribution.contentUrl'")
+            else:
+                raise ValueError(
+                    "'source' or 'follow' argument should be provided."
+                )
+        self._forge.download(self, follow, path, overwrite, cross_bucket, content_type)
 
     @classmethod
     def from_resource(cls, forge: KnowledgeGraphForge, data: Union[Resource, List[Resource]],
                       store_metadata: bool = False):
         def _(d):
             resource_json = forge.as_json(d)
             dataset = cls(forge, **resource_json)
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/resources/entity_linking_candidate.py` & `nexusforge-0.8.1/kgforge/specializations/resources/entity_linking_candidate.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/stores/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/stores/bluebrain_nexus.py` & `nexusforge-0.8.1/kgforge/specializations/stores/bluebrain_nexus.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 import json
 import mimetypes
 import re
 from asyncio import Semaphore, Task
 from enum import Enum
 from json import JSONDecodeError
 
+from kgforge.core.commons.dictionaries import update_dict
 from kgforge.core.commons.es_query_builder import ESQueryBuilder
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from urllib.parse import quote_plus, unquote, urlparse, parse_qs
+from kgforge.core.commons.sparql_query_builder import SPARQLQueryBuilder
 
 import nexussdk as nexus
 import requests
 from aiohttp import ClientSession, MultipartWriter
 from aiohttp.hdrs import CONTENT_DISPOSITION, CONTENT_TYPE
 from numpy import nan
 from pyld import jsonld
@@ -60,14 +62,15 @@
 from kgforge.core.conversions.rdf import as_jsonld, from_jsonld
 from kgforge.core.wrappings.dict import DictWrapper
 from kgforge.core.wrappings.paths import Filter, create_filters_from_dict
 from kgforge.specializations.mappers import DictionaryMapper
 from kgforge.specializations.mappings import DictionaryMapping
 from kgforge.specializations.stores.nexus.service import BatchAction, Service
 
+
 class CategoryDataType(Enum):
     DATETIME = "datetime"
     NUMBER = "number"
     BOOLEAN = "boolean"
     LITERAL = "literal"
 
 
@@ -128,17 +131,17 @@
         )
 
     @property
     def mapping(self) -> Optional[Callable]:
         return DictionaryMapping
 
     @property
-    def mapper(self) -> Optional[Callable]:
+    def mapper(self) -> Optional[DictionaryMapper]:
         return DictionaryMapper
-
+    
     def register(
         self, data: Union[Resource, List[Resource]], schema_id: str = None
     ) -> None:
         run(
             self._register_one,
             self._register_many,
             data,
@@ -205,26 +208,32 @@
             metadata_context=None,
             context_resolver=self.service.resolve_context
         )
 
         try:
             schema = quote_plus(schema_id) if schema_id else "_"
             url_base = f"{self.service.url_resources}/{schema}"
-            url = (
-                f"{url_base}/{quote_plus(data['@id'])}"
-                if hasattr(data, "@id")
-                else url_base
-            )
             params_register = copy.deepcopy(self.service.params.get("register", None))
-            response = requests.post(
-                url,
-                headers=self.service.headers,
-                data=json.dumps(data, ensure_ascii=True),
-                params=params_register,
-            )
+            identifier = resource.get_identifier()
+            if identifier:
+                url = f"{url_base}/{quote_plus(identifier)}"
+                response = requests.put(
+                    url,
+                    headers=self.service.headers,
+                    data=json.dumps(data, ensure_ascii=True),
+                    params=params_register,
+                )
+            else:
+                url = url_base
+                response = requests.post(
+                    url,
+                    headers=self.service.headers,
+                    data=json.dumps(data, ensure_ascii=True),
+                    params=params_register,
+                )
             response.raise_for_status()
 
         except nexus.HTTPError as e:
             raise RegistrationError(_error_message(e))
         else:
             response_json = response.json()
             resource.id = response_json["@id"]
@@ -339,160 +348,188 @@
         else:
             url = url_resource
         try:
             response = requests.get(
                 url, params=query_params, headers=self.service.headers
             )
             response.raise_for_status()
+        except HTTPError as er:
+            if cross_bucket:
+                nexus_path = f"{self.service.endpoint}/resources/" 
+            else:
+                nexus_path = self.service.url_resources
+            # Try to use the id as it was given
+            if id.startswith(nexus_path):
+                url_resource = id_without_query
+                if retrieve_source and not cross_bucket:
+                    url = "/".join((id_without_query, "source"))
+                else: 
+                    url = id_without_query
+                try:
+                    response = requests.get(
+                        url, params=query_params, headers=self.service.headers
+                    )
+                    response.raise_for_status()
+                except HTTPError as e:
+                    raise RetrievalError(_error_message(e))
+            else:
+                raise RetrievalError(_error_message(er))
+        finally:
             if retrieve_source and not cross_bucket:
 
                 response_metadata = requests.get(
                     url_resource, params=query_params, headers=self.service.headers
                 )
                 response_metadata.raise_for_status()
-            if retrieve_source and cross_bucket:
+            elif retrieve_source and cross_bucket and response and ('_self' in response.json()):
                 response_metadata = requests.get(
                     "/".join([response.json()["_self"], "source"]), params=query_params, headers=self.service.headers
                 )
                 response_metadata.raise_for_status()
-
-        except HTTPError as e:
-            raise RetrievalError(_error_message(e))
-        else:
+            else:
+                response_metadata = True  # when retrieve_source is False
+        if response and response_metadata:
             try:
                 data = response.json()
                 resource = self.service.to_resource(data)
+            except Exception as e:
+                raise ValueError(e)
+
+            try:
                 if retrieve_source and not cross_bucket:
                     data = response_metadata.json()
                 if retrieve_source and cross_bucket:
                     resource = self.service.to_resource(response_metadata.json())
             except Exception as e:
                 self.service.synchronize_resource(
-                    resource, data, self.retrieve.__name__, False, False
+                        resource, data, self.retrieve.__name__, False, False
                 )
                 raise ValueError(e)
+
+
             finally:
                 self.service.synchronize_resource(
                     resource, data, self.retrieve.__name__, True, True
                 )
             return resource
 
-    def _retrieve_filename(self, id: str) -> str:
+    def _retrieve_filename(self, id: str) -> Tuple[str, str]:
         try:
             response = requests.get(id, headers=self.service.headers)
             response.raise_for_status()
             metadata = response.json()
-            return metadata["_filename"]
+            return metadata["_filename"], metadata["_mediaType"]
         except HTTPError as e:
             raise DownloadingError(_error_message(e))
 
     def _download_many(
         self,
         urls: List[str],
         paths: List[str],
         store_metadata: Optional[DictWrapper],
         cross_bucket: bool,
+        content_type: str,
+        buckets: List[str]
     ) -> None:
         async def _bulk():
             loop = asyncio.get_event_loop()
             semaphore = Semaphore(self.service.max_connection)
-            async with ClientSession(headers=self.service.headers_download) as session:
+            headers = self.service.headers_download if not content_type else update_dict(self.service.headers_download, {"Accept":content_type})
+            async with ClientSession(headers=headers) as session:
                 tasks = (
-                    _create_task(x, y, z, loop, semaphore, session)
-                    for x, y, z in zip(urls, paths, store_metadata)
+                    _create_task(x, y, z, b, loop, semaphore, session)
+                    for x, y, z, b in zip(urls, paths, store_metadata, buckets)
                 )
                 return await asyncio.gather(*tasks)
 
-        def _create_task(url, path, store_metadata, loop, semaphore, session):
+        def _create_task(url, path, store_metadata, bucket, loop, semaphore, session):
             return loop.create_task(
-                _download(url, path, store_metadata, semaphore, session)
+                _download(url, path, store_metadata, bucket, semaphore, session)
             )
 
-        async def _download(url, path, store_metadata, semaphore, session):
+        async def _download(url, path, store_metadata, bucket, semaphore, session):
             async with semaphore:
                 params_download = copy.deepcopy(self.service.params.get("download", {}))
-                url_base, org, project = self._prepare_download_one(
-                    url, path, store_metadata, cross_bucket
-                )
-                async with session.get(url_base, params=params_download) as response:
+                async with session.get(url, params=params_download) as response:
                     try:
                         response.raise_for_status()
                     except Exception as e:
                         raise DownloadingError(
-                            f"Downloading from {org}/{project}:{_error_message(e)}"
+                            f"Downloading url {url} from bucket {bucket} failed: {_error_message(e)}"
                         )
                     else:
                         with open(path, "wb") as f:
                             data = await response.read()
                             f.write(data)
 
         return asyncio.run(_bulk())
 
     def _download_one(
         self,
         url: str,
         path: str,
         store_metadata: Optional[DictWrapper],
         cross_bucket: bool,
+        content_type: str,
+        bucket: str
     ) -> None:
-        url_base, org, project = self._prepare_download_one(
-            url, path, store_metadata, cross_bucket
-        )
+        
         try:
             params_download = copy.deepcopy(self.service.params.get("download", {}))
+            headers = self.service.headers_download if not content_type else update_dict(self.service.headers_download, {"Accept": content_type})
+
             response = requests.get(
-                url=url_base,
-                headers=self.service.headers_download,
+                url=url,
+                headers=headers,
                 params=params_download
             )
             response.raise_for_status()
         except Exception as e:
             raise DownloadingError(
-                f"Downloading from {org}/{project} failed :{_error_message(e)}"
+                f"Downloading from bucket {bucket} failed: {_error_message(e)}"
             )
         else:
             with open(path, "wb") as f:
                 for chunk in response.iter_content(chunk_size=4096):
                     f.write(chunk)
 
     def _prepare_download_one(
         self,
         url: str,
-        path: str,
         store_metadata: Optional[DictWrapper],
-        cross_bucket: bool,
+        cross_bucket: bool
     ) -> Tuple[str, str, str]:
-        # this is a hack since _self and _id have the same uuid
-        file_id = url.split("/")[-1]
-        file_id = unquote(file_id)
-        if file_id.startswith("http"):
-            file_id = file_id.split("/")[-1]
-        if len(file_id) < 1:
-            raise DownloadingError("Invalid file name")
         if cross_bucket:
             if store_metadata is not None:
                 project = store_metadata._project.split("/")[-1]
                 org = store_metadata._project.split("/")[-2]
             else:
                 raise ValueError(
                     f"Downloading non registered file is not allowed when cross_bucket is set to {cross_bucket}"
                 )
         else:
             org = self.service.organisation
             project = self.service.project
-
-        url_base = "/".join(
-            (
-                self.service.url_base_files,
-                quote_plus(org),
-                quote_plus(project),
-                quote_plus(file_id),
+        file_id = url.split("/")[-1]
+        file_id = unquote(file_id)
+        if len(file_id) < 1:
+            raise DownloadingError(f"Invalid file url: {url}")
+        elif file_id.startswith("http"):
+            url_base = url
+        else: 
+            # this is a hack since _self and _id have the same uuid
+            url_base = "/".join(
+                (
+                    self.service.url_base_files,
+                    quote_plus(org),
+                    quote_plus(project),
+                    quote_plus(file_id),
+                )
             )
-        )
-        return url_base, org, project
+        return url_base, f"{org}/{project}"
 
     # CR[U]D.
 
     def update(self, data: Union[Resource, List[Resource]], schema_id: str) -> None:
         run(
             self._update_one,
             self._update_many,
@@ -673,15 +710,16 @@
             self.service.elastic_endpoint["type"],
         ]:
             raise ValueError(
                 f"The provided search_endpoint value '{search_endpoint}' is not supported. Supported "
                 f"search_endpoint values are: '{self.service.sparql_endpoint['type'], self.service.elastic_endpoint['type']}'"
             )
         if "filters" in params:
-            raise ValueError("A 'filters' key was provided as params. Filters should be provided as iterable to be unpacked.")
+            raise ValueError(
+                "A 'filters' key was provided as params. Filters should be provided as iterable to be unpacked.")
 
         if bucket and not cross_bucket:
             not_supported(("bucket", True))
 
         if filters and isinstance(filters[0], dict):
             filters = create_filters_from_dict(filters[0])
         filters = list(filters) if not isinstance(filters, list) else filters
@@ -693,24 +731,25 @@
                 )
             project_filter = ""
             if bucket:
                 project_filter = f"Filter (?_project = <{'/'.join([self.endpoint, 'projects', bucket])}>)"
             elif not cross_bucket:
                 project_filter = f"Filter (?_project = <{'/'.join([self.endpoint, 'projects', self.organisation, self.project])}>)"
 
-            query_statements, query_filters = build_sparql_query_statements(
-                self.model_context, filters
+            query_statements, query_filters = SPARQLQueryBuilder.build(
+                None, resolvers, self.model_context, *filters
             )
             retrieve_source = params.get("retrieve_source", True)
             store_metadata_statements = []
             if retrieve_source:
                 _vars = ["?id"]
                 for i, k in enumerate(self.service.store_metadata_keys):
                     _vars.append(f"?{k}")
-                    store_metadata_statements.insert(i+2, f"<{self.metadata_context.terms[k].id}> ?{k}")
+                    store_metadata_statements.insert(
+                        i + 2, f"<{self.metadata_context.terms[k].id}> ?{k}")
                 deprecated_filter = f"Filter (?_deprecated = {format_type[CategoryDataType.BOOLEAN](deprecated)})"
                 query_filters.append(deprecated_filter)
             else:
                 _vars = ["?id", "?_project", "?_rev"]
                 store_metadata_statements.append(f"<{self.service.revision_property}> ?_rev")
                 store_metadata_statements.append(f"<{self.service.project_property}> ?_project")
                 query_statements.append(
@@ -817,15 +856,15 @@
                 excludes=excludes,
             )
 
             return self.elastic(
                 json.dumps(query), debug=debug, limit=limit, offset=offset
             )
 
-    def _sparql(self, query: str, limit: int, offset: int = None, **params) -> List[Resource]:
+    def _sparql(self, query: str) -> List[Resource]:
         try:
             response = requests.post(
                 self.service.sparql_endpoint["endpoint"],
                 data=query,
                 headers=self.service.headers_sparql,
             )
             response.raise_for_status()
@@ -872,25 +911,27 @@
 
                 return [triples_to_resource(s, t) for s, t in subject_triples.items()]
 
             else:
                 # SELECT QUERY
                 results = data["results"]["bindings"]
                 return [
-                    Resource(**{k: json.loads(str(v["value"]).lower()) if v['type'] =='literal' and
-                                                                          ('datatype' in v and v['datatype']=='http://www.w3.org/2001/XMLSchema#boolean')
-                                                                       else (int(v["value"]) if v['type'] =='literal' and
-                                                                             ('datatype' in v and v['datatype']=='http://www.w3.org/2001/XMLSchema#integer')
-                                                                             else v["value"]
-                                                                             )
-                                for k, v in x.items()} )
+                    Resource(**{k: json.loads(str(v["value"]).lower()) if v['type'] == 'literal' and
+                                ('datatype' in v and v['datatype'] ==
+                                 'http://www.w3.org/2001/XMLSchema#boolean')
+                                else (int(v["value"]) if v['type'] == 'literal' and
+                                      ('datatype' in v and v['datatype'] ==
+                                       'http://www.w3.org/2001/XMLSchema#integer')
+                                      else v["value"]
+                                      )
+                                for k, v in x.items()})
                     for x in results
                 ]
 
-    def _elastic(self, query: str, limit: int, offset: int = None) -> List[Resource]:
+    def _elastic(self, query: str) -> List[Resource]:
         try:
             response = requests.post(
                 self.service.elastic_endpoint["endpoint"],
                 data=query,
                 headers=self.service.headers_elastic,
             )
             response.raise_for_status()
@@ -974,14 +1015,64 @@
                 deprecated_property=deprecated_property,
                 content_type=content_type,
                 accept=accept,
                 files_upload_config=files_upload_config,
                 files_download_config=files_download_config,
                 **params,
             )
+            
+    def rewrite_uri(self, uri: str, context: Context, **kwargs) -> str:
+        is_file = kwargs.get("is_file", True)
+        encoding = kwargs.get("encoding", None)
+
+        # try decoding the url first
+        raw_url = unquote(uri)
+        if is_file: # for files
+            url_base = '/'.join([self.endpoint, 'files', self.bucket])
+        else: # for resources
+            url_base = '/'.join([self.endpoint, 'resources', self.bucket])
+        matches = re.match(r"[\w\.:%/-]+/(\w+):(\w+)/[\w\.-/:%]+", raw_url)
+        if matches:
+            groups = matches.groups()
+            old_schema = f"{groups[0]}:{groups[1]}"
+            resolved = context.expand(groups[0])
+            if raw_url.startswith(url_base):
+                extended_schema = resolved + groups[1]
+                url = raw_url.replace(old_schema, quote_plus(extended_schema))
+                schema_and_id = url.split(url_base+"/")[1]
+                id = schema_and_id.split(quote_plus(extended_schema)+"/")[-1]
+                if not is_valid_url(id):        
+                    resolved_id = context.resolve_iri(id)
+                else:
+                    resolved_id = id
+                return url.replace(id, quote_plus(resolved_id))
+            else:
+                extended_schema = ''.join([resolved, groups[1]])
+                url = raw_url.replace(old_schema, extended_schema)
+        else:
+            url = raw_url
+        if url.startswith(url_base):
+            schema_and_id = url.split(url_base)[1]
+            if "/_/" in schema_and_id: # has _ schema
+                 id = schema_and_id.split("/_/")[-1]
+            else:
+                id = schema_and_id.split("/")[-1]
+            if not is_valid_url(id):
+                resolved_id = context.resolve_iri(id)
+            else:
+                resolved_id = id
+            if resolved_id in schema_and_id:
+                return uri # expanded already given
+            else:
+                return url.replace(id, quote_plus(resolved_id))
+        if not is_file and "/_/" not in url: # adding _ for empty schema
+            uri = "/".join((url_base, "_", quote_plus(url, encoding=encoding)))
+        else:
+            uri = "/".join((url_base, quote_plus(url, encoding=encoding)))
+        return uri
 
 
 def _error_message(error: HTTPError) -> str:
     def format_message(msg):
         return "".join([msg[0].lower(), msg[1:-1], msg[-1] if msg[-1] != "." else ""])
 
     try:
@@ -999,69 +1090,14 @@
         pass
     try:
         return format_message(error.response.text())
     except Exception:
         return format_message(str(error))
 
 
-def build_sparql_query_statements(context: Context, *conditions) -> Tuple[List, List]:
-    statements = list()
-    filters = list()
-    for index, f in enumerate(*conditions):
-        last_path = f.path[-1]
-        try:
-            last_term = context.terms[last_path]
-        except KeyError:
-            last_term = None
-        if last_path in ["id", "@id"]:
-            property_path = "/".join(f.path[:-1])
-        elif last_path == "@type":
-            minus_last_path = f.path[:-1]
-            minus_last_path.append("type")
-            property_path = "/".join(minus_last_path)
-        else:
-            property_path = "/".join(f.path)
-        try:
-            if (
-                last_path in ["type", "@type"]
-                or last_path in ["id", "@id"]
-                or (last_term is not None and last_term.type == "@id")
-            ):
-                if f.operator == "__eq__":
-                    statements.append(f"{property_path} {_box_value_as_full_iri(f.value)}")
-                elif f.operator == "__ne__":
-                    statements.append(f"{property_path} ?v{index}")
-                    filters.append(f"FILTER(?v{index} != {f.value})")
-                else:
-                    raise NotImplementedError(
-                        f"supported operators are '==' and '!=' when filtering by type or id."
-                    )
-            else:
-                parsed_type, parsed_value = _parse_type(f.value, parse_str=False)
-                value_type = type_map[parsed_type]
-                value = format_type[value_type](parsed_value if parsed_value else f.value)
-                if value_type is CategoryDataType.LITERAL:
-                    if f.operator not in ["__eq__", "__ne__"]:
-                        raise NotImplementedError(f"supported operators are '==' and '!=' when filtering with a str.")
-                    statements.append(f"{property_path} ?v{index}")
-                    filters.append(f"FILTER(?v{index} = {_box_value_as_full_iri(value)})")
-                else:
-                    statements.append(f"{property_path} ?v{index}")
-                    filters.append(
-                        f"FILTER(?v{index} {sparql_operator_map[f.operator]} {_box_value_as_full_iri(value)})"
-                    )
-        except NotImplementedError as nie:
-            raise ValueError(f"Operator '{sparql_operator_map[f.operator]}' is not supported with the value '{f.value}': {str(nie)}")
-    return statements, filters
-
-
-def _box_value_as_full_iri(value):
-    return f"<{value}>" if is_valid_url(value) else value
-
-
 def _create_select_query(vars_, statements, distinct, search_in_graph):
     where_clauses = (
         f"{{ Graph ?g {{{statements}}}}}" if search_in_graph else f"{{{statements}}}"
     )
     join_vars_ = ' '.join(vars_)
     select_vars = f"DISTINCT {join_vars_}" if distinct else f"{join_vars_}"
     return f"SELECT {select_vars} WHERE {where_clauses}"
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/stores/demo_store.py` & `nexusforge-0.8.1/kgforge/specializations/stores/demo_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,17 @@
     @staticmethod
     def _archive_id(rid: str, version: int) -> str:
         return f"{rid}_version={version}"
 
     @staticmethod
     def _tag_id(rid: str, tag: str) -> str:
         return f"{rid}_tag={tag}"
+    
+    def rewrite_ur(self, uri: str, context: Context, **kwargs) -> str:
+        raise not_supported()
 
     class RecordExists(Exception):
         pass
 
     class RecordMissing(Exception):
         pass
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/stores/nexus/__init__.py` & `nexusforge-0.8.1/kgforge/specializations/stores/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/stores/nexus/service.py` & `nexusforge-0.8.1/kgforge/specializations/stores/nexus/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from kgforge.core import Resource
 from kgforge.core.commons.actions import (
     Action,
     collect_lazy_actions,
     execute_lazy_actions,
     LazyAction,
 )
+from kgforge.core.commons.exceptions import ConfigurationError
 from kgforge.core.commons.context import Context
 from kgforge.core.conversions.rdf import (
     _from_jsonld_one,
     _remove_ld_keys,
     as_jsonld,
     recursive_resolve,
 )
@@ -90,15 +91,14 @@
         deprecated_property: bool,
         content_type: str,
         accept: str,
         files_upload_config: Dict,
         files_download_config: Dict,
         **params,
     ):
-
         nexus.config.set_environment(endpoint)
         self.endpoint = endpoint
         self.organisation = org
         self.project = prj
         self.model_context = model_context
         self.context_cache: Dict = dict()
         self.max_connection = max_connection
@@ -237,14 +237,16 @@
             nest_asyncio.apply()
         except RuntimeError:
             pass
 
     def get_project_context(self) -> Dict:
         project_data = nexus.projects.fetch(self.organisation, self.project)
         context = {"@base": project_data["base"], "@vocab": project_data["vocab"]}
+        for mapping in project_data['apiMappings']:
+            context[mapping['prefix']] = mapping['namespace']
         return context
 
     def resolve_context(self, iri: str, local_only: Optional[bool] = False) -> Dict:
         if iri in self.context_cache:
             return self.context_cache[iri]
         try:
             context_to_resolve = (
@@ -261,14 +263,17 @@
                 except URLError:
                     raise ValueError(f"{context_to_resolve} is not resolvable")
                 else:
                     document = context.document["@context"]
             else:
                 raise ValueError(f"{context_to_resolve} is not resolvable")
         else:
+            # Make sure context is not deprecated
+            if '_deprecated' in resource and resource['_deprecated']:
+                raise ConfigurationError(f"Context {context_to_resolve} exists but was deprecated")
             document = json.loads(json.dumps(resource["@context"]))
         if isinstance(document, list):
             if self.store_context in document:
                 document.remove(self.store_context)
             if self.store_local_context in document:
                 document.remove(self.store_local_context)
         self.context_cache.update({context_to_resolve: document})
```

### Comparing `nexusforge-0.8.0rc3/kgforge/specializations/stores/rdflib_graph.py` & `nexusforge-0.8.1/kgforge/specializations/stores/rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/nexusforge.egg-info/PKG-INFO` & `nexusforge-0.8.1/nexusforge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusforge
-Version: 0.8.0rc3
+Version: 0.8.1
 Summary: Building and Using Knowledge Graphs made easy.
 Home-page: https://github.com/BlueBrain/nexus-forge
 Author: Blue Brain Project, EPFL
 License: UNKNOWN
 Description: Blue Brain Nexus Forge
         ======================
         
@@ -97,12 +97,12 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: linking_sklearn
```

### Comparing `nexusforge-0.8.0rc3/nexusforge.egg-info/SOURCES.txt` & `nexusforge-0.8.1/nexusforge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 examples/notebooks/getting-started/02 - Datasets.ipynb
 examples/notebooks/getting-started/03 - Storing.ipynb
 examples/notebooks/getting-started/04 - Querying.ipynb
 examples/notebooks/getting-started/05 - Versioning.ipynb
 examples/notebooks/getting-started/06 - JSON IO.ipynb
 examples/notebooks/getting-started/07 - DataFrame IO.ipynb
 examples/notebooks/getting-started/08 - Formatting.ipynb
-examples/notebooks/getting-started/09 - Resolving-test.ipynb
 examples/notebooks/getting-started/09 - Resolving.ipynb
 examples/notebooks/getting-started/10 - Reshaping.ipynb
 examples/notebooks/getting-started/11 - Modeling.ipynb
 examples/notebooks/getting-started/12 - Mapping.ipynb
 examples/notebooks/getting-started/13 - JSON-LD IO.ipynb
 examples/notebooks/getting-started/14 - RDF IO.ipynb
 examples/notebooks/getting-started/15 - SQL IO.ipynb
@@ -118,17 +117,19 @@
 kgforge/core/commons/attributes.py
 kgforge/core/commons/context.py
 kgforge/core/commons/dictionaries.py
 kgforge/core/commons/es_query_builder.py
 kgforge/core/commons/exceptions.py
 kgforge/core/commons/execution.py
 kgforge/core/commons/files.py
+kgforge/core/commons/formatter.py
 kgforge/core/commons/imports.py
 kgforge/core/commons/parser.py
 kgforge/core/commons/query_builder.py
+kgforge/core/commons/sparql_query_builder.py
 kgforge/core/commons/strategies.py
 kgforge/core/conversions/__init__.py
 kgforge/core/conversions/dataframe.py
 kgforge/core/conversions/json.py
 kgforge/core/conversions/rdf.py
 kgforge/core/wrappings/__init__.py
 kgforge/core/wrappings/dict.py
@@ -219,14 +220,14 @@
 tests/specializations/mappers/test_mappers.py
 tests/specializations/mappings/test_mappings.py
 tests/specializations/models/data.py
 tests/specializations/models/demo_model.feature
 tests/specializations/models/test_demo_model.py
 tests/specializations/models/test_models.py
 tests/specializations/models/test_rdf_model.py
-tests/specializations/resolvers/test_resolvers.py
+tests/specializations/resolvers/test_resolver.py
 tests/specializations/resources/test_datasets.py
 tests/specializations/resources/test_resources.py
 tests/specializations/stores/demo_store.feature
 tests/specializations/stores/test_bluebrain_nexus.py
 tests/specializations/stores/test_demo_store.py
 tests/specializations/stores/test_stores.py
```

### Comparing `nexusforge-0.8.0rc3/setup.py` & `nexusforge-0.8.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,44 +31,42 @@
     },
     description="Building and Using Knowledge Graphs made easy.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     keywords="framework knowledge graph data science",
     url="https://github.com/BlueBrain/nexus-forge",
     packages=find_packages(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     setup_requires=[
         "setuptools_scm",
     ],
     install_requires=[
         "hjson",
         "pyyaml",
         "pandas",
         "nexus-sdk",
         "aiohttp",
-        "nest_asyncio",
-        "rdflib>=6.0.0",
+        "rdflib==6.2.0",
         "pyLD",
         "pyshacl==v0.17.2",
         "nest-asyncio>=1.5.1",
         "pyparsing>=2.0.2",
         "owlrl>=5.2.3",
         "elasticsearch_dsl==7.4.0"
     ],
     extras_require={
         "dev": [
             "tox",
             "pytest",
             "pytest-bdd==3.4.0",
             "pytest-cov",
             "pytest-mock",
-            "codecov",
         ],
         "docs": ["sphinx", "sphinx-bluebrain-theme"],
-        "linking_sklearn": ["sklearn"],
+        "linking_sklearn": ["scikit-learn"],
     },
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `nexusforge-0.8.0rc3/tests/__init__.py` & `nexusforge-0.8.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/conftest.py` & `nexusforge-0.8.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,19 @@
             "Person": "foaf:Person",
             "name": "foaf:name",
         }
     }
 
 
 @pytest.fixture
+def bbn_deprecated_property() -> str:
+    return "https://bluebrain.github.io/nexus/vocabulary/deprecated"
+
+
+@pytest.fixture
 def metadata_context() -> Context:
     document = {
         "deprecated": "https://store.net/vocabulary/deprecated",
         "version": "https://store.net/vocabulary/version",
     }
     return Context(document, "http://store.org/metadata.json")
 
@@ -432,14 +437,24 @@
                     "resolver": resolver,
                     "origin": "directory",
                     "source": "tests/data/demo-resolver/",
                     "targets": [
                         {
                             "identifier": "sex",
                             "bucket": "sex.json",
+                            "filters":[
+                                {
+                                "path": "type",
+                                "value": "class"
+                                },
+                                {
+                                "path": "label",
+                                "value": "female"
+                                }
+                            ]
                         },
                     ],
                     "result_resource_mapping": "../../configurations/demo-resolver/term-to-resource-mapping.hjson",
                 },
             ],
         },
     }
```

### Comparing `nexusforge-0.8.0rc3/tests/core/archetypes/test_store.py` & `nexusforge-0.8.1/tests/core/archetypes/test_store.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/commons/test_actions.py` & `nexusforge-0.8.1/tests/core/commons/test_actions.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/commons/test_attributes.py` & `nexusforge-0.8.1/tests/core/commons/test_attributes.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/commons/test_context.py` & `nexusforge-0.8.1/tests/core/commons/test_context.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/commons/test_dictionaries.py` & `nexusforge-0.8.1/tests/core/commons/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/commons/test_es_query_builder.py` & `nexusforge-0.8.1/tests/core/commons/test_es_query_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,14 +631,41 @@
                                 ),
                             ).to_dict()
                         ],
                     )
                 ),
                 id="rewrite_type_id",
             ),
+            pytest.param(
+                (
+                    [
+                        Filter(
+                            operator="__eq__",
+                            path=["brainLocation", "brainRegion", "label"],
+                            value=["A label", "Another label"],
+                        )
+                    ]
+                ),
+                ({}),
+                (
+                    elasticsearch_dsl.Search()
+                    .query(
+                        elasticsearch_dsl.query.Bool(
+                            filter=[
+                                elasticsearch_dsl.query.Terms(
+                                    **{
+                                        "brainLocation.brainRegion.label.keyword": ["A label", "Another label"]
+                                    }
+                                )
+                            ]
+                        )
+                    )
+                ),
+                id="build_query_with_multiple_values",
+            )
         ],
     )
     def test_build(self, filters, params, es_query, es_mapping_dict):
         es_mapping = elasticsearch_dsl.Mapping()
         es_mapping._update_from_dict(es_mapping_dict)
         query = ESQueryBuilder.build(es_mapping_dict, None, None, filters, **params)
         assert isinstance(query, dict)
```

### Comparing `nexusforge-0.8.0rc3/tests/core/commons/test_execution.py` & `nexusforge-0.8.1/tests/core/commons/test_execution.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/conversions/conftest.py` & `nexusforge-0.8.1/tests/core/conversions/conftest.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/conversions/test_dataframe.py` & `nexusforge-0.8.1/tests/core/conversions/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/conversions/test_json.py` & `nexusforge-0.8.1/tests/core/conversions/test_json.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/conversions/test_rdf.py` & `nexusforge-0.8.1/tests/core/conversions/test_rdf.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/resource.feature` & `nexusforge-0.8.1/tests/core/resource.feature`

 * *Files 7% similar despite different names*

```diff
@@ -15,8 +15,12 @@
 
   Scenario: Create and update a resource.
     Given I create a resource with a property.
     Then I assigned _synchronized to True so the resource should give _inner_sync equals True.
 
   Scenario: Create and update a nested resource.
     Given I create a resource with an other resource as property.
-    Then I changed a nested property so the resource should give _synchronized equals False.
+    Then I changed a nested property so the resource should give _synchronized equals False.
+  
+  Scenario: Create a resource with id and type.
+    Given I create a resource with an id and type.
+    Then I should be able to get its type and identifier.
```

### Comparing `nexusforge-0.8.0rc3/tests/core/test_forge.py` & `nexusforge-0.8.1/tests/core/test_forge.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,11 +45,11 @@
 
     def test_resolver_does_not_return_if_print(self, config):
         forge = KnowledgeGraphForge(config)
         resolvers_dict = forge.resolvers(output="print")
         assert resolvers_dict is None
 
     def test_resolver_returns_correct_dictionary(self, config):
-        dict_result = {'terms': {'sex': {'bucket': 'sex.json'}}}
+        dict_result = {'terms': {'sex': {'bucket': 'sex.json', 'filters':{'label': 'female', 'type': 'class'}}}}
         forge = KnowledgeGraphForge(config)
         resolvers_dict = forge.resolvers(output="dict")
         assert resolvers_dict == dict_result
```

### Comparing `nexusforge-0.8.0rc3/tests/core/test_reshaping.py` & `nexusforge-0.8.1/tests/core/test_reshaping.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/test_resolving.py` & `nexusforge-0.8.1/tests/core/test_resolving.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/test_resource.py` & `nexusforge-0.8.1/tests/core/test_resource.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,15 +42,20 @@
 @given("I create a resource from a JSON dict and exclude fields.")
 def resource_from_json_na_many(json_one):
     return Resource.from_json(json_one, na=["v1a","v2a"])
 
 
 @given("I create a resource with an other resource as property.")
 def nresource():
-    return Resource(type="Entity", contribution=Resource(type="Contribution"))
+    return Resource(type="Entity", contribution=Resource(type="Contribution"),
+                    used=[Resource(type="Entity"), Resource(type="Dataset")])
+
+@given("I create a resource with an id and type.")
+def resource_id_type():
+    return Resource(id="https://id", type="Person", name="name")
 
 
 @when("I create a resource with a reserved attribute. Creation should fail.")
 def reserved_attribute_error():
     with pytest.raises(NotImplementedError):
         Resource(_validated=True)
 
@@ -66,24 +71,56 @@
     assert list(encode(resource_from_json_na_many).values()) == ["123","Type"]
 
 
 @then("I should be able to access the nested resource properties as JSONPath.")
 def access_nested_property(nresource):
     assert nresource.type == "Entity"
     assert nresource.contribution.type == "Contribution"
+    assert nresource.used[0].type == "Entity"
+    assert nresource.used[1].type == "Dataset"
 
 
 @then("I assigned _synchronized to True so the resource should give _inner_sync equals True.")
 def change_property(resource):
     resource._synchronized = True
     assert resource._inner_sync == True
     resource.type = "test"
     assert resource._synchronized == False
 
 
 @then("I changed a nested property so the resource should give _synchronized equals False.")
 def change_nested_property(nresource):
     nresource._synchronized = True 
     assert nresource._inner_sync == True
+    # Change some property
     nresource.contribution.type = "test"
     assert nresource._synchronized == False
-    assert nresource._inner_sync == False
+    assert nresource._inner_sync == False
+    # Synchronize again
+    nresource._synchronized = True 
+    assert nresource._inner_sync == True
+    # Change a list
+    for u in nresource.used:
+        u.value = 10
+    assert nresource._synchronized == False
+    assert nresource._inner_sync == False
+
+@then("I should be able to get its type and identifier.")
+def change_nested_property(resource_id_type):
+    assert resource_id_type.has_identifier(return_attribute=True) == (True, "id")
+    assert resource_id_type.has_identifier() is True
+    assert resource_id_type.has_type(return_attribute=True) == (True, "type")
+    assert resource_id_type.has_type() is True
+    
+    assert resource_id_type.get_identifier() == "https://id"
+    assert resource_id_type.get_type() == "Person"
+
+    resource_no_id_no_type = Resource(name="name")
+    assert resource_no_id_no_type.has_identifier(return_attribute=True) == (False, None)
+    assert resource_no_id_no_type.has_identifier() is False
+    assert resource_no_id_no_type.has_type(return_attribute=True) == (False, None)
+    assert resource_no_id_no_type.has_type() is False
+    
+    assert resource_no_id_no_type.get_identifier() is None
+    assert resource_no_id_no_type.get_type() is None
+
+
```

### Comparing `nexusforge-0.8.0rc3/tests/core/wrappings/test_dict.py` & `nexusforge-0.8.1/tests/core/wrappings/test_dict.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/core/wrappings/test_paths.py` & `nexusforge-0.8.1/tests/core/wrappings/test_paths.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/NeuronMorphology.hjson` & `nexusforge-0.8.1/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/NeuronMorphology.hjson`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/PatchedCell.hjson` & `nexusforge-0.8.1/tests/data/demo-model/mappings/allen-cell-types-database/DictionaryMapping/PatchedCell.hjson`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/demo-model/vocabulary.json` & `nexusforge-0.8.1/tests/data/demo-model/vocabulary.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/demo-resolver/cell_types.json` & `nexusforge-0.8.1/tests/data/demo-resolver/cell_types.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/demo-resolver/structure_layer.json` & `nexusforge-0.8.1/tests/data/demo-resolver/structure_layer.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/shacl-model/commons/shapes-1.json` & `nexusforge-0.8.1/tests/data/shacl-model/commons/shapes-1.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/shacl-model/commons/shapes-2.json` & `nexusforge-0.8.1/tests/data/shacl-model/commons/shapes-2.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/shacl-model/commons/shapes-3.json` & `nexusforge-0.8.1/tests/data/shacl-model/commons/shapes-3.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/data/shacl-model/context.json` & `nexusforge-0.8.1/tests/data/shacl-model/context.json`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/mappers/test_mappers.py` & `nexusforge-0.8.1/tests/specializations/mappers/test_mappers.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/mappings/test_mappings.py` & `nexusforge-0.8.1/tests/specializations/mappings/test_mappings.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/models/data.py` & `nexusforge-0.8.1/tests/specializations/models/data.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/models/demo_model.feature` & `nexusforge-0.8.1/tests/specializations/models/demo_model.feature`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/models/test_demo_model.py` & `nexusforge-0.8.1/tests/specializations/models/test_demo_model.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/models/test_models.py` & `nexusforge-0.8.1/tests/specializations/models/test_models.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/models/test_rdf_model.py` & `nexusforge-0.8.1/tests/specializations/models/test_rdf_model.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/resolvers/test_resolvers.py` & `nexusforge-0.8.1/tests/specializations/resources/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
 
-# Placeholder for the generic parameterizable test suite for resolvers.
+# Placeholder for the generic parameterizable test suite for resources.
```

### Comparing `nexusforge-0.8.0rc3/tests/specializations/resources/test_datasets.py` & `nexusforge-0.8.1/tests/specializations/resources/test_datasets.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/resources/test_resources.py` & `nexusforge-0.8.1/kgforge/core/commons/formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,8 +8,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 # General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with Blue Brain Nexus Forge. If not, see <https://choosealicense.com/licenses/lgpl-3.0/>.
 
-# Placeholder for the generic parameterizable test suite for resources.
+from enum import Enum, auto
+
+
+class Formatter(Enum):
+    # format using str.format(*args, **kwargs).
+    STR = auto()
+    # URI rewriter.
+    URI_REWRITER = auto()
+
```

### Comparing `nexusforge-0.8.0rc3/tests/specializations/stores/demo_store.feature` & `nexusforge-0.8.1/tests/specializations/stores/demo_store.feature`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/stores/test_bluebrain_nexus.py` & `nexusforge-0.8.1/tests/specializations/stores/test_bluebrain_nexus.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,36 +18,37 @@
 from urllib.parse import urljoin
 from urllib.request import pathname2url
 from uuid import uuid4
 
 import nexussdk
 import pytest
 from typing import Callable, Union, List
+from collections import OrderedDict
 
 from kgforge.core import Resource
 from kgforge.core.archetypes import Store
 from kgforge.core.commons.context import Context
 from kgforge.core.conversions.rdf import _merge_jsonld
 from kgforge.core.wrappings.dict import wrap_dict
 from kgforge.core.wrappings.paths import Filter, create_filters_from_dict
+from kgforge.core.commons.sparql_query_builder import SPARQLQueryBuilder
 from kgforge.specializations.stores.bluebrain_nexus import (
     BlueBrainNexus,
-    build_sparql_query_statements,
     _create_select_query,
 )
 
 # FIXME mock Nexus for unittests
 # TODO To be port to the generic parameterizable test suite for stores in test_stores.py. DKE-135.
 from kgforge.specializations.stores.nexus import Service
 
 BUCKET = "test/kgforge"
-NEXUS = "https://nexus-instance.org/"
+NEXUS = "https://nexus-instance.org"
 TOKEN = "token"
-NEXUS_PROJECT_CONTEXT = {"base": "http://data.net/", "vocab": "http://vocab.net/"}
-
+NEXUS_PROJECT_CONTEXT = {"base": "http://data.net", "vocab": "http://vocab.net",
+                         "apiMappings": [{'namespace': 'https://neuroshapes.org/dash/', 'prefix': 'datashapes'}]}
 VERSIONED_TEMPLATE = "{x.id}?rev={x._store_metadata._rev}"
 FILE_RESOURCE_MAPPING = os.sep.join(
     (os.path.curdir, "tests", "data", "nexus-store", "file-to-resource-mapping.hjson")
 )
 
 
 @pytest.fixture
@@ -126,14 +127,24 @@
 
 
 @pytest.fixture
 def nexus_store_unauthorized():
     return BlueBrainNexus(endpoint=NEXUS, bucket=BUCKET, token="invalid token")
 
 
+@pytest.fixture
+def nexus_context():
+    context_document = dict()
+    context_document["@base"] = NEXUS_PROJECT_CONTEXT["base"]
+    context_document["@vocab"] = NEXUS_PROJECT_CONTEXT["vocab"]
+    for mapping in NEXUS_PROJECT_CONTEXT['apiMappings']:
+        context_document[mapping['prefix']] = mapping['namespace']
+    return Context(context_document)
+
+
 def test_config_error():
     with pytest.raises(ValueError):
         BlueBrainNexus(endpoint="test", bucket="invalid", token="")
 
 
 def test_config(nexus_store):
     assert nexus_store.organisation == "test"
@@ -161,14 +172,73 @@
     payload["@context"] = context
     result = nexus_store.service.to_resource(payload)
     assert str(result) == str(registered_building)
     assert getattr(result, "context") == registered_building.context
     assert str(result._store_metadata) == str(registered_building._store_metadata)
 
 
+@pytest.mark.parametrize("url,is_file, expected",
+                         [
+                            pytest.param(       
+                                ("myverycoolid123456789"),
+                                (True),
+                                ("https://nexus-instance.org/files/test/kgforge/myverycoolid123456789"),
+                                id="simple-file-id",
+                            ),
+                            pytest.param(       
+                                ("http://data.net/myverycoolid123456789"),
+                                (False),
+                                ("https://nexus-instance.org/resources/test/kgforge/_/http%3A%2F%2Fdata.net%2Fmyverycoolid123456789"),
+                                id="simple-resource-id",
+                            ),
+                            pytest.param(
+                                ("http://data.net/07ed2dab-587a-4144-90c7-4cdd252cfa3f"),
+                                (True),
+                                ("https://nexus-instance.org/files/test/kgforge/http%3A%2F%2Fdata.net%2F07ed2dab-587a-4144-90c7-4cdd252cfa3f"),
+                                id="file-id",
+                            ),
+                            pytest.param(
+                                ("https://nexus-instance.org/files/test/kgforge/myverycoolid123456789"),
+                                (True),
+                                ("https://nexus-instance.org/files/test/kgforge/http%3A%2F%2Fdata.net%2Fmyverycoolid123456789"),
+                                id="file-self",
+                            )
+                            ,
+                            pytest.param(
+                                ("https://nexus-instance.org/resources/test/kgforge/datashapes:example/43edd8bf-5dfe-45cd-b6d8-1a604dd6beca"),
+                                (False),
+                                ("https://nexus-instance.org/resources/test/kgforge/https%3A%2F%2Fneuroshapes.org%2Fdash%2Fexample/http%3A%2F%2Fdata.net%2F43edd8bf-5dfe-45cd-b6d8-1a604dd6beca"),
+                                id="resource-schema-self",
+                            ),
+                            pytest.param(
+                                ("https://nexus-instance.org/resources/test/kgforge/_/43edd8bf-5dfe-45cd-b6d8-1a604dd6beca"),
+                                (False),
+                                ("https://nexus-instance.org/resources/test/kgforge/_/http%3A%2F%2Fdata.net%2F43edd8bf-5dfe-45cd-b6d8-1a604dd6beca"),
+                                id="resource-empty-schema-self",
+                            ),
+                            pytest.param(
+                                ("https://nexus-instance.org/files/test/kgforge/http%3A%2F%2Fdata.net%2F632a7644-b07e-4fcd-a537-9162e3444106"),
+                                (True),
+                                ("https://nexus-instance.org/files/test/kgforge/http%3A%2F%2Fdata.net%2F632a7644-b07e-4fcd-a537-9162e3444106"),
+                                id="file-given-expanded-url-encoded-self",
+                            ),
+                            pytest.param(
+                                ("https://nexus-instance.org/resources/test/kgforge/_/http%3A%2F%2Fdata.net%2F43edd8bf-5dfe-45cd-b6d8-1a604dd6beca"),
+                                (False),
+                                ("https://nexus-instance.org/resources/test/kgforge/_/http%3A%2F%2Fdata.net%2F43edd8bf-5dfe-45cd-b6d8-1a604dd6beca"),
+                                id="resource-empty-schema-url-encoded-self",
+                            )
+                            
+                            
+                         ])
+def test_rewrite_uri(nexus_store, nexus_context, url, is_file, expected):
+    uri = nexus_store.rewrite_uri(url, context=nexus_context, is_file=is_file, encoding=None)
+    assert expected == uri
+
+
 class TestQuerying:
     @pytest.fixture
     def context(self):
         document = {
             "@context": {
                 "@vocab": "http://example.org/vocab/",
                 "contribution": {
@@ -295,29 +365,29 @@
                     ["FILTER(?v0 != Person)"],
                 ),
                 id="filter-by-id",
             ),
         ],
     )
     def test_filter_to_query_statements(self, context, filters, expected):
-        statements = build_sparql_query_statements(context, filters)
+        statements = SPARQLQueryBuilder.build(None, None, context, *list(filters))
         assert statements == expected
 
     @pytest.mark.parametrize(
         "filters",
         [
             pytest.param(
                 (Filter(["agent", "name"], "__le__", "Allen Institute"),),
                 id="range_query_str",
             )
         ]
     )
     def test_filter_to_query_statements_exceptions(self, context, filters):
         with pytest.raises(ValueError):
-            build_sparql_query_statements(context, filters)
+            SPARQLQueryBuilder.build(None, None, context, *list(filters))
 
     def test_create_select_query(self):
         statements = f"?id type <https://github.com/BlueBrain/nexus-forge>"
         vars_ = ["?id", "?project"]
         query = _create_select_query(vars_, statements, distinct=False, search_in_graph=True)
         assert (
             query
@@ -410,14 +480,33 @@
                             path=["affiliation", "id"],
                             value="https://www.grid.ac/institutes/grid.5333.6",
                         ),
                     ]
                 ),
                 id="json_filter_id",
             ),
+            pytest.param(
+                (
+                    {
+                        "type": "Person",
+                        "affiliation/id":"https://www.grid.ac/institutes/grid.5333.6"
+                    }
+                ),
+                (
+                    [
+                        Filter(operator="__eq__", path=["type"], value="Person"),
+                        Filter(
+                            operator="__eq__",
+                            path=["affiliation", "id"],
+                            value="https://www.grid.ac/institutes/grid.5333.6",
+                        )
+                    ]
+                ),
+                id="json_key_sequence_path",
+            )
         ],
     )
     def test_dict_to_filters(self, filters, expected):
         filters_from_dict = create_filters_from_dict(filters)
         assert filters_from_dict == expected
```

### Comparing `nexusforge-0.8.0rc3/tests/specializations/stores/test_demo_store.py` & `nexusforge-0.8.1/tests/specializations/stores/test_demo_store.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tests/specializations/stores/test_stores.py` & `nexusforge-0.8.1/tests/specializations/stores/test_stores.py`

 * *Files identical despite different names*

### Comparing `nexusforge-0.8.0rc3/tox.ini` & `nexusforge-0.8.1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
     pytest
     pytest-bdd
     pytest-mock
 
 [tox]
 envlist =
     lint
-    py{37,38}
+    py{38,39}
 
 indexserver =
     default = https://bbpteam.epfl.ch/repository/devpi/simple
 
 [testenv]
 deps = {[base]testdeps}
 commands = pytest tests
 
 [testenv:lint]
-basepython=python3.6
+basepython=python3.8
 deps =
     pycodestyle
     pylint
 commands =
     pycodestyle {[base]name}
     pylint -j2 {[base]name}
 
@@ -40,8 +40,8 @@
 whitelist_externals = make
 
 # E731: do not assign a lambda expression, use a def
 # W503: line break after binary operator
 # W504: line break before binary operator
 [pycodestyle]
 ignore = E731,W503,W504
-max-line-length = 100
+max-line-length = 200
```

