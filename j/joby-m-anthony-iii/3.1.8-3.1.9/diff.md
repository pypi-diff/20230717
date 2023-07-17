# Comparing `tmp/joby_m_anthony_iii-3.1.8.tar.gz` & `tmp/joby_m_anthony_iii-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jmanthony1\Documents\GitHub\joby_m_anthony_iii\dist\.tmp-kd4kw2kv\joby_m_anthony_iii-3.1.8.tar", last modified: Mon Jan 30 02:27:06 2023, max compression
+gzip compressed data, was "C:\Users\jmanthony1\Documents\GitHub\joby_m_anthony_iii\dist\.tmp-7vp5m995\joby_m_anthony_iii-3.1.9.tar", last modified: Mon Jul 17 13:25:24 2023, max compression
```

## Comparing `joby_m_anthony_iii-3.1.8.tar` & `joby_m_anthony_iii-3.1.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/
--rw-rw-rw-   0        0        0     1094 2022-07-07 19:12:47.000000 joby_m_anthony_iii-3.1.8/LICENSE
--rw-rw-rw-   0        0        0     2770 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      976 2022-07-28 19:39:15.000000 joby_m_anthony_iii-3.1.8/README.md
--rw-rw-rw-   0        0        0      748 2023-01-30 02:25:11.000000 joby_m_anthony_iii-3.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/setup.cfg
--rw-rw-rw-   0        0        0      779 2022-07-08 12:47:43.000000 joby_m_anthony_iii-3.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii/
--rw-rw-rw-   0        0        0      540 2022-07-19 20:22:56.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii/__init__.py
--rw-rw-rw-   0        0        0   149382 2023-01-30 02:24:53.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii/numerical_methods.py
-drwxrwxrwx   0        0        0        0 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii.egg-info/
--rw-rw-rw-   0        0        0     2770 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-01-30 02:27:06.000000 joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/
+-rw-rw-rw-   0        0        0     1094 2022-07-07 19:12:47.000000 joby_m_anthony_iii-3.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2770 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2022-07-28 19:39:15.000000 joby_m_anthony_iii-3.1.9/README.md
+-rw-rw-rw-   0        0        0      748 2023-07-17 13:01:02.000000 joby_m_anthony_iii-3.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      779 2022-07-08 12:47:43.000000 joby_m_anthony_iii-3.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii/
+-rw-rw-rw-   0        0        0      540 2022-07-19 20:22:56.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii/__init__.py
+-rw-rw-rw-   0        0        0   149713 2023-07-17 13:14:47.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii/numerical_methods.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii.egg-info/
+-rw-rw-rw-   0        0        0     2770 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 13:25:24.000000 joby_m_anthony_iii-3.1.9/tests/
+-rw-rw-rw-   0        0        0    94131 2023-07-17 13:23:53.000000 joby_m_anthony_iii-3.1.9/tests/test_numerical_methods.py
```

### Comparing `joby_m_anthony_iii-3.1.8/LICENSE` & `joby_m_anthony_iii-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `joby_m_anthony_iii-3.1.8/PKG-INFO` & `joby_m_anthony_iii-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joby_m_anthony_iii
-Version: 3.1.8
+Version: 3.1.9
 Summary: Numerical methods/techniques.
 Author-email: "Joby M. Anthony III" <jmanthony1@liberty.edu>
 License: MIT License
         
         Copyright (c) 2022 Joby Anthony III
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `joby_m_anthony_iii-3.1.8/README.md` & `joby_m_anthony_iii-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `joby_m_anthony_iii-3.1.8/pyproject.toml` & `joby_m_anthony_iii-3.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=47", "wheel>=0.37.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joby_m_anthony_iii"
-version = "3.1.8"
+version = "3.1.9"
 description = "Numerical methods/techniques."
 readme = "README.md"
 authors = [{ name = "Joby M. Anthony III", email = "jmanthony1@liberty.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `joby_m_anthony_iii-3.1.8/setup.py` & `joby_m_anthony_iii-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii/__init__.py` & `joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii/__init__.py`

 * *Files identical despite different names*

### Comparing `joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii/numerical_methods.py` & `joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii/numerical_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -3207,38 +3207,44 @@
 		h: Optional[float]=None,
 		scheme: Optional[str]="open"
 	):
 		self.__domain_name, self.__function_name = "x", "f"#_retrieve_name(domain), _retrieve_name(function)
 		BadDomainError = lambda domain_name: f"Input domain, '{domain_name}' was not a one-dimensional array."
 		BadFunctionError = lambda function_name: f"Input range, '{function_name}' must be expression, not list or tuple."
 		if isinstance(domain, type(None)):
