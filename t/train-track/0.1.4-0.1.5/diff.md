# Comparing `tmp/train_track-0.1.4.tar.gz` & `tmp/train_track-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "train_track-0.1.4.tar", last modified: Mon Feb 28 20:46:32 2022, max compression
+gzip compressed data, was "train_track-0.1.5.tar", last modified: Mon Jul 17 12:57:37 2023, max compression
```

## Comparing `train_track-0.1.4.tar` & `train_track-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 thierry   (1001) thierry   (1001)        0 2022-02-28 20:46:32.608546 train_track-0.1.4/
--rw-rw-r--   0 thierry   (1001) thierry   (1001)      112 2021-03-11 13:49:16.000000 train_track-0.1.4/.gitignore
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    35141 2021-03-11 13:49:16.000000 train_track-0.1.4/LICENSE
--rw-rw-r--   0 thierry   (1001) thierry   (1001)       16 2021-03-11 13:49:16.000000 train_track-0.1.4/MANIFEST.in
--rw-rw-r--   0 thierry   (1001) thierry   (1001)     2966 2022-02-28 20:46:32.608546 train_track-0.1.4/PKG-INFO
--rw-rw-r--   0 thierry   (1001) thierry   (1001)     1828 2022-02-28 20:44:55.000000 train_track-0.1.4/README.rst
--rw-rw-r--   0 thierry   (1001) thierry   (1001)        5 2022-02-28 20:45:11.000000 train_track-0.1.4/VERSION
--rw-rw-r--   0 thierry   (1001) thierry   (1001)      656 2021-03-11 13:49:16.000000 train_track-0.1.4/makefile
--rw-rw-r--   0 thierry   (1001) thierry   (1001)   171953 2021-03-11 13:49:16.000000 train_track-0.1.4/sage-train-track-users-guide.pdf
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    20946 2021-03-11 13:49:16.000000 train_track-0.1.4/sage-train-track-users-guide.tex
--rw-rw-r--   0 thierry   (1001) thierry   (1001)       38 2022-02-28 20:46:32.608546 train_track-0.1.4/setup.cfg
--rw-rw-r--   0 thierry   (1001) thierry   (1001)     1808 2021-03-11 13:49:16.000000 train_track-0.1.4/setup.py
-drwxrwxr-x   0 thierry   (1001) thierry   (1001)        0 2022-02-28 20:46:32.604546 train_track-0.1.4/train_track/
--rw-rw-r--   0 thierry   (1001) thierry   (1001)      293 2021-03-11 13:49:16.000000 train_track-0.1.4/train_track/__init__.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    86237 2021-06-04 16:50:41.000000 train_track-0.1.4/train_track/convex_core.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    35041 2021-05-21 08:29:51.000000 train_track-0.1.4/train_track/free_group.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    71114 2021-06-01 14:12:26.000000 train_track-0.1.4/train_track/free_group_automorphism.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    34670 2021-03-11 13:49:16.000000 train_track-0.1.4/train_track/graph_map.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)   147110 2021-03-11 13:49:16.000000 train_track-0.1.4/train_track/graph_self_map.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    21900 2021-03-11 13:49:16.000000 train_track-0.1.4/train_track/inverse_alphabet.py
--rwxrwxr-x   0 thierry   (1001) thierry   (1001)    48603 2021-06-04 16:46:11.000000 train_track-0.1.4/train_track/inverse_graph.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    22255 2021-06-01 14:32:17.000000 train_track-0.1.4/train_track/marked_graph.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)     7864 2021-03-11 13:49:16.000000 train_track-0.1.4/train_track/test_train_track.py
--rw-rw-r--   0 thierry   (1001) thierry   (1001)    72019 2021-05-21 08:29:51.000000 train_track-0.1.4/train_track/train_track_map.py
-drwxrwxr-x   0 thierry   (1001) thierry   (1001)        0 2022-02-28 20:46:32.608546 train_track-0.1.4/train_track.egg-info/
--rw-rw-r--   0 thierry   (1001) thierry   (1001)     2966 2022-02-28 20:46:32.000000 train_track-0.1.4/train_track.egg-info/PKG-INFO
--rw-rw-r--   0 thierry   (1001) thierry   (1001)      596 2022-02-28 20:46:32.000000 train_track-0.1.4/train_track.egg-info/SOURCES.txt
--rw-rw-r--   0 thierry   (1001) thierry   (1001)        1 2022-02-28 20:46:32.000000 train_track-0.1.4/train_track.egg-info/dependency_links.txt
--rw-rw-r--   0 thierry   (1001) thierry   (1001)       12 2022-02-28 20:46:32.000000 train_track-0.1.4/train_track.egg-info/top_level.txt
+drwxrwxr-x   0 thierry   (1001) thierry   (1001)        0 2023-07-17 12:57:37.867133 train_track-0.1.5/
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)      112 2021-03-11 13:49:16.000000 train_track-0.1.5/.gitignore
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    35141 2021-03-11 13:49:16.000000 train_track-0.1.5/LICENSE
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)       16 2021-03-11 13:49:16.000000 train_track-0.1.5/MANIFEST.in
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)     2537 2023-07-17 12:57:37.867133 train_track-0.1.5/PKG-INFO
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)     1828 2023-07-17 09:24:12.000000 train_track-0.1.5/README.rst
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)        5 2023-07-17 12:56:38.000000 train_track-0.1.5/VERSION
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)      656 2021-03-11 13:49:16.000000 train_track-0.1.5/makefile
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)   171953 2021-03-11 13:49:16.000000 train_track-0.1.5/sage-train-track-users-guide.pdf
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    20946 2021-03-11 13:49:16.000000 train_track-0.1.5/sage-train-track-users-guide.tex
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)       38 2023-07-17 12:57:37.867133 train_track-0.1.5/setup.cfg
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)     1808 2021-03-11 13:49:16.000000 train_track-0.1.5/setup.py
+drwxrwxr-x   0 thierry   (1001) thierry   (1001)        0 2023-07-17 12:57:37.863133 train_track-0.1.5/train_track/
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)      293 2021-03-11 13:49:16.000000 train_track-0.1.5/train_track/__init__.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    85543 2023-07-17 09:29:08.000000 train_track-0.1.5/train_track/convex_core.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    34996 2023-07-17 09:29:08.000000 train_track-0.1.5/train_track/free_group.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    71096 2023-07-17 09:29:08.000000 train_track-0.1.5/train_track/free_group_automorphism.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    34725 2023-07-17 12:05:45.000000 train_track-0.1.5/train_track/graph_map.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)   147116 2023-07-17 12:39:34.000000 train_track-0.1.5/train_track/graph_self_map.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    21900 2021-03-11 13:49:16.000000 train_track-0.1.5/train_track/inverse_alphabet.py
+-rwxrwxr-x   0 thierry   (1001) thierry   (1001)    48672 2023-07-17 09:29:08.000000 train_track-0.1.5/train_track/inverse_graph.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    22253 2023-07-17 09:29:08.000000 train_track-0.1.5/train_track/marked_graph.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)     7864 2021-03-11 13:49:16.000000 train_track-0.1.5/train_track/test_train_track.py
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)    72058 2023-07-17 12:12:14.000000 train_track-0.1.5/train_track/train_track_map.py
+drwxrwxr-x   0 thierry   (1001) thierry   (1001)        0 2023-07-17 12:57:37.867133 train_track-0.1.5/train_track.egg-info/
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)     2537 2023-07-17 12:57:37.000000 train_track-0.1.5/train_track.egg-info/PKG-INFO
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)      596 2023-07-17 12:57:37.000000 train_track-0.1.5/train_track.egg-info/SOURCES.txt
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)        1 2023-07-17 12:57:37.000000 train_track-0.1.5/train_track.egg-info/dependency_links.txt
+-rw-rw-r--   0 thierry   (1001) thierry   (1001)       12 2023-07-17 12:57:37.000000 train_track-0.1.5/train_track.egg-info/top_level.txt
```

### Comparing `train_track-0.1.4/LICENSE` & `train_track-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `train_track-0.1.4/PKG-INFO` & `train_track-0.1.5/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,55 @@
-Metadata-Version: 1.1
-Name: train_track
-Version: 0.1.4
-Summary: Train-tracks for freegroup automorphisms
-Home-page: https://github.com/coulbois/sage-train-track
-Author: Thierry Coulbois, Dominique Benielli
-Author-email: thierry.coulbois@univ-amu.fr
-License: GPLv3.0
-Description: sage-train-track
-        ================
-        
-        Free group automorphisms and train-track representatives in python/sage. 
-        
-        This is a Sage optional package. It contains code to handle free group
-        automorphisms (inversion, composition, etc.) and to compute
-        train-track representatives (absolute and relative, stable and
-        unstable) as defined by Bestvina and Handel. This includes the
-        computation of Nielsen paths and indices of iwip automorphisms and
-        much more. Convex cores of pairs of tree as defined by Guirardel also
-        appear.
-        
-        Installation::
-        
-          sage -pip install train_track
-        
-        Warning: it seems that Mac OS X 10.13 and later has a security
-        conflict between SIP and SSL and does not succeed in downloading the
-        package from https://pypi.python.org. To overcome this difficulty,
-        just download the tarball train_track-0.1.4.tar.gz from
-        
-          https://pypi.python.org/simple/train_track
-        
-        and run::
-        
-          sage -pip install /path/to/train_track-0.1.4.tar.gz
-        
-        Warning: if you lack intstallation privilege, you can install only for
-        yourself::
-        
-          sage -pip install --user train_track
-          
-        On Cocalc.com installation can be done either from a terminal as above
-        or from a cell::
-        
-          !sage -pip install train_track
-        
-        Warning, Cocalc free accounts do not have access to internet, first
-        download the tarball then install.
-          
-        Usage::
-        
-            sage: from train_track import *
-        
-        
-        After this command, you can play with free groups and their automorphisms::
-        
-            sage: FreeGroup('a,b,c')
-            Free Group on generators {a, b, c}
-            sage: FreeGroupAutomorphism('a->bCb,b->Bc,c->BcBa')
-            Automorphism of the Free Group on generators {a, b, c}: a->a*b,b->a*c,c->a
-            sage: free_group_automorphisms.Cohen_Lustig_1_6()
-            Automorphism of the Free Group on generators {a, b, c}: a->c^3*a*c^-3,b->c^-1*a*c^2*a^-1*b*c^-1,c->a*c^2*a^-1*b*c^2*a*c^-2*b^-1*a*c^-2*a^-1*c^4*a^-1*c^-3
-            
-        
-Keywords: SageMath Freegroup Automorphism Train-track
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 2.7
+sage-train-track
+================
+
+Free group automorphisms and train-track representatives in python/sage. 
+
+This is a Sage optional package. It contains code to handle free group
+automorphisms (inversion, composition, etc.) and to compute
+train-track representatives (absolute and relative, stable and
+unstable) as defined by Bestvina and Handel. This includes the
+computation of Nielsen paths and indices of iwip automorphisms and
+much more. Convex cores of pairs of tree as defined by Guirardel also
+appear.
+
+Installation::
+
+  sage -pip install train_track
+
+Warning: it seems that Mac OS X 10.13 and later has a security
+conflict between SIP and SSL and does not succeed in downloading the
+package from https://pypi.python.org. To overcome this difficulty,
+just download the tarball train_track-0.1.4.tar.gz from
+
+  https://pypi.python.org/simple/train_track
+
+and run::
+
+  sage -pip install /path/to/train_track-0.1.4.tar.gz
+
+Warning: if you lack intstallation privilege, you can install only for
+yourself::
+
+  sage -pip install --user train_track
+  
+On Cocalc.com installation can be done either from a terminal as above
+or from a cell::
+
+  !sage -pip install train_track
+
+Warning, Cocalc free accounts do not have access to internet, first
+download the tarball then install.
+  
+Usage::
+
+    sage: from train_track import *
+
+
+After this command, you can play with free groups and their automorphisms::
+
+    sage: FreeGroup('a,b,c')
+    Free Group on generators {a, b, c}
+    sage: FreeGroupAutomorphism('a->bCb,b->Bc,c->BcBa')
+    Automorphism of the Free Group on generators {a, b, c}: a->a*b,b->a*c,c->a
+    sage: free_group_automorphisms.Cohen_Lustig_1_6()
+    Automorphism of the Free Group on generators {a, b, c}: a->c^3*a*c^-3,b->c^-1*a*c^2*a^-1*b*c^-1,c->a*c^2*a^-1*b*c^2*a*c^-2*b^-1*a*c^-2*a^-1*c^4*a^-1*c^-3
+
```

