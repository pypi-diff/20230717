# Comparing `tmp/b2sim-1.1.1.tar.gz` & `tmp/b2sim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.1.1.tar", last modified: Fri Jul 14 02:57:14 2023, max compression
+gzip compressed data, was "b2sim-1.2.0.tar", last modified: Sat Jul 15 02:09:46 2023, max compression
```

## Comparing `b2sim-1.1.1.tar` & `b2sim-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.893132 b2sim-1.1.1/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.1.1/LICENSE
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.1.1/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-14 02:57:14.884618 b2sim-1.1.1/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    12903 2023-07-12 18:41:22.000000 b2sim-1.1.1/README.md
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.265361 b2sim-1.1.1/b2sim/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.1.1/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10817 2023-07-12 23:37:31.000000 b2sim-1.1.1/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8804 2023-07-12 20:35:37.000000 b2sim-1.1.1/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   103703 2023-07-14 02:24:33.000000 b2sim-1.1.1/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     4135 2023-07-14 02:54:35.000000 b2sim-1.1.1/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.768344 b2sim-1.1.1/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-07-12 20:07:14.000000 b2sim-1.1.1/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      418 2023-07-12 18:41:22.000000 b2sim-1.1.1/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.524260 b2sim-1.1.1/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-14 02:57:14.896128 b2sim-1.1.1/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-14 02:25:19.000000 b2sim-1.1.1/setup.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:09.278011 b2sim-1.2.0/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.2.0/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.2.0/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-17 02:40:09.272028 b2sim-1.2.0/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    14949 2023-07-14 03:20:53.000000 b2sim-1.2.0/README.md
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:08.752678 b2sim-1.2.0/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.2.0/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    13405 2023-07-17 01:51:34.000000 b2sim-1.2.0/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     9150 2023-07-14 20:10:34.000000 b2sim-1.2.0/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   104947 2023-07-17 02:28:20.000000 b2sim-1.2.0/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     4879 2023-07-16 00:00:41.000000 b2sim-1.2.0/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:09.192068 b2sim-1.2.0/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-07-15 23:21:43.000000 b2sim-1.2.0/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      613 2023-07-15 23:55:30.000000 b2sim-1.2.0/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-17 02:40:09.015348 b2sim-1.2.0/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-17 02:40:08.000000 b2sim-1.2.0/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-17 02:40:07.000000 b2sim-1.2.0/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-17 02:40:09.279909 b2sim-1.2.0/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-17 02:39:47.000000 b2sim-1.2.0/setup.py
```

### Comparing `b2sim-1.1.1/LICENSE` & `b2sim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.1.1/README.md` & `b2sim-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 ## For noobs:
 1. Install python on your computer here: https://www.anaconda.com/download/
 2. Open the anaconda prompt and type `pip install b2sim`.
 3. Your installation of anaconda came with a program called "Jupyter Notebook", which allows you to create and edit .ipynb files which you will use to operate the code. Open Jupyter, and create a new .ipynb file wherever you wish on your computer.
 4. In the first cell of this new .ipynb file you've created, type `import b2sim as b2` and hit enter. 
 5. Congratulations, you now have a file which you can use to generate simulations! Check out the tutorial files in this repo (examples folder) for more info on how to operate the library.
