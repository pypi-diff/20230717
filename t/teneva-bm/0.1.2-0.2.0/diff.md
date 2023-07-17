# Comparing `tmp/teneva_bm-0.1.2.tar.gz` & `tmp/teneva_bm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.1.2.tar", last modified: Wed Jun 14 13:42:54 2023, max compression
+gzip compressed data, was "teneva_bm-0.2.0.tar", last modified: Mon Jul 17 20:18:42 2023, max compression
```

## Comparing `teneva_bm-0.1.2.tar` & `teneva_bm-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,47 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-14 13:42:54.231277 teneva_bm-0.1.2/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.1.2/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.1.2/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3733 2023-06-14 13:42:54.231426 teneva_bm-0.1.2/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2431 2023-06-14 13:42:10.000000 teneva_bm-0.1.2/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      978 2023-06-13 08:10:16.000000 teneva_bm-0.1.2/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-06-14 13:42:54.231930 teneva_bm-0.1.2/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2556 2023-04-26 15:12:02.000000 teneva_bm-0.1.2/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-14 13:42:54.228975 teneva_bm-0.1.2/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      919 2023-06-14 13:42:06.000000 teneva_bm-0.1.2/teneva_bm/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7346 2023-04-26 18:37:08.000000 teneva_bm-0.1.2/teneva_bm/bm.py
--rw-r--r--   0 andrei     (501) staff       (20)     2988 2023-04-26 18:32:42.000000 teneva_bm-0.1.2/teneva_bm/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2338 2023-04-26 18:36:21.000000 teneva_bm-0.1.2/teneva_bm/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-04-26 18:33:04.000000 teneva_bm-0.1.2/teneva_bm/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2333 2023-04-26 18:36:30.000000 teneva_bm-0.1.2/teneva_bm/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2778 2023-04-26 18:36:34.000000 teneva_bm-0.1.2/teneva_bm/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3007 2023-04-26 18:36:39.000000 teneva_bm-0.1.2/teneva_bm/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2462 2023-04-26 17:51:04.000000 teneva_bm-0.1.2/teneva_bm/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2374 2023-04-26 18:36:44.000000 teneva_bm-0.1.2/teneva_bm/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     2763 2023-04-26 18:36:49.000000 teneva_bm-0.1.2/teneva_bm/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3077 2023-04-26 18:36:52.000000 teneva_bm-0.1.2/teneva_bm/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2192 2023-04-26 18:33:36.000000 teneva_bm-0.1.2/teneva_bm/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     2702 2023-04-26 18:36:59.000000 teneva_bm-0.1.2/teneva_bm/bm_func_schwefel.py
--rw-r--r--   0 andrei     (501) staff       (20)     5259 2023-06-14 13:41:12.000000 teneva_bm-0.1.2/teneva_bm/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)     3127 2023-04-26 18:18:14.000000 teneva_bm-0.1.2/teneva_bm/bm_oc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     1702 2023-04-26 18:18:05.000000 teneva_bm-0.1.2/teneva_bm/bm_oc_simple_constr.py
--rw-r--r--   0 andrei     (501) staff       (20)     2902 2023-04-26 18:33:58.000000 teneva_bm-0.1.2/teneva_bm/bm_qubo_knap_amba.py
--rw-r--r--   0 andrei     (501) staff       (20)     1883 2023-04-26 18:14:29.000000 teneva_bm-0.1.2/teneva_bm/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2578 2023-04-26 18:14:02.000000 teneva_bm-0.1.2/teneva_bm/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2584 2023-04-26 18:13:28.000000 teneva_bm-0.1.2/teneva_bm/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)    11307 2023-04-26 18:12:04.000000 teneva_bm-0.1.2/teneva_bm/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1699 2023-04-26 18:34:12.000000 teneva_bm-0.1.2/teneva_bm/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-14 13:42:54.230963 teneva_bm-0.1.2/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3733 2023-06-14 13:42:54.000000 teneva_bm-0.1.2/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      858 2023-06-14 13:42:54.000000 teneva_bm-0.1.2/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-06-14 13:42:54.000000 teneva_bm-0.1.2/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-06-14 13:42:54.000000 teneva_bm-0.1.2/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-06-14 13:42:54.000000 teneva_bm-0.1.2/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.787340 teneva_bm-0.2.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.2.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.2.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    13380 2023-07-17 20:18:42.787765 teneva_bm-0.2.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    12119 2023-07-17 20:06:47.000000 teneva_bm-0.2.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      652 2023-07-17 09:21:50.000000 teneva_bm-0.2.0/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-17 20:18:42.789018 teneva_bm-0.2.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.2.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.769823 teneva_bm-0.2.0/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      169 2023-07-17 20:06:24.000000 teneva_bm-0.2.0/teneva_bm/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)    14607 2023-07-17 19:17:31.000000 teneva_bm-0.2.0/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.778434 teneva_bm-0.2.0/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.2.0/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-17 14:30:03.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2444 2023-07-17 14:32:24.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2423 2023-07-17 14:32:05.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2438 2023-07-17 14:32:52.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2886 2023-07-17 14:33:30.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3008 2023-07-17 14:34:01.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 14:34:28.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2550 2023-07-17 14:34:49.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2873 2023-07-17 14:35:06.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3189 2023-07-17 14:35:23.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2171 2023-07-17 14:35:48.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2824 2023-07-17 14:36:05.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.779935 teneva_bm-0.2.0/teneva_bm/oc/
+-rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.2.0/teneva_bm/oc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3326 2023-07-17 18:44:45.000000 teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2180 2023-07-17 18:45:47.000000 teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.783177 teneva_bm-0.2.0/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      168 2023-07-13 07:41:50.000000 teneva_bm-0.2.0/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2886 2023-07-17 19:08:37.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_amba.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1866 2023-07-17 19:22:24.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2662 2023-07-17 15:10:35.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2668 2023-07-17 19:22:18.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3270 2023-07-17 20:15:06.000000 teneva_bm-0.2.0/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.786674 teneva_bm-0.2.0/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.2.0/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6982 2023-07-17 20:05:20.000000 teneva_bm-0.2.0/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    11422 2023-07-17 19:32:33.000000 teneva_bm-0.2.0/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1919 2023-07-17 19:22:56.000000 teneva_bm-0.2.0/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.771859 teneva_bm-0.2.0/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    13380 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1105 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.1.2/LICENSE.txt` & `teneva_bm-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.2/setup.py` & `teneva_bm-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
         if not os.path.isdir(path):
             continue
         packages.extend(find_packages('%s.%s'%(package, name), path))
     return packages
 
 
 here = os.path.abspath(os.path.dirname(__file__))
