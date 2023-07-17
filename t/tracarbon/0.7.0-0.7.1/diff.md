# Comparing `tmp/tracarbon-0.7.0.tar.gz` & `tmp/tracarbon-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracarbon-0.7.0.tar", max compression
+gzip compressed data, was "tracarbon-0.7.1.tar", max compression
```

## Comparing `tracarbon-0.7.0.tar` & `tracarbon-0.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0    10265 2023-07-15 20:17:41.581233 tracarbon-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     9752 2023-07-15 20:17:41.581233 tracarbon-0.7.0/README.md
--rw-r--r--   0        0        0     2702 2023-07-15 20:17:41.585233 tracarbon-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0      246 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/__init__.py
--rw-r--r--   0        0        0       70 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/__main__.py
--rw-r--r--   0        0        0     3158 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/builder.py
--rw-r--r--   0        0        0     4609 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/cli/__init__.py
--rwxr-xr-x   0        0        0     2320 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/conf.py
--rw-r--r--   0        0        0      111 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/emissions/__init__.py
--rw-r--r--   0        0        0     6361 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/emissions/carbon_emissions.py
--rw-r--r--   0        0        0      734 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exceptions.py
--rwxr-xr-x   0        0        0      237 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/__init__.py
--rwxr-xr-x   0        0        0     2288 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/datadog_exporter.py
--rwxr-xr-x   0        0        0     4999 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/exporter.py
--rw-r--r--   0        0        0     2203 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/json_exporter.py
--rw-r--r--   0        0        0     2605 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/prometheus_exporter.py
--rwxr-xr-x   0        0        0      963 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/stdout.py
--rw-r--r--   0        0        0    10784 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/general_metrics.py
--rwxr-xr-x   0        0        0      210 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/__init__.py
--rw-r--r--   0        0        0     1303 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/cloud_providers.py
--rw-r--r--   0        0        0     4876 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/containers.py
--rw-r--r--   0        0        0        0 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/data/__init__.py
--rw-r--r--   0        0        0   160142 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/data/aws-instances.csv
--rw-r--r--   0        0        0     4720 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/energy.py
--rw-r--r--   0        0        0     1362 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/gpu.py
--rwxr-xr-x   0        0        0     1653 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/hardware.py
--rw-r--r--   0        0        0     6166 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/rapl.py
--rw-r--r--   0        0        0     7242 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/sensors.py
--rwxr-xr-x   0        0        0       85 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/__init__.py
--rw-r--r--   0        0        0     6103 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/country.py
--rw-r--r--   0        0        0        0 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/data/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json
--rw-r--r--   0        0        0     1180 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/data/grid-emissions-factors-aws.csv
--rwxr-xr-x   0        0        0     1576 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/location.py
--rw-r--r--   0        0        0        0 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/py.typed
--rw-r--r--   0        0        0    11335 1970-01-01 00:00:00.000000 tracarbon-0.7.0/PKG-INFO
+-rwxr-xr-x   0        0        0    10265 2023-07-17 09:13:09.701008 tracarbon-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     9815 2023-07-17 09:13:09.701008 tracarbon-0.7.1/README.md
+-rw-r--r--   0        0        0     2721 2023-07-17 09:13:09.701008 tracarbon-0.7.1/pyproject.toml
+-rwxr-xr-x   0        0        0      246 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/__main__.py
+-rw-r--r--   0        0        0     3141 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/builder.py
+-rw-r--r--   0        0        0     4609 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/cli/__init__.py
+-rwxr-xr-x   0        0        0     2320 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/conf.py
+-rw-r--r--   0        0        0      111 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/emissions/__init__.py
+-rw-r--r--   0        0        0     6262 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/emissions/carbon_emissions.py
+-rw-r--r--   0        0        0      734 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/exceptions.py
+-rwxr-xr-x   0        0        0      237 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/exporters/__init__.py
+-rwxr-xr-x   0        0        0     2294 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/exporters/datadog_exporter.py
+-rwxr-xr-x   0        0        0     5988 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/exporters/exporter.py
+-rw-r--r--   0        0        0     2209 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/exporters/json_exporter.py
+-rw-r--r--   0        0        0     2611 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/exporters/prometheus_exporter.py
+-rwxr-xr-x   0        0        0      969 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/exporters/stdout.py
+-rw-r--r--   0        0        0    10780 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/general_metrics.py
+-rwxr-xr-x   0        0        0      210 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/hardwares/__init__.py
+-rw-r--r--   0        0        0     1303 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/hardwares/cloud_providers.py
+-rw-r--r--   0        0        0     4876 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/hardwares/containers.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:13:09.705008 tracarbon-0.7.1/tracarbon/hardwares/data/__init__.py
+-rw-r--r--   0        0        0   160142 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/hardwares/data/aws-instances.csv
+-rw-r--r--   0        0        0     4720 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/hardwares/energy.py
+-rw-r--r--   0        0        0     1362 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/hardwares/gpu.py
+-rwxr-xr-x   0        0        0     1653 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/hardwares/hardware.py
+-rw-r--r--   0        0        0     6166 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/hardwares/rapl.py
+-rw-r--r--   0        0        0     7242 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/hardwares/sensors.py
+-rwxr-xr-x   0        0        0       85 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/locations/__init__.py
+-rw-r--r--   0        0        0     6103 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/locations/country.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/locations/data/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json
+-rw-r--r--   0        0        0     1180 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/locations/data/grid-emissions-factors-aws.csv
+-rwxr-xr-x   0        0        0     1576 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/locations/location.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:13:09.709008 tracarbon-0.7.1/tracarbon/py.typed
+-rw-r--r--   0        0        0    11438 1970-01-01 00:00:00.000000 tracarbon-0.7.1/PKG-INFO
```

### Comparing `tracarbon-0.7.0/LICENSE.txt` & `tracarbon-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/README.md` & `tracarbon-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 
 ```sh
 # Install one or more exporters from the list
 pip install 'tracarbon[datadog,prometheus,kubernetes]'
 ```
 
 ### 🔌 Devices: energy consumption
