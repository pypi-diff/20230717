# Comparing `tmp/MLXpress-0.1.7-py3-none-any.whl.zip` & `tmp/MLXpress-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7279 bytes, number of entries: 11
+Zip file size: 9138 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 13:51 MLXpress/__init__.py
--rw-rw-rw-  2.0 fat     1573 b- defN 23-Jul-15 06:59 MLXpress/diabetes.py
--rw-rw-rw-  2.0 fat     2576 b- defN 23-Jul-16 14:21 MLXpress/iris.py
+-rw-rw-rw-  2.0 fat     2338 b- defN 23-Jul-17 12:15 MLXpress/diabetes.py
+-rw-rw-rw-  2.0 fat     4011 b- defN 23-Jul-17 18:41 MLXpress/iris.py
 -rw-rw-rw-  2.0 fat     1200 b- defN 23-Jul-16 18:18 MLXpress/math.py
--rw-rw-rw-  2.0 fat     2419 b- defN 23-Jul-16 18:57 MLXpress/preprocessing.py
--rw-rw-rw-  2.0 fat     1833 b- defN 23-Jul-16 17:52 MLXpress/stats.py
--rw-rw-rw-  2.0 fat      900 b- defN 23-Jul-14 18:27 MLXpress/wine.py
--rw-rw-rw-  2.0 fat     2409 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      826 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/RECORD
-11 files, 13837 bytes uncompressed, 5897 bytes compressed:  57.4%
+-rw-rw-rw-  2.0 fat     5030 b- defN 23-Jul-17 17:33 MLXpress/preprocessing.py
+-rw-rw-rw-  2.0 fat     1870 b- defN 23-Jul-17 17:54 MLXpress/stats.py
+-rw-rw-rw-  2.0 fat     2733 b- defN 23-Jul-17 18:40 MLXpress/wine.py
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-Jul-17 18:52 MLXpress-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 18:52 MLXpress-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-17 18:52 MLXpress-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      827 b- defN 23-Jul-17 18:52 MLXpress-0.1.8.dist-info/RECORD
+11 files, 20519 bytes uncompressed, 7756 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: MLXpress/stats.py
 Comment: 
 
 Filename: MLXpress/wine.py
 Comment: 
 
-Filename: MLXpress-0.1.7.dist-info/METADATA
+Filename: MLXpress-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: MLXpress-0.1.7.dist-info/WHEEL
+Filename: MLXpress-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: MLXpress-0.1.7.dist-info/top_level.txt
+Filename: MLXpress-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: MLXpress-0.1.7.dist-info/RECORD
+Filename: MLXpress-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MLXpress/diabetes.py

```diff
@@ -8,28 +8,53 @@
 d = load_diabetes()
 X = d.data
 y = d.target
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=12)
 
 
 def regression(model, x=None, y=None):
+    """
+        Perform regression analysis using the specified model and calculate the Mean Squared Error (MSE).
+
+        Args:
+            model: The regression model.
+            x: The input features for prediction. If not provided, X_test will be used.
+            y: The target variable. If not provided, y_test will be used.
+
+        Returns:
+            The calculated MSE as a string.
+    """
     if x is None:
         x = X_test
     if y is None:
         y = y_test
     model.fit(X_train, y_train)
     y_pred = model.predict(x)
     mse = mean_squared_error(y_test, y_pred)
     MSE = f"The MSE of the model is {mse:.2f} "
+    print(MSE)
     return MSE
 
 
 def predict(model, x):
+    """
+       Perform prediction using the specified model on the given input features.
+
+       Args:
+           model: The regression model.
+           x: The input features for prediction.
+
+       Returns:
+           The predicted disease progression as a string.
+
+       """
     pred = model.predict(x)
-    pred1 = f"Predicted Disease Progression: {pred}"
+    pred_s = pred[0]
+    pred1 = f"Predicted Disease Progression: {pred_s:.2f}"
+    print(pred1)
     return pred1
 
 
 def vis(model, X=X_test, y=y_test):
     diabetes = load_diabetes()
     df = pd.DataFrame(X, columns=diabetes.feature_names)
     df['Target'] = y
```