-desc = 'Benchmarks library, based on a software product teneva, for tensor based multidimensional approximation and optimization methods'
+
+
+desc = 'Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods'
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     desc_long = f.read()
 
 
 with open(os.path.join(here, 'teneva_bm/__init__.py'), encoding='utf-8') as f:
     text = f.read()
     version = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", text, re.M)
@@ -36,36 +38,35 @@
     description=desc,
     long_description=desc_long,
     long_description_content_type='text/markdown',
     author='Andrei Chertkov',
     author_email='andre.chertkov@gmail.com',
     url='https://github.com/AndreiChertkov/teneva_bm',
     classifiers=[
-        'Development Status :: 3 - Alpha', # 4 - Beta, 5 - Production/Stable
+        'Development Status :: 4 - Beta', # 3 - Alpha, 5 - Production/Stable
         'License :: OSI Approved :: MIT License',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Framework :: Jupyter',
     ],
     keywords='benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition',
     packages=find_packages('teneva_bm', './teneva_bm/'),
     python_requires='>=3.8',
     project_urls={
         'Source': 'https://github.com/AndreiChertkov/teneva_bm',
     },
     license='MIT',
-    license_files = ('LICENSE.txt',),
+    license_files =('LICENSE.txt',),
 )
 
 
 if __name__ == '__main__':
     setup(
         **setup_args,
         install_requires=requirements,
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_ackley.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_ackley.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Ackley function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-32.768, 32.768]; the exact global minimum
+    is known: x = [0, ..., 0], y = 0.
     See https://www.sfu.ca/~ssurjano/ackley.html for details.
     See also the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("1. Ackley 1 Function"; Continuous, Differentiable, Non-separable,
     Scalable, Multimodal).
 """
@@ -76,34 +78,30 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncAckley().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_alpine.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_alpine.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Alpine function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-10, 10]; the exact global minimum
+    is known: x = [0, ..., 0], y = 0.
     See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("6. Alpine 1 Function"; Continuous, Non-Differentiable, Separable,
     Non-Scalable, Multimodal).
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
 class BmFuncAlpine(Bm):
     def __init__(self, d=50, n=15, name='FuncAlpine', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -46,40 +50,36 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncAlpine().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
+    text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_dixon.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_dixon.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Dixon function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-10, 10]; the exact global minimum
+    is known: x_i = 2^{(2^i-2) / 2^i} (i = 1, ..., d), y = 0.  Note that
+    this function achieves a global minimum at more than one point.
     See https://www.sfu.ca/~ssurjano/dixonpr.html for details.
     See also the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("48. Dixon & Price Function"; Continuous, Differentiable,
-    Non-Separable, Scalable, Unimodal). Note that this function achieves a
-    global minimum at more than one point.
+    Non-Separable, Scalable, Unimodal).
 """
 
 
 class BmFuncDixon(Bm):
     def __init__(self, d=50, n=15, name='FuncDixon', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -53,34 +55,30 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncDixon().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_exp.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_exp.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Exponential function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-1, 1]; the exact global minimum
