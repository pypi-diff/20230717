# Comparing `tmp/gitprprod-0.0.3.tar.gz` & `tmp/gitprprod-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitprprod-0.0.3.tar", last modified: Fri Jul 14 09:41:29 2023, max compression
+gzip compressed data, was "gitprprod-0.0.4.tar", last modified: Mon Jul 17 11:24:32 2023, max compression
```

## Comparing `gitprprod-0.0.3.tar` & `gitprprod-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 09:41:29.912637 gitprprod-0.0.3/
--rw-rw-rw-   0        0        0      865 2023-07-14 09:41:29.912637 gitprprod-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-12 07:12:52.000000 gitprprod-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 09:41:29.892428 gitprprod-0.0.3/git_pr/
--rw-rw-rw-   0        0        0        0 2023-07-11 10:47:17.000000 gitprprod-0.0.3/git_pr/__init__.py
--rw-rw-rw-   0        0        0     2485 2023-07-13 06:56:32.000000 gitprprod-0.0.3/git_pr/git_pr.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:41:29.912637 gitprprod-0.0.3/gitprprod.egg-info/
--rw-rw-rw-   0        0        0      865 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5319 2023-07-14 09:41:12.000000 gitprprod-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 09:41:29.912637 gitprprod-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 11:24:32.385777 gitprprod-0.0.4/
+-rw-rw-rw-   0        0        0      865 2023-07-17 11:24:32.385777 gitprprod-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:12:52.000000 gitprprod-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:24:32.351562 gitprprod-0.0.4/git_pr/
+-rw-rw-rw-   0        0        0        0 2023-07-11 10:47:17.000000 gitprprod-0.0.4/git_pr/__init__.py
+-rw-rw-rw-   0        0        0     2986 2023-07-17 11:23:46.000000 gitprprod-0.0.4/git_pr/git_pr.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:24:32.382423 gitprprod-0.0.4/gitprprod.egg-info/
+-rw-rw-rw-   0        0        0      865 2023-07-17 11:24:32.000000 gitprprod-0.0.4/gitprprod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-17 11:24:32.000000 gitprprod-0.0.4/gitprprod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:24:32.000000 gitprprod-0.0.4/gitprprod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-17 11:24:32.000000 gitprprod-0.0.4/gitprprod.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-17 11:24:32.000000 gitprprod-0.0.4/gitprprod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 11:24:32.000000 gitprprod-0.0.4/gitprprod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5319 2023-07-17 10:15:30.000000 gitprprod-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:24:32.385777 gitprprod-0.0.4/setup.cfg
```

### Comparing `gitprprod-0.0.3/PKG-INFO` & `gitprprod-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitprprod
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Project for git pr
 Author-email: Abhinandan <abhinandan.x@nxp.com>
 Maintainer-email: Abhinandan <abhinandan.x@nxp.com>
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `gitprprod-0.0.3/git_pr/git_pr.py` & `gitprprod-0.0.4/git_pr/git_pr.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import argparse
 import subprocess
 import boto3
 import botocore
 import os
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+# logger = logging.getLogger(__name__)
+# logger.setLevel(logging.INFO)
 
 
 def get_current_repository():
     """get current repository"""
     try:
         # repo_output = subprocess.run(
         #     ["git", "rev-parse", "--show-toplevel"], check=False
@@ -30,55 +30,61 @@
         logging.error(
             "could not get repo name, please check if you are inside a git repository"
         )
 
 
 def create_pull_request(repo, branch_name, args):
     """create pull request"""
-    cc_client = boto3.client("codecommit")
+    if args.profile:
+        session = boto3.Session(profile_name=args.profile)
+    else:
+        session = boto3._get_default_session()
+    cc_client = session.client("codecommit")
     print(branch_name)
     try:
-        cc_client.create_pull_request(
+        response = cc_client.create_pull_request(
             title=args.title,
             description=args.description,
             targets=[
                 {
                     "repositoryName": repo,
                     "sourceReference": branch_name,  # args.source_branch,
                     "destinationReference": args.target_branch,
                 }
             ],
         )
-        logging.info("PR Created")
+        logging.info("PR created successfully; here is the link\n")
+        pr_url = f"https://{session.region_name}.console.aws.amazon.com/codesuite/codecommit/repositories/{repo}/pull-requests/{response['pullRequest']['pullRequestId']}?region={session.region_name}"
+        print(pr_url)
+        logging.info(response["pullRequest"]["pullRequestId"])
     except botocore.exceptions.ClientError as error:
         raise error
 
 
 def main():
     """main"""
     parser = argparse.ArgumentParser(description="codecommit command line parameter")
 
     # parser.add_argument("-r", "--repository", help="repository name")
     parser.add_argument("-sb", "--source_branch", help="enter source branch")
     parser.add_argument(
         "-tb", "--target_branch", help="enter target branch", default="main"
     )
+    parser.add_argument("-p", "--profile", help="aws profile")
     parser.add_argument(
         "-t", "--title", help="title of the pull request", required=True
     )
     parser.add_argument(
         "-desc", "--description", help="Pull Request Description Message", required=True
     )
 
     args = parser.parse_args()
 
     branch_name = get_current_repository()
     if branch_name:
         repository_name = (os.path.basename(os.getcwd())).strip("'")
 
         create_pull_request(repository_name, branch_name, args)
-    # else:
-    #     logger.error("")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gitprprod-0.0.3/gitprprod.egg-info/PKG-INFO` & `gitprprod-0.0.4/gitprprod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitprprod
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Project for git pr
 Author-email: Abhinandan <abhinandan.x@nxp.com>
 Maintainer-email: Abhinandan <abhinandan.x@nxp.com>
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `gitprprod-0.0.3/pyproject.toml` & `gitprprod-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "gitprprod"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.3"  # Required
+version = "0.0.4"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A Python Project for git pr"  # Optional
 
 # This is an optional longer description of your project that represents
```