## MLXpress/iris.py

```diff
@@ -9,38 +9,75 @@
 iris = load_iris()
 X = iris.data
 y = iris.target
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=12)
 
 
 def classification(model, x=None, y=None):
+    """
+      Perform classification using the specified model and calculate accuracy.
+
+      Parameters:
+      - model: The classification model.
+      - x: The input data. If None, it uses X_test.
+      - y: The target labels. If None, it uses y_test.
+
+      Returns:
+      - ac1: The accuracy of the model as a string.
+      """
     if x is None:
         x = X_test
     if y is None:
         y = y_test
     model.fit(X_train, y_train)
     y_pred = model.predict(x)
     cm = confusion_matrix(y, y_pred)
     fig = plt.figure(num="Confusion Matrix")
     sns.heatmap(cm, annot=True, cmap='Blues')
 
 
     plt.show()
     ac = accuracy_score(y_test, y_pred)
-    ac1 = f"The accuracy of the model is {ac * 100:.2f} %"
+    ac1 = f"The accuracy of the model is {ac * 100:.2f} % and the other metrics are as follows:\n"
+    print(ac1)
+    cr=classification_report(y_test, y_pred)
+    print(cr)
     return ac1
 
 
 def predict(model, x):
+    """
+        Perform prediction using the specified model.
+
+        Parameters:
+        - model: The trained model.
+        - x: The input data for prediction.
+
+        Returns:
+        - pred1: The prediction result as a string.
+
+        """
+
     pred = model.predict(x)
     pred1 = f"The instance belongs to class {pred}"
+    print(pred1)
     return pred1
 
 
 def vis(model, X=X_test, y=y_test):
+    """
+       Visualize box plots for each feature based on the target variable.
+
+       Parameters:
+       - model: The model used for visualization.
+       - X: The input data. Defaults to X_test.
+       - y: The target variable. Defaults to y_test.
+
+       """
+
     iris = load_iris()
     df = pd.DataFrame(X, columns=iris.feature_names)
     df['Target'] = iris.target_names[y]
     # Create a box plot for each feature
     fig, axes = plt.subplots(2, 2, figsize=(10, 8))
     for i, feature in enumerate(iris.feature_names):
         row = i // 2
@@ -52,14 +89,25 @@
 
     # Set the title of the figure
     plt.suptitle('Box Plot')
     plt.show()
 
 
 def clustering(model, num_clusters):
+    """
+       Perform clustering using the specified model and calculate silhouette score.
+
+       Parameters:
+       - model: The clustering model.
+       - num_clusters: The number of clusters to create.
+
+       Returns:
+       - labels: The cluster labels as an array.
+
+       """
     model.fit(X)
     labels = model.labels_
     silhouette = silhouette_score(X, labels)
 
     print("Cluster Labels:")
     for sample_idx, label in enumerate(labels):
         print(f"Sample {sample_idx + 1}: Cluster {label}")
@@ -68,14 +116,21 @@
     return labels
 
 
 
 
 
 def vis_clusters(model):
+    """
+       Visualize the clustering results.
+
+       Parameters:
+       - model: The clustering model.
+
+       """
     features = globals().get('X')
 
     if features is None:
         raise ValueError("Features must be set as a global variable.")
 
     labels = model.labels_
```

## MLXpress/preprocessing.py