+    is known: x = [0, ..., 0], y = -1.
     See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("54. Exponential Function"; Continuous, Differentiable,
     Non-Separable, Scalable, Multimodal).
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
 class BmFuncExp(Bm):
     def __init__(self, d=50, n=15, name='FuncExp', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -48,40 +52,36 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncExp().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
+    text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_griewank.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_qing.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,103 +2,87 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Griewank function (continuous).
+    Analytical Qing function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
-    See https://www.sfu.ca/~ssurjano/griewank.html for details.
-    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
+    Default grid limits are [0, 500] (note that we limit this function
+    to this domain instead of often used [-500, 500] to make sure it has
+    a single global minimum); the exact global minimum
+    is known: x_i = \sqrt{i} (i = 1, ..., d), y = 0.
+    See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("59. Griewank Function"; Continuous, Differentiable, Non-Separable,
+    ("98. Qing Function"; Continuous, Differentiable, Separable
     Scalable, Multimodal).
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
-class BmFuncGriewank(Bm):
-    def __init__(self, d=50, n=15, name='FuncGriewank', desc=DESC):
+class BmFuncQing(Bm):
+    def __init__(self, d=50, n=15, name='FuncQing', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-100., +100.)
+        self.set_grid(0., +500.)
 
         self.set_min(
-            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
-            x=[0.]*self.d,
+            x=np.sqrt(np.arange(1, self.d+1)),
             y=0.)
 
         self.with_cores = True
 
     @property
     def is_func(self):
         return True
 
     def _cores(self, X):
-        Y = self._cores_mul([np.cos(x/np.sqrt(i)) for i,x in enumerate(X.T,1)])
-        Y[-1] *= -1
-        return teneva.add(Y, self._cores_add([x**2 / 4000. for x in X.T], a0=1))
+        return self._cores_add([(x**2 - i)**2 for i, x in enumerate(X.T, 1)])
 
     def _f_batch(self, X):
-        y1 = np.sum(X**2, axis=1) / 4000
-
-        y2 = np.cos(X / np.sqrt(np.arange(self.d) + 1))
-        y2 = - np.prod(y2, axis=1)
-
-        y3 = 1.
-
-        return y1 + y2 + y3
+        return np.sum((X**2 - np.arange(1, self.d+1))**2, axis=1)
 
     def _f_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
 
-        y1 = torch.sum(x**2) / 4000
-
-        y2 = torch.cos(x / torch.sqrt(torch.arange(d) + 1.))
-        y2 = - torch.prod(y2)
-
-        y3 = 1.
-
-        return y1 + y2 + y3
+        return torch.sum((x**2 - torch.arange(1, d+1))**2)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncGriewank().prep()
+    bm = BmFuncQing().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
+    text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_michalewicz.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_michalewicz.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Michalewicz function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [0, pi]; the exact global minimum is known
+    only for the case of dimensions 2, 5, and 10; in this cases, only the
+    corresponding value of the function is known, but not the argument.
     See https://www.sfu.ca/~ssurjano/michal.html for details.
     See also Charlie Vanaret, Jean-Baptiste Gotteland, Nicolas Durand,
     Jean-Marc Alliot. "Certified global minima for a benchmark of difficult
     optimization problems". arXiv preprint arXiv:2003.09867 2020
     (the function has d! local minima, and it is multimodal).
-    Note that the value of the global minimum is known only for the case of
-    dimensions 2, 5, and 10. In this cases, only the corresponding value of
-    the function is known, but not the argument.
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
 class BmFuncMichalewicz(Bm):
     def __init__(self, d=50, n=15, name='FuncMichalewicz', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -71,34 +73,30 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncMichalewicz().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
+    text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_piston.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_piston.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Piston function (continuous).
-    The dimension is "7" and the mode size may be any (default is n=15).
+    The dimension is 7 and the mode size may be any (default is n=15),
+    each mode has its own (substantially different) limits.
     See Vitaly Zankin, Gleb Ryzhakov, Ivan Oseledets. "Gradient descent
     based D-optimal design for the least-squares polynomial approximation".
     arXiv preprint arXiv:1806.06631 2018 for details.
 """
 
 
 class BmFuncPiston(Bm):
@@ -67,28 +68,24 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncPiston().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_qing.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_schaffer.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,84 +2,75 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Qing function (continuous).
+    Analytical Schaffer function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-100, 100]; the exact global minimum
+    is known: x = [0, ..., 0], y = 0.
     See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("98. Qing Function"; Continuous, Differentiable, Separable
-    Scalable, Multimodal). Note that we limit this function to the
-    [0, 500] domain to make sure it has a single global minimum.
+    ("136. Schaffer F6 Function"; Continuous, Differentiable,
+    Non-Separable, Scalable, Multimodal).
 """
 
 
-class BmFuncQing(Bm):
-    def __init__(self, d=50, n=15, name='FuncQing', desc=DESC):
+class BmFuncSchaffer(Bm):
+    def __init__(self, d=50, n=15, name='FuncSchaffer', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(0., +500.)
+        self.set_grid(-100., +100.)
 
-        self.set_min(y=0., x=np.sqrt(np.arange(1, self.d+1)))
-
-        self.with_cores = True
+        self.set_min(
+            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
+            x=[0.]*self.d,
+            y=0.)
 
     @property
     def is_func(self):
         return True
 
-    def _cores(self, X):
-        return self._cores_add([(x**2 - i)**2 for i, x in enumerate(X.T, 1)])
-
     def _f_batch(self, X):
-        return np.sum((X**2 - np.arange(1, self.d+1))**2, axis=1)
+        Z = X[:, :-1]**2 + X[:, 1:]**2
+        Y = 0.5 + (np.sin(np.sqrt(Z))**2 - 0.5) / (1. + 0.001 * Z)**2
+        return np.sum(Y, axis=1)
 
     def _f_pt(self, x):
         """Draft."""
-        d = torch.tensor(self.d)
-
-        return torch.sum((x**2 - torch.arange(1, d+1))**2)
+        z = x[:-1]**2 + x[1:]**2
+        y = 0.5 + (torch.sin(torch.sqrt(z))**2 - 0.5) / (1. + 0.001 * z)**2
+        return torch.sum(y)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncQing().prep()
+    bm = BmFuncSchaffer().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
-    Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
-    text += f'{e:-10.1e}'
-    print(text)
-
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_rastrigin.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_rastrigin.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Rastrigin function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-5.12, 5.12]; the exact global minimum
+    is known: x = [0, ..., 0], y = 0.
     See https://www.sfu.ca/~ssurjano/rastr.html for details.
     See also the work Johannes M Dieterich, Bernd Hartke. "Empirical review
     of standard benchmark functions using evolutionary global optimization".
     Applied Mathematics 2012; 3:1552-1564.
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
 class BmFuncRastrigin(Bm):
     def __init__(self, d=50, n=15, name='FuncRastrigin', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -65,40 +69,36 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncRastrigin().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
+    text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_rosenbrock.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Rosenbrock function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-2.048, 2.048]; the exact global minimum
+    is known: x = [1, ..., 1], y = 0.
     See https://www.sfu.ca/~ssurjano/rosen.html for details.
     See also the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("105. Rosenbrock Function"; Continuous, Differentiable,
     Non-Separable, Scalable, Unimodal).
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
 class BmFuncRosenbrock(Bm):
     def __init__(self, d=50, n=15, name='FuncRosenbrock', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -69,40 +73,36 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncRosenbrock().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
+    text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_schaffer.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_griewank.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,77 +2,103 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Schaffer function (continuous).
+    Analytical Griewank function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
-    See the work Momin Jamil, Xin-She Yang. "A literature survey of
+    Default grid limits are [-100, 100]; the exact global minimum
+    is known: x = [0, ..., 0], y = 0.
+    See https://www.sfu.ca/~ssurjano/griewank.html for details.
+    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("136. Schaffer F6 Function"; Continuous, Differentiable,
-    Non-Separable, Scalable, Multimodal).
+    ("59. Griewank Function"; Continuous, Differentiable, Non-Separable,
+    Scalable, Multimodal).
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
-class BmFuncSchaffer(Bm):
-    def __init__(self, d=50, n=15, name='FuncSchaffer', desc=DESC):
+class BmFuncGriewank(Bm):
+    def __init__(self, d=50, n=15, name='FuncGriewank', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-100., +100.)
 
         self.set_min(
             i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
             x=[0.]*self.d,
             y=0.)
 
+        self.with_cores = True
+
     @property
     def is_func(self):
         return True
 
+    def _cores(self, X):
+        Y = self._cores_mul([np.cos(x/np.sqrt(i)) for i,x in enumerate(X.T,1)])
+        Y[-1] *= -1
+        return teneva.add(Y, self._cores_add([x**2 / 4000. for x in X.T], a0=1))
+
     def _f_batch(self, X):
-        Z = X[:, :-1]**2 + X[:, 1:]**2
-        Y = 0.5 + (np.sin(np.sqrt(Z))**2 - 0.5) / (1. + 0.001 * Z)**2
-        return np.sum(Y, axis=1)
+        y1 = np.sum(X**2, axis=1) / 4000
+
+        y2 = np.cos(X / np.sqrt(np.arange(self.d) + 1))
+        y2 = - np.prod(y2, axis=1)
+
+        y3 = 1.
+
+        return y1 + y2 + y3
 
     def _f_pt(self, x):
         """Draft."""
-        z = x[:-1]**2 + x[1:]**2
-        y = 0.5 + (torch.sin(torch.sqrt(z))**2 - 0.5) / (1. + 0.001 * z)**2
-        return torch.sum(y)
+        d = torch.tensor(self.d)
+
+        y1 = torch.sum(x**2) / 4000
+
+        y2 = torch.cos(x / torch.sqrt(torch.arange(d) + 1.))
+        y2 = - torch.prod(y2)
+
+        y3 = 1.
+
+        return y1 + y2 + y3
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncSchaffer().prep()
+    bm = BmFuncGriewank().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'TT-cores accuracy on train data          :  '
+    Y = bm.build_cores()
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
+    text += f'{e:-10.1e}'
+    print(text)
+
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_func_schwefel.py` & `teneva_bm-0.2.0/teneva_bm/func/bm_func_schwefel.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Schwefel function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
+    Default grid limits are [-500, 500]; the exact global minimum
+    is known: x = [420.9687, ..., 420.9687], y = 0.
     See https://www.sfu.ca/~ssurjano/schwef.html for details.
     See also the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("128. Schwefel 2.26 Function"; Continuous, Differentiable,
     Separable, Scalable, Multimodal).
+    Note that the method "build_cores" for construction of the function
+    in the TT-format on the discrete grid is available.
 """
 
 
 class BmFuncSchwefel(Bm):
     def __init__(self, d=50, n=15, name='FuncSchwefel', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -59,40 +63,36 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmFuncSchwefel().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'TT-cores accuracy on train data   :  '
+    text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
-    e = teneva.accuracy_on_data(Y, bm.I_trn, bm.y_trn)
+    e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_matmul.py` & `teneva_bm-0.2.0/teneva_bm/various/bm_matmul.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,33 +2,57 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Problem for fast size x size matrix multiplication (like Strassen
-    algorithm in the case size = 2) in terms of the tensor based
-    formulation (the search for the rank-7 CP decomposition is performed).
-    The dimension and mode size are determined automatically, but the rank
-    argument should be set manually in the case if size > 2 (e.g., for the
-    size = 3, the best known rank is 23).
+    Problem for fast "size x size" matrix multiplication (like Strassen
+    algorithm in the case "size = 2") in terms of the tensor based
+    formulation (e.g., the search for the rank-7 CP decomposition is
+    performed in the case of the "size = 2"). The objective function is
+    the norm of the difference between the exact tensor and the result of
+    multiplication using the chosen operations (determined by CP factors).
+    The dimension is determined automatically, but the rank argument should
+    be set manually in the case if "size > 2" (e.g., for the "size = 3", the
+    best known rank is "23"). The default mode size is "3", which relates to
+    a standard matrix multiplication task; in this case, we are looking for a
+    decomposition with factor matrix entries "-1, 0, 1". A mode size of "5"
+    is also supported, which relates to the possible values "-2, -1, 0, 1, 2".
+    If the "only2" flag is set during initialization, then only two factor
+    matrices will be constructed, and the third matrix will be restored as a
+    solution to the corresponding system of linear equations.
+    For more details, see the work Fawzi, A., et al. "Discovering faster
+    matrix multiplication algorithms with reinforcement learning." Nature
+    610.7930 (2022): 47-53.
 """
 
 
 class BmMatmul(Bm):
-    def __init__(self, name='Matmul', size=2, rank=7, desc=DESC, only2=False):
-        E = [-1, 0, 1] # Possible items of the factor matrices
-        T = _tensor_generate(size, size, size)
-        d = (2 if only2 else 3) * T.shape[0] * rank
-        n = len(E)
-
-        super().__init__(d, n, name, desc)
+    def __init__(self, d=None, n=3, name='Matmul', desc=DESC, size=2, rank=7,
+                 only2=False):
+        T_real = _tensor_generate(size, size, size)
+        d_real = (2 if only2 else 3) * size**2 * rank
+
+        super().__init__(d_real, n, name, desc)
+
+        if d is not None:
+            self.set_err('Dimension number (d) should not be set manually')
+
+        # Possible items of the factor matrices:
+        if n == 3:
+            E = [-1, 0, 1]
+        elif n == 5:
+            E = [-2, -1, 0, 1, 2]
+        else:
+            E = []
+            self.set_err('Invalid mode size. May be only 3 and 5')
 
-        if size == 2:
+        if size == 2 and n == 3:
+            # Strassen algorithm:
             self.set_min(i=np.array([
                 2, 1, 2, 1, 2, 0, 1,
                 1, 1, 1, 1, 2, 1, 2,
                 1, 2, 1, 1, 1, 2, 1,
                 2, 2, 1, 2, 1, 1, 0,
 
                 2, 2, 1, 0, 1, 2, 1,
@@ -38,28 +62,30 @@
 
                 2, 1, 1, 2, 0, 1, 2,
                 1, 1, 2, 1, 2, 1, 1,
                 1, 2, 1, 2, 1, 1, 1,
                 2, 0, 2, 1, 1, 2, 1], dtype=int),
                 y=0.)
 
-        self.T = T
+        self.T = T_real
         self.E = E
         self.size = size
         self.rank = rank
         self.only2 = only2
 
     @property
     def is_tens(self):
         return True
 
     def prep(self):
+        self.check_err()
+
         self.loss = _loss_build(self.T, self.E, self.rank, self.only2)
 
-        self._is_prep = True
+        self.is_prep = True
         return self
 
     def recover(self, i):
         x = _ind_to_poi(i, self.E)
 
         if self.only2:
             U, V = _factor_from_poi(x, self.rank, True)
@@ -69,68 +95,70 @@
 
         return U, V, W
 
     def _f(self, i):
         return self.loss(i)
 
 
-def _factor_from_poi(x, q, only2=False, order_spec=False):
-    """Build canonical rank-q factors from flatten "x"."""
+def _factor_from_poi(x, rank, only2=False, order_spec=False):
+    """Build canonical rank-"rank" factors from flatten "x"."""
     k = 2 if only2 else 3
-    n = x.size // (k * q)
+    n = x.size // (k * rank)
 
     if order_spec and not only2:
         raise ValueError('Is not supported')
+
     elif order_spec:
-        U = np.array([x[n*2*j:n*2*j+n] for j in range(q)]).T
-        V = np.array([x[n*2*j+n:n*2*j+2*n] for j in range(q)]).T
+        U = np.array([x[n*2*j:n*2*j+n] for j in range(rank)]).T
+        V = np.array([x[n*2*j+n:n*2*j+2*n] for j in range(rank)]).T
+
     else:
-        U = x[:n*q].reshape((n, q))
-        V = x[n*q:2*n*q].reshape((n, q))
+        U = x[:n*rank].reshape((n, rank))
+        V = x[n*rank:2*n*rank].reshape((n, rank))
 
     if only2:
         return U, V
 
-    W = x[2*n*q:].reshape((n, q))
+    W = x[2*n*rank:].reshape((n, rank))
 
     return U, V, W
 
 
 def _factor_recover(U, V, T):
     """Build 3th factor matrix from 2 given factor matrices and 3D tensor."""
     n = T.shape[-1]
-    q = U.shape[-1]
+    rank = U.shape[-1]
 
-    A = np.einsum('nr,mr->nmr', U, V).reshape(-1, q)
+    A = np.einsum('nr,mr->nmr', U, V).reshape(-1, rank)
     R = T.reshape(-1, n)
 
     W = np.linalg.lstsq(A, R, rcond=-1)[0].T
 
     return W
 
 
 def _ind_to_poi(I, E=[-1, 0, 1]):
     """Transform tensor multi-index into point from discrete values "E"."""
     return np.asarray(E)[list(I)]
 
 
-def _loss_build(T_real, E, q, only2=True, order_spec=False, fast=False):
+def _loss_build(T_real, E, rank, only2=True, order_spec=False, fast=False):
     """Prepare the loss function for the tensor based formulation."""
     if fast:
         T = T_real.reshape(-1, T_real.shape[-1])
 
     def loss(i):
         x = _ind_to_poi(i, E)
 
         if only2:
-            U, V = _factor_from_poi(x, q, True, order_spec)
+            U, V = _factor_from_poi(x, rank, True, order_spec)
             if not fast:
                 W = _factor_recover(U, V, T_real)
         else:
-            U, V, W = _factor_from_poi(x, q, False, order_spec)
+            U, V, W = _factor_from_poi(x, rank, False, order_spec)
 
         if only2 and fast:
             # NOTE: this code may be invalid now (compare with fast=False)
             A = np.einsum('nr,mr->nmr', U, V).reshape(-1, U.shape[-1])
             Q = np.linalg.qr(A)[0]
             D = T - Q @ (Q.T @ T)
             e = np.linalg.norm(D.reshape(-1))
@@ -155,36 +183,46 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmMatmul(size=2, rank=7).prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    if bm.size == 2:
-        text = 'Value at minimum (real vs calc)   :  '
+    if bm.size == 2 and bm.n[0] == 3:
+        text = 'Value at the minimum (real vs calc)      :  '
         y_real = bm.y_min_real
         y_calc = bm[bm.i_min_real]
-        text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+        text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
+        print(text)
 
+    text = 'Check "only2" case                       :  '
+    bm = BmMatmul(size=2, rank=7, only2=True).prep()
+    i = [np.random.choice(k) for k in bm.n]
+    y = bm[i]
+    text += f'{y:-10.3e}'
+    print(text)
+
+    text = 'Check "recover" error                    :  '
+    bm = BmMatmul(size=2, rank=7).prep()
+    U, V, W = bm.recover(bm.i_min_real)
+    T_appr = np.einsum('nr,mr,sr->nms', U, V, W)
+    e = np.linalg.norm(T_appr.reshape(-1) - bm.T.reshape(-1))
+    text += f'{e:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_oc_simple.py` & `teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,66 +9,66 @@
     with_gekko = False
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Discrete optimal control (OC) problem with simple 1D ODE "x**3 - i", where
-    "i" is a binary control variable.
+    Discrete optimal control (OC) problem with simple 1D ODE "x**3 - i",
+    where "x = x(t)" is a state variable, "x(0) = x_ini" and "i" is a
+    binary control variable. The loss function for the optimal control
+    problem is "0.5 * (x-x_ref)^2", where "x_ref" is a target value, and
+    the maximum time value is "t_max". Note that for some control values
+    the solver (gekko) fails, in this case we return the value "y_err".
+    By default (see parameters of the "set_opts" function), "x_ini = 0.8",
+    "x_ref = 0.7", "t_max = 1" and "y_err = 1.E+50".
     The dimension may be any (default is 50), and the mode size should be 2.
     The benchmark needs "gekko==1.0.6" library (it is used for ODE solution).
 """
 
 
 class BmOcSimple(Bm):
     def __init__(self, d=50, n=2, name='OcSimple', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n[0] != 2:
             self.set_err('Mode size (n) should be "2"')
         if not with_gekko:
-            self.set_err('Need "gekko" module')
+            msg = 'Need "gekko" module. For installation please run '
+            msg += '"pip install gekko==1.0.6"'
+            self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
-    def bm_constr(self, i):
-        """Constraint (optional)."""
-        return None
-
     def bm_ode(self, x, i):
         """Target ordinary differential equation (ODE)."""
         return x**3 - i
 
     def bm_obj(self, x, i):
         """Objective function for ODE solution."""
         return 0.5 * (x - self.opt_x_ref)**2
 
     def set_opts(self, x_ini=0.8, x_ref=0.7, t_max=1., y_err=1.E+50):
-        """Setting options specific to this benchmark.
+        """Setting options specific to the benchmark.
 
         Args:
             x_ini (float): initial condition for the ODE.
             x_ref (float): target (reference) value for solution of the ODE.
             t_max (float): upper limit for time variable in the ODE.
             y_err (float): returned value if GEKKO solver ends with error.
 
         """
         self.opt_x_ini = x_ini
         self.opt_x_ref = x_ref
         self.opt_times = np.linspace(0, t_max, self.d)
         self.opt_y_err = y_err
 
     def _f(self, i):
-        y_constr = self.bm_constr(i)
-        if y_constr is not None:
-            return y_constr
-
         solver = GEKKO(remote=False)
         solver.options.IMODE = 4
         solver.time = self.opt_times
 
         x = solver.Var(value=self.opt_x_ini, name='x')
         c = solver.Param(list(i), name='i')
         y = solver.Var(value=0.)
@@ -87,20 +87,16 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmOcSimple().prep()
     print(bm.info())
 
-    text = 'Range of y for 100 random samples : '
-    bm.build_trn(1.E+2)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+2)
+    print(bm.info_history())
 
     text = 'Value at a random multi-index     :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_oc_simple_constr.py` & `teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple_constr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import numpy as np
 import teneva
 
 
-from teneva_bm import BmOcSimple
+from teneva_bm.oc import BmOcSimple
 
 
 DESC = """
-    Discrete optimal control (OC) problem with simple 1D ODE "x**3 - i" and
-    constraint of the special form, where "i" is a binary control variable.
+    Discrete optimal control (OC) problem with constraint of the special
+    form. This benchmark is the same as "BmOcSimple", except the constraint.
+    Please see the description of BmOcSimple for more details. Note that in
+    the case if constraint fails, we return the penalty value "1.E+42".
     The dimension may be any (default is 50), and the mode size should be 2.
     The benchmark needs "gekko==1.0.6" library (it is used for ODE solution).
-    TODO: add options for constraint.
 """
 
 
 class BmOcSimpleConstr(BmOcSimple):
     def __init__(self, d=50, n=2, name='OcSimpleConstr', desc=DESC):
         super().__init__(d, n, name, desc)
 
-    def bm_constr(self, i):
-        """Constraint."""
-        v = 1.E+42
+        self.penalty_constr = 1.E+42
+        self.with_constr = True
+
+    def _constr(self, i):
         s = ''.join([str(k) for k in i])
-        if s.startswith('10'): return v
-        if s.startswith('110'): return v
-        if s.endswith('01'): return v
-        if s.endswith('011'): return v
-        if '010' in s: return v
-        if '0110' in s: return v
+
+        condition_false = False
+        condition_false = condition_false or s.startswith('10')
+        condition_false = condition_false or s.startswith('110')
+        condition_false = condition_false or s.startswith('01')
+        condition_false = condition_false or s.startswith('011')
+        condition_false = condition_false or s.startswith('010')
+        condition_false = condition_false or s.startswith('0110')
+
+        return not condition_false
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmOcSimpleConstr().prep()
     print(bm.info())
 
-    text = 'Range of y for 100 random samples : '
-    bm.build_trn(1.E+2)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+2)
+    print(bm.info_history())
 
     text = 'Value at a random multi-index     :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
@@ -53,7 +55,19 @@
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
+
+    text = 'Value at a valid multi-index      :  '
+    i = [1] * bm.d
+    y = bm[i]
+    text += f'{y:-10.3e}'
+    print(text)
+
+    text = 'Value at an invalid multi-index   :  '
+    i = [1, 0] + [0] * (bm.d-2)
+    y = bm[i]
+    text += f'{y:-10.3e}'
+    print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_qubo_knap_amba.py` & `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_amba.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 from teneva_bm import Bm
 
 
 DESC = """
     Binary knapsack problem with fixed weights wi in [5, 20], profits pi in
     [50, 100] (i = 1, 2, . . . , d) and the maximum capacity C = 1000. It is
-    from work (Dong et al., 2021) (problem k3; d = 50), where anglemodulated
-    bat algorithm (AMBA) algorithm was proposed for high-dimensional binary
+    from the work (Dong et al., 2021) (problem k3; d = 50), where angle
+    modulated bat algorithm (AMBA) was proposed for high-dimensional binary
     optimization problems with application to antenna topology optimization.
-    The dimension should be 50, and the mode size should be 2.
+    The dimension should be 50, and the mode size should be 2; the exact
+    global minimum is known: i = [1, 1, 0, ...] (see code), y = -3103.
 """
 
 
 class BmQuboKnapAmba(Bm):
     def __init__(self, d=50, n=2, name='QuboKnapAmba', desc=DESC):
         super().__init__(d, n, name, desc)
 
@@ -31,62 +32,60 @@
             y=-3103.)
 
     @property
     def is_tens(self):
         return True
 
     def prep(self):
+        self.check_err()
+        
         self.bm_w = [
             80, 82, 85, 70, 72, 70, 66, 50, 55, 25, 50, 55, 40, 48, 59, 32, 22,
             60, 30, 32, 40, 38, 35, 32, 25, 28, 30, 22, 50, 30, 45, 30, 60, 50,
             20, 65, 20, 25, 30, 10, 20, 25, 15, 10, 10, 10, 4, 4, 2, 1]
 
         self.bm_p = [
             220, 208, 198, 192, 180, 180, 165, 162, 160, 158, 155, 130, 125,
             122, 120, 118, 115, 110, 105, 101, 100, 100, 98, 96, 95, 90, 88, 82,
             80, 77, 75, 73, 72, 70, 69, 66, 65, 63, 60, 58, 56, 50, 30, 20, 15,
             10, 8, 5, 3, 1]
 
         self.bm_C = 1000
 
-        self._is_prep = True
+        self.is_prep = True
         return self
 
     def _f(self, i):
         cost = np.dot(self.bm_p, i)
         constr = np.dot(self.bm_w, i)
         return 0 if constr > self.bm_C else -cost
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboKnapAmba().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm[bm.i_min_real]
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_qubo_knap_quad.py` & `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,53 +23,53 @@
 class BmQuboKnapQuad(Bm):
     def __init__(self, d=50, n=2, name='QuboKnapQuad', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n[0] != 2:
             self.set_err('Mode size (n) should be "2"')
         if not with_qubogen:
-            self.set_err('Need "qubogen" module')
+            msg = 'Need "qubogen" module. For installation please run '
+            msg += '"pip install qubogen==0.1.1"'
+            self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
     def prep(self):
+        self.check_err()
+
         v = np.diag(np.random.random(self.d)) / 3.
         a = np.random.random(self.d)
         b = np.mean(a)
         self.bm_Q = qubogen.qubo_qkp(v, a, b)
 
-        self._is_prep = True
+        self.is_prep = True
         return self
 
     def _f_batch(self, I):
         return ((I @ self.bm_Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboKnapQuad().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_qubo_maxcut.py` & `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,35 +30,42 @@
 class BmQuboMaxcut(Bm):
     def __init__(self, d=50, n=2, name='QuboMaxcut', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n[0] != 2:
             self.set_err('Mode size (n) should be "2"')
         if not with_networkx:
-            self.set_err('Need "networkx" module')
+            msg = 'Need "networkx" module. For installation please run '
+            msg += '"pip install networkx==3.0"'
+            self.set_err(msg)
         if not with_qubogen:
-            self.set_err('Need "qubogen" module')
+            msg = 'Need "qubogen" module. For installation please run '
+            msg += '"pip install qubogen==0.1.1"'
+            self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
     def prep(self):
-        graph = nx.fast_gnp_random_graph(n=self.d, p=self.opt_prob_con,
-            seed=self.opt_seed)
+        self.check_err()
+
+        graph = nx.fast_gnp_random_graph(n=self.d,
+            p=self.opt_prob_con, seed=self.opt_seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
+
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
         self.bm_Q = qubogen.qubo_max_cut(g)
 
-        self._is_prep = True
+        self.is_prep = True
         return self
 
     def set_opts(self, prob_con=0.5, seed=42):
-        """Setting options specific to this benchmark.
+        """Setting options specific to the benchmark.
 
         Args:
             prob_con (float): probability of the connection in the graph.
             seed (int): seed for the random graph.
 
         """
         self.opt_prob_con = prob_con
@@ -70,28 +77,24 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboMaxcut().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_qubo_mvc.py` & `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,35 +30,42 @@
 class BmQuboMvc(Bm):
     def __init__(self, d=50, n=2, name='QuboMVC', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n[0] != 2:
             self.set_err('Mode size (n) should be "2"')
         if not with_networkx:
-            self.set_err('Need "networkx" module')
+            msg = 'Need "networkx" module. For installation please run '
+            msg += '"pip install networkx==3.0"'
+            self.set_err(msg)
         if not with_qubogen:
-            self.set_err('Need "qubogen" module')
+            msg = 'Need "qubogen" module. For installation please run '
+            msg += '"pip install qubogen==0.1.1"'
+            self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
     def prep(self):
+        self.check_err()
+
         graph = nx.fast_gnp_random_graph(n=self.d, p=self.opt_prob_con,
             seed=self.opt_seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
+
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
         self.bm_Q = qubogen.qubo_mvc(g)
 
-        self._is_prep = True
+        self.is_prep = True
         return self
 
     def set_opts(self, prob_con=0.5, seed=42):
-        """Setting options specific to this benchmark.
+        """Setting options specific to the benchmark.
 
         Args:
             prob_con (float): probability of the connection in the graph.
             seed (int): seed for the random graph.
 
         """
         self.opt_prob_con = prob_con
@@ -70,28 +77,24 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboMvc().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_topopt.py` & `teneva_bm-0.2.0/teneva_bm/various/bm_topopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,36 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Discrete Topology optimization task. This is draft!!!
-    The dimension and mode size are defined from nx and ny parameters.
+    Discrete Topology optimization task. This is a draft!!!
+    The dimension and mode size are defined from "nx" and "ny" parameters.
 """
 
 
 class BmTopopt(Bm):
-    def __init__(self, nx=128, ny=32, name='BmTopopt', desc=DESC):
-        super().__init__(nx*ny, 2, name, desc)
+    def __init__(self, d=None, n=2, name='BmTopopt', desc=DESC, nx=128, ny=32):
+        super().__init__(nx*ny, n, name, desc)
+
+        if d is not None:
+            self.set_err('Dimension number (d) should not be set manually')
+        if not self.is_n_equal or self.n[0] != 2:
+            self.set_err('Mode size (n) should be "2"')
 
         self.nx = nx
         self.ny = ny
 
     @property
     def is_tens(self):
         return True
 
-    def optimize_bm(self):
+    def optimize_baseline(self):
         solver = TopOptLite(self.nx, self.ny, self.opt_penal, self.opt_rmin)
         solver.init(Emin=1.E-9, Emax=1.0)
         solver.prep()
         x_ini = self.opt_k_frac * np.ones(self.nx * self.ny, dtype=float)
         x_opt = solver.solve(x_ini)
         return x_opt
 
@@ -47,18 +52,20 @@
 
         if fpath:
             plt.savefig(fpath, bbox_inches='tight')
         else:
             plt.show()
 
     def prep(self):
+        self.check_err()
+
         self.bm_f = topopt_lite(self.nx, self.ny,
             self.opt_k_frac, self.opt_penal, self.opt_rmin)
 
-        self._is_prep = True
+        self.is_prep = True
         return self
 
     def set_opts(self, k_frac=0.4, penal=3., rmin=5.4):
         """Setting options specific to this benchmark.
 
         Args:
             k_frac (float): ?.
@@ -329,28 +336,24 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmTopopt().prep()
     print(bm.info())
 
-    text = 'Range of y for 100 random samples : '
-    bm.build_trn(1.E+2)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+2)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
```

### Comparing `teneva_bm-0.1.2/teneva_bm/bm_wall_simple.py` & `teneva_bm-0.2.0/teneva_bm/various/bm_wall_simple.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Simple example of the special discrete function ("wall"), which is
-    difficult to optimize by tensor methods.
+    difficult to optimize by tensor methods. The exact global minimum
+    is known: i = [0, ..., 0], y = 0. The target function returns "0" if
+    the requested multi-index is optimal; returns a large number ("10 * d")
+    if the requested multi-index matches the optimal one in at least one
+    element; and returns the first element of the multi-index otherwise.
     The dimension and mode size may be any (default are d=10, n=50).
 """
 
 
 class BmWallSimple(Bm):
     def __init__(self, d=10, n=50, name='WallSimple', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_min(i=np.zeros(self.d, dtype=int), y=0.)
+        self.set_min(
+            i=np.zeros(self.d, dtype=int),
+            y=0.)
 
     @property
     def is_tens(self):
         return True
 
     def _f(self, i):
         if len(np.where(i == self.i_min_real)[0]) == self.d:
@@ -33,34 +39,30 @@
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmWallSimple().prep()
     print(bm.info())
 
-    text = 'Range of y for 10K random samples : '
-    bm.build_trn(1.E+4)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm[bm.i_min_real]
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

