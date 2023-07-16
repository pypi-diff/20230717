# Comparing `tmp/finqual-0.2.0.tar.gz` & `tmp/finqual-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-0.2.0.tar", last modified: Sun Jul  9 23:40:40 2023, max compression
+gzip compressed data, was "finqual-1.0.0.tar", last modified: Sun Jul 16 22:47:18 2023, max compression
```

## Comparing `finqual-0.2.0.tar` & `finqual-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 23:40:40.012618 finqual-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4966 2023-07-09 23:40:40.012618 finqual-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4444 2023-07-09 23:39:19.000000 finqual-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 23:40:39.992825 finqual-0.2.0/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.2.0/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 23:40:40.011617 finqual-0.2.0/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.2.0/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   120333 2023-07-09 21:10:07.000000 finqual-0.2.0/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-09 23:40:39.992825 finqual-0.2.0/finqual.egg-info/
--rw-rw-rw-   0        0        0     4966 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 23:40:40.012618 finqual-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-07-09 23:34:31.000000 finqual-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.369020 finqual-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4874 2023-07-16 22:47:18.369020 finqual-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4352 2023-07-16 22:41:03.000000 finqual-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.364015 finqual-1.0.0/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-1.0.0/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.368019 finqual-1.0.0/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-1.0.0/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   130768 2023-07-15 09:40:35.000000 finqual-1.0.0/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.367017 finqual-1.0.0/finqual.egg-info/
+-rw-rw-rw-   0        0        0     4874 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 22:47:18.369020 finqual-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-07-16 22:46:45.000000 finqual-1.0.0/setup.py
```

### Comparing `finqual-0.2.0/LICENSE.txt` & `finqual-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.2.0/PKG-INFO` & `finqual-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.2.0
+Version: 1.0.0
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,14 +17,15 @@
 ## Features
 
 finqual has the following features:
  
 - Ability to call the income statement, balance sheet or cash flow statement for any company on SEC's Electronic Data Gathering, Analysis, and Retrieval (EDGAR) system.
 - Retrieve comparables companies for a chosen ticker on varying industry classifications (e.g. more general industry classifications or more detailed classifications)
 - Breakdown of chosen financial ratios for a chosen ticker
+- Custom balance sheet for banks and other financial services firms
 
 This has two key features that enable better programmatic access compared to other providers:
 - Ability to call up to 10 requests per second, with built-in rate limiter
 - No restriction on the number of calls within a certain timeframe
 
 ## Quick-start guide
 
@@ -56,44 +57,43 @@
 ```
 
 From there, we use this initalised "Ticker" instance to call the desired function. These functions are:
 ```
 """
 Financial statement functions
 """
-fq.Ticker("TSLA").income(start, end, quarter = None)
+fq.Ticker("TSLA").income(start, end, quarter)
 
-fq.Ticker("TSLA").balance(start, end, quarter = None)
+fq.Ticker("TSLA").balance(start, end, quarter)
 
-fq.Ticker("TSLA").cashflow(start, end, quarter = None)
+fq.Ticker("TSLA").cashflow(start, end, quarter)
 
 """
 Other fundamental financial research functions
 """
 fq.Ticker("TSLA").ratios(start, end)
 
 fq.Ticker("TSLA").comparables(n, level = None)
 ```
 
-The financial statement functions (`income`, `balance` and `cashflow`) takes a mandatory timeframe input (`start` and `end`), and then an optional input to return the quarterly results within that timeframe, otherwise defaulting to returning annual results.
+The financial statement functions (`income`, `balance` and `cashflow`) takes a mandatory timeframe input `start` and `end`, and then an optional input to return the quarterly results within that timeframe by setting `quarter = True`, otherwise defaulting to returning annual results.
 
 The `ratios` function calculates selected financial ratios for the specified timeframe and returns the mean average over that timeframe. The selected financial ratios are a selection of liquidity, profitability and valuation ratios, which are commonly used to compare against other companies,
 
-The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible.
+The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible within the package.
 
 ## Dependencies
 
 Only four packages are required, with the following versions confirmed to be working:
 
-| Package   | Version  |
-|-----------|----------|
+| Package   | Version   |
+|-----------|-----------|
 | pandas    | >= 2.0.2  |
 | numpy     | >= 1.24.3 |
-| requests  | >= 2.31.0 |
+| requests  | >= 2.28.1 |
 | ratelimit | >= 2.2.1  |
 | datetime  | >= 5.1    |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database
-- Banks and financial institutions have different balance sheets compared to other normal companies, so a standardised balance sheet for banks and similar firms is still to be looked at
```

### Comparing `finqual-0.2.0/README.md` & `finqual-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ## Features
 
 finqual has the following features:
  
 - Ability to call the income statement, balance sheet or cash flow statement for any company on SEC's Electronic Data Gathering, Analysis, and Retrieval (EDGAR) system.
 - Retrieve comparables companies for a chosen ticker on varying industry classifications (e.g. more general industry classifications or more detailed classifications)
 - Breakdown of chosen financial ratios for a chosen ticker
+- Custom balance sheet for banks and other financial services firms
 
 This has two key features that enable better programmatic access compared to other providers:
 - Ability to call up to 10 requests per second, with built-in rate limiter
 - No restriction on the number of calls within a certain timeframe
 
 ## Quick-start guide
 
@@ -44,44 +45,43 @@
 ```
 
 From there, we use this initalised "Ticker" instance to call the desired function. These functions are:
 ```
 """
 Financial statement functions
 """
-fq.Ticker("TSLA").income(start, end, quarter = None)
+fq.Ticker("TSLA").income(start, end, quarter)
 
-fq.Ticker("TSLA").balance(start, end, quarter = None)
+fq.Ticker("TSLA").balance(start, end, quarter)
 
-fq.Ticker("TSLA").cashflow(start, end, quarter = None)
+fq.Ticker("TSLA").cashflow(start, end, quarter)
 
 """
 Other fundamental financial research functions
 """
 fq.Ticker("TSLA").ratios(start, end)
 
 fq.Ticker("TSLA").comparables(n, level = None)
 ```
 
-The financial statement functions (`income`, `balance` and `cashflow`) takes a mandatory timeframe input (`start` and `end`), and then an optional input to return the quarterly results within that timeframe, otherwise defaulting to returning annual results.
+The financial statement functions (`income`, `balance` and `cashflow`) takes a mandatory timeframe input `start` and `end`, and then an optional input to return the quarterly results within that timeframe by setting `quarter = True`, otherwise defaulting to returning annual results.
 
 The `ratios` function calculates selected financial ratios for the specified timeframe and returns the mean average over that timeframe. The selected financial ratios are a selection of liquidity, profitability and valuation ratios, which are commonly used to compare against other companies,
 
-The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible.
+The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible within the package.
 
 ## Dependencies
 
 Only four packages are required, with the following versions confirmed to be working:
 
-| Package   | Version  |
-|-----------|----------|
+| Package   | Version   |
+|-----------|-----------|
 | pandas    | >= 2.0.2  |
 | numpy     | >= 1.24.3 |
-| requests  | >= 2.31.0 |
+| requests  | >= 2.28.1 |
 | ratelimit | >= 2.2.1  |
 | datetime  | >= 5.1    |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database
-- Banks and financial institutions have different balance sheets compared to other normal companies, so a standardised balance sheet for banks and similar firms is still to be looked at
```

### Comparing `finqual-0.2.0/finqual/data/sec_sic.csv` & `finqual-1.0.0/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-0.2.0/finqual/finqual.py` & `finqual-1.0.0/finqual/finqual.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 class Ticker():
 
     def __init__(self, ticker):
         self.ticker = ticker
         self.cik = self.CIK()
         self.data = self.SEC()
