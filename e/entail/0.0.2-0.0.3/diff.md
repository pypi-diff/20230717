# Comparing `tmp/entail-0.0.2.tar.gz` & `tmp/entail-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entail-0.0.2.tar", last modified: Thu Jul 13 05:18:49 2023, max compression
+gzip compressed data, was "entail-0.0.3.tar", last modified: Mon Jul 17 06:21:27 2023, max compression
```

## Comparing `entail-0.0.2.tar` & `entail-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 05:18:49.704338 entail-0.0.2/
--rw-r--r--   0 haowu4     (501) staff       (20)      147 2023-07-13 05:18:49.704231 entail-0.0.2/PKG-INFO
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 05:18:49.703186 entail-0.0.2/entail/
--rw-r--r--   0 haowu4     (501) staff       (20)       87 2023-07-12 04:37:13.000000 entail-0.0.2/entail/__init__.py
--rw-r--r--   0 haowu4     (501) staff       (20)      117 2023-07-12 00:12:40.000000 entail-0.0.2/entail/chat.py
--rw-r--r--   0 haowu4     (501) staff       (20)     1858 2023-07-12 04:35:55.000000 entail-0.0.2/entail/config.py
--rw-r--r--   0 haowu4     (501) staff       (20)     4322 2023-07-13 05:17:22.000000 entail-0.0.2/entail/core.py
--rw-r--r--   0 haowu4     (501) staff       (20)     4520 2023-07-12 17:05:34.000000 entail-0.0.2/entail/env.py
--rw-r--r--   0 haowu4     (501) staff       (20)      625 2023-07-11 18:21:50.000000 entail-0.0.2/entail/main.py
--rw-r--r--   0 haowu4     (501) staff       (20)     2379 2023-07-12 18:38:59.000000 entail-0.0.2/entail/results.py
--rw-r--r--   0 haowu4     (501) staff       (20)     1321 2023-07-12 16:48:49.000000 entail-0.0.2/entail/utils.py
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 05:18:49.703808 entail-0.0.2/entail.egg-info/
--rw-r--r--   0 haowu4     (501) staff       (20)      147 2023-07-13 05:18:49.000000 entail-0.0.2/entail.egg-info/PKG-INFO
--rw-r--r--   0 haowu4     (501) staff       (20)      325 2023-07-13 05:18:49.000000 entail-0.0.2/entail.egg-info/SOURCES.txt
--rw-r--r--   0 haowu4     (501) staff       (20)        1 2023-07-13 05:18:49.000000 entail-0.0.2/entail.egg-info/dependency_links.txt
--rw-r--r--   0 haowu4     (501) staff       (20)       39 2023-07-13 05:18:49.000000 entail-0.0.2/entail.egg-info/requires.txt
--rw-r--r--   0 haowu4     (501) staff       (20)        7 2023-07-13 05:18:49.000000 entail-0.0.2/entail.egg-info/top_level.txt
--rw-r--r--   0 haowu4     (501) staff       (20)       38 2023-07-13 05:18:49.704379 entail-0.0.2/setup.cfg
--rw-r--r--   0 haowu4     (501) staff       (20)      348 2023-07-13 05:18:42.000000 entail-0.0.2/setup.py
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 05:18:49.704063 entail-0.0.2/tests/
--rw-r--r--   0 haowu4     (501) staff       (20)      191 2023-07-11 17:08:15.000000 entail-0.0.2/tests/test_e2e.py
--rw-r--r--   0 haowu4     (501) staff       (20)      195 2023-07-11 17:08:46.000000 entail-0.0.2/tests/test_loader.py
+drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-17 06:21:27.098401 entail-0.0.3/
+-rw-r--r--   0 haowu4     (501) staff       (20)      147 2023-07-17 06:21:27.098286 entail-0.0.3/PKG-INFO
+drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-17 06:21:27.096659 entail-0.0.3/entail/
+-rw-r--r--   0 haowu4     (501) staff       (20)       87 2023-07-12 04:37:13.000000 entail-0.0.3/entail/__init__.py
+-rw-r--r--   0 haowu4     (501) staff       (20)       53 2023-07-15 17:52:18.000000 entail-0.0.3/entail/assertion.py
+-rw-r--r--   0 haowu4     (501) staff       (20)     1858 2023-07-12 04:35:55.000000 entail-0.0.3/entail/config.py
+-rw-r--r--   0 haowu4     (501) staff       (20)     5009 2023-07-17 06:06:19.000000 entail-0.0.3/entail/core.py
+-rw-r--r--   0 haowu4     (501) staff       (20)     4548 2023-07-17 06:11:45.000000 entail-0.0.3/entail/env.py
+-rw-r--r--   0 haowu4     (501) staff       (20)      625 2023-07-11 18:21:50.000000 entail-0.0.3/entail/main.py
+-rw-r--r--   0 haowu4     (501) staff       (20)    10074 2023-07-17 06:20:13.000000 entail-0.0.3/entail/results.py
+-rw-r--r--   0 haowu4     (501) staff       (20)     1321 2023-07-12 16:48:49.000000 entail-0.0.3/entail/utils.py
+drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-17 06:21:27.097416 entail-0.0.3/entail.egg-info/
+-rw-r--r--   0 haowu4     (501) staff       (20)      147 2023-07-17 06:21:27.000000 entail-0.0.3/entail.egg-info/PKG-INFO
+-rw-r--r--   0 haowu4     (501) staff       (20)      352 2023-07-17 06:21:27.000000 entail-0.0.3/entail.egg-info/SOURCES.txt
+-rw-r--r--   0 haowu4     (501) staff       (20)        1 2023-07-17 06:21:27.000000 entail-0.0.3/entail.egg-info/dependency_links.txt
+-rw-r--r--   0 haowu4     (501) staff       (20)       39 2023-07-17 06:21:27.000000 entail-0.0.3/entail.egg-info/requires.txt
+-rw-r--r--   0 haowu4     (501) staff       (20)        7 2023-07-17 06:21:27.000000 entail-0.0.3/entail.egg-info/top_level.txt
+-rw-r--r--   0 haowu4     (501) staff       (20)       38 2023-07-17 06:21:27.098446 entail-0.0.3/setup.cfg
+-rw-r--r--   0 haowu4     (501) staff       (20)      348 2023-07-17 06:21:19.000000 entail-0.0.3/setup.py
+drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-17 06:21:27.098132 entail-0.0.3/tests/
+-rw-r--r--   0 haowu4     (501) staff       (20)      191 2023-07-11 17:08:15.000000 entail-0.0.3/tests/test_e2e.py
+-rw-r--r--   0 haowu4     (501) staff       (20)      195 2023-07-11 17:08:46.000000 entail-0.0.3/tests/test_loader.py
+-rw-r--r--   0 haowu4     (501) staff       (20)     5421 2023-07-17 06:05:26.000000 entail-0.0.3/tests/test_results.py
```

### Comparing `entail-0.0.2/entail/config.py` & `entail-0.0.3/entail/config.py`

 * *Files identical despite different names*

### Comparing `entail-0.0.2/entail/core.py` & `entail-0.0.3/entail/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,25 +44,38 @@
     def none_of(children: list['Hypothesis']):
         return Hypothesis(quantifier=Quantifier.none_of, children=children)
 
     @staticmethod
     def of(value: str):
         return Hypothesis(quantifier=None, value=value)
 
