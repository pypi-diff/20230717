# Comparing `tmp/energypylinear-0.1.2.tar.gz` & `tmp/energypylinear-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energypylinear-0.1.2.tar", max compression
+gzip compressed data, was "energypylinear-0.2.0.tar", max compression
```

## Comparing `energypylinear-0.1.2.tar` & `energypylinear-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
--rw-r--r--   0        0        0     2645 2023-07-03 10:23:55.944732 energypylinear-0.1.2/README.md
--rw-r--r--   0        0        0      927 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/__init__.py
--rw-r--r--   0        0        0      167 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/accounting/__init__.py
--rw-r--r--   0        0        0     4014 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/accounting/accounting.py
--rw-r--r--   0        0        0      134 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/__init__.py
--rw-r--r--   0        0        0     1593 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/asset.py
--rw-r--r--   0        0        0    11253 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/battery.py
--rw-r--r--   0        0        0     3624 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/boiler.py
--rw-r--r--   0        0        0     9910 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/chp.py
--rw-r--r--   0        0        0    15201 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/evs.py
--rw-r--r--   0        0        0    12290 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/site.py
--rw-r--r--   0        0        0     2553 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/spill.py
--rw-r--r--   0        0        0     2520 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/valve.py
--rw-r--r--   0        0        0     1418 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/data_generation.py
--rw-r--r--   0        0        0      734 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/defaults.py
--rw-r--r--   0        0        0      357 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/flags.py
--rw-r--r--   0        0        0      650 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/freq.py
--rw-r--r--   0        0        0     6627 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/interval_data.py
--rw-r--r--   0        0        0     4723 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/objectives.py
--rw-r--r--   0        0        0     5367 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/optimizer.py
--rw-r--r--   0        0        0     6122 2023-07-03 10:23:55.952733 energypylinear-0.1.2/energypylinear/plot.py
--rw-r--r--   0        0        0    15471 2023-07-03 10:23:55.952733 energypylinear-0.1.2/energypylinear/results.py
--rw-r--r--   0        0        0      841 2023-07-03 10:23:55.952733 energypylinear-0.1.2/energypylinear/utils.py
--rw-r--r--   0        0        0     1063 2023-07-03 10:23:55.952733 energypylinear-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 energypylinear-0.1.2/setup.py
--rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 energypylinear-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2506 2023-07-17 19:04:10.334779 energypylinear-0.2.0/README.md
+-rw-r--r--   0        0        0      968 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/accounting/__init__.py
+-rw-r--r--   0        0        0     4559 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/accounting/accounting.py
+-rw-r--r--   0        0        0      134 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/__init__.py
+-rw-r--r--   0        0        0     1392 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/asset.py
+-rw-r--r--   0        0        0    12062 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/battery.py
+-rw-r--r--   0        0        0     3722 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/boiler.py
+-rw-r--r--   0        0        0     9916 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/chp.py
+-rw-r--r--   0        0        0    26899 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/evs.py
+-rw-r--r--   0        0        0    12291 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/site.py
+-rw-r--r--   0        0        0     2631 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/spill.py
+-rw-r--r--   0        0        0     2617 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/assets/valve.py
+-rw-r--r--   0        0        0     1453 2023-07-17 19:04:10.338779 energypylinear-0.2.0/energypylinear/data_generation.py
+-rw-r--r--   0        0        0      927 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/debug.py
+-rw-r--r--   0        0        0      770 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/defaults.py
+-rw-r--r--   0        0        0      423 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/flags.py
+-rw-r--r--   0        0        0      650 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/freq.py
+-rw-r--r--   0        0        0     9832 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/interval_data.py
+-rw-r--r--   0        0        0     2951 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/logger.py
+-rw-r--r--   0        0        0     6641 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/objectives.py
+-rw-r--r--   0        0        0     5901 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/optimizer.py
+-rw-r--r--   0        0        0     8335 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/plot.py
+-rw-r--r--   0        0        0      212 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/results/__init__.py
+-rw-r--r--   0        0        0     5518 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/results/checks.py
+-rw-r--r--   0        0        0    14507 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/results/extract.py
+-rw-r--r--   0        0        0     1515 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/results/schema.py
+-rw-r--r--   0        0        0     1296 2023-07-17 19:04:10.342779 energypylinear-0.2.0/energypylinear/results/warnings.py
+-rw-r--r--   0        0        0     1431 2023-07-17 19:04:10.342779 energypylinear-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 energypylinear-0.2.0/setup.py
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 energypylinear-0.2.0/PKG-INFO
```

### Comparing `energypylinear-0.1.2/README.md` & `energypylinear-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 Energy balances are performed on electricity, high & low temperature heat.
 
 ## Setup
 
 Requires Python 3.10+:
 
-```shell
+```shell-session
 $ pip install energypylinear
 ```
 
 ## Quick Start
 
 ### Asset API
 
@@ -37,54 +37,53 @@
 ```python
 import energypylinear as epl
 
 #  2.0 MW, 4.0 MWh battery
 asset = epl.battery.Battery(power_mw=2, capacity_mwh=4, efficiency=0.9)
 
 results = asset.optimize(
-  electricity_prices=[100.0, 50, 200, -100, 0, 200, 100, -100],
-  freq_mins=60,
-  initial_charge_mwh=1,
-  final_charge_mwh=3
+  electricity_prices=[100.0, 50, 200, -100, 0, 200, 100, -100]
 )
 ```
 
-You can find documentation of how to optimize other assets in [how-to/optimize-assets](https://docs.adgefficiency.com/energy-py-linear/how-to/dispach-assets), and Python examples in [energy-py-linear/examples/examples](https://github.com/ADGEfficiency/energy-py-linear/tree/main/examples).
+See how to optimize other asset types in [how-to/optimize-assets](https://energypylinear.adgefficiency.com/latest/how-to/dispatch-assets/). 
 
 ### Site API
 
 The site API allows optimizing multiple assets at once:
 
 ```python
 import energypylinear as epl
 
 site = epl.Site(assets=[
+  #  2.0 MW, 4.0 MWh battery
   epl.Battery(power_mw=2.0, capacity_mwh=4.0),
+  #  30 MW generator
   epl.Generator(
     electric_power_max_mw=100,
     electric_power_min_mw=30,
     electric_efficiency_pct=0.4
   ),
-  epl.evs.EVs(charger_mws=[100, 100])
+  #  2 EV chargers & 4 charge events
+  epl.EVs(
+      chargers_power_mw=[100, 100],
+      charge_events_capacity_mwh=[50, 100, 30, 40],
+      charge_events=[
+          [1, 0, 0, 0, 0],
+          [0, 1, 1, 1, 0],
+          [0, 0, 0, 1, 1],
+          [0, 1, 0, 0, 0]
+      ]
+  )
 ])
 
 results = site.optimize(
   electricity_prices=[100, 50, 200, -100, 0],
   high_temperature_load_mwh=[105, 110, 120, 110, 105],
-  low_temperature_load_mwh=[105, 110, 120, 110, 105],
-  freq_mins=60,
-  initial_charge_mwh=1,
-  final_charge_mwh=3,
-  charge_events=[
-      [1, 0, 0, 0, 0],
-      [0, 1, 1, 1, 0],
-      [0, 0, 0, 1, 1],
-      [0, 1, 0, 0, 0],
-  ],
-  charge_event_mwh=[50, 100, 30, 40]
+  low_temperature_load_mwh=[105, 110, 120, 110, 105]
 )
 ```
 
 The site API will optimize the assets together, and return the results for each asset. 
 
 ### Examples
 
@@ -103,8 +102,8 @@
 
 ```shell
 $ make test
 ```
 
 ## Documentation 
 
-Documentation is hosted at [energypylinear.adgefficiency.com](https://energypylinear.adgefficiency.com/latest).
+Hosted at [energypylinear.adgefficiency.com/latest](https://energypylinear.adgefficiency.com/latest).
```

### Comparing `energypylinear-0.1.2/energypylinear/__init__.py` & `energypylinear-0.2.0/energypylinear/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,34 @@
     accounting,
     assets,
     data_generation,
     defaults,
     interval_data,
     plot,
     results,
-    utils,
 )
 from energypylinear.accounting import get_accounts
-from energypylinear.assets import battery, chp, evs, site, spill, valve
+from energypylinear.assets import battery, chp, site, spill, valve
 from energypylinear.assets.battery import Battery
 from energypylinear.assets.boiler import Boiler
 from energypylinear.assets.chp import Generator
 from energypylinear.assets.evs import EVs
 from energypylinear.assets.site import Site
+from energypylinear.flags import Flags
 from energypylinear.freq import Freq
 from energypylinear.interval_data import IntervalData
 from energypylinear.objectives import objectives
 from energypylinear.optimizer import Optimizer
 
 __all__ = [
     "Battery",
-    "Generator",
     "Boiler",
-    "Site",
-    "Optimizer",
     "EVs",
+    "Flags",
     "Freq",
+    "Generator",
     "IntervalData",
+    "Optimizer",
+    "Site",
     "get_accounts",
-    "utils",
+    "objectives",
 ]
```

### Comparing `energypylinear-0.1.2/energypylinear/accounting/accounting.py` & `energypylinear-0.2.0/energypylinear/accounting/accounting.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 
 class Account(pydantic.BaseModel):
     """An account containing economic cost and carbon emissions."""
 
     cost: float
     emissions: float
 
+    def __str__(self) -> str:
+        return f"<Account profit={-1 * self.cost:.2f} emissions={self.emissions:.4f}>"
+
+    def __repr__(self) -> str:
+        #  TODO
+        return f"<Account profit={-1 * self.cost:.2f} emissions={self.emissions:.4f}>"
+
     def __sub__(self, other: object) -> "Account":
         """
         self == other -> True, else False
         """
         if not isinstance(other, Account):
             raise NotImplementedError("Cannot compare {other} to Account")
 