```diff
@@ -3,62 +3,131 @@
 from sklearn.model_selection import train_test_split
 from sklearn.impute import SimpleImputer
 from sklearn.feature_selection import SelectKBest, f_classif
 from sklearn.feature_selection import SelectKBest, f_regression
 from sklearn.model_selection import cross_val_score
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import SVC
+import pandas as pd
 def handle_missing_values(data):
+    """
+      Handle missing values in the input data by replacing them with the mean of each column.
+
+      Parameters:
+          data (numpy.ndarray or pandas.DataFrame): Input data with missing values.
+
+      Returns:
+          None
+      """
     # Create an instance of SimpleImputer
     imputer = SimpleImputer(strategy='mean')
 
     # Handle missing values by replacing them with the mean of each column
     data_imputed = imputer.fit_transform(data)
 
     print("Missing values handled. Imputed data:")
-    print(data_imputed)
+    print(pd.DataFrame(data_imputed, columns=data.columns))
 
-def perform_cross_validation(X, y, model='logistic', scoring='accuracy', cv=5):
+def perform_cross_validation(X, y, model='logistic', scoring='accuracy', cv=2):
+    """
+        Perform cross-validation on the input data using the specified model.
+
+        Parameters:
+            X (numpy.ndarray or pandas.DataFrame): Input features.
+            y (numpy.ndarray or pandas.Series): Target variable.
+            model (str, optional): Model to use for cross-validation. Default is 'logistic'.
+            scoring (str, optional): Scoring metric for cross-validation. Default is 'accuracy'.
+            cv (int, optional): Number of cross-validation folds. Default is 5.
+
+        Returns:
+            None
+        """
     if model == 'logistic':
-        clf = LogisticRegression()
+        clf = LogisticRegression(max_iter=10000)
     elif model == 'svm':
         clf = SVC()
     else:
         raise ValueError("Invalid model specified. Please choose 'logistic' or 'svm'.")
 
     scores = cross_val_score(clf, X, y, cv=cv, scoring=scoring)
     print(f"Cross Validation {scoring.capitalize()}:")
-    print(scores)
+    for i, score in enumerate(scores):
+        print(f"Fold {i + 1}: {score:.4f}")  # Print cross-validation scores with 4 decimal places
 
-def select_best_features(X, y, k=5):
+def select_best_features(X, y, k='all'):
+    """
+       Select the top k best features using the specified scoring function.
+
+       Parameters:
+           X (numpy.ndarray or pandas.DataFrame): Input features.
+           y (numpy.ndarray or pandas.Series): Target variable.
+           k (int, optional): Number of top features to select. Default is 5.
+
+       Returns:
+           None
+       """
     selector = SelectKBest(score_func=f_classif, k=k)
     X_new = selector.fit_transform(X, y)
     selected_features = X.columns[selector.get_support()]
     print("Selected Features:")
-    print(selected_features)
+    print(selected_features.tolist())
 def scale_data(X, scaler='standard'):
+    """
+        Scale the input data using the specified scaler.
+
+        Parameters:
+            X (numpy.ndarray or pandas.DataFrame): Input data to be scaled.
+            scaler (str, optional): Scaler to use for scaling. Default is 'standard'.
+
+        Returns:
+            None
+        """
     if scaler == 'standard':
         scaler = StandardScaler()
     elif scaler == 'normal':
         scaler = MinMaxScaler()
     else:
         raise ValueError("Invalid scaler specified. Please choose 'standard' or 'normal'.")
 
     X_scaled = scaler.fit_transform(X)
     print("Scaled Data:")
-    print(X_scaled)
+    print(pd.DataFrame(X_scaled, columns=X.columns))
 def remove_low_variance_features(X, threshold=0.1):
+    """
+       Remove features with low variance from the input data.
+
+       Parameters:
+           X (numpy.ndarray or pandas.DataFrame): Input data.
+           threshold (float, optional): Threshold for variance. Features with variance below this threshold will be removed. Default is 0.1.
+
+       Returns:
+           None
+       """
     selector = VarianceThreshold(threshold=threshold)
     X_high_variance = selector.fit_transform(X)
-
     print("High variance features:")
-    print(X_high_variance)
+    print(pd.DataFrame(X_high_variance, columns=X.columns))
+
+
 
 def split_data(X, y, test_size=0.2, random_state=None):
-    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
+    """
+        Split the input data into training and testing sets.
 
+        Parameters:
+            X (numpy.ndarray or pandas.DataFrame): Input features.
+            y (numpy.ndarray or pandas.Series): Target variable.
+            test_size (float, optional): Proportion of the data to be used for testing. Default is 0.2.
+            random_state (int or None, optional): Random seed for reproducibility. Default is None.
+
+        Returns:
+            None
+        """
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
     print("Train/Test split:")
-    print("X_train:", X_train)
-    print("X_test:", X_test)
-    print("y_train:", y_train)
-    print("y_test:", y_test)
+    print("X_train:\n", X_train)
+    print("X_test:\n", X_test)
+    print("y_train:\n", y_train)
+    print("y_test:\n", y_test)
+
+
```

