# Comparing `tmp/Bgolearn-2.2.0.tar.gz` & `tmp/Bgolearn-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bgolearn-2.2.0.tar", last modified: Mon Jul 17 02:06:04 2023, max compression
+gzip compressed data, was "Bgolearn-2.2.1.tar", last modified: Mon Jul 17 03:33:33 2023, max compression
```

## Comparing `Bgolearn-2.2.0.tar` & `Bgolearn-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:06:04.810840 Bgolearn-2.2.0/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:06:04.809801 Bgolearn-2.2.0/Bgolearn/
--rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.2.0/Bgolearn/BGO_eval.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.2.0/Bgolearn/BGOclf.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.2.0/Bgolearn/BGOmax.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.2.0/Bgolearn/BGOmin.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    21169 2023-06-17 08:28:15.000000 Bgolearn-2.2.0/Bgolearn/BGOsampling.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     1129 2023-07-17 01:55:17.000000 Bgolearn-2.2.0/Bgolearn/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:06:04.810543 Bgolearn-2.2.0/Bgolearn.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      300 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       43 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 02:06:04.810714 Bgolearn-2.2.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.2.0/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-17 02:06:04.810881 Bgolearn-2.2.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-07-17 02:05:54.000000 Bgolearn-2.2.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 03:33:33.042426 Bgolearn-2.2.1/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 03:33:33.041480 Bgolearn-2.2.1/Bgolearn/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    24206 2023-07-17 02:28:21.000000 Bgolearn-2.2.1/Bgolearn/BGO_eval.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     3956 2023-07-17 03:25:17.000000 Bgolearn-2.2.1/Bgolearn/BGOclf.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18384 2023-07-17 02:35:43.000000 Bgolearn-2.2.1/Bgolearn/BGOmax.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18347 2023-07-17 02:40:08.000000 Bgolearn-2.2.1/Bgolearn/BGOmin.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    21894 2023-07-17 03:26:08.000000 Bgolearn-2.2.1/Bgolearn/BGOsampling.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     2472 2023-07-17 03:31:27.000000 Bgolearn-2.2.1/Bgolearn/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 03:33:33.042087 Bgolearn-2.2.1/Bgolearn.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      300 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       43 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 03:33:33.042283 Bgolearn-2.2.1/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.2.1/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-17 03:33:33.042474 Bgolearn-2.2.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-07-17 03:33:07.000000 Bgolearn-2.2.1/setup.py
```

### Comparing `Bgolearn-2.2.0/Bgolearn/BGO_eval.py` & `Bgolearn-2.2.1/Bgolearn/BGO_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     # [[],[],...]
     Total_area = 0
     for i in range(len(array)):
         Total_area += cal_area(array[i],length)
     return Total_area
 
 class BGO_Efficient(object):
-    def __init__(self,Ture_fun,Def_Domain, Kriging_model, opt_num, ret_noise,min_search):
+    def __init__(self,Ture_fun,Def_Domain, Kriging_model, opt_num, ret_noise, min_search):
         
         self.Ture_fun = Ture_fun
         self.Def_Domain = np.array(Def_Domain) 
         self.dim = len(pd.DataFrame(self.Def_Domain).iloc[0,:])
         self.total_space = len(self.Def_Domain)
         self.Ymax = Ture_fun(self.Def_Domain).max()
         self.Ymin = Ture_fun(self.Def_Domain).min()
```

### Comparing `Bgolearn-2.2.0/Bgolearn/BGOclf.py` & `Bgolearn-2.2.1/Bgolearn/BGOclf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import warnings
 import numpy as np
 
 class Boundary(object):
-    def __init__(self,model,data_matrix, Measured_response, virtual_samples, opt_num):
+    def __init__(self,model,data_matrix, Measured_response, virtual_samples, opt_num, scale_virtual_samples):
         warnings.filterwarnings('ignore')
         self.model = model
         self.data_matrix = np.array(data_matrix)
         self.Measured_response = np.array(Measured_response)
         __fea_num = len(self.data_matrix[0])
         self.virtual_samples = np.array(virtual_samples).reshape(-1,__fea_num)
-        self.probs = model.fit(data_matrix, Measured_response).predict_proba(self.virtual_samples)
+        self.probs = model.fit(data_matrix, Measured_response).predict_proba(scale_virtual_samples)
         self.opt_num = opt_num
         
 
     def Least_cfd(self,):
         Lc = []
         for i in range(len(self.probs)):
             max_pro = np.array(self.probs[i]).max()
```

### Comparing `Bgolearn-2.2.0/Bgolearn/BGOmax.py` & `Bgolearn-2.2.1/Bgolearn/BGOmax.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 from scipy.stats import norm
 
 # cal norm prob.
 def norm_des(x):
     return 1 / np.sqrt(2 * np.pi) * np.exp(- x ** 2 / 2)
 
 class Global_max(object):