@@ -57,14 +64,21 @@
     electricity: ElectricityAccount = pydantic.Field(..., repr=False)
     gas: GasAccount = pydantic.Field(..., repr=False)
 
     cost: float
     profit: float
     emissions: float
 
+    def __str__(self) -> str:
+        return f"<Accounts profit={self.profit:.2f} emissions={self.emissions:.4f}>"
+
+    def __repr__(self) -> str:
+        #  TODO
+        return f"<Accounts profit={self.profit:.2f} emissions={self.emissions:.4f}>"
+
 
 def get_one_gas_account(
     interval_data: "epl.interval_data.IntervalData",
     results: pd.DataFrame,
 ) -> GasAccount:
     """Calculate a single gas account from interval data and results."""
     return GasAccount(
@@ -104,14 +118,15 @@
     )
 
 
 def get_accounts(
     interval_data: "epl.interval_data.IntervalData",
     simulation: pd.DataFrame,
     validate: bool = True,
+    verbose: bool = True,
 ) -> Accounts:
     """
     Create one pair of gas and electricity accounts.
     for given of interval data and simulation results.
 
     `interval_data` gives the prices ($/MWh) and carbon intensities (tC/MWh) used
     in the calculation of cost and carbon emissions.
@@ -120,15 +135,15 @@
     calculation of cost and carbon emissions.
 
     Args:
         interval_data: holds prices and carbon intensities.
         simulation: simulation results.
     """
     if validate:
-        epl.results.validate_results(interval_data, simulation)
+        epl.results.validate_results(interval_data, simulation, verbose=verbose)
     electricity = get_one_electricity_account(interval_data, simulation)
     gas = get_one_gas_account(interval_data, simulation)
 
     return Accounts(
         electricity=electricity,
         gas=gas,
         cost=electricity.cost + gas.cost,
```

### Comparing `energypylinear-0.1.2/energypylinear/assets/battery.py` & `energypylinear-0.2.0/energypylinear/assets/battery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Battery asset for optimizing battery dispatch for price or carbon arbitrage."""
-import collections
 import pathlib
 import typing
 
 import numpy as np
 import pulp
 import pydantic
 
@@ -33,103 +32,98 @@
         return name
 
 
 class BatteryOneInterval(AssetOneInterval):
     """Battery asset data for a single interval"""
 
     cfg: BatteryConfig
-    charge_mwh: pulp.LpVariable
-    charge_binary: typing.Union[pulp.LpVariable, int]
-    discharge_mwh: pulp.LpVariable
-    discharge_binary: typing.Union[pulp.LpVariable, int]
-    losses_mwh: pulp.LpVariable
+    electric_charge_mwh: pulp.LpVariable
+    electric_charge_binary: pulp.LpVariable | int
+    electric_discharge_mwh: pulp.LpVariable
+    electric_discharge_binary: pulp.LpVariable | int
+    electric_loss_mwh: pulp.LpVariable
     initial_charge_mwh: pulp.LpVariable
     final_charge_mwh: pulp.LpVariable
     efficiency_pct: float
 
 
 def constrain_only_charge_or_discharge(
     optimizer: Optimizer,
-    vars: collections.defaultdict,
+    battery: AssetOneInterval,
     flags: Flags,
 ) -> None:
     """Constrain battery to only charge or discharge.
 
-    Usually flagged off - slows things down a lot (~2x as slow).
+    Usually flagged off - slows things down a lot (~2x as slow).  Instead of forcing only charge or
+    discharge, the objective function just takes the difference to calculate net charge.
     """
+    assert isinstance(battery, BatteryOneInterval)
     if flags.include_charge_discharge_binary_variables:
-        batteries = epl.utils.filter_assets(vars, "battery")
-        for battery in batteries:
-            optimizer.constrain_max(
-                battery.charge_mwh, battery.charge_binary, battery.cfg.capacity_mwh
-            )
-            optimizer.constrain_max(
-                battery.discharge_mwh,
-                battery.discharge_binary,
-                battery.cfg.capacity_mwh,
-            )
-            optimizer.constrain(battery.charge_binary + battery.discharge_binary <= 1)
+        optimizer.constrain_max(
+            battery.electric_charge_mwh,
+            battery.electric_charge_binary,
+            battery.cfg.capacity_mwh,
+        )
+        optimizer.constrain_max(
+            battery.electric_discharge_mwh,
+            battery.electric_discharge_binary,
+            battery.cfg.capacity_mwh,
+        )
+        optimizer.constrain(
+            battery.electric_charge_binary + battery.electric_discharge_binary <= 1
+        )
 
 
 def constrain_battery_electricity_balance(
-    optimizer: Optimizer, vars: collections.defaultdict
+    optimizer: Optimizer, battery: AssetOneInterval
 ) -> None:
     """Constrain energy balance in a single interval - also calculates losses."""
-
-    assets = vars["assets"][-1]
-    batteries = [a for a in assets if isinstance(a, epl.battery.BatteryOneInterval)]
-
-    for battery in batteries:
-        optimizer.constrain(
-            battery.initial_charge_mwh
-            + battery.charge_mwh
-            - battery.discharge_mwh
-            - battery.losses_mwh
-            == battery.final_charge_mwh
-        )
-        optimizer.constrain(
-            battery.losses_mwh == battery.charge_mwh * (1 - battery.efficiency_pct)
-        )
+    assert isinstance(battery, BatteryOneInterval)
+    optimizer.constrain(
+        battery.initial_charge_mwh
+        + battery.electric_charge_mwh
+        - battery.electric_discharge_mwh
+        - battery.electric_loss_mwh
+        == battery.final_charge_mwh
+    )
+    optimizer.constrain(
+        battery.electric_loss_mwh
+        == battery.electric_charge_mwh * (1 - battery.efficiency_pct)
+    )
 
 
 def constrain_connection_batteries_between_intervals(
-    optimizer: Optimizer, vars: collections.defaultdict
+    optimizer: Optimizer,
+    batteries: list[list[AssetOneInterval]],
 ) -> None:
     """Constrain battery dispatch between two adjacent intervals."""
-    batteries = epl.utils.filter_all_assets(vars, "battery")
 
     #  if in first interval, do nothing
     #  could also do something based on `i` here...
     if len(batteries) < 2:
         return None
 
     else:
         old = batteries[-2]
         new = batteries[-1]
         for alt, neu in zip(old, new, strict=True):
+            assert isinstance(alt, BatteryOneInterval)
+            assert isinstance(neu, BatteryOneInterval)
             optimizer.constrain(alt.final_charge_mwh == neu.initial_charge_mwh)
 
 
 def constrain_initial_final_charge(
-    optimizer: Optimizer,
-    vars: collections.defaultdict,
+    optimizer: Optimizer, initial: AssetOneInterval, final: AssetOneInterval
 ) -> None:
     """Constrain the battery state of charge at the start and end of the simulation."""
+    assert isinstance(initial, BatteryOneInterval)
+    assert isinstance(final, BatteryOneInterval)
 
-    assets = vars["assets"][0]
-    first = [a for a in assets if isinstance(a, epl.battery.BatteryOneInterval)]
-    for battery in first:
-        optimizer.constrain(
-            battery.initial_charge_mwh == battery.cfg.initial_charge_mwh
-        )
-
-    assets = vars["assets"][-1]
-    last = [a for a in assets if isinstance(a, epl.battery.BatteryOneInterval)]
-    for battery in last:
-        optimizer.constrain(battery.final_charge_mwh == battery.cfg.final_charge_mwh)
+    optimizer.constrain(initial.initial_charge_mwh == initial.cfg.initial_charge_mwh)
+    optimizer.constrain(final.final_charge_mwh == final.cfg.final_charge_mwh)
 
 
 class Battery:
     """Battery asset - handles optimization and plotting of results over many intervals.
 
     Args:
         power_mw - the maximum power output of the battery in mega-watts, used for both charge and discharge.
@@ -151,15 +145,15 @@
             power_mw=power_mw,
             capacity_mwh=capacity_mwh,
             efficiency_pct=efficiency,
         )
 
     def __repr__(self) -> str:
         """A string representation of self."""