## MLXpress/stats.py

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import statistics as stats
 import matplotlib.pyplot as plt
 import seaborn as sns
+from scipy import stats
 from scipy.stats import skew
 def analyze(data):
     statistics = calculate_statistics(data)
     distribution_nature = determine_distribution_nature(data)
     print(f"The data is {distribution_nature} skewed")
     statistics['Distribution Nature'] = distribution_nature
     visualize_distribution(data)
@@ -13,15 +14,15 @@
     visualize_histogram(data)
 
     return statistics
 
 def calculate_statistics(data):
     mean = np.mean(data)
     median = np.median(data)
-    mode = stats.mode(data)
+    mode = stats.mode(data).mode.item()
     iqr = np.percentile(data, 75) - np.percentile(data, 25)
     data_range = np.max(data) - np.min(data)
     variance = np.var(data)
     std_dev = np.std(data)
 
     stat = {
         'Mean': mean,
```

## MLXpress/wine.py

```diff
@@ -1,30 +1,95 @@
 from sklearn.datasets import load_wine
 from sklearn.model_selection import train_test_split
-from sklearn.metrics import confusion_matrix,classification_report,accuracy_score
+from sklearn.metrics import confusion_matrix, classification_report, accuracy_score
 import matplotlib.pyplot as plt
 import seaborn as sns
+import pandas as pd
+
 wine = load_wine()
 X = wine.data
 y = wine.target
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3,random_state=12)
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=12)
+
+
+def classification(model, x=None, y=None):
+    """
+      Perform classification using the specified model and calculate accuracy.
 
+      Parameters:
+      - model: The classification model.
+      - x: The input data. If None, it uses X_test.
+      - y: The target labels. If None, it uses y_test.
 
-def classification(model,x=None, y=None):
+      Returns:
+      - ac1: The accuracy of the model as a string.
+      """
     if x is None:
         x = X_test
     if y is None:
         y = y_test
     model.fit(X_train, y_train)
     y_pred = model.predict(x)
     cm = confusion_matrix(y, y_pred)
-    sns.heatmap(cm,annot=True,cmap='Blues')
+    fig = plt.figure(num="Confusion Matrix")
+    sns.heatmap(cm, annot=True, cmap='Blues')
+
     plt.show()
     ac = accuracy_score(y_test, y_pred)
-    ac1= f"The accuracy of the model is {ac*100:.2f} %"
+    ac1 = f"The accuracy of the model is {ac * 100:.2f} % and the other metrics are as follows:\n"
+    print(ac1)
+    cr = classification_report(y_test, y_pred)
+    print(cr)
     return ac1
-def predict(model,x):
-    pred=model.predict(x)
-    pred1=f"The instance belongs to class {pred}"
+
+
+def predict(model, x):
+    """
+        Perform prediction using the specified model.
+
+        Parameters:
+        - model: The trained model.
+        - x: The input data for prediction.
+
+        Returns:
+        - pred1: The prediction result as a string.
+
+        """
+
+    pred = model.predict(x)
+    pred1 = f"The instance belongs to class {pred}"
+    print(pred1)
     return pred1
 
 
