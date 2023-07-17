# Comparing `tmp/activitypubdantic-0.0.2.tar.gz` & `tmp/activitypubdantic-0.0.3.tar.gz`

## Comparing `activitypubdantic-0.0.2.tar` & `activitypubdantic-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0    22858 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic_test.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/create_docs.sh
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/developer_requirements.txt
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/requirements.txt
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/.github/workflows/distribute.yaml
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/__init__.py
--rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/get_class.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/get_model.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/__init__.py
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/activity.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/actor.py
--rw-r--r--   0        0        0    22796 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/core.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/link.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/object.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/_utils/__init__.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/_utils/language_types.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/_utils/mime_types.py
--rw-r--r--   0        0        0    47723 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/get_class.html
--rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/get_model.html
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/index.html
--rw-r--r--   0        0        0    94892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/activity.html
--rw-r--r--   0        0        0    41007 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/actor.html
--rw-r--r--   0        0        0   113691 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/core.html
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/index.html
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/link.html
--rw-r--r--   0        0        0    36238 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/object.html
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/article.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/create.json
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/like.json
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/note.json
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/person.json
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/accept.json
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/add.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/article.json
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/collection.json
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/image.json
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/move.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/person.json
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/place.json
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/question.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/tombstone.json
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/accept.json
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/create.json
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/follow.json
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/person.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/poll.json
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/LICENSE
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    10400 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    23455 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic_test.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/create_docs.sh
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/developer_requirements.txt
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/__init__.py
+-rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/get_class.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/get_model.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/__init__.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/activity.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/actor.py
+-rw-r--r--   0        0        0    22798 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/core.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/link.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/object.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/_utils/__init__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/_utils/language_types.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/activitypubdantic/models/_utils/mime_types.py
+-rw-r--r--   0        0        0    63781 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/get_class.html
+-rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/get_model.html
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/index.html
+-rw-r--r--   0        0        0    94892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/models/activity.html
+-rw-r--r--   0        0        0    41007 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/models/actor.html
+-rw-r--r--   0        0        0   113695 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/models/core.html
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/models/index.html
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/models/link.html
+-rw-r--r--   0        0        0    36238 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/docs/models/object.html
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitypub/article.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitypub/create.json
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitypub/like.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitypub/note.json
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitypub/person.json
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/accept.json
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/add.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/article.json
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/collection.json
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/image.json
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/move.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/person.json
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/place.json
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/question.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/activitystreams/tombstone.json
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/mastodon/accept.json
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/mastodon/create.json
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/mastodon/follow.json
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/mastodon/person.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/json/mastodon/poll.json
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/LICENSE
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 activitypubdantic-0.0.3/PKG-INFO
```

### Comparing `activitypubdantic-0.0.2/activitypubdantic_test.py` & `activitypubdantic-0.0.3/activitypubdantic_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,22 @@
         # Load the model and class
         output_model = ap.get_model(input_json)
         output_class = ap.get_class(input_json)
         output_data = output_class.data()
 
         # Assert that the data is the same
         assert len(output_data["to"]) == len(input_json["to"])
+        assert set(output_class.deliver_to()) == set(
+            [
+                "https://rhiaro.co.uk/#amy",
+                "https://dustycloud.org/followers",
+                "https://e14n.com/evan",
+                "https://rhiaro.co.uk/followers/",
+            ]
+        )
         assert output_model.type == input_json["type"] == output_data["type"] == "Like"
 
     def test_article(self):
         """
         Test that the Article model can load the example from the spec.
         """
         with open("json/activitypub/article.json", "r") as f:
@@ -152,14 +160,20 @@
         # Load the model and class
         output_model = ap.get_model(input_json)
         output_class = ap.get_class(input_json)
         output_data = output_class.data()
 
         # Assert that the data is the same
         assert output_data["name"] == input_json["name"]
+        assert set(output_class.deliver_to()) == set(
+            [
+                "https://e14n.com/evan",
+                "https://rhiaro.co.uk/followers/",
+            ]
+        )
         assert output_data["content"] == input_json["content"]
         assert (
             output_model.type == input_json["type"] == output_data["type"] == "Article"
         )
 
 
 class TestActivityStreams:
@@ -587,11 +601,14 @@
         # Load the model and class
         output_model = ap.get_model(input_json)
         output_class = ap.get_class(input_json)
         output_data = output_class.data()
 
         # Assert that the data is the same
         assert output_data["actor"][0]["type"] == "Object"
+        assert set(output_class.deliver_to()) == set(
+            ["https://activitypub.academy/users/dibutus_godorviol"]
+        )
         assert len(output_data["to"]) == len(input_json["to"]) == 1
         assert (
             output_model.type == input_json["type"] == output_data["type"] == "Accept"
         )
```

### Comparing `activitypubdantic-0.0.2/.github/workflows/distribute.yaml` & `activitypubdantic-0.0.3/.github/workflows/test.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-name: publish distribution
+name: test
 
 on:
-  release:
-    types: [published]
+  push:
+    branches:
+      - main
+  pull_request:
+    branches:
+      - main
 
 jobs:
   build:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
@@ -15,13 +19,10 @@
         with:
           python-version: "3.x"
       - name: Display Python version
         run: python -c "import sys; print(sys.version)"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install build
-      - name: Publish package
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_PROJECT_TOKEN }}
+          pip install -r developer_requirements.txt
+      - name: Test ActivityPubdantic
+        run: pytest
```

### Comparing `activitypubdantic-0.0.2/activitypubdantic/__init__.py` & `activitypubdantic-0.0.3/activitypubdantic/__init__.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/get_model.py` & `activitypubdantic-0.0.3/activitypubdantic/get_model.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/__init__.py` & `activitypubdantic-0.0.3/activitypubdantic/models/__init__.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/activity.py` & `activitypubdantic-0.0.3/activitypubdantic/models/activity.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/actor.py` & `activitypubdantic-0.0.3/activitypubdantic/models/actor.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/core.py` & `activitypubdantic-0.0.3/activitypubdantic/models/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
     _link_list_no_spaces_or_commas = field_validator("rel", mode="before")(
         validate_list_no_spaces_or_commas
     )
     _link_list_links_or_objects = field_validator("preview", mode="before")(
         validate_list_links_or_objects
     )
 
-    # Initialize with an optional positional argument for id
+    # Initialize with an optional positional argument for href
     def __init__(self, href: HttpUrl = None, **kwargs) -> None:
         if href:
             super(LinkModel, self).__init__(href=href, **kwargs)
         else:
             super(LinkModel, self).__init__(**kwargs)
```

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/link.py` & `activitypubdantic-0.0.3/activitypubdantic/models/link.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/object.py` & `activitypubdantic-0.0.3/activitypubdantic/models/object.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/_utils/language_types.py` & `activitypubdantic-0.0.3/activitypubdantic/models/_utils/language_types.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/activitypubdantic/models/_utils/mime_types.py` & `activitypubdantic-0.0.3/activitypubdantic/models/_utils/mime_types.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/docs/get_class.html` & `activitypubdantic-0.0.3/docs/get_class.html`

 * *Files 25% similar despite different names*

