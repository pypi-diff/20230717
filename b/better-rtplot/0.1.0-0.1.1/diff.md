# Comparing `tmp/better_rtplot-0.1.0.tar.gz` & `tmp/better_rtplot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_rtplot-0.1.0.tar", max compression
+gzip compressed data, was "better_rtplot-0.1.1.tar", max compression
```

## Comparing `better_rtplot-0.1.0.tar` & `better_rtplot-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-28 20:16:53.824192 better_rtplot-0.1.0/LICENSE
--rw-r--r--   0        0        0     8211 2023-06-28 19:48:45.454291 better_rtplot-0.1.0/README.md
--rw-r--r--   0        0        0      428 2023-06-28 20:28:21.084806 better_rtplot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7589 2023-03-10 19:34:26.076818 better_rtplot-0.1.0/rtplot/client.py
--rw-r--r--   0        0        0     6240 2023-03-09 21:43:09.016987 better_rtplot-0.1.0/rtplot/example_code.py
--rw-r--r--   0        0        0     1057 2023-06-12 20:25:54.204024 better_rtplot-0.1.0/rtplot/plot_log.py
--rw-r--r--   0        0        0       71 2023-03-09 21:43:09.016987 better_rtplot-0.1.0/rtplot/saved_plots/.gitignore
--rw-r--r--   0        0        0    23464 2023-06-28 19:48:45.454291 better_rtplot-0.1.0/rtplot/server.py
--rw-r--r--   0        0        0     8905 1970-01-01 00:00:00.000000 better_rtplot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-28 20:16:53.824192 better_rtplot-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8211 2023-06-28 19:48:45.454291 better_rtplot-0.1.1/README.md
+-rw-r--r--   0        0        0      439 2023-07-17 19:14:25.480852 better_rtplot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7588 2023-07-17 19:06:32.364262 better_rtplot-0.1.1/rtplot/client.py
+-rw-r--r--   0        0        0     6240 2023-03-09 21:43:09.016987 better_rtplot-0.1.1/rtplot/example_code.py
+-rw-r--r--   0        0        0     1062 2023-07-13 18:31:13.985659 better_rtplot-0.1.1/rtplot/plot_log.py
+-rw-r--r--   0        0        0       71 2023-03-09 21:43:09.016987 better_rtplot-0.1.1/rtplot/saved_plots/.gitignore
+-rw-r--r--   0        0        0    22802 2023-07-17 19:02:58.496380 better_rtplot-0.1.1/rtplot/server.py
+-rw-r--r--   0        0        0     8860 1970-01-01 00:00:00.000000 better_rtplot-0.1.1/PKG-INFO
```

### Comparing `better_rtplot-0.1.0/LICENSE` & `better_rtplot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.0/README.md` & `better_rtplot-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.0/rtplot/client.py` & `better_rtplot-0.1.1/rtplot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     local_address = "tcp://127.0.0.1:5555"
     configure_ip(ip = local_address)
 
 def plot_to_neurobionics_tv():
     """Send data to a plot in the same computer"""
 
-    tv_computer_address = "tcp://141.212.77.109:5555"
+    tv_computer_address = "tcp://141.212.77.23:5555"
     configure_ip(ip = tv_computer_address)
     
 
 def configure_port(new_port:int):
     """Change the port
     
     Keyword Arguments:
```

### Comparing `better_rtplot-0.1.0/rtplot/example_code.py` & `better_rtplot-0.1.1/rtplot/example_code.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.0/rtplot/plot_log.py` & `better_rtplot-0.1.1/rtplot/plot_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 trace_names = data.columns
 
 #Plot the data
 #Set which trace goes in which plot
 legend_handles = [[] for i in range(num_subplots)]
 for i,subplot in enumerate(subplots):
     k = int(subplot)
-    handel, = axs[k].plot(data.values[:-1,i], label=trace_names[i])
+    handel, = axs[k].plot(time,data.values[:-1,i], label=trace_names[i])
     legend_handles[k].append(handel)
 
 #Add each legend
 for ii in range(num_subplots):
     axs[ii].legend(handles=legend_handles[ii])
 
 #Show the plot
```

### Comparing `better_rtplot-0.1.0/rtplot/server.py` & `better_rtplot-0.1.1/rtplot/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 import datetime
 
 ############################
 # Command Line Arguments #
 ###########################
 
 # Create command line arguments
-parser = argparse.ArgumentParser()
+parser = argparse.ArgumentParser(
+    # help=("Plotter for real time data. By default it will accept plots, however"
+    # "" )
+)
 
 # Add argument to enable bigger fonts
 parser.add_argument(
     "-p",
     "--pi_ip",
     help=(
         "The IP address for the pi, if you don't add"
@@ -44,30 +47,14 @@
 parser.add_argument(
     "-b",
     "--bigscreen",
     help="Increase fonts to print in the big screen",
     action="store_true",
 )
 
-# Add argument to run local plots
-parser.add_argument(
-    "-l", "--local", help="Run local plotting server", action="store_true"
-)
-
-# Add argument to expect the pi to connect to us
-parser.add_argument(
-    "-s",
-    "--static_ip",
-    help=(
-        "Use this to connect the pi to your computer. Pi needs to run "
-        "configure_ip('your_ip')"
-    ),
-    action="store_true",
-)
-
 # Add argument to create subplots in separate columns instead of rows
 parser.add_argument(
     "-c",
     "--column",
     help="Create new plots in separate columns",
     action="store_false",
 )
@@ -153,17 +140,14 @@
 # Else set to normal size
 else:
     axis_label_style = {"font-size": "10pt"}
     title_style = {"size": "14pt"}
     legend_style = {"labelTextSize": "8pt"}
     tick_size = 12
 
-# Get flag for local plotting
-fixed_address = args.local or args.static_ip
-
 # Define if a new subplot is placed in a
 # new row or columns
 NEW_SUBPLOT_IN_ROW = args.column
 
 # Define if debug text output is set on
 DEBUG_TEXT_ENABLED = args.debug
 
@@ -191,24 +175,15 @@
     else:
         connect_string = f"tcp://{args.pi_ip}:5555"
     
     #Connect to that socket
     socket.connect(connect_string)
     print(f"Connected to {connect_string}")
 
-# Elif default to a known address
-elif not fixed_address:
-    # Connect to neurobionics pi - default behaviour for now
-    connect_string = "tcp://10.0.0.200:5555"
-
-    socket.connect(connect_string)
-    print(f"Connected to {connect_string}")
-
-# If we have a fixed address, then the subscriber can reach us
-# good for local plots or fixed ip address
+# Default behavior, wait for people to connect to you
 else:
     # Bind so that you can get more
     socket.bind("tcp://*:5555")
     print("Bounded every ip address on port :5555")
 
 # Initialize subscriber
 socket.setsockopt_string(zmq.SUBSCRIBE, "")
```

### Comparing `better_rtplot-0.1.0/PKG-INFO` & `better_rtplot-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: better-rtplot
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: GPL V3.0
 Author: jmontp
 Author-email: jmontp@umich.edu
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pyarrow (==11.0.0)
 Requires-Dist: pyqtgraph (==0.13.0)
-Requires-Dist: pyside6 (==6.4.1)
+Requires-Dist: pyside6 (<=6.4.0)
 Requires-Dist: pyzmq (==25.0.0)
 Description-Content-Type: text/markdown
 
 ![Logo of the project](https://github.com/jmontp/rtplot/blob/master/.images/signature-stationery.png)
 
 # Real Time Plotting with pyqtgraph and ZMQ
```

