# Comparing `tmp/yarrow_diagrams-0.0.2.2.tar.gz` & `tmp/yarrow_diagrams-0.0.3.0.tar.gz`

## Comparing `yarrow_diagrams-0.0.2.2.tar` & `yarrow_diagrams-0.0.3.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/__init__.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/bipartite_multigraph.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/cupy.py
--rw-r--r--   0        0        0    12819 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/diagram.py
--rw-r--r--   0        0        0    13057 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/finite_function.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/array/__init__.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/array/cupy.py
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/array/numpy.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/decompose/frobenius.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/functor/functor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/segmented/__init__.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/segmented/finite_function.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/segmented/operations.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/LICENSE
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/__init__.py
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/bipartite_multigraph.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/cupy.py
+-rw-r--r--   0        0        0    12972 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/diagram.py
+-rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/finite_function.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/array/__init__.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/array/cupy.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/array/numpy.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/decompose/frobenius.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/functor/__init__.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/functor/functor.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/functor/optic.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/numpy/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/numpy/layer.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/segmented/__init__.py
+-rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/segmented/finite_function.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/segmented/operations.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/PKG-INFO
```

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/bipartite_multigraph.py` & `yarrow_diagrams-0.0.3.0/yarrow/bipartite_multigraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 As with other classes, these graphs are implemented with an abstract base class
 :py:class:`AbstractBipartiteMultigraph`,
 whose concrete instantiations choose a backend.
 For example, :py:class:`BipartiteMultigraph` are backed by numpy arrays.
 """
 from dataclasses import dataclass
-from yarrow.finite_function import AbstractFiniteFunction, FiniteFunction
+from yarrow.finite_function import AbstractFiniteFunction
 
 class AbstractBipartiteMultigraph:
     """ The type of bipartite multigraphs, parametrised by cls._Fun, the
     underlying representation of finite functions """
     def __init__(self, wi, wo, xi, xo, wn, pi, po, xn):
         """Create a BipartiteMultigraph from its component finite functions.
         For more details see :cite:p:`dpafsd`, Section 3.2.
@@ -98,15 +98,16 @@
 
         Returns:
             AbstractBipartiteMultigraph: The empty bipartite multigraph with no edges and no nodes.
         """
         assert wn.source == 0
         assert xn.source == 0
         e = cls._Fun.initial(0)
-        return cls(e, e, e, e, wn, e, e, xn)
+        pi = po = cls._Fun.initial(None)
+        return cls(e, e, e, e, wn, pi, po, xn)
 
     @classmethod
     def discrete(cls, wn: AbstractFiniteFunction, xn: AbstractFiniteFunction):
         """
         Create the discrete graph of n wires for a given monoidal signature Σ
         whose maps are all initial except for `wn`.
 
@@ -267,11 +268,7 @@
     # same memory location in the 'u' array can happen in parallel, with an
     # arbitrary write succeeding.
     # Note that this doesn't affect correctness because q and f are co-forks,
     # and q is a coequalizer.
     # However, this won't perform well on e.g., GPU hardware. FIXME!
     u[q.table] = f.table
     return type(f)(target, u)
-
-class BipartiteMultigraph(AbstractBipartiteMultigraph):
-    """ AbstractBipartiteMultigraphs backed by numpy arrays """
-    _Fun = FiniteFunction
```

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/cupy.py` & `yarrow_diagrams-0.0.3.0/yarrow/cupy.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,42 @@
 .. danger::
    **Experimental Module**
 
    This code is not thoroughly tested.
    It's included here as a proof-of-concept for GPU acceleration.
    The way backends are selected is also likely to change in the future.
 """
+# Abstract implementations
 from yarrow.finite_function import *
 from yarrow.bipartite_multigraph import *
 from yarrow.diagram import *
+from yarrow.segmented.finite_function import AbstractIndexedCoproduct, AbstractSegmentedFiniteFunction
 
+# Array backend
 import yarrow.array.cupy as cupy
 
-class CupyFiniteFunction(AbstractFiniteFunction):
+class FiniteFunction(AbstractFiniteFunction):
     """ CuPy-backed finite functions """
     _Array = cupy
 
-class CupyBipartiteMultigraph(AbstractBipartiteMultigraph):
+class IndexedCoproduct(AbstractIndexedCoproduct):
+    _Fun = FiniteFunction
+
+class BipartiteMultigraph(AbstractBipartiteMultigraph):
     """ CuPy-backed bipartite multigraphs """
-    _Fun = CupyFiniteFunction
+    _Fun = FiniteFunction
 
-class CupyDiagram(AbstractDiagram):
+class Diagram(AbstractDiagram):
     """ CuPy-backed string diagrams """
-    _Fun = CupyFiniteFunction
-    _Graph = CupyBipartiteMultigraph
+    _Fun = FiniteFunction
+    _Graph = BipartiteMultigraph
+
+class SegmentedFiniteFunction(AbstractSegmentedFiniteFunction):
+    _Array = cupy
+    _Fun = FiniteFunction
+
+# If we had types, this would be 'type-level function' giving us the
+# implementation of each of these classes in terms of the base (Numpy-backed
+# FiniteFunction)
+FiniteFunction.IndexedCoproduct = IndexedCoproduct
+FiniteFunction.BipartiteMultigraph = BipartiteMultigraph
+FiniteFunction.Diagram = Diagram
```

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/diagram.py` & `yarrow_diagrams-0.0.3.0/yarrow/diagram.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,23 +34,21 @@
 Summary
 -------
 
 .. autosummary::
     :template: class.rst
 
     AbstractDiagram
-    Diagram
 """
 from dataclasses import astuple
 