```diff
@@ -159,36 +159,100 @@
     def make_public(self):
         &#34;&#34;&#34;
         Remove any fields (bto and bcc) that should not be public.
         &#34;&#34;&#34;
         self.bto = None
         self.bcc = None
 
+    def deliver_to(self, depth: int = 2):
+        &#34;&#34;&#34;
+        Recursively iterate to determine the audience.
+        Use depth to set how deep the recursion should go.
+        Some IDs may indicate collections, which must be handled differently.
+        &#34;&#34;&#34;
+        audience_fields = [&#34;to&#34;, &#34;bto&#34;, &#34;cc&#34;, &#34;bcc&#34;, &#34;audience&#34;]
+        audience_members = []
+        delivery_objects = [self._internal_data()]
+        current_depth = 0
+
+        # Iterate checking for the existence of delivery objects and our depth
+        while current_depth &lt;= depth and len(delivery_objects) &gt; 0:
+            new_delivery_objects = []
+            for o in delivery_objects:
+                for k, v in o.items():
+                    if k in audience_fields and v:
+                        audience_members += v
+
+                    # If the key is an object, add it to the delivery objects
+                    elif isinstance(v, dict) and v:
+                        new_delivery_objects.append(v)
+
+            # Set the new delivery objects
+            delivery_objects = new_delivery_objects
+
+            # Increase the delivery depth before looping again
+            current_depth += 1
+
+        # Get the id of each audience member and remove duplicates
+        audience_members = [
+            str(a[&#34;id&#34;]) if isinstance(a, dict) and &#34;id&#34; in a else str(a)
+            for a in audience_members
+        ]
+        audience_members = list(set(audience_members))
+
+        # Return the audience members
+        return audience_members
+
     def create(self):
         &#34;&#34;&#34;
         Produce a new Activity of type Create with this Object.
+        After insertion into database, add an ID.
         &#34;&#34;&#34;
         if self._internal_data() == {}:
-            raise ValueError(&#34;Cannot Create an empty Object.&#34;)
+            raise ValueError(&#34;Cannot create an empty Object.&#34;)
         return get_class(
             {
                 &#34;type&#34;: &#34;Create&#34;,
+                &#34;actor&#34;: self.actor,
                 &#34;object&#34;: self._internal_data(),
                 &#34;to&#34;: self.to,
                 &#34;bto&#34;: self.bto,
                 &#34;cc&#34;: self.cc,
                 &#34;bcc&#34;: self.bcc,
                 &#34;audience&#34;: self.audience,
                 &#34;published&#34;: datetime.now(),
             }
         )
 
     def delete(self):
         &#34;&#34;&#34;
-        Produce a new Tombstone of this Object.
+        Produce a new Activity of type Delete with this Object.
+        Only provide an ID and published time for the Object.
+        After insertion into database, add an ID.
+        &#34;&#34;&#34;
+        return get_class(
+            {
+                &#34;type&#34;: &#34;Delete&#34;,
+                &#34;actor&#34;: self.actor,
+                &#34;object&#34;: {
+                    &#34;id&#34;: self.id,
+                    &#34;published&#34;: self.published,
+                },
+                &#34;to&#34;: self.to,
+                &#34;bto&#34;: self.bto,
+                &#34;cc&#34;: self.cc,
+                &#34;bcc&#34;: self.bcc,
+                &#34;audience&#34;: self.audience,
+                &#34;published&#34;: datetime.now(),
+            }
+        )
+
+    def tombstone(self):
+        &#34;&#34;&#34;
+        Produce a new Tombstone.
         &#34;&#34;&#34;
         return get_class(
             {
                 &#34;type&#34;: &#34;Tombstone&#34;,
                 &#34;id&#34;: self.id,
                 &#34;published&#34;: self.published,
                 &#34;updated&#34;: datetime.now(),
@@ -204,14 +268,15 @@
 
     # Core type
     core_type = &#34;Activity&#34;
 
     def undo(self):
         &#34;&#34;&#34;
         Produce a new Undo of this Activity.
+        After insertion into database, add an ID.
         &#34;&#34;&#34;
         return get_class(
             {
                 &#34;type&#34;: &#34;Undo&#34;,
                 &#34;object&#34;: self._internal_data(),
             }
         )
@@ -221,37 +286,79 @@
     &#34;&#34;&#34;
     Actor data and associated functions.
     &#34;&#34;&#34;
 
     # Core type
     core_type = &#34;Actor&#34;
 
-    def act(self, action_type: str, object: Object):
+    def activity(self, action_type: str, object: Object = None):
         &#34;&#34;&#34;
         Produce a new Activity of the given type with this Actor as the actor
         and the given Object as the object of the activity.
-        IntransitiveActivity will result in a validation failure.
+        Intransitive Activities have no object.
+        After insertion into database, add an ID.
         &#34;&#34;&#34;
         return get_class(
             {
                 &#34;type&#34;: action_type,
                 &#34;actor&#34;: self._internal_data(),
-                &#34;object&#34;: object.data(),
+                &#34;object&#34;: object.data() if object else None,
             }
         )
 
 
 class Collection(Object):
     &#34;&#34;&#34;
     Collection data and associated functions.
     &#34;&#34;&#34;
 
     # Core type
     core_type = &#34;Collection&#34;
 
+    def add(self, object: Object = None):
+        &#34;&#34;&#34;
+        Add an Object to the Collection.
+        &#34;&#34;&#34;
+        if object._internal_data() == {}:
+            raise ValueError(&#34;Cannot add an empty Object.&#34;)
+
+        # Use the items or ordered_items fields
+        if &#34;items&#34; in self._internal_data():
+            self.items.insert(0, object.data())
+            items_count = len(self.items)
+        elif &#34;ordered_items&#34; in self._internal_data():
+            self.ordered_items.insert(0, object.data())
+            items_count = len(self.ordered_items)
+
+        # Update total items
+        self.total_items = items_count
+
+    def remove(self, object: Object = None):
+        &#34;&#34;&#34;
+        Remove an Object from the Collection.
+        The Object must have an ID.
+        &#34;&#34;&#34;
+        if object._internal_data() == {}:
+            raise ValueError(&#34;Cannot remove an empty Object.&#34;)
+        if object.id is None:
+            raise ValueError(&#34;Cannot remove an Object without an ID.&#34;)
+
+        # Use the items or ordered_items fields
+        if &#34;items&#34; in self._internal_data():
+            self.items = [i for i in self.items if &#34;id&#34; in i and i[&#34;id&#34;] != object.id]
+            items_count = len(self.items)
+        elif &#34;ordered_items&#34; in self._internal_data():
+            self.ordered_items = [
+                i for i in self.ordered_items if &#34;id&#34; in i and i[&#34;id&#34;] != object.id
+            ]
+            items_count = len(self.ordered_items)
+
+        # Update total items
+        self.total_items = items_count
+
 
 &#34;&#34;&#34;
 MAPPING DICTIONARY
 &#34;&#34;&#34;
 
 
 # Map type names to their classes
@@ -435,14 +542,15 @@
 
     # Core type
     core_type = &#34;Activity&#34;
 
     def undo(self):
         &#34;&#34;&#34;
         Produce a new Undo of this Activity.
+        After insertion into database, add an ID.
         &#34;&#34;&#34;
         return get_class(
             {
                 &#34;type&#34;: &#34;Undo&#34;,
                 &#34;object&#34;: self._internal_data(),
             }
         )</code></pre>
@@ -461,22 +569,24 @@
 </dl>
 <h3>Methods</h3>
 <dl>
 <dt id="activitypubdantic.get_class.Activity.undo"><code class="name flex">
 <span>def <span class="ident">undo</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Produce a new Undo of this Activity.</p></div>
+<div class="desc"><p>Produce a new Undo of this Activity.
+After insertion into database, add an ID.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def undo(self):
     &#34;&#34;&#34;
     Produce a new Undo of this Activity.
+    After insertion into database, add an ID.
     &#34;&#34;&#34;
     return get_class(
         {
             &#34;type&#34;: &#34;Undo&#34;,
             &#34;object&#34;: self._internal_data(),
         }
     )</code></pre>
@@ -486,16 +596,18 @@
 <h3>Inherited members</h3>
 <ul class="hlist">
 <li><code><b><a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a></b></code>:
 <ul class="hlist">
 <li><code><a title="activitypubdantic.get_class.Object.create" href="#activitypubdantic.get_class.Object.create">create</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.data" href="#activitypubdantic.get_class.Base.data">data</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.delete" href="#activitypubdantic.get_class.Object.delete">delete</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.deliver_to" href="#activitypubdantic.get_class.Object.deliver_to">deliver_to</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.json" href="#activitypubdantic.get_class.Base.json">json</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.make_public" href="#activitypubdantic.get_class.Object.make_public">make_public</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.tombstone" href="#activitypubdantic.get_class.Object.tombstone">tombstone</a></code></li>
 </ul>
 </li>
 </ul>
 </dd>
 <dt id="activitypubdantic.get_class.Actor"><code class="flex name class">
 <span>class <span class="ident">Actor</span></span>
 <span>(</span><span>model: Union[<a title="activitypubdantic.models.core.ActivityModel" href="models/core.html#activitypubdantic.models.core.ActivityModel">ActivityModel</a>, <a title="activitypubdantic.models.actor.ActorModel" href="models/actor.html#activitypubdantic.models.actor.ActorModel">ActorModel</a>, <a title="activitypubdantic.models.core.CollectionModel" href="models/core.html#activitypubdantic.models.core.CollectionModel">CollectionModel</a>, <a title="activitypubdantic.models.core.LinkModel" href="models/core.html#activitypubdantic.models.core.LinkModel">LinkModel</a>, <a title="activitypubdantic.models.core.ObjectModel" href="models/core.html#activitypubdantic.models.core.ObjectModel">ObjectModel</a>], input_json: dict, default_languages: list = ['en', 'en-US'])</span>
@@ -510,25 +622,26 @@
     &#34;&#34;&#34;
     Actor data and associated functions.
     &#34;&#34;&#34;
 
     # Core type
     core_type = &#34;Actor&#34;
 
-    def act(self, action_type: str, object: Object):
+    def activity(self, action_type: str, object: Object = None):
         &#34;&#34;&#34;
         Produce a new Activity of the given type with this Actor as the actor
         and the given Object as the object of the activity.
-        IntransitiveActivity will result in a validation failure.
+        Intransitive Activities have no object.
+        After insertion into database, add an ID.
         &#34;&#34;&#34;
         return get_class(
             {
                 &#34;type&#34;: action_type,
                 &#34;actor&#34;: self._internal_data(),
-                &#34;object&#34;: object.data(),
+                &#34;object&#34;: object.data() if object else None,
             }
         )</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a></li>
 <li><a title="activitypubdantic.get_class.Base" href="#activitypubdantic.get_class.Base">Base</a></li>
@@ -538,50 +651,54 @@
 <dt id="activitypubdantic.get_class.Actor.core_type"><code class="name">var <span class="ident">core_type</span></code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 </dl>
 <h3>Methods</h3>
 <dl>
-<dt id="activitypubdantic.get_class.Actor.act"><code class="name flex">
-<span>def <span class="ident">act</span></span>(<span>self, action_type: str, object: <a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a>)</span>
+<dt id="activitypubdantic.get_class.Actor.activity"><code class="name flex">
+<span>def <span class="ident">activity</span></span>(<span>self, action_type: str, object: <a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a> = None)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Produce a new Activity of the given type with this Actor as the actor
 and the given Object as the object of the activity.
-IntransitiveActivity will result in a validation failure.</p></div>
+Intransitive Activities have no object.
+After insertion into database, add an ID.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def act(self, action_type: str, object: Object):
+<pre><code class="python">def activity(self, action_type: str, object: Object = None):
     &#34;&#34;&#34;
     Produce a new Activity of the given type with this Actor as the actor
     and the given Object as the object of the activity.
-    IntransitiveActivity will result in a validation failure.
+    Intransitive Activities have no object.
+    After insertion into database, add an ID.
     &#34;&#34;&#34;
     return get_class(
         {
             &#34;type&#34;: action_type,
             &#34;actor&#34;: self._internal_data(),
-            &#34;object&#34;: object.data(),
+            &#34;object&#34;: object.data() if object else None,
         }
     )</code></pre>
 </details>
 </dd>
 </dl>
 <h3>Inherited members</h3>
 <ul class="hlist">
 <li><code><b><a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a></b></code>:
 <ul class="hlist">
 <li><code><a title="activitypubdantic.get_class.Object.create" href="#activitypubdantic.get_class.Object.create">create</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.data" href="#activitypubdantic.get_class.Base.data">data</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.delete" href="#activitypubdantic.get_class.Object.delete">delete</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.deliver_to" href="#activitypubdantic.get_class.Object.deliver_to">deliver_to</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.json" href="#activitypubdantic.get_class.Base.json">json</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.make_public" href="#activitypubdantic.get_class.Object.make_public">make_public</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.tombstone" href="#activitypubdantic.get_class.Object.tombstone">tombstone</a></code></li>
 </ul>
 </li>
 </ul>
 </dd>
 <dt id="activitypubdantic.get_class.Base"><code class="flex name class">
 <span>class <span class="ident">Base</span></span>
 <span>(</span><span>model: Union[<a title="activitypubdantic.models.core.ActivityModel" href="models/core.html#activitypubdantic.models.core.ActivityModel">ActivityModel</a>, <a title="activitypubdantic.models.actor.ActorModel" href="models/actor.html#activitypubdantic.models.actor.ActorModel">ActorModel</a>, <a title="activitypubdantic.models.core.CollectionModel" href="models/core.html#activitypubdantic.models.core.CollectionModel">CollectionModel</a>, <a title="activitypubdantic.models.core.LinkModel" href="models/core.html#activitypubdantic.models.core.LinkModel">LinkModel</a>, <a title="activitypubdantic.models.core.ObjectModel" href="models/core.html#activitypubdantic.models.core.ObjectModel">ObjectModel</a>], input_json: dict, default_languages: list = ['en', 'en-US'])</span>
@@ -747,37 +864,145 @@
 </summary>
 <pre><code class="python">class Collection(Object):
     &#34;&#34;&#34;
     Collection data and associated functions.
     &#34;&#34;&#34;
 
     # Core type
-    core_type = &#34;Collection&#34;</code></pre>
+    core_type = &#34;Collection&#34;
+
+    def add(self, object: Object = None):
+        &#34;&#34;&#34;
+        Add an Object to the Collection.
+        &#34;&#34;&#34;
+        if object._internal_data() == {}:
+            raise ValueError(&#34;Cannot add an empty Object.&#34;)
+
+        # Use the items or ordered_items fields
+        if &#34;items&#34; in self._internal_data():
+            self.items.insert(0, object.data())
+            items_count = len(self.items)
+        elif &#34;ordered_items&#34; in self._internal_data():
+            self.ordered_items.insert(0, object.data())
+            items_count = len(self.ordered_items)
+
+        # Update total items
+        self.total_items = items_count
+
+    def remove(self, object: Object = None):
+        &#34;&#34;&#34;
+        Remove an Object from the Collection.
+        The Object must have an ID.
+        &#34;&#34;&#34;
+        if object._internal_data() == {}:
+            raise ValueError(&#34;Cannot remove an empty Object.&#34;)
+        if object.id is None:
+            raise ValueError(&#34;Cannot remove an Object without an ID.&#34;)
+
+        # Use the items or ordered_items fields
+        if &#34;items&#34; in self._internal_data():
+            self.items = [i for i in self.items if &#34;id&#34; in i and i[&#34;id&#34;] != object.id]
+            items_count = len(self.items)
+        elif &#34;ordered_items&#34; in self._internal_data():
+            self.ordered_items = [
+                i for i in self.ordered_items if &#34;id&#34; in i and i[&#34;id&#34;] != object.id
+            ]
+            items_count = len(self.ordered_items)
+
+        # Update total items
+        self.total_items = items_count</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li><a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a></li>
 <li><a title="activitypubdantic.get_class.Base" href="#activitypubdantic.get_class.Base">Base</a></li>
 </ul>
 <h3>Class variables</h3>
 <dl>
 <dt id="activitypubdantic.get_class.Collection.core_type"><code class="name">var <span class="ident">core_type</span></code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 </dl>
+<h3>Methods</h3>
+<dl>
+<dt id="activitypubdantic.get_class.Collection.add"><code class="name flex">
+<span>def <span class="ident">add</span></span>(<span>self, object: <a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a> = None)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Add an Object to the Collection.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def add(self, object: Object = None):
+    &#34;&#34;&#34;
+    Add an Object to the Collection.
+    &#34;&#34;&#34;
+    if object._internal_data() == {}:
+        raise ValueError(&#34;Cannot add an empty Object.&#34;)
+
+    # Use the items or ordered_items fields
+    if &#34;items&#34; in self._internal_data():
+        self.items.insert(0, object.data())
+        items_count = len(self.items)
+    elif &#34;ordered_items&#34; in self._internal_data():
+        self.ordered_items.insert(0, object.data())
+        items_count = len(self.ordered_items)
+
+    # Update total items
+    self.total_items = items_count</code></pre>
+</details>
+</dd>
+<dt id="activitypubdantic.get_class.Collection.remove"><code class="name flex">
+<span>def <span class="ident">remove</span></span>(<span>self, object: <a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a> = None)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Remove an Object from the Collection.
+The Object must have an ID.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def remove(self, object: Object = None):
+    &#34;&#34;&#34;
+    Remove an Object from the Collection.
+    The Object must have an ID.
+    &#34;&#34;&#34;
+    if object._internal_data() == {}:
+        raise ValueError(&#34;Cannot remove an empty Object.&#34;)
+    if object.id is None:
+        raise ValueError(&#34;Cannot remove an Object without an ID.&#34;)
+
+    # Use the items or ordered_items fields
+    if &#34;items&#34; in self._internal_data():
+        self.items = [i for i in self.items if &#34;id&#34; in i and i[&#34;id&#34;] != object.id]
+        items_count = len(self.items)
+    elif &#34;ordered_items&#34; in self._internal_data():
+        self.ordered_items = [
+            i for i in self.ordered_items if &#34;id&#34; in i and i[&#34;id&#34;] != object.id
+        ]
+        items_count = len(self.ordered_items)
+
+    # Update total items
+    self.total_items = items_count</code></pre>
+</details>
+</dd>
+</dl>
 <h3>Inherited members</h3>
 <ul class="hlist">
 <li><code><b><a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a></b></code>:
 <ul class="hlist">
 <li><code><a title="activitypubdantic.get_class.Object.create" href="#activitypubdantic.get_class.Object.create">create</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.data" href="#activitypubdantic.get_class.Base.data">data</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.delete" href="#activitypubdantic.get_class.Object.delete">delete</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.deliver_to" href="#activitypubdantic.get_class.Object.deliver_to">deliver_to</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.json" href="#activitypubdantic.get_class.Base.json">json</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.make_public" href="#activitypubdantic.get_class.Object.make_public">make_public</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.tombstone" href="#activitypubdantic.get_class.Object.tombstone">tombstone</a></code></li>
 </ul>
 </li>
 </ul>
 </dd>
 <dt id="activitypubdantic.get_class.Link"><code class="flex name class">
 <span>class <span class="ident">Link</span></span>
 <span>(</span><span>model: Union[<a title="activitypubdantic.models.core.ActivityModel" href="models/core.html#activitypubdantic.models.core.ActivityModel">ActivityModel</a>, <a title="activitypubdantic.models.actor.ActorModel" href="models/actor.html#activitypubdantic.models.actor.ActorModel">ActorModel</a>, <a title="activitypubdantic.models.core.CollectionModel" href="models/core.html#activitypubdantic.models.core.CollectionModel">CollectionModel</a>, <a title="activitypubdantic.models.core.LinkModel" href="models/core.html#activitypubdantic.models.core.LinkModel">LinkModel</a>, <a title="activitypubdantic.models.core.ObjectModel" href="models/core.html#activitypubdantic.models.core.ObjectModel">ObjectModel</a>], input_json: dict, default_languages: list = ['en', 'en-US'])</span>
@@ -838,36 +1063,100 @@
     def make_public(self):
         &#34;&#34;&#34;
         Remove any fields (bto and bcc) that should not be public.
         &#34;&#34;&#34;
         self.bto = None
         self.bcc = None
 
+    def deliver_to(self, depth: int = 2):
+        &#34;&#34;&#34;
+        Recursively iterate to determine the audience.
+        Use depth to set how deep the recursion should go.
+        Some IDs may indicate collections, which must be handled differently.
+        &#34;&#34;&#34;
+        audience_fields = [&#34;to&#34;, &#34;bto&#34;, &#34;cc&#34;, &#34;bcc&#34;, &#34;audience&#34;]
+        audience_members = []
+        delivery_objects = [self._internal_data()]
+        current_depth = 0
+
+        # Iterate checking for the existence of delivery objects and our depth
+        while current_depth &lt;= depth and len(delivery_objects) &gt; 0:
+            new_delivery_objects = []
+            for o in delivery_objects:
+                for k, v in o.items():
+                    if k in audience_fields and v:
+                        audience_members += v
+
+                    # If the key is an object, add it to the delivery objects
+                    elif isinstance(v, dict) and v:
+                        new_delivery_objects.append(v)
+
+            # Set the new delivery objects
+            delivery_objects = new_delivery_objects
+
+            # Increase the delivery depth before looping again
+            current_depth += 1
+
+        # Get the id of each audience member and remove duplicates
+        audience_members = [
+            str(a[&#34;id&#34;]) if isinstance(a, dict) and &#34;id&#34; in a else str(a)
+            for a in audience_members
+        ]
+        audience_members = list(set(audience_members))
+
+        # Return the audience members
+        return audience_members
+
     def create(self):
         &#34;&#34;&#34;
         Produce a new Activity of type Create with this Object.
+        After insertion into database, add an ID.
         &#34;&#34;&#34;
         if self._internal_data() == {}:
-            raise ValueError(&#34;Cannot Create an empty Object.&#34;)
+            raise ValueError(&#34;Cannot create an empty Object.&#34;)
         return get_class(
             {
                 &#34;type&#34;: &#34;Create&#34;,
+                &#34;actor&#34;: self.actor,
                 &#34;object&#34;: self._internal_data(),
                 &#34;to&#34;: self.to,
                 &#34;bto&#34;: self.bto,
                 &#34;cc&#34;: self.cc,
                 &#34;bcc&#34;: self.bcc,
                 &#34;audience&#34;: self.audience,
                 &#34;published&#34;: datetime.now(),
             }
         )
 
     def delete(self):
         &#34;&#34;&#34;
-        Produce a new Tombstone of this Object.
+        Produce a new Activity of type Delete with this Object.
+        Only provide an ID and published time for the Object.
+        After insertion into database, add an ID.
+        &#34;&#34;&#34;
+        return get_class(
+            {
+                &#34;type&#34;: &#34;Delete&#34;,
+                &#34;actor&#34;: self.actor,
+                &#34;object&#34;: {
+                    &#34;id&#34;: self.id,
+                    &#34;published&#34;: self.published,
+                },
+                &#34;to&#34;: self.to,
+                &#34;bto&#34;: self.bto,
+                &#34;cc&#34;: self.cc,
+                &#34;bcc&#34;: self.bcc,
+                &#34;audience&#34;: self.audience,
+                &#34;published&#34;: datetime.now(),
+            }
+        )
+
+    def tombstone(self):
+        &#34;&#34;&#34;
+        Produce a new Tombstone.
         &#34;&#34;&#34;
         return get_class(
             {
                 &#34;type&#34;: &#34;Tombstone&#34;,
                 &#34;id&#34;: self.id,
                 &#34;published&#34;: self.published,
                 &#34;updated&#34;: datetime.now(),
@@ -894,28 +1183,31 @@
 </dl>
 <h3>Methods</h3>
 <dl>
 <dt id="activitypubdantic.get_class.Object.create"><code class="name flex">
 <span>def <span class="ident">create</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Produce a new Activity of type Create with this Object.</p></div>
+<div class="desc"><p>Produce a new Activity of type Create with this Object.
+After insertion into database, add an ID.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def create(self):
     &#34;&#34;&#34;
     Produce a new Activity of type Create with this Object.
+    After insertion into database, add an ID.
     &#34;&#34;&#34;
     if self._internal_data() == {}:
-        raise ValueError(&#34;Cannot Create an empty Object.&#34;)
+        raise ValueError(&#34;Cannot create an empty Object.&#34;)
     return get_class(
         {
             &#34;type&#34;: &#34;Create&#34;,
+            &#34;actor&#34;: self.actor,
             &#34;object&#34;: self._internal_data(),
             &#34;to&#34;: self.to,
             &#34;bto&#34;: self.bto,
             &#34;cc&#34;: self.cc,
             &#34;bcc&#34;: self.bcc,
             &#34;audience&#34;: self.audience,
             &#34;published&#34;: datetime.now(),
@@ -923,34 +1215,96 @@
     )</code></pre>
 </details>
 </dd>
 <dt id="activitypubdantic.get_class.Object.delete"><code class="name flex">
 <span>def <span class="ident">delete</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Produce a new Tombstone of this Object.</p></div>
+<div class="desc"><p>Produce a new Activity of type Delete with this Object.
+Only provide an ID and published time for the Object.
+After insertion into database, add an ID.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def delete(self):
     &#34;&#34;&#34;
-    Produce a new Tombstone of this Object.
+    Produce a new Activity of type Delete with this Object.
+    Only provide an ID and published time for the Object.
+    After insertion into database, add an ID.
     &#34;&#34;&#34;
     return get_class(
         {
-            &#34;type&#34;: &#34;Tombstone&#34;,
-            &#34;id&#34;: self.id,
-            &#34;published&#34;: self.published,
-            &#34;updated&#34;: datetime.now(),
-            &#34;deleted&#34;: datetime.now(),
+            &#34;type&#34;: &#34;Delete&#34;,
+            &#34;actor&#34;: self.actor,
+            &#34;object&#34;: {
+                &#34;id&#34;: self.id,
+                &#34;published&#34;: self.published,
+            },
+            &#34;to&#34;: self.to,
+            &#34;bto&#34;: self.bto,
+            &#34;cc&#34;: self.cc,
+            &#34;bcc&#34;: self.bcc,
+            &#34;audience&#34;: self.audience,
+            &#34;published&#34;: datetime.now(),
         }
     )</code></pre>
 </details>
 </dd>
+<dt id="activitypubdantic.get_class.Object.deliver_to"><code class="name flex">
+<span>def <span class="ident">deliver_to</span></span>(<span>self, depth: int = 2)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Recursively iterate to determine the audience.
+Use depth to set how deep the recursion should go.
+Some IDs may indicate collections, which must be handled differently.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def deliver_to(self, depth: int = 2):
+    &#34;&#34;&#34;
+    Recursively iterate to determine the audience.
+    Use depth to set how deep the recursion should go.
+    Some IDs may indicate collections, which must be handled differently.
+    &#34;&#34;&#34;
+    audience_fields = [&#34;to&#34;, &#34;bto&#34;, &#34;cc&#34;, &#34;bcc&#34;, &#34;audience&#34;]
+    audience_members = []
+    delivery_objects = [self._internal_data()]
+    current_depth = 0
+
+    # Iterate checking for the existence of delivery objects and our depth
+    while current_depth &lt;= depth and len(delivery_objects) &gt; 0:
+        new_delivery_objects = []
+        for o in delivery_objects:
+            for k, v in o.items():
+                if k in audience_fields and v:
+                    audience_members += v
+
+                # If the key is an object, add it to the delivery objects
+                elif isinstance(v, dict) and v:
+                    new_delivery_objects.append(v)
+
+        # Set the new delivery objects
+        delivery_objects = new_delivery_objects
+
+        # Increase the delivery depth before looping again
+        current_depth += 1
+
+    # Get the id of each audience member and remove duplicates
+    audience_members = [
+        str(a[&#34;id&#34;]) if isinstance(a, dict) and &#34;id&#34; in a else str(a)
+        for a in audience_members
+    ]
+    audience_members = list(set(audience_members))
+
+    # Return the audience members
+    return audience_members</code></pre>
+</details>
+</dd>
 <dt id="activitypubdantic.get_class.Object.make_public"><code class="name flex">
 <span>def <span class="ident">make_public</span></span>(<span>self)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Remove any fields (bto and bcc) that should not be public.</p></div>
 <details class="source">
 <summary>
@@ -960,14 +1314,38 @@
     &#34;&#34;&#34;
     Remove any fields (bto and bcc) that should not be public.
     &#34;&#34;&#34;
     self.bto = None
     self.bcc = None</code></pre>
 </details>
 </dd>
+<dt id="activitypubdantic.get_class.Object.tombstone"><code class="name flex">
+<span>def <span class="ident">tombstone</span></span>(<span>self)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Produce a new Tombstone.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def tombstone(self):
+    &#34;&#34;&#34;
+    Produce a new Tombstone.
+    &#34;&#34;&#34;
+    return get_class(
+        {
+            &#34;type&#34;: &#34;Tombstone&#34;,
+            &#34;id&#34;: self.id,
+            &#34;published&#34;: self.published,
+            &#34;updated&#34;: datetime.now(),
+            &#34;deleted&#34;: datetime.now(),
+        }
+    )</code></pre>
+</details>
+</dd>
 </dl>
 <h3>Inherited members</h3>
 <ul class="hlist">
 <li><code><b><a title="activitypubdantic.get_class.Base" href="#activitypubdantic.get_class.Base">Base</a></b></code>:
 <ul class="hlist">
 <li><code><a title="activitypubdantic.get_class.Base.data" href="#activitypubdantic.get_class.Base.data">data</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Base.json" href="#activitypubdantic.get_class.Base.json">json</a></code></li>
@@ -1003,44 +1381,48 @@
 <li><code><a title="activitypubdantic.get_class.Activity.core_type" href="#activitypubdantic.get_class.Activity.core_type">core_type</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Activity.undo" href="#activitypubdantic.get_class.Activity.undo">undo</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="activitypubdantic.get_class.Actor" href="#activitypubdantic.get_class.Actor">Actor</a></code></h4>
 <ul class="">
-<li><code><a title="activitypubdantic.get_class.Actor.act" href="#activitypubdantic.get_class.Actor.act">act</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Actor.activity" href="#activitypubdantic.get_class.Actor.activity">activity</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Actor.core_type" href="#activitypubdantic.get_class.Actor.core_type">core_type</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="activitypubdantic.get_class.Base" href="#activitypubdantic.get_class.Base">Base</a></code></h4>
 <ul class="">
 <li><code><a title="activitypubdantic.get_class.Base.data" href="#activitypubdantic.get_class.Base.data">data</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Base.json" href="#activitypubdantic.get_class.Base.json">json</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="activitypubdantic.get_class.Collection" href="#activitypubdantic.get_class.Collection">Collection</a></code></h4>
 <ul class="">
+<li><code><a title="activitypubdantic.get_class.Collection.add" href="#activitypubdantic.get_class.Collection.add">add</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Collection.core_type" href="#activitypubdantic.get_class.Collection.core_type">core_type</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Collection.remove" href="#activitypubdantic.get_class.Collection.remove">remove</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="activitypubdantic.get_class.Link" href="#activitypubdantic.get_class.Link">Link</a></code></h4>
 <ul class="">
 <li><code><a title="activitypubdantic.get_class.Link.core_type" href="#activitypubdantic.get_class.Link.core_type">core_type</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="activitypubdantic.get_class.Object" href="#activitypubdantic.get_class.Object">Object</a></code></h4>
-<ul class="">
+<ul class="two-column">
 <li><code><a title="activitypubdantic.get_class.Object.core_type" href="#activitypubdantic.get_class.Object.core_type">core_type</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.create" href="#activitypubdantic.get_class.Object.create">create</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.delete" href="#activitypubdantic.get_class.Object.delete">delete</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.deliver_to" href="#activitypubdantic.get_class.Object.deliver_to">deliver_to</a></code></li>
 <li><code><a title="activitypubdantic.get_class.Object.make_public" href="#activitypubdantic.get_class.Object.make_public">make_public</a></code></li>
+<li><code><a title="activitypubdantic.get_class.Object.tombstone" href="#activitypubdantic.get_class.Object.tombstone">tombstone</a></code></li>
 </ul>
 </li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
```

