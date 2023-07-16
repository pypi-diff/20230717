# Comparing `tmp/AgenciBr-0.1.7.tar.gz` & `tmp/AgenciBr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgenciBr-0.1.7.tar", last modified: Wed Jul  5 01:33:32 2023, max compression
+gzip compressed data, was "AgenciBr-0.1.8.tar", last modified: Sun Jul 16 22:57:52 2023, max compression
```

## Comparing `AgenciBr-0.1.7.tar` & `AgenciBr-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-05 01:33:32.155426 AgenciBr-0.1.7/
-drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-05 01:33:32.155426 AgenciBr-0.1.7/AgenciBr/
--rw-rw-r--   0 thigs     (1000) thigs     (1000)     8438 2023-01-05 19:28:24.000000 AgenciBr-0.1.7/AgenciBr/Alexandre.py
--rw-rw-r--   0 thigs     (1000) thigs     (1000)    36112 2023-07-04 17:10:28.000000 AgenciBr-0.1.7/AgenciBr/Ana.py
--rw-rw-r--   0 thigs     (1000) thigs     (1000)    19414 2023-07-04 19:21:07.000000 AgenciBr-0.1.7/AgenciBr/Ideam.py
--rw-rw-r--   0 thigs     (1000) thigs     (1000)    51057 2023-07-04 17:10:08.000000 AgenciBr-0.1.7/AgenciBr/Inemet.py
--rw-rw-r--   0 thigs     (1000) thigs     (1000)     4258 2023-01-19 16:22:36.000000 AgenciBr-0.1.7/AgenciBr/Merge.py
--rw-rw-r--   0 thigs     (1000) thigs     (1000)      316 2023-01-06 10:25:08.000000 AgenciBr-0.1.7/AgenciBr/__init__.py
--rw-rw-r--   0 thigs     (1000) thigs     (1000)    41108 2023-03-19 00:17:34.000000 AgenciBr-0.1.7/AgenciBr/indice.py
-drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-05 01:33:32.155426 AgenciBr-0.1.7/AgenciBr.egg-info/
--rw-rw-r--   0 thigs     (1000) thigs     (1000)     5732 2023-07-05 01:33:32.000000 AgenciBr-0.1.7/AgenciBr.egg-info/PKG-INFO
--rw-rw-r--   0 thigs     (1000) thigs     (1000)      328 2023-07-05 01:33:32.000000 AgenciBr-0.1.7/AgenciBr.egg-info/SOURCES.txt
--rw-rw-r--   0 thigs     (1000) thigs     (1000)        1 2023-07-05 01:33:32.000000 AgenciBr-0.1.7/AgenciBr.egg-info/dependency_links.txt
--rw-rw-r--   0 thigs     (1000) thigs     (1000)       74 2023-07-05 01:33:32.000000 AgenciBr-0.1.7/AgenciBr.egg-info/requires.txt
--rw-rw-r--   0 thigs     (1000) thigs     (1000)        9 2023-07-05 01:33:32.000000 AgenciBr-0.1.7/AgenciBr.egg-info/top_level.txt
--rw-rw-r--   0 thigs     (1000) thigs     (1000)     1079 2022-10-18 20:59:14.000000 AgenciBr-0.1.7/LICENSE
--rw-rw-r--   0 thigs     (1000) thigs     (1000)     5732 2023-07-05 01:33:32.155426 AgenciBr-0.1.7/PKG-INFO
--rw-rw-r--   0 thigs     (1000) thigs     (1000)     5411 2023-07-04 13:46:40.000000 AgenciBr-0.1.7/README.md
--rw-rw-r--   0 thigs     (1000) thigs     (1000)       38 2023-07-05 01:33:32.155426 AgenciBr-0.1.7/setup.cfg
--rw-rw-r--   0 thigs     (1000) thigs     (1000)      594 2023-07-05 01:33:11.000000 AgenciBr-0.1.7/setup.py
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-16 22:57:52.983622 AgenciBr-0.1.8/
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-16 22:57:52.983622 AgenciBr-0.1.8/AgenciBr/
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     8438 2023-01-05 19:28:24.000000 AgenciBr-0.1.8/AgenciBr/Alexandre.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    33906 2023-07-12 00:58:34.000000 AgenciBr-0.1.8/AgenciBr/Ana.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    15259 2023-07-13 01:09:10.000000 AgenciBr-0.1.8/AgenciBr/Ideam.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    39088 2023-07-13 00:42:35.000000 AgenciBr-0.1.8/AgenciBr/Inemet.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     7845 2023-07-12 20:02:12.000000 AgenciBr-0.1.8/AgenciBr/Merge.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)      316 2023-01-06 10:25:08.000000 AgenciBr-0.1.8/AgenciBr/__init__.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    42221 2023-07-13 14:01:41.000000 AgenciBr-0.1.8/AgenciBr/indice.py
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-16 22:57:52.983622 AgenciBr-0.1.8/AgenciBr.egg-info/
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     5732 2023-07-16 22:57:52.000000 AgenciBr-0.1.8/AgenciBr.egg-info/PKG-INFO
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)      328 2023-07-16 22:57:52.000000 AgenciBr-0.1.8/AgenciBr.egg-info/SOURCES.txt
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)        1 2023-07-16 22:57:52.000000 AgenciBr-0.1.8/AgenciBr.egg-info/dependency_links.txt
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)       74 2023-07-16 22:57:52.000000 AgenciBr-0.1.8/AgenciBr.egg-info/requires.txt
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)        9 2023-07-16 22:57:52.000000 AgenciBr-0.1.8/AgenciBr.egg-info/top_level.txt
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     1079 2022-10-18 20:59:14.000000 AgenciBr-0.1.8/LICENSE
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     5732 2023-07-16 22:57:52.983622 AgenciBr-0.1.8/PKG-INFO
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     5411 2023-07-04 13:46:40.000000 AgenciBr-0.1.8/README.md
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)       38 2023-07-16 22:57:52.983622 AgenciBr-0.1.8/setup.cfg
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)      594 2023-07-16 22:55:02.000000 AgenciBr-0.1.8/setup.py
```

### Comparing `AgenciBr-0.1.7/AgenciBr/Alexandre.py` & `AgenciBr-0.1.8/AgenciBr/Alexandre.py`

 * *Files identical despite different names*

### Comparing `AgenciBr-0.1.7/AgenciBr/Ana.py` & `AgenciBr-0.1.8/AgenciBr/Ana.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
             return len(df) + 1 + 4
 
         def dataframe(path):
             df = pd.read_csv(path, skiprows=linha_inicio_df(path), sep=sep, encoding=encoding,
                              index_col=index_col, on_bad_lines=on_bad_lines)
             if comma_to_dot:
                 temp = []
+                
+                df = df.drop_duplicates(subset='Data', keep="last")
                 for k in df['Data']:
                     temp.append(datetime.datetime.strptime(k, '%d/%m/%Y'))
                 df['Data'] = temp.copy()
                 df = df.sort_values(by='Data')
                 df = df.reset_index()
                 return df.replace({',': '.'}, regex=True)
             else:
@@ -46,17 +48,15 @@
                     temp.append(datetime.datetime.strptime(k, '%d/%m/%Y'))
                 df['Data'] = temp.copy()
                 df = df.sort_values(by='Data')
                 df = df.reset_index()
 
                 return df
 
-        def altitude():
-            return 10
-        def get_startdata():
+        def get_startdate():
             if self.type == "format1":
                 return self.dataframe["time"][0]
             return self.dataframe['Data'][0]
         def get_enddate():
             if self.type == "format1":
                 return self.dataframe["time"][-1]
 
@@ -66,21 +66,23 @@
         if not list:
             self.dataframe = dataframe(arquivo)
             self.type = "original"
             self.code = find_cod(pd.read_csv(arquivo, nrows=50, index_col=False,
                                                on_bad_lines='skip', encoding='latin-1'))
             self.fonte = pd.read_csv(arquivo, nrows=2, index_col=False,
                                      on_bad_lines='skip', encoding='latin-1')
-            self.startdate = get_startdata()
+            self.startdate = get_startdate()
             self.enddate = get_enddate()
             self.len = len(self.dataframe)
             self.type_data = 'pr'
             self.lat = lat
             self.lon = lon