-| **Devices** |                                                                                                                                              **Description**                                                                                                                                              |
-|-------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-| Mac         |                                                                                                              ✅ Global energy consumption of your Mac (must be plugged into a wall adapter).                                                                                                               |
+| **Devices** |                                                                                                                                                           **Description**                                                                                                                                                            |
+|-------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| Mac         |                                                                                                                            ✅ Global energy consumption of your Mac (must be plugged into a wall adapter).                                                                                                                            |
 | Linux       | ⚠️ Only with [RAPL](https://web.eece.maine.edu/~vweaver/projects/rapl/). See [#1](https://github.com/fvaleye/tracarbon/issues/1). It works with containers on [Kubernetes](https://kubernetes.io/) using the [Metric API](https://kubernetes.io/docs/tasks/debug/debug-cluster/resource-metrics-pipeline/#metrics-api) if available. |
-| Windows     |                                                                                                           ❌ Not yet implemented. See [#184](https://github.com/hubblo-org/scaphandre/pull/184).                                                                                                           |
+| Windows     |                                                                                                                        ❌ Not yet implemented. See [#184](https://github.com/hubblo-org/scaphandre/pull/184).                                                                                                                         |
 
-| **Cloud Provider** |                                                                                                  **Description**                                                                                                  |
-|--------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-| AWS                | ✅ Use the hardware's usage with the EC2 instances carbon emissions datasets of [cloud-carbon-coefficients](https://github.com/cloud-carbon-footprint/cloud-carbon-coefficients/blob/main/data/aws-instances.csv). |
-| GCP                |                                                                                              ❌ Not yet implemented.                                                                                               |
-| Azure              |                                                                                              ❌ Not yet implemented.                                                                                               |
+| **Cloud Provider** |                                                                                             **Description**                                                                                              |
+|--------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| AWS                | ✅ Use the hardware's usage with the EC2 instances carbon emissions datasets of [cloud-carbon-coefficients](https://github.com/cloud-carbon-footprint/ccf-coefficients/blob/main/data/aws-instances.csv). |
+| GCP                |                                                                                          ❌ Not yet implemented.                                                                                          |
+| Azure              |                                                                                          ❌ Not yet implemented.                                                                                          |
 
 ## 📡 Exporters
 | **Exporter** |          **Description**          |
 |--------------|:---------------------------------:|
 | Stdout       |   Print the metrics in Stdout.    |
 | JSON         | Write the metrics in a JSON file. |
 | Prometheus   |  Send the metrics to Prometheus.  |
```

### Comparing `tracarbon-0.7.0/pyproject.toml` & `tracarbon-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tracarbon"
 authors = ["Florian Valeye <fvaleye@github.com>"]
-version = "0.7.0"
+version = "0.7.1"
 description = "Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions."
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["energy", "sustainability", "energy-consumption", "electricity-consumption", "energy-efficiency", "carbon-footprint", "carbon-emissions"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
@@ -22,15 +22,16 @@
 psutil = "^5.9.4"
 ujson = "^5.8.0"
 msgpack = "^1.0.4"
 pydantic = ">=1.10.7,<3.0.0"
 typer = ">=0.7,<0.10"
 ec2-metadata = "^2.13.0"
 python-dotenv = ">=0.21,<1.1"
-datadog = {version = ">=0.44,<0.46", optional = true}
+asyncer = "^0.0.2"
+datadog = {version = ">=0.44,<0.47", optional = true}
 prometheus-client = {version = ">=0.16,<0.18", optional = true}
 kubernetes = {version = "^26.1.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.3"
 black = "^23.3.0"
 isort = "^5.12.0"
@@ -40,15 +41,15 @@
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.3.1"
 pytest-clarity = "^1.0.1"
 sphinx = "^7.0.1"
 pydata-sphinx-theme = "^0.13.3"
 toml = "^0.10.2"
 types-ujson = "^5.8.0"
-datadog = ">=0.44,<0.46"
+datadog = ">=0.44,<0.47"
 prometheus-client = ">=0.16,<0.18"
 types-requests = "^2.31.0"
 bandit = "^1.7.4"
 radon = "^6.0.1"
 types-aiofiles = "^23.1.0"
 kubernetes = "^26.1.0"
 autodoc_pydantic = "1.9.0"
```

### Comparing `tracarbon-0.7.0/tracarbon/builder.py` & `tracarbon-0.7.1/tracarbon/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from typing import Dict, Optional
 
 from pydantic import BaseModel
 
 from tracarbon.conf import TracarbonConfiguration
-from tracarbon.exporters import Exporter, MetricGenerator, MetricReport, StdoutExporter
+from tracarbon.exporters import Exporter, MetricReport, StdoutExporter
 from tracarbon.general_metrics import CarbonEmissionGenerator
 from tracarbon.locations import Country, Location
 
 
 class TracarbonReport(BaseModel):
     """
     Tracarbon report to store running statistics.
```

### Comparing `tracarbon-0.7.0/tracarbon/cli/__init__.py` & `tracarbon-0.7.1/tracarbon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/conf.py` & `tracarbon-0.7.1/tracarbon/conf.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/emissions/carbon_emissions.py` & `tracarbon-0.7.1/tracarbon/emissions/carbon_emissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 
 class CarbonUsageUnit(Enum):
     """
     Carbon usage unit.
     """
 
-    CO2_G_KWH = "co2g/kwh"
-    CO2_MG_KWH = "co2mg/kwh"
+    CO2_G = "co2g"
+    CO2_MG = "co2mg"
 
 
 class CarbonUsage(BaseModel):
     """
     Carbon Usage of the different types.
     """
 
     host_carbon_usage: float = 0.0
     cpu_carbon_usage: Optional[float] = None
     memory_carbon_usage: Optional[float] = None
     gpu_carbon_usage: Optional[float] = None
-    unit: CarbonUsageUnit = CarbonUsageUnit.CO2_G_KWH
+    unit: CarbonUsageUnit = CarbonUsageUnit.CO2_G
 
     def get_carbon_usage_on_type(self, usage_type: UsageType) -> Optional[float]:
         """
         Get the carbon usage based on the type.
 
         :param: usage_type: the type of energy to return
         :return: the carbon of the type
@@ -50,48 +50,42 @@
     def convert_unit(self, unit: CarbonUsageUnit) -> None:
         """
         Convert the carbon usage with the right carbon usage type.
 
         :param: unit: the carbon usage unit for the conversion
         """
         if self.unit != unit:
-            if (
-                unit == CarbonUsageUnit.CO2_G_KWH
-                and self.unit == CarbonUsageUnit.CO2_MG_KWH
-            ):
+            if unit == CarbonUsageUnit.CO2_G and self.unit == CarbonUsageUnit.CO2_MG:
                 self.host_carbon_usage = self.host_carbon_usage / 1000
                 self.cpu_carbon_usage = (
                     self.cpu_carbon_usage / 1000 if self.cpu_carbon_usage else None
                 )
                 self.memory_carbon_usage = (
                     self.memory_carbon_usage / 1000
                     if self.memory_carbon_usage
                     else None
                 )
                 self.gpu_carbon_usage = (
                     self.gpu_carbon_usage / 1000 if self.gpu_carbon_usage else None
                 )
-                self.unit = CarbonUsageUnit.CO2_G_KWH
-            elif (
-                unit == CarbonUsageUnit.CO2_MG_KWH
-                and self.unit == CarbonUsageUnit.CO2_G_KWH
-            ):
+                self.unit = CarbonUsageUnit.CO2_G
+            elif unit == CarbonUsageUnit.CO2_MG and self.unit == CarbonUsageUnit.CO2_G:
                 self.host_carbon_usage = self.host_carbon_usage * 1000
                 self.cpu_carbon_usage = (
                     self.cpu_carbon_usage * 1000 if self.cpu_carbon_usage else None
                 )
                 self.memory_carbon_usage = (
                     self.memory_carbon_usage * 1000
                     if self.memory_carbon_usage
                     else None
                 )
                 self.gpu_carbon_usage = (
                     self.gpu_carbon_usage * 1000 if self.gpu_carbon_usage else None
                 )
-                self.unit = CarbonUsageUnit.CO2_MG_KWH
+                self.unit = CarbonUsageUnit.CO2_MG
 
 
 class CarbonEmission(Sensor):
     """
     Carbon Metric sensor in watts per second to calculate the CO2g/kwh emitted.
     """
 
@@ -119,19 +113,19 @@
     async def get_co2_usage(self) -> CarbonUsage:
         """
         Run the Carbon Emission sensor and get the carbon emission generated.
 
         :return: the carbon usage.
         """
         energy_usage = await self.get_energy_usage()
-        logger.debug(f"Energy consumption run: {energy_usage}")
+        energy_usage.convert_unit(unit=EnergyUsageUnit.WATT)
+        logger.debug(f"Energy consumption run: {energy_usage}W")
 
         co2g_per_kwh = await self.location.get_latest_co2g_kwh()
         logger.debug(f"Carbon Emission of the location: {co2g_per_kwh}g CO2 eq/kWh")
-        energy_usage.convert_unit(unit=EnergyUsageUnit.WATT)
         host_carbon_usage = Power.co2g_from_watts_hour(
             Power.watts_to_watt_hours(
                 watts=energy_usage.host_energy_usage,
                 previous_energy_measurement_time=self.previous_energy_consumption_time,
             ),
             co2g_per_kwh=co2g_per_kwh,
         )
@@ -166,8 +160,9 @@
         return CarbonUsage(
             host_carbon_usage=host_carbon_usage,
             cpu_carbon_usage=cpu_carbon_usage if cpu_carbon_usage > 0 else None,
             memory_carbon_usage=memory_carbon_usage
             if memory_carbon_usage > 0
             else None,
             gpu_carbon_usage=gpu_carbon_usage if gpu_carbon_usage > 0 else None,
+            unit=CarbonUsageUnit.CO2_G,
         )
```

### Comparing `tracarbon-0.7.0/tracarbon/exceptions.py` & `tracarbon-0.7.1/tracarbon/exceptions.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/exporters/datadog_exporter.py` & `tracarbon-0.7.1/tracarbon/exporters/datadog_exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 
             :param metric_generator: the metric generators
             :return:
             """
             async for metric in metric_generator.generate():
                 metric_value = await metric.value()
                 if metric_value:
+                    await self.add_metric_to_report(metric=metric, value=metric_value)
                     metric_name = metric.format_name(
                         metric_prefix_name=self.metric_prefix_name
                     )
                     logger.info(
                         f"Sending metric[{metric_name}] with value [{metric_value}] and tags{metric.format_tags()} to Datadog."
                     )
                     self.stats.gauge(
                         metric_name, metric_value, tags=metric.format_tags()
                     )
-                    self.add_metric_to_report(metric=metric, value=metric_value)
 
         @classmethod
         def get_name(cls) -> str:
             """
             Get the name of the exporter.
 
             :return: the Exporter's name
```

### Comparing `tracarbon-0.7.0/tracarbon/exporters/exporter.py` & `tracarbon-0.7.1/tracarbon/exporters/exporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import sys
 from abc import ABCMeta, abstractmethod
+from datetime import datetime
 from threading import Event, Timer
 from typing import AsyncGenerator, Awaitable, Callable, Dict, List, Optional
 
+from asyncer import asyncify
 from loguru import logger
 from pydantic import BaseModel
 
 from tracarbon.hardwares.hardware import HardwareInfo
 from tracarbon.locations import Location
 
 
@@ -54,14 +56,16 @@
 class MetricReport(BaseModel):
     """
     MetricReport is a report of the generated metrics.
     """
 
     exporter_name: str
     metric: "Metric"
+    average_interval_in_seconds: Optional[float] = None
+    last_report_time: Optional[datetime] = None
     total: float = 0.0
     average: float = 0.0
     minimum: float = sys.float_info.max
     maximum: float = 0.0
     call_count: int = 0
 
     class Config:
@@ -145,34 +149,56 @@
         """
         Launch the exporter with all the metric generators.
         """
         for metric_generator in self.metric_generators:
             logger.debug(f"Running MetricGenerator[{metric_generator}].")
             await self.launch(metric_generator=metric_generator)
 
-    def add_metric_to_report(self, metric: "Metric", value: float) -> "MetricReport":
+    async def add_metric_to_report(
+        self, metric: "Metric", value: float
+    ) -> "MetricReport":
         """
-        Add the generated metric to the report.
+        Add the generated metric to the report asynchronously.
 
         :param metric: the metric to add
         :param value: the metric value to add
+        :return:
         """
-        if metric.name not in self.metric_report:
-            self.metric_report[metric.name] = MetricReport(
-                exporter_name=self.get_name(), metric=metric
-            )
-        metric_report = self.metric_report[metric.name]
-        metric_report.total += value
-        metric_report.call_count += 1
-        metric_report.average = metric_report.total / metric_report.call_count
-        if value < metric_report.minimum:
-            metric_report.minimum = value
-        if value > metric_report.maximum:
-            metric_report.maximum = value
-        return metric_report
+
+        def add_metric_to_report() -> MetricReport:
+            if metric.name not in self.metric_report:
+                self.metric_report[metric.name] = MetricReport(
+                    exporter_name=self.get_name(), metric=metric
+                )
+            metric_report = self.metric_report[metric.name]
+            now = datetime.now()
+            if metric_report.last_report_time:
+                time_difference_in_s = (
+                    now - metric_report.last_report_time
+                ).total_seconds()
+                metric_report.average_interval_in_seconds = (
+                    time_difference_in_s
+                    if not metric_report.average_interval_in_seconds
+                    else (
+                        metric_report.average_interval_in_seconds + time_difference_in_s
+                    )
+                    / 2
+                )
+
+            metric_report.last_report_time = now
+            metric_report.total += value
+            metric_report.call_count += 1
+            metric_report.average = metric_report.total / metric_report.call_count
+            if value < metric_report.minimum:
+                metric_report.minimum = value
+            if value > metric_report.maximum:
+                metric_report.maximum = value
+            return metric_report
+
+        return await asyncify(add_metric_to_report)()
 
     @classmethod
     @abstractmethod
     def get_name(cls) -> str:
         """
         Get the name of the exporter.
```

### Comparing `tracarbon-0.7.0/tracarbon/exporters/json_exporter.py` & `tracarbon-0.7.1/tracarbon/exporters/json_exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         Launch the Stdout exporter with the metrics.
 
         :param metric_generator: the metric generator
         """
         async for metric in metric_generator.generate():
             metric_value = await metric.value()
             if metric_value:
+                await self.add_metric_to_report(metric=metric, value=metric_value)
                 file_exists = os.path.isfile(self.path)
                 async with aiofiles.open(self.path, "a+") as file:
                     if file_exists:
                         await file.write(f",{os.linesep}")
                     else:
                         await file.write(f"[{os.linesep}")
                     await file.write(
@@ -53,15 +54,14 @@
                                 ),
                                 "metric_value": metric_value,
                                 "metric_tags": metric.format_tags(),
                             },
                             indent=self.indent,
                         )
                     )
-                self.add_metric_to_report(metric=metric, value=metric_value)
 
     @classmethod
     def get_name(cls) -> str:
         """
         Get the name of the exporter.
 
         :return: the Exporter's name
```

### Comparing `tracarbon-0.7.0/tracarbon/exporters/prometheus_exporter.py` & `tracarbon-0.7.1/tracarbon/exporters/prometheus_exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,21 +49,21 @@
                     self.prometheus_metrics[metric_name] = Gauge(
                         metric_name,
                         f"Tracarbon metric {metric_name}",
                         [tag.key for tag in metric.tags],
                     )
                 metric_value = await metric.value()
                 if metric_value:
+                    await self.add_metric_to_report(metric=metric, value=metric_value)
                     logger.info(
                         f"Sending metric[{metric_name}] with value [{metric_value}] and labels{metric.format_tags()} to Prometheus."
                     )
                     self.prometheus_metrics[metric_name].labels(
                         *[tag.value for tag in metric.tags]
                     ).set(metric_value)
-                    self.add_metric_to_report(metric=metric, value=metric_value)
 
         @classmethod
         def get_name(cls) -> str:
             """
             Get the name of the exporter.
 
             :return: the Exporter's name
```

### Comparing `tracarbon-0.7.0/tracarbon/exporters/stdout.py` & `tracarbon-0.7.1/tracarbon/exporters/stdout.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,18 @@
         Launch the Stdout exporter with the metrics.
 
         :param metric_generator: the metric generator
         """
         async for metric in metric_generator.generate():
             metric_value = await metric.value()
             if metric_value:
+                await self.add_metric_to_report(metric=metric, value=metric_value)
                 logger.info(
                     f"Metric name[{metric.format_name(metric_prefix_name=self.metric_prefix_name)}], value[{metric_value}], tags{metric.format_tags()}"
                 )
-                self.add_metric_to_report(metric=metric, value=metric_value)
 
     @classmethod
     def get_name(cls) -> str:
         """
         Get the name of the exporter.
 
         :return: the Exporter's name
```

### Comparing `tracarbon-0.7.0/tracarbon/general_metrics.py` & `tracarbon-0.7.1/tracarbon/general_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         async def generate(self) -> AsyncGenerator[Metric, None]:
             """
             Generate metrics for the carbon emission with Kubernetes.
 
             :return: an async generator of the metrics
             """
             carbon_usage = await self.carbon_emission.get_co2_usage()
-            carbon_usage.convert_unit(unit=CarbonUsageUnit.CO2_MG_KWH)
+            carbon_usage.convert_unit(unit=CarbonUsageUnit.CO2_MG)
 
             for pod in self.kubernetes.get_pods_usage():
                 for container in pod.containers:
 
                     async def get_cpu_pod_carbon_emission() -> Optional[float]:
                         """
                         Get the CPU carbon emission of the pod.
```

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/cloud_providers.py` & `tracarbon-0.7.1/tracarbon/hardwares/cloud_providers.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/containers.py` & `tracarbon-0.7.1/tracarbon/hardwares/containers.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/data/aws-instances.csv` & `tracarbon-0.7.1/tracarbon/hardwares/data/aws-instances.csv`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/energy.py` & `tracarbon-0.7.1/tracarbon/hardwares/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         else:
             time_difference_in_seconds = 1
         return watts * (time_difference_in_seconds / Power.SECONDS_TO_HOURS_FACTOR)
 
     @staticmethod
     def co2g_from_watts_hour(watts_hour: float, co2g_per_kwh: float) -> float:
         """
-        Calculate the CO2g generated using watt hours and the CO2g/kwh.
+        Calculate the CO2g generated using watt-hours and the CO2g/kwh.
 
         :return: the CO2g generated by the energy consumption
         """
         return (watts_hour / Power.WH_TO_KWH_FACTOR) * co2g_per_kwh
 
     @staticmethod
     def watts_from_microjoules(
```

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/gpu.py` & `tracarbon-0.7.1/tracarbon/hardwares/gpu.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/hardware.py` & `tracarbon-0.7.1/tracarbon/hardwares/hardware.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/rapl.py` & `tracarbon-0.7.1/tracarbon/hardwares/rapl.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/hardwares/sensors.py` & `tracarbon-0.7.1/tracarbon/hardwares/sensors.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/locations/country.py` & `tracarbon-0.7.1/tracarbon/locations/country.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json` & `tracarbon-0.7.1/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/locations/data/grid-emissions-factors-aws.csv` & `tracarbon-0.7.1/tracarbon/locations/data/grid-emissions-factors-aws.csv`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/tracarbon/locations/location.py` & `tracarbon-0.7.1/tracarbon/locations/location.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.7.0/PKG-INFO` & `tracarbon-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracarbon
-Version: 0.7.0
+Version: 0.7.1
 Summary: Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions.
 License: Apache-2.0
 Keywords: energy,sustainability,energy-consumption,electricity-consumption,energy-efficiency,carbon-footprint,carbon-emissions
 Author: Florian Valeye
 Author-email: fvaleye@github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: datadog
 Provides-Extra: kubernetes
 Provides-Extra: prometheus
 Requires-Dist: aiocache (>=0.12.1,<0.13.0)
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: datadog (>=0.44,<0.46) ; extra == "datadog"
+Requires-Dist: asyncer (>=0.0.2,<0.0.3)
+Requires-Dist: datadog (>=0.44,<0.47) ; extra == "datadog"
 Requires-Dist: ec2-metadata (>=2.13.0,<3.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0) ; extra == "kubernetes"
 Requires-Dist: loguru (>=0.6,<0.8)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: prometheus-client (>=0.16,<0.18) ; extra == "prometheus"
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<3.0.0)
@@ -59,25 +60,25 @@
 
 ```sh
 # Install one or more exporters from the list
 pip install 'tracarbon[datadog,prometheus,kubernetes]'
 ```
 
 ### 🔌 Devices: energy consumption
-| **Devices** |                                                                                                                                              **Description**                                                                                                                                              |
-|-------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-| Mac         |                                                                                                              ✅ Global energy consumption of your Mac (must be plugged into a wall adapter).                                                                                                               |
+| **Devices** |                                                                                                                                                           **Description**                                                                                                                                                            |
+|-------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| Mac         |                                                                                                                            ✅ Global energy consumption of your Mac (must be plugged into a wall adapter).                                                                                                                            |
 | Linux       | ⚠️ Only with [RAPL](https://web.eece.maine.edu/~vweaver/projects/rapl/). See [#1](https://github.com/fvaleye/tracarbon/issues/1). It works with containers on [Kubernetes](https://kubernetes.io/) using the [Metric API](https://kubernetes.io/docs/tasks/debug/debug-cluster/resource-metrics-pipeline/#metrics-api) if available. |
-| Windows     |                                                                                                           ❌ Not yet implemented. See [#184](https://github.com/hubblo-org/scaphandre/pull/184).                                                                                                           |
+| Windows     |                                                                                                                        ❌ Not yet implemented. See [#184](https://github.com/hubblo-org/scaphandre/pull/184).                                                                                                                         |
 
-| **Cloud Provider** |                                                                                                  **Description**                                                                                                  |
-|--------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-| AWS                | ✅ Use the hardware's usage with the EC2 instances carbon emissions datasets of [cloud-carbon-coefficients](https://github.com/cloud-carbon-footprint/cloud-carbon-coefficients/blob/main/data/aws-instances.csv). |
-| GCP                |                                                                                              ❌ Not yet implemented.                                                                                               |
-| Azure              |                                                                                              ❌ Not yet implemented.                                                                                               |
+| **Cloud Provider** |                                                                                             **Description**                                                                                              |
+|--------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| AWS                | ✅ Use the hardware's usage with the EC2 instances carbon emissions datasets of [cloud-carbon-coefficients](https://github.com/cloud-carbon-footprint/ccf-coefficients/blob/main/data/aws-instances.csv). |
+| GCP                |                                                                                          ❌ Not yet implemented.                                                                                          |
+| Azure              |                                                                                          ❌ Not yet implemented.                                                                                          |
 
 ## 📡 Exporters
 | **Exporter** |          **Description**          |
 |--------------|:---------------------------------:|
 | Stdout       |   Print the metrics in Stdout.    |
 | JSON         | Write the metrics in a JSON file. |
 | Prometheus   |  Send the metrics to Prometheus.  |
```

