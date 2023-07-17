# Comparing `tmp/robingrad-0.0.2.tar.gz` & `tmp/robingrad-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingrad-0.0.2.tar", last modified: Fri Jul 14 10:03:58 2023, max compression
+gzip compressed data, was "robingrad-0.0.3.tar", last modified: Mon Jul 17 16:28:44 2023, max compression
```

## Comparing `robingrad-0.0.2.tar` & `robingrad-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.284901 robingrad-0.0.2/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.2/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2173 2023-07-14 10:03:58.284440 robingrad-0.0.2/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      512 2023-07-13 15:18:38.000000 robingrad-0.0.2/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-12 14:06:21.000000 robingrad-0.0.2/pyproject.toml
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.280449 robingrad-0.0.2/robingrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-14 10:03:44.000000 robingrad-0.0.2/robingrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.2/robingrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.2/robingrad/lab.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.283136 robingrad-0.0.2/robingrad/nn/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.2/robingrad/nn/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10607 2023-07-14 10:01:34.000000 robingrad-0.0.2/robingrad/tensor.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.282620 robingrad-0.0.2/robingrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2173 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      320 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-14 10:03:58.285042 robingrad-0.0.2/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.283616 robingrad-0.0.2/tests/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.2/tests/test_tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.209900 robingrad-0.0.3/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.3/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-17 16:28:44.209467 robingrad-0.0.3/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1356 2023-07-17 16:28:33.000000 robingrad-0.0.3/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-17 16:28:30.000000 robingrad-0.0.3/pyproject.toml
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.203974 robingrad-0.0.3/robingrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-17 13:45:08.000000 robingrad-0.0.3/robingrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.3/robingrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.3/robingrad/lab.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.207115 robingrad-0.0.3/robingrad/nn/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.3/robingrad/nn/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1659 2023-07-17 15:58:41.000000 robingrad-0.0.3/robingrad/optim.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.3/robingrad/state.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10337 2023-07-17 14:12:32.000000 robingrad-0.0.3/robingrad/tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.206605 robingrad-0.0.3/robingrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-17 16:28:44.210030 robingrad-0.0.3/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.208377 robingrad-0.0.3/tests/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.3/tests/test_tensor.py
```

### Comparing `robingrad-0.0.2/LICENSE` & `robingrad-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.2/pyproject.toml` & `robingrad-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robingrad"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Something between Tinygrad and Micrograd"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `robingrad-0.0.2/robingrad/graph.py` & `robingrad-0.0.3/robingrad/graph.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.2/robingrad/lab.py` & `robingrad-0.0.3/robingrad/lab.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.2/robingrad/tensor.py` & `robingrad-0.0.3/robingrad/tensor.py`

 * *Files 27% similar despite different names*