#### html2text {}

```diff
@@ -143,36 +143,100 @@
     def make_public(self):
         """
         Remove any fields (bto and bcc) that should not be public.
         """
         self.bto = None
         self.bcc = None
 
+    def deliver_to(self, depth: int = 2):
+        """
+        Recursively iterate to determine the audience.
+        Use depth to set how deep the recursion should go.
+        Some IDs may indicate collections, which must be handled differently.
+        """
+        audience_fields = ["to", "bto", "cc", "bcc", "audience"]
+        audience_members = []
+        delivery_objects = [self._internal_data()]
+        current_depth = 0
+
+        # Iterate checking for the existence of delivery objects and our depth
+        while current_depth <= depth and len(delivery_objects) > 0:
+            new_delivery_objects = []
+            for o in delivery_objects:
+                for k, v in o.items():
+                    if k in audience_fields and v:
+                        audience_members += v
+
+                    # If the key is an object, add it to the delivery objects
+                    elif isinstance(v, dict) and v:
+                        new_delivery_objects.append(v)
+
+            # Set the new delivery objects
+            delivery_objects = new_delivery_objects
+
+            # Increase the delivery depth before looping again
+            current_depth += 1
+
+        # Get the id of each audience member and remove duplicates
+        audience_members = [
+            str(a["id"]) if isinstance(a, dict) and "id" in a else str(a)
+            for a in audience_members
+        ]
+        audience_members = list(set(audience_members))
+
+        # Return the audience members
+        return audience_members
+
     def create(self):
         """
         Produce a new Activity of type Create with this Object.
+        After insertion into database, add an ID.
         """
         if self._internal_data() == {}:
-            raise ValueError("Cannot Create an empty Object.")
+            raise ValueError("Cannot create an empty Object.")
         return get_class(
             {
                 "type": "Create",
+                "actor": self.actor,
                 "object": self._internal_data(),
                 "to": self.to,
                 "bto": self.bto,
                 "cc": self.cc,
                 "bcc": self.bcc,
                 "audience": self.audience,
                 "published": datetime.now(),
             }
         )
 
     def delete(self):
         """
-        Produce a new Tombstone of this Object.
+        Produce a new Activity of type Delete with this Object.
+        Only provide an ID and published time for the Object.
+        After insertion into database, add an ID.
+        """
+        return get_class(
+            {
+                "type": "Delete",
+                "actor": self.actor,
+                "object": {
+                    "id": self.id,
+                    "published": self.published,
+                },
+                "to": self.to,
+                "bto": self.bto,
+                "cc": self.cc,
+                "bcc": self.bcc,
+                "audience": self.audience,
+                "published": datetime.now(),
+            }
+        )
+
+    def tombstone(self):
+        """
+        Produce a new Tombstone.
         """
         return get_class(
             {
                 "type": "Tombstone",
                 "id": self.id,
                 "published": self.published,
                 "updated": datetime.now(),
@@ -188,14 +252,15 @@
 
     # Core type
     core_type = "Activity"
 
     def undo(self):
         """
         Produce a new Undo of this Activity.
+        After insertion into database, add an ID.
         """
         return get_class(
             {
                 "type": "Undo",
                 "object": self._internal_data(),
             }
         )
@@ -205,37 +270,81 @@
     """
     Actor data and associated functions.
     """
 
     # Core type
     core_type = "Actor"
 
-    def act(self, action_type: str, object: Object):
+    def activity(self, action_type: str, object: Object = None):
         """
         Produce a new Activity of the given type with this Actor as the actor
         and the given Object as the object of the activity.
-        IntransitiveActivity will result in a validation failure.
+        Intransitive Activities have no object.
+        After insertion into database, add an ID.
         """
         return get_class(
             {
                 "type": action_type,
                 "actor": self._internal_data(),
-                "object": object.data(),
+                "object": object.data() if object else None,
             }
         )
 
 
 class Collection(Object):
     """
     Collection data and associated functions.
     """
 
     # Core type
     core_type = "Collection"
 
+    def add(self, object: Object = None):
+        """
+        Add an Object to the Collection.
+        """
+        if object._internal_data() == {}:
+            raise ValueError("Cannot add an empty Object.")
+
+        # Use the items or ordered_items fields
+        if "items" in self._internal_data():
+            self.items.insert(0, object.data())
+            items_count = len(self.items)
+        elif "ordered_items" in self._internal_data():
+            self.ordered_items.insert(0, object.data())
+            items_count = len(self.ordered_items)
+
+        # Update total items
+        self.total_items = items_count
+
+    def remove(self, object: Object = None):
+        """
+        Remove an Object from the Collection.
+        The Object must have an ID.
+        """
+        if object._internal_data() == {}:
+            raise ValueError("Cannot remove an empty Object.")
+        if object.id is None:
+            raise ValueError("Cannot remove an Object without an ID.")
+
+        # Use the items or ordered_items fields
+        if "items" in self._internal_data():
+            self.items = [i for i in self.items if "id" in i and i["id"] !=
+object.id]
+            items_count = len(self.items)
+        elif "ordered_items" in self._internal_data():
+            self.ordered_items = [
+                i for i in self.ordered_items if "id" in i and i["id"] !=
+object.id
+            ]
+            items_count = len(self.ordered_items)
+
+        # Update total items
+        self.total_items = items_count
+
 
 """
 MAPPING DICTIONARY
 """
 
 
 # Map type names to their classes
@@ -397,106 +506,116 @@
 
           # Core type
           core_type = "Activity"
 
           def undo(self):
               """
               Produce a new Undo of this Activity.
+              After insertion into database, add an ID.
               """
               return get_class(
                   {
                       "type": "Undo",
                       "object": self._internal_data(),
                   }
               )
       **** Ancestors ****
           * Object
           * Base
       **** Class variables ****
         var core_type
       **** Methods ****
         def undo(self)
-            Produce a new Undo of this Activity.
+            Produce a new Undo of this Activity. After insertion into database,
+            add an ID.
               Expand source code
             def undo(self):
                 """
                 Produce a new Undo of this Activity.
+                After insertion into database, add an ID.
                 """
                 return get_class(
                     {
                         "type": "Undo",
                         "object": self._internal_data(),
                     }
                 )
       **** Inherited members ****
           * Object:
                 o create
                 o data
                 o delete
+                o deliver_to
                 o json
                 o make_public
+                o tombstone
   class Actor (model:Â Union
   [ActivityModel,Â ActorModel,Â CollectionModel,Â LinkModel,Â ObjectModel],
   input_json:Â dict, default_languages:Â listÂ =Â ['en', 'en-US'])
       Actor data and associated functions.
         Expand source code
       class Actor(Object):
           """
           Actor data and associated functions.
           """
 
           # Core type
           core_type = "Actor"
 
-          def act(self, action_type: str, object: Object):
+          def activity(self, action_type: str, object: Object = None):
               """
               Produce a new Activity of the given type with this Actor as the
       actor
               and the given Object as the object of the activity.
-              IntransitiveActivity will result in a validation failure.
+              Intransitive Activities have no object.
+              After insertion into database, add an ID.
               """
               return get_class(
                   {
                       "type": action_type,
                       "actor": self._internal_data(),
-                      "object": object.data(),
+                      "object": object.data() if object else None,
                   }
               )
       **** Ancestors ****
           * Object
           * Base
       **** Class variables ****
         var core_type
       **** Methods ****
-        def act(self, action_type:Â str, object:Â Object)
+        def activity(self, action_type:Â str, object:Â ObjectÂ =Â None)
             Produce a new Activity of the given type with this Actor as the
             actor and the given Object as the object of the activity.
-            IntransitiveActivity will result in a validation failure.
+            Intransitive Activities have no object. After insertion into
+            database, add an ID.
               Expand source code
-            def act(self, action_type: str, object: Object):
+            def activity(self, action_type: str, object: Object = None):
                 """
                 Produce a new Activity of the given type with this Actor as the
             actor
                 and the given Object as the object of the activity.
-                IntransitiveActivity will result in a validation failure.
+                Intransitive Activities have no object.
+                After insertion into database, add an ID.
                 """
                 return get_class(
                     {
                         "type": action_type,
                         "actor": self._internal_data(),
-                        "object": object.data(),
+                        "object": object.data() if object else None,
                     }
                 )
       **** Inherited members ****
           * Object:
                 o create
                 o data
                 o delete
+                o deliver_to
                 o json
                 o make_public
+                o tombstone
   class Base (model:Â Union
   [ActivityModel,Â ActorModel,Â CollectionModel,Â LinkModel,Â ObjectModel],
   input_json:Â dict, default_languages:Â listÂ =Â ['en', 'en-US'])
       Base extends default functions to all other classes.
         Expand source code
       class Base:
           """
@@ -640,26 +759,119 @@
       class Collection(Object):
           """
           Collection data and associated functions.
           """
 
           # Core type
           core_type = "Collection"
+
+          def add(self, object: Object = None):
+              """
+              Add an Object to the Collection.
+              """
+              if object._internal_data() == {}:
+                  raise ValueError("Cannot add an empty Object.")
+
+              # Use the items or ordered_items fields
+              if "items" in self._internal_data():
+                  self.items.insert(0, object.data())
+                  items_count = len(self.items)
+              elif "ordered_items" in self._internal_data():
+                  self.ordered_items.insert(0, object.data())
+                  items_count = len(self.ordered_items)
+
+              # Update total items
+              self.total_items = items_count
+
+          def remove(self, object: Object = None):
+              """
+              Remove an Object from the Collection.
+              The Object must have an ID.
+              """
+              if object._internal_data() == {}:
+                  raise ValueError("Cannot remove an empty Object.")
+              if object.id is None:
+                  raise ValueError("Cannot remove an Object without an ID.")
+
+              # Use the items or ordered_items fields
+              if "items" in self._internal_data():
+                  self.items = [i for i in self.items if "id" in i and i["id"]
+      != object.id]
+                  items_count = len(self.items)
+              elif "ordered_items" in self._internal_data():
+                  self.ordered_items = [
+                      i for i in self.ordered_items if "id" in i and i["id"] !=
+      object.id
+                  ]
+                  items_count = len(self.ordered_items)
+
+              # Update total items
+              self.total_items = items_count
       **** Ancestors ****
           * Object
           * Base
       **** Class variables ****
         var core_type
+      **** Methods ****
+        def add(self, object:Â ObjectÂ =Â None)
+            Add an Object to the Collection.
+              Expand source code
+            def add(self, object: Object = None):
+                """
+                Add an Object to the Collection.
+                """
+                if object._internal_data() == {}:
+                    raise ValueError("Cannot add an empty Object.")
+
+                # Use the items or ordered_items fields
+                if "items" in self._internal_data():
+                    self.items.insert(0, object.data())
+                    items_count = len(self.items)
+                elif "ordered_items" in self._internal_data():
+                    self.ordered_items.insert(0, object.data())
+                    items_count = len(self.ordered_items)
+
+                # Update total items
+                self.total_items = items_count
+        def remove(self, object:Â ObjectÂ =Â None)
+            Remove an Object from the Collection. The Object must have an ID.
+              Expand source code
+            def remove(self, object: Object = None):
+                """
+                Remove an Object from the Collection.
+                The Object must have an ID.
+                """
+                if object._internal_data() == {}:
+                    raise ValueError("Cannot remove an empty Object.")
+                if object.id is None:
+                    raise ValueError("Cannot remove an Object without an ID.")
+
+                # Use the items or ordered_items fields
+                if "items" in self._internal_data():
+                    self.items = [i for i in self.items if "id" in i and i
+            ["id"] != object.id]
+                    items_count = len(self.items)
+                elif "ordered_items" in self._internal_data():
+                    self.ordered_items = [
+                        i for i in self.ordered_items if "id" in i and i["id"]
+            != object.id
+                    ]
+                    items_count = len(self.ordered_items)
+
+                # Update total items
+                self.total_items = items_count
       **** Inherited members ****
           * Object:
                 o create
                 o data
                 o delete
+                o deliver_to
                 o json
                 o make_public
+                o tombstone
   class Link (model:Â Union
   [ActivityModel,Â ActorModel,Â CollectionModel,Â LinkModel,Â ObjectModel],
   input_json:Â dict, default_languages:Â listÂ =Â ['en', 'en-US'])
       Link data and associated functions.
         Expand source code
       class Link(Base):
           """
@@ -692,36 +904,103 @@
           def make_public(self):
               """
               Remove any fields (bto and bcc) that should not be public.
               """
               self.bto = None
               self.bcc = None
 
+          def deliver_to(self, depth: int = 2):
+              """
+              Recursively iterate to determine the audience.
+              Use depth to set how deep the recursion should go.
+              Some IDs may indicate collections, which must be handled
+      differently.
+              """
+              audience_fields = ["to", "bto", "cc", "bcc", "audience"]
+              audience_members = []
+              delivery_objects = [self._internal_data()]
+              current_depth = 0
+
+              # Iterate checking for the existence of delivery objects and our
+      depth
+              while current_depth <= depth and len(delivery_objects) > 0:
+                  new_delivery_objects = []
+                  for o in delivery_objects:
+                      for k, v in o.items():
+                          if k in audience_fields and v:
+                              audience_members += v
+
+                          # If the key is an object, add it to the delivery
+      objects
+                          elif isinstance(v, dict) and v:
+                              new_delivery_objects.append(v)
+
+                  # Set the new delivery objects
+                  delivery_objects = new_delivery_objects
+
+                  # Increase the delivery depth before looping again
+                  current_depth += 1
+
+              # Get the id of each audience member and remove duplicates
+              audience_members = [
+                  str(a["id"]) if isinstance(a, dict) and "id" in a else str(a)
+                  for a in audience_members
+              ]
+              audience_members = list(set(audience_members))
+
+              # Return the audience members
+              return audience_members
+
           def create(self):
               """
               Produce a new Activity of type Create with this Object.
+              After insertion into database, add an ID.
               """
               if self._internal_data() == {}:
-                  raise ValueError("Cannot Create an empty Object.")
+                  raise ValueError("Cannot create an empty Object.")
               return get_class(
                   {
                       "type": "Create",
+                      "actor": self.actor,
                       "object": self._internal_data(),
                       "to": self.to,
                       "bto": self.bto,
                       "cc": self.cc,
                       "bcc": self.bcc,
                       "audience": self.audience,
                       "published": datetime.now(),
                   }
               )
 
           def delete(self):
               """
-              Produce a new Tombstone of this Object.
+              Produce a new Activity of type Delete with this Object.
+              Only provide an ID and published time for the Object.
+              After insertion into database, add an ID.
+              """
+              return get_class(
+                  {
+                      "type": "Delete",
+                      "actor": self.actor,
+                      "object": {
+                          "id": self.id,
+                          "published": self.published,
+                      },
+                      "to": self.to,
+                      "bto": self.bto,
+                      "cc": self.cc,
+                      "bcc": self.bcc,
+                      "audience": self.audience,
+                      "published": datetime.now(),
+                  }
+              )
+
+          def tombstone(self):
+              """
+              Produce a new Tombstone.
               """
               return get_class(
                   {
                       "type": "Tombstone",
                       "id": self.id,
                       "published": self.published,
                       "updated": datetime.now(),
@@ -734,59 +1013,136 @@
           * Activity
           * Actor
           * Collection
       **** Class variables ****
         var core_type
       **** Methods ****
         def create(self)
-            Produce a new Activity of type Create with this Object.
+            Produce a new Activity of type Create with this Object. After
+            insertion into database, add an ID.
               Expand source code
             def create(self):
                 """
                 Produce a new Activity of type Create with this Object.
+                After insertion into database, add an ID.
                 """
                 if self._internal_data() == {}:
-                    raise ValueError("Cannot Create an empty Object.")
+                    raise ValueError("Cannot create an empty Object.")
                 return get_class(
                     {
                         "type": "Create",
+                        "actor": self.actor,
                         "object": self._internal_data(),
                         "to": self.to,
                         "bto": self.bto,
                         "cc": self.cc,
                         "bcc": self.bcc,
                         "audience": self.audience,
                         "published": datetime.now(),
                     }
                 )
         def delete(self)
-            Produce a new Tombstone of this Object.
+            Produce a new Activity of type Delete with this Object. Only
+            provide an ID and published time for the Object. After insertion
+            into database, add an ID.
               Expand source code
             def delete(self):
                 """
-                Produce a new Tombstone of this Object.
+                Produce a new Activity of type Delete with this Object.
+                Only provide an ID and published time for the Object.
+                After insertion into database, add an ID.
                 """
                 return get_class(
                     {
-                        "type": "Tombstone",
-                        "id": self.id,
-                        "published": self.published,
-                        "updated": datetime.now(),
-                        "deleted": datetime.now(),
+                        "type": "Delete",
+                        "actor": self.actor,
+                        "object": {
+                            "id": self.id,
+                            "published": self.published,
+                        },
+                        "to": self.to,
+                        "bto": self.bto,
+                        "cc": self.cc,
+                        "bcc": self.bcc,
+                        "audience": self.audience,
+                        "published": datetime.now(),
                     }
                 )
+        def deliver_to(self, depth:Â intÂ =Â 2)
+            Recursively iterate to determine the audience. Use depth to set how
+            deep the recursion should go. Some IDs may indicate collections,
+            which must be handled differently.
+              Expand source code
+            def deliver_to(self, depth: int = 2):
+                """
+                Recursively iterate to determine the audience.
+                Use depth to set how deep the recursion should go.
+                Some IDs may indicate collections, which must be handled
+            differently.
+                """
+                audience_fields = ["to", "bto", "cc", "bcc", "audience"]
+                audience_members = []
+                delivery_objects = [self._internal_data()]
+                current_depth = 0
+
+                # Iterate checking for the existence of delivery objects and
+            our depth
+                while current_depth <= depth and len(delivery_objects) > 0:
+                    new_delivery_objects = []
+                    for o in delivery_objects:
+                        for k, v in o.items():
+                            if k in audience_fields and v:
+                                audience_members += v
+
+                            # If the key is an object, add it to the delivery
+            objects
+                            elif isinstance(v, dict) and v:
+                                new_delivery_objects.append(v)
+
+                    # Set the new delivery objects
+                    delivery_objects = new_delivery_objects
+
+                    # Increase the delivery depth before looping again
+                    current_depth += 1
+
+                # Get the id of each audience member and remove duplicates
+                audience_members = [
+                    str(a["id"]) if isinstance(a, dict) and "id" in a else str
+            (a)
+                    for a in audience_members
+                ]
+                audience_members = list(set(audience_members))
+
+                # Return the audience members
+                return audience_members
         def make_public(self)
             Remove any fields (bto and bcc) that should not be public.
               Expand source code
             def make_public(self):
                 """
                 Remove any fields (bto and bcc) that should not be public.
                 """
                 self.bto = None
                 self.bcc = None
+        def tombstone(self)
+            Produce a new Tombstone.
+              Expand source code
+            def tombstone(self):
+                """
+                Produce a new Tombstone.
+                """
+                return get_class(
+                    {
+                        "type": "Tombstone",
+                        "id": self.id,
+                        "published": self.published,
+                        "updated": datetime.now(),
+                        "deleted": datetime.now(),
+                    }
+                )
       **** Inherited members ****
           * Base:
                 o data
                 o json
 
 ****** Index ******
     * **** Super-module ****
@@ -795,23 +1151,27 @@
           o get_class
           o get_class_from_model
     * **** Classes ****
           o *** Activity ***
                 # core_type
                 # undo
           o *** Actor ***
-                # act
+                # activity
                 # core_type
           o *** Base ***
                 # data
                 # json
           o *** Collection ***
+                # add
                 # core_type
+                # remove
           o *** Link ***
                 # core_type
           o *** Object ***
                 # core_type
                 # create
                 # delete
+                # deliver_to
                 # make_public
+                # tombstone
 
 Generated by pdoc0.10.0.
```