-    def __init__(self,Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise):
+    def __init__(self,Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise,row_features):
         self.Kriging_model = Kriging_model
         self.data_matrix = np.array(data_matrix)
         self.Measured_response = np.array(Measured_response)
         __fea_num = len(self.data_matrix[0])
         self.virtual_samples = np.array(virtual_samples).reshape(-1,__fea_num)
         if ret_noise == 0:
             self.virtual_samples_mean, self.virtual_samples_std = self.Kriging_model().fit_pre(
                 self.data_matrix, self.Measured_response, self.virtual_samples)
         else:
             self.virtual_samples_mean, self.virtual_samples_std = self.Kriging_model().fit_pre(
                 self.data_matrix, self.Measured_response, self.virtual_samples,0.0)
         self.opt_num = opt_num
         self.ret_noise = ret_noise
+        self.row_features = row_features
         warnings.filterwarnings('ignore')
    
     
     
     def EI(self,):
         cur_optimal_value = self.Measured_response.max()
         print('current optimal is :', cur_optimal_value)
@@ -37,21 +38,21 @@
             EI_list.append(EI)
        
         EI_list = np.array(EI_list)
         
         return_x = []
         if self.opt_num == 1:
             EI_opt_index = np.random.choice(np.flatnonzero(EI_list == EI_list.max()))
-            print('The next datum recomended by Expected Improvement : \n x = ', self.virtual_samples[EI_opt_index])
-            return_x.append(self.virtual_samples[EI_opt_index])
+            print('The next datum recomended by Expected Improvement : \n x = ', self.row_features[EI_opt_index])
+            return_x.append(self.row_features[EI_opt_index])
         elif type(self.opt_num) == int:
             EI_opt_index = np.argpartition(EI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(EI_opt_index)):