-        return f"<energypylinear.Battery, power: {self.cfg.power_mw} MW, capacity: {self.cfg.capacity_mwh} MWh>"
+        return f"<energypylinear.Battery power: {self.cfg.power_mw} MW, capacity: {self.cfg.capacity_mwh} MWh>"
 
     def setup_initial_final_charge(
         self, initial_charge_mwh: float, final_charge_mwh: float | None
     ) -> None:
         """Processes the options for initial and final charge."""
         self.cfg.initial_charge_mwh = min(initial_charge_mwh, self.cfg.capacity_mwh)
         self.cfg.final_charge_mwh = (
@@ -170,66 +164,90 @@
 
     def one_interval(
         self, optimizer: Optimizer, i: int, freq: Freq, flags: Flags
     ) -> BatteryOneInterval:
         """Create Battery asset data for a single interval."""
         return BatteryOneInterval(
             cfg=self.cfg,
-            charge_mwh=optimizer.continuous(
+            electric_charge_mwh=optimizer.continuous(
                 f"{self.cfg.name}-charge_mwh-{i}", up=freq.mw_to_mwh(self.cfg.power_mw)
             ),
-            discharge_mwh=optimizer.continuous(
+            electric_discharge_mwh=optimizer.continuous(
                 f"{self.cfg.name}-discharge_mwh-{i}",
                 up=freq.mw_to_mwh(self.cfg.power_mw),
             ),
-            charge_binary=optimizer.binary(f"{self.cfg.name}-charge_binary-{i}")
+            electric_charge_binary=optimizer.binary(
+                f"{self.cfg.name}-charge_binary-{i}"
+            )
             if flags.include_charge_discharge_binary_variables
             else 0,
-            discharge_binary=optimizer.binary(f"{self.cfg.name}-discharge_binary-{i}")
+            electric_discharge_binary=optimizer.binary(
+                f"{self.cfg.name}-discharge_binary-{i}"
+            )
             if flags.include_charge_discharge_binary_variables
             else 0,
-            losses_mwh=optimizer.continuous(f"{self.cfg.name}-losses_mwh-{i}"),
+            electric_loss_mwh=optimizer.continuous(
+                f"{self.cfg.name}-electric_loss_mwh-{i}"
+            ),
             initial_charge_mwh=optimizer.continuous(
                 f"{self.cfg.name}-initial_charge_mwh-{i}",
                 low=0,
                 up=self.cfg.capacity_mwh,
             ),
             final_charge_mwh=optimizer.continuous(
                 f"{self.cfg.name}-final_charge_mwh-{i}", low=0, up=self.cfg.capacity_mwh
             ),
             efficiency_pct=self.cfg.efficiency_pct,
         )
 
     def constrain_within_interval(
         self,
         optimizer: Optimizer,
-        vars: collections.defaultdict,
+        ivars: "epl.interval_data.IntervalVars",
         interval_data: "epl.IntervalData",
         i: int,
         freq: Freq,
         flags: Flags = Flags(),
     ) -> None:
         """Constrain Battery dispatch within a single interval"""
-        constrain_only_charge_or_discharge(optimizer, vars, flags)
-        constrain_battery_electricity_balance(optimizer, vars)
-        constrain_connection_batteries_between_intervals(optimizer, vars)
+        batteries = ivars.filter_objective_variables(
+            BatteryOneInterval, i=-1, asset_name=self.cfg.name
+        )
+        assert len(batteries) == 1
+        battery: AssetOneInterval = batteries[0][0]
+        constrain_only_charge_or_discharge(optimizer, battery, flags)
+        constrain_battery_electricity_balance(optimizer, battery)
+
+        #  this is one battery asset, all intervals
+        all_batteries = ivars.filter_objective_variables(
+            BatteryOneInterval, i=None, asset_name=self.cfg.name
+        )
+        assert isinstance(all_batteries, list)
+        # assert type(all_batteries) == list[list[BatteryOneInterval]]
+        constrain_connection_batteries_between_intervals(optimizer, all_batteries)
 
     def constrain_after_intervals(
         self,
         optimizer: Optimizer,
-        vars: collections.defaultdict,
+        ivars: "epl.interval_data.IntervalVars",
         interval_data: "epl.IntervalData",
     ) -> None:
         """Constrain battery dispatch after all interval asset models are created."""
-        constrain_initial_final_charge(optimizer, vars)
+        initial = ivars.filter_objective_variables(
+            BatteryOneInterval, i=0, asset_name=self.cfg.name
+        )[0][0]
+        final = ivars.filter_objective_variables(
+            BatteryOneInterval, i=-1, asset_name=self.cfg.name
+        )[0][0]
+        constrain_initial_final_charge(optimizer, initial, final)
 
     def optimize(
         self,
-        electricity_prices: np.ndarray | list[float],
-        gas_prices: np.ndarray | list[float] | None = None,
+        electricity_prices: np.ndarray | typing.Sequence[float],
+        gas_prices: np.ndarray | typing.Sequence[float] | None = None,
         electricity_carbon_intensities: np.ndarray | list[float] | None = None,
         freq_mins: int = defaults.freq_mins,
         initial_charge_mwh: float = 0.0,
         final_charge_mwh: float | None = None,
         objective: str = "price",
         flags: Flags = Flags(),
         verbose: bool = True,
@@ -248,56 +266,54 @@
             objective: the optimization objective - either "price" or "carbon".
             flags: boolean flags to change simulation and results behaviour.
             verbose: level of printing.
 
         Returns:
             epl.results.SimulationResult
         """
-        self.optimizer = Optimizer()
+        self.optimizer = Optimizer(verbose=verbose)
         freq = Freq(freq_mins)
         interval_data = epl.interval_data.IntervalData(
             electricity_prices=electricity_prices,
             gas_prices=gas_prices,
             electricity_carbon_intensities=electricity_carbon_intensities,
         )
         self.site = epl.Site()
         self.spill = epl.spill.Spill()
 
         self.setup_initial_final_charge(initial_charge_mwh, final_charge_mwh)
 
-        vars: collections.defaultdict[str, typing.Any] = collections.defaultdict(list)
+        ivars = epl.interval_data.IntervalVars()
         for i in interval_data.idx:
-            vars["sites"].append(
-                self.site.one_interval(self.optimizer, self.site.cfg, i, freq)
-            )
-            vars["assets"].append(
+            ivars.append(self.site.one_interval(self.optimizer, self.site.cfg, i, freq))
+            ivars.append(
                 [
                     self.one_interval(self.optimizer, i, freq, flags),
                     self.spill.one_interval(self.optimizer, i, freq),
                 ]
             )
 
-            self.site.constrain_within_interval(self.optimizer, vars, interval_data, i)
+            self.site.constrain_within_interval(self.optimizer, ivars, interval_data, i)
             self.constrain_within_interval(
-                self.optimizer, vars, interval_data, i, freq, flags=flags
+                self.optimizer, ivars, interval_data, i, freq, flags=flags
             )
 
-        self.constrain_after_intervals(self.optimizer, vars, interval_data)
+        self.constrain_after_intervals(self.optimizer, ivars, interval_data)
 
-        assert len(interval_data.idx) == len(vars["assets"]) == len(vars["sites"])
+        assert len(interval_data.idx) == len(ivars.objective_variables)
 
         objective_fn = epl.objectives[objective]
-        self.optimizer.objective(objective_fn(self.optimizer, vars, interval_data))
+        self.optimizer.objective(objective_fn(self.optimizer, ivars, interval_data))
         status = self.optimizer.solve(verbose=verbose)
 
         self.interval_data = interval_data
         return epl.results.extract_results(
-            interval_data, vars, feasible=status.feasible, verbose=verbose
+            interval_data, ivars, feasible=status.feasible, verbose=verbose
         )
 
     def plot(
         self,
         results: "epl.results.SimulationResult",
-        path: typing.Union[pathlib.Path, str],
+        path: pathlib.Path | str
     ) -> None:
         """Plot simulation results."""
         return epl.plot.plot_battery(results, pathlib.Path(path))
```

### Comparing `energypylinear-0.1.2/energypylinear/assets/boiler.py` & `energypylinear-0.2.0/energypylinear/assets/boiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,37 +68,40 @@
             ),
             cfg=self.cfg,
         )
 
     def constrain_within_interval(
         self,
         optimizer: Optimizer,
-        vars: dict,
+        ivars: "epl.interval_data.IntervalVars",
         interval_data: "epl.IntervalData",
         i: int,
         freq: Freq,
         flags: Flags = Flags(),
     ) -> None:
         """Constrain boiler upper and lower bounds for generating high & low temperature heat."""
-        boilers = epl.utils.filter_assets(vars, "boiler")
-        for asset in boilers:
-            optimizer.constrain(
-                asset.gas_consumption_mwh
-                == asset.high_temperature_generation_mwh
-                * (1 / asset.cfg.high_temperature_efficiency_pct)
-            )
-            optimizer.constrain_max(
-                asset.high_temperature_generation_mwh,
-                asset.binary,
-                freq.mw_to_mwh(asset.cfg.high_temperature_generation_max_mw),
-            )
-            optimizer.constrain_min(
-                asset.high_temperature_generation_mwh,
-                asset.binary,
-                freq.mw_to_mwh(asset.cfg.high_temperature_generation_min_mw),
-            )
+        boilers = ivars.filter_objective_variables(
+            BoilerOneInterval, i=-1, asset_name=self.cfg.name
+        )
+        boiler = boilers[0][0]
+        assert isinstance(boiler, BoilerOneInterval)
+        optimizer.constrain(
+            boiler.gas_consumption_mwh
+            == boiler.high_temperature_generation_mwh
+            * (1 / boiler.cfg.high_temperature_efficiency_pct)
+        )
+        optimizer.constrain_max(
+            boiler.high_temperature_generation_mwh,
+            boiler.binary,
+            freq.mw_to_mwh(boiler.cfg.high_temperature_generation_max_mw),
+        )
+        optimizer.constrain_min(
+            boiler.high_temperature_generation_mwh,
+            boiler.binary,
+            freq.mw_to_mwh(boiler.cfg.high_temperature_generation_min_mw),
+        )
 
     def constrain_after_intervals(
         self, *args: typing.Any, **kwargs: typing.Any
     ) -> None:
         """Constrain asset after all interval asset models are created."""
         return
```

### Comparing `energypylinear-0.1.2/energypylinear/assets/chp.py` & `energypylinear-0.2.0/energypylinear/assets/chp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """CHP asset for optimizing dispatch of combined heat and power (CHP) generators."""
-import collections
 import pathlib
 import typing
 
 import numpy as np
 import pulp
 import pydantic
 
@@ -103,22 +102,22 @@
             ),
             cfg=self.cfg,
         )
 
     def constrain_within_interval(
         self,
         optimizer: Optimizer,
-        vars: dict,
+        ivars: "epl.interval_data.IntervalVars",
         interval_data: "epl.IntervalData",
         i: int,
         freq: Freq,
         flags: Flags = Flags(),
     ) -> None:
         """Constrain generator upper and lower bounds for generating electricity, high & low temperature heat."""
-        assets = vars["assets"][-1]
+        assets = ivars.objective_variables[-1]
         generators = [a for a in assets if isinstance(a, epl.chp.GeneratorOneInterval)]
         for asset in generators:
             if asset.cfg.electric_efficiency_pct > 0:
                 optimizer.constrain(
                     asset.gas_consumption_mwh
                     == asset.electric_generation_mwh
                     * (1 / asset.cfg.electric_efficiency_pct)
@@ -148,21 +147,21 @@
         self, *args: typing.Tuple[typing.Any], **kwargs: typing.Any
     ) -> None:
         """Constrain asset after all interval asset models are created."""
         return
 
     def optimize(
         self,
-        electricity_prices: typing.Union[np.ndarray, list[float]],
-        gas_prices: typing.Union[None, np.ndarray, float] = None,
-        electricity_carbon_intensities: typing.Union[
-            None, np.ndarray, list[float], float
-        ] = None,
-        high_temperature_load_mwh: typing.Union[None, np.ndarray, list[float]] = None,
-        low_temperature_load_mwh: typing.Union[None, np.ndarray, list[float]] = None,
+        electricity_prices: np.ndarray | typing.Sequence[float],
+        gas_prices: np.ndarray | typing.Sequence[float] | float | None = None,
+        # fmt: off
+        electricity_carbon_intensities: np.ndarray| typing.Sequence[float] | float | None = None,
+        high_temperature_load_mwh: np.ndarray| typing.Sequence[float] | float| None = None,
+        low_temperature_load_mwh: np.ndarray| typing.Sequence[float] | float | None = None,
+        # fmt: on
         freq_mins: int = defaults.freq_mins,
         objective: str = "price",
         flags: Flags = Flags(),
     ) -> "epl.results.SimulationResult":
         """
         Optimize the CHP generator's dispatch using a mixed-integer linear program.
 
@@ -196,50 +195,50 @@
             + max(interval_data.low_temperature_load_mwh)
         )
         self.boiler = epl.Boiler(
             high_temperature_generation_max_mw=default_boiler_size,
             high_temperature_efficiency_pct=defaults.default_boiler_efficiency_pct,
         )
 
-        vars: collections.defaultdict[str, typing.Any] = collections.defaultdict(list)
+        ivars = epl.interval_data.IntervalVars()
         for i in interval_data.idx:
-            vars["sites"].append(
-                self.site.one_interval(self.optimizer, self.site.cfg, i, freq)
-            )
-            vars["assets"].append(
+            ivars.append(self.site.one_interval(self.optimizer, self.site.cfg, i, freq))
+            ivars.append(
                 [
                     self.one_interval(self.optimizer, i, freq),
                     self.boiler.one_interval(self.optimizer, i, freq),
                     self.valve.one_interval(self.optimizer, i, freq),
                     self.spill.one_interval(self.optimizer, i, freq),
                 ]
             )
 
-            self.site.constrain_within_interval(self.optimizer, vars, interval_data, i)
-            self.constrain_within_interval(self.optimizer, vars, interval_data, i, freq)
+            self.site.constrain_within_interval(self.optimizer, ivars, interval_data, i)
+            self.constrain_within_interval(
+                self.optimizer, ivars, interval_data, i, freq
+            )
             self.boiler.constrain_within_interval(
-                self.optimizer, vars, interval_data, i, freq
+                self.optimizer, ivars, interval_data, i, freq
             )
             self.valve.constrain_within_interval(
-                self.optimizer, vars, interval_data, i, freq
+                self.optimizer, ivars, interval_data, i, freq
             )
             self.spill.constrain_within_interval(
-                self.optimizer, vars, interval_data, i, freq
+                self.optimizer, ivars, interval_data, i, freq
             )
 
-        assert len(interval_data.idx) == len(vars["assets"])
+        assert len(interval_data.idx) == len(ivars.objective_variables)
 
         objective_fn = epl.objectives[objective]
-        self.optimizer.objective(objective_fn(self.optimizer, vars, interval_data))
+        self.optimizer.objective(objective_fn(self.optimizer, ivars, interval_data))
         status = self.optimizer.solve()
         self.interval_data = interval_data
         return epl.results.extract_results(
-            interval_data, vars, feasible=status.feasible, flags=flags
+            interval_data, ivars, feasible=status.feasible, flags=flags
         )
 
     def plot(
         self,
         results: "epl.results.SimulationResult",
-        path: typing.Union[pathlib.Path, str],
+        path: pathlib.Path | str
     ) -> None:
         """Plot simulation results."""
         return epl.plot.plot_chp(results, pathlib.Path(path))
```

### Comparing `energypylinear-0.1.2/energypylinear/assets/site.py` & `energypylinear-0.2.0/energypylinear/assets/site.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """Site asset for optimizing dispatch of combined heat and power (CHP) generators."""
-import collections
 import typing
 
-import numpy as np
 import pulp
 import pydantic
 
 import energypylinear as epl
 from energypylinear.defaults import defaults
 from energypylinear.flags import Flags
 from energypylinear.freq import Freq
 from energypylinear.optimizer import Optimizer
 
 
 class SiteConfig(pydantic.BaseModel):
     """Site configuration."""
 
+    name: str = "site"
+
     import_limit_mw: float = 10000
     export_limit_mw: float = 10000
 
 
 class SiteOneInterval(pydantic.BaseModel):
     """Site data for a single interval."""
 
+    cfg: SiteConfig
+
     import_power_mwh: pulp.LpVariable
     export_power_mwh: pulp.LpVariable
     import_power_bin: pulp.LpVariable
     export_power_bin: pulp.LpVariable
 
     import_limit_mwh: float
     export_limit_mwh: float
@@ -35,92 +37,101 @@
         """pydantic.BaseModel configuration."""
 
         arbitrary_types_allowed: bool = True
 
 
 def constrain_site_electricity_balance(
     optimizer: Optimizer,
-    vars: dict,
+    cfg: SiteConfig,
+    ivars: "epl.interval_data.IntervalVars",
     interval_data: "epl.interval_data.IntervalData",
     i: int,
 ) -> None:
     """Constrain site electricity balance.
 
     in = out + accumulation
     import + generation = (export + load) + (charge - discharge)
     import + generation - (export + load) - (charge - discharge) = 0
     """
-    assets = vars["assets"][-1]
-    site = vars["sites"][-1]
-    spills = epl.utils.filter_assets(vars, "spill")
+    assets = ivars.objective_variables[-1]
+    site = ivars.filter_site(i=-1, site_name=cfg.name)
+    spills = ivars.filter_objective_variables(epl.assets.spill.SpillOneInterval, i=-1)[
+        0
+    ]
 
     assert interval_data.electricity_load_mwh is not None
     optimizer.constrain(
         (
             site.import_power_mwh
             - site.export_power_mwh
             - interval_data.electricity_load_mwh[i]
             + optimizer.sum([a.electric_generation_mwh for a in assets])
             - optimizer.sum([a.electric_load_mwh for a in assets])
-            - optimizer.sum([a.charge_mwh for a in assets])
-            + optimizer.sum([a.discharge_mwh for a in assets])
+            - optimizer.sum([a.electric_charge_mwh for a in assets])
+            + optimizer.sum([a.electric_discharge_mwh for a in assets])
             + (spills[-1].electric_generation_mwh if spills else 0)
             - (spills[-1].electric_load_mwh if spills else 0)
         )
         == 0
     )
 
 
-def constrain_site_import_export(optimizer: Optimizer, vars: dict) -> None:
+def constrain_site_import_export(
+    optimizer: Optimizer,
+    cfg: SiteConfig,
+    ivars: "epl.interval_data.IntervalVars",
+) -> None:
     """Constrain to only do one of import and export electricity in an interval."""
-    site = vars["sites"][-1]
+    site = ivars.filter_site(i=-1, site_name=cfg.name)
     optimizer.constrain(
         site.import_power_mwh - site.import_limit_mwh * site.import_power_bin <= 0
     )
     optimizer.constrain(
         site.export_power_mwh - site.export_limit_mwh * site.export_power_bin <= 0
     )
     optimizer.constrain(site.import_power_bin + site.export_power_bin == 1)
 
 
 def constrain_site_high_temperature_heat_balance(
     optimizer: Optimizer,
-    vars: dict,
+    cfg: SiteConfig,
+    ivars: "epl.interval_data.IntervalVars",
     interval_data: "epl.interval_data.IntervalData",
     i: int,
 ) -> None:
     """Constrain high temperature energy balance.
 
     in = out + accumulation
     generation = load
     generation - load = 0
     """
-    assets = vars["assets"][-1]
+    assets = ivars.objective_variables[-1]
     assert interval_data.high_temperature_load_mwh is not None
     optimizer.constrain(
         optimizer.sum([a.high_temperature_generation_mwh for a in assets])
         - optimizer.sum([a.high_temperature_load_mwh for a in assets])
         - interval_data.high_temperature_load_mwh[i]
         == 0
     )
 
 
 def constrain_site_low_temperature_heat_balance(
     optimizer: Optimizer,
-    vars: dict,
+    cfg: SiteConfig,
+    ivars: "epl.interval_data.IntervalVars",
     interval_data: "epl.interval_data.IntervalData",
     i: int,
 ) -> None:
     """Constrain low temperature energy balance.
 
     in = out + accumulation
     generation = load
     generation - load = 0
     """
-    assets = vars["assets"][-1]
+    assets = ivars.objective_variables[-1]
     assert interval_data.low_temperature_load_mwh is not None
     optimizer.constrain(
         optimizer.sum([a.low_temperature_generation_mwh for a in assets])
         - optimizer.sum([a.low_temperature_load_mwh for a in assets])
         - interval_data.low_temperature_load_mwh[i]
         == 0
     )
@@ -154,14 +165,15 @@
         return f"<energypylinear.Site assets: {len(self.assets)}>"
 
     def one_interval(
         self, optimizer: Optimizer, site: SiteConfig, i: int, freq: Freq
     ) -> SiteOneInterval:
         """Create Site asset data for a single interval."""
         return SiteOneInterval(
+            cfg=site,
             import_power_mwh=optimizer.continuous(
                 f"import_power_mw-{i}", up=freq.mw_to_mwh(self.cfg.import_limit_mw)
             ),
             export_power_mwh=optimizer.continuous(
                 f"export_power_mw-{i}", up=freq.mw_to_mwh(self.cfg.import_limit_mw)
             ),
             import_power_bin=optimizer.binary(f"import_power_bin-{i}"),
@@ -169,23 +181,27 @@
             import_limit_mwh=freq.mw_to_mwh(site.import_limit_mw),
             export_limit_mwh=freq.mw_to_mwh(site.export_limit_mw),
         )
 
     def constrain_within_interval(
         self,
         optimizer: Optimizer,
-        vars: dict,
+        ivars: "epl.interval_data.IntervalVars",
         interval_data: "epl.interval_data.IntervalData",
         i: int,
     ) -> None:
         """Constrain site within a single interval."""
-        constrain_site_electricity_balance(optimizer, vars, interval_data, i)
-        constrain_site_import_export(optimizer, vars)
-        constrain_site_high_temperature_heat_balance(optimizer, vars, interval_data, i)
-        constrain_site_low_temperature_heat_balance(optimizer, vars, interval_data, i)
+        constrain_site_electricity_balance(optimizer, self.cfg, ivars, interval_data, i)
+        constrain_site_import_export(optimizer, self.cfg, ivars)
+        constrain_site_high_temperature_heat_balance(
+            optimizer, self.cfg, ivars, interval_data, i
+        )
+        constrain_site_low_temperature_heat_balance(
+            optimizer, self.cfg, ivars, interval_data, i
+        )
 
     def optimize(
         self,
         electricity_prices: typing.Union[float, typing.Iterable[float]],
         gas_prices: typing.Optional[typing.Union[float, typing.Iterable[float]]] = None,
         electricity_carbon_intensities: typing.Optional[
             typing.Union[float, typing.Iterable[float]]
@@ -193,21 +209,20 @@
         high_temperature_load_mwh: typing.Optional[
             typing.Union[float, typing.Iterable[float]]
         ] = None,
         low_temperature_load_mwh: typing.Optional[
             typing.Union[float, typing.Iterable[float]]
         ] = None,
         charge_events: typing.Union[list[list[int]], typing.Iterable[int], None] = None,
-        charge_event_mwh: typing.Union[list[int], typing.Iterable[float], None] = None,
         freq_mins: int = defaults.freq_mins,
         initial_charge_mwh: float = 0.0,
         final_charge_mwh: typing.Union[float, None] = None,
         objective: str = "price",
         flags: Flags = Flags(),
-        verbose: int = 0,
+        verbose: bool = True,
     ) -> "epl.results.SimulationResult":
         """Optimize sites dispatch using a mixed-integer linear program.
 
         Args:
             electricity_prices: the price of electricity in each interval.
             gas_prices: the prices of natural gas, used in CHP and boilers in each interval.
             electricity_carbon_intensities: carbon intensity of electricity in each interval.
@@ -221,54 +236,47 @@
                     [1, 0, 0, 0, 0],
                     [0, 1, 1, 1, 0],
                     [0, 0, 0, 1, 1],
                     [0, 1, 0, 0, 0],
                 ]
                 ```
 
-            charge_event_mwh: 1D array of the total charge energy required for each charge event - total across all intervals in mega-watts.
-                Length is the number of charge events.
-                ```
-                charge_event_mwh = [50, 100, 30, 40]
-                ```
-
             freq_mins: the size of an interval in minutes.
             initial_charge_mwh: initial charge state of the battery in mega-watt hours.
             final_charge_mwh: final charge state of the battery in mega-watt hours.
             objective: the optimization objective - either "price" or "carbon".
             flags: boolean flags to change simulation and results behaviour.
             verbose: level of printing.
 
         Returns:
             epl.results.SimulationResult
         """
+
+        #  TODO could be `asset.before_intervals()`
         for asset in self.assets:
             if isinstance(asset, epl.Battery):
                 asset.setup_initial_final_charge(initial_charge_mwh, final_charge_mwh)
 
+            if isinstance(asset, epl.EVs):
+                assert (
+                    asset.charge_events is not None
+                ), "EV asset should have charge events defined in it's __init__"
+
         self.optimizer = Optimizer()
         freq = Freq(freq_mins)
 
-        if charge_events is not None:
-            charge_events = np.array(charge_events).T
-            charge_event_mwh = np.array(charge_event_mwh)
-            evs = epl.interval_data.EVIntervalData(
-                charge_events=charge_events,
-                charge_event_mwh=charge_event_mwh,
-            )
-        else:
-            evs = None
-
+        #  not using the evs' interval data here
+        #  instead that data structure is only made inside the ev assets
         interval_data = epl.interval_data.IntervalData(
             electricity_prices=electricity_prices,
             gas_prices=gas_prices,
             electricity_carbon_intensities=electricity_carbon_intensities,
             high_temperature_load_mwh=high_temperature_load_mwh,
             low_temperature_load_mwh=low_temperature_load_mwh,
-            evs=evs,
+            evs=None,
         )
 
         self.spill = epl.spill.Spill()
         self.valve = epl.valve.Valve()
 
         self.assets.append(self.spill)
         self.assets.append(self.valve)
@@ -277,62 +285,59 @@
         assert len(names) == len(
             set(names)
         ), f"Asset names must be unique, your assets are called {names}"
 
         #  warn about sites without boilers?  warn sites without valve / spill?
 
         #  this is needed for evs_one_interval
-        for asset in self.assets:
-            asset.interval_data = interval_data
+        # for asset in self.assets:
+        #     asset.interval_data = interval_data
 
-        vars: collections.defaultdict[str, typing.Any] = collections.defaultdict(list)
+        ivars = epl.interval_data.IntervalVars()
         for i in interval_data.idx:
-
-            #  setup blocks / data for site and assets
-            vars["sites"].append(self.one_interval(self.optimizer, self.cfg, i, freq))
+            ivars.append(self.one_interval(self.optimizer, self.cfg, i, freq))
             assets = []
             for asset in self.assets:
-                neu_assets = asset.one_interval(self.optimizer, i, freq, flags)
 
+                neu_assets = asset.one_interval(self.optimizer, i, freq, flags)
                 #  tech debt TODO
                 #  EV is special beacuse it returns many blocks per step
                 if isinstance(asset, epl.EVs):
-                    #  evs and spill_evs - NOT the arrays
-                    assets.extend(neu_assets[0])
-                    assets.extend(neu_assets[2])
-                    vars["evs-array"].append(neu_assets[1])
-                    vars["spill-evs-array"].append(neu_assets[3])
+                    evs, evs_array, spill_evs, spill_evs_array = neu_assets
+                    assets.extend(evs)
+                    assets.extend(spill_evs)
+                    ivars.append(evs_array)
+                    ivars.append(spill_evs_array)
                 else:
                     assets.append(neu_assets)
 
-            vars["assets"].append(assets)
+            ivars.append(assets)
 
-            #  constrain within interval
-            self.constrain_within_interval(self.optimizer, vars, interval_data, i)
+            self.constrain_within_interval(self.optimizer, ivars, interval_data, i)
             for asset in self.assets:
                 asset.constrain_within_interval(
-                    self.optimizer, vars, interval_data, i, flags=flags, freq=freq
+                    self.optimizer, ivars, interval_data, i, flags=flags, freq=freq
                 )
 
         for asset in self.assets:
             asset.constrain_after_intervals(
                 self.optimizer,
-                vars,
+                ivars,
                 interval_data,
             )
 
-        assert len(interval_data.idx) == len(vars["assets"]) == len(vars["sites"])
+        assert len(interval_data.idx) == len(ivars.objective_variables)
 
         objective_fn = epl.objectives[objective]
         self.optimizer.objective(
             objective_fn(
                 self.optimizer,
-                vars,
+                ivars,
                 interval_data,
             )
         )
 
         status = self.optimizer.solve(verbose=verbose)
         self.interval_data = interval_data
         return epl.results.extract_results(
-            interval_data, vars, feasible=status.feasible
+            interval_data, ivars, feasible=status.feasible, verbose=verbose
         )
```

### Comparing `energypylinear-0.1.2/energypylinear/assets/spill.py` & `energypylinear-0.2.0/energypylinear/assets/spill.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
     cfg: SpillConfig = SpillConfig()
     electric_generation_mwh: pulp.LpVariable
     electric_load_mwh: pulp.LpVariable
     high_temperature_generation_mwh: pulp.LpVariable
     low_temperature_load_mwh: pulp.LpVariable
 
+    electric_charge_mwh: float = 0.0
+    electric_discharge_mwh: float = 0.0
+
 
 class Spill:
     """Spill asset - allows excess or insufficient balances to be filled in."""
 
     def __init__(self, name: str = "spill"):
         """Initialize a Spill asset model."""
         self.cfg = SpillConfig(name=name)
```

### Comparing `energypylinear-0.1.2/energypylinear/assets/valve.py` & `energypylinear-0.2.0/energypylinear/assets/valve.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,22 +60,24 @@
                 f"{self.cfg.name}-low_temperature_generation_mwh-{i}", low=0
             ),
         )
 
     def constrain_within_interval(
         self,
         optimizer: "epl.optimizer.Optimizer",
-        vars: dict,
+        ivars: "epl.interval_data.IntervalVars",
         interval_data: "epl.IntervalData",
         i: int,
         freq: "epl.freq.Freq",
         flags: epl.flags.Flags = epl.flags.Flags(),
     ) -> None:
         """Constrain thermal balance across the valve."""
-        valve = epl.utils.filter_assets(vars, "valve")[-1]
+        valve = ivars.filter_objective_variables(
+            ValveOneInterval, i=-1, asset_name=self.cfg.name
+        )[0][0]
         optimizer.constrain(
             valve.high_temperature_load_mwh == valve.low_temperature_generation_mwh
         )
 
     def constrain_after_intervals(
         self, *args: typing.Any, **kwargs: typing.Any
     ) -> None:
```

### Comparing `energypylinear-0.1.2/energypylinear/data_generation.py` & `energypylinear-0.2.0/energypylinear/data_generation.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     normal_mu: float = 0,
     normal_std: float = 1,
     uniform_min: float = 0,
     uniform_max: float = 10,
     n_charge_events: int = 10,
     prices_mu: float = 100,
     prices_std: float = 20,
+    seed: int | None = 2,
 ) -> dict:
-    """Create interval data for the `epl.evs.EVs` smart electric charging asset."""
-    np.random.seed(2)
+    """Create interval data for the `epl.EVs` smart electric charging asset."""
+    np.random.seed(seed)
     electricity_prices = np.random.normal(prices_mu, prices_std, idx_length)
     charger_mws = np.random.randint(10, 100, n_chargers)
 
     charge_events = np.zeros((n_charge_events, idx_length))
     charge_length = min(idx_length - 2, charge_length)
 
     for step in range(charge_events.shape[0]):
@@ -31,10 +32,10 @@
         normal_mu, normal_std, n_charge_events
     ) + np.random.uniform(uniform_min, uniform_max, n_charge_events)
     charge_event_mwh = np.clip(charge_event_mwh, a_min=0, a_max=None)
 
     return {
         "electricity_prices": electricity_prices.tolist(),
         "charger_mws": charger_mws,
-        "charge_event_mwh": charge_event_mwh,
+        "charge_events_capacity_mwh": charge_event_mwh,
         "charge_events": charge_events,
     }
```

### Comparing `energypylinear-0.1.2/energypylinear/defaults.py` & `energypylinear-0.2.0/energypylinear/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     spill_objective_penalty: float = 1e11
 
     default_boiler_efficiency_pct: float = 0.8
 
     gas_carbon_intensity: float = 0.185
 
     spill_charge_max_mw: float = 1e4
+    spill_capacity_mwh: float = 1e4
 
     decimal_tolerance: int = 4
 
     #  used for < 0 stuff
-    epsilon: float = -1e-8
+    epsilon: float = -1e-4
 
 
 defaults = Defaults()
```

### Comparing `energypylinear-0.1.2/energypylinear/freq.py` & `energypylinear-0.2.0/energypylinear/freq.py`

 * *Files identical despite different names*

### Comparing `energypylinear-0.1.2/energypylinear/optimizer.py` & `energypylinear-0.2.0/energypylinear/optimizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Interface to the `pulp` optimization library to solve linear programming problems.
 
 The `Optimizer` allows creating linear constraints, variables, and objectives, along with a linear program solver.
 """
 import dataclasses
+import datetime
 import typing
 
 import pulp
 
+from energypylinear.logger import logger
+
 
 @dataclasses.dataclass
 class OptimizationStatus:
     """Result of a linear program optimization."""
 
     status: str
     feasible: bool
@@ -22,17 +25,19 @@
     Solver for linear programs. Interfaces with `pulp`.
 
     Attributes:
         prob: problem to be optimized.
         solver: solver to use for solving the optimization problem.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, verbose: bool = True) -> None:
         """Initialize an Optimizer."""
-        self.prob = pulp.LpProblem("prob", pulp.LpMinimize)
+        name = str(datetime.datetime.now())
+        name = name.replace(" ", "-")
+        self.prob = pulp.LpProblem(name, pulp.LpMinimize)
         self.solver = pulp.PULP_CBC_CMD(msg=0)
 
     def __repr__(self) -> str:
         """A string representation of self."""
         return f"<energypylinear.Optimizer variables: {len(self.variables())} constraints: {len(self.constraints())}>"
 
     def continuous(
@@ -41,25 +46,29 @@
         """Creates a new continuous linear programming variable.
 
         Args:
             name: The name of the variable.
             low: The lower bound of the variable.
             up: The upper bound of the variable.
         """
+        logger.debug("optimizer.continuous", name=name)
         return pulp.LpVariable(name=name, lowBound=low, upBound=up, cat="Continuous")
 
     def binary(self, name: str) -> pulp.LpVariable:
         """Creates a new binary linear programming variable.
 
         Args:
             name: The name of the variable.
         """
+        logger.debug("optimizer.binary", name=name)
         return pulp.LpVariable(name=name, cat="Binary")
 
-    def sum(self, vector: list[pulp.LpAffineExpression]) -> pulp.LpAffineExpression:
+    def sum(
+        self, vector: list[pulp.LpAffineExpression | float]
+    ) -> pulp.LpAffineExpression:
         """Sums a list of linear expressions.
 
         Args:
             vector: list of `LpAffineExpression` objects to sum.
         """
         return pulp.lpSum(vector)
 
@@ -87,34 +96,39 @@
     ) -> OptimizationStatus:
         """Solve the optimization problem.
 
         Args:
             verbose: a flag indicating how verbose the output should be.  0 for no output.
             allow_infeasible: whether an infeasible solution should raise an error.
         """
+        logger.debug(
+            "optimizer.solve",
+            variables=len(self.variables()),
+            constraints=len(self.constraints()),
+        )
         self.assert_no_duplicate_variables()
         self.solver.solve(self.prob)
 
         status = self.status()
         if verbose > 0:
-            print(f"status is {status}")
+            logger.info("optimizer.solve", status=status)
 
         feasible = status == "Optimal"
         if not allow_infeasible:
             assert feasible
 
         return OptimizationStatus(status=status, feasible=feasible)
 
     def assert_no_duplicate_variables(self) -> None:
         """Check there are no duplicate variable names in the optimization problem."""
         variables = self.variables()
         names = [v.name for v in variables]
         assert len(names) == len(
             set(names)
-        ), f"duplicate variables detected - {[x for x in names if names.count(x) >= 2]}"
+        ), f"duplicate variables detected - {len([x for x in names if names.count(x) >= 2])} of {len(names)}\n{sorted(set([x for x in names if names.count(x) >= 2]))}"
 
     def status(self) -> str:
         """Return the status of the optimization problem."""
         return pulp.LpStatus[self.prob.status]
 
     def constraints(self) -> list[pulp.LpConstraint]:
         """Constraints of the optimization problem."""
@@ -148,13 +162,13 @@
         """
         return self.constrain(-continuous + binary * min <= 0)
 
     def value(self, variable: typing.Union[float, pulp.LpVariable]) -> float:
         """Return the value of a linear program variable.
 
         Args:
-            variable: either a pupl variable or already numeric.
+            variable: either a pulp variable or number.
         """
         if isinstance(variable, pulp.LpVariable):
             return variable.value()
         else:
             return float(variable)
```

### Comparing `energypylinear-0.1.2/energypylinear/plot.py` & `energypylinear-0.2.0/energypylinear/plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 import energypylinear as epl
 
 mpl.rcParams["axes.titlesize"] = 10
 
 
 def find_column(df: pd.DataFrame, start: str, end: str) -> str:
     """Finds a column based on the start and end of the column name."""
-    cols = [c for c in df.columns if c.startswith(start) and c.endswith(end)]
+    cols: list[str] = [
+        c for c in df.columns.tolist() if c.startswith(start) and c.endswith(end)
+    ]
     assert len(cols) == 1
     return cols[0]
 
 
 def plot_battery(
     results: "epl.results.SimulationResult", path: pathlib.Path | str
 ) -> None:
@@ -41,16 +43,16 @@
     )
     axes[0].set_ylim()
     axes[0].set_title("Power Balance MWh (Import Positive)")
     axes[0].set_ylabel("MWh")
 
     #  TODO will need some work in a multi-battery world
     simulation["net-battery-charge"] = (
-        simulation[find_column(simulation, "battery-", "-charge_mwh")]
-        - simulation[find_column(simulation, "battery-", "-discharge_mwh")]
+        simulation[find_column(simulation, "battery-", "-electric_charge_mwh")]
+        - simulation[find_column(simulation, "battery-", "-electric_discharge_mwh")]
     )
     simulation.plot(
         ax=axes[1],
         x="Index",
         y="net-battery-charge",
     )
     axes[1].set_title("Battery Charge / Discharge MWh (Charge Positive)")