+    def to_str(self):
+        if self.quantifier == Quantifier.any_of:
+            children = "\n".join([c.to_str() for c in self.children])
+            return f"At least one of the following should be true: \n {children}"
+        elif self.quantifier == Quantifier.all_of:
+            children = "\n".join([c.to_str() for c in self.children])
+            return f"All of the following should be true: \n {children}"
+        elif self.quantifier == Quantifier.none_of:
+            children = "\n".join([c.to_str() for c in self.children])
+            return f"None of the following should be true: \n {children}"
+        else:
+            return self.value
+
 
 class Role(str, Enum):
     system = 'system'
     user = 'user'
     assistant = 'assistant'
     function = 'function'
 
 
 class Fn(BaseModel):
     name: str
-    args: dict
+    args: dict = Field(default_factory={})
 
 
 class Message(BaseModel):
     role: Role
     content: Optional[str] = None
     fn: Optional[Fn] = None
 
@@ -113,14 +126,15 @@
     history: chat history
     output: describe the desired output
     """
     name: Optional[str] = None
     description: Optional[str] = None
     tags: Optional[list[str]] = None
     external_info: Optional[dict] = None
+
     history: list[Message] = Field(default_factory=list)
     output: DesiredOutput = Field(default_factory=DesiredOutput)
     path: str = ''
 
 
 class RuleMatch(BaseModel):
     hypothesis: Hypothesis
```

### Comparing `entail-0.0.2/entail/env.py` & `entail-0.0.3/entail/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 
 from entail import ChatHandler, create_default_entailment, RunConfig, TestCase, utils, \
-    RuleMatch, Quantifier, Hypothesis
-from entail.results import TestResult, TestResults
+    RuleMatch, Quantifier, Hypothesis, Fn
+from entail.results import TestResult, TestResults, PRF1
 from entail.entailment import EntailmentModel
 
 
 @dataclass
 class NewTestEnv:
     handler: ChatHandler = None
     entailment: EntailmentModel = None
@@ -77,43 +77,42 @@
         else:
             todo = [t for t in self.tests]
 
         results = []
         for t in todo:
             ret = self.run_test(t)
             results.append(ret)
-        return TestResults(results=results)
+        return TestResults(results=results, config=self.config)
 
     def run_test(self, testcase: TestCase) -> TestResult:
+        reply = self.handler.response(testcase.history, external_information=testcase.external_info)
         result = TestResult(
             case=testcase,
+            reply=reply,
         )
-        reply = self.handler.response(testcase.history, external_information=testcase.external_info)
-        if reply.fn:
+
+        if testcase.output.should_call_function:
             if self.config.function:
                 result.compare_function(testcase.output.should_call_function, reply.fn)
-        elif reply.content:
+        else:
             if testcase.output.exact:
                 result.exact_match = testcase.output.exact == reply.content
             else:
                 if testcase.output.example:
                     if self.config.bleu:
                         result.bleu = utils.bleu(testcase.output.example, reply.content)
                     if self.config.rouge:
-                        result.rouge = utils.rouge(testcase.output.example, reply.content)
+                        result.rouge = PRF1(**utils.rouge(testcase.output.example, reply.content))
                     if self.config.meteor:
                         result.meteor = utils.meteor(testcase.output.example, reply.content)
-
                 if testcase.output.should_be:
                     if self.config.entail:
                         for hypothesis in testcase.output.should_be:
                             score = test_hypothesis(hypothesis, self.entailment, reply.content)
                             result.entails.append(RuleMatch(hypothesis=hypothesis, score=score))
-        else:
-            result.is_empty = True
 
         return result
 
 
 def test_hypothesis(hypothesis: Hypothesis, entailment: EntailmentModel, content: str):
     if hypothesis.quantifier == Quantifier.any_of:
         return max([test_hypothesis(x, entailment, content) for x in hypothesis.children])
```

### Comparing `entail-0.0.2/entail/main.py` & `entail-0.0.3/entail/main.py`

 * *Files identical despite different names*

### Comparing `entail-0.0.2/entail/utils.py` & `entail-0.0.3/entail/utils.py`

 * *Files identical despite different names*