```diff
@@ -47,144 +47,144 @@
         
     @staticmethod
     def normal(mean: Union[int, float], std: Union[int, float], shape: Tuple, **kwargs) -> "Tensor": return Tensor(np.random.normal(mean, std, shape), _origin="normal", **kwargs)
         
     @staticmethod
     def uniform(low: Union[int, float], high: Union[int, float], shape: Tuple, **kwargs) -> "Tensor": return Tensor(np.random.uniform(low, high, shape), _origin="uniform", **kwargs)    
 
-    def sum(self: "Tensor") -> "Tensor":
+    def sum(self) -> "Tensor":
         out = Tensor(self.data.sum(), dtype=self.data.dtype, _children=(self,), _op="sum()", _origin="sum", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad += np.ones_like(self.data) * out.grad
         out._backward = _backward
         
         return out
     
-    def relu(self: "Tensor") -> "Tensor":
+    def relu(self) -> "Tensor":
         out = Tensor(np.maximum(0, self.data), dtype=self.data.dtype, _children=(self,), _op="relu()", _origin="ReLU", requires_grad=self.requires_grad)
 
         def _backward():
             self.grad += (out.data > 0) * out.grad
         out._backward = _backward
 
         return out
     
-    def sigmoid(self: "Tensor") -> "Tensor":
+    def sigmoid(self) -> "Tensor":
         x = self.data
         t = (1 + np.exp(-x))**-1
         out = Tensor(t, dtype=self.data.dtype, _children=(self,), _op="sigmoid()", _origin="sigmoid", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad += t*(1-t) * out.grad 
         out._backward = _backward
 
         return out 
     
-    def tanh(self: "Tensor") -> "Tensor":
+    def tanh(self) -> "Tensor":
         x = self.data
         t = (np.exp(2*x) - 1)/(np.exp(2*x) + 1)
         out = Tensor(t, dtype=self.data.dtype, _children=(self,), _op="tanh()", _origin="tanh", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad += (1 - t**2) * out.grad
         out._backward = _backward
         
         return out
 
-    def exp(self: "Tensor") -> "Tensor":
+    def exp(self) -> "Tensor":
         x = self.data
         out = Tensor(np.exp(x), dtype=self.data.dtype, _children=(self,), _op="exp()", _origin="exp", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad += out.data * out.grad 
         out._backward = _backward
         
         return out
     
-    def log(self: "Tensor") -> "Tensor":
+    def log(self) -> "Tensor":
         if np.any(self.data <= 0):
             raise ValueError("can't log negative or zero value")
         x = self.data
         out = Tensor(np.log(x), dtype=self.data.dtype, _children=(self,), _op="log()", _origin="log", requires_grad=self.requires_grad)
 
         def _backward():
             self.grad = (x**(-1)) * out.grad
         out._backward = _backward
 
         return out
     
-    def __add__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
+    def __add__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         other = other if isinstance(other, Tensor) else Tensor.broadcast(self, other, dtype=self.data.dtype, requires_grad=self.requires_grad)
         out = Tensor(self.data + other.data, dtype=self.data.dtype, _children=(self, other), _op='+', _origin="__add__", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad += out.grad
             other.grad += out.grad
         out._backward = _backward
 
         return out
     
-    def __mul__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
+    def __mul__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         other = other if isinstance(other, Tensor) else Tensor.broadcast(self, other, dtype=self.data.dtype, requires_grad=self.requires_grad)
         out = Tensor(self.data * other.data, dtype=self.data.dtype, _children=(self, other), _op='*', _origin="__mul__", requires_grad=self.requires_grad)
 
         def _backward():
             self.grad += other.data * out.grad
             other.grad += self.data * out.grad
         out._backward = _backward
 
         return out
     
-    def __pow__(self: "Tensor", other: Union[int, float]) -> "Tensor":
+    def __pow__(self, other: Union[int, float]) -> "Tensor":
         assert isinstance(other, (int, float)), "only supporting int/float powers for now"
         out = Tensor(self.data ** other, dtype=self.data.dtype, _children=(self,), _op=f'**{other}', _origin="__pow__", requires_grad=self.requires_grad)
 
         def _backward():
             self.grad += (other * self.data**(other-1)) * out.grad
         out._backward = _backward
 
         return out
     
-    def __matmul__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
+    def __matmul__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         other = other if isinstance(other, Tensor) else Tensor(other, dtype=self.data.dtype, requires_grad=self.requires_grad)
         out = Tensor(self.data @ other.data, dtype=self.data.dtype, _children=(self, other), _op='@', _origin="__matmul__", requires_grad=self.requires_grad)
 
         def _backward():
             self.grad += out.grad @ other.data.T
             other.grad += self.data.T @ out.grad
         out._backward = _backward
 
         return out
     
-    def __rmatmul__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
+    def __rmatmul__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         return self @ other
     
-    def __neg__(self: "Tensor") -> "Tensor": # -self
+    def __neg__(self) -> "Tensor": # -self
         return self * Tensor.full_like(self, -1, requires_grad=self.requires_grad)
 
-    def __radd__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other + self
+    def __radd__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other + self
         return self + other
 
-    def __sub__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # self - other
+    def __sub__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # self - other
         return self + (-other)
 
-    def __rsub__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other - self
+    def __rsub__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other - self
         return other + (-self)
 
-    def __rmul__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other * self
+    def __rmul__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other * self
         return self * other
 
-    def __truediv__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # self / other
+    def __truediv__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # self / other
         return self * other**-1
 
-    def __rtruediv__(self: "Tensor", other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other / self
+    def __rtruediv__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor": # other / self
         return other * self**-1
     
-    def backward(self: "Tensor") -> None:
+    def backward(self) -> None:
         if self.shape != () and self.shape != (1,) and self.shape != (1,1):
             raise ValueError("Backward can only be called on a scalar tensor.")
         # topological order all of the children in the graph
         topo = []
         visited = set()
         def build_topo(v):
             if v not in visited:
@@ -196,51 +196,51 @@
 
         # go one variable at a time and apply the chain rule to get its gradient
         self.grad = 1
         for v in reversed(topo):
             v._backward()
             
     @property
-    def shape(self: "Tensor") -> Tuple[int, int]: return self.data.shape
+    def shape(self) -> Tuple[int, int]: return self.data.shape
 
     @property
-    def dtype(self: "Tensor") -> str: return self.data.dtype
+    def dtype(self) -> str: return self.data.dtype
             
-    def __repr__(self: "Tensor") -> str:
+    def __repr__(self) -> str:
         if self.requires_grad:
             return f"Tensor: {self._origin}\ndata: \n{self.data}\ngrad: \n{self.grad}\ndtype: {self.data.dtype}"
         else:
             return f"Tensor: {self._origin}\ndata: \n{self.data}\ndtype: {self.data.dtype}"
     
-    def __getitem__(self: "Tensor", val) -> "Tensor":
+    def __getitem__(self, val) -> "Tensor":
         out = Tensor(self.data[val], dtype=self.data.dtype, _children=(self,), _op="slice", _origin="slice", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad[val] += out.grad
         out._backward = _backward
 
         return out
 
-    def reshape(self: "Tensor", shape: Tuple[int, int]) -> "Tensor":
+    def reshape(self, shape: Tuple[int, int]) -> "Tensor":
         out = Tensor(self.data.reshape(shape), dtype=self.data.dtype, _children=(self,), _op="reshape", _origin="reshape", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad += out.grad.reshape(self.shape)
         out._backward = _backward
 
         return out
     
-    def transpose(self: "Tensor", ax1: int = 1, ax2: int = 0) -> "Tensor":
+    def transpose(self, ax1: int = 1, ax2: int = 0) -> "Tensor":
         out = Tensor(self.data.transpose(ax1, ax2), dtype=self.data.dtype, _children=(self,), _op="T", _origin="T", requires_grad=self.requires_grad)
 
         def _backward():
             self.grad += out.grad.transpose(ax1, ax2)
         out._backward = _backward
 
         return out
 
     @property
-    def T(self: "Tensor") -> "Tensor": return self.transpose()  
+    def T(self) -> "Tensor": return self.transpose()  
     
-    def linear(self: "Tensor", weight: "Tensor", bias: Optional["Tensor"] = None) -> "Tensor":
+    def linear(self, weight: "Tensor", bias: Optional["Tensor"] = None) -> "Tensor":
         x = self * weight if len(weight.shape) == 1 else self @ weight
         return x + bias if bias is not None else x
```

### Comparing `robingrad-0.0.2/tests/test_tensor.py` & `robingrad-0.0.3/tests/test_tensor.py`

 * *Files identical despite different names*