-            self.alt = altitude()
+            self.alt = None 
+            self.name = None
+            self.NumCity = None
             self.status = None
             self.city = None
             self.state = None
             self.list = list
 
         else:
             self.path = arquivo
@@ -99,30 +101,22 @@
             df.get_lonlat()
             lat = np.append(lat, df.lat)
             lon = np.append(lon, df.lon)
             code = np.append(code, df.code)
 
         df = pd.DataFrame({"code":code, "lat":lat, "lon":lon})
         return df
-    def report(self, path):
-        """
-        Save a txt file with importants informations
-
-        """
-        self.format1()
-        with open(path+"/report.txt", 'w') as f:
-            f.write(f"Station {self.city} {self.code}\n")
-            f.write(f"Empty data of : {self.empty_data()}\n")
-            f.write(f"Max value: {np.max(self.dataframe.iloc[:, 1])}\n")
-            v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
-            f.write(f"Date of max value: {v.day}/{v.month}/{v.year}\n")
-            f.write(f"Min value: {np.min(self.dataframe.iloc[:, 1])}\n")
-            v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
-            f.write(f"Date of min value: {v.day}/{v.month}/{v.year}\n")
-            f.close()
+    def get_info(self):
+        """Internal functions that get informations of the station"""
+        inv = pd.read_csv("./inventario_ana.csv", sep=",", low_memory=False)
+        a = inv[inv["Codigo"] == 466001]
+        self.lat = float(a["Latitude"])
+        self.lon = float(a["Longitude"])
+        self.alt = float(a["Altitude"])
+        self.name = str(a["Nome"])
     def only_mondata(self, list=False):
         """
         Remove all columns that is not referent of month precipitation and day, in original data from Agenci
 
         :param list:
         :return:
         """
@@ -160,15 +154,15 @@
                     lista_meses.append(f'Chuva{k}')
                     lista_meses.append(f'Clima{k}')
             columns = df.columns
             for a in columns:
                 if a not in lista_meses:
                     del df[a]
             self.type_data = "only_mondata"
-            self.dataframe = df.drop_duplicates(subset=["Data"])
+            self.dataframe = df.drop_duplicates(subset=["Data"], keep="last")
 
         else:
             return 'List is only True or False'
 
     def format1(self, comma_to_dot=True, grow=True, years=(0,0)):
         """
         We change the file format to
@@ -202,177 +196,108 @@
                 ...
                 2020-01-01  0.3
                 2020-01-02  0.0
 
         """
 
         import pandas as pd
-        from datetime import timedelta
-
+        from datetime import timedelta, datetime
         if years != (0,0) and self.type != "format1":
             # Organize the file by date, the lower to greater
-            df_ordenado = self.dataframe
-            df_ordenado['Data'] = pd.to_datetime(df_ordenado['Data'], format="%d/%m/%Y")
-            df_ordenado = df_ordenado.drop_duplicates(subset='Data')
+            df= self.dataframe
+            df['Data'] = pd.to_datetime(df['Data'], format="%d/%m/%Y")
+            df = df.drop_duplicates(subset='Data', keep="last")
 
             if comma_to_dot:
-                df_ordenado = df_ordenado.replace({',': '.'}, regex=True)
-                df_ordenado = df_ordenado.reset_index()
-                df_ordenado = df_ordenado.drop(columns='index')
-                self.dataframe = df_ordenado
+                df = df.replace({',': '.'}, regex=True)
+                df = df.reset_index()
+                df = df.drop(columns='index')
+                self.dataframe = df
             if not grow:
-                self.daframe = df_ordenado.sort_values(by=['Data'], ascending=True)
+                self.dataframe = df.sort_values(by=['Data'], ascending=True)
 
             data = np.array([])
             pr = np.array([])
             self.only_mondata()
 
-            # remove data that don't exits
+            # remove date that don't exits
             colum = self.dataframe.columns
             n=0
-            for linha in range(len(self.dataframe)):
-                for dia in range(1, 32):
+            for linha in range(len(self.dataframe)):#Follow Rows
+                for dia in range(1, 32): #Follow Columns
                     try:
                         temp = self.dataframe[colum[0]][linha]
-                        data = np.append(data, datetime.date(temp.year, temp.month, dia))  # check if the date is real
+                        data = np.append(data, pd.to_datetime(datetime(temp.year, temp.month, dia)))  # check if the date is real
                         pr = np.append(pr, float(self.dataframe[colum[dia]][linha]))
                     except:
-                        n+= 0
+                        pass
 
             # chech if have date jump
+            a = pd.date_range(start=str(years[0]), end=str(years[1]), freq='D')
+            a = a[:-1]
+            pr_def = np.full(len(a), np.nan)
+            for i in range(len(data)):
+                ind = np.argwhere(data[i] == a)
+                pr_def[ind] = pr[i]
 
-            a = pd.date_range(start=self.startdate, end=self.enddate)
-
-            for i in range(len(a)):
-                try:
-                    while np.datetime64(data[i]) != np.datetime64(a[i]):
-                        data = np.insert(data, i, data[i-1]+timedelta(days=1))
-                        pr = np.insert(pr, i, 0)
-                        pr[i] = np.NaN
-                except:
-                    continue
-            data = pd.date_range(start=data[0], end=data[len(data)-1]) # change data to numpy datetime64
-            # select the year series
-            if (float(years[0]) in pd.DatetimeIndex(data).year) and (float(years[1]) not in pd.DatetimeIndex(data).year): # The first date is in array and end date not
-                if self.startdate != datetime(self.startdate.year, 1,1): # complete missing days start, if don't start in 1/1
-                    data = np.concatenate((pd.date_range(start=f"1/1/{int(self.startdate.year)}", end=self.startdate).to_numpy(), data[1:]))
-                    a = np.ones(np.size(pd.date_range(start=f"1/1/{int(years[0])}", end=self.startdate).to_numpy()))
-                    a[:] = np.nan
-                    pr = np.concatenate((a[:-1], pr))
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                i = np.where(date[0] == data)[0][0]
-                t = np.empty(np.size(date))
-                t[:] = np.nan
-                t[:len(pr[i:])] = pr[i:]
-                pr = t
-
-            elif  float(years[1]) in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(data).year: # The end date is in array and first date not
-                # complete end date to 31/12 if don't go
-                if self.enddate != datetime(self.enddate.year, 12, 31):
-                    t = np.empty((datetime(self.enddate.year, 12, 31)-self.enddate).days)
-                    t[:] = np.nan
-                    pr = np.concatenate((pr, t))
-                    data = np.concatenate((data, pd.date_range(start=data[-1], end=f"31/12/{int(self.enddate.year)}")))
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                # The index where is the end date
-                f = np.where(date[-1] == data)[0][0]
-
-                t = np.empty(len(date))
-                t[:] = np.nan
-                t[-len(data[:f]):] = pr[:f]
-                pr = t
-
-            elif float(years[1]) not in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(data).year: # The end date is not in array and first date not in
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                # The index of dates that we have data
-                i = np.where(data[0]== date)[0][0]
-                f = np.where(data[-1] == date)[0][0]
-                t = np.empty(np.size(date)) # will be precipitation data
-                t[:] = np.nan
-                # armazene the data
-                date[i:f] = data[:-1]
-                t[i:f] = pr[:-1]
-
-                # Change the variable name
-                pr = t
-
-            else: # both dates are in array
-
-                if self.startdate.date != datetime.date(self.enddate.year, 1,1): # complete missing days start, if don't start in 1/1
-                    data = np.concatenate([pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy(), data[1:]])
-                    a = np.ones(np.size(pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy()))
-                    a[:] = np.nan
-                    pr = np.concatenate([a[:-1], pr])
-
-                if self.enddate.date != datetime.date(self.enddate.year, 12, 31):
-                    t = np.empty(len(pd.date_range(start=data[-1], end=f"31/12/{self.enddate.year}")[1:]))
-                    t[:] = np.nan
-                    pr = np.concatenate((pr, t))
-                    data = np.concatenate((data[:], pd.date_range(start=data[-1], end=f"31/12/{self.enddate.year}")[1:]))
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                i = np.where(date[0] == data)[0][0]
-                f = np.where(date[-1] == data)[0][0]
-
-                date = data[i:f]
-                pr = pr[i:f]
-
-            self.dataframe = pd.DataFrame(list(zip(date, pr)), columns=['time', 'pr'])
+            df = pd.DataFrame(list(zip(a, pr_def)), columns=['time', 'pr'])
+            
 
             # atualize the format and len
             self.type = "format1"