-        #self.fiscal = self.fiscal_year()
+        self.SIC = self.SIC()
 
     def CIK(self):
         headers = {"Accept": "application/json, text/plain, */*", "Accept-Encoding": "gzip, deflate, br",
                    "Accept-Language": "en-US,en;q=0.9",
                    "Origin": "https://www.nasdaq.com",
                    "Referer": "https://www.nasdaq.com",
                    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"}
@@ -109,14 +109,25 @@
         else:  # start_month == end_month
             if start_day <= end_day:
                 return (start_month, start_day) <= (date_month, date_day) <= (end_month, end_day)
             else:  # Handle wraparound from end of year to start of year
                 return (start_month, start_day) <= (date_month, date_day) or (date_month, date_day) <= (
                     end_month, end_day)
 
+    def SIC(self):
+        this_dir, this_filename = os.path.split(__file__)
+        sic_path = os.path.join(this_dir, "data", "sec_sic.csv")
+
+        sic = pd.read_csv(sic_path, index_col=0)
+        sic = sic.dropna()
+
+        sic_code = sic[sic["ticker"] == self.ticker]["SIC"].values[0]
+
+        return sic_code
+
     def date_quarter(self, date, q1, q2, q3, q4):
         quarter_list = [(q1, 1), (q2, 2), (q3, 3), (q4, 4)]
         for quarter, quarter_num in quarter_list:
             if self.is_date_between(date, quarter):
                 return quarter_num
         return None
 
@@ -181,29 +192,44 @@
         item = node.name
         data = self.data
 
         if (category == "income"):
             """
             Creating search term
             """
-
             try:
                 df = pd.DataFrame(data["us-gaap"][item]["units"]["USD"])
                 df.dropna(inplace = True)
                 df["frame"] = df["frame"].str.replace('I', '')
 
                 if (quarter != None):
                     # If looking at quarter then:
                     search = "CY" + str(year) + "Q" + str(quarter)
                 else:
                     search = "CY" + str(year)
 
                 return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
 
             except:
+                pass
+
+            try:
+                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD/shares"])
+                df.dropna(inplace=True)
+                df["frame"] = df["frame"].str.replace('I', '')
+
+                if (quarter != None):
+                    # If looking at quarter then:
+                    search = "CY" + str(year) + "Q" + str(quarter)
+                else:
+                    search = "CY" + str(year)
+
+                return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
+
+            except:
                 return False
 
         if (category == "balance"):
 
             """
             Getting the desired item value
             """
@@ -335,33 +361,39 @@
         return values
 
     def income(self, start, end, category = "income", quarter = None, readable = None):
 
         df = self.income_helper(start, end, category, quarter, readable)
         df = df.drop(["Cost and Expenses", "Interest Expense", "Depreciation and Amortization"])
 
+        df = df.round(1).applymap('{:.1f}'.format).replace('\.0$', '', regex=True)
+
         return df
 
     def income_helper(self, start, end, category, quarter = None, readable = None):
         """
         Creating list of years and quarters for columns
         """
         year_list = [i for i in np.arange(end, start - 2, -1)]
         quarter_list = [str(i) + "Q" + str(j) for i in year_list for j in np.arange(4, 0, -1)]
+
         """
         Creating list of income statement items and their names
         """
         nodes = [rev, cor, gp, opex, ce,
                  oi,
-                 noi, pti, tax, ni, cce5_2,
-                 ide1_1]
+                 noi, pti, tax, ni,
+                 cce5_2,
+                 ide1_1,
+                 eps, eps_d]
         node_names = ["Revenues", "Cost of Revenue", "Gross Profit", "Operating Expenses", "Cost and Expenses",
                       "Operating Profit"
                      ,"Non-Operating Income/Expense", "Pretax Profit", "Tax", "Net Profit", "Depreciation and Amortization"
-                     ,"Interest Expense"]
+                     ,"Interest Expense"
+                     , "EPS", "Diluted EPS"]
         """
         Appending each node values for each year to a data
         """
         if quarter == True:
             data = [self.year_tree_item(i, start - 1, end, category, quarter) for i in nodes]
             df = pd.DataFrame(data, index = [node_names], columns = [quarter_list])
 
@@ -483,35 +515,60 @@
         """
         Creating list of years and quarters for columns
         """
         year_list = [i for i in np.arange(end, start - 1, -1)]
         quarter_list = [str(i) + "Q" + str(j) for i in year_list for j in np.arange(4, 0, -1)]
 
         """
-        Creating list of income statement items and their names
+        Getting SIC code
         """
 
-        nodes = [ca2_1, ca2_2, ca1_4, ca2_12, ca1_34, ca,
-                 nca1_13, nca1_19, nca1_36, nca,
-                 cl2_1, cl2_2, cl1_2, cl1_3, cl1_27, cl,
-                 ncl1_1, ncl1_2, ncl,
-                 se2_3, se2_8, se2_12, se2_14,
-                 se1_1, se1_2,
-                 a, l, se]
-
-        node_names = ["Cash and Cash Equivalents", "Short-term Investments", "Accounts Receivable, Net", "Inventories",
-                      "Other Current Assets", "Total Current Assets",
-                      "Property Plant and Equipment", "Intangibles", "Other Non-Current Assets",
-                      "Total Non-Current Assets",
-                      "Accounts Payable", "Accrued Liabilities", "Deferred Revenue", "Short-term Borrowings",
-                      "Other Current Liabilities", "Total Current Liabilities",
-                      "Long-Term Debt", "Non-Debt Long Term Liabilities", "Total Non-Current Liabilities",
-                      "Capital Stock", "Additional Paid In Capital", "Retained Earnings", "Accumulated Other Change",
-                      "Stockholder's Equity", "Minority Interest",
-                      "Total Assets", "Total Liabilities", "Total Equity"]
+        sic_code = self.SIC
+
+        bank_codes = [6022, 6021, 6211, 6029, 6035, 6199]
+
+        if sic_code in bank_codes:
+            nodes = [ca2_1, ba1_1, ba1_4,
+                     ba1_6, ba1_7, ba1_9, ba1_15, ba1_3, ba1_18,
+                     ba1_10, nca1_19, ba1_16, ba1_11, a,
+                     bl1_1, bl1_3, bl1_9,
+                     cl2_9, bl1_6,
+                     bl1_8, bl1_10, l,
+                     se2_3, se2_8, se2_12, se2_11,
+                     se1_1, se1_2, se]
+
+            node_names = ["Cash and Cash Equivalents", "Securities Purchased Under Agreements to Resell", "Net Loans",
+                          "Trading Securities", "Available-For-Sale Securities","Held-To-Maturity Securities", "Derivative Securities", "Securities Borrowed", "Financial Instruments Owned",
+                          "Property, Plant and Equipment", "Intangibles", "Accounts Receivables", "Other Assets", "Total Assets",
+                          "Securities Sold Under Agreements to Repurchase","Deposits", "Short Sales Obligations",
+                          "Short-Term Debt", "Long-Term Debt",
+                          "Accrued Expenses and Accounts Payable", "Other Liabilities", "Total Liabilities",
+                          "Common Stock", "Additional Paid In Capital", "Retained Earnings", "Accumulated Other Income",
+                          "Stockholder's Equity", "Minority Interest", "Total Equity"]
+
+
+        else:
+            nodes = [ca2_1, ca2_2, ca1_4, ca2_12, ca1_34, ca,
+                     nca1_13, nca1_19, nca1_36, nca,
+                     cl2_1, cl2_2, cl1_2, cl1_3, cl1_27, cl,
+                     ncl1_1, ncl1_2, ncl,
+                     se2_3, se2_8, se2_12, se2_14,
+                     se1_1, se1_2,
+                     a, l, se]
+
+            node_names = ["Cash and Cash Equivalents", "Short-term Investments", "Accounts Receivable, Net", "Inventories",
+                          "Other Current Assets", "Total Current Assets",
+                          "Property Plant and Equipment", "Intangibles", "Other Non-Current Assets",
+                          "Total Non-Current Assets",
+                          "Accounts Payable", "Accrued Liabilities", "Deferred Revenue", "Short-term Borrowings",
+                          "Other Current Liabilities", "Total Current Liabilities",
+                          "Long-Term Debt", "Non-Debt Long Term Liabilities", "Total Non-Current Liabilities",
+                          "Capital Stock", "Additional Paid In Capital", "Retained Earnings", "Accumulated Other Change",
+                          "Stockholder's Equity", "Minority Interest",
+                          "Total Assets", "Total Liabilities", "Total Equity"]
 
         """
         Appending each node values for each year to a data
         """
         if quarter == True:
             data = [self.year_tree_item(i, start, end, category = "balance", quarter=True) for i in nodes]  # Fetching the data
             df = pd.DataFrame(data, index=[node_names], columns=[quarter_list])  # Creating the dataframe with columns and index according to the list