### Comparing `train_track-0.1.4/makefile` & `train_track-0.1.5/makefile`

 * *Files identical despite different names*

### Comparing `train_track-0.1.4/sage-train-track-users-guide.pdf` & `train_track-0.1.5/sage-train-track-users-guide.pdf`

 * *Files identical despite different names*

### Comparing `train_track-0.1.4/sage-train-track-users-guide.tex` & `train_track-0.1.5/sage-train-track-users-guide.tex`

 * *Files identical despite different names*

### Comparing `train_track-0.1.4/setup.py` & `train_track-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `train_track-0.1.4/train_track/convex_core.py` & `train_track-0.1.5/train_track/convex_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -638,15 +638,17 @@
 
             sage: from train_track import *
             sage: from train_track.convex_core import ConvexCore
             sage: phi = FreeGroupAutomorphism("a->ab,b->ac,c->a")**2
             sage: C = ConvexCore(phi)
             sage: C._build_signed_ends()
             sage: print(C._signed_ends)
-            {'a': [(word: Ca, '+'), (word: Cb, '+'), (word: a, '+'), (word: b, '+'), (word: c, '+')], 'b': [(word: Bca, '+'), (word: Bcb, '+'), (word: Bcc, '+')], 'c': [(word: Ba, '+')]}
+            {'a': [(word: Ca, '+'), (word: Cb, '+'), (word: a, '+'), (word: b, '+'), (word: c, '+')],
+             'b': [(word: Bca, '+'), (word: Bcb, '+'), (word: Bcc, '+')],
+             'c': [(word: Ba, '+')]}
         """
 
         G0 = self._G0
         G1 = self._G1
 
         f = self._f01
         g = self._f10
@@ -1074,25 +1076,24 @@
 
         List of edges of ``self``.
 
         EXAMPLES::
 
             sage: from train_track import *
             sage: from train_track.convex_core import ConvexCore
-            sage: phi=FreeGroupAutomorphism("a->ab,b->ac,c->a")**2
-            sage: C=ConvexCore(phi)
-            sage: C.edges()
-            [[2, 3, ('b', 1)],
-             [3, 1, ('a', 1)],
-             [3, 0, ('c', 0)],
-             [1, 2, ('c', 0)],
-             [1, 0, ('b', 0)],
-             [0, 2, ('a', 1)]]
+            sage: phi = FreeGroupAutomorphism("a->ab,b->ac,c->a")**2
+            sage: C = ConvexCore(phi)
+            sage: sorted(C.edges())
+             [[0, 2, ('a', 1)],
+              [1, 0, ('b', 0)],
+              [1, 2, ('c', 0)],
+              [2, 3, ('b', 1)],
+              [3, 0, ('c', 0)],
+              [3, 1, ('a', 1)]]
         """