### Comparing `activitypubdantic-0.0.2/docs/get_model.html` & `activitypubdantic-0.0.3/docs/get_model.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/docs/index.html` & `activitypubdantic-0.0.3/docs/index.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/docs/models/activity.html` & `activitypubdantic-0.0.3/docs/models/activity.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/docs/models/actor.html` & `activitypubdantic-0.0.3/docs/models/actor.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/docs/models/core.html` & `activitypubdantic-0.0.3/docs/models/core.html`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
     _link_list_no_spaces_or_commas = field_validator(&#34;rel&#34;, mode=&#34;before&#34;)(
         validate_list_no_spaces_or_commas
     )
     _link_list_links_or_objects = field_validator(&#34;preview&#34;, mode=&#34;before&#34;)(
         validate_list_links_or_objects
     )
 
-    # Initialize with an optional positional argument for id
+    # Initialize with an optional positional argument for href
     def __init__(self, href: HttpUrl = None, **kwargs) -&gt; None:
         if href:
             super(LinkModel, self).__init__(href=href, **kwargs)
         else:
             super(LinkModel, self).__init__(**kwargs)
 
 
@@ -1556,15 +1556,15 @@
     _link_list_no_spaces_or_commas = field_validator(&#34;rel&#34;, mode=&#34;before&#34;)(
         validate_list_no_spaces_or_commas
     )
     _link_list_links_or_objects = field_validator(&#34;preview&#34;, mode=&#34;before&#34;)(
         validate_list_links_or_objects
     )
 