+def vis(model, X=X_test, y=y_test):
+    """
+    Visualize box plots for each feature based on the target variable.
+
+    Parameters:
+    - model: The model used for visualization.
+    - X: The input data. Defaults to X_test.
+    - y: The target variable. Defaults to y_test.
+    """
+
+    wine1 = load_wine()
+    df = pd.DataFrame(X, columns=wine1.feature_names)
+    df['Target'] = wine1.target_names[y]
+
+    num_features = len(wine1.feature_names)
+    num_rows = (num_features - 1) // 2 + 1
+    num_cols = min(2, num_features)
+
+    # Create subplots based on the number of features
+    fig, axes = plt.subplots(num_rows, num_cols, figsize=(10, 8))
+
+    for i, feature in enumerate(wine1.feature_names):
+        row = i // num_cols
+        col = i % num_cols
+        sns.boxplot(x='Target', y=feature, data=df, ax=axes[row, col])
+
+    # Adjust the spacing between subplots
+    plt.tight_layout()
+
+    # Set the title of the figure
+    plt.suptitle('Box Plot')
+    plt.show()
```

## Comparing `MLXpress-0.1.7.dist-info/METADATA` & `MLXpress-0.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.7
+Version: 0.1.8
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Home-page: UNKNOWN
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `MLXpress-0.1.7.dist-info/RECORD` & `MLXpress-0.1.8.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MLXpress/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-MLXpress/diabetes.py,sha256=R3mMXMMnqxgI5GuZiJQ0SYcIJxSMzToeTWJ22_Iiyxw,1573
-MLXpress/iris.py,sha256=c1oVXfM833l3M6v_GfZopic6uhmMXIrFbqVdbgVmhhw,2576
+MLXpress/diabetes.py,sha256=sP4Brs-s-rm-PDe1w8CTEucMQL_0a9Aey_pV1laaD7w,2338
+MLXpress/iris.py,sha256=rYRaVAMU6nuPnBhWD8EDnP1K6R9aGo0DlDJVvBqNlkc,4011
 MLXpress/math.py,sha256=jhPvmhTK65PdYU1VUBWPRZ_1c3DBawtKhea3i1bX8zs,1200
-MLXpress/preprocessing.py,sha256=7du6oM2ujArYKr0osdTaVSavb51ctV_ylEh2WzVBEo4,2419
-MLXpress/stats.py,sha256=gcPuIwlH1m5We7ziTncskC9ohse6uOLOZmbved1QS08,1833
-MLXpress/wine.py,sha256=SDOkZ3rxvVlpp60KcBVDqHH4sszQOUCE_haS6Jd6y1o,900
-MLXpress-0.1.7.dist-info/METADATA,sha256=3WpGE8QmaQbekhNouYI9LBdmEvx8xUJqgW9Sk7uXT7k,2409
-MLXpress-0.1.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-MLXpress-0.1.7.dist-info/top_level.txt,sha256=E_zzsORNP4ijnH3c0zliWBMP8u6EoATcbgfFHUzjBT4,9
-MLXpress-0.1.7.dist-info/RECORD,,
+MLXpress/preprocessing.py,sha256=EMzljypn1_32hnEgjd1etYBHf7Qv9IygtSylCfup4Qw,5030
+MLXpress/stats.py,sha256=6AEcgQ24z1ysKqKh0tAJwXfAj8jlz6qX4jpXDGJuvWI,1870
+MLXpress/wine.py,sha256=St4TJwC1nDE3zbm79sqLtCxoppKT-UTM-Y7XhtjWJZ0,2733
+MLXpress-0.1.8.dist-info/METADATA,sha256=tVeNqhE36HLApgE7wIroJwwRqECNq2ETT55F4yxb5zk,2409
+MLXpress-0.1.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+MLXpress-0.1.8.dist-info/top_level.txt,sha256=E_zzsORNP4ijnH3c0zliWBMP8u6EoATcbgfFHUzjBT4,9
+MLXpress-0.1.8.dist-info/RECORD,,
```