@@ -82,90 +84,166 @@
     axes[4].set_ylabel("tC/MWh")
 
     for ax in axes:
         ax.get_legend().remove()
     plt.tight_layout()
 
     if path.is_dir():
-        fig.savefig(path / "battery.png")
-    else:
-        fig.savefig(path)
+        path = path / "battery.png"
+    fig.savefig(path)
 
 
 def plot_evs(results: "epl.results.SimulationResult", path: pathlib.Path) -> None:
     """Plot electric vehicle simulation results."""
     simulation = results.simulation
-    fig, axes = plt.subplots(nrows=5)
 
-    charger_usage = simulation[
+    charger_charge = simulation[
         [
             c
             for c in simulation.columns
-            if c.startswith("charger-") and c.endswith("-charge_mwh")
+            if "charger-" in c and c.endswith("-electric_charge_mwh")
         ]
     ].values
+    charger_discharge = simulation[
+        [
+            c
+            for c in simulation.columns
+            if "charger-" in c and c.endswith("-electric_discharge_mwh")
+        ]
+    ].values
+    charger_usage = charger_charge - charger_discharge
+
     charge_event_usage = simulation[
         [
             c
             for c in simulation.columns
-            if c.startswith("charge-event-") and c.endswith("total-charge_mwh")
+            if "charge-event-" in c and c.endswith("electric_charge_mwh")
+        ]
+    ].values
+    discharge_event_usage = simulation[
+        [
+            c
+            for c in simulation.columns
+            if "charge-event-" in c and c.endswith("electric_discharge_mwh")
+        ]
+    ].values
+    charge_event_usage = charge_event_usage - discharge_event_usage
+
+    charge_event_initial_soc = simulation[
+        [
+            c
+            for c in simulation.columns
+            if "charge-event-" in c and c.endswith("initial_soc_mwh")
+        ]
+    ].values
+    charge_event_final_soc = simulation[
+        [
+            c
+            for c in simulation.columns
+            if "charge-event-" in c and c.endswith("final_soc_mwh")
         ]
     ].values
 
     fig, axes = plt.subplots(
         ncols=4, figsize=(14, 6), width_ratios=(5, 10, 1, 1), sharey=True
     )
 
+    data = [
+        *charger_usage.flatten(),
+        *charge_event_usage.flatten(),
+    ]
+    global_vmin = np.min(data)
+    global_vmax = np.max(data)
+
     heatmap_config = {
         "annot_kws": {
-            "size": 6,
+            "size": 12,
         },
         "annot": True,
+        "cbar": False,
+        "cmap": "coolwarm",
+        "vmin": global_vmin,
+        "vmax": global_vmax,
     }
     data = charger_usage
-    seaborn.heatmap(
-        data, ax=axes[0], **heatmap_config, mask=data == 0, fmt="g", cbar=False
-    )
-    axes[0].set_ylabel("Time")
+    seaborn.heatmap(data, ax=axes[0], **heatmap_config, mask=data == 0, fmt="g")
+    axes[0].set_ylabel("Interval")
     axes[0].set_xlabel("Chargers")
 
     data = charge_event_usage
-    #  want to unmask out the periods where charge_event was positive
     assert results.interval_data.evs is not None
+    charge_event_heatmap_config = heatmap_config.copy()
+    result_array = np.empty_like(charge_event_initial_soc, dtype=object)
+
+    for i, (a, b, c) in enumerate(
+        zip(charge_event_initial_soc.T, charge_event_usage.T, charge_event_final_soc.T)
+    ):
+        for j, values in enumerate(zip(a, b, c)):
+            result_array[
+                j, i
+            ] = f"initial: {values[0]:3.1f}\ncharge: {values[1]:3.1f}\nfinal: {values[2]:3.1f}"
+
+    print(result_array)
+    charge_event_heatmap_config["annot"] = result_array
     seaborn.heatmap(
         data,
         ax=axes[1],
-        **heatmap_config,
+        **charge_event_heatmap_config,
+        #  unmask out the periods where charge_event was positive
         mask=results.interval_data.evs.charge_events == 0,
-        fmt="g",
-        cbar_kws={"label": "Charge MWh", "location": "left"}
+        fmt="",
     )
-    axes[1].set_xlabel("Charge Events")
+    axes[1].set_xlabel("Charge Events Net Charge (Discharge is Negative)")
 
-    spill_charge_usage = simulation["charger-spill-charge_mwh"].values.reshape(-1, 1)
+    #   hardcoded asset name here TODO
+    spill_charge_usage = simulation[
+        "evs-charger-spill-evs-electric_charge_mwh"
+    ].values.reshape(-1, 1)
     data = spill_charge_usage
     seaborn.heatmap(
-        data, ax=axes[2], **heatmap_config, xticklabels=["spill"], fmt="g", cbar=False
+        data,
+        ax=axes[2],
+        **(heatmap_config | {"cmap": ["white"]}),
+        xticklabels=["spill"],
+        fmt="g",
     )
 
-    data = np.array(simulation["electricity_prices"]).reshape(-1, 1)
     seaborn.heatmap(
-        data, ax=axes[3], **heatmap_config, xticklabels=["price"], fmt="g", cbar=False
+        np.array(simulation["electricity_prices"]).reshape(-1, 1),
+        ax=axes[3],
+        **(heatmap_config | {"cmap": ["white"]}),
+        xticklabels=["price"],
+        fmt="g",
     )
+    # for ax in axes:
+    #     ax.grid(True)
+    # for ax in axes:
+    #     for spine in ax.spines.values():
+    #         spine.set_edgecolor('gray')
+    #         spine.set_linewidth(2)
+    from matplotlib.patches import Rectangle
+
+    for ax in axes:
+        border = Rectangle(
+            (0, 0),
+            1,
+            1,
+            edgecolor="gray",
+            facecolor="none",
+            transform=ax.transAxes,
+            figure=ax.figure,
+            linewidth=2,
+        )
+        ax.add_patch(border)
 
     plt.tight_layout()
-    pathlib.Path("./figs").mkdir(
-        exist_ok=True,
-        parents=True,
-    )
 
     if path.is_dir():
-        fig.savefig(path / "evs.png")
-    else:
-        fig.savefig(path)
+        path = path / "evs.png"
+    fig.savefig(path)
 
 
 def plot_chp(results: "epl.results.SimulationResult", path: pathlib.Path) -> None:
     """Plot CHP generator simulation results."""
     simulation = results.simulation
     fig, axes = plt.subplots(nrows=5, sharex=True, figsize=(12, 8))
     simulation["Index"] = np.arange(simulation.shape[0]).tolist()
@@ -204,15 +282,15 @@
     simulation.plot(
         "Index",
         "electricity_carbon_intensities",
         ax=axes[4],
     )
     axes[4].set_ylabel("tC/MWh")
     axes[4].set_title("Carbon Intensities")
+
     for ax in axes:
         ax.get_legend().remove()
     plt.tight_layout()
 
     if path.is_dir():
-        fig.savefig(path / "chp.png")
-    else:
-        fig.savefig(path)
+        path = path / "chp.png"
+    fig.savefig(path)
```

### Comparing `energypylinear-0.1.2/pyproject.toml` & `energypylinear-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "energypylinear"
-version = "0.1.2"
+version = "0.2.0"
 description = "Optimizing energy assets with mixed-integer linear programming."
 authors = ["Adam Green <adam.green@adgefficiency.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.12"
@@ -13,37 +13,57 @@
 pydantic = "^1.10.2"
 pandas = "^1.5.2"
 matplotlib = "^3.6.2"
 rich = "^12.0.0"
 seaborn = "^0.12.2"
 pandera = "^0.14.5"
 markdown-include = "^0.8.1"
+structlog = "^23.1.0"
 
 [tool.poetry.group.check.dependencies]
 black = "^22.10.0"
 isort = "^5.10.1"
 flake8-docstring-checker = "^1.1"
 ruff = "^0.0.275"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 coverage = "^6.5.0"
 hypothesis = "^6.61.0"
 phmdoctest = "^1.4.0"
 nbmake = "^1.3.5"
-pytest-testmon = "^1.4.5"
 pytest-sugar = "^0.9.6"
 coverage-badge = "^1.1.0"
+pytest-xdist = "^3.3.1"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.group.develop.dependencies]
 ipython = "^8.7.0"
 
 [tool.poetry.group.static.dependencies]
 mypy = "^0.991"
 
 
-[tool.poetry.group.dev.dependencies]
-mike = "^1.1.2"
+[tool.mypy]
+disallow_any_generics = false
+disallow_incomplete_defs = true
+disallow_untyped_calls = true
+disallow_untyped_defs = true
+implicit_reexport = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+
+[[tool.mypy.overrides]]
+module = [
+  'pandas',
+  'matplotlib',
+  'matplotlib.pyplot',
+  'matplotlib.patches',
+  'pulp',
+  'seaborn'
+]
+ignore_missing_imports = true
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `energypylinear-0.1.2/setup.py` & `energypylinear-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['energypylinear', 'energypylinear.accounting', 'energypylinear.assets']
+['energypylinear',
+ 'energypylinear.accounting',
+ 'energypylinear.assets',
+ 'energypylinear.results']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PuLP>=2.7.0,<3.0.0',
  'markdown-include>=0.8.1,<0.9.0',
  'matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.23.4,<2.0.0',
  'pandas>=1.5.2,<2.0.0',
  'pandera>=0.14.5,<0.15.0',
  'pydantic>=1.10.2,<2.0.0',
  'rich>=12.0.0,<13.0.0',
- 'seaborn>=0.12.2,<0.13.0']
+ 'seaborn>=0.12.2,<0.13.0',
+ 'structlog>=23.1.0,<24.0.0']
 
 setup_kwargs = {
     'name': 'energypylinear',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'Optimizing energy assets with mixed-integer linear programming.',
-    'long_description': '# energy-py-linear\n\n<img src="./static/coverage.svg"> [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)\n\n---\n\nDocumentation: [energypylinear.adgefficiency.com](https://energypylinear.adgefficiency.com/latest)\n\n---\n\nA Python library for optimizing energy assets with mixed-integer linear programming:\n\n- electric batteries,\n- combined heat & power (CHP) generators,\n- electric vehicle smart charging.\n\nAssets can be optimized to either maximize profit or minimize carbon emissions.  \n\nEnergy balances are performed on electricity, high & low temperature heat.\n\n## Setup\n\nRequires Python 3.10+:\n\n```shell\n$ pip install energypylinear\n```\n\n## Quick Start\n\n### Asset API\n\nThe asset API allows optimizing a single asset at once.\n\nWe can optimize an electric battery operating in wholesale price arbitrage using `epl.Battery`:\n\n```python\nimport energypylinear as epl\n\n#  2.0 MW, 4.0 MWh battery\nasset = epl.battery.Battery(power_mw=2, capacity_mwh=4, efficiency=0.9)\n\nresults = asset.optimize(\n  electricity_prices=[100.0, 50, 200, -100, 0, 200, 100, -100],\n  freq_mins=60,\n  initial_charge_mwh=1,\n  final_charge_mwh=3\n)\n```\n\nYou can find documentation of how to optimize other assets in [how-to/optimize-assets](https://docs.adgefficiency.com/energy-py-linear/how-to/dispach-assets), and Python examples in [energy-py-linear/examples/examples](https://github.com/ADGEfficiency/energy-py-linear/tree/main/examples).\n\n### Site API\n\nThe site API allows optimizing multiple assets at once:\n\n```python\nimport energypylinear as epl\n\nsite = epl.Site(assets=[\n  epl.Battery(power_mw=2.0, capacity_mwh=4.0),\n  epl.Generator(\n    electric_power_max_mw=100,\n    electric_power_min_mw=30,\n    electric_efficiency_pct=0.4\n  ),\n  epl.evs.EVs(charger_mws=[100, 100])\n])\n\nresults = site.optimize(\n  electricity_prices=[100, 50, 200, -100, 0],\n  high_temperature_load_mwh=[105, 110, 120, 110, 105],\n  low_temperature_load_mwh=[105, 110, 120, 110, 105],\n  freq_mins=60,\n  initial_charge_mwh=1,\n  final_charge_mwh=3,\n  charge_events=[\n      [1, 0, 0, 0, 0],\n      [0, 1, 1, 1, 0],\n      [0, 0, 0, 1, 1],\n      [0, 1, 0, 0, 0],\n  ],\n  charge_event_mwh=[50, 100, 30, 40]\n)\n```\n\nThe site API will optimize the assets together, and return the results for each asset. \n\n### Examples\n\nExamples as independent scripts are `./examples`:\n\n```shell\n$ ls ./examples\n./examples\n├── battery.py\n├── chp.py\n├── evs.py\n└── forecast-accuracy.py\n```\n\n## Test\n\n```shell\n$ make test\n```\n\n## Documentation \n\nDocumentation is hosted at [energypylinear.adgefficiency.com](https://energypylinear.adgefficiency.com/latest).\n',
+    'long_description': '# energy-py-linear\n\n<img src="./static/coverage.svg"> [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)\n\n---\n\nDocumentation: [energypylinear.adgefficiency.com](https://energypylinear.adgefficiency.com/latest)\n\n---\n\nA Python library for optimizing energy assets with mixed-integer linear programming:\n\n- electric batteries,\n- combined heat & power (CHP) generators,\n- electric vehicle smart charging.\n\nAssets can be optimized to either maximize profit or minimize carbon emissions.  \n\nEnergy balances are performed on electricity, high & low temperature heat.\n\n## Setup\n\nRequires Python 3.10+:\n\n```shell-session\n$ pip install energypylinear\n```\n\n## Quick Start\n\n### Asset API\n\nThe asset API allows optimizing a single asset at once.\n\nWe can optimize an electric battery operating in wholesale price arbitrage using `epl.Battery`:\n\n```python\nimport energypylinear as epl\n\n#  2.0 MW, 4.0 MWh battery\nasset = epl.battery.Battery(power_mw=2, capacity_mwh=4, efficiency=0.9)\n\nresults = asset.optimize(\n  electricity_prices=[100.0, 50, 200, -100, 0, 200, 100, -100]\n)\n```\n\nSee how to optimize other asset types in [how-to/optimize-assets](https://energypylinear.adgefficiency.com/latest/how-to/dispatch-assets/). \n\n### Site API\n\nThe site API allows optimizing multiple assets at once:\n\n```python\nimport energypylinear as epl\n\nsite = epl.Site(assets=[\n  #  2.0 MW, 4.0 MWh battery\n  epl.Battery(power_mw=2.0, capacity_mwh=4.0),\n  #  30 MW generator\n  epl.Generator(\n    electric_power_max_mw=100,\n    electric_power_min_mw=30,\n    electric_efficiency_pct=0.4\n  ),\n  #  2 EV chargers & 4 charge events\n  epl.EVs(\n      chargers_power_mw=[100, 100],\n      charge_events_capacity_mwh=[50, 100, 30, 40],\n      charge_events=[\n          [1, 0, 0, 0, 0],\n          [0, 1, 1, 1, 0],\n          [0, 0, 0, 1, 1],\n          [0, 1, 0, 0, 0]\n      ]\n  )\n])\n\nresults = site.optimize(\n  electricity_prices=[100, 50, 200, -100, 0],\n  high_temperature_load_mwh=[105, 110, 120, 110, 105],\n  low_temperature_load_mwh=[105, 110, 120, 110, 105]\n)\n```\n\nThe site API will optimize the assets together, and return the results for each asset. \n\n### Examples\n\nExamples as independent scripts are `./examples`:\n\n```shell\n$ ls ./examples\n./examples\n├── battery.py\n├── chp.py\n├── evs.py\n└── forecast-accuracy.py\n```\n\n## Test\n\n```shell\n$ make test\n```\n\n## Documentation \n\nHosted at [energypylinear.adgefficiency.com/latest](https://energypylinear.adgefficiency.com/latest).\n',
     'author': 'Adam Green',
     'author_email': 'adam.green@adgefficiency.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `energypylinear-0.1.2/PKG-INFO` & `energypylinear-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energypylinear
-Version: 0.1.2
+Version: 0.2.0
 Summary: Optimizing energy assets with mixed-integer linear programming.
 License: MIT
 Author: Adam Green
 Author-email: adam.green@adgefficiency.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pandera (>=0.14.5,<0.15.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: rich (>=12.0.0,<13.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Description-Content-Type: text/markdown
 
 # energy-py-linear
 
 <img src="./static/coverage.svg"> [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
 ---
@@ -41,15 +42,15 @@
 
 Energy balances are performed on electricity, high & low temperature heat.
 
 ## Setup
 
 Requires Python 3.10+:
 
-```shell
+```shell-session
 $ pip install energypylinear
 ```
 
 ## Quick Start
 
 ### Asset API
 
@@ -60,54 +61,53 @@
 ```python
 import energypylinear as epl
 
 #  2.0 MW, 4.0 MWh battery
 asset = epl.battery.Battery(power_mw=2, capacity_mwh=4, efficiency=0.9)
 
 results = asset.optimize(
-  electricity_prices=[100.0, 50, 200, -100, 0, 200, 100, -100],
-  freq_mins=60,
-  initial_charge_mwh=1,
-  final_charge_mwh=3
+  electricity_prices=[100.0, 50, 200, -100, 0, 200, 100, -100]
 )
 ```
 
-You can find documentation of how to optimize other assets in [how-to/optimize-assets](https://docs.adgefficiency.com/energy-py-linear/how-to/dispach-assets), and Python examples in [energy-py-linear/examples/examples](https://github.com/ADGEfficiency/energy-py-linear/tree/main/examples).
+See how to optimize other asset types in [how-to/optimize-assets](https://energypylinear.adgefficiency.com/latest/how-to/dispatch-assets/). 
 
 ### Site API
 
 The site API allows optimizing multiple assets at once:
 
 ```python
 import energypylinear as epl
 
 site = epl.Site(assets=[
+  #  2.0 MW, 4.0 MWh battery
   epl.Battery(power_mw=2.0, capacity_mwh=4.0),
+  #  30 MW generator
   epl.Generator(
     electric_power_max_mw=100,
     electric_power_min_mw=30,
     electric_efficiency_pct=0.4
   ),
-  epl.evs.EVs(charger_mws=[100, 100])
+  #  2 EV chargers & 4 charge events
+  epl.EVs(
+      chargers_power_mw=[100, 100],
+      charge_events_capacity_mwh=[50, 100, 30, 40],
+      charge_events=[
+          [1, 0, 0, 0, 0],
+          [0, 1, 1, 1, 0],
+          [0, 0, 0, 1, 1],
+          [0, 1, 0, 0, 0]
+      ]
+  )
 ])
 
 results = site.optimize(
   electricity_prices=[100, 50, 200, -100, 0],
   high_temperature_load_mwh=[105, 110, 120, 110, 105],
-  low_temperature_load_mwh=[105, 110, 120, 110, 105],
-  freq_mins=60,
-  initial_charge_mwh=1,
-  final_charge_mwh=3,
-  charge_events=[
-      [1, 0, 0, 0, 0],
-      [0, 1, 1, 1, 0],
-      [0, 0, 0, 1, 1],
-      [0, 1, 0, 0, 0],
-  ],
-  charge_event_mwh=[50, 100, 30, 40]
+  low_temperature_load_mwh=[105, 110, 120, 110, 105]
 )
 ```
 
 The site API will optimize the assets together, and return the results for each asset. 
 
 ### Examples
 
@@ -126,9 +126,9 @@
 
 ```shell
 $ make test
 ```
 
 ## Documentation 
 
-Documentation is hosted at [energypylinear.adgefficiency.com](https://energypylinear.adgefficiency.com/latest).
+Hosted at [energypylinear.adgefficiency.com/latest](https://energypylinear.adgefficiency.com/latest).
```

