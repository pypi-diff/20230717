# Comparing `tmp/pre-commit-vauxoo-7.0.8.tar.gz` & `tmp/pre-commit-vauxoo-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre-commit-vauxoo-7.0.8.tar", last modified: Thu Nov 10 22:47:59 2022, max compression
+gzip compressed data, was "pre-commit-vauxoo-7.0.9.tar", last modified: Tue Nov 15 16:56:34 2022, max compression
```

## Comparing `pre-commit-vauxoo-7.0.8.tar` & `pre-commit-vauxoo-7.0.9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.502646 pre-commit-vauxoo-7.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.482646 pre-commit-vauxoo-7.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     7354 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/.github/workflows/github-actions.yml
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-10 22:47:59.000000 pre-commit-vauxoo-7.0.8/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)    43711 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6879 2022-11-10 22:47:59.502646 pre-commit-vauxoo-7.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7371 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/ci/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3102 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/ci/templates/.appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.482646 pre-commit-vauxoo-7.0.8/ci/templates/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/ci/templates/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/ci/templates/.github/workflows/github-actions.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/ci/templates/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/ci/templates/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.482646 pre-commit-vauxoo-7.0.8/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/resources/module_autofix1/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/__manifest__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/resources/module_autofix1/demo/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/demo/demo.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.490646 pre-commit-vauxoo-7.0.8/resources/module_autofix1/models/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_autofix1/security/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/security/ir.model.access.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_autofix1/views/
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_autofix1/views/views.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_example1/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/__manifest__.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/deactivate.jinja
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_example1/demo/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/demo/demo.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_example1/models/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_example1/security/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/security/ir.model.access.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_example1/views/
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_example1/views/views.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_uninstallable/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_uninstallable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_uninstallable/__manifest__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_uninstallable/models/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_uninstallable/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_uninstallable/models/non_install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_warnings1/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/__manifest__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_warnings1/demo/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/demo/demo.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_warnings1/models/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_warnings1/security/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/security/ir.model.access.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.494646 pre-commit-vauxoo-7.0.8/resources/module_warnings1/views/
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/resources/module_warnings1/views/views.xml
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-11-10 22:47:59.502646 pre-commit-vauxoo-7.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3654 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.486646 pre-commit-vauxoo-7.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.498646 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.502646 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.bandit
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)     7117 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.eslintrc.json
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.flake8-optional
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pre-commit-config-autofix.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pre-commit-config-optional.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (121)    22592 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pylintrc-optional
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/doc8.ini
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     9559 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      558 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/git_hook_pre_commit
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.502646 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/hooks/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3080 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/hooks/check_deactivate_jinja.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/logging_colored.py
--rw-r--r--   0 runner    (1001) docker     (121)    15492 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/pre_commit_vauxoo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.498646 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6879 2022-11-10 22:47:59.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-11-10 22:47:59.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 22:47:59.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-10 22:47:59.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 22:45:34.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-10 22:47:59.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-10 22:47:59.000000 pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 22:47:59.502646 pre-commit-vauxoo-7.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     8127 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/tests/test_pre_commit_vauxoo.py
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/tox.ini
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-11-10 22:44:48.000000 pre-commit-vauxoo-7.0.8/variables.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.828852 pre-commit-vauxoo-7.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.804852 pre-commit-vauxoo-7.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     7354 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/.github/workflows/github-actions.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-15 16:56:34.000000 pre-commit-vauxoo-7.0.9/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (121)    43711 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6879 2022-11-15 16:56:34.828852 pre-commit-vauxoo-7.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7371 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3102 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/ci/templates/.appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.804852 pre-commit-vauxoo-7.0.9/ci/templates/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/ci/templates/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/ci/templates/.github/workflows/github-actions.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/ci/templates/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/ci/templates/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.808852 pre-commit-vauxoo-7.0.9/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/resources/module_autofix1/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/__manifest__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/resources/module_autofix1/demo/
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/demo/demo.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/resources/module_autofix1/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.812852 pre-commit-vauxoo-7.0.9/resources/module_autofix1/security/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/security/ir.model.access.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_autofix1/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_autofix1/views/views.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_example1/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/__manifest__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/deactivate.jinja
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_example1/demo/
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/demo/demo.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_example1/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_example1/security/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/security/ir.model.access.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_example1/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_example1/views/views.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_uninstallable/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_uninstallable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_uninstallable/__manifest__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_uninstallable/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_uninstallable/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_uninstallable/models/non_install.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_warnings1/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/__manifest__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_warnings1/demo/
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/demo/demo.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_warnings1/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_warnings1/security/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/security/ir.model.access.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.816852 pre-commit-vauxoo-7.0.9/resources/module_warnings1/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/resources/module_warnings1/views/views.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-11-15 16:56:34.828852 pre-commit-vauxoo-7.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3654 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.808852 pre-commit-vauxoo-7.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.820852 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.824852 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.bandit
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)     7117 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.flake8
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.flake8-optional
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pre-commit-config-autofix.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pre-commit-config-optional.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    22592 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pylintrc-optional
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/doc8.ini
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     9559 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      558 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/git_hook_pre_commit
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.828852 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/hooks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/hooks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3080 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/hooks/check_deactivate_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/logging_colored.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15492 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/pre_commit_vauxoo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.820852 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6879 2022-11-15 16:56:34.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-11-15 16:56:34.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 16:56:34.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-15 16:56:34.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 16:53:09.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 16:56:34.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-15 16:56:34.000000 pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 16:56:34.828852 pre-commit-vauxoo-7.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     8127 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/tests/test_pre_commit_vauxoo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-11-15 16:52:07.000000 pre-commit-vauxoo-7.0.9/variables.sh
```

### Comparing `pre-commit-vauxoo-7.0.8/.appveyor.yml` & `pre-commit-vauxoo-7.0.9/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/.bumpversion.cfg` & `pre-commit-vauxoo-7.0.9/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 7.0.8
+current_version = 7.0.9
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pre-commit-vauxoo-7.0.8/.cookiecutterrc` & `pre-commit-vauxoo-7.0.9/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/.github/workflows/github-actions.yml` & `pre-commit-vauxoo-7.0.9/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/.travis.yml` & `pre-commit-vauxoo-7.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/CONTRIBUTING.rst` & `pre-commit-vauxoo-7.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/LICENSE` & `pre-commit-vauxoo-7.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/PKG-INFO` & `pre-commit-vauxoo-7.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit-vauxoo
-Version: 7.0.8
+Version: 7.0.9
 Summary: pre-commit script to run automatically the configuration and variables custom from Vauxoo
 Home-page: https://github.com/Vauxoo/pre-commit-vauxoo
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://pre-commit-vauxoo.readthedocs.io/
 Project-URL: Changelog, https://pre-commit-vauxoo.readthedocs.io/en/latest/changelog.html