@@ -522,38 +579,43 @@
 
         df.columns = df.columns.get_level_values(0)
         df.index = df.index.get_level_values(0)
 
         """
         Sense-checking
         """
-        df.loc["Total Non-Current Assets"] = df.loc["Total Assets"] - df.loc["Total Current Assets"]
-        df.loc["Other Current Assets"] = df.loc["Total Current Assets"] - df.iloc[0:4].sum()
-        df.loc["Other Non-Current Assets"] = df.loc["Total Non-Current Assets"] - df.iloc[6:7].sum()
-
-        df.loc["Other Current Liabilities"] = df.loc["Total Current Liabilities"] - df.iloc[11:15].sum()
-        df.loc["Total Non-Current Liabilities"] = df.loc["Total Liabilities"] - df.loc["Total Current Liabilities"]
-        df.loc["Non-Debt Long Term Liabilities"] = df.loc["Total Non-Current Liabilities"] - df.loc["Long-Term Debt"]
+        if sic_code not in bank_codes:
+            df.loc["Total Non-Current Assets"] = df.loc["Total Assets"] - df.loc["Total Current Assets"]
+            df.loc["Other Current Assets"] = df.loc["Total Current Assets"] - df.iloc[0:4].sum()
+            df.loc["Other Non-Current Assets"] = df.loc["Total Non-Current Assets"] - df.iloc[6:7].sum()
+
+            df.loc["Other Current Liabilities"] = df.loc["Total Current Liabilities"] - df.iloc[11:15].sum()
+            df.loc["Total Non-Current Liabilities"] = df.loc["Total Liabilities"] - df.loc["Total Current Liabilities"]
+            df.loc["Non-Debt Long Term Liabilities"] = df.loc["Total Non-Current Liabilities"] - df.loc["Long-Term Debt"]
+
+            df.loc["Accumulated Other Change"] = df.loc["Stockholder's Equity"] - df.iloc[19:22].sum()
+            df.loc["Minority Interest"] = df.loc["Total Equity"] - df.loc["Stockholder's Equity"]
+
+        else:
 
-        df.loc["Accumulated Other Change"] = df.loc["Stockholder's Equity"] - df.iloc[19:22].sum()
-        df.loc["Minority Interest"] = df.loc["Total Equity"] - df.loc["Stockholder's Equity"]
+            df.loc["Other Assets"] = df.loc["Total Assets"] - df.iloc[0:12].sum()
+            df.loc["Other Liabilities"] = df.loc["Total Liabilities"] - df.iloc[14:20].sum()
 
         if readable == True:
 
             df = df.applymap(lambda x: '{:,}'.format(x))
             df = df.loc[:, (df != 0).any(axis=0)]
             return df
 
         else:
 
             df = df.loc[:, (df != 0).any(axis=0)]
             return df
 
     def comparables(self, n, level = None):
-
         this_dir, this_filename = os.path.split(__file__)
         sic_path = os.path.join(this_dir, "data", "sec_sic.csv")
 
         if level == None:
             level = 4
 
         sic = pd.read_csv(sic_path, index_col=0)
@@ -592,17 +654,19 @@
         surronding_companies = surronding_companies.rename(columns={'ticker': 'Ticker', 'title': 'Name'})
 
         return surronding_companies
 
     def ratios(self, start, end):
 
         df = self.data
+        sic_code = self.SIC
+        bank_codes = [6022, 6021, 6211, 6029, 6035, 6199]
 
         balance_r = self.balance(start - 1, end)
-        income_r = self.income(start, end)
+        income_r = self.income(start, end).astype(float)
         cash_r = self.cashflow(start, end)
 
         year_list = [i for i in np.arange(end, start - 1, -1)]
 
         cap_df = pd.DataFrame(df["dei"]["EntityPublicFloat"]["units"]["USD"])
         cap_df["fy"] = cap_df["frame"].str[2:6]
 
@@ -617,74 +681,227 @@
 
         ebitda = income_r.loc["EBITDA"]
         ebit = income_r.loc["EBIT"]
         net_profit = income_r.loc["Net Profit"]
         operating_profit = income_r.loc["Operating Profit"]
         tax = income_r.loc["Tax"]
 
-        current_assets = balance_r.loc["Total Current Assets"]
-        total_assets = balance_r.loc["Total Assets"]
-        current_liabilities = balance_r.loc["Total Current Liabilities"]
-        total_liabilities = balance_r.loc["Total Liabilities"]
-        total_se = balance_r.loc["Stockholder's Equity"]
-        total_equity = balance_r.loc["Total Equity"]
-        inventory = balance_r.loc["Inventories"]
-        cash = balance_r.loc["Cash and Cash Equivalents"]
+        if sic_code in bank_codes:
+            total_assets = balance_r.loc["Total Assets"]
+            total_liabilities = balance_r.loc["Total Liabilities"]
+            total_se = balance_r.loc["Stockholder's Equity"]
+            total_equity = balance_r.loc["Total Equity"]
+            cash = balance_r.loc["Cash and Cash Equivalents"]
 
-        fcf = cash_r.loc["Free Cash Flow"]
+        else:
+            current_assets = balance_r.loc["Total Current Assets"]
+            total_assets = balance_r.loc["Total Assets"]
+            current_liabilities = balance_r.loc["Total Current Liabilities"]
+            total_liabilities = balance_r.loc["Total Liabilities"]
+            total_se = balance_r.loc["Stockholder's Equity"]
+            total_equity = balance_r.loc["Total Equity"]
+            inventory = balance_r.loc["Inventories"]
+            cash = balance_r.loc["Cash and Cash Equivalents"]
+            nwc = (current_assets - current_liabilities).diff(-1)
 
-        nwc = (current_assets - current_liabilities).diff(-1)
+        fcf = cash_r.loc["Free Cash Flow"]
 
         d_a = pd.Series(self.year_tree_item(cce5_2, start, end, "income"), index=year_list)
         capex = pd.Series(self.year_tree_item(cce4_8, start, end, "cashflow"), index=year_list)
-        ufcf = operating_profit + tax - capex + d_a - nwc
+
+        if sic_code in bank_codes:
+            ufcf = operating_profit + tax - capex + d_a
+        else:
+            ufcf = operating_profit + tax - capex + d_a - nwc
 
         cap = cap + total_liabilities - cash
 
         ratio_df = pd.DataFrame(columns=year_list)
 
-        ratio_df.loc["Current Ratio"] = (current_assets / current_liabilities)
-        ratio_df.loc["Quick Ratio"] = ((current_assets - inventory) / current_liabilities)
+        if sic_code in bank_codes:
+            ratio_df.loc["Debt-to-Equity Ratio"] = (total_liabilities / total_se)
 
-        ratio_df.loc["Debt-to-Equity Ratio"] = (total_liabilities / total_se)
+            ratio_df.loc["Return on Equity"] = (net_profit / total_se)
+            ratio_df.loc["Return on Assets"] = (net_profit / total_assets)
+            ratio_df.loc["Return on Invested Capital"] = (operating_profit + tax) / (total_liabilities + total_equity)
 
-        ratio_df.loc["Return on Equity"] = (net_profit / total_se)
-        ratio_df.loc["Return on Assets"] = (net_profit / total_assets)
-        ratio_df.loc["Return on Capital Employed"] = ebit / (total_assets - current_liabilities)
-        ratio_df.loc["Return on Invested Capital"] = (operating_profit + tax) / (total_liabilities + total_equity)
+            ratio_df.loc["FCFF Yield"] = ufcf / (cap)
 
-        ratio_df.loc["FCFF Yield"] = ufcf / (cap)
+            ratio_df.loc["EV/EBITDA"] = (cap / ebitda)
 