-    # Initialize with an optional positional argument for id
+    # Initialize with an optional positional argument for href
     def __init__(self, href: HttpUrl = None, **kwargs) -&gt; None:
         if href:
             super(LinkModel, self).__init__(href=href, **kwargs)
         else:
             super(LinkModel, self).__init__(**kwargs)</code></pre>
 </details>
 <h3>Ancestors</h3>
```

#### html2text {}

```diff
@@ -482,15 +482,15 @@
     _link_list_no_spaces_or_commas = field_validator("rel", mode="before")(
         validate_list_no_spaces_or_commas
     )
     _link_list_links_or_objects = field_validator("preview", mode="before")(
         validate_list_links_or_objects
     )
 
-    # Initialize with an optional positional argument for id
+    # Initialize with an optional positional argument for href
     def __init__(self, href: HttpUrl = None, **kwargs) -> None:
         if href:
             super(LinkModel, self).__init__(href=href, **kwargs)
         else:
             super(LinkModel, self).__init__(**kwargs)
 
 
@@ -1273,15 +1273,15 @@
               validate_list_no_spaces_or_commas
           )
           _link_list_links_or_objects = field_validator("preview",
       mode="before")(
               validate_list_links_or_objects
           )
 
-          # Initialize with an optional positional argument for id
+          # Initialize with an optional positional argument for href
           def __init__(self, href: HttpUrl = None, **kwargs) -> None:
               if href:
                   super(LinkModel, self).__init__(href=href, **kwargs)
               else:
                   super(LinkModel, self).__init__(**kwargs)
       **** Ancestors ****
           * CoreModel