-
         return self._edges
 
     def vertices(self):
         """
         List of vertices of ``self``.
 
         .. WARNING:
@@ -1295,20 +1296,16 @@
 
         EXAMPLES::
 
             sage: from train_track import *
             sage: from train_track.convex_core import ConvexCore
             sage: phi = FreeGroupAutomorphism("a->abaababa,b->abaab")
             sage: C = ConvexCore(phi)
-            sage: C.squares_of_the_boundary()
-            [(1, 1), (0, 0), (3, 2), (4, 2), (8, 1), (5, 3), (2, 0), (6, 3)]
-            sage: C.squares_of_the_boundary(verbose=True)
-            [(1, 1), (0, 0), (3, 2), (4, 2), (8, 1), (5, 3), (2, 0), (6, 3)]
-
-
+            sage: sorted(C.squares_of_the_boundary())
+            [(0, 0), (1, 1), (2, 0), (3, 2), (4, 2), (5, 3), (6, 3), (8, 1)]
         """
 
         valence = dict(((e[0], e[1], e[2]), True) for e in self.edges())
         # valence[e]=True if the edge e has valence 0,
         # valence[e]=(i,j) if i is the unique square bounding e and e
         # is the j-th edge of i and False if there are at least two
         # squares bounding e.
@@ -1456,49 +1453,31 @@
 
         EXAMPLES::
 
             sage: from train_track import *
             sage: from train_track.convex_core import ConvexCore
             sage: phi = FreeGroupAutomorphism("a->abaababa,b->abaab")
             sage: C = ConvexCore(phi)
