# Comparing `tmp/indsl-6.6.0a1.tar.gz` & `tmp/indsl-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indsl-6.6.0a1.tar", max compression
+gzip compressed data, was "indsl-7.0.0.tar", max compression
```

## Comparing `indsl-6.6.0a1.tar` & `indsl-7.0.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0    11357 2023-07-12 12:40:01.134919 indsl-6.6.0a1/LICENSE
--rw-r--r--   0        0        0     9485 2023-07-12 12:40:01.134919 indsl-6.6.0a1/README.md
--rw-r--r--   0        0        0      568 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/__init__.py
--rw-r--r--   0        0        0       24 2023-07-12 12:40:38.231606 indsl-6.6.0a1/indsl/_version.py
--rw-r--r--   0        0        0     1110 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/__init__.py
--rw-r--r--   0        0        0     5161 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/completeness.py
--rw-r--r--   0        0        0     3881 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/datapoint_diff.py
--rw-r--r--   0        0        0     6673 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/gaps_identification.py
--rw-r--r--   0        0        0     7395 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/low_density_identification.py
--rw-r--r--   0        0        0    13211 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/outliers.py
--rw-r--r--   0        0        0     1739 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/rolling_stddev.py
--rw-r--r--   0        0        0      258 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/score/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/score/accuracy/__init__.py
--rw-r--r--   0        0        0     7964 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/score/base.py
--rw-r--r--   0        0        0       89 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/score/completeness/__init__.py
--rw-r--r--   0        0        0     4032 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/score/completeness/density.py
--rw-r--r--   0        0        0     5173 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/score/completeness/gap.py
--rw-r--r--   0        0        0     3911 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/value_decrease_indication.py
--rw-r--r--   0        0        0     3875 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/data_quality/value_decrease_indication_v1.py
--rw-r--r--   0        0        0      484 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/__init__.py
--rw-r--r--   0        0        0    12000 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/change_point_detector.py
--rw-r--r--   0        0        0    19019 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/cusum.py
--rw-r--r--   0        0        0     2595 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/drift_detector.py
--rw-r--r--   0        0        0     2249 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/drift_detector_v1.py
--rw-r--r--   0        0        0    22015 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/oscillation_detector.py
--rw-r--r--   0        0        0    10677 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/steady_state.py
--rw-r--r--   0        0        0     3414 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/unchanged_signal_detector.py
--rw-r--r--   0        0        0     2590 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/detect/utils.py
--rw-r--r--   0        0        0      265 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/drilling/__init__.py
--rw-r--r--   0        0        0     4302 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/drilling/flag_detection.py
--rw-r--r--   0        0        0      730 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/equipment/__init__.py
--rw-r--r--   0        0        0     7828 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/equipment/pump_parameters.py
--rw-r--r--   0        0        0     5837 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/equipment/valve_parameters.py
--rw-r--r--   0        0        0     6865 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/equipment/valve_parameters_.py
--rw-r--r--   0        0        0     9598 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/equipment/volume_vessel.py
--rw-r--r--   0        0        0      506 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/exceptions.py
--rw-r--r--   0        0        0      196 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/filter/__init__.py
--rw-r--r--   0        0        0     2102 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/filter/simple_filters.py
--rw-r--r--   0        0        0     2881 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/filter/wavelet_filter.py
--rw-r--r--   0        0        0     2786 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/filter/wavelet_filter_v1.py
--rw-r--r--   0        0        0      151 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/fluid_dynamics/__init__.py
--rw-r--r--   0        0        0      973 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/fluid_dynamics/dimensionless.py
--rw-r--r--   0        0        0      906 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/fluid_dynamics/friction.py
--rw-r--r--   0        0        0      214 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/forecast/__init__.py
--rw-r--r--   0        0        0     4624 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/forecast/arma_predictor.py
--rw-r--r--   0        0        0     5254 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/forecast/holt_winters_predictor.py
--rw-r--r--   0        0        0      315 2023-07-12 12:40:01.338920 indsl-6.6.0a1/indsl/not_listed_operations/__init__.py
--rw-r--r--   0        0        0     3482 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/not_listed_operations/deprecated_functions.py
--rw-r--r--   0        0        0      398 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/not_listed_operations/utils.py
--rw-r--r--   0        0        0      510 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/not_listed_operations/versioning_test.py
--rw-r--r--   0        0        0      388 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/not_listed_operations/versioning_test_v1.py
--rw-r--r--   0        0        0      502 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/__init__.py
--rw-r--r--   0        0        0     1378 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/engineering_calcs.py
--rw-r--r--   0        0        0     6667 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/gas_density_calcs.py
--rw-r--r--   0        0        0     4479 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/live_fluid_properties.py
--rw-r--r--   0        0        0     5783 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/shut_in_detector.py
--rw-r--r--   0        0        0     3142 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/shut_in_variables.py
--rw-r--r--   0        0        0     3087 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/tab_fp_identifier.json
--rw-r--r--   0        0        0     3353 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/oil_and_gas/well_prod_status.py
--rw-r--r--   0        0        0      129 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/regression/__init__.py
--rw-r--r--   0        0        0     2470 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/regression/polynomial.py
--rw-r--r--   0        0        0     4144 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/README.md
--rw-r--r--   0        0        0      313 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/__init__.py
--rw-r--r--   0        0        0     1113 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/auto_align.py
--rw-r--r--   0        0        0     3693 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/group_by.py
--rw-r--r--   0        0        0     4763 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/interpolate.py
--rw-r--r--   0        0        0     5381 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/interpolate_v1.py
--rw-r--r--   0        0        0     6853 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/reindex.py
--rw-r--r--   0        0        0     7911 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/reindex_v1.py
--rw-r--r--   0        0        0     8543 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/resample.py
--rw-r--r--   0        0        0     8670 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/resample/resample_v1.py
--rw-r--r--   0        0        0      420 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/signals/__init__.py
--rw-r--r--   0        0        0    26910 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/signals/generator.py
--rw-r--r--   0        0        0    12149 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/signals/noise.py
--rw-r--r--   0        0        0      955 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/signals/polynomial.py
--rw-r--r--   0        0        0     8149 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/README.md
--rw-r--r--   0        0        0      474 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/__init__.py
--rw-r--r--   0        0        0     2691 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/alma.py
--rw-r--r--   0        0        0     1186 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/arma_smoother.py
--rw-r--r--   0        0        0     1892 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/butterworth.py
--rw-r--r--   0        0        0     2227 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/butterworth_v1.py
--rw-r--r--   0        0        0     2102 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/chebyshev.py
--rw-r--r--   0        0        0     5736 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/eweight_ma.py
--rw-r--r--   0        0        0     5899 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/eweight_ma_v1.py
--rw-r--r--   0        0        0    73573 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/img/ma_min_periods1.png
--rw-r--r--   0        0        0    63892 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/img/ma_min_periods5.png
--rw-r--r--   0        0        0    52202 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/img/zoom_min_periods5.png
--rw-r--r--   0        0        0     3007 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/lweight_ma.py
--rw-r--r--   0        0        0     3053 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/lweight_ma_v1.py
--rw-r--r--   0        0        0      730 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/moving_averages.md
--rw-r--r--   0        0        0     2856 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/savitzky_golay.py
--rw-r--r--   0        0        0     1275 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/simple_ma.py
--rw-r--r--   0        0        0     1420 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/smooth/simple_ma_v1.py
--rw-r--r--   0        0        0      494 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/statistics/README.md
--rw-r--r--   0        0        0      231 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/statistics/__init__.py
--rw-r--r--   0        0        0     2313 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/statistics/confidence.py
--rw-r--r--   0        0        0     1948 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/statistics/correlation.py
--rw-r--r--   0        0        0    26141 2023-07-12 12:40:01.342920 indsl-6.6.0a1/indsl/statistics/img/csaps_vs_scipy.png
--rw-r--r--   0        0        0    26153 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/statistics/img/dbscan_principle.png
--rw-r--r--   0        0        0    69055 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/statistics/img/input_timeseries.png
--rw-r--r--   0        0        0    69329 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/statistics/img/output_function.png
--rw-r--r--   0        0        0   102644 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/statistics/img/process_function.png
--rw-r--r--   0        0        0     4926 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/statistics/outliers.md
--rw-r--r--   0        0        0    13787 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/statistics/outliers.py
--rw-r--r--   0        0        0    13229 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/statistics/outliers_v1.py
--rw-r--r--   0        0        0       78 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/sustainability/__init__.py
--rw-r--r--   0        0        0     5009 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/sustainability/co2_emissions_calculations.py
--rw-r--r--   0        0        0     1558 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/logarithmic_functions.py
--rw-r--r--   0        0        0     3000 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/logical_operations.py
--rw-r--r--   0        0        0     7912 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/numerical_calculus.py
--rw-r--r--   0        0        0     2573 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/numerical_calculus_v1.py
--rw-r--r--   0        0        0     5479 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/operators.py
--rw-r--r--   0        0        0     3610 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/trigonometric_functions.py
--rw-r--r--   0        0        0    15026 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/ts_utils.py
--rw-r--r--   0        0        0    18839 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/ts_utils/utility_functions.py
--rw-r--r--   0        0        0      773 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/type_check.py
--rw-r--r--   0        0        0     1653 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/validations.py
--rw-r--r--   0        0        0     4843 2023-07-12 12:40:01.346920 indsl-6.6.0a1/indsl/versioning.py
--rw-r--r--   0        0        0     3120 2023-07-12 12:40:38.147605 indsl-6.6.0a1/pyproject.toml
--rw-r--r--   0        0        0    10839 1970-01-01 00:00:00.000000 indsl-6.6.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 16:04:03.390569 indsl-7.0.0/LICENSE
+-rw-r--r--   0        0        0     9485 2023-07-17 16:04:03.390569 indsl-7.0.0/README.md
+-rw-r--r--   0        0        0      568 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-17 16:04:37.690636 indsl-7.0.0/indsl/_version.py
+-rw-r--r--   0        0        0     1110 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/completeness.py
+-rw-r--r--   0        0        0     3881 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/datapoint_diff.py
+-rw-r--r--   0        0        0     6673 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/gaps_identification.py
+-rw-r--r--   0        0        0     7395 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/low_density_identification.py
+-rw-r--r--   0        0        0    13211 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/outliers.py
+-rw-r--r--   0        0        0     1739 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/rolling_stddev.py
+-rw-r--r--   0        0        0      258 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/score/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/score/accuracy/__init__.py
+-rw-r--r--   0        0        0     7964 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/score/base.py
+-rw-r--r--   0        0        0       89 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/score/completeness/__init__.py
+-rw-r--r--   0        0        0     4032 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/score/completeness/density.py
+-rw-r--r--   0        0        0     5173 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/score/completeness/gap.py
+-rw-r--r--   0        0        0     3911 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/value_decrease_indication.py
+-rw-r--r--   0        0        0     3875 2023-07-17 16:04:03.606567 indsl-7.0.0/indsl/data_quality/value_decrease_indication_v1.py
+-rw-r--r--   0        0        0      484 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/__init__.py
+-rw-r--r--   0        0        0    12000 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/change_point_detector.py
+-rw-r--r--   0        0        0    19019 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/cusum.py
+-rw-r--r--   0        0        0     2595 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/drift_detector.py
+-rw-r--r--   0        0        0     2249 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/drift_detector_v1.py
+-rw-r--r--   0        0        0    24501 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/oscillation_detector.py
+-rw-r--r--   0        0        0    10677 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/steady_state.py
+-rw-r--r--   0        0        0     3414 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/unchanged_signal_detector.py
+-rw-r--r--   0        0        0     2590 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/detect/utils.py
+-rw-r--r--   0        0        0      265 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/drilling/__init__.py
+-rw-r--r--   0        0        0     4302 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/drilling/flag_detection.py
+-rw-r--r--   0        0        0      730 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/equipment/__init__.py
+-rw-r--r--   0        0        0     7828 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/equipment/pump_parameters.py
+-rw-r--r--   0        0        0     5837 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/equipment/valve_parameters.py
+-rw-r--r--   0        0        0     6865 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/equipment/valve_parameters_.py
+-rw-r--r--   0        0        0     9598 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/equipment/volume_vessel.py
+-rw-r--r--   0        0        0      506 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/exceptions.py
+-rw-r--r--   0        0        0      196 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/filter/__init__.py
+-rw-r--r--   0        0        0     2102 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/filter/simple_filters.py
+-rw-r--r--   0        0        0     2881 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/filter/wavelet_filter.py
+-rw-r--r--   0        0        0     2786 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/filter/wavelet_filter_v1.py
+-rw-r--r--   0        0        0      151 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/fluid_dynamics/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/fluid_dynamics/dimensionless.py
+-rw-r--r--   0        0        0      906 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/fluid_dynamics/friction.py
+-rw-r--r--   0        0        0      214 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/forecast/__init__.py
+-rw-r--r--   0        0        0     4624 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/forecast/arma_predictor.py
+-rw-r--r--   0        0        0     5254 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/forecast/holt_winters_predictor.py
+-rw-r--r--   0        0        0      315 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/not_listed_operations/__init__.py
+-rw-r--r--   0        0        0     3482 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/not_listed_operations/deprecated_functions.py
+-rw-r--r--   0        0        0      398 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/not_listed_operations/utils.py
+-rw-r--r--   0        0        0      510 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/not_listed_operations/versioning_test.py
+-rw-r--r--   0        0        0      388 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/not_listed_operations/versioning_test_v1.py
+-rw-r--r--   0        0        0      502 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/__init__.py
+-rw-r--r--   0        0        0     1378 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/engineering_calcs.py
+-rw-r--r--   0        0        0     6667 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/gas_density_calcs.py
+-rw-r--r--   0        0        0     4479 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/live_fluid_properties.py
+-rw-r--r--   0        0        0     5783 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/shut_in_detector.py
+-rw-r--r--   0        0        0     3142 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/shut_in_variables.py
+-rw-r--r--   0        0        0     3087 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/tab_fp_identifier.json
+-rw-r--r--   0        0        0     3353 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/oil_and_gas/well_prod_status.py
+-rw-r--r--   0        0        0      129 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/regression/__init__.py
+-rw-r--r--   0        0        0     2470 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/regression/polynomial.py
+-rw-r--r--   0        0        0     4144 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/README.md
+-rw-r--r--   0        0        0      313 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/__init__.py
+-rw-r--r--   0        0        0     1113 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/auto_align.py
+-rw-r--r--   0        0        0     3693 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/group_by.py
+-rw-r--r--   0        0        0     4763 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/interpolate.py
+-rw-r--r--   0        0        0     5381 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/interpolate_v1.py
+-rw-r--r--   0        0        0     6853 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/reindex.py
+-rw-r--r--   0        0        0     7911 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/reindex_v1.py
+-rw-r--r--   0        0        0     8543 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/resample.py
+-rw-r--r--   0        0        0     8670 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/resample/resample_v1.py
+-rw-r--r--   0        0        0      420 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/signals/__init__.py
+-rw-r--r--   0        0        0    26910 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/signals/generator.py
+-rw-r--r--   0        0        0    12149 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/signals/noise.py
+-rw-r--r--   0        0        0      955 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/signals/polynomial.py
+-rw-r--r--   0        0        0     8149 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/README.md
+-rw-r--r--   0        0        0      474 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/__init__.py
+-rw-r--r--   0        0        0     2691 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/alma.py
+-rw-r--r--   0        0        0     1186 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/arma_smoother.py
+-rw-r--r--   0        0        0     1892 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/butterworth.py
+-rw-r--r--   0        0        0     2227 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/butterworth_v1.py
+-rw-r--r--   0        0        0     2102 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/chebyshev.py
+-rw-r--r--   0        0        0     5736 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/eweight_ma.py
+-rw-r--r--   0        0        0     5899 2023-07-17 16:04:03.610567 indsl-7.0.0/indsl/smooth/eweight_ma_v1.py
+-rw-r--r--   0        0        0    73573 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/img/ma_min_periods1.png
+-rw-r--r--   0        0        0    63892 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/img/ma_min_periods5.png
+-rw-r--r--   0        0        0    52202 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/img/zoom_min_periods5.png
+-rw-r--r--   0        0        0     3007 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/lweight_ma.py
+-rw-r--r--   0        0        0     3053 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/lweight_ma_v1.py
+-rw-r--r--   0        0        0      730 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/moving_averages.md
+-rw-r--r--   0        0        0     2856 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/savitzky_golay.py
+-rw-r--r--   0        0        0     1275 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/simple_ma.py
+-rw-r--r--   0        0        0     1420 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/smooth/simple_ma_v1.py
+-rw-r--r--   0        0        0      494 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/README.md
+-rw-r--r--   0        0        0      231 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/__init__.py
+-rw-r--r--   0        0        0     2313 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/confidence.py
+-rw-r--r--   0        0        0     1948 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/correlation.py
+-rw-r--r--   0        0        0    26141 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/img/csaps_vs_scipy.png
+-rw-r--r--   0        0        0    26153 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/img/dbscan_principle.png
+-rw-r--r--   0        0        0    69055 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/img/input_timeseries.png
+-rw-r--r--   0        0        0    69329 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/img/output_function.png
+-rw-r--r--   0        0        0   102644 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/img/process_function.png
+-rw-r--r--   0        0        0     4926 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/outliers.md
+-rw-r--r--   0        0        0    13787 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/outliers.py
+-rw-r--r--   0        0        0    13229 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/statistics/outliers_v1.py
+-rw-r--r--   0        0        0       78 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/sustainability/__init__.py
+-rw-r--r--   0        0        0     5009 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/sustainability/co2_emissions_calculations.py
+-rw-r--r--   0        0        0     1558 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/ts_utils/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/ts_utils/logarithmic_functions.py
+-rw-r--r--   0        0        0     3000 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/ts_utils/logical_operations.py
+-rw-r--r--   0        0        0     7912 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/ts_utils/numerical_calculus.py
+-rw-r--r--   0        0        0     2573 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/ts_utils/numerical_calculus_v1.py
+-rw-r--r--   0        0        0     5479 2023-07-17 16:04:03.614567 indsl-7.0.0/indsl/ts_utils/operators.py
+-rw-r--r--   0        0        0     3610 2023-07-17 16:04:03.618567 indsl-7.0.0/indsl/ts_utils/trigonometric_functions.py
+-rw-r--r--   0        0        0    15026 2023-07-17 16:04:03.618567 indsl-7.0.0/indsl/ts_utils/ts_utils.py
+-rw-r--r--   0        0        0    18839 2023-07-17 16:04:03.618567 indsl-7.0.0/indsl/ts_utils/utility_functions.py
+-rw-r--r--   0        0        0      773 2023-07-17 16:04:03.618567 indsl-7.0.0/indsl/type_check.py
+-rw-r--r--   0        0        0     1653 2023-07-17 16:04:03.618567 indsl-7.0.0/indsl/validations.py
+-rw-r--r--   0        0        0     4843 2023-07-17 16:04:03.618567 indsl-7.0.0/indsl/versioning.py
+-rw-r--r--   0        0        0     3118 2023-07-17 16:04:37.626635 indsl-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10837 1970-01-01 00:00:00.000000 indsl-7.0.0/PKG-INFO
```

### Comparing `indsl-6.6.0a1/LICENSE` & `indsl-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/README.md` & `indsl-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/__init__.py` & `indsl-7.0.0/indsl/__init__.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/__init__.py` & `indsl-7.0.0/indsl/data_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/completeness.py` & `indsl-7.0.0/indsl/data_quality/completeness.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/datapoint_diff.py` & `indsl-7.0.0/indsl/data_quality/datapoint_diff.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/gaps_identification.py` & `indsl-7.0.0/indsl/data_quality/gaps_identification.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/low_density_identification.py` & `indsl-7.0.0/indsl/data_quality/low_density_identification.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/outliers.py` & `indsl-7.0.0/indsl/data_quality/outliers.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/rolling_stddev.py` & `indsl-7.0.0/indsl/data_quality/rolling_stddev.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/score/base.py` & `indsl-7.0.0/indsl/data_quality/score/base.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/score/completeness/density.py` & `indsl-7.0.0/indsl/data_quality/score/completeness/density.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/score/completeness/gap.py` & `indsl-7.0.0/indsl/data_quality/score/completeness/gap.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/value_decrease_indication.py` & `indsl-7.0.0/indsl/data_quality/value_decrease_indication.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/data_quality/value_decrease_indication_v1.py` & `indsl-7.0.0/indsl/data_quality/value_decrease_indication_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/detect/change_point_detector.py` & `indsl-7.0.0/indsl/detect/change_point_detector.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/detect/cusum.py` & `indsl-7.0.0/indsl/detect/cusum.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/detect/drift_detector.py` & `indsl-7.0.0/indsl/detect/drift_detector.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/detect/drift_detector_v1.py` & `indsl-7.0.0/indsl/detect/drift_detector_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/detect/oscillation_detector.py` & `indsl-7.0.0/indsl/detect/oscillation_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,78 @@
 from scipy.signal import argrelextrema, lfilter
 
 from indsl.exceptions import UserTypeError, UserValueError
 from indsl.type_check import check_types
 
 
 @check_types