```

### Comparing `activitypubdantic-0.0.2/docs/models/index.html` & `activitypubdantic-0.0.3/docs/models/index.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/docs/models/link.html` & `activitypubdantic-0.0.3/docs/models/link.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/docs/models/object.html` & `activitypubdantic-0.0.3/docs/models/object.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/activitypub/create.json` & `activitypubdantic-0.0.3/json/activitypub/create.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/activitypub/person.json` & `activitypubdantic-0.0.3/json/activitypub/person.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/activitystreams/add.json` & `activitypubdantic-0.0.3/json/activitystreams/add.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/activitystreams/collection.json` & `activitypubdantic-0.0.3/json/activitystreams/collection.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/activitystreams/question.json` & `activitypubdantic-0.0.3/json/activitystreams/question.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/mastodon/accept.json` & `activitypubdantic-0.0.3/json/mastodon/accept.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/mastodon/create.json` & `activitypubdantic-0.0.3/json/mastodon/create.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/mastodon/person.json` & `activitypubdantic-0.0.3/json/mastodon/person.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/json/mastodon/poll.json` & `activitypubdantic-0.0.3/json/mastodon/poll.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/.gitignore` & `activitypubdantic-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/LICENSE` & `activitypubdantic-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.2/README.md` & `activitypubdantic-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 # ActivityPubdantic
 
