# Comparing `tmp/amin_qvm-1.0.7.tar.gz` & `tmp/amin_qvm-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amin_qvm-1.0.7.tar", last modified: Fri Jun 16 16:05:26 2023, max compression
+gzip compressed data, was "amin_qvm-1.0.8.tar", last modified: Mon Jul 17 10:26:52 2023, max compression
```

## Comparing `amin_qvm-1.0.7.tar` & `amin_qvm-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 16:05:26.673110 amin_qvm-1.0.7/
--rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.7/LICENSE.ttxt
--rw-rw-rw-   0        0        0     7355 2023-06-16 16:05:26.666184 amin_qvm-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 16:05:26.571508 amin_qvm-1.0.7/amin_qvm/
--rw-rw-rw-   0        0        0    91665 2023-06-16 15:28:14.000000 amin_qvm-1.0.7/amin_qvm/QuantumComputer.py
--rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.7/amin_qvm/__init__.py
--rw-rw-rw-   0        0        0     4467 2023-06-16 15:25:30.000000 amin_qvm-1.0.7/amin_qvm/functions.py
--rw-rw-rw-   0        0        0      518 2023-06-16 11:00:36.000000 amin_qvm-1.0.7/amin_qvm/test.py
-drwxrwxrwx   0        0        0        0 2023-06-16 16:05:26.648566 amin_qvm-1.0.7/amin_qvm.egg-info/
--rw-rw-rw-   0        0        0     7355 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 16:05:26.674112 amin_qvm-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-06-16 15:29:06.000000 amin_qvm-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 10:26:52.104606 amin_qvm-1.0.8/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5462 2023-07-17 10:26:52.100606 amin_qvm-1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 10:26:52.100606 amin_qvm-1.0.8/amin_qvm/
+-rw-r--r--   0 runner    (1000) runner    (1000)    89367 2023-07-17 09:32:45.000000 amin_qvm-1.0.8/amin_qvm/QuantumComputer.py
+-rw-------   0 runner    (1000) runner    (1000)     4467 2023-07-17 09:32:45.000000 amin_qvm-1.0.8/amin_qvm/functions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 10:26:52.100606 amin_qvm-1.0.8/amin_qvm.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5462 2023-07-17 10:26:52.000000 amin_qvm-1.0.8/amin_qvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      232 2023-07-17 10:26:52.000000 amin_qvm-1.0.8/amin_qvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 10:26:52.000000 amin_qvm-1.0.8/amin_qvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       51 2023-07-17 10:26:52.000000 amin_qvm-1.0.8/amin_qvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 10:26:52.000000 amin_qvm-1.0.8/amin_qvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      550 2023-07-17 07:48:55.000000 amin_qvm-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 10:26:52.104606 amin_qvm-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1218 2023-07-17 10:26:35.000000 amin_qvm-1.0.8/setup.py
```

### Comparing `amin_qvm-1.0.7/amin_qvm/QuantumComputer.py` & `amin_qvm-1.0.8/amin_qvm/QuantumComputer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,24 @@
-#!/usr/bin/env python
-# Author: Amin Alogaili
-
 import numpy as np
 import unittest
 import re
 import random
 import itertools
 from functools import reduce
 from math import sqrt,pi,e,log
 import time
-
-def normalize_state(alpha, beta):
-    """Compute a normalized quantum state given arbitrary amplitudes.
-    
-    Args:
-        alpha (complex): The amplitude associated with the |0> state.
-        beta (complex): The amplitude associated with the |1> state.
-        
-    Returns:
-        array[complex]: A vector (numpy array) with 2 elements that represents
-        a normalized quantum state.
-    """
-
-    #[a', b'] BASED ON alpha AND beta SUCH THAT |a'|^2 + |b'|^2 = 1
-    normalized = alpha * ket_0 + beta * ket_1
-    normal = np.linalg.norm(normalized)
-    normalized = normalized/normal
-    return(normalized)
-
-def inner_product(state_1, state_2):
-    """Compute the inner product between two states.
-    
-    Args:
-        state_1 (array[complex]): A normalized quantum state vector
-        state_2 (array[complex]): A second normalized quantum state vector
-        
-    Returns:
-        complex: The value of the inner product <state_1 | state_2>.
-    """
- 
-    ##################
-    Conjugate = np.conjugate(state_1)
-    Inner = np.dot(Conjugate, state_2)
-    ##################
-    # COMPUTE AND RETURN THE INNER PRODUCT
-
-    return  Inner
-def feature_map(qc, data, qubits):
-    # Encode the data using a Pauli feature map
-    for i, value in enumerate(data):
-        qc.execute(f"rx({value * np.pi}) q[{qubits[i]}];")
-        qc.execute(f"rz({value * np.pi}) q[{qubits[i]}];")
-
-def estimate_inner_product(qc, qubits):
-    # Estimate the inner product of the quantum states
-    for qubit in qubits:
-        qc.execute(f"h q[{qubit}];")
-    for i in range(len(qubits) - 1):
-        qc.execute(f"cx q[{qubits[i]}], q[{qubits[i + 1]}];")
-    for qubit in qubits:
-        qc.execute(f"measure q[{qubit}];")
-    return np.mean([qc.qubits[qubit].get_state() for qubit in qubits])
-
-def apply_quantum_kernel(qc, training_data, test_data):
-    num_qubits = len(training_data[0])
-    qubits = [f"q{i}" for i in range(num_qubits)]
-
-    kernel_matrix = np.zeros((len(test_data), len(training_data)))
-
-    for i, test_point in enumerate(test_data):
-        qc.reset()
-        feature_map(qc, test_point, qubits)
-        for j, training_point in enumerate(training_data):
-            qc.reset()
-            feature_map(qc, training_point, qubits)
-            kernel_matrix[i, j] = estimate_inner_product(qc, qubits)
-
-    return kernel_matrix
-
+from funcs import *
+from microcontrollerconnectivity import *
+from base import *
+import sys
 ####
 ## Gates
 ####
 class Gate(object):
-	i_=np.complex(0,1)
+	i_= complex(0,1)
 	## One qubit gates
 	# Hadamard gate
 	H=1./sqrt(2)*np.matrix('1 1; 1 -1') 
 	# Pauli gates
 	X=np.matrix('0 1; 1 0')
 	Y=np.matrix([[0, -i_],[i_, 0]])
 	Z=np.matrix([[1,0],[0,-1]])
```

### Comparing `amin_qvm-1.0.7/amin_qvm/functions.py` & `amin_qvm-1.0.8/amin_qvm/functions.py`

 * *Files identical despite different names*