-def oscillation_detector(data: pd.Series, order: int = 4, threshold: float = 0.2, visualize: bool = False) -> pd.Series:
+def oscillation_detector_plot(data: pd.Series, order: int = 4, threshold: float = 0.2) -> pd.Series:
+    """Oscillations.
+
+    This function identifies if a signal contains one or more oscillatory components and plots the result. It is based on the paper by Sharma et al. [#]_.
+    The method uses Linear Predictive Coding (LPC) and is implemented as a 3 step process:
+
+        1. Estimate the LPC coefficients from the prediction polynomial. These are used to estimate a fit to the
+           data.
+        2. Estimate the roots of the LPC coefficients.
+        3. Estimate the distance of each root to the unit circle in the complex plane.
+
+    If the distance of any root is close to the unit circle (less than 0.2) the signal is considered to have an
+    oscillatory component
+
+
+    Args:
+        data: Time series
+        order: Polynomial order.
+            Order of the prediction polynomial. Defaults to 4.
+        threshold: Threshold.
+            Maximum distance of a root to the unit circle for which the signal is considered to have an oscillatory
+            component. Defaults to 0.2
+
+    Returns:
+        pd.Series: Oscillation region.
+            Regions where oscillations were detected. Ocillations detected =1, no detection =0.
+
+
+    Warnings:
+        Large variations in sampling time may affect the proficiency of the algorithm. The algorithm works best on time series with
+        uniform sampling frequency. If non-uniformly sampled, you can use a resampling method to fill the missing
+        data.
+
+    Raises:
+        RuntimeError: Length of interpolated data does not match predicted data.
+
+    References:
+        .. [#] Sharma et al. "Automatic signal detection and quantification in process control loops using linear
+               predictive coding." Eng. Sc. & Tech. an Intnl. Journal 2020.
+    """
+    (
+        delta_t,
+        data_interp,
+        data_predicted,
+        detected,
+        data_freqs,
+        time_interp,
+        amplitude,
+        roots,
+        distances,
+    ) = _oscillation_detector(data, order, threshold)
+
+    # If oscillations detected find amplitude of peak frequencies, and plot if requested.
+    if detected:
+        residuals = data_interp - data_predicted
+        peaks = _peak_freq_components(residuals, data_interp, delta_t, visualize=True)
+    else:
+        return pd.Series(index=data_freqs, data=np.zeros(len(data_freqs)))
+
+    return _oscillation_region(data_freqs, peaks)
+
+
+@check_types
+def oscillation_detector(data: pd.Series, order: int = 4, threshold: float = 0.2) -> pd.Series:
     """Oscillations.
 
     This function identifies if a signal contains one or more oscillatory components. It is based on the paper by Sharma et al. [#]_.
     The method uses Linear Predictive Coding (LPC) and is implemented as a 3 step process:
 
         1. Estimate the LPC coefficients from the prediction polynomial. These are used to estimate a fit to the
            data.
@@ -36,17 +99,14 @@
     Args:
         data: Time series
         order: Polynomial order.
             Order of the prediction polynomial. Defaults to 4.
         threshold: Threshold.
             Maximum distance of a root to the unit circle for which the signal is considered to have an oscillatory
             component. Defaults to 0.2
-        visualize (boolean): Visualize
-            True - Plots the results
-            False (default) - No plot is generated
 
     Returns:
         pd.Series: Oscillation region.
             Regions where oscillations were detected. Ocillations detected =1, no detection =0.
 
 
     Warnings:
@@ -72,23 +132,28 @@
         roots,
         distances,
     ) = _oscillation_detector(data, order, threshold)
 
     # If oscillations detected find amplitude of peak frequencies, and plot if requested.
     if detected:
         residuals = data_interp - data_predicted
-        peaks = _peak_freq_components(residuals, data_interp, delta_t, visualize)
+        peaks = _peak_freq_components(residuals, data_interp, delta_t, visualize=False)
+    else:
+        return pd.Series(index=data_freqs, data=np.zeros(len(data_freqs)))
+
+    return _oscillation_region(data_freqs, peaks)
+
 
+def _oscillation_region(data_freqs: np.ndarray, peaks: tuple) -> pd.Series:
     # obtain the output pd.Series where the oscillation is detected
     detection = np.zeros(len(data_freqs))
     for freq in peaks[0]["frequencies"]:
         detection[np.where(data_freqs == freq)] = 1
 
-    oscillation_region = pd.Series(index=data_freqs, data=detection)
-    return oscillation_region
+    return pd.Series(index=data_freqs, data=detection)
 
 
 def _oscillation_detector(data, order, threshold):
     # This is a helper function to avoid repeated code which is being used by two functions
     time = np.array([item.value / 1e9 for item in data.index])
     data_ = data.to_numpy()
```

### Comparing `indsl-6.6.0a1/indsl/detect/steady_state.py` & `indsl-7.0.0/indsl/detect/steady_state.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/detect/unchanged_signal_detector.py` & `indsl-7.0.0/indsl/detect/unchanged_signal_detector.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/detect/utils.py` & `indsl-7.0.0/indsl/detect/utils.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/drilling/flag_detection.py` & `indsl-7.0.0/indsl/drilling/flag_detection.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/equipment/__init__.py` & `indsl-7.0.0/indsl/equipment/__init__.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/equipment/pump_parameters.py` & `indsl-7.0.0/indsl/equipment/pump_parameters.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/equipment/valve_parameters.py` & `indsl-7.0.0/indsl/equipment/valve_parameters.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/equipment/valve_parameters_.py` & `indsl-7.0.0/indsl/equipment/valve_parameters_.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/equipment/volume_vessel.py` & `indsl-7.0.0/indsl/equipment/volume_vessel.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/filter/simple_filters.py` & `indsl-7.0.0/indsl/filter/simple_filters.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/filter/wavelet_filter.py` & `indsl-7.0.0/indsl/filter/wavelet_filter.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/filter/wavelet_filter_v1.py` & `indsl-7.0.0/indsl/filter/wavelet_filter_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/fluid_dynamics/dimensionless.py` & `indsl-7.0.0/indsl/fluid_dynamics/dimensionless.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/fluid_dynamics/friction.py` & `indsl-7.0.0/indsl/fluid_dynamics/friction.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/forecast/arma_predictor.py` & `indsl-7.0.0/indsl/forecast/arma_predictor.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/forecast/holt_winters_predictor.py` & `indsl-7.0.0/indsl/forecast/holt_winters_predictor.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/not_listed_operations/deprecated_functions.py` & `indsl-7.0.0/indsl/not_listed_operations/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/oil_and_gas/engineering_calcs.py` & `indsl-7.0.0/indsl/oil_and_gas/engineering_calcs.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/oil_and_gas/gas_density_calcs.py` & `indsl-7.0.0/indsl/oil_and_gas/gas_density_calcs.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/oil_and_gas/live_fluid_properties.py` & `indsl-7.0.0/indsl/oil_and_gas/live_fluid_properties.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/oil_and_gas/shut_in_detector.py` & `indsl-7.0.0/indsl/oil_and_gas/shut_in_detector.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/oil_and_gas/shut_in_variables.py` & `indsl-7.0.0/indsl/oil_and_gas/shut_in_variables.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/oil_and_gas/tab_fp_identifier.json` & `indsl-7.0.0/indsl/oil_and_gas/tab_fp_identifier.json`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/oil_and_gas/well_prod_status.py` & `indsl-7.0.0/indsl/oil_and_gas/well_prod_status.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/regression/polynomial.py` & `indsl-7.0.0/indsl/regression/polynomial.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/README.md` & `indsl-7.0.0/indsl/resample/README.md`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/auto_align.py` & `indsl-7.0.0/indsl/resample/auto_align.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/group_by.py` & `indsl-7.0.0/indsl/resample/group_by.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/interpolate.py` & `indsl-7.0.0/indsl/resample/interpolate.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/interpolate_v1.py` & `indsl-7.0.0/indsl/resample/interpolate_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/reindex.py` & `indsl-7.0.0/indsl/resample/reindex.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/reindex_v1.py` & `indsl-7.0.0/indsl/resample/reindex_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/resample.py` & `indsl-7.0.0/indsl/resample/resample.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/resample/resample_v1.py` & `indsl-7.0.0/indsl/resample/resample_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/signals/generator.py` & `indsl-7.0.0/indsl/signals/generator.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/signals/noise.py` & `indsl-7.0.0/indsl/signals/noise.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/signals/polynomial.py` & `indsl-7.0.0/indsl/signals/polynomial.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/README.md` & `indsl-7.0.0/indsl/smooth/README.md`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/alma.py` & `indsl-7.0.0/indsl/smooth/alma.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/arma_smoother.py` & `indsl-7.0.0/indsl/smooth/arma_smoother.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/butterworth.py` & `indsl-7.0.0/indsl/smooth/butterworth.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/butterworth_v1.py` & `indsl-7.0.0/indsl/smooth/butterworth_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/chebyshev.py` & `indsl-7.0.0/indsl/smooth/chebyshev.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/eweight_ma.py` & `indsl-7.0.0/indsl/smooth/eweight_ma.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/eweight_ma_v1.py` & `indsl-7.0.0/indsl/smooth/eweight_ma_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/img/ma_min_periods1.png` & `indsl-7.0.0/indsl/smooth/img/ma_min_periods1.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/img/ma_min_periods5.png` & `indsl-7.0.0/indsl/smooth/img/ma_min_periods5.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/img/zoom_min_periods5.png` & `indsl-7.0.0/indsl/smooth/img/zoom_min_periods5.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/lweight_ma.py` & `indsl-7.0.0/indsl/smooth/lweight_ma.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/lweight_ma_v1.py` & `indsl-7.0.0/indsl/smooth/lweight_ma_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/moving_averages.md` & `indsl-7.0.0/indsl/smooth/moving_averages.md`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/savitzky_golay.py` & `indsl-7.0.0/indsl/smooth/savitzky_golay.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/simple_ma.py` & `indsl-7.0.0/indsl/smooth/simple_ma.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/smooth/simple_ma_v1.py` & `indsl-7.0.0/indsl/smooth/simple_ma_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/confidence.py` & `indsl-7.0.0/indsl/statistics/confidence.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/correlation.py` & `indsl-7.0.0/indsl/statistics/correlation.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/img/csaps_vs_scipy.png` & `indsl-7.0.0/indsl/statistics/img/csaps_vs_scipy.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/img/dbscan_principle.png` & `indsl-7.0.0/indsl/statistics/img/dbscan_principle.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/img/input_timeseries.png` & `indsl-7.0.0/indsl/statistics/img/input_timeseries.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/img/output_function.png` & `indsl-7.0.0/indsl/statistics/img/output_function.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/img/process_function.png` & `indsl-7.0.0/indsl/statistics/img/process_function.png`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/outliers.md` & `indsl-7.0.0/indsl/statistics/outliers.md`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/outliers.py` & `indsl-7.0.0/indsl/statistics/outliers.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/statistics/outliers_v1.py` & `indsl-7.0.0/indsl/statistics/outliers_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/sustainability/co2_emissions_calculations.py` & `indsl-7.0.0/indsl/sustainability/co2_emissions_calculations.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/__init__.py` & `indsl-7.0.0/indsl/ts_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/logarithmic_functions.py` & `indsl-7.0.0/indsl/ts_utils/logarithmic_functions.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/logical_operations.py` & `indsl-7.0.0/indsl/ts_utils/logical_operations.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/numerical_calculus.py` & `indsl-7.0.0/indsl/ts_utils/numerical_calculus.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/numerical_calculus_v1.py` & `indsl-7.0.0/indsl/ts_utils/numerical_calculus_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/operators.py` & `indsl-7.0.0/indsl/ts_utils/operators.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/trigonometric_functions.py` & `indsl-7.0.0/indsl/ts_utils/trigonometric_functions.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/ts_utils.py` & `indsl-7.0.0/indsl/ts_utils/ts_utils.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/ts_utils/utility_functions.py` & `indsl-7.0.0/indsl/ts_utils/utility_functions.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/type_check.py` & `indsl-7.0.0/indsl/type_check.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/validations.py` & `indsl-7.0.0/indsl/validations.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/indsl/versioning.py` & `indsl-7.0.0/indsl/versioning.py`

 * *Files identical despite different names*

### Comparing `indsl-6.6.0a1/pyproject.toml` & `indsl-7.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "indsl"
-version = "6.6.0a1"
+version = "7.0.0"
 description = "Industrial Data Science Library by Cognite"
 authors = ["Cognite"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/indsl"
 documentation = "https://indsl.docs.cognite.com"
 homepage = "https://indsl.docs.cognite.com"
```

### Comparing `indsl-6.6.0a1/PKG-INFO` & `indsl-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indsl
-Version: 6.6.0a1
+Version: 7.0.0
 Summary: Industrial Data Science Library by Cognite
 Home-page: https://indsl.docs.cognite.com
 License: Apache-2.0
 Author: Cognite
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: indsl Version: 6.6.0a1 Summary: Industrial Data
+Metadata-Version: 2.1 Name: indsl Version: 7.0.0 Summary: Industrial Data
 Science Library by Cognite Home-page: https://indsl.docs.cognite.com License:
 Apache-2.0 Author: Cognite Requires-Python: >=3.8,<3.12 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Requires-Dist: PyWavelets (>=1.2.0,<2.0.0)
```