+            df = df[(df.iloc[:, 0].dt.year <= years[1])]
+            self.dataframe = df[df.iloc[:, 0].dt.year >= years[0]]
             self.len = len(self.dataframe)
-        elif self.type != 'format1': # If the data is not the format1
-            # Organize the file by date, the lower to greater
-            df_ordenado = self.dataframe
-            df_ordenado['Data'] = pd.to_datetime(df_ordenado['Data'], format="%d/%m/%Y")
-            df_ordenado = df_ordenado.drop_duplicates(subset='Data')
+            self.enddate = df.iloc[-1,0] 
+            self.startdate = df.iloc[0, 0]
+
+
+        elif self.type != 'format1': # If the data is not the
+            df= self.dataframe
+            df['Data'] = pd.to_datetime(df['Data'], format="%d/%m/%Y")
+            df = df.drop_duplicates(subset='Data', keep="last")
 
             if comma_to_dot:
-                df_ordenado = df_ordenado.replace({',': '.'}, regex=True)
-                df_ordenado = df_ordenado.reset_index()
-                df_ordenado = df_ordenado.drop(columns='index')
-                self.dataframe = df_ordenado
-            if grow:
-                self.daframe = df_ordenado.sort_values(by=['Data'], ascending=True)
+                df = df.replace({',': '.'}, regex=True)
+                df = df.reset_index()
+                df = df.drop(columns='index')
+                self.dataframe = df
+            if not grow:
+                self.dataframe = df.sort_values(by=['Data'], ascending=True)
 
             data = np.array([])
             pr = np.array([])
             self.only_mondata()
 
-            # indução
+            # remove data that don't exits
             colum = self.dataframe.columns
+            n=0
             for linha in range(len(self.dataframe)):
                 for dia in range(1, 32):
                     try:
                         temp = self.dataframe[colum[0]][linha]
-                        data = np.append(data, datetime.datetime(temp.year, temp.month, dia)) # check if the date is real
+                        data = np.append(data, pd.to_datetime(datetime(temp.year, temp.month, dia)))  # check if the date is real
                         pr = np.append(pr, float(self.dataframe[colum[dia]][linha]))
                     except:
-                        continue
+                        n+= 0
+            a = pd.date_range(start=str(self.enddate.year), end=str(self.enddate.year), freq='D')
+            a = a[:-1]
+            pr_def = np.full(len(a), np.nan)
+            for i in range(len(data)):
+                ind = np.argwhere(data[i] == a)
+                pr[ind] = pr[i]
 
-            # chech if have date jump
-            a = pd.date_range(start=self.startdate, end=self.enddate)
 
-            for i in range(len(a)):
-                try:
-                    while np.datetime64(data[i]) != np.datetime64(a[i]):
-                        data = np.insert(data, i, data[i - 1] + timedelta(days=1))
-                        pr = np.insert(pr, i, 0)
-                        pr[i] = np.NaN
-                except:
-                    continue
-            data = pd.date_range(start=self.startdate, end=self.enddate)  # change data to numpy datetime64
-            self.dataframe = pd.DataFrame(list(zip(data, pr)), columns=['time', 'pr'])
+            self.dataframe = pd.DataFrame(list(zip(a, pr_def)), columns=['time', 'pr'])
+
             # atualize the format and len
             self.type = "format1"
             self.len = len(self.dataframe)
+            self.enddate = df.iloc[-1,0] 
+            self.startdate = df.iloc[0, 0]
 
     def date(self, line):
         """
         This function get a especific date in a line
         :param linha:
         :return:
         """
@@ -404,14 +329,54 @@
                 if c!="Data" and c!= "Chuva31" and c!= "Chuva30" and c!= "Chuva29":
                     s += np.sum(np.isnan(self.dataframe[f'{c}'].to_numpy("float32")))
             print("You are using the original data and this is a estimative, use format1 before to be precise")
             if type == "relative":
                 return s
             return (s/(self.enddate-self.startdate).days)*100
 
+    def report(self, path):
+            """
+            Save a txt file with importants informations
+
+            """
+            self.format1()
+            with open(path, 'w') as f:
+                f.write(f"Station {self.city} {self.code}\n")
+                f.write(f"Empty data of : {self.empty_data()}\n")
+                f.write(f"Max value: {np.max(self.dataframe.iloc[:, 1])}\n")
+                v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of max value: {v.day}/{v.month}/{v.year}\n")
+                f.write(f"Min value: {np.min(self.dataframe.iloc[:, 1])}\n")
+                v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of min value: {v.day}/{v.month}/{v.year}\n")
+                f.close()
+    def report_mf(self, path_in, path_out, years=(0,0)):
+        """
+        Save a txt file with imports informations of multiples files
+
+        :param path_in: folder when are the files, only the files
+        :param path_out: Folder when the output will be save
+        """
+    
+        files = os.listdir(path_in)
+        df = pd.DataFrame(columns=["Code of station", "Period", "Missing data","Missing Data (%)", "Max value", "Date of max"])
+        df["Code of station"] = np.arange(len(files))
+        for i in range(len(files)):
+            ana = Ana(path_in+"/"+files[i])
+            if years==(0,0):
+                ana.format1()
+            else:
+                ana.format1(years=years)
+            df.iloc[i, 0] = ana.code #Salva o código da estação 
+            df.iloc[i, 1] = f"{ana.startdate}-{ana.enddate}" #Salva o período da estação 
+            df.iloc[i, 2] = ana.empty_data() #Salva os dados faltantes 
+            df.iloc[i, 3] = ana.empty_data(type="relative")#Salva os dados faltantes relativos 
+            df.iloc[i, 4] = np.max(ana.dataframe.iloc[:, 1]) #Salva o valor máximo 
+            df.iloc[i, 5] = ana.dataframe.iloc[np.argmax(ana.dataframe.iloc[:,1]), 0] # Salva a data do valor máximo
+        df.to_csv(path_out)
     # select data or return a data
     def get_year(self,year, with_x=False, return_x0=False):
         """
         From array muti-year, return a year specific
         :param year: can by a Int, or list of Int
         :param with_x:
         :param return_x0: Return the index init
@@ -527,19 +492,27 @@
         # add variable attribute metadata
         ds.attrs['lat'] = 'Units: °'
         ds.attrs['lon'] = 'Units: °'
         ds.attrs['time'] = 'daily data of time'
 
         ds.to_netcdf(path)
 
-    def to_csv(self, pasta, sep=';', index=False, var="all"):
+    def to_csv(self, path, sep=';', index=False, var="all"):
         if var=="all":
-            self.dataframe.to_csv(pasta, sep=sep, index=index)
+            self.get_info()
+            with open(f"{path}", "w") as f:
+                f.write(f"var,value\n")
+                f.write(f"lon,{self.lon}\n")
+                f.write(f"lat, {self.lat}\n")
+                f.write(f"alt,{self.alt}\n")
+                f.write(f"name,{self.name}\n")
+                f.write(f"numcity, {self.NumCity}\n")
+                f.write(f"{self.dataframe.to_csv(index=False)}")
         else:
-            a = self.dataframe[f"{var}"].to_csv(pasta, sep=sep, index=index)
+            a = self.dataframe[f"{var}"].to_csv(path, sep=sep, index=index)
 
     def haversine(self, lon1, lat1):
         """
         Calculate the great circle distance in kilometers between a point and the stations self
         on the earth (specified in decimal degrees)
         
         :param lon1: float, position longitude
@@ -636,17 +609,15 @@
         for k in range(size):
 
             y[k] = y[k]/d[k]
         if retornar:
             if with_x:
                 return x, y
             return y
-        print(x.size, y.size)
         self.dataframe = pd.DataFrame(zip(x.tolist(), y.tolist()), columns=['time', 'pr'])