+![CI](https://github.com/joewlos/activitypubdantic/actions/workflows/test.yaml/badge.svg?branch=main)
+[![PyPI version](https://badge.fury.io/py/activitypubdantic.svg)](https://badge.fury.io/py/activitypubdantic)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
+
 ### Validate and Interact with ActivityPub JSON
 
 [GitHub Repository](https://github.com/joewlos/activitypubdantic)
 
 [ActivityPubdantic Documentation](https://www.joewlos.com/activitypubdantic/)
 
 [ActivityPub Protocol](https://www.w3.org/TR/activitypub/)
 
 [ActivityStreams Specification](https://www.w3.org/TR/activitystreams-vocabulary/)
 
-## Development Note
-
-The current version of **ActivityPubdantic** available on PyPi is still undergoing testing and upgrades. If you plan to use **ActivityPubdantic** in your project, please keep in mind that its features and capabilities are likely to evolve and grow. Please see the [contributing](#contributing) section of this README for further information about **ActivityPubdantic**'s development.
-
 ## What Is ActivityPubdantic?
 
 **ActivityPubdantic** is a suite of tools for validating ActivityPub JSON and constructing consistent representations of ActivityPub notifications and content. [Pydantic](https://docs.pydantic.dev/latest/) models enable the validation logic and can be imported for use in custom-coded classes or FastAPI routes.
 
 ## Why Does ActivityPub JSON Require Validation?
 
-[ActivityPub](https://www.w3.org/TR/activitypub/) is a protocol for decentralized social networking. It defines client-to-server and server-to-server interactions and relies on [ActivityStreams](https://www.w3.org/TR/activitystreams-vocabulary/#dfn-orderedcollection) for its vocabulary. Many of the protocol's definitions are purposefully unrestrictive, giving developers the freedom to implement only the features relevant to their products or to adjust to meet their particular requirements.
+[ActivityPub](https://www.w3.org/TR/activitypub/) is a protocol for decentralized social networking. It defines client-to-server and server-to-server interactions and relies on [ActivityStreams](https://www.w3.org/TR/activitystreams-vocabulary/#dfn-orderedcollection) for its vocabulary. Many of the protocol's specifications are purposefully unrestrictive, giving developers the freedom to implement only the features relevant to their products or to adjust to meet their particular requirements.
 
-However, that flexibility presents challenges for assessing data validity and simplifying developers' code. **ActivityPubdantic** helps solve those challenges by using ActivityPub's "type" field to identify proper checks for other fields and standardize their structures. [Examples](#examples) are available in the sections below.
+However, that flexibility presents challenges for assessing data validity and simplifying developers' code. **ActivityPubdantic** helps developers overcome those challenges by using ActivityPub's `type` field to identify proper checks for other fields and standardize their structures. [Examples](https://github.com/joewlos/activitypubdantic/tree/main#examples) are available in the sections below.
 
-[Mastodon](https://docs.joinmastodon.org/spec/activitypub/) supports ActivityPub, and Meta's [Threads](https://apps.apple.com/us/app/threads-an-instagram-app/id6446901002) app plans to conform to the protocol sometime in the [near future](https://techcrunch.com/2023/07/05/adam-mosseri-says-metas-threads-app-wont-have-activitypub-support-at-launch/). **ActivityPubdantic** includes a test suite, which uses examples from ActivityPub, ActivityStreams, and Mastodon to test its parsing and validation. As Threads and other platforms implement ActivityPub, those tests (and more broadly, this package) will be updated to stay current.
+[Mastodon](https://docs.joinmastodon.org/spec/activitypub/) supports ActivityPub, and Meta's [Threads](https://apps.apple.com/us/app/threads-an-instagram-app/id6446901002) app plans to conform to the protocol sometime in the [near future](https://techcrunch.com/2023/07/05/adam-mosseri-says-metas-threads-app-wont-have-activitypub-support-at-launch/). **ActivityPubdantic** includes a `pytest` script, which uses examples from ActivityPub, ActivityStreams, and Mastodon to test its parsing and validation. As Threads and other platforms implement ActivityPub, those tests (and more broadly, this package) will be updated to stay current.
 
 ## Installation
 
-Install the package with `pip`:
+Install **ActivityPubdantic** with `pip`:
 
 ```console
 pip install activitypubdantic
 ```
 
-Most developer use cases will use one or both of the following import statements:
+Most developer use cases will require one or both of the following import statements, which serve different purposes:
 
 ```python
 # Use classes for validation and common operations
 import activitypubdantic as ap
 
 # Use models in FastAPI routes
 from activitypubdantic.models import *
 ```
 
 ## Examples
 
-The following examples include simple use cases and code snippets for **ActivityPubdantic**. For a more thorough listing of **ActivityPubdantic's** classes, functions, and models, check out its [documentation](https://www.joewlos.com/activitypubdantic/).
+The following examples include simple use cases and code snippets for **ActivityPubdantic**. For a more thorough listing of **ActivityPubdantic**'s classes, functions, and models, check out its [documentation](https://www.joewlos.com/activitypubdantic/).
 
 ### Parsing Activity, Collection, Link, and Object JSON
 
 `Activities`, `Collections`, `Links`, and `Objects` are the core concepts around which ActivityPub and ActivityStreams are built. By reducing their complexity and standardizing their representation, **ActivityPubdantic** helps resolve potential pain points for developers.
 
-ActivityPub's protocol includes an [example](https://www.w3.org/TR/activitypub/#client-to-server-interactions) of a `Like` activity. The example's `to` field is a list, while its `cc` field is a string. Both formats are valid, but they require slightly different handling in subsequent lines of code. To resolve that difference, **ActivityPubdantic** rewrites it, so those fields are always presented as lists of dictionaries.
+ActivityPub's protocol includes an [example](https://www.w3.org/TR/activitypub/#client-to-server-interactions) of a `Like` activity. The example's `to` field is a list, while its `cc` field is a string. Both formats are valid, but they require slightly different handling in subsequent lines of code. To resolve that difference, **ActivityPubdantic** copies and rewrites the JSON, so those fields are always represented as lists of dictionaries.
 
 ```python
 import activitypubdantic as ap
 
 # Example JSON from ActivityPub documentation
 example_json = {
   "@context": ["https://www.w3.org/ns/activitystreams",
@@ -75,17 +76,17 @@
 output_class = ap.get_class(example_json)
 
 # Produce the parsed and validated JSON string
 output_json = output_class.json()
 print(output_json)  # See JSON below
 ```
 
-`get_class()` reads the `example_json` and uses its type to select the applicable Pydantic model. It then uses Pydantic validators for each field to assert they comply with the protocol and then restructures them.
+`get_class()` reads the `example_json` and uses its type to select the applicable Pydantic model. That model then uses validators for each field to assert they comply with the protocol and then restructures them.
 
-The `output_json` is longer and, at first glance, more complex. But because it contains types for each item in its fields and it standardizes the structures of similar fields – like `to` and `cc` – it is more descriptive and easier to consistently manipulate.
+The `output_json` is longer and, at first glance, more difficult to read. But because it contains types for each item in its fields and it standardizes the structures of similar fields – like `to` and `cc` – it is more descriptive and easier to consistently manipulate.
 
 ```json
 {
   "@context": [
     "https://www.w3.org/ns/activitystreams",
     {
       "@language": "en"
@@ -128,23 +129,23 @@
     "@context": "https://www.w3.org/ns/activitystreams",
     "type": "Object",
     "id": "https://rhiaro.co.uk/2016/05/minimal-activitypub"
   }
 }
 ```
 
-However, not every project requires this degree of granularity. For example, some servers may already have logic that ignores additional fields and only iterates through `id` URLs in the JSON.
+However, not every project requires that degree of granularity. For example, some servers may already have logic that ignores additional fields and only iterates through `id` URLs in the JSON.
 
 ```python
 # Use the verbose keyword argument
 short_output_json = output_class.json(verbose=False)
 print(short_output_json)  # See JSON below
 ```
 
-Setting `verbose=False` shortens the output, retaining consistency but eliminating unneeded data for simpler implementations.
+Setting `verbose=False` shortens the output, retaining consistency but eliminating unneeded data for more concise tasks.
 
 ```json
 {
   "@context": [
     "https://www.w3.org/ns/activitystreams",
     {
       "@language": "en"
@@ -161,50 +162,50 @@
   "actor": ["https://dustycloud.org/chris/"],
   "object": "https://rhiaro.co.uk/2016/05/minimal-activitypub"
 }
 ```
 
 ### Validating FastAPI Request Bodies
 
-[FastAPI](https://fastapi.tiangolo.com/) uses Pydantic models to validate [request bodies](https://fastapi.tiangolo.com/tutorial/body/). After importing **ActivityPubdantic** models directly, developers can automatically validate requests and then use the `get_class_from_model()` function to smoothly interact with the ActivityPub JSON.
+[FastAPI](https://fastapi.tiangolo.com/) uses Pydantic models to validate [request bodies](https://fastapi.tiangolo.com/tutorial/body/). After importing **ActivityPubdantic** models directly, developers can automatically validate requests and then use the `get_class_from_model()` function to smoothly interact with ActivityPub JSON.
 
 When the same `Like` activity is sent in the POST request to `/outbox`, the request body is validated by FastAPI and loaded into an **ActivityPubdantic** class to produce clean JSON.
 
 ```python
 import activitypubdantic as ap
 from activitypubdantic.models import *
 from fastapi import FastAPI, Response
 
 app = FastAPI()
 
 # Route for an ActivityPub outbox
 @app.post("/outbox", status_code=201)
 async def outbox(activity: ActivityModel, response: Response):
 
-    # Initialize the class and perform relevant operations
+    # Initialize the class and perform relevant data manipulations
     activity_class = ap.get_class_from_model(activity)
     activity_class.make_public()
 
-    # Save the JSON in this user's outbox collection in the database
+    # Save the JSON in the outbox in the database
     print(activity_class.json())
 
-    # Use the class's type to set the header
+    # Use the type to set the header
     response.headers["Location"] = "https://example.com/{0}/{1}".format(
         activity_class.type.lower(),
         1,  # ID should come from the database
     )
 
     # Return with header and status code
     return
 ```
 
-Methods – like `make_public()` – perform common operations on the data. In this case, `make_public()` removes the `bto` and `bcc` attributes from the class instance, if they exist. Additionally, the class instance helps specify a location in the response header, per the ActivityPub [documentation](https://www.w3.org/TR/activitypub/#client-to-server-interactions) for client-to-server interactions.
+Methods – like `make_public()` – perform common operations on the data. In this case, `make_public()` removes the `bto` and `bcc` attributes from the class instance, if they exist. Additionally, the `type` attribute specifies a location in the response header, per the ActivityPub [documentation](https://www.w3.org/TR/activitypub/#client-to-server-interactions) for client-to-server interactions.
 
 ## Contributing
 
 **ActivityPubdantic** is still a work in progress. If you find it valuable for your project but notice bugs, need changes, or require additional features or support for other ActivityPub platforms, [open an issue](https://github.com/joewlos/activitypubdantic/issues) or fork to [start a PR](https://github.com/joewlos/activitypubdantic/pulls).
 
-The `developer_requirements.txt` file includes all of the packages your virtual environment needs to start, including `pdoc3` for generating new documentation and `pytest` for unit tests.
+The `developer_requirements.txt` file includes all of the packages your virtual environment needs, including `pdoc3` for generating new documentation, `black` for formatting, and `pytest` for unit tests.
 
-Keep in mind, all PRs require GitHub to successfully run the test suite, so if you significantly change **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
+Keep in mind, all PRs require a successful run of the GitHub Workflow for testing, so if you significantly change **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
 
 Thank you for your interest!
```

### Comparing `activitypubdantic-0.0.2/pyproject.toml` & `activitypubdantic-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "activitypubdantic"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Joe Wlos", email="joewlos17@gmail.com" },
 ]
 description = "Pydantic Models for ActivityPub with Classes for Enabling Interactions"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["pydantic>=2.0.2"]
+dependencies = ["pydantic==2.0.3"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `activitypubdantic-0.0.2/PKG-INFO` & `activitypubdantic-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 Metadata-Version: 2.1
 Name: activitypubdantic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pydantic Models for ActivityPub with Classes for Enabling Interactions
 Project-URL: Homepage, https://github.com/joewlos/activitypubdantic
 Project-URL: Documentation, https://www.joewlos.com/activitypubdantic/
 Author-email: Joe Wlos <joewlos17@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: pydantic>=2.0.2
+Requires-Dist: pydantic==2.0.3
 Description-Content-Type: text/markdown
 
 # ActivityPubdantic
 
+![CI](https://github.com/joewlos/activitypubdantic/actions/workflows/test.yaml/badge.svg?branch=main)
+[![PyPI version](https://badge.fury.io/py/activitypubdantic.svg)](https://badge.fury.io/py/activitypubdantic)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
+
 ### Validate and Interact with ActivityPub JSON
 
 [GitHub Repository](https://github.com/joewlos/activitypubdantic)
 
 [ActivityPubdantic Documentation](https://www.joewlos.com/activitypubdantic/)
 
 [ActivityPub Protocol](https://www.w3.org/TR/activitypub/)
 
 [ActivityStreams Specification](https://www.w3.org/TR/activitystreams-vocabulary/)
 
-## Development Note
-
-The current version of **ActivityPubdantic** available on PyPi is still undergoing testing and upgrades. If you plan to use **ActivityPubdantic** in your project, please keep in mind that its features and capabilities are likely to evolve and grow. Please see the [contributing](#contributing) section of this README for further information about **ActivityPubdantic**'s development.
-
 ## What Is ActivityPubdantic?
 
 **ActivityPubdantic** is a suite of tools for validating ActivityPub JSON and constructing consistent representations of ActivityPub notifications and content. [Pydantic](https://docs.pydantic.dev/latest/) models enable the validation logic and can be imported for use in custom-coded classes or FastAPI routes.
 
 ## Why Does ActivityPub JSON Require Validation?
 
-[ActivityPub](https://www.w3.org/TR/activitypub/) is a protocol for decentralized social networking. It defines client-to-server and server-to-server interactions and relies on [ActivityStreams](https://www.w3.org/TR/activitystreams-vocabulary/#dfn-orderedcollection) for its vocabulary. Many of the protocol's definitions are purposefully unrestrictive, giving developers the freedom to implement only the features relevant to their products or to adjust to meet their particular requirements.
+[ActivityPub](https://www.w3.org/TR/activitypub/) is a protocol for decentralized social networking. It defines client-to-server and server-to-server interactions and relies on [ActivityStreams](https://www.w3.org/TR/activitystreams-vocabulary/#dfn-orderedcollection) for its vocabulary. Many of the protocol's specifications are purposefully unrestrictive, giving developers the freedom to implement only the features relevant to their products or to adjust to meet their particular requirements.
 
-However, that flexibility presents challenges for assessing data validity and simplifying developers' code. **ActivityPubdantic** helps solve those challenges by using ActivityPub's "type" field to identify proper checks for other fields and standardize their structures. [Examples](#examples) are available in the sections below.
+However, that flexibility presents challenges for assessing data validity and simplifying developers' code. **ActivityPubdantic** helps developers overcome those challenges by using ActivityPub's `type` field to identify proper checks for other fields and standardize their structures. [Examples](https://github.com/joewlos/activitypubdantic/tree/main#examples) are available in the sections below.
 
-[Mastodon](https://docs.joinmastodon.org/spec/activitypub/) supports ActivityPub, and Meta's [Threads](https://apps.apple.com/us/app/threads-an-instagram-app/id6446901002) app plans to conform to the protocol sometime in the [near future](https://techcrunch.com/2023/07/05/adam-mosseri-says-metas-threads-app-wont-have-activitypub-support-at-launch/). **ActivityPubdantic** includes a test suite, which uses examples from ActivityPub, ActivityStreams, and Mastodon to test its parsing and validation. As Threads and other platforms implement ActivityPub, those tests (and more broadly, this package) will be updated to stay current.
+[Mastodon](https://docs.joinmastodon.org/spec/activitypub/) supports ActivityPub, and Meta's [Threads](https://apps.apple.com/us/app/threads-an-instagram-app/id6446901002) app plans to conform to the protocol sometime in the [near future](https://techcrunch.com/2023/07/05/adam-mosseri-says-metas-threads-app-wont-have-activitypub-support-at-launch/). **ActivityPubdantic** includes a `pytest` script, which uses examples from ActivityPub, ActivityStreams, and Mastodon to test its parsing and validation. As Threads and other platforms implement ActivityPub, those tests (and more broadly, this package) will be updated to stay current.
 
 ## Installation
 
-Install the package with `pip`:
+Install **ActivityPubdantic** with `pip`:
 
 ```console
 pip install activitypubdantic
 ```
 
-Most developer use cases will use one or both of the following import statements:
+Most developer use cases will require one or both of the following import statements, which serve different purposes:
 
 ```python
 # Use classes for validation and common operations
 import activitypubdantic as ap
 
 # Use models in FastAPI routes
 from activitypubdantic.models import *
 ```
 
 ## Examples
 
-The following examples include simple use cases and code snippets for **ActivityPubdantic**. For a more thorough listing of **ActivityPubdantic's** classes, functions, and models, check out its [documentation](https://www.joewlos.com/activitypubdantic/).
+The following examples include simple use cases and code snippets for **ActivityPubdantic**. For a more thorough listing of **ActivityPubdantic**'s classes, functions, and models, check out its [documentation](https://www.joewlos.com/activitypubdantic/).
 
 ### Parsing Activity, Collection, Link, and Object JSON
 
 `Activities`, `Collections`, `Links`, and `Objects` are the core concepts around which ActivityPub and ActivityStreams are built. By reducing their complexity and standardizing their representation, **ActivityPubdantic** helps resolve potential pain points for developers.
 
-ActivityPub's protocol includes an [example](https://www.w3.org/TR/activitypub/#client-to-server-interactions) of a `Like` activity. The example's `to` field is a list, while its `cc` field is a string. Both formats are valid, but they require slightly different handling in subsequent lines of code. To resolve that difference, **ActivityPubdantic** rewrites it, so those fields are always presented as lists of dictionaries.
+ActivityPub's protocol includes an [example](https://www.w3.org/TR/activitypub/#client-to-server-interactions) of a `Like` activity. The example's `to` field is a list, while its `cc` field is a string. Both formats are valid, but they require slightly different handling in subsequent lines of code. To resolve that difference, **ActivityPubdantic** copies and rewrites the JSON, so those fields are always represented as lists of dictionaries.
 
 ```python
 import activitypubdantic as ap
 
 # Example JSON from ActivityPub documentation
 example_json = {
   "@context": ["https://www.w3.org/ns/activitystreams",
@@ -90,17 +91,17 @@
 output_class = ap.get_class(example_json)
 
 # Produce the parsed and validated JSON string
 output_json = output_class.json()
 print(output_json)  # See JSON below
 ```
 
-`get_class()` reads the `example_json` and uses its type to select the applicable Pydantic model. It then uses Pydantic validators for each field to assert they comply with the protocol and then restructures them.
+`get_class()` reads the `example_json` and uses its type to select the applicable Pydantic model. That model then uses validators for each field to assert they comply with the protocol and then restructures them.
 
-The `output_json` is longer and, at first glance, more complex. But because it contains types for each item in its fields and it standardizes the structures of similar fields – like `to` and `cc` – it is more descriptive and easier to consistently manipulate.
+The `output_json` is longer and, at first glance, more difficult to read. But because it contains types for each item in its fields and it standardizes the structures of similar fields – like `to` and `cc` – it is more descriptive and easier to consistently manipulate.
 
 ```json
 {
   "@context": [
     "https://www.w3.org/ns/activitystreams",
     {
       "@language": "en"
@@ -143,23 +144,23 @@
     "@context": "https://www.w3.org/ns/activitystreams",
     "type": "Object",
     "id": "https://rhiaro.co.uk/2016/05/minimal-activitypub"
   }
 }
 ```
 
-However, not every project requires this degree of granularity. For example, some servers may already have logic that ignores additional fields and only iterates through `id` URLs in the JSON.
+However, not every project requires that degree of granularity. For example, some servers may already have logic that ignores additional fields and only iterates through `id` URLs in the JSON.
 
 ```python
 # Use the verbose keyword argument
 short_output_json = output_class.json(verbose=False)
 print(short_output_json)  # See JSON below
 ```
 
-Setting `verbose=False` shortens the output, retaining consistency but eliminating unneeded data for simpler implementations.
+Setting `verbose=False` shortens the output, retaining consistency but eliminating unneeded data for more concise tasks.
 
 ```json
 {
   "@context": [
     "https://www.w3.org/ns/activitystreams",
     {
       "@language": "en"
@@ -176,50 +177,50 @@
   "actor": ["https://dustycloud.org/chris/"],
   "object": "https://rhiaro.co.uk/2016/05/minimal-activitypub"
 }
 ```
 
 ### Validating FastAPI Request Bodies
 
-[FastAPI](https://fastapi.tiangolo.com/) uses Pydantic models to validate [request bodies](https://fastapi.tiangolo.com/tutorial/body/). After importing **ActivityPubdantic** models directly, developers can automatically validate requests and then use the `get_class_from_model()` function to smoothly interact with the ActivityPub JSON.
+[FastAPI](https://fastapi.tiangolo.com/) uses Pydantic models to validate [request bodies](https://fastapi.tiangolo.com/tutorial/body/). After importing **ActivityPubdantic** models directly, developers can automatically validate requests and then use the `get_class_from_model()` function to smoothly interact with ActivityPub JSON.
 
 When the same `Like` activity is sent in the POST request to `/outbox`, the request body is validated by FastAPI and loaded into an **ActivityPubdantic** class to produce clean JSON.
 
 ```python
 import activitypubdantic as ap
 from activitypubdantic.models import *
 from fastapi import FastAPI, Response
 
 app = FastAPI()
 
 # Route for an ActivityPub outbox
 @app.post("/outbox", status_code=201)
 async def outbox(activity: ActivityModel, response: Response):
 
-    # Initialize the class and perform relevant operations
+    # Initialize the class and perform relevant data manipulations
     activity_class = ap.get_class_from_model(activity)
     activity_class.make_public()
 
-    # Save the JSON in this user's outbox collection in the database
+    # Save the JSON in the outbox in the database
     print(activity_class.json())
 
-    # Use the class's type to set the header
+    # Use the type to set the header
     response.headers["Location"] = "https://example.com/{0}/{1}".format(
         activity_class.type.lower(),
         1,  # ID should come from the database
     )
 
     # Return with header and status code
     return
 ```
 
-Methods – like `make_public()` – perform common operations on the data. In this case, `make_public()` removes the `bto` and `bcc` attributes from the class instance, if they exist. Additionally, the class instance helps specify a location in the response header, per the ActivityPub [documentation](https://www.w3.org/TR/activitypub/#client-to-server-interactions) for client-to-server interactions.
+Methods – like `make_public()` – perform common operations on the data. In this case, `make_public()` removes the `bto` and `bcc` attributes from the class instance, if they exist. Additionally, the `type` attribute specifies a location in the response header, per the ActivityPub [documentation](https://www.w3.org/TR/activitypub/#client-to-server-interactions) for client-to-server interactions.
 
 ## Contributing
 
 **ActivityPubdantic** is still a work in progress. If you find it valuable for your project but notice bugs, need changes, or require additional features or support for other ActivityPub platforms, [open an issue](https://github.com/joewlos/activitypubdantic/issues) or fork to [start a PR](https://github.com/joewlos/activitypubdantic/pulls).
 
-The `developer_requirements.txt` file includes all of the packages your virtual environment needs to start, including `pdoc3` for generating new documentation and `pytest` for unit tests.
+The `developer_requirements.txt` file includes all of the packages your virtual environment needs, including `pdoc3` for generating new documentation, `black` for formatting, and `pytest` for unit tests.
 
-Keep in mind, all PRs require GitHub to successfully run the test suite, so if you significantly change **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
+Keep in mind, all PRs require a successful run of the GitHub Workflow for testing, so if you significantly change **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
 
 Thank you for your interest!
```