-from yarrow.finite_function import AbstractFiniteFunction, FiniteFunction
-from yarrow.bipartite_multigraph import BipartiteMultigraph, AbstractBipartiteMultigraph
+from yarrow.finite_function import AbstractFiniteFunction
+from yarrow.bipartite_multigraph import AbstractBipartiteMultigraph
 
 # for tensor_operations
-from yarrow.segmented.finite_function import AbstractSegmentedFiniteFunction
 from yarrow.segmented.operations import Operations
 
 class AbstractDiagram:
     """ Implements diagrams parametrised by an underlying choice of backend.
     To use this class, inherit from it and set class members:
 
     - ``_Fun`` (finite functions)
@@ -190,14 +188,26 @@
         """
         assert x.source == 0
         assert w.source == s.target
         assert w.source == t.target
         G = cls._Graph.discrete(w, x)
         return cls(s, t, G)
 
+    @classmethod
+    def half_spider(cls,
+                    s: AbstractFiniteFunction,
+                    w: AbstractFiniteFunction,
+                    x: AbstractFiniteFunction):
+        """ Create a *Frobenius Half-Spider*, which is a spider whose target map is the identity """
+        # s : A → W
+        # w : W → Σ₀
+        assert s.target == w.source
+        t = cls._Fun.identity(w.source)
+        return cls.spider(s, t, w, x)
+
     def dagger(self):
         """Swap the *source* and *target* maps of the diagram.
 
         Returns:
             AbstractDiagram: The dagger functor applied to this diagram.
         """
         return type(self)(self.t, self.s, self.G)
@@ -304,33 +314,32 @@
             s = f.s.inject0(g.G.W) >> q,
             t = g.t.inject1(f.G.W) >> q,
             G = h.G.coequalize_wires(q))
 
     def __rshift__(f, g):
         return f.compose(g)
 
-    # TODO: IMPROVE THIS
     @classmethod
     def tensor_list(cls, ds: 'List[AbstractDiagram]', wn=None, xn=None):
         """ Compute the tensor product of a list of diagrams. O(n) time in the size of the result.
 
         .. warning::
             Does not speed up to O(log n) in the parallel case
         """
         if len(ds) == 0:
             assert wn is not None
             assert xn is not None
-            return Diagram.empty(wn, xn)
+            return cls.empty(wn, xn)
 
         assert wn is None
         assert xn is None
         s = cls._Fun.tensor_list([d.s for d in ds])
         t = cls._Fun.tensor_list([d.t for d in ds])
         G = cls._Graph.coproduct_list([d.G for d in ds])