-			domain = np.arange(a, b+h, h)
-		elif np.sum(np.array(domain).shape) > np.sum(np.array(domain).shape[0]):
-			raise IndexError(BadDomainError(self.__domain_name))
+			self.domain = np.arange(a, b+h, h)
+		elif isinstance(domain, (list, tuple, np.ndarray)):
+			if np.sum(np.array(domain).shape) > np.sum(np.array(domain).shape[0]):
+				raise IndexError(BadDomainError(self.__domain_name))
+			else:
+				self.domain = np.array(domain)
+				if a == None: a = domain[0]
+				if b == None: b = domain[-1]
+				if h == None: h = domain[1] - domain[0]
 		else: raise IndexError(BadDomainError(self.__domain_name))
 		if isinstance(function, (list, tuple, np.ndarray)):
-			function = np.array(function)
+			self.function = np.array(function)
 		elif isinstance(function, FunctionType):
 			# if isinstance(function, str):
 			# 	self.function_str = function_str = ex.fast_parse_latex(function)
 			# 	function = lambda x: ex.fast_eval_latex(function_str, {variable: x})
-			self.function = function = make_array(domain, function)
+			self.function = make_array(self.domain, function)
 			#print("String expression converted to lambda function.")
 		#elif not isinstance(function,(FunctionType, sp.Expr)):
 		#	if np.sum(domain.shape) > np.sum(domain.shape[0]): raise ValueError("ERROR! " + bad_X)
 		#	else: raise ValueError("ERROR! " + bad_f)
 		else: raise TypeError(BadFunctionError(self.__function_name))
-		if isinstance(domain, type(None)):
-			self.domain = np.arange(a, b, h)
-		else:
-			self.domain = np.array(domain)
-			# self.variable = variable
-			if a == None: a = domain[0]
-			if b == None: b = domain[-1]
-			if h == None: h = domain[1]-domain[0]
+		# if isinstance(domain, type(None)):
+		# 	self.domain = np.arange(a, b, h)
+		# else:
+		# 	self.domain = np.array(domain)
+		# 	# self.variable = variable
+		# 	if a == None: a = domain[0]
+		# 	if b == None: b = domain[-1]
+		# 	if h == None: h = domain[1]-domain[0]
 		self.a, self.b, self.h = float(a), float(b), float(h)
 		self.scheme = scheme
 
 	def simpson(self) -> Tuple[np.ndarray, np.ndarray, float]:
 		r"""Gives exact result for polynomials of degree < 3 because error function utilizes the fourth derivative.
 
 		Notes
@@ -3257,17 +3263,17 @@
 			Domain and range used to calculate numeric integral.
 		F : float
 			Numeric integral.
 		"""
 		f, X = self.function, self.domain
 		a, b, h = self.a, self.b, self.h
 		if self.scheme == "open":
-			n = math.ceil((b-a)/h)
 			XJ1, XJ2, XJ, = [], [], [a]
 			YJ1, YJ2, YJ, = [], [], [f(a) if not isinstance(f, np.ndarray) else f[0]]
+			n = math.ceil((b-a)/h) if not isinstance(f, np.ndarray) else len(X) - 1
 			for j in range(1, int(n/2)):
 				XJ1.append(a + 2*j*h)
 				YJ1.append(f(XJ1[-1]) if not isinstance(f, np.ndarray) else f[2*j])
 			z1 = np.sum(YJ1)
 			for j in range(1, int(n/2+1)):
 				XJ2.append(a + (2*j - 1)*h)
 				YJ2.append(f(XJ2[-1]) if not isinstance(f, np.ndarray) else f[2*j-1])
@@ -3307,15 +3313,15 @@
 		F : float
 			Numeric integral.
 		"""
 		f, X = self.function, self.domain
 		a, b, h = self.a, self.b, self.h
 		if self.scheme == "open":
 			XJ, YJ = [a], [f(a) if not isinstance(f, np.ndarray) else f[0]]
-			n = math.ceil((b-a)/h)
+			n = math.ceil((b-a)/h) if not isinstance(f, np.ndarray) else len(X) - 1
 			for j in range(1, n):
 				XJ.append(a + j*h)
 				YJ.append(f(XJ[-1]) if not isinstance(f, np.ndarray) else f[j])
 			z = np.sum(YJ[1:])
 			XJ.append(b);
 			YJ.append(f(b) if not isinstance(f, np.ndarray) else f[-1])
 			X = XJ; Y = YJ
```

### Comparing `joby_m_anthony_iii-3.1.8/src/joby_m_anthony_iii.egg-info/PKG-INFO` & `joby_m_anthony_iii-3.1.9/src/joby_m_anthony_iii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joby-m-anthony-iii
-Version: 3.1.8
+Version: 3.1.9
 Summary: Numerical methods/techniques.
 Author-email: "Joby M. Anthony III" <jmanthony1@liberty.edu>
 License: MIT License
         
         Copyright (c) 2022 Joby Anthony III
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

