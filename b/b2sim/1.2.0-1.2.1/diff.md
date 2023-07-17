# Comparing `tmp/b2sim-1.2.0.tar.gz` & `tmp/b2sim-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.2.0.tar", last modified: Sat Jul 15 02:09:46 2023, max compression
+gzip compressed data, was "b2sim-1.2.1.tar", last modified: Sat Jul 15 03:26:03 2023, max compression
```

## Comparing `b2sim-1.2.0.tar` & `b2sim-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:09.278011 b2sim-1.2.0/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.2.0/LICENSE
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.2.0/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-17 02:40:09.272028 b2sim-1.2.0/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    14949 2023-07-14 03:20:53.000000 b2sim-1.2.0/README.md
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:08.752678 b2sim-1.2.0/b2sim/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.2.0/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    13405 2023-07-17 01:51:34.000000 b2sim-1.2.0/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     9150 2023-07-14 20:10:34.000000 b2sim-1.2.0/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   104947 2023-07-17 02:28:20.000000 b2sim-1.2.0/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     4879 2023-07-16 00:00:41.000000 b2sim-1.2.0/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:09.192068 b2sim-1.2.0/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-07-15 23:21:43.000000 b2sim-1.2.0/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      613 2023-07-15 23:55:30.000000 b2sim-1.2.0/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:09.015348 b2sim-1.2.0/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-17 02:40:08.000000 b2sim-1.2.0/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-17 02:40:09.279909 b2sim-1.2.0/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-17 02:39:47.000000 b2sim-1.2.0/setup.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 05:03:56.275197 b2sim-1.2.1/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.2.1/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.2.1/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-17 05:03:56.264188 b2sim-1.2.1/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    16225 2023-07-17 02:57:10.000000 b2sim-1.2.1/README.md
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 05:03:54.311998 b2sim-1.2.1/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.2.1/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    13456 2023-07-17 04:45:34.000000 b2sim-1.2.1/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     9288 2023-07-17 04:54:06.000000 b2sim-1.2.1/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   105016 2023-07-17 04:56:40.000000 b2sim-1.2.1/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     4879 2023-07-16 00:00:41.000000 b2sim-1.2.1/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 05:03:55.992909 b2sim-1.2.1/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-07-15 23:21:43.000000 b2sim-1.2.1/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      613 2023-07-15 23:55:30.000000 b2sim-1.2.1/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 05:03:55.535765 b2sim-1.2.1/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-17 05:03:51.000000 b2sim-1.2.1/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-17 05:03:52.000000 b2sim-1.2.1/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-17 05:03:51.000000 b2sim-1.2.1/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-17 05:03:51.000000 b2sim-1.2.1/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-17 05:03:51.000000 b2sim-1.2.1/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-17 05:03:56.280190 b2sim-1.2.1/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-17 05:03:41.000000 b2sim-1.2.1/setup.py
```

### Comparing `b2sim-1.2.0/LICENSE` & `b2sim-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.2.0/README.md` & `b2sim-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,21 @@
 
 If it's your first time ever contributing to the code, follow these steps to made the contribution process easy and hassle-free:
 1. Download [GitHub Desktop](https://desktop.github.com/).
 2. Clone the repository to your desktop.
 3. When you're ready to make changes after working on the code, [create a pull request](https://www.nexmo.com/legacy-blog/2020/10/01/how-to-create-a-pull-request-with-github-desktop).
 
 # Update Log
+- (July 14, 2023 - v1.2.0)
+   - Support for engineer overclocks has been added. You can now buy and sell overclocks and use them on farms. See the tutorial file on farms for an example on how to use this new feature.
+   - New argument `mode` for the `Rounds` class. You can initialize the Rounds class with one of four different modes: Stall Factor, Stall Times, Manual, and Theoretical Stall Factor. The details for initialization of the `Rounds` class is briefly explained in the tutorial files.
+   - New argument `max_send_time` for eco sends. This is essentially the same thing as putting a `time` argument on the next eco send but this second syntax option may prove easier to use than `time` in some cases.
+   - All actions now support the `buffer` argument.
+   - New methods `upgrade` and `payout` and `overclock` for the `MonkeyFarm` class. Previously, the handling of modifiers to farm payouts (such as the BRF buff given by Banana Central) was handled by the the `GameState` class. To improve readability for potential contributors *and* better accomodate for the overclock feature, this responsibility is handled by the `MonkeyFarm` class itself.
+   - Fixed an oversight which caused some actions to not work because they did not have a 'Message' parameter.
 - (July 13, 2023 - v1.1.1)
    - Fixed a bug which caused the sim to behave incorrectly when an eco send was specified but a queue wasn't.
    - You can now specify stall times directly when initializing the `Rounds` class, by doing something like `Rounds([(0,6), (1,8.5), (2,10.5), (3,7), (7,8)], mode = 'Stall Times')`. In a later update I will flesh out the tutorial files so that it is more clear how to operate this new mode.
 - (July 12, 2023 - v1.1.0)
    - Reogranized `GameState.processBuyQueue` by introducing for it a new helper method `GameState.processAction`. Potential contributors should now have an easier time adding new actions to the simulator.
    - Within the `sellFarm` and `sellAllFarms` actions, you can now specify whether to withdraw from the farm (assuming it is a bank) before selling or not.
    - You can now specify an argument `queue_threshold` for the `ecoSend` function. This argument prevents the simulator from allowing the attack queue to fill up with more sends than allowed by `queue_threshold`. This is useful for cases of sending multiple ZOMGs on R22 or multiple BADs on R30, where in either case, it is useful to wait until the previous bloon has finished sending before sending the next one so as to minimize self-drain.
```

### Comparing `b2sim-1.2.0/b2sim/actions.py` & `b2sim-1.2.1/b2sim/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #######
 # FARMS
 #######
 
-def buyFarm(buffer = 0, min_buy_time = 0):
+def buyFarm(upgrades = (0,0,0), buffer = 0, min_buy_time = 0):
     return {
         'Type': 'Buy Farm',
+        'Upgrades': upgrades,
         'Buffer': buffer,
         'Minimum Buy Time': min_buy_time,
         'Message': 'Buy Farm'
     }
 
 def upgradeFarm(index, path, buffer = 0, min_buy_time = 0):
     return {
```

### Comparing `b2sim-1.2.0/b2sim/info.py` & `b2sim-1.2.1/b2sim/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # %%
 import pandas as pd
 import os
+from copy import deepcopy as dc
 
 # %%
 
 # These dictionaries contain all the "hard-coded" values that the simulator uses. I could've put this all in one dictionary but decided against it to improve presentability.
 
 farm_payout_values = {
     
@@ -265,23 +266,25 @@
             crosspath_money_spent += farm_upgrades_costs[i][j]
             for k in range(3,6):
                 #Iterates through the different tiers
                 upgrades_of_interest = [0,0,k]
                 upgrades_of_interest[i] = j+1
                 farm_sellback_values[tuple(upgrades_of_interest)] = farm_sellback_values[(0,0,k)] + crosspath_money_spent
 
+    farm_total_cost_values = dc(farm_sellback_values)
+
     for key in farm_sellback_values:
         if key[2] >= 2:
             farm_sellback_values[key] = (sellback_value+0.1)*farm_sellback_values[key]
         else:
             farm_sellback_values[key] = sellback_value*farm_sellback_values[key]
 
-    return farm_sellback_values
+    return farm_total_cost_values, farm_sellback_values
 
-farm_sellback_values = computeSellbackValues(farm_upgrades_costs, farm_cost)
+farm_total_cost_values, farm_sellback_values = computeSellbackValues(farm_upgrades_costs, farm_cost)
 
 # %%
 
 dirname = os.path.dirname(__file__)
 filename = os.path.join(dirname, "templates/eco_send_info.csv")
 
 eco_send_table = pd.read_csv(filename)
```

### Comparing `b2sim-1.2.0/b2sim/main.py` & `b2sim-1.2.1/b2sim/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1336,18 +1336,19 @@
         if dict_obj['Type'] == 'Buy Defense':
             if stage == 'check':
                 h_cash, h_loan = impact(h_cash, h_loan, -1*dict_obj['Cost'])
             # We don't need to do anything here in the processing stage
         # FARM RELATED MATTERS
         elif dict_obj['Type'] == 'Buy Farm':
             if stage == 'check':
-                h_new_cash, h_new_loan = impact(h_cash, h_loan, -1*farm_globals['Farm Cost'])
+                farm_cost = farm_total_cost_values[dict_obj['Upgrades']]
+                h_cash, h_loan = impact(h_cash, h_loan, -1*farm_cost)
             else:
                 self.logs.append("Purchasing farm!")
-                farm_info = initFarm(purchase_time = payout['Time'], upgrades = [0,0,0])
+                farm_info = initFarm(purchase_time = payout['Time'], upgrades = list(dict_obj['Upgrades']))
                 farm = MonkeyFarm(farm_info)
                 self.farms.append(farm)
 
                 #For revenue and expense tracking
                 farm.revenue = 0
                 farm.expenses = farm_globals['Farm Cost']
         elif dict_obj['Type'] == 'Upgrade Farm':
```

### Comparing `b2sim-1.2.0/b2sim/rounds.py` & `b2sim-1.2.1/b2sim/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.2.0/b2sim/templates/eco_send_info.csv` & `b2sim-1.2.1/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

### Comparing `b2sim-1.2.0/b2sim/templates/nat_send_lengths.csv` & `b2sim-1.2.1/b2sim/templates/nat_send_lengths.csv`

 * *Files identical despite different names*