-                print('The {num}-th datum recomended by Expected Improvement : \n x = '.format(num =j+1), self.virtual_samples[EI_opt_index[j]])
-                return_x.append(self.virtual_samples[EI_opt_index[j]])
+                print('The {num}-th datum recomended by Expected Improvement : \n x = '.format(num =j+1), self.row_features[EI_opt_index[j]])
+                return_x.append(self.row_features[EI_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return EI_list,np.array(return_x)
 
     
     
     def EI_plugin(self,):
@@ -69,21 +70,21 @@
             EIp_list.append(EIp)
        
         EIp_list = np.array(EIp_list)
         
         return_x = []
         if self.opt_num == 1:
             EIp_opt_index = np.random.choice(np.flatnonzero(EIp_list == EIp_list.max()))
-            print('The next datum recomended by Expected Improvement with plugin : \n x = ', self.virtual_samples[EIp_opt_index])
-            return_x.append(self.virtual_samples[EIp_opt_index])
+            print('The next datum recomended by Expected Improvement with plugin : \n x = ', self.row_features[EIp_opt_index])
+            return_x.append(self.row_features[EIp_opt_index])
         elif type(self.opt_num) == int:
             EIp_opt_index = np.argpartition(EIp_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(EIp_opt_index)):
-                print('The {num}-th datum recomended by Expected Improvement with plugin : \n x = '.format(num =j+1), self.virtual_samples[EIp_opt_index[j]])
-                return_x.append(self.virtual_samples[EIp_opt_index[j]])
+                print('The {num}-th datum recomended by Expected Improvement with plugin : \n x = '.format(num =j+1), self.row_features[EIp_opt_index[j]])
+                return_x.append(self.row_features[EIp_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return EIp_list,np.array(return_x)
     
     
     def Augmented_EI(self, alpha = 1, tao = 0):
         """
@@ -107,21 +108,21 @@
             AEI = EI * (1 - tao/np.sqrt(self.virtual_samples_std[i]**2 + tao**2))
             AEI_list.append(AEI)
         AEI_list = np.array(AEI_list)
         
         return_x =[]
         if self.opt_num == 1:
             AEI_opt_index = np.random.choice(np.flatnonzero(AEI_list == AEI_list.max()))
-            print('The next datum recomended by Augmented_EI : \n x = ', self.virtual_samples[AEI_opt_index])
-            return_x.append(self.virtual_samples[AEI_opt_index])
+            print('The next datum recomended by Augmented_EI : \n x = ', self.row_features[AEI_opt_index])
+            return_x.append(self.row_features[AEI_opt_index])
         elif type(self.opt_num) == int:
             AEI_opt_index = np.argpartition(AEI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(AEI_opt_index)):
-                print('The {num}-th datum recomended by Augmented_EI : \n x = '.format(num =j+1), self.virtual_samples[AEI_opt_index[j]])
-                return_x.append(self.virtual_samples[AEI_opt_index[j]])
+                print('The {num}-th datum recomended by Augmented_EI : \n x = '.format(num =j+1), self.row_features[AEI_opt_index[j]])
+                return_x.append(self.row_features[AEI_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
 
         return AEI_list,np.array(return_x)
 
     def EQI(self, beta = 0.5,tao_new = 0):
         """
@@ -147,21 +148,21 @@
             EQI = (__mean[i] - cur_optimal_value) * norm.cdf( Var_Z ) + __std[i] * norm_des(Var_Z)
             EQI_list.append(EQI)
         EQI_list = np.array(EQI_list)
         
         return_x = []
         if self.opt_num == 1:
             EQI_opt_index = np.random.choice(np.flatnonzero(EQI_list == EQI_list.max()))
-            print('The next datum recomended by Expected Quantile Improvement : \n x = ', self.virtual_samples[EQI_opt_index])
-            return_x.append(self.virtual_samples[EQI_opt_index])    
+            print('The next datum recomended by Expected Quantile Improvement : \n x = ', self.row_features[EQI_opt_index])
+            return_x.append(self.row_features[EQI_opt_index])    
         elif type(self.opt_num) == int:
             EQI_opt_index = np.argpartition(EQI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(EQI_opt_index)):
-                print('The {num}-th datum recomended by Expected Quantile Improvement : \n x = '.format(num =j+1), self.virtual_samples[EQI_opt_index[j]])
-                return_x.append(self.virtual_samples[EQI_opt_index[j]])
+                print('The {num}-th datum recomended by Expected Quantile Improvement : \n x = '.format(num =j+1), self.row_features[EQI_opt_index[j]])
+                return_x.append(self.row_features[EQI_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
 
         return EQI_list,np.array(return_x)
 
 
     def Reinterpolation_EI(self, ):
@@ -183,21 +184,21 @@
             REI_list.append(REI)
        
         REI_list = np.array(REI_list)
         
         return_x = []
         if self.opt_num == 1:
             REI_opt_index = np.random.choice(np.flatnonzero(REI_list == REI_list.max()))
-            print('The next datum recomended by Reinterpolation Expected Improvement : \n x = ', self.virtual_samples[REI_opt_index])
-            return_x.append(self.virtual_samples[REI_opt_index])
+            print('The next datum recomended by Reinterpolation Expected Improvement : \n x = ', self.row_features[REI_opt_index])
+            return_x.append(self.row_features[REI_opt_index])
         elif type(self.opt_num) == int:
             REI_opt_index = np.argpartition(REI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(REI_opt_index)):
-                print('The {num}-th datum recomended by Reinterpolation Expected Improvement : \n x = '.format(num =j+1), self.virtual_samples[REI_opt_index[j]])
-                return_x.append(self.virtual_samples[REI_opt_index[j]])
+                print('The {num}-th datum recomended by Reinterpolation Expected Improvement : \n x = '.format(num =j+1), self.row_features[REI_opt_index[j]])
+                return_x.append(self.row_features[REI_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return REI_list,np.array(return_x)
 
 
 
     def UCB(self, alpha=1):
@@ -205,21 +206,21 @@
         :param alpha: tradeoff coefficient, default 1
         """
         UCB_list = np.array(self.virtual_samples_mean) + alpha * np.array(self.virtual_samples_std)
         
         return_x = []
         if self.opt_num == 1:
             UCB_opt_index = np.random.choice(np.flatnonzero(UCB_list == UCB_list.max()))
-            print('The next datum recomended by Upper confidence bound  : \n x = ', self.virtual_samples[UCB_opt_index])
-            return_x.append(self.virtual_samples[UCB_opt_index])
+            print('The next datum recomended by Upper confidence bound  : \n x = ', self.row_features[UCB_opt_index])
+            return_x.append(self.row_features[UCB_opt_index])
         elif type(self.opt_num) == int:
             UCB_opt_index = np.argpartition(UCB_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(UCB_opt_index)):
-                print('The {num}-th datum recomended by Upper confidence bound : \n x = '.format(num =j+1), self.virtual_samples[UCB_opt_index[j]])
-                return_x.append(self.virtual_samples[UCB_opt_index[j]])
+                print('The {num}-th datum recomended by Upper confidence bound : \n x = '.format(num =j+1), self.row_features[UCB_opt_index[j]])
+                return_x.append(self.row_features[UCB_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
 
         return UCB_list,np.array(return_x)
     
     def PoI(self, tao = 0):
         """
@@ -237,21 +238,21 @@
                 PoI_list.append(PoI)
         
             PoI_list = np.array(PoI_list)
             
             return_x = []
             if self.opt_num == 1:
                 PoI_opt_index = np.random.choice(np.flatnonzero(PoI_list == PoI_list.max()))
-                print('The next datum recomended by Probability of Improvement  : \n x = ', self.virtual_samples[PoI_opt_index])
-                return_x.append(self.virtual_samples[PoI_opt_index])
+                print('The next datum recomended by Probability of Improvement  : \n x = ', self.row_features[PoI_opt_index])
+                return_x.append(self.row_features[PoI_opt_index])
             elif type(self.opt_num) == int:
                 PoI_opt_index = np.argpartition(PoI_list, -self.opt_num)[-self.opt_num:]
                 for j in range(len(PoI_opt_index)):
-                    print('The {num}-th datum recomended by Probability of Improvement  : \n x = '.format(num =j+1), self.virtual_samples[PoI_opt_index[j]])
-                    return_x.append(self.virtual_samples[PoI_opt_index[j]])
+                    print('The {num}-th datum recomended by Probability of Improvement  : \n x = '.format(num =j+1), self.row_features[PoI_opt_index[j]])
+                    return_x.append(self.row_features[PoI_opt_index[j]])
             else:
                 print('The input para. opt_num must be an int')
             return PoI_list,np.array(return_x)
     
     def Thompson_sampling(self,):
         # x* is derived by searching at the vistual space 
         # sample = np.len(virtual_samples)
@@ -291,21 +292,21 @@
         estimated_Entropy_y_conditional = Entropy_y_conditional / sam_num            
         PES_list = Entropy_y_ori - estimated_Entropy_y_conditional
         
 
         return_x = []
         if self.opt_num == 1:
             PES_opt_index = np.random.choice(np.flatnonzero(PES_list == PES_list.max()))
-            print('The next datum recomended by Predictive Entropy Search  : \n x = ', self.virtual_samples[PES_opt_index])
-            return_x.append(self.virtual_samples[PES_opt_index])
+            print('The next datum recomended by Predictive Entropy Search  : \n x = ', self.row_features[PES_opt_index])
+            return_x.append(self.row_features[PES_opt_index])
         elif type(self.opt_num) == int:
             PES_opt_index = np.argpartition(PES_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(PES_opt_index)):
-                print('The {num}-th datum recomended by Predictive Entropy Search  : \n x = '.format(num =j+1), self.virtual_samples[PES_opt_index[j]])
-                return_x.append(self.virtual_samples[PES_opt_index[j]])
+                print('The {num}-th datum recomended by Predictive Entropy Search  : \n x = '.format(num =j+1), self.row_features[PES_opt_index[j]])
+                return_x.append(self.row_features[PES_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return PES_list,np.array(return_x)
     
 
     def Knowledge_G(self,MC_num = 50):
         """
@@ -337,18 +338,18 @@
             MC_result = MC_batch_max / MC_num
             KD_list.append( MC_result - current_max)
         KD_list = np.array(KD_list)
         
         return_x = []
         if self.opt_num == 1:
             KD_opt_index = np.random.choice(np.flatnonzero(KD_list == KD_list.max()))
-            print('The next datum recomended by Knowledge Gradient : \n x = ', self.virtual_samples[KD_opt_index])
-            return_x.append(self.virtual_samples[KD_opt_index])
+            print('The next datum recomended by Knowledge Gradient : \n x = ', self.row_features[KD_opt_index])
+            return_x.append(self.row_features[KD_opt_index])
         elif type(self.opt_num) == int:
             KD_opt_index = np.argpartition(KD_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(KD_opt_index)):
-                print('The {num}-th datum recomended by Knowledge Gradient : \n x = '.format(num =j+1), self.virtual_samples[KD_opt_index[j]])
-                return_x.append(self.virtual_samples[KD_opt_index[j]])
+                print('The {num}-th datum recomended by Knowledge Gradient : \n x = '.format(num =j+1), self.row_features[KD_opt_index[j]])
+                return_x.append(self.row_features[KD_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return KD_list,np.array(return_x)
```

### Comparing `Bgolearn-2.2.0/Bgolearn/BGOmin.py` & `Bgolearn-2.2.1/Bgolearn/BGOmin.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 from scipy.stats import norm
 
 # cal norm prob.
 def norm_des(x):
     return 1 / np.sqrt(2 * np.pi) * np.exp(- x ** 2 / 2)
 
 class Global_min(object):
-    def __init__(self,Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise):
+    def __init__(self,Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise, row_features):
         self.Kriging_model = Kriging_model
         self.data_matrix = np.array(data_matrix)
         self.Measured_response = np.array(Measured_response)
         __fea_num = len(self.data_matrix[0])
         self.virtual_samples = np.array(virtual_samples).reshape(-1,__fea_num)
         if ret_noise == 0:
             self.virtual_samples_mean, self.virtual_samples_std = self.Kriging_model().fit_pre(
                 self.data_matrix, self.Measured_response, self.virtual_samples)
         else:
             self.virtual_samples_mean, self.virtual_samples_std = self.Kriging_model().fit_pre(
                 self.data_matrix, self.Measured_response, self.virtual_samples,0.0)
         self.opt_num = opt_num
         self.ret_noise = ret_noise
+        self.row_features = row_features
         warnings.filterwarnings('ignore')
    
     
     
     def EI(self,):
         cur_optimal_value = self.Measured_response.min()
         print('current optimal is :', cur_optimal_value)
@@ -36,27 +37,25 @@
             EI_list.append(EI)
        
         EI_list = np.array(EI_list)
 
         return_x = []
         if self.opt_num == 1:
             EI_opt_index = np.random.choice(np.flatnonzero(EI_list == EI_list.max()))
-            print('The next datum recomended by Expected Improvement : \n x = ', self.virtual_samples[EI_opt_index])
-            return_x.append(self.virtual_samples[EI_opt_index])
+            print('The next datum recomended by Expected Improvement : \n x = ', self.row_features[EI_opt_index])
+            return_x.append(self.row_features[EI_opt_index])
         elif type(self.opt_num) == int:
             EI_opt_index = np.argpartition(EI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(EI_opt_index)):
-                print('The {num}-th datum recomended by Expected Improvement : \n x = '.format(num =j+1), self.virtual_samples[EI_opt_index[j]])
-                return_x.append(self.virtual_samples[EI_opt_index[j]])
+                print('The {num}-th datum recomended by Expected Improvement : \n x = '.format(num =j+1), self.row_features[EI_opt_index[j]])
+                return_x.append(self.row_features[EI_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return EI_list, np.array(return_x)
 
-    
-    
     def EI_plugin(self,):
         if self.ret_noise == 0:
             __train_ypre,_ = self.Kriging_model().fit_pre(self.data_matrix,self.Measured_response, self.data_matrix)
         else:
             __train_ypre,_ = self.Kriging_model().fit_pre(self.data_matrix,self.Measured_response, self.data_matrix,0.0)
         cur_optimal_value = __train_ypre.min()
         print('current optimal is :', cur_optimal_value)
@@ -68,21 +67,21 @@
             EIp_list.append(EIp)
        
         EIp_list = np.array(EIp_list)
         
         return_x = []
         if self.opt_num == 1:
             EIp_opt_index = np.random.choice(np.flatnonzero(EIp_list == EIp_list.max()))
-            print('The next datum recomended by Expected Improvement with plugin : \n x = ', self.virtual_samples[EIp_opt_index])
-            return_x.append(self.virtual_samples[EIp_opt_index])    
+            print('The next datum recomended by Expected Improvement with plugin : \n x = ', self.row_features[EIp_opt_index])
+            return_x.append(self.row_features[EIp_opt_index])    
         elif type(self.opt_num) == int:
             EIp_opt_index = np.argpartition(EIp_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(EIp_opt_index)):
-                print('The {num}-th datum recomended by Expected Improvement with plugin : \n x = '.format(num =j+1), self.virtual_samples[EIp_opt_index[j]])
-                return_x.append(self.virtual_samples[EIp_opt_index[j]])
+                print('The {num}-th datum recomended by Expected Improvement with plugin : \n x = '.format(num =j+1), self.row_features[EIp_opt_index[j]])
+                return_x.append(self.row_features[EIp_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return EIp_list,np.array(return_x)
     
     
     def Augmented_EI(self, alpha = 1, tao = 0):
         """
@@ -106,21 +105,21 @@
             AEI = EI * (1 - tao/np.sqrt(self.virtual_samples_std[i]**2 + tao**2))
             AEI_list.append(AEI)
         AEI_list = np.array(AEI_list)
         
         return_x = []
         if self.opt_num == 1:
             AEI_opt_index = np.random.choice(np.flatnonzero(AEI_list == AEI_list.max()))
-            print('The next datum recomended by Augmented_EI : \n x = ', self.virtual_samples[AEI_opt_index])
-            return_x.append(self.virtual_samples[AEI_opt_index])
+            print('The next datum recomended by Augmented_EI : \n x = ', self.row_features[AEI_opt_index])
+            return_x.append(self.row_features[AEI_opt_index])
         elif type(self.opt_num) == int:
             AEI_opt_index = np.argpartition(AEI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(AEI_opt_index)):
-                print('The {num}-th datum recomended by Augmented_EI : \n x = '.format(num =j+1), self.virtual_samples[AEI_opt_index[j]])
-                return_x.append(self.virtual_samples[AEI_opt_index[j]]) 
+                print('The {num}-th datum recomended by Augmented_EI : \n x = '.format(num =j+1), self.row_features[AEI_opt_index[j]])
+                return_x.append(self.row_features[AEI_opt_index[j]]) 
         else:
             print('The input para. opt_num must be an int')
 
         return AEI_list,np.array(return_x)
 
     def EQI(self, beta = 0.5,tao_new = 0):
         """
@@ -146,21 +145,21 @@
             EQI = (cur_optimal_value - __mean[i]) * norm.cdf( Var_Z ) + __std[i] * norm_des(Var_Z)
             EQI_list.append(EQI)
         EQI_list = np.array(EQI_list)
         
         return_x = []
         if self.opt_num == 1:
             EQI_opt_index = np.random.choice(np.flatnonzero(EQI_list == EQI_list.max()))
-            print('The next datum recomended by Expected Quantile Improvement : \n x = ', self.virtual_samples[EQI_opt_index])
-            return_x.append(self.virtual_samples[EQI_opt_index])
+            print('The next datum recomended by Expected Quantile Improvement : \n x = ', self.row_features[EQI_opt_index])
+            return_x.append(self.row_features[EQI_opt_index])
         elif type(self.opt_num) == int:
             EQI_opt_index = np.argpartition(EQI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(EQI_opt_index)):
-                print('The {num}-th datum recomended by Expected Quantile Improvement : \n x = '.format(num =j+1), self.virtual_samples[EQI_opt_index[j]])
-                return_x.append(self.virtual_samples[EQI_opt_index[j]])
+                print('The {num}-th datum recomended by Expected Quantile Improvement : \n x = '.format(num =j+1), self.row_features[EQI_opt_index[j]])
+                return_x.append(self.row_features[EQI_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
 
         return EQI_list,np.array(return_x)
 
     def Reinterpolation_EI(self, ):
         if self.ret_noise == 0: 
@@ -181,43 +180,41 @@
             REI_list.append(REI)
        
         REI_list = np.array(REI_list)
         
         return_x = []
         if self.opt_num == 1:
             REI_opt_index = np.random.choice(np.flatnonzero(REI_list == REI_list.max()))
-            print('The next datum recomended by Reinterpolation Expected Improvement : \n x = ', self.virtual_samples[REI_opt_index])
-            return_x.append(self.virtual_samples[REI_opt_index])
+            print('The next datum recomended by Reinterpolation Expected Improvement : \n x = ', self.row_features[REI_opt_index])
+            return_x.append(self.row_features[REI_opt_index])
         elif type(self.opt_num) == int:
             REI_opt_index = np.argpartition(REI_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(REI_opt_index)):
-                print('The {num}-th datum recomended by Reinterpolation Expected Improvement : \n x = '.format(num =j+1), self.virtual_samples[REI_opt_index[j]])
-                return_x.append(self.virtual_samples[REI_opt_index[j]]) 
+                print('The {num}-th datum recomended by Reinterpolation Expected Improvement : \n x = '.format(num =j+1), self.row_features[REI_opt_index[j]])
+                return_x.append(self.row_features[REI_opt_index[j]]) 
         else:
             print('The input para. opt_num must be an int')
         return REI_list,np.array(return_x)
 
-
-
     def UCB(self, alpha=1):
         """
         :param alpha: tradeoff coefficient, default 1
         """
         UCB_list = np.array(self.virtual_samples_mean) - alpha * np.array(self.virtual_samples_std)
         
         return_x = []
         if self.opt_num == 1:
             UCB_opt_index = np.random.choice(np.flatnonzero(UCB_list == UCB_list.min()))
-            print('The next datum recomended by Upper confidence bound  : \n x = ', self.virtual_samples[UCB_opt_index])
-            return_x.append(self.virtual_samples[UCB_opt_index])    
+            print('The next datum recomended by Upper confidence bound  : \n x = ', self.row_features[UCB_opt_index])
+            return_x.append(self.row_features[UCB_opt_index])    
         elif type(self.opt_num) == int:
             UCB_opt_index = np.argpartition(UCB_list, self.opt_num)[:self.opt_num]
             for j in range(len(UCB_opt_index)):
-                print('The {num}-th datum recomended by Upper confidence bound : \n x = '.format(num =j+1), self.virtual_samples[UCB_opt_index[j]])
-                return_x.append(self.virtual_samples[UCB_opt_index[j]])
+                print('The {num}-th datum recomended by Upper confidence bound : \n x = '.format(num =j+1), self.row_features[UCB_opt_index[j]])
+                return_x.append(self.row_features[UCB_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
 
         return UCB_list,np.array(return_x)
     
     def PoI(self, tao = 0):
         """
@@ -234,21 +231,21 @@
                 PoI_list.append(PoI)
         
             PoI_list = np.array(PoI_list)
             
             return_x = []
             if self.opt_num == 1:
                 PoI_opt_index = np.random.choice(np.flatnonzero(PoI_list == PoI_list.max()))
-                print('The next datum recomended by Probability of Improvement  : \n x = ', self.virtual_samples[PoI_opt_index])
-                return_x.append(self.virtual_samples[PoI_opt_index])
+                print('The next datum recomended by Probability of Improvement  : \n x = ', self.row_features[PoI_opt_index])
+                return_x.append(self.row_features[PoI_opt_index])
             elif type(self.opt_num) == int:
                 PoI_opt_index = np.argpartition(PoI_list, -self.opt_num)[-self.opt_num:]
                 for j in range(len(PoI_opt_index)):
-                    print('The {num}-th datum recomended by Probability of Improvement  : \n x = '.format(num =j+1), self.virtual_samples[PoI_opt_index[j]])
-                    return_x.append(self.virtual_samples[PoI_opt_index[j]])
+                    print('The {num}-th datum recomended by Probability of Improvement  : \n x = '.format(num =j+1), self.row_features[PoI_opt_index[j]])
+                    return_x.append(self.row_features[PoI_opt_index[j]])
             else:
                 print('The input para. opt_num must be an int')
             return PoI_list,np.array(return_x)
     
     def Thompson_sampling(self,):
         # x* is derived by searching at the vistual space 
         # sample = np.len(virtual_samples)
@@ -287,21 +284,21 @@
             Entropy_y_conditional += 0.5*np.log(2*np.pi*np.e*(post_std**2))
         estimated_Entropy_y_conditional = Entropy_y_conditional / sam_num            
         PES_list = Entropy_y_ori - estimated_Entropy_y_conditional
         
         return_x = []
         if self.opt_num == 1:
             PES_opt_index = np.random.choice(np.flatnonzero(PES_list == PES_list.max()))
-            print('The next datum recomended by Predictive Entropy Search  : \n x = ', self.virtual_samples[PES_opt_index])
-            return_x.append(self.virtual_samples[PES_opt_index])
+            print('The next datum recomended by Predictive Entropy Search  : \n x = ', self.row_features[PES_opt_index])
+            return_x.append(self.row_features[PES_opt_index])
         elif type(self.opt_num) == int:
             PES_opt_index = np.argpartition(PES_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(PES_opt_index)):
-                print('The {num}-th datum recomended by Predictive Entropy Search  : \n x = '.format(num =j+1), self.virtual_samples[PES_opt_index[j]])
-                return_x.append(self.virtual_samples[PES_opt_index[j]])
+                print('The {num}-th datum recomended by Predictive Entropy Search  : \n x = '.format(num =j+1), self.row_features[PES_opt_index[j]])
+                return_x.append(self.row_features[PES_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return PES_list,np.array(return_x)
     
 
     def Knowledge_G(self,MC_num = 50):
         """
@@ -333,18 +330,18 @@
             MC_result = MC_batch_min / MC_num
             KD_list.append( current_min - MC_result)
         KD_list = np.array(KD_list)
 
         return_x = []
         if self.opt_num == 1:
             KD_opt_index = np.random.choice(np.flatnonzero(KD_list == KD_list.max()))
-            print('The next datum recomended by Knowledge Gradient : \n x = ', self.virtual_samples[KD_opt_index])
-            return_x.append(self.virtual_samples[KD_opt_index])
+            print('The next datum recomended by Knowledge Gradient : \n x = ', self.row_features[KD_opt_index])
+            return_x.append(self.row_features[KD_opt_index])
         elif type(self.opt_num) == int:
             KD_opt_index = np.argpartition(KD_list, -self.opt_num)[-self.opt_num:]
             for j in range(len(KD_opt_index)):
-                print('The {num}-th datum recomended by Knowledge Gradient : \n x = '.format(num =j+1), self.virtual_samples[KD_opt_index[j]])
-                return_x.append(self.virtual_samples[KD_opt_index[j]])
+                print('The {num}-th datum recomended by Knowledge Gradient : \n x = '.format(num =j+1), self.row_features[KD_opt_index[j]])
+                return_x.append(self.row_features[KD_opt_index[j]])
         else:
             print('The input para. opt_num must be an int')
         return KD_list,np.array(return_x)
```

### Comparing `Bgolearn-2.2.0/Bgolearn/BGOsampling.py` & `Bgolearn-2.2.1/Bgolearn/BGOsampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import inspect
 import os
 import time
 import warnings
 import numpy as np
 import pandas as pd
+import copy
 from .BGOmax import Global_max
 from .BGOmin import Global_min
 from .BGOclf import Boundary
 from .BGO_eval import BGO_Efficient
+from sklearn.preprocessing import MinMaxScaler
 from sklearn.model_selection import LeaveOneOut
 from sklearn.metrics import r2_score
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_squared_error
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import  RBF, WhiteKernel
 from sklearn.model_selection import KFold
@@ -75,24 +77,34 @@
         :param CV_test: 'LOOCV' or an int, default False (pass test) 
                 if CV_test = 'LOOCV', LOOCV will be applied,
                 elif CV_test = int, e.g., CV_test = 10, 10 folds cross validation will be applied.
         
         :return: 1: array; potential of each candidate. 2: array/float; recommended candidate(s).
 
         """
+        # Fit and transform the input data matrix
+        virtual_samples = preprocess_data(virtual_samples)
+        data_matrix = preprocess_data(data_matrix)
+        Measured_response = preprocess_data(Measured_response)
+
+        row_features = copy.deepcopy(virtual_samples)
+        scaler = MinMaxScaler()
+        data_matrix = scaler.fit_transform(data_matrix)
+        virtual_samples = scaler.transform(virtual_samples)
+
         timename = time.localtime(time.time())
         namey, nameM, named, nameh, namem = timename.tm_year, timename.tm_mon, timename.tm_mday, timename.tm_hour, timename.tm_min
 
         warnings.filterwarnings('ignore')
 
         if Mission == 'Classification':
             if type(Classifier) == str:
                 model = Classifier_selection(Classifier)
                 print(model)
-                BGOmodel = Boundary(model,data_matrix, Measured_response, virtual_samples, opt_num)
+                BGOmodel = Boundary(model,data_matrix, Measured_response, row_features, opt_num, virtual_samples)
                 return BGOmodel
             else:
                 print('Type Error! Classifier should be one of the following:')
                 print('GaussianProcess; LogisticRegression;NaiveBayes;SVM;RandomForest')
 
 
         elif Mission == 'Regression':
@@ -100,15 +112,15 @@
             if Kriging_model == None:
                 kernel = 1 * RBF() 
                 if noise_std == None:
                     # call the default model;
                     class Kriging_model(object):
                         def fit_pre(self,xtrain,ytrain,xtest,):
                             # estimating Noise Level of training dataset
-                            noise_ker = WhiteKernel(noise_level_bounds=(0.001,0.5))
+                            noise_ker = WhiteKernel(noise_level_bounds=(0.01,0.5))
                             GPr = GaussianProcessRegressor(kernel= 1 * RBF()+noise_ker,normalize_y=True).fit(xtrain,ytrain)
                             noise_level = np.exp(GPr.kernel_.theta[1])
         
                             # ret_std is a placeholder for homogenous noise
                             # instantiated mode
                             mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_level).fit(xtrain,ytrain)
                             # defined the attribute's outputs
@@ -276,29 +288,29 @@
                                                                                 minute=namem),encoding='utf-8-sig')
 
 
 
 
             # BGO
             if min_search == True:
-                BGOmodel = Global_min(Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise)
+                BGOmodel = Global_min(Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise,row_features)
             elif min_search == False: 
-                BGOmodel = Global_max(Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise)
+                BGOmodel = Global_max(Kriging_model,data_matrix, Measured_response, virtual_samples, opt_num, ret_noise,row_features)
             else:
                 print('type ERROR! -opt_num-')
             return BGOmodel
         else:
             print('type ERROR! -MISSION-')
 
     def test(self,Ture_fun, Def_Domain,noise_std = 1e-5, Kriging_model = None, opt_num = 1 ,min_search = True):
         
         """
         PACKAGE: Bayesian global optimization learn .
 
-        6 Apr 2023, version 1.4, Bin Cao, ZheJiang LAB, Hangzhou, CHINA. (MGI, SHU, Shanghai, CHINA).
+        6 Apr 2023, version 1.4, Bin Cao, ZheJiang LAB, Hangzhou, CHINA.
         
         :param Ture_fun: the true function being evaluated. e.g.,
                 def function(X):
                     X = np.array(X)
                     Y = 0.013*X**4 - 0.25*X**3 + 1.61*X**2 - 4.1*X + 8
                     return Y
 
@@ -357,35 +369,28 @@
                             print('the input data is not muached with heterogenous noise size') 
                         # defined the attribute's outputs
                         mean,std = mdoel.predict(xtest,return_std=True)
                         return mean,std  
                 print('The internal model is instantiated with heterogenous noise')
         else: 
             print('The external model is instantiated')
-           
-        
         
         # position incluse 'self'
         if len(inspect.getargspec(Kriging_model().fit_pre)[0]) == 5:
             ret_noise = True
         elif len(inspect.getargspec(Kriging_model().fit_pre)[0]) == 4:
             ret_noise = False
         else:
             print('type ERROR! -ILLEGAL form of Krigging-')
 
-
-
         print('Evaluation is executed')
         
         Eval_model = BGO_Efficient(Ture_fun,Def_Domain, Kriging_model, opt_num, ret_noise,min_search)
         return Eval_model
       
-  
-
-
 def Bgo_KFold(x_train, y_train,cv):
     x_train = np.array(x_train)
     y_train = np.array(y_train)
     kfolder = KFold(n_splits=cv, shuffle=True,random_state=0)
     kfold = kfolder.split(x_train, y_train)
     return kfold
 
@@ -393,15 +398,14 @@
     if CV_test == 'LOOCV':
         return 'LOOCV'
     elif type(CV_test) == int:
         return '{}-CVs'.format(CV_test)
     else:
         print('type error')
 
-
 def Classifier_selection(Classifier):
     if Classifier == 'GaussianProcess':
         from sklearn.gaussian_process import GaussianProcessClassifier 
         model = GaussianProcessClassifier(kernel= 1*RBF(1.0) ,random_state=0)
     elif Classifier == 'LogisticRegression':
         from sklearn.linear_model import LogisticRegression
         model = LogisticRegression(random_state=0,class_weight='balanced',multi_class='multinomial')
@@ -413,7 +417,17 @@
         model = SVC(probability=True)
     elif Classifier == 'RandomForest':
         from sklearn.ensemble import RandomForestClassifier
         model = RandomForestClassifier(max_depth=4,random_state=0)
     else :
         print('type ERROR! -Classifier-')
     return model
+
+
+def preprocess_data(data):
+    if isinstance(data, np.ndarray):
+        if data.ndim == 1:
+            data = np.reshape(data, (-1, 1))
+    elif isinstance(data, list):
+        data = np.array(data).reshape(-1, 1)
+    data = np.array(data)
+    return data
```

### Comparing `Bgolearn-2.2.0/Bgolearn.egg-info/PKG-INFO` & `Bgolearn-2.2.1/Bgolearn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.2.0/PKG-INFO` & `Bgolearn-2.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.2.0/README.md` & `Bgolearn-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.0/setup.py` & `Bgolearn-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='Bgolearn',  # 包名
-    version='2.2.0',  # 版本
+    version='2.2.1',  # 版本
     description="A Bayesian global optimization package for material design",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