-        return Diagram(s, t, G)
+        return cls(s, t, G)
 
     @classmethod
     def tensor_operations(cls, ops: Operations):
         pass # hide the docstring for now
         """ Compute the X-fold tensoring of operations
 
         .. code-block:: text
@@ -374,12 +383,7 @@
                 # e.g. 0 1 2 | 0 1 | 0 1 2 3 ...
                 pi = Fun(None, Array.segmented_arange(s_type.sources.table)),
                 po = Fun(None, Array.segmented_arange(t_type.sources.table)),
                 # wires: sources first, then targets
                 wi = i0,
                 wo = i1,
                 wn = s_type.values + t_type.values))
-
-class Diagram(AbstractDiagram):
-    """ Diagrams with the numpy backend """
-    _Fun = FiniteFunction
-    _Graph = BipartiteMultigraph
```

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/finite_function.py` & `yarrow_diagrams-0.0.3.0/yarrow/finite_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 And in parallel:
 
 >>> FiniteFunction.identity(5) @ FiniteFunction.terminal(5)
 FiniteFunction(6, [0 1 2 3 4 5 5 5 5 5])
 """
 
 from typing import List
-import yarrow.array.numpy as numpy
+# import yarrow.array.numpy as numpy
 
 DTYPE='int64'
 
 class AbstractFiniteFunction:
     """
     Finite functions parametrised over the underlying array type (the "backend").
     This implementation assumes there is a cls._Array member implementing various primitives.
@@ -121,15 +121,15 @@
         Returns:
             The composition f ; g.
 
         Raises:
             ValueError: if self.target != g.source
         """
         if f.target != g.source:
-            raise ValueError("Can't compose FiniteFunction {f} with {g}: f.source != g.target")
+            raise ValueError(f"Can't compose FiniteFunction {f} with {g}: f.target != g.source")
 
         source = f.source
         target = g.target
         # Use array indexing to compute composition in parallel (if applicable
         # cls._Array backend is used)
         table = g.table[f.table]
 
@@ -257,25 +257,54 @@
     ################################################################################
     # FiniteFunction also has cartesian structure which is useful
     @classmethod
     def terminal(cls, a, dtype=DTYPE):
         """ Compute the terminal map ``! : a → 1``. """
         return cls(1, cls._Array.zeros(a, dtype=DTYPE))
 
+    # TODO: rename this "element"?
+    @classmethod
+    def singleton(cls, x, b, dtype=DTYPE):
+        """ return the singleton array ``[x]`` whose domain is ``b``. """
+        assert x < b
+        return cls(b, cls._Array.full(1, x, dtype=dtype))
+
     ################################################################################
     # Sorting morphisms
     def argsort(f: 'AbstractFiniteFunction'):
         """
         Given a finite function                     ``f : A → B``
         Return the *stable* sorting permutation     ``p : A → A``
         such that                                   ``p >> f``  is monotonic.
         """
         return type(f)(f.source, f._Array.argsort(f.table))
 
     ################################################################################
+    # Useful permutations
+
+    # Given generating objects A_i and B_i for i ∈ ord{n},
+    #   interleave : (A₀ ● A₁ ● ... ● An) ● (B₀ ● B₁ ● ... ● Bn) → (A₀ ● B₀) ● .. ● (An ● Bn)
+    @classmethod
+    def interleave(cls, N: int):
+        table = cls._Array.zeros(2*N, dtype=int)
+        table[0:N] = cls._Array.arange(N)*2
+        table[N:] = table[0:N] + 1
+        return cls(2*N, table)
+
+    # Given generating objects A_i and B_i for i ∈ ord{n},
+    #   cointerleave : (A₀ ● B₀) ● .. ● (An ● Bn) → (A₀ ● A₁ ● ... ● An) ● (B₀ ● B₁ ● ... ● Bn)
+    @classmethod
+    def cointerleave(cls, N):
+        table = cls._Array.zeros(2*N, dtype=int)
+        table[0::2] = cls._Array.arange(N)
+        table[1::2] = table[0::2] + N
+        return cls(2*N, table)
+
+
+    ################################################################################
     # Sequential-only methods
 
     @classmethod
     def coproduct_list(cls, fs: List['AbstractFiniteFunction'], target=None):
         """ Compute the coproduct of a list of finite functions. O(n) in size of the result.
 
         .. warning::
@@ -299,15 +328,15 @@
         if len(fs) == 0:
             return cls.initial(0)
 
         targets = cls._Array.array([f.target for f in fs])
         offsets = cls._Array.zeros(len(targets) + 1, dtype=type(fs[0].source))
         offsets[1:] = cls._Array.cumsum(targets) # exclusive scan
         table = cls._Array.concatenate([f.table + offset for f, offset in zip(fs, offsets[:-1])])
-        return FiniteFunction(offsets[-1], table)
+        return cls(offsets[-1], table)
 
 
     ################################################################################
     # Finite coproducts
     def injections(s: 'AbstractFiniteFunction', a: 'AbstractFiniteFunction'):
         """
         Given a finite function ``s : N → K``