-        print(self.dataframe)
         self.type_data = 'format1'
 
     # Download data
     def download(self,codigo="NaN", format='csv', dir='', tipo_especifico=False, save_zip=False,
                  state="NaN", city="Nan"):
         """
         Download the Ana data. Code from https://github.com/joaohuf/Ferramentas_HidroWeb
```

### Comparing `AgenciBr-0.1.7/AgenciBr/Ideam.py` & `AgenciBr-0.1.8/AgenciBr/Ideam.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 import matplotlib.pyplot as plt
 from datetime import timedelta
 
 #Site to get data http://dhime.ideam.gov.co/atencionciudadano/
 
 class Ideam():
     def __init__(self, path, encoding='utf-8', sep='|', type='t_maxmin', serie='diário'):
+        def type_data(df, type):
+            return type
 
         def dataframe():
             if type == 't_maxmin':
                 df = pd.read_csv(path, encoding=encoding,
                                  index_col=False, sep=sep)
                 df["Fecha"] = pd.to_datetime(df['Fecha']).dt.date
                 return df
 
         import pandas as pd
         self.dataframe = dataframe()
-        self.type = type
+        self.type = "original" 
         self.len = len(self.dataframe)
-        self.type_data = 'original'
+        self.type_data = type_data(self.dataframe, type)
         self.startdate = self.dataframe['Fecha'][0]
         self.enddate = self.dataframe['Fecha'][len(self.dataframe) - 1]
-
     def byYear(self, year, var):
         """
         This function get the file and the var and return the data from this year
 
         :param year: type int
         :param var: type str with data var to get
         :return: data from colum 'var' and data in year 'year'
@@ -47,15 +48,15 @@
     def report(self, path):
         """
         Save a txt file with importants informations
 
         """
         self.format1()
         if (self.type_data == "precipitation"):
-            with open(path+"/report.txt", 'w') as f:
+            with open(path, 'w') as f:
                 #f.write(f"Station {self.city} {self.code}\n")
                 f.write(f"Empty data of : {self.empty_data()}\n")
                 f.write(f"Max value: {np.max(self.dataframe.iloc[:, 1])}\n")
                 v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
                 f.write(f"Date of max value: {v.day}/{v.month}/{v.year}\n")
                 f.write(f"Min value: {np.min(self.dataframe.iloc[:, 1])}\n")
                 v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
@@ -245,140 +246,60 @@
             self.dataframe['Fecha'] = pd.to_datetime(self.dataframe['Fecha'])
             self.dataframe['Valor'] = np.array(self.dataframe['Valor']).astype(float)
             self.dataframe = self.dataframe.rename(columns={'Fecha': 'time', 'Valor': 'pr'})
             if comma_to_dot:
                 self.dataframe = self.dataframe.replace({',': '.'}, regex=True)
 
             data = self.dataframe["time"]
-            date = pd.date_range(start=self.startdate,
-                                 end=self.enddate)  # change data to numpy datetime64
             pr = self.dataframe["pr"]
-            for i in range(len(date)):
-                if data[i] != date[i]:
-                    t = pd.date_range(data[i - 1], data[i])[1:-1]
-                    data = np.concatenate((data[:i], t, data[i:]))
-                    pr = np.concatenate((pr[:i+1], (len(t)-2) * [np.NaN], pr[i-1:]))
-
-            if (float(years[0]) in pd.DatetimeIndex(data).year) and (float(years[1]) not in pd.DatetimeIndex(
-                    data).year):  # The first date is in array and end date not
-                if self.startdate != datetime(self.startdate.year, 1,
-                                              1):  # complete missing days start, if don't start in 1/1
-                    data = np.concatenate((pd.date_range(start=f"1/1/{int(self.startdate.year)}",
-                                                         end=self.startdate).to_numpy(), data[1:]))
-                    a = np.ones(np.size(pd.date_range(start=f"1/1/{int(years[0])}", end=self.startdate).to_numpy()))
-                    a[:] = np.nan
-                    pr = np.concatenate((a[:-1], pr))
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                i = np.where(date[0] == data)[0][0]
-                t = np.empty(np.size(date))
-                t[:] = np.nan
-                t[:len(pr[i:])] = pr[i:]
-                pr = t
-
-            elif float(years[1]) in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                    data).year:  # The end date is in array and first date not
-                # complete end date to 31/12 if don't go
-
-                if self.enddate != datetime.date(self.enddate.year, 12, 31):
-                    t = np.empty((datetime.date(self.enddate.year, 12, 31) - self.enddate).days)
-                    t[:] = np.nan
-                    pr = np.concatenate((pr, t))
-                    data = np.concatenate((data[:-1], pd.date_range(start=data[-1], end=f"31/12/{int(self.enddate.year)}")))
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                # The index where is the end date
-                f = np.where(date[-1] == data)[0][0]
-
-                t = np.empty(len(date))
-                t[:] = np.nan
-                t[-len(data[:f]):] = pr[:f]
-                pr = t
-
-            elif float(years[1]) not in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                    data).year:  # The end date is not in array and first date not in
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                # The index of dates that we have data
-                print(date, data)
-                i = np.where(data[0] == date)[0][0]
-                f = np.where(data[-1] == date)[0][0]
-                t = np.empty(np.size(date))  # will be precipitation data
-                t[:] = np.nan
-                # armazene the data
-                date[i:f] = data[:-1]
-                t[i:f] = pr[:-1]
-
-                # Change the variable name
-                pr = t
-
-
-            else:  # both dates ar e in array
-                if self.startdate != datetime.date(self.enddate.year, 1,
-                                              1):  # complete missing days start, if don't start in 1/1
-
-                    data = np.concatenate(
-                        [pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate), data[1:]])
-
-                    a = np.ones(
-                        np.size(pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy()))
-
-                    a[:] = np.nan
 
-                    pr = np.concatenate([a[:-1], pr])
-
-                if self.enddate != datetime.date(self.enddate.year, 12, 31):
-                    t = np.empty((datetime.date(self.enddate.year, 12, 31) - self.enddate).days)
-
-                    t[:] = np.nan
-
-                    pr = np.concatenate((pr, t))
-
-                    data = np.concatenate((data, pd.date_range(start=data[-1], end=f"31/12/{self.enddate.year}")[1:]))
-
-                date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-                # index of strat date and end date(i, f)
-
-                i = np.where(date[0] == data)[0][0]
-
-                f = np.where(date[-1] == data)[0][0]
-
-                date = data[i:f]
+            # chech if have date jump
+            a = pd.date_range(start=str(years[0]), end=str(years[1]), freq='D')
+            a=a[:-1]
+            pr_def = np.full(len(a), np.nan)
+            for i in range(len(data)):
+                ind = np.argwhere(data[i] == a)
+                pr_def[ind] = pr[i]
 
-                pr = pr[i:f]
+            df = pd.DataFrame(list(zip(a, pr_def)), columns=['time', 'pr'])
 
-            self.dataframe = pd.DataFrame(list(zip(date, pr)), columns=['time', 'pr'])
+            # atualize the format and len
+            self.type = "format1"
+            df = df[(df.iloc[:, 0].dt.year <= years[1])]
+            self.dataframe = df[df.iloc[:, 0].dt.year >= years[0]]
+            self.len = len(self.dataframe)
+            self.enddate = df.iloc[-1,0] 
+            self.startdate = df.iloc[0, 0]
 
             # atualize the format and len
             self.type = "format1"
             self.len = len(self.dataframe)
 
         elif self.type != "format1":
-            print(self.dataframe)
             self.dataframe['Fecha'] = pd.to_datetime(self.dataframe['Fecha'])
             self.dataframe['Valor'] = np.array(self.dataframe['Valor']).astype(float)
             self.dataframe = self.dataframe.rename(columns={'Fecha': 'time', 'Valor': 'pr'})
             if comma_to_dot:
                 self.dataframe = self.dataframe.replace({',': '.'}, regex=True)
 
             colum = self.dataframe.columns
             data = pd.to_datetime(self.dataframe[colum[0]])
             pr = self.dataframe[colum[1]].to_numpy()
 
             # chech if have date jump