```

### Comparing `pre-commit-vauxoo-7.0.8/README.rst` & `pre-commit-vauxoo-7.0.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     :alt: PyPI Wheel
     :target: https://pypi.org/project/pre-commit-vauxoo
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pre-commit-vauxoo.svg
     :alt: Supported versions
     :target: https://pypi.org/project/pre-commit-vauxoo
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/Vauxoo/pre-commit-vauxoo/v7.0.8.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/Vauxoo/pre-commit-vauxoo/v7.0.9.svg
     :alt: Commits since latest release
-    :target: https://github.com/Vauxoo/pre-commit-vauxoo/compare/v7.0.8...main
+    :target: https://github.com/Vauxoo/pre-commit-vauxoo/compare/v7.0.9...main
 
 
 
 .. end-badges
 
 pre-commit script to run automatically the configuration and variables custom from Vauxoo
```

### Comparing `pre-commit-vauxoo-7.0.8/ci/bootstrap.py` & `pre-commit-vauxoo-7.0.9/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/ci/templates/.appveyor.yml` & `pre-commit-vauxoo-7.0.9/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/ci/templates/.github/workflows/github-actions.yml` & `pre-commit-vauxoo-7.0.9/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/ci/templates/.travis.yml` & `pre-commit-vauxoo-7.0.9/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/ci/templates/tox.ini` & `pre-commit-vauxoo-7.0.9/ci/templates/tox.ini`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/docs/conf.py` & `pre-commit-vauxoo-7.0.9/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "pre-commit-vauxoo"
 year = "2022"
 author = "Vauxoo"
 copyright = "{}, {}".format(year, author)
-version = release = "7.0.8"
+version = release = "7.0.9"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/Vauxoo/pre-commit-vauxoo/issues/%s", "#"),
     "pr": ("https://github.com/Vauxoo/pre-commit-vauxoo/pull/%s", "PR #"),
 }
```