@@ -340,18 +369,14 @@
         k = a >> s # avoid recomputation
         r = Array.segmented_arange(k.table)
         # NOTE: p[-1] is sum(s).
         cls = type(s)
         return cls(p[-1], r + cls._Array.repeat(p[a.table], k.table))
 
 
-class FiniteFunction(AbstractFiniteFunction):
-    """ Finite functions backed by numpy arrays """
-    _Array = numpy
-
 def argsort(f: AbstractFiniteFunction):
     """ Applies a stable 'argsort' to the underlying array of a finite function.
     When that finite function is a permutation, this inverts it.
     """
     return type(f)(f.source, f._Array.argsort(f.table))
 
 def bincount(f: AbstractFiniteFunction):
@@ -367,7 +392,14 @@
     # the bincount of an array
     #   f : A → B
     # is a finite function
     #   g : B → A+1
     # where
     #   g(b) = |{b . ∃a. f(a) = b}|
     return type(f)(len(f)+1, f._Array.bincount(f.table, minlength=f.target))
+
+def cumsum(f: AbstractFiniteFunction) -> AbstractFiniteFunction:
+    Fun = type(f)
+    Array = Fun._Array
+    table = Array.zeros(len(f) + 1, dtype=f.table.dtype)
+    table[1:] = Array.cumsum(f.table)
+    return Fun(table[-1]+1, table[:-1])
```

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/array/__init__.py` & `yarrow_diagrams-0.0.3.0/yarrow/array/__init__.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/array/cupy.py` & `yarrow_diagrams-0.0.3.0/yarrow/array/cupy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/array/numpy.py` & `yarrow_diagrams-0.0.3.0/yarrow/array/numpy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.2/yarrow/decompose/frobenius.py` & `yarrow_diagrams-0.0.3.0/yarrow/decompose/frobenius.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from dataclasses import dataclass
-from yarrow.finite_function import FiniteFunction, argsort
-from yarrow.bipartite_multigraph import BipartiteMultigraph
-from yarrow.diagram import Diagram
+from yarrow.diagram import AbstractDiagram
 
-def frobenius_decomposition(d: Diagram) -> Diagram:
+def frobenius_decomposition(d: AbstractDiagram) -> AbstractDiagram:
     """ Given a Diagram, permute its xi, xo, pi, and po maps to be in
     (generator, port) order.
     """
     # A Frobenius Decomposition is really just diagram whose edges are put in
     # "generator, port" order.
     # Obtaining the half spiders and tensorings from such a diagram is trivial:
     # - s, t  are the source, targets of the diagram
```

### Comparing `yarrow_diagrams-0.0.2.2/LICENSE` & `yarrow_diagrams-0.0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.2/README.md` & `yarrow_diagrams-0.0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.2/pyproject.toml` & `yarrow_diagrams-0.0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yarrow-diagrams"
-version = "0.0.2.2"
+version = "0.0.3.0"
 authors = [
   { name="Paul Wilson", email="paul@statusfailed.com" }
 ]
 description = "yarrow diagrams"
 readme = "README.md"
 requires-python = ">= 3.7"
 classifiers = [
```

### Comparing `yarrow_diagrams-0.0.2.2/PKG-INFO` & `yarrow_diagrams-0.0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarrow-diagrams
-Version: 0.0.2.2
+Version: 0.0.3.0
 Summary: yarrow diagrams
 Project-URL: Homepage, https://yarrow.id
 Project-URL: Github, https://github.com/yarrow-id/diagrams/
 Project-URL: Documentation, https://yarrow-diagrams.readthedocs.io/
 Author-email: Paul Wilson <paul@statusfailed.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