+6. (Bonus step) Instead of Jupyter Notebook, I recommend using [Visual Studio Code](https://code.visualstudio.com/) to operate the code. VS Code comes with a number of bells and whistles and QOL features that can speed up the code-writing process.
 
 ## For experienced coders:
 1. Type `pip install b2sim` in the terminal to download.
 2. Check out the tutorial files in this repo (tutorials folder) for more info on how to operate the library.
 
 ## Alternative installation instructions:
 If for whatever reason pip installation does not work, try the following:
@@ -27,15 +28,30 @@
 3. **Complete Farm support:** The simulator supports IMF Loans and Monkeyopolis. Also, the simulator supports compound purchases, such as selling into Monkey Wall Street.
 4. **Advanced Optimization Potential:** The code can be used in conjuction with optimization or nonlinear root-finding methods to determine the absolute best times to makes your moves during the game.
 
 # Contributing to the Code
 
 Potential contributors are urged to join the [b2 popology discord](https://discord.gg/YBkvcdBN4H) where I can be easily reached with a ping. Look in the "issues" section of this repo for tasks which need to be completed but have not yet been tended to.
 
+## First-Time Contributors
+
+If it's your first time ever contributing to the code, follow these steps to made the contribution process easy and hassle-free:
+1. Download [GitHub Desktop](https://desktop.github.com/).
+2. Clone the repository to your desktop.
+3. When you're ready to make changes after working on the code, [create a pull request](https://www.nexmo.com/legacy-blog/2020/10/01/how-to-create-a-pull-request-with-github-desktop).
+
 # Update Log
+- (July 13, 2023 - v1.1.1)
+   - Fixed a bug which caused the sim to behave incorrectly when an eco send was specified but a queue wasn't.
+   - You can now specify stall times directly when initializing the `Rounds` class, by doing something like `Rounds([(0,6), (1,8.5), (2,10.5), (3,7), (7,8)], mode = 'Stall Times')`. In a later update I will flesh out the tutorial files so that it is more clear how to operate this new mode.
+- (July 12, 2023 - v1.1.0)
+   - Reogranized `GameState.processBuyQueue` by introducing for it a new helper method `GameState.processAction`. Potential contributors should now have an easier time adding new actions to the simulator.
+   - Within the `sellFarm` and `sellAllFarms` actions, you can now specify whether to withdraw from the farm (assuming it is a bank) before selling or not.
+   - You can now specify an argument `queue_threshold` for the `ecoSend` function. This argument prevents the simulator from allowing the attack queue to fill up with more sends than allowed by `queue_threshold`. This is useful for cases of sending multiple ZOMGs on R22 or multiple BADs on R30, where in either case, it is useful to wait until the previous bloon has finished sending before sending the next one so as to minimize self-drain.
+   - The tutorials folder has a new file which covers the simulation of rushes.
 - (July 11, 2023 - v1.0.9)
    - Adjusted the lengths of some of the rounds in `nat_send_lengths.csv`
    - Fixed an error in `eco_send_info.csv` which caused Grouped Reds and Grouped Blues to be unavailable in the simulator on Round 11
    - Fixed a bug which made the code throw an error if a fail-safe was triggered as a consequence of the simulator attempting to use an eco send after it became unavailable.
    - Renamed "examples" folder to "tutorials". Revised the tutorial files so that they are more instructive.
    - Updated `GameState.viewCashEcoHistory` so that it is easier to see when key transactions or changes in eco occur during the simulation.
 - (July 10, 2023 - v1.0.8)
```

### Comparing `b2sim-1.1.1/b2sim/info.py` & `b2sim-1.2.0/b2sim/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,17 @@
     'IMF Loan Amount': 20000,
     'IMF Initial Cooldown': 20,
     'IMF Usage Cooldown': 90,
     'Monkey Wall Street Bonus': 10000,
     'Monkeynomics Payout': 20000,
     'Monkeynomics Initial Cooldown': 20,
     'Monkeynomics Usage Cooldown': 60,
-    'Banana Central Multiplier': 1.25
+    'Banana Central Multiplier': 1.25,
+    'Start of Round Bank Payment': 400,
+    'Start of Round Bank Multiplier': 1.2
 }
 
 # This is admittedly not the cleanest way of organizing this info but
 # this way was the most compatible with older versions of the code
 boat_globals = {
     'Merchantmen Cost': 2800,
     'Upgrade Costs': [5400, 19000], # Upgrade costs of favored trades and Trade Empire respectively
@@ -181,14 +183,22 @@
 }
 
 hero_globals = {
     'Jericho Number of Steals': 10,
     'Jericho Steal Interval': 1
 }
 
+engi_globals = {
+    'Overclock Cost': 15350,
+    'Ultraboost Upgrade Cost': 100000,
+    'Overclock Usage Cooldown': 45, #There is no initial cooldown for the Overclock active
+    'Ultraboost Usage Cooldown': 20,
+    'Overclock Payout Modifier': 1.5
+}
+
 # %%
 
 boat_upgrades_costs = boat_globals['Upgrade Costs']
 boat_payout_values = boat_globals['Payout Values']
 boat_sell_values = boat_globals['Sellback Values'] 
 
 farm_upgrades_costs = farm_globals['Farm Upgrade Costs']
```

### Comparing `b2sim-1.1.1/b2sim/main.py` & `b2sim-1.2.0/b2sim/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,23 @@
         if self.heli_farms is not None:
             self.special_poperations = self.heli_farms['Special Poperations Index']
             self.heli_key = len(self.heli_farms) - 2
         else:
             self.special_poperations = None
             self.heli_key = 0
 
+        # Next, overclocks!
+        overclock_info = initial_state.get('Overclocks')
+        if overclock_info is not None:
+            self.overclocks = overclock_info['Overclocks']
+            self.ultraboost_index = overclock_info['Ultraboost Index']
+        else:
+            self.overclocks = []
+            self.ultraboost_index = None
+
         #~~~~~~~~~~~~
         #HERO SUPPORT
         #~~~~~~~~~~~~
 
         self.jericho_steal_time = float('inf') #Represents the time when Jericho's steal is to be activated.
         self.jericho_steal_amount = 25 #Represents the amount of money Jericho steals
 
@@ -246,15 +255,15 @@
             
         self.logs.append("MESSAGE FROM GameState.__init__(): ")
         self.logs.append("Initialized Game State!")
         self.logs.append("The current game round is %s"%(self.current_round))
         self.logs.append("The current game time is %s seconds"%(self.current_time))
         self.logs.append("The game round start times are given by %s \n"%(self.rounds.round_starts))
         
-    def viewCashEcoHistory(self, dim = (15,18), display_farms = True, font_size = 12):
+    def viewCashEcoHistory(self, dim = (12,6), display_farms = True, font_size = 12):
         self.logs.append("MESSAGE FROM GameState.viewCashEcoHistory():")
         self.logs.append("Graphing history of cash and eco!")
 
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         #Create a table that shows when each significant event in simulation occurs
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -561,15 +570,15 @@
         self.simulation_start_time = self.current_time
         
         # If a target round is given, compute the target_time from that
         if target_round is not None:
             target_time = self.rounds.getTimeFromRound(target_round)
 
         # Append messages to the event messages list showing when each round starts
-        given_round = self.current_round
+        given_round = np.floor(self.rounds.getRoundFromTime(self.current_time, get_frac_part = True) + 1)
         end_round = self.rounds.getRoundFromTime(target_time)
         while given_round <= end_round:
             self.event_messages.append({
                 'Time': self.rounds.getTimeFromRound(given_round),
                 'Type': "Round",
                 'Message': "Round %s start"%(given_round)
             })
@@ -579,15 +588,15 @@
         if target_time < self.current_time:
             target_time = self.current_time
         
         while self.current_time < target_time:
             intermediate_time = min(max(np.floor(self.current_time/interval + 1)*interval,self.current_time + interval/2),target_time)
             self.logs.append("Advancing game to time %s"%(np.round(intermediate_time,3)))
             self.advanceGameState(target_time = intermediate_time)
-            self.logs.append("----------")
+            #self.logs.append("----------")
 
         # Sort the messages in self.event_messages so that they are listed chronologically
         self.event_messages = sorted(self.event_messages, key=lambda x: x['Time']) 
 
         #FOR SPOONOIL: Show warning messages for fail-safes triggered during simulation
         self.showWarnings(self.warnings)
         
@@ -714,19 +723,19 @@
                     farm.account_value = 0
                     new_cash, new_loan = impact(self.cash,self.loan,farm.max_account_value)
                     farm.revenue += new_cash - self.cash #Track the money generated by the farm
                     self.cash, self.loan = new_cash, new_loan
                     self.logs.append("The bank at index %s reached max capacity! Withdrawing money"%(key))
                 self.logs.append("The bank's new account value is %s"%(farm.account_value))
             elif payout['Payout Type'] == 'Bank Interest':
-                #Identify the bank that we're paying and deposit $400, then give 20% interest
+                #Identify the bank that we're paying and deposit the start of round bank bonus, then give interest
                 key = payout['Index']
                 farm = self.farms[key]
-                farm.account_value += 400
-                farm.account_value *= 1.2
+                farm.account_value += farm.payout(payout['Time'], bank_interest = True)
+                farm.account_value *= farm_globals['Start of Round Bank Multiplier']
                 self.logs.append("Awarded bank interest at time %s to the farm at index %s"%(np.round(payout['Time'],2), key))
                 if farm.account_value >= farm.max_account_value:
                     farm.account_value = 0
                     new_cash, new_loan = impact(self.cash,self.loan,farm.max_account_value)
                     farm.revenue += new_cash - self.cash #Track the money generated by the farm
                     self.cash, self.loan = new_cash, new_loan
                     self.logs.append("The bank at index %s reached max capacity! Withdrawing money"%(key))
@@ -790,15 +799,18 @@
             #Record the cash & eco history and advance the game time
             #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
             
             #print("New cash and eco is (%s,%s)"%(np.round(self.cash,2), np.round(self.eco,2)))
             self.time_states.append(payout['Time'])
             self.cash_states.append(self.cash)
             self.eco_states.append(self.eco)
-            self.logs.append("Recorded cash and eco values (%s,%s) at time %s"%(np.round(self.cash,2),np.round(self.eco,2),np.round(payout['Time'],2)))
+
+            #If either the cash or eco values changed since last time, record this in the log
+            if len(self.cash_states) == 1 or self.cash_states[-1] != self.cash_states[-2] or len(self.eco_states) == 1 or self.eco_states[-1] != self.eco_states[-2]:
+                self.logs.append("Recorded cash and eco values (%s,%s) at time %s"%(np.round(self.cash,2),np.round(self.eco,2),np.round(payout['Time'],2)))
             
             # NOTE: The last payment is a "ghost" payment to be awarded at the target time.
             self.current_time = payout['Time']
 
             #If a purchase occured in the buy queue, exit the processing of payments early
             if made_purchase == True:
                 target_time = self.current_time
@@ -996,38 +1008,38 @@
                                             'Source': 'Farm'
                                         }
                                         payout_times.append(payout_entry)
                                     payout_entry = {
                                         'Time': farm_time,
                                         'Payout Type': 'Bank Payment',
                                         'Index': key,
-                                        'Payout': farm.payout_amount,
+                                        'Payout': farm.payout(farm_time),
                                         'Source': 'Farm'
                                     }
                                 elif i == 0 and farm.upgrades[2] == 5 and self.current_round + self.inc > farm_purchase_round:
                                     payout_entry = {
                                         'Time': farm_time,
                                         'Payout Type': 'Direct',
-                                        'Payout': farm.payout_amount + farm_globals['Monkey Wall Street Bonus'],
+                                        'Payout': farm.payout(farm_time, mws_bonus = True),
                                         'Source': 'Farm',
                                         'Index': key
                                     }
                                 elif farm.upgrades[0] == 4 and self.T5_exists[0] == True:
                                     payout_entry = {
                                         'Time': farm_time,
                                         'Payout Type': 'Direct',
-                                        'Payout': farm.payout_amount*farm_globals['Banana Central Multplier'],
+                                        'Payout': farm.payout(farm_time, brf_buff = True),
                                         'Source': 'Farm',
                                         'Index': key
                                     }
                                 else:
                                     payout_entry = {
                                         'Time': farm_time,
                                         'Payout Type': 'Direct',
-                                        'Payout': farm.payout_amount,
+                                        'Payout': farm.payout(farm_time),
                                         'Source': 'Farm',
                                         'Index': key
                                     }
                                 payout_times.append(payout_entry)
                             elif farm_time > target_time:
                                 #self.logs.append("The payout time of %s is too late! Excluding payout time!"%(farm_time))
                                 self.flag = True
@@ -1200,14 +1212,20 @@
                             self.min_buy_time = farm.min_use_time
                         elif farm.min_use_time is None:
                             #If the farm doesn't have a min_use_time designated, it can't be an IMF farm!
                             self.logs.append("Warning! Buy queue entry includes attempt to take out a loan from a farm that is not an IMF Loan! Aborting buy queue!")
                             self.warnings.append(len(self.logs)-1)
                             self.valid_action_flag = False
                             break
+
+                    #If the dict_obj is a Overclock use, force self.min_buy_time to be least the use time of the Overclock
+                    if dict_obj['Type'] == 'Use Overclock':
+                        ind = dict_obj['Engineer Index']
+                        if self.overclocks[ind]['Use Time'] is not None and self.overclocks[ind]['Use Time'] > self.min_buy_time:
+                            self.min_buy_time = self.overclocks[ind]['Use Time']
                     
                 # self.logs.append("Determined the minimum buy time of the next purchase to be %s"%(self.min_buy_time))
                         
             # If we have not yet reached the minimum buy time, break the while loop. 
             # We will check this condition again later:
             if payout['Time'] < self.min_buy_time:
                 break
@@ -1321,18 +1339,15 @@
             # We don't need to do anything here in the processing stage
         # FARM RELATED MATTERS
         elif dict_obj['Type'] == 'Buy Farm':
             if stage == 'check':
                 h_new_cash, h_new_loan = impact(h_cash, h_loan, -1*farm_globals['Farm Cost'])
             else:
                 self.logs.append("Purchasing farm!")
-                farm_info = {
-                    'Purchase Time': self.current_time,
-                    'Upgrades': [0,0,0]
-                }
+                farm_info = initFarm(purchase_time = payout['Time'], upgrades = [0,0,0])
                 farm = MonkeyFarm(farm_info)
                 self.farms.append(farm)
 
                 #For revenue and expense tracking
                 farm.revenue = 0
                 farm.expenses = farm_globals['Farm Cost']
         elif dict_obj['Type'] == 'Upgrade Farm':
@@ -1355,53 +1370,31 @@
             else:
                 ind = dict_obj['Index']
                 path = dict_obj['Path']
                 
                 self.logs.append("Upgrading path %s of the farm at index %s"%(path, ind))
                 farm = self.farms[ind]
 
-                #For expense tracking
-                farm.expenses += farm_upgrades_costs[path][farm.upgrades[path]]
-
-                farm.upgrades[path] += 1
+                farm.upgrade(path, payout['Time'])
 
-                #Update the payout information of the farm
-                farm.payout_amount = farm_payout_values[tuple(farm.upgrades)][0]
-                farm.payout_frequency = farm_payout_values[tuple(farm.upgrades)][1]
-                
-                #So that we can accurately track payments for the farm
-                farm.purchase_time = payout['Time']
-                
-                #Update the sellback value of the farm
-                farm.sell_value = farm_sellback_values[tuple(farm.upgrades)]
-                
                 self.logs.append("The new farm has upgrades (%s,%s,%s)"%(farm.upgrades[0],farm.upgrades[1],farm.upgrades[2]))
                 
-                #If the resulting farm is a Monkey Bank, indicate as such and set its max account value appropriately
-                if farm.upgrades[1] >= 3 and path == 1:
-                    farm.bank = True
-                    farm.max_account_value = farm_bank_capacity[farm.upgrades[1]]
-                    self.logs.append("The new farm is a bank! The bank's max capacity is %s"%(farm.max_account_value))
-                    
-                #If the resulting farm is an IMF Loan or Monkeyopolis, determine the earliest time the loan can be used
-                if farm.upgrades[1] > 3 and path == 1:
-                    farm.min_use_time = payout['Time'] + farm_globals['Monkeynomics Initial Cooldown']
-                
                 #If the resulting farm is a Banana Central, activate the BRF buff, giving them 25% more payment amount
                 if farm.upgrades[0] == 5 and path == 0:
                     self.logs.append("The new farm is a Banana Central!")
                     self.T5_exists[0] = True
                     
-                #If the resutling farm is a Monkeyopolis, mark the x5x_exists flag as true to prevent the user from trying to have multiple of them
-                if farm.upgrades[1] == 5:
+                #If the resutling farm is a Monkeynomics, mark the x5x_exists flag as true to prevent the user from trying to have multiple of them
+                if farm.upgrades[1] == 5 and path == 1:
                     self.T5_exists[1] = True
                 
                 #If the resulting farm is a MWS, mark the MWS_exists flag as true to prevent the user from trying to have multiple of them.
-                if farm.upgrades[2] == 5:
+                if farm.upgrades[2] == 5 and path == 2:
                     self.T5_exists[2] = True
+                
         elif dict_obj['Type'] == 'Sell Farm':
             if stage == 'check':
                 ind = dict_obj['Index']
                 farm = self.farms[ind]
                 withdraw = dict_obj['Withdraw']
 
                 #Check whether the farm is actually on screen before selling it:
@@ -1433,14 +1426,15 @@
                     self.T5_exists[1] = False
                 elif farm.upgrades[2] == 5:
                     self.T5_exists[2] = False
 
                 #Mark the farm's sell time. The code checks whether this value is a number or not before trying to compute farm payments
                 farm.sell_time = payout['Time']
         elif dict_obj['Type'] == 'Sell All Farms':
+            withdraw = dict_obj['Withdraw']
             if stage == 'check':
                 for farm in self.farms:
                     if farm.sell_time is None:
                         h_new_cash, h_new_loan = h_cash, h_loan
                         #Withdraw from the bank first, provided that the withdraw argument is True *and* the farm given is actually a bank
                         if withdraw and farm.upgrades[1] >= 3:
                             h_new_cash, h_new_loan = impact(h_new_cash, h_new_loan, farm.account_value)
@@ -1715,15 +1709,87 @@
                 self.logs.append("Triggered automated heli farm purchases until time %s"%(self.heli_farm_max_buy_time))
         # JERICHO RELATED MATTERS
         elif dict_obj['Type'] == 'Jericho Steal':
             if stage != 'check':
                 self.jericho_steal_time = dict_obj['Minimum Buy Time']
                 self.jericho_steal_amount = dict_obj['Steal Amount']
                 self.cash, self.loan = impact(self.cash,self.loan, dict_obj['Steal Amount']) #If this line is not here, the sim would fail to capture the jeri payment that occurs immediately upon activation.
+        # OVERCLOCK RELATED MATTERS
+        elif dict_obj['Type'] == 'Buy Overclock':
+            if stage == 'check':
+                h_cash, h_loan = impact(h_cash, h_loan, -1*engi_globals['Overclock Cost'])
+            else:
+                self.logs.append("Purchasing overclock!")
+                self.overclocks.append({
+                    'Initial Purchase Time': payout['Time'],
+                    'Use Time': payout['Time'],
+                    'Sell Time': None
+                })
+        elif dict_obj['Type'] == 'Use Overclock':
+            ind = dict_obj['Engineer Index']
+            overclock = self.overclocks[ind]
+
+            if stage == 'check':
+                if overclock['Sell Time'] is not None:
+                    self.logs.append("WARNING! Tried to use an overclock that was already sold! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+            else:
+                # Overclock the farm
+                farm = self.farms[dict_obj['Farm Index']]
+                farm.overclock(payout['Time'])
+
+                # Update the use time of the overclock
+                if self.ultraboost_index is not None and ind == self.ultraboost_index:
+                    #The overclock is in fact an ultraboost
+                    overclock['Use Time'] = payout['Time'] + engi_globals['Ultraboost Usage Cooldown']
+                else:
+                    #The overclock is just a normal overclock
+                    overclock['Use Time'] = payout['Time'] + engi_globals['Overclock Usage Cooldown']
+
+
+        elif dict_obj['Type'] == 'Sell Overclock':
+            ind = dict_obj['Index']
+            overclock = self.overclocks[ind]
+            if stage == 'check':
+                #Check whether the overclock is actually on screen before selling it:
+                if overclock['Sell Time'] is None:
+                    if self.ultraboost_index is not None and ind == self.ultraboost_index:
+                        sell_value = game_globals['Sellback Value']*(engi_globals['Overclock Cost'] + engi_globals['Ultraboost Upgrade Cost'])
+                    else:
+                        sell_value = game_globals['Sellback Value']*engi_globals['Overclock Cost']
+                    h_cash, h_loan = impact(h_cash, h_loan, sell_value)
+                else:
+                    self.logs.append("WARNING! Tried to sell an overclock that is not on screen! Aborting buy queue")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+            else:
+                ind = dict_obj['Index']
+                overclock = self.overclocks[ind]
+                overclock['Sell Time'] = payout['Time']
+
+                #If the overclock being sold is an ultraboost, update the ultraboost index
+                if self.ultraboost_index is not None and ind == self.ultraboost_index:
+                    self.ultraboost_index = None
                 
+                self.logs.append("Selling the overclock at index %s"%(ind))
+        elif dict_obj['Type'] == 'Buy Ultraboost':
+            if stage == 'check':
+                #Do not allow the ultraboost to be purchased if there is already an ultraboost on screen.
+                if self.ultraboost_index is not None:
+                    self.logs.append("WARNING! There is already an Ultraboost on screen! Aborting buy queue")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                h_cash, h_loan = impact(h_cash, h_loan, engi_globals['Ultraboost Upgrade Cost'])
+            else:
+                ind = dict_obj['Index']
+                overclock = self.overclocks[ind]
+                overclock['Use Time'] = payout['Time'] #The Ultraboost ability is battle ready.
+                self.ultraboost_index = ind
+
         if stage == 'check':
             return h_cash, h_loan
         elif stage == 'process':
             return None
             
 # %% [markdown]
 # Now it's time to define the MonkeyFarm class!
@@ -1762,149 +1828,83 @@
         self.max_account_value = farm_bank_capacity[self.upgrades[1]]
         
         #Regarding the IMF Loan/Monkeyopolis active ability
         self.min_use_time = None
         if self.upgrades[1] >= 4:
             self.min_use_time = self.purchase_time + farm_globals['Monkeynomics Initial Cooldown']
 
+        ###################
+        #OVERCLOCK FEATURES
+        ###################
+
+        self.overclock_expiration_time = initial_state.get('Overclock Expiration Time')
+
         ##################
         # REVENUE TRACKING
         ##################
 
         # Rather than remove a farm from the simulator when sold, we will just mark its sell time and tell the simulator not to consider payments from this farm anymore
         self.sell_time = None
 
         self.revenue = 0
         self.expenses = 0
 
         # Tracks hypothetical revenue while processing the buy queue.
         # In general this is necessary because of the impact of Loans on revenue generation.
         self.h_revenue = 0
 
+    def payout(self, time, mws_bonus = False, brf_buff = False, bank_interest = False):
+        #This method should be used over calling self.payout_amount directly because it automatically accounts for overclock & MWS buffs
 
-
-# %% [markdown]
-# The goal of a simulator like this is to compare different strategies and see which one is better. To this end, we define a function capable of simulating multiple game states at once and comparing them.
-
-# %%
-def compareStrategies(initial_state, eco_queues, buy_queues, target_time = None, target_round = 30, display_farms = True, font_size = 12):
-    
-    # Log file in case we need to check outputs
-    logs = []
-    
-    # Given an common initial state and N different tuples of (eco_queue, buy_queue), 
-    # Build N different instances of GameState, advance them to the target_time (or target round if specified)
-    # Finally, graph their cash and eco histories
-    
-    # To begin, let's form the GameState objects we will use in our analysis!
-    game_states = []
-    farm_incomes = []
-    N = len(eco_queues)
-    for i in range(N):
-        init = initial_state
-        init['Eco Queue'] = eco_queues[i]
-        init['Buy Queue'] = buy_queues[i]
-        #print(init['Supply Drops'])
-        game_states.append(GameState(init))
-    
-    #########################
-    # GRAPH CASH & ECO STATES
-    #########################
-    
-    #Now intialize the graphs, one for cash and one for eco
-    fig, ax = plt.subplots(2)
-    fig.set_size_inches(8,12)
-    
-    #For each GameState object, advance the time, and then graph the cash and eco history
-    i = 0
-    cash_min = None
-    if target_round is not None:
-        #Use the target round instead of the target time if specified
-        target_time = game_states[0].rounds.getTimeFromRound(target_round)
-
-    for game_state in game_states:
-        logs.append("Simulating Game State %s"%(i))
-        game_state.fastForward(target_time = target_time)
-        
-        ax[0].plot(game_state.time_states, game_state.cash_states, label = "Cash of Game State %s"%(i))
-        ax[1].plot(game_state.time_states, game_state.eco_states, label = "Eco of Game State %s"%(i))
-        
-        farm_income = 0
-        for key in game_state.farms.keys():
-            #WARNING: This is not a great measure to go by if the player has farms
-            farm = game_state.farms[key]
-            if game_state.T5_exists[0] == True and farm.upgrades[0] == 4:
-                #If the farm is a BRF being buffed by Banana Central
-                farm_income += 1.25*farm.payout_amount*farm.payout_frequency
-            elif farm.upgrades[2] == 5:
-                #If the farm is a Monkey Wall Street
-                farm_income += 10000 + farm.payout_amount*farm.payout_frequency
-            elif farm.upgrades[1] >= 3:
-                #This is an *estimate* based on the impact of one round of bank payments
-                farm_income = farm_income + 1.2*(farm.payout_amount*farm.payout_frequency + 400)
-            else:
-                farm_income += farm.payout_amount*farm.payout_frequency
-        farm_incomes.append(farm_income)
-            
-        
-        if cash_min is None:
-            cash_min = min(game_state.cash_states)
-            eco_min = min(game_state.eco_states)
-            
-            cash_max = max(game_state.cash_states)
-            eco_max = max(game_state.eco_states)
-            
+        if bank_interest:
+            payout_amount = farm_globals['Start of Round Bank Payment']
         else:
-            candidate_cash_min = min(game_state.cash_states)
-            candidate_eco_min = min(game_state.eco_states)
-            
-            if candidate_cash_min < cash_min:
-                cash_min = candidate_cash_min
-            if candidate_eco_min < eco_min:
-                eco_min = candidate_eco_min
-            
-            candidate_cash_max = max(game_state.cash_states)
-            candidate_eco_max = max(game_state.eco_states)
-            
-            if candidate_cash_max > cash_max:
-                cash_max = candidate_cash_max
-            if candidate_eco_max > eco_max:
-                eco_max = candidate_eco_max
-        
-        i += 1
-
-    ####################
-    # GRAPH ROUND STARTS
-    ####################
-    
-    # Also, graph when the rounds start
-    # DEVELOPER'S NOTE: We are dealing with multiple game states where the stall factor in each game state may change
-    # For now, I will just take the round starts from game state 0, but I'll have to adjust this later on down the road.
-    
-    round_to_graph = initial_state['Rounds'].getRoundFromTime(game_states[0].time_states[0]) + 1
-    while initial_state['Rounds'].round_starts[round_to_graph] <= game_states[0].time_states[-1]:
-        logs.append("Graphing round %s, which starts at time %s"%(str(round_to_graph),str(initial_state['Rounds'].round_starts[round_to_graph])))
-        ax[0].plot([initial_state['Rounds'].round_starts[round_to_graph], initial_state['Rounds'].round_starts[round_to_graph]],[cash_min, cash_max], label = "R" + str(round_to_graph) + " start")
-        ax[1].plot([initial_state['Rounds'].round_starts[round_to_graph], initial_state['Rounds'].round_starts[round_to_graph]],[eco_min, eco_max], label = "R" + str(round_to_graph) + " start")
-        round_to_graph += 1
-
-    #################
-    # DISPLAY VISUALS
-    #################
-    
-    ax[0].set_title("Cash vs Time")
-    ax[1].set_title("Eco vs Time")
+            payout_amount = self.payout_amount
+        
+        # First, apply the MWS bonus if relevant:
+        # Note that the code which ensures the MWS bonus is paid out at only the correct times is handled by the GameState class, not the MonkeyFarm class!
+        if mws_bonus and self.upgrades[2] >= 5:
+            payout_amount += farm_globals['Monkey Wall Street Bonus']
+        
+        # Next, if the farm is being buffed by overclock, apply the overclock buff to the payout:
+        # NOTE: The start of round bank interest payment is NOT eligible to be overclock-buffed.
+        if self.overclock_expiration_time is not None and time < self.overclock_expiration_time and not bank_interest:
+            payout_amount *= engi_globals['Overclock Payout Modifier']
+
+        # Finally, if the farm is being buffed by Banana Central, apply that buff to this farm's payment
+        if brf_buff and self.upgrades[0] == 4:
+            payout_amount *= farm_globals['Banana Central Multiplier']
 
-    ax[0].set_ylabel("Cash")
-    ax[1].set_ylabel("Eco")
+        # Finally, return the payout!
+        return payout_amount
+    
+    def upgrade(self, path, time):
+        #For expense tracking
+        self.expenses += farm_upgrades_costs[path][self.upgrades[path]]
 
-    ax[1].set_xlabel("Time (seconds)")
+        self.upgrades[path] += 1
 
-    ax[0].legend(loc='upper left', fontsize = font_size)
-    ax[1].legend(loc='upper left', fontsize = font_size)
-    
-    d = {'Game State': [i for i in range(N)], 'Farm Income': [farm_incomes[i] for i in range(N)]}
-    df = pd.DataFrame(data=d)
-    
-    fig.tight_layout()
-    display(df)
-    logs.append("Successfully generated graph! \n")
+        #Update the payout information of the farm
+        self.payout_amount = farm_payout_values[tuple(self.upgrades)][0]
+        self.payout_frequency = farm_payout_values[tuple(self.upgrades)][1]
+        
+        #So that we can accurately track payments for the farm
+        self.purchase_time = time
+        
+        #Update the sellback value of the farm
+        self.sell_value = farm_sellback_values[tuple(self.upgrades)]
+        
+        #If the resulting farm is a Monkey Bank, indicate as such and set its max account value appropriately
+        if self.upgrades[1] >= 3 and path == 1:
+            self.bank = True
+            self.max_account_value = farm_bank_capacity[self.upgrades[1]]
+            # self.logs.append("The new farm is a bank! The bank's max capacity is %s"%(farm.max_account_value))
+            
+        #If the resulting farm is an IMF Loan or Monkeyopolis, determine the earliest time the loan can be used
+        if self.upgrades[1] > 3 and path == 1:
+            self.min_use_time = time + farm_globals['Monkeynomics Initial Cooldown']
+
+    def overclock(self, time):
+        #What tier of farm do we have right now?
+        tier = max(self.upgrades[0],self.upgrades[1], self.upgrades[2])
+        uptime = 105 - 15*tier
+        self.overclock_expiration_time = time + uptime
```

### Comparing `b2sim-1.1.1/b2sim/templates/eco_send_info.csv` & `b2sim-1.2.0/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