-            a = pd.date_range(self.startdate, self.enddate)
-            for i in range(len(a)):
-                if data[i] != a[i]:
-                    t = pd.date_range(data[i - 1], data[i])[1:-1]
-                    data = np.concatenate((data[:i], t, data[i:]))
-                    pr = np.concatenate((pr[:i+1], (len(t)-2) * [np.NaN], pr[i-1:]))
-            data = pd.date_range(self.startdate,
-                                 end=self.enddate)  # change data to numpy datetime64
+            a = pd.date_range(start=self.startdate, end=self.enddate, freq='D')
+            a=a[:-1]
+            pr_def = np.full(len(a), np.nan)
+            for i in range(len(data)):
+                ind = np.argwhere(data[i] == a)
+                pr_def[ind] = pr[i]
+
+            self.dataframe = pd.DataFrame(list(zip(a, pr_def)), columns=['time', 'pr'])
+
 
-            self.dataframe = pd.DataFrame(list(zip(data, pr)), columns=['time', 'pr'])
         self.type_data = 'precipitation'
         self.type = "format1"
 
     def get_year(self,year, with_x=False, return_x0=False):
         """
         English:
             From array multi-year, return a year specific
```

### Comparing `AgenciBr-0.1.7/AgenciBr/Inemet.py` & `AgenciBr-0.1.8/AgenciBr/Inemet.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 if 'Codigo' in temp:
                     ind = temp.index('Codigo')
                     temp = temp[ind + 2]
                     return temp
                 line_codigo += 1
 
         def type_data(x):
-            if x == ("t_maxmin" or "precipitation"):  #If user say the variable
+            if x in ("t_maxmin", "precipitation"):  #If user say the variable
                 return x
             df = pd.read_csv(path, skiprows=linha_inicio_df(path), nrows=50, on_bad_lines='skip')
             temp = str.lower(''.join(df.columns))
             if 'temperatura' in temp:
                 if "minima" and 'maxima' in temp:
 
                     del df
@@ -128,15 +128,15 @@
                     return temp
                 line_codigo += 1
 
         def dataframe():
             if self.type_data == 't_maxmin':
                 df = pd.read_csv(path, encoding=encoding,
                                          index_col=False, sep=sep, skiprows=linha_inicio_df(path))
-                df.columns = ['Data', 'max', 'min', '']
+                df.columns = ['Data', 'max', 'min','']
                 df = df.drop(columns='')
                 return df
             elif self.type_data == 'precipitation':
                 df = pd.read_csv(path, encoding=encoding,
                                  index_col=False, sep=sep, skiprows=linha_inicio_df(path))
                 df.columns = ['Data', 'pr', '']
                 df = df.drop(columns='')
@@ -175,20 +175,20 @@
     def empty_data(self, type='absolute'):
         import math
 
         if self.type != "format1":
             self.format1(comma_to_dot=True)
         # if data is temperature
         if self.type_data == 't_maxmin':
-            c = np.sum(np.isnan(self.dataframe.iloc[:,1])) # Nan of max temperature
-            c+= np.sum(np.isnan(self.dataframe.iloc[:,2])) #Nan of min temperature
+            cmax = np.sum(np.isnan(self.dataframe.iloc[:,1])) # Nan of max temperature
+            cmin = np.sum(np.isnan(self.dataframe.iloc[:,2])) #Nan of min temperature
             if type == 'relative':
-                return (c / len(self.dataframe)) * 100
+                return ((cmax / len(self.dataframe)) * 100, (cmin/len(self.dataframe))*100)
             elif type == 'absolute':
-                return c
+                return cmax, cmin
             else:
                 raise "select one of two possibles types 'relative' or 'absolute'"
 
         # se estamos tratando de precipitação
         elif self.type_data == 'precipitation':
             c = np.sum(np.isnan(self.dataframe.iloc[:, 1]))
             if type == 'relative':
@@ -200,15 +200,15 @@
     def report(self, path):
         """
         Save a txt file with importants informations
 
         """
         self.format1()
         if (self.type_data == "t_maxmin"):
-            with open(path+"/report.txt", 'w') as f:
+            with open(path, 'w') as f:
                 f.write(f"Station {self.city} {self.code}\n")
                 f.write(f"Empty data of {self.type_data} : {self.empty_data()}\n")
                 f.write(f"Max value of max temperature: {np.max(self.dataframe.iloc[:, 1])}\n")
                 f.write(f"Max value of min temperature: {np.max(self.dataframe.iloc[:, 2])}\n")
                 v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
                 f.write(f"Date of max value of max temperature: {v.day}/{v.month}/{v.year}\n")
                 v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 2]),0]
@@ -217,25 +217,51 @@
                 f.write(f"Min value of min temperature: {np.min(self.dataframe.iloc[:, 2])}\n")
                 v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
                 f.write(f"Date of min value of max temperature: {v.day}/{v.month}/{v.year}\n")
                 v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 2]),0]
                 f.write(f"Date of min value of min temperature: {v.day}/{v.month}/{v.year}\n")
                 f.close()
         elif (self.type_data == "precipitation"):
-            with open(path+"/report.txt", 'w') as f:
+            with open(path, 'w') as f:
                 f.write(f"Station {self.city} {self.code}\n")
                 f.write(f"Empty data of {self.type_data}: {self.empty_data()}\n")
                 f.write(f"Max value: {np.max(self.dataframe.iloc[:, 1])}\n")
                 v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
                 f.write(f"Date of max value: {v.day}/{v.month}/{v.year}\n")
                 f.write(f"Min value: {np.min(self.dataframe.iloc[:, 1])}\n")
                 v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
                 f.write(f"Date of min value: {v.day}/{v.month}/{v.year}\n")
                 f.close()
+    def report_mf(self, path_in, path_out, var="precipitation", years=(0, 0)):
+            """
+            Save a txt file with imports informations of multiples files
 
+            :param path_in: folder when are the files, only the files
+            :param path_out: Folder when the output will be save
+            """
+            import pandas as pd
+            files = os.listdir(path_in)
+            if ( var == "t_maxmin" ):
+                df = pd.DataFrame(columns=["Code of station", "Period", "Missing data Tmax","Missing data Tmin", "Max value Tmax","Max value Tmin", "Date of max Tmax", "Date max Tmin"])
+                df["Code of station"] = np.arange(len(files))
+                for i in range(len(files)):
+                    ana = Inemet(path_in+"/"+files[i])
+                    if (years == (0,0)):
+                        ana.format1()
+                    else:
+                        ana.format1(years=years)
+                    df.iloc[i, 0] = ana.code #Salva o código da estação 
+                    df.iloc[i, 1] = f"{ana.startdate.day}/{ana.startdate.month}/{ana.startdate.year} - {ana.enddate.day}/{ana.enddate.day}/{ana.enddate.year}" #Salva o período da estação 
+                    df.iloc[i, 2], df.iloc[i, 3] = ana.empty_data() #Salva os dados faltantes 
+                    df.iloc[i, 4] = np.max(ana.dataframe.iloc[:, 1]) #Salva o valor máximo 
+                    df.iloc[i, 5] = np.max(ana.dataframe.iloc[:, 2]) #Salva o valor máximo 
+                    df.iloc[i, 6] = ana.dataframe.iloc[np.argmax(ana.dataframe.iloc[:, 1]), 0]
+                    df.iloc[i, 7] = ana.dataframe.iloc[np.argmax(ana.dataframe.iloc[:, 2]), 0]
+                df.to_csv(path_out)
+             
     def plot(self):
         """
 
         :param title:
         :param xlabel:
         :param ylabel:
         :return:
@@ -335,136 +361,75 @@
         if self.type_data == 'precipitation':
             import datetime
             # if change to format1 and complete the years
             if self.type != 'format1' and years != (0, 0):
                 from datetime import datetime
 
                 # organize the file from smaller to larger
-                df_ordenado = self.dataframe
-                df_ordenado['Data'] = pd.to_datetime(df_ordenado['Data'], format="%Y-%m-%d")
-                df_ordenado = df_ordenado.drop_duplicates(subset='Data')
-                df_ordenado = df_ordenado.rename(columns={"Data": 'time'})
+                df = self.dataframe
+                df['Data'] = pd.to_datetime(df['Data'], format="%Y-%m-%d")
+                df = df.drop_duplicates(subset='Data', keep="last")
+                df = df.rename(columns={"Data": 'time'})
 
                 if comma_to_dot:
-                    df_ordenado = df_ordenado.replace({',': '.'}, regex=True)
-                    df_ordenado = df_ordenado.reset_index()
-                    df_ordenado = df_ordenado.drop(columns='index')
-                    self.dataframe = df_ordenado
+                    df = df.replace({',': '.'}, regex=True)
+                    df = df.reset_index()
+                    df = df.drop(columns='index')
+                    self.dataframe = df
                 if not grow:
-                    self.dataframe = df_ordenado.sort_values(by=['time'], ascending=True)
+                    self.dataframe = df.sort_values(by=['time'], ascending=True)
 
                 a = pd.date_range(start=datetime.date(self.startdate),
                                      end=self.enddate)
-                data = pd.to_datetime(df_ordenado["time"])
-                pr = np.array(df_ordenado['pr'])
+                a=a[:-1]
+                data = pd.to_datetime(df["time"])
+                pr = np.array(df['pr'])
                 for i in range(len(a)):
                     if data[i] != a[i]:
                         t = pd.date_range(data[i - 1], data[i])[1:-1]
                         data = np.concatenate((data[:i], t, data[i:]))
                         pr = np.concatenate((pr[:i+1], (len(t)-2) * [np.NaN], pr[i-1:]))
                 data = pd.date_range(start=datetime.date(self.startdate),
                                      end=self.enddate)  # change data to numpy datetime64
                 del a
 
-                # select the year series
-                if (float(years[0]) in pd.DatetimeIndex(data).year) and (float(years[1]) not in pd.DatetimeIndex(
-                        data).year):  # The first date is in array and end date not
-                    if self.startdate != datetime(self.startdate.year, 1, 1):  # complete missing days start, if don't start in 1/1
-                        data = np.concatenate(
-                            (pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy(), data[1:]))
-                        a = np.ones(np.size(pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy()))
-                        a[:] = np.nan
-                        pr = np.concatenate((a[:-1], pr))
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    i = np.where(date[0] == data)[0][0]
-                    t = np.empty(np.size(date))
-                    t[:] = np.nan
-                    t[:len(pr[i:])] = pr[i:]
-                    pr = t
-
-                elif float(years[1]) in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                        data).year:  # The end date is in array and first date not
-                    # complete end date to 31/12 if don't go
-                    if self.enddate != datetime(self.enddate.year, 12, 31):
-                        t = np.empty((datetime(self.enddate.year, 12, 31) - self.enddate).days)
-                        t[:] = np.nan
-                        pr = np.concatenate((pr, t))
-                        data = np.concatenate(
-                            (data, pd.date_range(start=data[-1], end=f"31/12/{self.enddate.year}")))
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    # The index where is the end date
-                    f = np.where(date[-1] == data)[0][0]
-
-                    t = np.empty(len(date))
-                    t[:] = np.nan
-                    t[-len(data[:f]):] = pr[:f]
-                    pr = t
-
-                elif float(years[1]) not in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                        data).year:  # The end date is not in array and first date not in
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    # The index of dates that we have data
-                    i = np.where(data[0] == date)[0][0]
-                    f = np.where(data[-1] == date)[0][0]
-                    t = np.empty(np.size(date))  # will be precipitation data
-                    t[:] = np.nan
-
-                    # armazene the data
-                    date[i:f] = data[:-1]
-                    t[i:f] = pr[:-1]
-                    # Change the variable name
-                    pr = t
-
-                else:  # both dates are in array
-                    if self.startdate != datetime(self.startdate.year, 1, 1):  # complete missing days start, if don't start in 1/1
-                        data = np.concatenate(
-                            (pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy(), data[1:]))
-
-                        a = np.ones(np.size(pd.date_range(start=f"1/1/{int(years[0])}", end=self.startdate).to_numpy()))
-                        a[:] = np.nan
-                        pr = np.concatenate((a[:-1], pr))
-                    if self.enddate != datetime(self.enddate.year, 12, 31) and self.enddate.year == years[-1]:
-                        t = np.empty((datetime(self.enddate.year, 12, 31) - self.enddate).days)
-                        t[:] = np.nan
-                        pr = np.concatenate((pr, t))
-                        data = np.concatenate(
-                            (data, pd.date_range(start=data[-1], end=f"31/12/{int(self.enddate.year)}")[1:]))
-
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-                    # index of strat date and end date(i, f)
-                    i = np.where(date[0] == data)[0][0]
-                    f = np.where(date[-1] == data)[0][0]
-
-                    date = data[i:f+1]
-                    pr = pr[i:f+1]
+                # chech if have date jump
+                a = pd.date_range(start=str(years[0]), end=str(years[1]), freq='D')
+                a=a[:-1]
+                pr_def = np.full(len(a), np.nan)
+                for i in range(len(data)):
+                    ind = np.argwhere(data[i] == a)
+                    pr_def[ind] = pr[i]
 
-                self.dataframe = pd.DataFrame(list(zip(date, pr)), columns=['time', 'pr'])
+                df = pd.DataFrame(list(zip(a, pr_def)), columns=['time', 'pr'])
 
                 # atualize the format and len
                 self.type = "format1"
+                df = df[(df.iloc[:, 0].dt.year <= years[1])]
+                self.dataframe = df[df.iloc[:, 0].dt.year >= years[0]]
                 self.len = len(self.dataframe)
+                self.enddate = df.iloc[-1,0] 
+                self.startdate = df.iloc[0, 0]
+
 
             elif self.type != 'format1':
                 from datetime import datetime
 
                 # organize the file from smaler to larger
-                df_ordenado = self.dataframe
-                df_ordenado['Data'] = pd.to_datetime(df_ordenado['Data'], format="%Y-%m-%d")
-                df_ordenado = df_ordenado.drop_duplicates(subset='Data')
-                df_ordenado = df_ordenado.rename(columns={"Data":'time'})
+                df = self.dataframe
+                df['Data'] = pd.to_datetime(df['Data'], format="%Y-%m-%d")
+                df = df.drop_duplicates(subset='Data', keep="last")
+                df = df.rename(columns={"Data":'time'})
                 if comma_to_dot:
-                    df_ordenado = df_ordenado.replace({',': '.'}, regex=True)
-                    df_ordenado = df_ordenado.reset_index()
-                    df_ordenado = df_ordenado.drop(columns='index')
-                    self.dataframe = df_ordenado
+                    df = df.replace({',': '.'}, regex=True)
+                    df = df.reset_index()
+                    df = df.drop(columns='index')
+                    self.dataframe = df
                 if not grow:
-                    self.dataframe = df_ordenado.sort_values(by=['time'], ascending=True)
+                    self.dataframe = df.sort_values(by=['time'], ascending=True)
 
                 colum = self.dataframe.columns
                 data = pd.to_datetime(self.dataframe[colum[0]])
                 pr = self.dataframe[colum[1]].to_numpy()
 
                 # chech if have date jump
                 a = np.arange(self.startdate, self.enddate, timedelta(days=1)).astype(datetime)
@@ -479,29 +444,29 @@
                 df = pd.DataFrame(list(zip(data, pr)), columns=['time', 'pr'])
                 self.dataframe = df
 
         elif self.type_data == 't_maxmin':
             from datetime import datetime
 
             # organize the date from smallest to bigest
-            df_ordenado = self.dataframe
-            df_ordenado['Data'] = pd.to_datetime(df_ordenado['Data'], format="%Y-%m-%d")
-            df_ordenado = df_ordenado.drop_duplicates(subset='Data')
+            df = self.dataframe
+            df['Data'] = pd.to_datetime(df['Data'], format="%Y-%m-%d")
+            df = df.drop_duplicates(subset='Data', keep="last")
 
             # comma to point
             if comma_to_dot:
-                df_ordenado = df_ordenado.replace({',': '.'}, regex=True)
-                df_ordenado = df_ordenado.reset_index()
-                df_ordenado = df_ordenado.drop(columns='index')
-                df_ordenado = df_ordenado.rename(columns={"Data": 'time'})
-                self.dataframe = df_ordenado
+                df = df.replace({',': '.'}, regex=True)
+                df = df.reset_index()
+                df = df.drop(columns='index')
+                df = df.rename(columns={"Data": 'time'})
+                self.dataframe = df
 
             if not grow:
-                df_ordenado = df_ordenado.rename(columns={'Data': 'Data'})
-                self.dataframe = df_ordenado.sort_values(by=['Data'], ascending=True)
+                df = df.rename(columns={'Data': 'Data'})
+                self.dataframe = df.sort_values(by=['Data'], ascending=True)
                 self.dataframe = self.dataframe.rename(columns={"Data": 'time'})
             # if change to format1 and complete the years
             if self.type != 'format1' and years != (0, 0):
                 colum = self.dataframe.columns
                 data = pd.to_datetime(self.dataframe[colum[0]])
                 max = np.array(self.dataframe[colum[1]].to_numpy())
                 min = np.array(self.dataframe[colum[2]].to_numpy())
@@ -512,126 +477,38 @@
                 # chech if have date jump
                 for i in range(len(a)):
                     if data[i] != a[i]:
                         t = pd.date_range(data[i - 1], data[i])[1:-1]
                         data = np.concatenate((data[:i], t, data[i:]))
                         max = np.concatenate((max[:i], len(t) * [np.NaN], max[i:]))
                         min = np.concatenate((min[:i], len(t) * [np.NaN], min[i:]))
-                data = pd.date_range(start=datetime.date(self.startdate),
-                                     end=self.enddate)  # change data to numpy datetime64
-                # select the year series
-                if (float(years[0]) in pd.DatetimeIndex(data).year) and (float(years[1]) not in pd.DatetimeIndex(
-                        data).year):  # The first date is in array and end date not
-                    if self.startdate != datetime(self.startdate.year, 1,
-                                                  1):  # complete missing days start, if don't start in 1/1
-                        data = np.concatenate(
-                            (
-                            pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy(), data[1:]))
-                        a = np.ones(
-                            np.size(pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy()))
-                        a[:] = np.nan
-                        max = np.concatenate((a[:-1], max))
-                        min = np.concatenate((a[:-1], min))
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    i = np.where(date[0] == data)[0][0]
-                    tmax = np.empty(np.size(date))
-                    tmin = np.empty(np.size(date))
-                    tmax[:] = np.nan
-                    tmax[:len(max[i:])] = max[i:]
-                    max = tmax
-                    tmin[:] = np.nan
-                    tmin[:len(min[i:])] = min[i:]
-                    min = tmin
-
-                elif float(years[1]) in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                        data).year:  # The end date is in array and first date not
-                    # complete end date to 31/12 if don't go
-                    if self.enddate != datetime(self.enddate.year, 12, 31):
-                        t = np.empty((datetime(self.enddate.year, 12, 31) - self.enddate).days)
-                        t[:] = np.nan
-                        max = np.concatenate((max, t))
-                        min = np.concatenate((min, t))
-                        data = np.concatenate(
-                            (data, pd.date_range(start=data[-1], end=f"31/12/{self.enddate.year}")))
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    # The index where is the end date
-                    f = np.where(date[-1] == data)[0][0]
-
-                    tmax = np.empty(len(date))
-                    tmax[:] = np.nan
-                    tmax[-len(data[:f]):] = max[:f]
-                    max = tmax
-                    tmin = np.empty(len(date))
-                    tmin[:] = np.nan
-                    tmin[-len(data[:f]):] = min[:f]
-                    min = tmin
-
-                elif float(years[1]) not in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                        data).year:  # The end date is not in array and first date not in
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    # The index of dates that we have data
-                    i = np.where(data[0] == date)[0][0]
-                    f = np.where(data[-1] == date)[0][0]
-                    t = np.empty(np.size(date))  # will be temperature data
-                    t[:] = np.nan
-
-                    # armazene the data
-                    date[i:f] = data[:-1]
-                    t[i:f] = max[:-1]
-                    max = t
-
-                    t = np.empty(np.size(date))  # will be temperature data
-                    t[:] = np.nan
-                    date[i:f] = data[:-1]
-                    t[i:f] = min[:-1]
-                    min = t
-
-                else:  # both dates are in array
-                    if self.startdate != datetime(self.startdate.year, 1,
-                                                  1):  # complete missing days start, if don't start in 1/1
-                        data = np.concatenate(
-                            (
-                            pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy(), data[1:]))
-
-                        a = np.ones(np.size(pd.date_range(start=f"1/1/{int(years[0])}", end=self.startdate).to_numpy()))
-                        a[:] = np.nan
-                        max = np.concatenate((a[:-1], max))
-                        min = np.concatenate((a[:-1], min))
-                    if self.enddate != datetime(self.enddate.year, 12, 31) and self.enddate.year == years[-1]:
-                        t = np.empty((datetime(self.enddate.year, 12, 31) - self.enddate).days)
-                        t[:] = np.nan
-                        max = np.concatenate((max, t))
-                        min = np.concatenate((min, t))
-                        data = np.concatenate(
-                            (data, pd.date_range(start=data[-1], end=f"31/12/{int(self.enddate.year)}")[1:]))
-
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-                    # index of strat date and end date(i, f)
-                    i = np.where(date[0] == data)[0][0]
-                    f = np.where(date[-1] == data)[0][0]
-
-                    date = data[i:f + 1]
-                    max = max[i:f+1]
-                    min = min[i:f+1]
-
-                self.dataframe = pd.DataFrame(list(zip(date, max, min)), columns=['time', 'max', "min"])
 
+                a = pd.date_range(start=str(years[0]), end=str(years[1]), freq='D')
+                a=a[:-1]
+                max_def = np.full(len(a), np.nan)
+                min_def = np.full(len(a), np.nan)
+                for i in range(len(data)):
+                    ind = np.argwhere(data[i] == a)
+                    max_def[ind] = max[i]
+                    min_def[ind] = min[i]
                 # atualize the format and len
+                self.dataframe = pd.DataFrame(list(zip(a, max, min)), columns=['time', 'max', "min"])
                 self.type = "format1"
                 self.len = len(self.dataframe)
+                self.enddate = df.iloc[-1,0] 
+                self.startdate = df.iloc[0, 0]
+
             elif self.type != "format1":
                 colum = self.dataframe.columns
                 data = pd.to_datetime(self.dataframe[colum[0]])
                 max = self.dataframe[colum[1]].to_numpy()
                 min = self.dataframe[colum[2]].to_numpy()
                 a = pd.date_range(start=datetime.date(self.startdate),
                                      end=self.enddate)
+                a=a[:-1]
 
 
                 # chech if have date jump
                 for i in range(len(a)):
                     if data[i] != a[i]:
                         t = pd.date_range(data[i - 1], data[i])[1:-1]
                         data = np.concatenate((data[:i], t, data[i:]))
@@ -645,26 +522,26 @@
                 self.type = "format1"
                 self.len = len(self.dataframe)
                 self.dataframe = pd.DataFrame(list(zip(data, max, min)), columns=['time', 'max', 'min'])
         elif self.type_data == 't_med':
             from datetime import datetime
         
             # Organizando o arquivo pela datas do menor até o maior
-            df_ordenado = self.dataframe
-            df_ordenado['Data'] = pd.to_datetime(df_ordenado['Data'], format="%Y-%m-%d")
-            df_ordenado = df_ordenado.drop_duplicates(subset='Data')
+            df = self.dataframe
+            df['Data'] = pd.to_datetime(df['Data'], format="%Y-%m-%d")
+            df = df.drop_duplicates(subset='Data', keep="last")
             if comma_to_dot:
-                df_ordenado = df_ordenado.replace({',': '.'}, regex=True)
-                df_ordenado = df_ordenado.rename(columns={'Data': 'time'})
-                df_ordenado = df_ordenado.reset_index()
-                df_ordenado = df_ordenado.drop(columns='index')
-                self.dataframe = df_ordenado
+                df = df.replace({',': '.'}, regex=True)
+                df = df.rename(columns={'Data': 'time'})
+                df = df.reset_index()
+                df = df.drop(columns='index')
+                self.dataframe = df
             if not grow:
-                df_ordenado = df_ordenado.rename(columns={'Data': 'time'})
-                self.dataframe = df_ordenado.sort_values(by=['time'], ascending=True)
+                df = df.rename(columns={'Data': 'time'})
+                self.dataframe = df.sort_values(by=['time'], ascending=True)
 
             colum = self.dataframe.columns
             data = self.dataframe[colum[0]].to_numpy()
             med = self.dataframe[colum[1]].to_numpy()
             date = pd.date_range(start=datetime.date(self.startdate),
                                  end=self.enddate)  # change data to numpy datetime64
             # chech if have date jump
@@ -673,101 +550,25 @@
                     while np.datetime64(data[i]) != np.datetime64(date[i]):
                         data = np.insert(data, i, data[i - 1] + timedelta(days=1))
                         med = np.insert(med, i, np.NaN)
                 except:
                     continue
 
             if self.type == "format1" and years != (0,0):
-                # select the year series
-                if (float(years[0]) in pd.DatetimeIndex(data).year) and (float(years[1]) not in pd.DatetimeIndex(
-                        data).year):  # The first date is in array and end date not
-                    if self.startdate != datetime(self.startdate.year, 1,
-                                                  1):  # complete missing days start, if don't start in 1/1
-                        data = np.concatenate(
-                            (
-                                pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy(),
-                                data[1:]))
-                        a = np.ones(
-                            np.size(pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy()))
-                        a[:] = np.nan
-                        med = np.concatenate((a[:-1], med))
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    i = np.where(date[0] == data)[0][0]
-                    t = np.empty(np.size(date))
-                    t[:] = np.nan
-                    t[:len(med[i:])] = med[i:]
-                    med = t
-
-                elif float(years[1]) in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                        data).year:  # The end date is in array and first date not
-                    # complete end date to 31/12 if don't go
-                    if self.enddate != datetime(self.enddate.year, 12, 31):
-                        t = np.empty((datetime(self.enddate.year, 12, 31) - self.enddate).days)
-                        t[:] = np.nan
-                        med = np.concatenate((med, t))
-                        data = np.concatenate(
-                            (data, pd.date_range(start=data[-1], end=f"31/12/{self.enddate.year}")))
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    # The index where is the end date
-                    f = np.where(date[-1] == data)[0][0]
-
-                    t = np.empty(len(date))
-                    t[:] = np.nan
-                    t[-len(data[:f]):] = med[:f]
-                    med = t
-
-                elif float(years[1]) not in pd.DatetimeIndex(data).year and float(years[0]) not in pd.DatetimeIndex(
-                        data).year:  # The end date is not in array and first date not in
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-
-                    # The index of dates that we have data
-                    i = np.where(data[0] == date)[0][0]
-                    f = np.where(data[-1] == date)[0][0]
-                    t = np.empty(np.size(date))  # will be temperature data
-                    t[:] = np.nan
-
-                    # armazene the data
-                    date[i:f] = data[:-1]
-                    t[i:f] = med[:-1]
-                    med = t
-
-                else:  # both dates are in array
-                    if self.startdate != datetime(self.startdate.year, 1,
-                                                  1):  # complete missing days start, if don't start in 1/1
-                        data = np.concatenate(
-                            (
-                                pd.date_range(start=f"1/1/{self.startdate.year}", end=self.startdate).to_numpy(),
-                                data[1:]))
-
-                        a = np.ones(np.size(pd.date_range(start=f"1/1/{int(years[0])}", end=self.startdate).to_numpy()))
-                        a[:] = np.nan
-                        med = np.concatenate((a[:-1], med))
-                    if self.enddate != datetime(self.enddate.year, 12, 31) and self.enddate.year == years[-1]:
-                        t = np.empty((datetime(self.enddate.year, 12, 31) - self.enddate).days)
-                        t[:] = np.nan
-                        med = np.concatenate((med, t))
-                        data = np.concatenate(
-                            (data, pd.date_range(start=data[-1], end=f"31/12/{int(self.enddate.year)}")[1:]))
-
-                    date = pd.date_range(start=f"01/01/{int(years[0])}", end=f"31/12/{int(years[1])}").to_numpy()
-                    # index of strat date and end date(i, f)
-                    i = np.where(date[0] == data)[0][0]
-                    f = np.where(date[-1] == data)[0][0]
-
-                    date = data[i:f + 1]
-                    med = med[i:f + 1]
-
                 self.dataframe = pd.DataFrame(list(zip(date, med)), columns=['time', "med"])
 
                 # atualize the format and len
                 self.len = len(self.dataframe)
             elif self.type == "format":
                 self.dataframe = pd.DataFrame(list(zip(data, med)), columns=['time', 'med'])
+
+                # atualize the format and len
+                self.type = "format1"
+                self.len = len(self.dataframe)
+
         self.type = 'format1'
 
     def get_month(self, month, year, with_x=False):
         """
         From array muti-year, return a month specific
         :param month: The month to select as Int, or list of month to get
         :param year: The year to select
```

### Comparing `AgenciBr-0.1.7/AgenciBr/indice.py` & `AgenciBr-0.1.8/AgenciBr/indice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
 
-import numpy
 import numpy as np
 import pandas as pd
 
 # The index are based in: https://www.climdex.org/learn/indices/
 class Indice:
     def __init__(self, df):
         self.dataframe = df
@@ -563,11 +562,41 @@
             fim = self.date(self.len-1).year  # Ano de termino
             for ano in range(inicio, fim + 1):
                 for mes in range(1, 13):
                     try:
                         rx1day = np.append(rx1day,
                                            np.max(self.ByMonth(ano, mes, var=var)))  # o máximo de precipitação diária no ano
                     except:
-                        oi=1
+                        pass
             if with_x:
                 return pd.date_range(start =f'{inicio}-{self.date(0).month}-01',end =f'{fim}-{self.date(self.len-1).month}-1', freq = '1M'), rx1day[:-1]
             return rx1day
+    def Mann_Kendall_Test(self, type_data = None):
+        def sign(v):
+            if (v>0):
+                return 1
+            elif (v==0):
+                return 0
+            else:
+                return -1
+        def p_value(s):
+            if (s>0):
+                return (s-1)/np.std(np.array(self.dataframe.iloc[:,1]))  
+            elif (s==0):
+                return 0
+            else:
+                return (s+1)/np.std(np.array(self.dataframe.iloc[:, 1]))
+        if (type_data == "precipitation"):
+            s = 0
+            for i in range(self.len):
+                for j in range(i, self.len):
+                    s += sign(self.dataframe.iloc[j,1] - self.dataframe.iloc[i, 1])
+            return (s, p_value(s)) 
+        elif (type_data == "t_maxmin"):
+            smax = smin = 0
+            for i in range(self.len):
+                for j in range(self.len):
+                    smax += sign(self.dataframe.iloc[j,1] - self.dataframe.iloc[i, 1])
+                    smin += sign(self.dataframe.iloc[j,2] - self.dataframe.iloc[i, 2])
+            return (smax, p_value(smax)), (smin, p_value(smin))
+
+
```

### Comparing `AgenciBr-0.1.7/AgenciBr.egg-info/PKG-INFO` & `AgenciBr-0.1.8/AgenciBr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgenciBr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package to work with data from brazilian agenci
 Home-page: UNKNOWN
 Author: Thiago Santos
 Author-email: tthiagosantos38@gmail.com
 License: MIT License
 Keywords: Ana,Inemet,Ideam
 Platform: UNKNOWN
```

### Comparing `AgenciBr-0.1.7/LICENSE` & `AgenciBr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `AgenciBr-0.1.7/PKG-INFO` & `AgenciBr-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgenciBr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package to work with data from brazilian agenci
 Home-page: UNKNOWN
 Author: Thiago Santos
 Author-email: tthiagosantos38@gmail.com
 License: MIT License
 Keywords: Ana,Inemet,Ideam
 Platform: UNKNOWN
```

### Comparing `AgenciBr-0.1.7/README.md` & `AgenciBr-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `AgenciBr-0.1.7/setup.py` & `AgenciBr-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='AgenciBr',
-    version='0.1.7',
+    version='0.1.8',
     license='MIT License',
     author='Thiago Santos',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='tthiagosantos38@gmail.com',
     keywords='Ana, Inemet, Ideam',
     description=u'Package to work with data from brazilian agenci',
```