-            sage: C.surface_boundary()
-            [(2, 7, ('a', 1, -1)),
-             (7, 2, ('A', 1, 1)),
+            sage: sorted(C.surface_boundary())
+            [(0, 1, ('A', 0, -1)),
+             (0, 8, ('B', 0, 1)),
              (1, 0, ('a', 0, 1)),
-             (0, 1, ('A', 0, -1)),
+             (1, 11, ('A', 1, -1)),
+             (2, 3, ('A', 0, 1)),
+             (2, 7, ('a', 1, -1)),
+             (3, 2, ('a', 0, -1)),
              (3, 4, ('b', 0, 1)),
              (4, 3, ('B', 0, -1)),
-             (3, 2, ('a', 0, -1)),
-             (2, 3, ('A', 0, 1)),
-             (7, 8, ('b', 1, -1)),
-             (8, 7, ('B', 1, 1)),
-             (11, 1, ('a', 1, 1)),
-             (1, 11, ('A', 1, -1)),
-             (8, 0, ('b', 0, -1)),
-             (0, 8, ('B', 0, 1)),
              (4, 11, ('b', 1, 1)),
-             (11, 4, ('B', 1, -1))]
-            sage: C.surface_boundary(verbose=True)
-            [(2, 7, ('a', 1, -1)),
              (7, 2, ('A', 1, 1)),
-             (1, 0, ('a', 0, 1)),
-             (0, 1, ('A', 0, -1)),
-             (3, 4, ('b', 0, 1)),
-             (4, 3, ('B', 0, -1)),
-             (3, 2, ('a', 0, -1)),
-             (2, 3, ('A', 0, 1)),
              (7, 8, ('b', 1, -1)),
+             (8, 0, ('b', 0, -1)),
              (8, 7, ('B', 1, 1)),
              (11, 1, ('a', 1, 1)),
-             (1, 11, ('A', 1, -1)),
-             (8, 0, ('b', 0, -1)),
-             (0, 8, ('B', 0, 1)),
-             (4, 11, ('b', 1, 1)),
              (11, 4, ('B', 1, -1))]
-
         """
 
         if orientation is None:
             orientation = getattr(self, '_squares_orientation', None)
 
         if orientation is None:
             orientation = self.squares_orientation()
@@ -1614,17 +1593,17 @@
         A1 = T1.alphabet()
 
         # Let ``self`` be the convex core of trees T0 and T1. T0 and
         # T1 need to be roses. The trees T0 and T1 may be given as
         # embedded inside the surface. In this case the edges outgoing
         # from the sole vertex are cyclically ordered.
 
-        if len(T0.vertices()) != 1:
+        if T0.num_verts() != 1:
             raise ValueError('The tree on side 0 must be a rose')
-        if len(T1.vertices()) != 1:
+        if T1.num_verts() != 1:
             raise ValueError('The tree on side 1 must be a rose')
 
         if cyclic_order_0 is None:
             cyclic_order_0 = getattr(T0, 'cyclic_order', None)
         if cyclic_order_1 is None:
             cyclic_order_1 = getattr(T1, 'cyclic_order', None)
```

### Comparing `train_track-0.1.4/train_track/free_group.py` & `train_track-0.1.5/train_track/free_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,17 +264,16 @@
 
     def __hash__(self):
         r"""
         TESTS::
 
             sage: from train_track import *
             sage: G.<a,b> = FreeGroup()
-            sage: hash(a*b*b*~a)
-            -485698212495963022 # 64-bit
-            -1876767630         # 32-bit
+            sage: hash(a*b*b*~a) # random
+            -1876767630
         """
         return hash(self.Tietze())
 
     def _latex_(self):
         r"""
         Return a LaTeX representation
 
@@ -405,17 +404,17 @@
             sage: x = a^2 * b^(-3) * a^(-2)
             sage: x.Tietze()
             (1, 1, -2, -2, -2, -1, -1)
 
         TESTS::
 
             sage: type(a.Tietze())
-            <... 'tuple'>
+            <class 'tuple'>
             sage: type(a.Tietze()[0])
-            <type 'sage.rings.integer.Integer'>
+            <class 'sage.rings.integer.Integer'>
         """
         tl = self.gap().TietzeWordAbstractWord()
         return tuple(tl.sage())
 
     def fox_derivative(self, gen, im_gens=None, ring=None):
         r"""
         Return the Fox derivative of ``self`` with respect to a given
@@ -826,15 +825,15 @@
 
     EXAMPLES:
 
     First construct a LibGAP free group::
 
         sage: F = libgap.FreeGroup(['a', 'b'])
         sage: type(F)
-        <type 'sage.libs.gap.element.GapElement'>
+        <class 'sage.libs.gap.element.GapElement'>
 
     Now wrap it::
 
         sage: from train_track.free_group import wrap_FreeGroup
         sage: wrap_FreeGroup(F)
         Free Group on generators {a, b}
```

### Comparing `train_track-0.1.4/train_track/free_group_automorphism.py` & `train_track-0.1.5/train_track/free_group_automorphism.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,20 +494,20 @@
         EXAMPLES::
 
             sage: from train_track import *
             sage: f = FreeGroupAutomorphism('a->AD,b->Adac,c->bd,d->c')
             sage: f.to_word_morphism()
             WordMorphism: a->a^-1,d^-1, a^-1->da, b->a^-1,d,a,c, b^-1->c^-1,a^-1,d^-1,a, c->bd, c^-1->d^-1,b^-1, d->c, d^-1->c^-1
             sage: f.to_word_morphism().periodic_points()
-               [[word: a^-1,d,a,c,c,c,a^-1,d^-1,d^-1,b^-1,d,a,c,a^-1,d^-1,b,d,b,d,b,d,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,b,d,d,a,c^-1,a^-1,d,a,...,
-                 word: d,a,c,a^-1,d^-1,b,d,b,d,b,d,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,b,d,d,a,c^-1,a^-1,d,a,c,c,a^-1,d,a,c,c,a^-1,d,a,...,
-                 word: c,a^-1,d^-1,b,d,d,a,c^-1,a^-1,d,a,c,c,a^-1,d,a,c,c,a^-1,d,a,c,c,c,a^-1,d^-1,d^-1,b^-1,d^-1,b^-1,d^-1,b^-1,d,a,c^-1,a^-1,d^-1,b,d,d,...,
-                 word: b,d,d,a,c^-1,a^-1,d,a,c,c,c,a^-1,d^-1,d^-1,b^-1,d,a,c,a^-1,d^-1,b,d,b,d,d,a,c,a^-1,d^-1,b,d,b,d,d,a,c,a^-1,d^-1,b,d,...],
-                [word: c^-1,c^-1,a^-1,d^-1,a,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,d^-1,b^-1,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,d^-1,b^-1,d,a,c^-1,a^-1,d,a,c,...,
-                 word: d^-1,b^-1,d^-1,b^-1,d,a,c^-1,a^-1,d^-1,d^-1,b^-1,d^-1,b^-1,d,a,c^-1,a^-1,d^-1,b,d,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,d^-1,b^-1,d^-1,b^-1,d^-1,b^-1,d,a,c^-1,...]]
+            [[word: a^-1,d,a,c,c,c,a^-1,d^-1,d^-1,b^-1,d,a,c,a^-1,d^-1,b,d,b,d,b,d,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,b,d,d,a,c^-1,a^-1,d,a,...,
+              word: d,a,c,a^-1,d^-1,b,d,b,d,b,d,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,b,d,d,a,c^-1,a^-1,d,a,c,c,a^-1,d,a,c,c,a^-1,d,a,...,
+              word: c,a^-1,d^-1,b,d,d,a,c^-1,a^-1,d,a,c,c,a^-1,d,a,c,c,a^-1,d,a,c,c,c,a^-1,d^-1,d^-1,b^-1,d^-1,b^-1,d^-1,b^-1,d,a,c^-1,a^-1,d^-1,b,d,d,...,
+              word: b,d,d,a,c^-1,a^-1,d,a,c,c,c,a^-1,d^-1,d^-1,b^-1,d,a,c,a^-1,d^-1,b,d,b,d,d,a,c,a^-1,d^-1,b,d,b,d,d,a,c,a^-1,d^-1,b,d,...],
+             [word: c^-1,c^-1,a^-1,d^-1,a,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,d^-1,b^-1,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,d^-1,b^-1,d,a,c^-1,a^-1,d,a,c,...,
+              word: d^-1,b^-1,d^-1,b^-1,d,a,c^-1,a^-1,d^-1,d^-1,b^-1,d^-1,b^-1,d,a,c^-1,a^-1,d^-1,b,d,d,a,c^-1,c^-1,c^-1,a^-1,d^-1,a,c,a^-1,d^-1,d^-1,b^-1,d^-1,b^-1,d^-1,b^-1,d,a,c^-1,...]]
         """
         F = self._domain
         A = F.gens()
 
         if compact:
             use_str = True
             upper_case_as_inverse = True
```

### Comparing `train_track-0.1.4/train_track/graph_map.py` & `train_track-0.1.5/train_track/graph_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     sage: from train_track.inverse_graph import GraphWithInverses
     sage: from train_track.graph_map import GraphMap
     sage: G = GraphWithInverses({'a':(0,0),'b':(0,1),'c':(1,0)})
     sage: A = AlphabetWithInverses(2)
     sage: H = GraphWithInverses.rose_graph(A)
     sage: print(GraphMap(G,H,"a->ab,b->b,c->B"))
     Graph map:
-    a: 0->0, c: 1->0, b: 0->1
+    a: 0->0, b: 0->1, c: 1->0
     a: 0->0, b: 0->0
-    edge map: a->ab, c->B, b->b
+    edge map: a->ab, b->b, c->B
 """
 #
 # *****************************************************************************
 #       Copyright (C) 2013 Thierry Coulbois <thierry.coulbois@univ-amu.fr>
 #
 #  Distributed under the terms of the GNU General Public License (GPL)
 #                  http://www.gnu.org/licenses/
@@ -468,15 +468,15 @@
         A1 = G1.alphabet()
         T1 = G1.spanning_tree()
 
         G2 = self.codomain()
         A2 = G2.alphabet()
         T2 = G2.spanning_tree()
 
-        A = AlphabetWithInverses(len(A1) - len(G1.vertices()) + 1)
+        A = AlphabetWithInverses(len(A1) - G1.num_verts() + 1)
         F = FreeGroup(A.positive_letters())
 
         map = dict()
         translate = dict()
 
         i = 0
         for a in A1.positive_letters():
@@ -568,22 +568,22 @@
         """
         G1 = self.domain()
         A1 = G1.alphabet()
         G2 = self.codomain()
 
         edge_map = dict((a, self.image(a)) for a in A1)
 
-        adjacent_vertex = dict((v,v) for v in G1.vertices())  # a
+        adjacent_vertex = dict((v,v) for v in G1.vertices(sort=False))  # a
         # class of vertices linked by a tree which is contracted by
         # self to a point
 
         done = False
         while not done:
             done = True
-            gates = dict((v,[]) for v in G1.vertices())  # the gates
+            gates = dict((v,[]) for v in G1.vertices(sort=False))  # the gates
             # outgoing from a contracted tree
             minimal_edge = dict() # The minimal edge (in lexicographic
             # order) outgoing from a contracted forest.
             
             for a in A1:
                 u = edge_map[a]
                 v = G1.initial_vertex(a)
@@ -600,19 +600,19 @@
                         gates[vv] = gates[vv] + gates[ww]
                         if ww in minimal_edge:
                             if vv not in minimal_edge:
                                 minimal_edge[vv] = minimal_edge[ww]
                             elif minimal_edge[ww] < minimal_edge[vv]:
                                 minimal_edge[vv] = minimal_edge[ww]                                
 
-                        for t in G1.vertices():
+                        for t in G1.vertices(sort=False):
                             if adjacent_vertex[t] ==  ww:
                                 adjacent_vertex[t] = vv
 
-            for v in G1.vertices():
+            for v in G1.vertices(sort=False):
                 if v == adjacent_vertex[v]:
                     gates[v].sort()
                     i = 0
 
                     while i < len(gates[v]):
                         prefix = gates[v][i]
                         j = i+1
@@ -766,15 +766,15 @@
 
     def stallings_folding(self):
         """
         Implement Stallings' folding to get an immersion from ``self``.
 
         The domain of ``self`` is fold until we get an
         immersion. Intended to be used to compute the pullback of two
-        graph maps and the intersection of subgroupes of a free group.
+        graph maps and the intersection of subgroups of a free group.
 
         ALGORITHM:
 
         We first subdivide edges of the domain according to length of
         their image.
 
         Then fold one gate at one vertex and update the edge map and
@@ -790,17 +790,17 @@
             sage: A = AlphabetWithInverses(2)
             sage: G = GraphWithInverses.rose_graph(A)
             sage: H = GraphWithInverses.rose_graph(A)
             sage: f = GraphMap(G,H,"a->aba,b->ab")
             sage: f.stallings_folding()
             sage: print(f)
             Graph map:
-            a: 1->1, c: 1->1
+            b: 3->3, c: 3->3
             a: 0->0, b: 0->0
-            edge map: a->a, c->b
+            edge map: b->a, c->b
 
         REFERENCES:
 
         .. [Stallings] J. Stallings, Topology of Finite Graphs,
 
         AUTHOR:
 
@@ -885,17 +885,17 @@
             sage: G =  GraphWithInverses.rose_graph(AlphabetWithInverses(2))
             sage: n1 = WordMorphism({'x0':['a','a'],'x1':['b','a']})
             sage: n2 = WordMorphism({'a0':['b','a'],'a1':['b','b','b','a','B','a']})
             sage: f1 = GraphMap(G1,G,n1)
             sage: f2 = GraphMap(G2,G,n2)
             sage: print(f1.pullback(f2))
             Graph map:
-            a0: (0, 0)->(1, 2), a1: (0, 2)->(1, 0), a2: (0, 2)->(1, 3), a3: (0, 3)->(1, 4), a4: (0, 4)->(1, 3), a5: (1, 2)->(0, 0), a6: (1, 4)->(0, 3)
+            a0: (0, 0)->(2, 6), a1: (0, 3)->(2, 4), a2: (0, 4)->(2, 3), a3: (0, 6)->(2, 0), a4: (0, 6)->(2, 3), a5: (2, 4)->(0, 3), a6: (2, 6)->(0, 0)
             a: 0->0, b: 0->0
-            edge map: a0->b, a1->a, a2->b, a3->b, a4->a, a5->a, a6->a
+            edge map: a0->b, a1->b, a2->a, a3->a, a4->b, a5->a, a6->a
 
         AUTHORS:
 
         - Radhika GUPTA
         """
         import itertools
         # First convert self and f2 into immersions
@@ -903,16 +903,16 @@
         other.stallings_folding()
 
         G3 = GraphWithInverses()
         A = AlphabetWithInverses(0, type='a0')
         d = {}
         # get set of vertices
         V = []
-        for i in itertools.product(self.domain().vertices(),
-                                   other.domain().vertices()):
+        for i in itertools.product(self.domain().vertices(sort=False),
+                                   other.domain().vertices(sort=False)):
             V.append(i)
 
         # add edges
         for v in V:
             for w in V:
                 for e1 in self.domain().alphabet().positive_letters():
                     if self.domain().initial_vertex(e1) == v[0] \
```

### Comparing `train_track-0.1.4/train_track/graph_self_map.py` & `train_track-0.1.5/train_track/graph_self_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     sage: from train_track import *
     sage: from train_track.graph_self_map import GraphSelfMap
     sage: A = AlphabetWithInverses(5)
     sage: f = GraphSelfMap.from_edge_map("a->a,b->b,c->c,d->eCEAd,e->eCEAdbDaecEae", A)
     sage: print(f)
     Graph self map:
-    Marked graph: a: 0->0, b: 2->2, c: 1->1, d: 0->2, e: 0->1
+    Marked graph: a: 0->0, b: 1->1, c: 2->2, d: 0->1, e: 0->2
     Marking: a->a, b->dbD, c->ecE
     Edge map: a->a, b->b, c->c, d->eCEAd, e->eCEAdbDaecEae
 
 """
 
 # *****************************************************************************
 #       Copyright (C) 2013 Thierry Coulbois <thierry.coulbois@univ-amu.fr>
@@ -71,15 +71,15 @@
         Marked graph: a: 0->0, b: 0->0, c: 0->0
         Marking: a->a, b->b, c->c
         Edge map: a->ab, b->ac, c->a
         sage: A = AlphabetWithInverses(5)
         sage: f = GraphSelfMap.from_edge_map("a->a,b->b,c->c,d->eCEAd,e->eCEAdbDaecEae",A)
         sage: print(f)
         Graph self map:
-        Marked graph: a: 0->0, b: 2->2, c: 1->1, d: 0->2, e: 0->1
+        Marked graph: a: 0->0, b: 1->1, c: 2->2, d: 0->1, e: 0->2
         Marking: a->a, b->dbD, c->ecE
         Edge map: a->a, b->b, c->c, d->eCEAd, e->eCEAdbDaecEae
 
     AUTHORS:
 
     - Thierry Coulbois (2013-05-16)
 
@@ -145,15 +145,15 @@
                 result += b
             result += ", "
         result = result[:-2]
         if self._strata:
             if len(self._strata) == 1:
                 result += "\nIrreducible representative"
             else:
-                result += "\nStrata: " + self._strata.__str__()
+                result += "\nStrata: " + str(list(map(sorted,self._strata)))
         return result
 
     @staticmethod
     def from_edge_map(edge_map, alphabet=None, path=None):
         """
         Builds a ``GraphSelfMap`` from an edge map.
 
@@ -180,15 +180,15 @@
         a ``GraphSelfMap`` from an edge map.
 
         EXAMPLES::
 
             sage: from train_track.graph_self_map import GraphSelfMap
             sage: print(GraphSelfMap.from_edge_map("a->a,b->b,c->c,d->eCEAd,e->dbDae"))
             Graph self map:
-            Marked graph: a: 0->0, b: 2->2, c: 1->1, d: 0->2, e: 0->1
+            Marked graph: a: 0->0, b: 1->1, c: 2->2, d: 0->1, e: 0->2
             Marking: a->a, b->dbD, c->ecE
             Edge map: a->a, b->b, c->c, d->eCEAd, e->dbDae
             sage: print(GraphSelfMap.from_edge_map("a->a,b->b,c->c,d->eCEAd,e->dbDae",path="ab"))
             Graph self map:
             Marked graph: a: 0->0, b: 0->0, c: 1->1, d: 0->0, e: 0->1
             Marking: a->a, b->b, c->ecE, d->d
             Edge map: a->a, b->b, c->c, d->eCEAd, e->dbDae
@@ -1861,15 +1861,15 @@
 
             sage: from train_track import *
             sage: phi = FreeGroupAutomorphism("a->acba,b->acb,c->c")
             sage: f = phi.train_track(relative=True)
             sage: f.relative_indivisible_nielsen_paths(stratum=1)
             [[word: acb, word: ba]]
         """
-
+        
         G = self._domain
         A = G._alphabet
 
         result = []
         image = []
         next = []
         places = []  # To prevent infinite matching pseudo-paths
@@ -1879,14 +1879,17 @@
             extension[A.inverse_letter(a)] = []
 
         edge_turns = self.edge_turns(stratum)
         for t in edge_turns:
             extension[A.inverse_letter(t[0])].append(t[1])
             extension[A.inverse_letter(t[1])].append(t[0])
 
+        if verbose:
+            print("Extensions outgoing from edges:",extension)
+
         fold_turns = self.fold_turns(stratum)
         for t in fold_turns:
             result.append((Word(), Word()))
             image.append((Word(), Word()))  # tigthen image of result
             next.append((t[0], t[1]))  # letters to add to result
             x = G.initial_vertex(t[0])
             places.append(set([(x, -1, x - 1)]))
@@ -2126,15 +2129,15 @@
             sage: from train_track import *
             sage: phi = FreeGroupAutomorphism("a->adb,b->adc,c->a,d->d")**3
             sage: f = phi.rose_representative()
             sage: f.stratify()
             [{'d'}, {'a', 'b', 'c', 'd'}]
             sage: inps = f.relative_indivisible_nielsen_paths(stratum=1)
             sage: f.relative_inessential_inp(inps=inps, stratum=1)
-            [word: adb, word: bda]
+            [word: bda, word: cda]
 
         .. WARNING::
 
             The ``stratum`` stratum of ``self`` must be irreducible,
             exponential and satisfies the relative train-track
             conditions RTT-i, RTT-ii and RTT-iii.
 
@@ -2205,24 +2208,24 @@
             sage: from train_track import *
             sage: phi = FreeGroupAutomorphism("a->adb,b->adc,c->a,d->d")**3
             sage: f = phi.rose_representative()
             sage: f.stratify()
             [{'d'}, {'a', 'b', 'c', 'd'}]
             sage: inps = f.relative_indivisible_nielsen_paths(stratum=1)
             sage: f.fold_inp_in_relative_train_track(inps[0],1)
-            WordMorphism: A->AEDBEDAEDAE, B->BEDAEDAE, C->C, D->D, a->eadeadebdea, b->eadeadeb, c->c, d->d
+            WordMorphism: A->AEDBEDBE, B->BEDC, C->C, D->D, a->ebdebdea, b->cdeb, c->c, d->d
             sage: f.stratify()
             [{'d'}, {'a', 'b', 'c', 'd', 'e'}]
             sage: print(f)
             Graph self map:
             Marked graph: a: 1->0, b: 1->0, c: 0->0, d: 0->0, e: 0->1
             Marking: a->eadeadebdea, b->eadeadeb, c->c, d->d
             Edge map: a->adebdea, b->bdeadcdeadeadebdeadeadeadeb,
             c->eadeadebdeadeadeadebdeadeadebdeadc, d->d, e->eade
-            Strata: [set(['d']), set(['a', 'c', 'b', 'e'])]
+            Strata: [['d'], ['a', 'b', 'c', 'e']]
 
         .. WARNING::
 
             This has no effects on the strata of ``self`` (use
             ``GraphSelfMap.stratify()`` afterward)
         """
         G = self._domain
@@ -2426,17 +2429,17 @@
 
             sage: from train_track import *
             sage: phi = FreeGroupAutomorphism("a->adB,b->adc,c->a,d->d")
             sage: f = phi.rose_representative()
             sage: f.stratify()
             [{'d'}, {'a', 'b', 'c', 'd'}]
             sage: f.relative_matrix(1)
-            [1 1 1]
+            [0 1 0]
             [0 0 1]
-            [1 0 0]
+            [1 1 1]
         """
 
         from sage.matrix.constructor import matrix
 
         M = matrix(len(self._strata[stratum]))
         index = dict((a, j) for j, a in enumerate(self._strata[stratum]))
         for j, a in enumerate(self._strata[stratum]):
@@ -2536,15 +2539,15 @@
             [{'b'}, {'a', 'b'}]
 
             sage: print(f)
             Graph self map:
             Marked graph: a: 0->0, b: 0->0
             Marking: a->a, b->b
             Edge map: a->ab, b->b
-            Strata: [set(['b']), set(['a'])]
+            Strata: [['b'], ['a']]
 
         .. SEEALSO::
 
             :meth:`train_track.graph_self_map.GraphSelfMap.maximal_filtration()`
         """
 
         filtration = self.maximal_filtration(
@@ -2725,15 +2728,15 @@
             WordMorphism: A->A, B->DB, C->C, a->a, b->bd, c->c
 
             sage: print(f)
             Graph self map:
             Marked graph: a: 0->0, b: 0->1, c: 0->0, d: 1->0
             Marking: a->a, b->bd, c->c
             Edge map: a->abd, b->c, c->c, d->a
-            Strata: [set(['c']), set(['b']), set(['a', 'd'])]
+            Strata: [['c'], ['b'], ['a', 'd']]
         """
         A = self._domain.alphabet()
         Dfinverse = dict((e, []) for e in self._strata[s])
         subdivide = []
 
         for e in self._strata[s]:
             Dfinverse[A.inverse_letter(e)] = []
@@ -3472,15 +3475,15 @@
             sage: f.update_strata(m)
             {0: [0], 1: [1]}
             sage: print(f)
             Graph self map:
             Marked graph: a: 0->0, b: 0->0, c: 0->2, e: 2->3, f: 3->0
             Marking: a->a, b->cefb, c->Bcefb
             Edge map: a->acefb, b->a, c->cef, e->cef, f->FEC
-            Strata: [set(['c', 'e', 'f']), set(['a', 'b'])]
+            Strata: [['c', 'e', 'f'], ['a', 'b']]
         """
         G = self._domain
         A = G.alphabet()
         result_morph = None
 
         for p in paths:
             if result_morph:
@@ -3635,15 +3638,15 @@
             sage: f.relative_train_track()
             WordMorphism: A->A, B->B, C->C, D->eD, E->E, a->a, b->b, c->c, d->dE, e->e
             sage: print(f)
             Graph self map:
             Marked graph: a: 0->0, b: 0->0, c: 0->0, d: 0->0, e: 0->0
             Marking: a->a, b->b, c->c, d->dE, e->e
             Edge map: a->acb, b->a, c->cdE, d->d, e->dE
-            Strata: [set(['d']), set(['e']), set(['c']), set(['a', 'b'])]
+            Strata: [['d'], ['e'], ['c'], ['a', 'b']]
         """
 
         if verbose:
             print("Reduction")
         result_morph = self.relative_reduce(
             safe_strata=range(len(self._strata)),
             verbose=verbose and verbose > 1 and verbose - 1)
@@ -3793,15 +3796,15 @@
             sage: f.stable_relative_train_track()
             WordMorphism: A->A, B->B, C->C, D->eD, E->E, a->a, b->b, c->c, d->dE, e->e
             sage: print(f)
             Graph self map:
             Marked graph: a: 0->0, b: 0->0, c: 0->0, d: 0->0, e: 0->0
             Marking: a->a, b->b, c->c, d->dE, e->e
             Edge map: a->acb, b->a, c->cdE, d->d, e->dE
-            Strata: [set(['d']), set(['e']), set(['c']), set(['a', 'b'])]
+            Strata: [['d'], ['e'], ['c'], ['a', 'b']]
         """
 
         G = self._domain
         A = G.alphabet()
 
         result_morph = self.relative_reduce(
             safe_strata=range(len(self._strata)),
```

### Comparing `train_track-0.1.4/train_track/inverse_alphabet.py` & `train_track-0.1.5/train_track/inverse_alphabet.py`

 * *Files identical despite different names*

### Comparing `train_track-0.1.4/train_track/inverse_graph.py` & `train_track-0.1.5/train_track/inverse_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
 
         # DiGraph.__init__(self,data=data, loops=True,multiedges=True,
         #                 vertex_labels=True, pos=None, format=None,
         #                        boundary=[], weighted=None,
         #                 implementation='c_graph', sparse=True)
 
-        for e in self.edges():
+        for e in self.edges(sort=False):
             self._initial[e[2]] = e[0]
             self._terminal[e[2]] = e[1]
             self._initial[alphabet.inverse_letter(e[2])] = e[1]
             self._terminal[alphabet.inverse_letter(e[2])] = e[0]
 
     def copy(self):
         """
@@ -407,15 +407,15 @@
             sage: G = GraphWithInverses([[0,0,'a'],[0,1,'b'],[1,0,'c']])
             sage: G.new_vertex()
             2
         """
         i = 0
         done = False
         while not done:
-            if i not in self.vertices():
+            if i not in self.vertices(sort=False):
                 done = True
             i = i + 1
         return i - 1
 
     def new_vertices(self, n):
         """
         A list of length ``n`` of integers that are not vertices of
@@ -432,15 +432,15 @@
             sage: G = GraphWithInverses([[0,0,'a'],[0,1,'b'],[1,0,'c']])
             sage: G.new_vertices(3)
             [2, 3, 4]
         """
         i = 0
         result = []
         while n > 0:
-            if i not in self.vertices():
+            if i not in self.vertices(sort=False):
                 result.append(i)
                 n = n - 1
             i = i + 1
         return result
 
     def add_vertex(self, i=None):
         """
@@ -462,15 +462,15 @@
             sage: G = GraphWithInverses([[0,0,'a'],[0,1,'b'],[1,0,'c']])
             sage: G.add_vertex()
             2
 
             sage: print (G)
             a: 0->0, b: 0->1, c: 1->0
 
-            sage: print (G.vertices())
+            sage: print (G.vertices(sort=True))
             [0, 1, 2]
         """
         if i is None:
             i = self.new_vertex()
         DiGraph.add_vertex(self, i)
         return i
 
@@ -1042,26 +1042,26 @@
 
             sage: from train_track.inverse_graph import GraphWithInverses
             sage: G = GraphWithInverses([[0,0,'a'],[0,1,'b'],[1,2,'c']])
             sage: G.tails()
             [['b', 'c']]
         """
         outgoing = {}
-        outgoing.update((v, []) for v in self.vertices())
+        outgoing.update((v, []) for v in self.vertices(sort=False))
         A = self._alphabet
         for a in A.positive_letters():
             outgoing[self.initial_vertex(a)].append(a)
             outgoing[self.terminal_vertex(a)].append(A.inverse_letter(a))
 
         valence_1 = []
         edges_1 = []
         done = False
         while not done:
             done = True
-            for v in self.vertices():
+            for v in self.vertices(sort=False):
                 if len(outgoing[v]) == 1:
                     done = False
                     valence_1.append(v)
                     e = outgoing[v][0]
                     vv = self.terminal_vertex(e)
                     outgoing[vv].remove(A.inverse_letter(e))
                     outgoing[v].remove(e)
@@ -1086,15 +1086,15 @@
 
             sage: from train_track.inverse_graph import GraphWithInverses
             sage: G = GraphWithInverses([[0,0,'a'],[0,1,'b'],[1,2,'c']])
             sage: G.valence_2_vertices()
             [['C', 'B']]
         """
         outgoing = {}
-        outgoing.update((v, []) for v in self.vertices())
+        outgoing.update((v, []) for v in self.vertices(sort=False))
         A = self._alphabet
         for a in A:
             outgoing[self.initial_vertex(a)].append(a)
         valence_2 = set(v for v in outgoing if len(outgoing[v]) == 2)
 
         lines = []
```

### Comparing `train_track-0.1.4/train_track/marked_graph.py` & `train_track-0.1.5/train_track/marked_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,14 @@
         sage: G = GraphWithInverses({'a':(0,0),'b':(0,1),'c':(1,0)})
         sage: G = MarkedGraph(G)
         sage: G = MarkedMetricGraph(G)
         sage: print(G)
         Marked graph: a: 0->0, b: 0->1, c: 1->0
         Marking: a->a, b->bc
         Length: a:1, b:1, c:1
-
     """
 
     def __init__(self, graph=None, marking=None, length=None, alphabet=None,
                  marking_alphabet=None):
         """
         Initialize ``self``.
 
@@ -481,15 +480,14 @@
             sage: G = GraphWithInverses({'a':(0,1),'b':(1,1),'c':(1,0)})
             sage: G = MarkedGraph(G)
             sage: G = MarkedMetricGraph(G)
             sage: print(G)
             Marked graph: a: 0->1, b: 1->1, c: 1->0
             Marking: a->abA, b->ac
             Length: a:1, b:1, c:1
-
         """
 
         MarkedGraph.__init__(self, graph=graph,
                              marking=marking,
                              alphabet=alphabet,
                              marking_alphabet=marking_alphabet)
```

### Comparing `train_track-0.1.4/train_track/test_train_track.py` & `train_track-0.1.5/train_track/test_train_track.py`

 * *Files identical despite different names*

### Comparing `train_track-0.1.4/train_track/train_track_map.py` & `train_track-0.1.5/train_track/train_track_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                 result += b
             result += ", "
         result = result[:-2]
         if self._strata:
             if len(self._strata) == 1:
                 result += "\nIrreducible representative"
             else:
-                result += "\nStrata: " + self._strata.__str__()
+                result += "\nStrata: "+ str(list(map(sorted, self._strata)))
 
         return result
 
     def is_train_track(self, verbose=False):
         """
         Return ``True`` because this is a train track map.
 
@@ -460,15 +460,15 @@
             sage: f = phi.rose_conjugacy_representative()
             sage: ff = TrainTrackMap(f)
             sage: ff.stable_local_whitehead_graph(0)
             Subgraph of (): Graph on 4 vertices
         """
         lwg = self.local_whitehead_graph(v)
 
-        directions = lwg.vertices()
+        directions = lwg.vertices(sort=False)
         images = directions
 
         # Looking for a period for the vertex v
         reached_vertices = set([v])
         w = v
         done = False
         while not done:
@@ -1185,15 +1185,15 @@
 
             - :meth:`sage.combinat.words.train_track_map.TrainTrackMap.local_whitehead_graph()`
             - :meth:`sage.combinat.words.train_track_map.TrainTrackMap.whitehead_connected_components()`
         """
 
         return len(
             self.whitehead_connected_components(verbose)) == len(
-            self.domain().vertices())
+            self.domain().vertices(sort=False))
 
     def periodic_nielsen_loops(self, pnps=None, verbose=False):
         """
         List of loops made of periodic Nielsen paths of ``self``.
 
         Such a loop is a periodic element of ``self``.
 
@@ -1443,15 +1443,15 @@
             sage: from train_track import *
             sage: from train_track.train_track_map import TrainTrackMap
             sage: phi = FreeGroupAutomorphism("a->bca,b->bcacacb,c->cac")
             sage: f = TrainTrackMap(phi.rose_representative())
             sage: G = f.ideal_whitehead_graph()
             sage: G
             Graph on 6 vertices
-            sage: G.vertices(sort=False)
+            sage: G.vertices(sort=True)
             ['B', 'C', 'b', 'c', 'loop', word: aBCAbc]
 
         .. WARNING:
 
             If pnps is not given computes them by calling
             ``self.periodic_nielsen_paths()``. Thus it is assumed that
             ``self`` is an expanding train-track.
@@ -1514,15 +1514,15 @@
                         break
             else:
                 germ_classes[i1].append(vv2)
 
         if verbose:
             print("Classes of germ at the end of pnps:", germ_classes)
 
-        for v in G.vertices():
+        for v in G.vertices(sort=False):
             iwg = iwg.union(self.stable_local_whitehead_graph(v))
 
         if verbose:
             print("Graph before identification of "
                    "equivalent germs:", iwg.edges())
 
         # Now mod out the graph by inps
@@ -1753,15 +1753,16 @@
         EXAMPLE::
 
             sage: from train_track import *
             sage: from train_track.train_track_map import TrainTrackMap
             sage: phi = FreeGroupAutomorphism("a->bca,b->bcacacb,c->cac")
             sage: f = TrainTrackMap(phi.rose_representative())
             sage: f.whitehead_connected_components()
-            [['a', 'b', 'C'], ['A', 'c', 'B']]
+            [['C', 'a', 'b'], ['B', 'c', 'A']]
+
 
         .. SEEALSO::
 
             :meth:`local_whitehead_graph()`
         """
         G = self.domain()
         A = G.alphabet()
@@ -1959,15 +1960,15 @@
                        " have a strictly positive power")
             return False
         if verbose:
             print("Fully irreducible: the matrix of self has a strictly "
                    "positive power")
         c = self.whitehead_connected_components(
             verbose and verbose > 1 and verbose - 1)
-        if len(c) > len(self.domain().vertices()):
+        if len(c) > self.domain().num_verts():
             if verbose:
                 print("The local Whitehead graphs are not "
                        "connected. Connected components of germs:", c)
             return False
         if verbose:
             print("Local Whitehead graphs are connected")
         pnps = self.periodic_nielsen_paths(
```

### Comparing `train_track-0.1.4/train_track.egg-info/SOURCES.txt` & `train_track-0.1.5/train_track.egg-info/SOURCES.txt`

 * *Files identical despite different names*