### Comparing `pre-commit-vauxoo-7.0.8/pytest.ini` & `pre-commit-vauxoo-7.0.9/pytest.ini`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/resources/module_autofix1/__manifest__.py` & `pre-commit-vauxoo-7.0.9/resources/module_autofix1/__manifest__.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/resources/module_autofix1/views/views.xml` & `pre-commit-vauxoo-7.0.9/resources/module_autofix1/views/views.xml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/resources/module_example1/__manifest__.py` & `pre-commit-vauxoo-7.0.9/resources/module_example1/__manifest__.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/resources/module_example1/views/views.xml` & `pre-commit-vauxoo-7.0.9/resources/module_example1/views/views.xml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/resources/module_warnings1/__manifest__.py` & `pre-commit-vauxoo-7.0.9/resources/module_warnings1/__manifest__.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/resources/module_warnings1/views/views.xml` & `pre-commit-vauxoo-7.0.9/resources/module_warnings1/views/views.xml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/setup.cfg` & `pre-commit-vauxoo-7.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/setup.py` & `pre-commit-vauxoo-7.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="pre-commit-vauxoo",
-    version="7.0.8",
+    version="7.0.9",
     license="LGPL-3.0-or-later",
     description="pre-commit script to run automatically the configuration and variables custom from Vauxoo",
     long_description_content_type="text/x-rst",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", generate_changelog()),
     ),
```

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.editorconfig` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.editorconfig`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.eslintrc.json` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.flake8` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.flake8`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.flake8-optional` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.flake8-optional`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pre-commit-config-autofix.yaml` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pre-commit-config-autofix.yaml`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pre-commit-config-optional.yaml` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pre-commit-config-optional.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       - id: oca-checks-odoo-module
       - id: oca-checks-po
   - repo: https://github.com/PyCQA/doc8
     rev: v1.0.0
     hooks:
       - id: doc8
         name: RST lint
-  - repo: https://gitlab.com/PyCQA/flake8
+  - repo: https://github.com/PyCQA/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         name: flake8 + bugbear optional checks
         additional_dependencies: ["flake8-bugbear==22.7.1"]
         args:
           - --config=.flake8-optional
```

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pre-commit-config.yaml` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # External scripts
     (scripts/)
   )
 default_language_version:
   python: python3
   node: "14.13.0"
 repos:
-  - repo: https://gitlab.com/PyCQA/flake8
+  - repo: https://github.com/PyCQA/flake8
     rev: 4.0.1
     hooks:
       - id: flake8
         name: flake8 mandatory checks
   - repo: https://github.com/OCA/pylint-odoo
     rev: v8.0.16
     hooks:
```

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pylintrc` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pylintrc`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cfg/.pylintrc-optional` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cfg/.pylintrc-optional`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/cli.py` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/cli.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/git_hook_pre_commit` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/git_hook_pre_commit`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/hooks/check_deactivate_jinja.py` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/hooks/check_deactivate_jinja.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/logging_colored.py` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/logging_colored.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo/pre_commit_vauxoo.py` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo/pre_commit_vauxoo.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/PKG-INFO` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit-vauxoo
-Version: 7.0.8
+Version: 7.0.9
 Summary: pre-commit script to run automatically the configuration and variables custom from Vauxoo
 Home-page: https://github.com/Vauxoo/pre-commit-vauxoo
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://pre-commit-vauxoo.readthedocs.io/
 Project-URL: Changelog, https://pre-commit-vauxoo.readthedocs.io/en/latest/changelog.html
```

### Comparing `pre-commit-vauxoo-7.0.8/src/pre_commit_vauxoo.egg-info/SOURCES.txt` & `pre-commit-vauxoo-7.0.9/src/pre_commit_vauxoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/tests/test_pre_commit_vauxoo.py` & `pre-commit-vauxoo-7.0.9/tests/test_pre_commit_vauxoo.py`

 * *Files identical despite different names*

### Comparing `pre-commit-vauxoo-7.0.8/tox.ini` & `pre-commit-vauxoo-7.0.9/tox.ini`

 * *Files identical despite different names*