-        ratio_df.loc["EV/EBITDA"] = (cap / ebitda)
+        else:
+            ratio_df.loc["Current Ratio"] = (current_assets / current_liabilities)
+            ratio_df.loc["Quick Ratio"] = ((current_assets - inventory) / current_liabilities)
+
+            ratio_df.loc["Debt-to-Equity Ratio"] = (total_liabilities / total_se)
+
+            ratio_df.loc["Return on Equity"] = (net_profit / total_se)
+            ratio_df.loc["Return on Assets"] = (net_profit / total_assets)
+            ratio_df.loc["Return on Capital Employed"] = ebit / (total_assets - current_liabilities)
+            ratio_df.loc["Return on Invested Capital"] = (operating_profit + tax) / (total_liabilities + total_equity)
+
+            ratio_df.loc["FCFF Yield"] = ufcf / (cap)
+
+            ratio_df.loc["EV/EBITDA"] = (cap / ebitda)
 
         ratio_df.dropna(axis=1, how='all', inplace=True)
 
         ratio_df["Mean"] = ratio_df.mean(axis=1)
 
         return ratio_df
 
 """
+Banks and financial services balance sheet items
+"""
+
+#ca3_1 # Cash due from banks
+#ca3_2 # Deposits from other banks
+
+"""
+Banks - Assets
+"""
+
+#Level 1
+ba1_1 = Node("FederalFundsSoldAndSecuritiesPurchasedUnderAgreementsToResell", attribute = "debit") #Securities Purchased Under Agreements to Resell
+ba1_12 = Node("CarryingValueOfFederalFundsSoldSecuritiesPurchasedUnderAgreementsToResellAndDepositsPaidForSecuritiesBorrowed", attribute = "debit", parent = ba1_1)
+ba1_13 = Node("CarryingValueOfSecuritiesPurchasedUnderAgreementsToResellAndDepositsPaidForSecuritiesBorrowed", attribute = "debit", parent = ba1_12)
+
+
+
+ba1_4 = Node("NotesReceivableNet", attribute = "debit") #Loans and Leases, Net
+ba1_5 = Node("FinancingReceivableExcludingAccruedInterestAfterAllowanceForCreditLoss", attribute = "debit", parent = ba1_4) #Loans and Leases
+
+ba1_3 = Node("SecuritiesBorrowed", attribute = "debit") # Securities Borrowed
+
+ba1_14 = Node("MarketableSecurities", attribute = "debit") #Marketable Securities
+
+ba1_6 = Node("TradingSecurities", attribute = "debit", parent = ba1_14) #Trading Securities
+
+ba1_15 = Node("DerivativeAssets", attribute = "debit", parent = ba1_14) #Derivative Assets
+
+ba1_7 = Node("AvailableForSaleSecuritiesDebtSecurities", attribute = "debit", parent = ba1_14) #Available-For-Sale Securities
+ba1_8 = Node("DebtSecuritiesAvailableForSaleExcludingAccruedInterest", attribute = "debit", parent = ba1_7) #Available-For-Sale Securities
+
+ba1_9 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestAfterAllowanceForCreditLoss", attribute = "debit", parent = ba1_14) #Held-To-Maturity Securities
+ba1_17 = Node("DebtSecuritiesHeldToMaturityAmortizedCostAfterAllowanceForCreditLoss", attribute = "debit", parent = ba1_9)
+
+ba1_10 = Node("PropertyPlantAndEquipmentAndFinanceLeaseRightOfUseAssetAfterAccumulatedDepreciationAndAmortization", attribute = "debit") #Premises and Equipment
+
+ba1_11 = Node("OtherAssets", attribute = "debit")
+
+ba1_16 = Node("AccountsReceivableNet", attribute = "debit") # Accounts Receivables
+
+ba1_18 = Node("FinancialInstrumentsOwnedAtFairValue", attribute = "debit") #Financial Instruments Owned
+
+#Level 2
+ba2_1 = Node("FederalFundsSold", attribute = "debit", parent = ba1_13)
+ba2_2 = Node("SecuritiesPurchasedUnderAgreementsToResell", attribute = "debit", parent = ba1_13)
+
+ba2_3 = Node("FinancingReceivableAllowanceForCreditLossExcludingAccruedInterest", attribute = "credit", parent = ba1_5)
+ba2_4 = Node("FinancingReceivableAllowanceForCreditLosses", attribute = "credit", parent = ba2_3)
+
+ba2_5 = Node("FinancingReceivableExcludingAccruedInterestBeforeAllowanceForCreditLoss", attribute = "debit", parent = ba1_5)
+ba2_6 = Node("NotesReceivableGross", attribute = "debit", parent = ba2_5) # Gross loans
+
+ba2_7 = Node("TradingSecuritiesDebt", attribute = "debit", parent = ba1_6)
+ba2_8 = Node("EquitySecuritiesFvNiCurrentAndNoncurrent", attribute = "debit", parent = ba1_6)
+
+ba2_9 = Node("DebtSecuritiesHeldToMaturityAllowanceForCreditLossExcludingAccruedInterest", attribute = "credit", parent = ba1_17)
+ba2_22 = Node("DebtSecuritiesHeldToMaturityAllowanceForCreditLoss", attribute = "credit", parent = ba2_9)
+ba2_10 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestBeforeAllowanceForCreditLoss", attribute = "debit", parent = ba1_17)
+ba2_21 = Node("HeldToMaturitySecurities", attribute = "debit", parent = ba2_10)
+
+ba2_11 = Node("FinanceLeaseRightOfUseAsset", attribute = "credit", parent = ba1_10)
+ba2_12 = Node("PropertyPlantAndEquipmentNet", attribute = "debit", parent = ba1_10)
+
+ba2_13 = Node("ReceivablesFromCustomers", attribute = "debit", parent = ba1_16)
+ba2_20 = Node("ContractWithCustomerReceivableAfterAllowanceForCreditLossCurrent", attribute = "debit", parent = ba2_13)
+ba2_14 = Node("ReceivablesFromBrokersDealersAndClearingOrganizations", attribute = "debit", parent = ba1_16)
+ba2_15 = Node("AccountsReceivableFromSecuritization", attribute = "debit", parent = ba1_16)
+ba2_16 = Node("AccountsReceivableBilledForLongTermContractsOrPrograms", attribute = "debit", parent = ba1_16)
+ba2_17 = Node("NotesReceivableGross", attribute = "debit", parent = ba1_16)
+ba2_18 = Node("AccruedInvestmentIncomeReceivable", attribute = "debit", parent = ba1_16)
+ba2_19 = Node("PremiumsReceivableAtCarryingValue", attribute = "debit", parent = ba1_16)
+ba2_20 = Node("OtherReceivables", attribute = "debit", parent = ba1_16)
+
+"""
+Banks - Liabilities
+"""
+#Level 1
+bl1_1 = Node("FederalFundsPurchasedAndSecuritiesSoldUnderAgreementsToRepurchase", attribute = "credit") #Securities Loaned
+bl1_2 = Node("CarryingValueOfSecuritiesSoldUnderRepurchaseAgreementsAndDepositsReceivedForSecuritiesLoaned", attribute = "credit", parent = bl1_1)
+
+bl1_3 = Node("Deposits", attribute = "credit") #Total Deposits
+
+bl1_4 = Node("TradingLiabilities", attribute = "credit") #Trading Liabilities
+
+bl1_5 = Node("ShortTermBorrowings", attribute = "credit") #Short-Term Debt
+
+bl1_6 = Node("LongTermDebtAndCapitalLeaseObligationsIncludingCurrentMaturities", attribute = "credit") #Long-Term Debt
+
+bl1_8 = Node("AccountsPayableAndAccruedLiabilitiesCurrentAndNoncurrent", attribute = "credit") # Accounts Payable and Accrued Liabilities
+
+bl1_9 = Node("FinancialInstrumentsSoldNotYetPurchasedAtFairValue", attribute = "credit") # Short-sales
+
+bl1_10 = Node("Other", attribute = "credit")
+
+#Level 2
+bl2_1 = Node("FederalFundsPurchased", attribute = "credit", parent = bl1_2)
+bl2_2 = Node("SecuritiesSoldUnderAgreementsToRepurchase", attribute = "credit", parent = bl1_2)
+
+bl2_3 = Node("LongTermDebt", attribute = "credit", parent = bl1_6)
+
+bl2_4 = Node("AccountsPayableCurrentAndNoncurrent", attribute = "credit", parent = bl1_8)
+bl2_5 = Node("AccruedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl1_8)
+
+
+#Level 3
+
+bl3_1 = Node("AccruedLiabilitiesAndOtherLiabilities", attribute = "credit", parent = bl2_5)
+bl3_2 = Node("EmployeeRelatedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl2_5)
+bl3_3 = Node("OtherAccruedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl2_5)
+
+bl3_4 = Node("PayablesToCustomers", attribute = "credit", parent = bl2_4)
+bl3_5 = Node("AccountsPayableTradeCurrentAndNoncurrent", attribute = "credit", parent = bl2_4)
+bl3_6 = Node("AccountsPayableInterestBearingCurrentAndNoncurrent", attribute = "credit", parent = bl2_4)
+
+#Level 4
+
+bl4_1 = Node("AccruedEmployeeBenefitsCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
+bl4_2 = Node("AccruedSalariesCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
+bl4_3 = Node("WorkersCompensationLiabilityCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
+bl4_4 = Node("OtherEmployeeRelatedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
+
+
+
+
+"""
+EPS
+"""
+
+eps = Node("EarningsPerShareBasic", attribute = "credit")
+eps_d = Node("EarningsPerShareDiluted", attribute = "credit")
+
+"""
 Net Income
 """
+
 ni = Node("NetIncomeLoss", attribute="credit")
 
 # Level 1
 ni1_1 = Node("ProfitLoss", attribute="credit", parent=ni)
 
 """
 Pre-tax income
 """
-pti = Node("IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest",
-           attribute="credit", parent=ni)
+pti = Node("IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest", attribute="credit", parent=ni)
 
 # Level 1
 
-pti1_1 = Node(
-    "IncomeLossFromContinuingOperationsBeforeIncomeTaxesMinorityInterestAndIncomeLossFromEquityMethodInvestments",
-    attribute="credit", parent=pti)
+pti1_1 = Node("IncomeLossFromContinuingOperationsBeforeIncomeTaxesMinorityInterestAndIncomeLossFromEquityMethodInvestments", attribute="credit", parent=pti)
 
 """
 Tax
 """
 tax = Node("IncomeTaxExpenseBenefit", attribute="debit", parent=ni)
 
 """
@@ -858,16 +1075,15 @@
 opex2_32 = Node("OrderFlowFees", attribute="debit", parent=opex1_11)
 opex2_33 = Node("ClearanceFees", attribute="debit", parent=opex1_11)
 
 # Level 3
 
 opex3_1 = Node("ResearchAndDevelopmentExpenseExcludingAcquiredInProcessCost", attribute="debit", parent=opex2_1)
 opex3_2 = Node("ResearchAndDevelopmentExpenseSoftwareExcludingAcquiredInProcessCost", attribute="debit", parent=opex2_1)
-opex3_3 = Node("ResearchAndDevelopmentAssetAcquiredOtherThanThroughBusinessCombinationWrittenOff", attribute="debit",
-               parent=opex2_1)
+opex3_3 = Node("ResearchAndDevelopmentAssetAcquiredOtherThanThroughBusinessCombinationWrittenOff", attribute="debit", parent=opex2_1)
 
 opex3_4 = Node("DepreciationNonproduction", attribute="debit", parent=opex2_2)
 opex3_5 = Node("DepletionOfOilAndGasProperties", attribute="debit", parent=opex2_2)
 opex3_6 = Node("AmortizationOfDeferredCharges", attribute="debit", parent=opex2_2)
 opex3_7 = Node("OtherDepreciationAndAmortization", attribute="debit", parent=opex2_2)
 
 opex3_8 = Node("RestructuringCharges", attribute="debit", parent=opex2_6)
@@ -923,16 +1139,15 @@
 opex4_5 = Node("FinanceLeaseRightOfUseAssetAmortization", attribute="debit", parent=opex3_6)
 opex4_6 = Node("AmortizationOfPowerContractsEmissionCredits", attribute="debit", parent=opex3_6)
 opex4_7 = Node("AmortizationOfNuclearFuelLease", attribute="debit", parent=opex3_6)
 opex4_8 = Node("AmortizationOfAdvanceRoyalty", attribute="debit", parent=opex3_6)
 opex4_9 = Node("AmortizationOfDeferredPropertyTaxes", attribute="debit", parent=opex3_6)
 opex4_10 = Node("AmortizationOfRateDeferral", attribute="debit", parent=opex3_6)
 opex4_11 = Node("AmortizationOfDeferredHedgeGains", attribute="debit", parent=opex3_6)
-opex4_12 = Node("AmortizationAndDepreciationOfDecontaminatingAndDecommissioningAssets", attribute="debit",
-                parent=opex3_6)
+opex4_12 = Node("AmortizationAndDepreciationOfDecontaminatingAndDecommissioningAssets", attribute="debit", parent=opex3_6)
 opex4_13 = Node("OtherAmortizationOfDeferredCharges", attribute="debit", parent=opex3_6)
 
 opex4_14 = Node("BusinessExitCosts1", attribute="debit", parent=opex3_8)
 opex4_15 = Node("SeveranceCosts1", attribute="debit", parent=opex3_8)
 opex4_16 = Node("OtherRestructuringCosts", attribute="debit", parent=opex3_8)
 
 opex4_17 = Node("GoodwillAndIntangibleAssetImpairment", attribute="debit", parent=opex3_14)
@@ -984,18 +1199,16 @@
 noi1_10 = Node("GainsLossesOnSalesOfOtherRealEstate", attribute="credit", parent=noi)
 noi1_11 = Node("BankOwnedLifeInsuranceIncome", attribute="credit", parent=noi)
 noi1_12 = Node("RealEstateInvestmentPartnershipRevenue", attribute="credit", parent=noi)
 noi1_13 = Node("ConversionGainsAndLossesOnForeignInvestments", attribute="credit", parent=noi)
 noi1_14 = Node("ProfitLossFromRealEstateOperations", attribute="credit", parent=noi)
 noi1_15 = Node("MortgageServicingRightsMSRImpairmentRecovery", attribute="credit", parent=noi)
 noi1_16 = Node("DebtInstrumentConvertibleBeneficialConversionFeature", attribute="credit", parent=noi)
-noi1_17 = Node("PublicUtilitiesAllowanceForFundsUsedDuringConstructionCapitalizedCostOfEquity", attribute="credit",
-               parent=noi)
-noi1_18 = Node("NetPeriodicDefinedBenefitsExpenseReversalOfExpenseExcludingServiceCostComponent", attribute="debit",
-               parent=noi)
+noi1_17 = Node("PublicUtilitiesAllowanceForFundsUsedDuringConstructionCapitalizedCostOfEquity", attribute="credit", parent=noi)
+noi1_18 = Node("NetPeriodicDefinedBenefitsExpenseReversalOfExpenseExcludingServiceCostComponent", attribute="debit", parent=noi)
 noi1_19 = Node("OtherNonoperatingIncomeExpense", attribute="credit", parent=noi)
 noi1_20 = Node("UnusualOrInfrequentItemNetGainLoss", attribute="debit", parent=noi)
 
 # Level 2
 
 noi2_1 = Node("NonoperatingGainsLosses", attribute="credit", parent=noi1_1)
 noi2_2 = Node("RoyaltyIncomeNonoperating", attribute="credit", parent=noi1_1)
@@ -1007,37 +1220,34 @@
 
 noi2_8 = Node("ForeignCurrencyTransactionGainLossRealized", attribute="credit", parent=noi1_6)
 noi2_9 = Node("ForeignCurrencyTransactionGainLossUnrealized", attribute="credit", parent=noi1_6)
 
 noi2_10 = Node("OtherNonoperatingIncome", attribute="credit", parent=noi1_19)
 noi2_11 = Node("OtherNonoperatingExpense", attribute="debit", parent=noi1_19)
 
-noi2_12 = Node("DiscontinuedApplicationOfSpecializedAccountingForRegulatedOperations", attribute="credit",
-               parent=noi1_20)
+noi2_12 = Node("DiscontinuedApplicationOfSpecializedAccountingForRegulatedOperations", attribute="credit", parent=noi1_20)
 noi2_13 = Node("UnusualOrInfrequentItemGainGross", attribute="credit", parent=noi1_20)
 noi2_14 = Node("UnusualOrInfrequentItemNetOfInsuranceProceeds", attribute="debit", parent=noi1_20)
 
 # Level 3
 
 noi3_1 = Node("GainLossOnInvestments", attribute="credit", parent=noi2_1)
 noi3_2 = Node("VentureCapitalGainsLossesNet", attribute="credit", parent=noi2_1)
 noi3_3 = Node("DisposalGroupNotDiscontinuedOperationGainLossOnDisposal", attribute="credit", parent=noi2_1)
 noi3_4 = Node("GainLossOnSaleOfStockInSubsidiaryOrEquityMethodInvestee", attribute="credit", parent=noi2_1)
 noi3_5 = Node("DeconsolidationGainOrLossAmount", attribute="credit", parent=noi2_1)
-noi3_6 = Node("GainLossOnSaleOfPreviouslyUnissuedStockBySubsidiaryOrEquityInvesteeNonoperatingIncome",
-              attribute="credit", parent=noi2_1)
+noi3_6 = Node("GainLossOnSaleOfPreviouslyUnissuedStockBySubsidiaryOrEquityInvesteeNonoperatingIncome", attribute="credit", parent=noi2_1)
 noi3_7 = Node("GainLossOnSaleOfInterestInProjects", attribute="credit", parent=noi2_1)
 noi3_8 = Node("GainLossOnDerivativeInstrumentsNetPretax", attribute="credit", parent=noi2_1)
 noi3_9 = Node("BusinessCombinationBargainPurchaseGainRecognizedAmount", attribute="credit", parent=noi2_1)
 noi3_10 = Node("OtherNonoperatingGainsLosses", attribute="credit", parent=noi2_1)
 
 noi3_11 = Node("LeveragedLeasesIncomeStatementIncomeFromLeveragedLeases", attribute="credit", parent=noi2_6)
 noi3_12 = Node("LeveragedLeasesIncomeStatementIncomeTaxExpenseOnLeveragedLeases", attribute="debit", parent=noi2_6)
-noi3_13 = Node("LeveragedLeasesIncomeStatementInvestmentTaxCreditRecognizedOnLeveragedLeases", attribute="credit",
-               parent=noi2_6)
+noi3_13 = Node("LeveragedLeasesIncomeStatementInvestmentTaxCreditRecognizedOnLeveragedLeases", attribute="credit", parent=noi2_6)
 
 noi3_14 = Node("InvestmentIncomeInterestAndDividend", attribute="credit", parent=noi2_6)
 noi3_15 = Node("InvestmentIncomeNetAmortizationOfDiscountAndPremium", attribute="credit", parent=noi2_6)
 noi3_16 = Node("InvestmentIncomeInvestmentExpense", attribute="debit", parent=noi2_6)
 
 noi3_17 = Node("OtherNonoperatingAssetRelatedIncome", attribute="credit", parent=noi2_10)
 
@@ -1060,16 +1270,15 @@
 noi4_9 = Node("InvestmentIncomeDividend", attribute="credit", parent=noi3_14)
 
 noi4_10 = Node("InvestmentIncomeAmortizationOfDiscount", attribute="credit", parent=noi3_15)
 noi4_11 = Node("InvestmentIncomeAmortizationOfPremium", attribute="credit", parent=noi3_15)
 
 # Level 5
 
-noi5_1 = Node("GainLossOnInterestRateDerivativeInstrumentsNotDesignatedAsHedgingInstruments", attribute="credit",
-              parent=noi4_7)
+noi5_1 = Node("GainLossOnInterestRateDerivativeInstrumentsNotDesignatedAsHedgingInstruments", attribute="credit", parent=noi4_7)
 noi5_2 = Node("GainLossOnDerivativeInstrumentsHeldForTradingPurposesNet", attribute="credit", parent=noi4_7)
 
 noi5_3 = Node("InterestIncomeRelatedParty", attribute="credit", parent=noi4_8)
 
 """
 Costs and Expenses
 """
@@ -1107,16 +1316,15 @@
 ide2_3 = Node("DebtRelatedCommitmentFeesAndDebtIssuanceCosts", attribute="debit", parent=ide1_1)
 ide2_4 = Node("FinanceLeaseInterestExpense", attribute="debit", parent=ide1_1)
 ide2_5 = Node("InterestExpenseRelatedParty", attribute="debit", parent=ide1_1)
 ide2_6 = Node("InterestExpenseOther", attribute="debit", parent=ide1_1)
 ide2_7 = Node("InterestExpenseDeposits", attribute="debit", parent=ide1_1)
 ide2_8 = Node("InterestExpenseTradingLiabilities", attribute="debit", parent=ide1_1)
 ide2_9 = Node("InterestExpenseBorrowings", attribute="debit", parent=ide1_1)
-ide2_10 = Node("InterestExpenseBeneficialInterestsIssuedByConsolidatedVariableInterestEntities", attribute="debit",
-               parent=ide1_1)
+ide2_10 = Node("InterestExpenseBeneficialInterestsIssuedByConsolidatedVariableInterestEntities", attribute="debit", parent=ide1_1)
 ide2_11 = Node("InterestExpenseTrustPreferredSecurities", attribute="debit", parent=ide1_1)
 
 ide2_10 = Node("GainsLossesOnExtinguishmentOfDebtBeforeWriteOffOfDeferredDebtIssuanceCost", attribute="credit",
                parent=ide1_2)
 ide2_11 = Node("WriteOffOfDeferredDebtIssuanceCost", attribute="debit", parent=ide1_2)
 
 # Level 3
@@ -1128,18 +1336,16 @@
 
 # Level 4
 ide4_1 = Node("InterestExpenseNOWAccountsMoneyMarketAccountsAndSavingsDeposits", attribute="debit", parent=ide3_1)
 ide4_2 = Node("InterestExpenseDemandDepositAccounts", attribute="debit", parent=ide3_1)
 ide4_3 = Node("InterestExpenseTimeDeposits", attribute="debit", parent=ide3_1)
 ide4_4 = Node("InterestExpenseOtherDomesticDeposits", attribute="debit", parent=ide3_1)
 
-ide4_5 = Node("InterestExpenseFederalFundsPurchasedAndSecuritiesSoldUnderAgreementsToRepurchase", attribute="debit",
-              parent=ide3_3)
-ide4_6 = Node("InterestExpenseShortTermBorrowingsExcludingFederalFundsAndSecuritiesSoldUnderAgreementsToRepurchase",
-              attribute="debit", parent=ide3_3)
+ide4_5 = Node("InterestExpenseFederalFundsPurchasedAndSecuritiesSoldUnderAgreementsToRepurchase", attribute="debit", parent=ide3_3)
+ide4_6 = Node("InterestExpenseShortTermBorrowingsExcludingFederalFundsAndSecuritiesSoldUnderAgreementsToRepurchase", attribute="debit", parent=ide3_3)
 
 ide4_7 = Node("InterestExpenseLongTermDebt", attribute="debit", parent=ide3_4)
 ide4_8 = Node("InterestExpenseCapitalSecurities", attribute="debit", parent=ide3_4)
 
 # Level 5
 
 ide5_1 = Node("InterestExpenseNegotiableOrderOfWithdrawalNOWDeposits", attribute="debit", parent=ide4_1)
@@ -1148,16 +1354,15 @@
 
 ide5_4 = Node("InterestExpenseTimeDepositsLessThan100000", attribute="debit", parent=ide4_3)
 ide5_5 = Node("InterestExpenseTimeDeposits100000OrMore", attribute="debit", parent=ide4_3)
 
 ide5_6 = Node("InterestExpenseFederalFundsPurchased", attribute="debit", parent=ide4_5)
 ide5_7 = Node("InterestExpenseSecuritiesSoldUnderAgreementsToRepurchase", attribute="debit", parent=ide4_5)
 
-ide5_8 = Node("InterestExpenseFederalHomeLoanBankAndFederalReserveBankAdvancesShortTerm", attribute="debit",
-              parent=ide4_6)
+ide5_8 = Node("InterestExpenseFederalHomeLoanBankAndFederalReserveBankAdvancesShortTerm", attribute="debit", parent=ide4_6)
 ide5_9 = Node("InterestExpenseCommercialPaper", attribute="debit", parent=ide4_6)
 ide5_10 = Node("InterestExpenseOtherShortTermBorrowings", attribute="debit", parent=ide4_6)
 
 ide5_11 = Node("InterestExpenseSubordinatedNotesAndDebentures", attribute="debit", parent=ide4_7)
 ide5_12 = Node("InterestExpenseJuniorSubordinatedDebentures", attribute="debit", parent=ide4_7)
 ide5_13 = Node("InterestExpenseMediumTermNotes", attribute="debit", parent=ide4_7)
 ide5_14 = Node("InterestExpenseFederalHomeLoanBankAndFederalReserveBankAdvancesLongTerm", attribute="debit",
@@ -1199,29 +1404,22 @@
 ca1_13 = Node("DeferredRentAssetNetCurrent", attribute="debit", parent=ca)
 ca1_14 = Node("AssetsHeldInTrustCurrent", attribute="debit", parent=ca)
 ca1_15 = Node("AdvancesOnInventoryPurchases", attribute="debit", parent=ca)
 ca1_16 = Node("FinancingReceivableAccruedInterestAfterAllowanceForCreditLoss", attribute="debit", parent=ca)
 ca1_17 = Node("AccountsReceivableNoncurrentAccruedInterestAfterAllowanceForCreditLoss", attribute="debit", parent=ca)
 ca1_18 = Node("DebtSecuritiesHeldToMaturityAccruedInterestAfterAllowanceForCreditLoss", attribute="debit", parent=ca)
 ca1_19 = Node("NetInvestmentInLeaseAccruedInterestAfterAllowanceForCreditLoss", attribute="debit", parent=ca)
-ca1_20 = Node("SalesTypeLeaseNetInvestmentInLeaseAccruedInterestAfterAllowanceForCreditLoss", attribute="debit",
-              parent=ca)
-ca1_21 = Node("DirectFinancingLeaseNetInvestmentInLeaseAccruedInterestAfterAllowanceForCreditLoss", attribute="debit",
-              parent=ca)
+ca1_20 = Node("SalesTypeLeaseNetInvestmentInLeaseAccruedInterestAfterAllowanceForCreditLoss", attribute="debit", parent=ca)
+ca1_21 = Node("DirectFinancingLeaseNetInvestmentInLeaseAccruedInterestAfterAllowanceForCreditLoss", attribute="debit", parent=ca)
 ca1_22 = Node("FinancialAssetAmortizedCostAccruedInterestAfterAllowanceForCreditLoss", attribute="debit", parent=ca)
-ca1_23 = Node("DebtSecuritiesAvailableForSaleAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit",
-              parent=ca)
-ca1_24 = Node("FinancingReceivableExcludingAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit",
-              parent=ca)
-ca1_25 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestAfterAllowanceForCreditLossCurrent",
-              attribute="debit", parent=ca)
-ca1_26 = Node("NetInvestmentInLeaseExcludingAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit",
-              parent=ca)
-ca1_27 = Node("DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestAfterAllowanceForCreditLossCurrent",
-              attribute="debit", parent=ca)
+ca1_23 = Node("DebtSecuritiesAvailableForSaleAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit", parent=ca)
+ca1_24 = Node("FinancingReceivableExcludingAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit", parent=ca)
+ca1_25 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit", parent=ca)
+ca1_26 = Node("NetInvestmentInLeaseExcludingAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit", parent=ca)
+ca1_27 = Node("DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestAfterAllowanceForCreditLossCurrent", attribute="debit", parent=ca)
 ca1_28 = Node("AdvanceRoyaltiesCurrent", attribute="debit", parent=ca)
 ca1_29 = Node("AssetsOfDisposalGroupIncludingDiscontinuedOperationCurrent", attribute="debit", parent=ca)
 ca1_30 = Node("AssetsHeldForSaleNotPartOfDisposalGroupCurrent", attribute="debit", parent=ca)
 ca1_31 = Node("DepositsAssetsCurrent", attribute="debit", parent=ca)
 ca1_32 = Node("IntangibleAssetsCurrent", attribute="debit", parent=ca)
 ca1_33 = Node("BusinessCombinationContingentConsiderationAssetCurrent", attribute="debit", parent=ca)
 ca1_34 = Node("OtherAssetsCurrent", attribute="debit", parent=ca)
@@ -1255,18 +1453,16 @@
               parent=ca1_25)
 
 ca2_18 = Node("NetInvestmentInLeaseExcludingAccruedInterestBeforeAllowanceForCreditLossCurrent", attribute="debit",
               parent=ca1_26)
 ca2_19 = Node("NetInvestmentInLeaseAllowanceForCreditLossExcludingAccruedInterestCurrent", attribute="credit",
               parent=ca1_26)
 
-ca2_20 = Node("DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestBeforeAllowanceForCreditLossCurrent",
-              attribute="debit", parent=ca1_27)
-ca2_21 = Node("DebtSecuritiesAvailableForSaleAmortizedCostAllowanceForCreditLossExcludingAccruedInterestCurrent",
-              attribute="credit", parent=ca1_27)
+ca2_20 = Node("DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestBeforeAllowanceForCreditLossCurrent", attribute="debit", parent=ca1_27)
+ca2_21 = Node("DebtSecuritiesAvailableForSaleAmortizedCostAllowanceForCreditLossExcludingAccruedInterestCurrent", attribute="credit", parent=ca1_27)
 
 ca2_22 = Node("DisposalGroupIncludingDiscontinuedOperationCashAndCashEquivalents", attribute="debit", parent=ca1_29)
 ca2_23 = Node("DisposalGroupIncludingDiscontinuedOperationInventoryCurrent", attribute="debit", parent=ca1_29)
 ca2_24 = Node("DisposalGroupIncludingDiscontinuedOperationOtherCurrentAssets", attribute="debit", parent=ca1_29)
 ca2_25 = Node("DisposalGroupIncludingDiscontinuedOperationAccountsNotesAndLoansReceivableNet", attribute="debit",
               parent=ca1_29)
 ca2_26 = Node("DisposalGroupIncludingDiscontinuedOperationGoodwillCurrent", attribute="debit", parent=ca1_29)
@@ -1396,29 +1592,23 @@
 nca1_2 = Node("FinanceLeaseRightOfUseAsset", attribute="debit", parent=nca)
 nca1_3 = Node("OperatingLeaseRightOfUseAsset", attribute="debit", parent=nca)
 nca1_4 = Node("NetInvestmentInLeaseNoncurrent", attribute="debit", parent=nca)
 nca1_5 = Node("AccountsReceivableExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit",
               parent=nca)
 nca1_6 = Node("FinancingReceivableExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit",
               parent=nca)
-nca1_7 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent",
-              attribute="debit", parent=nca)
-nca1_8 = Node("NetInvestmentInLeaseExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit",
-              parent=nca)
-nca1_9 = Node(
-    "DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent",
-    attribute="debit", parent=nca)
-nca1_10 = Node("LeveragedLeasesNetInvestmentInLeveragedLeasesDisclosureInvestmentInLeveragedLeasesNet",
-               attribute="debit", parent=nca)
+nca1_7 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
+nca1_8 = Node("NetInvestmentInLeaseExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
+nca1_9 = Node("DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
+nca1_10 = Node("LeveragedLeasesNetInvestmentInLeveragedLeasesDisclosureInvestmentInLeveragedLeasesNet", attribute="debit", parent=nca)
 nca1_11 = Node("InventoryRealEstate", attribute="debit", parent=nca)
 nca1_12 = Node("NontradeReceivablesNoncurrent", attribute="debit", parent=nca)
 nca1_13 = Node("PropertyPlantAndEquipmentNet", attribute="debit", parent=nca)
 nca1_14 = Node("PropertyPlantAndEquipmentCollectionsNotCapitalized", attribute="debit", parent=nca)
-nca1_15 = Node("DebtSecuritiesAvailableForSaleAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit",
-               parent=nca)
+nca1_15 = Node("DebtSecuritiesAvailableForSaleAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
 nca1_16 = Node("OilAndGasPropertySuccessfulEffortMethodNet", attribute="debit", parent=nca)
 nca1_17 = Node("OilAndGasPropertyFullCostMethodNet", attribute="debit", parent=nca)
 nca1_18 = Node("LongTermInvestmentsAndReceivablesNet", attribute="debit", parent=nca)
 nca1_19 = Node("IntangibleAssetsNetIncludingGoodwill", attribute="debit", parent=nca)
 nca1_20 = Node("PrepaidExpenseNoncurrent", attribute="debit", parent=nca)
 nca1_21 = Node("ContractWithCustomerAssetNetNoncurrent", attribute="debit", parent=nca)
 nca1_22 = Node("CapitalizedContractCostNetNoncurrent", attribute="debit", parent=nca)
@@ -1441,39 +1631,28 @@
 
 # Level 2
 
 nca2_1 = Node("InventoryDrillingNoncurrent", attribute="debit", parent=nca1_1)
 nca2_2 = Node("InventoryGasInStorageUndergroundNoncurrent", attribute="debit", parent=nca1_1)
 nca2_3 = Node("OtherInventoryNoncurrent", attribute="debit", parent=nca1_1)
 
-nca2_4 = Node("AccountsReceivableExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit",
-              parent=nca1_5)
-nca2_5 = Node("AccountsReceivableAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit",
-              parent=nca1_5)
-
-nca2_6 = Node("FinancingReceivableExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit",
-              parent=nca1_6)
-nca2_7 = Node("FinancingReceivableAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit",
-              parent=nca1_6)
-
-nca2_8 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent",
-              attribute="debit", parent=nca1_7)
-nca2_9 = Node("DebtSecuritiesHeldToMaturityAllowanceForCreditLossExcludingAccruedInterestNoncurrent",
-              attribute="credit", parent=nca1_7)
-
-nca2_10 = Node("NetInvestmentInLeaseExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit",
-               parent=nca1_8)
-nca2_11 = Node("NetInvestmentInLeaseAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit",
-               parent=nca1_8)
-
-nca2_12 = Node(
-    "DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent",
-    attribute="debit", parent=nca1_9)
-nca2_13 = Node("DebtSecuritiesAvailableForSaleAmortizedCostAllowanceForCreditLossExcludingAccruedInterestNoncurrent",
-               attribute="credit", parent=nca1_9)
+nca2_4 = Node("AccountsReceivableExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca1_5)
+nca2_5 = Node("AccountsReceivableAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit", parent=nca1_5)
+
+nca2_6 = Node("FinancingReceivableExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca1_6)
+nca2_7 = Node("FinancingReceivableAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit", parent=nca1_6)
+
+nca2_8 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca1_7)
+nca2_9 = Node("DebtSecuritiesHeldToMaturityAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit", parent=nca1_7)
+
+nca2_10 = Node("NetInvestmentInLeaseExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca1_8)
+nca2_11 = Node("NetInvestmentInLeaseAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit", parent=nca1_8)
+
+nca2_12 = Node("DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestBeforeAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca1_9)
+nca2_13 = Node("DebtSecuritiesAvailableForSaleAmortizedCostAllowanceForCreditLossExcludingAccruedInterestNoncurrent", attribute="credit", parent=nca1_9)
 
 nca2_13 = Node("InventoryRealEstateImprovements", attribute="debit", parent=nca1_11)
 nca2_14 = Node("InventoryRealEstateHeldForSale", attribute="debit", parent=nca1_11)
 nca2_15 = Node("InventoryRealEstateLandAndLandDevelopmentCosts", attribute="debit", parent=nca1_11)
 nca2_16 = Node("InventoryRealEstateConstructionInProcess", attribute="debit", parent=nca1_11)
 nca2_17 = Node("InventoryRealEstateMortgageLoansHeldInInventory", attribute="debit", parent=nca1_11)
 nca2_18 = Node("InventoryOperativeBuilders", attribute="debit", parent=nca1_11)
```

### Comparing `finqual-0.2.0/finqual.egg-info/PKG-INFO` & `finqual-1.0.0/finqual.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.2.0
+Version: 1.0.0
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,14 +17,15 @@
 ## Features
 
 finqual has the following features:
  
 - Ability to call the income statement, balance sheet or cash flow statement for any company on SEC's Electronic Data Gathering, Analysis, and Retrieval (EDGAR) system.
 - Retrieve comparables companies for a chosen ticker on varying industry classifications (e.g. more general industry classifications or more detailed classifications)
 - Breakdown of chosen financial ratios for a chosen ticker
+- Custom balance sheet for banks and other financial services firms
 
 This has two key features that enable better programmatic access compared to other providers:
 - Ability to call up to 10 requests per second, with built-in rate limiter
 - No restriction on the number of calls within a certain timeframe
 
 ## Quick-start guide
 
@@ -56,44 +57,43 @@
 ```
 
 From there, we use this initalised "Ticker" instance to call the desired function. These functions are:
 ```
 """
 Financial statement functions
 """
-fq.Ticker("TSLA").income(start, end, quarter = None)
+fq.Ticker("TSLA").income(start, end, quarter)
 
-fq.Ticker("TSLA").balance(start, end, quarter = None)
+fq.Ticker("TSLA").balance(start, end, quarter)
 
-fq.Ticker("TSLA").cashflow(start, end, quarter = None)
+fq.Ticker("TSLA").cashflow(start, end, quarter)
 
 """
 Other fundamental financial research functions
 """
 fq.Ticker("TSLA").ratios(start, end)
 
 fq.Ticker("TSLA").comparables(n, level = None)
 ```
 
-The financial statement functions (`income`, `balance` and `cashflow`) takes a mandatory timeframe input (`start` and `end`), and then an optional input to return the quarterly results within that timeframe, otherwise defaulting to returning annual results.
+The financial statement functions (`income`, `balance` and `cashflow`) takes a mandatory timeframe input `start` and `end`, and then an optional input to return the quarterly results within that timeframe by setting `quarter = True`, otherwise defaulting to returning annual results.
 
 The `ratios` function calculates selected financial ratios for the specified timeframe and returns the mean average over that timeframe. The selected financial ratios are a selection of liquidity, profitability and valuation ratios, which are commonly used to compare against other companies,
 
-The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible.
+The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible within the package.
 
 ## Dependencies
 
 Only four packages are required, with the following versions confirmed to be working:
 
-| Package   | Version  |
-|-----------|----------|
+| Package   | Version   |
+|-----------|-----------|
 | pandas    | >= 2.0.2  |
 | numpy     | >= 1.24.3 |
-| requests  | >= 2.31.0 |
+| requests  | >= 2.28.1 |
 | ratelimit | >= 2.2.1  |
 | datetime  | >= 5.1    |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database
-- Banks and financial institutions have different balance sheets compared to other normal companies, so a standardised balance sheet for banks and similar firms is still to be looked at
```

### Comparing `finqual-0.2.0/setup.py` & `finqual-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open('README.md', 'r') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='finqual',
-    version='0.2.0',
+    version='1.0.0',
     description='A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.',
     author='Myztika',
     packages=['finqual'],
     package_dir = {'finqual':"finqual"},
     package_data={'finqual': ['data/*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
```

