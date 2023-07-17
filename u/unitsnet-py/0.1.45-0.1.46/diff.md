# Comparing `tmp/unitsnet-py-0.1.45.tar.gz` & `tmp/unitsnet-py-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitsnet-py-0.1.45.tar", last modified: Wed Jul 12 13:17:55 2023, max compression
+gzip compressed data, was "unitsnet-py-0.1.46.tar", last modified: Mon Jul 17 18:41:41 2023, max compression
```

## Comparing `unitsnet-py-0.1.45.tar` & `unitsnet-py-0.1.46.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:55.953173 unitsnet-py-0.1.45/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 13:17:04.000000 unitsnet-py-0.1.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-12 13:17:55.949173 unitsnet-py-0.1.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27203 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-12 13:17:49.000000 unitsnet-py-0.1.45/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:17:55.953173 unitsnet-py-0.1.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 13:17:50.000000 unitsnet-py-0.1.45/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:55.917172 unitsnet-py-0.1.45/unitsnet_py/
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:55.949173 unitsnet-py-0.1.45/unitsnet_py/units/
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/amount_of_substance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/amplitude_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/apparent_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/apparent_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/area.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/area_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/area_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/brake_specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/capacitance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/coefficient_of_thermal_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/compressibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/density.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/dynamic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_admittance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_conductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_current_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_current_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_inductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_potential_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_potential_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_potential_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-12 13:17:46.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_resistivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/electric_surface_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/energy_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/force.py
--rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/force_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/force_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/fuel_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/heat_transfer_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/impulse.py
--rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/information.py
--rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/irradiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/jerk.py
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/kinematic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/leak_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/linear_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/linear_power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/luminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/luminous_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/luminous_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/magnetic_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/magnetic_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/mass_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/mass_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/mass_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/mass_fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/mass_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/molar_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/molar_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/molar_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/molar_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/molarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/permittivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/porous_medium_permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/power.py
--rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/power_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)    34511 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/pressure_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/ratio_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/reactive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/reactive_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/reciprocal_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/reciprocal_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/relative_humidity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/rotational_acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/rotational_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/rotational_stiffness.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/rotational_stiffness_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-12 13:17:47.000000 unitsnet-py-0.1.45/unitsnet_py/units/solid_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/specific_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/specific_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/specific_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/specific_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/standard_volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/temperature_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/temperature_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/temperature_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/thermal_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/thermal_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/torque_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/turbidity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/vitamin_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/volume_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/volume_flow_per_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/volume_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/volumetric_heat_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-12 13:17:48.000000 unitsnet-py-0.1.45/unitsnet_py/units/warping_moment_of_inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:55.917172 unitsnet-py-0.1.45/unitsnet_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-12 13:17:55.000000 unitsnet-py-0.1.45/unitsnet_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-12 13:17:55.000000 unitsnet-py-0.1.45/unitsnet_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:17:55.000000 unitsnet-py-0.1.45/unitsnet_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 13:17:55.000000 unitsnet-py-0.1.45/unitsnet_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-17 18:40:49.000000 unitsnet-py-0.1.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27203 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-17 18:41:34.000000 unitsnet-py-0.1.46/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-17 18:41:35.000000 unitsnet-py-0.1.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.439574 unitsnet-py-0.1.46/unitsnet_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/unitsnet_py/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/amount_of_substance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/amplitude_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/apparent_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/apparent_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/area_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/area_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/brake_specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/capacitance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/coefficient_of_thermal_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/compressibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/dynamic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_admittance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_conductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_current_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_current_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_inductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_resistivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_surface_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/energy_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/force_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/force_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/fuel_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/heat_transfer_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/irradiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/jerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/kinematic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/leak_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/linear_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/linear_power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminous_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminous_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/magnetic_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/magnetic_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/permittivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/porous_medium_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/power_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34511 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/pressure_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/ratio_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reactive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reactive_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/relative_humidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/solid_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/standard_volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/thermal_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/thermal_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/torque_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/turbidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/vitamin_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_flow_per_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volumetric_heat_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/warping_moment_of_inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.439574 unitsnet-py-0.1.46/unitsnet_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/top_level.txt
```

### Comparing `unitsnet-py-0.1.45/LICENSE` & `unitsnet-py-0.1.46/LICENSE`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/PKG-INFO` & `unitsnet-py-0.1.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.45
+Version: 0.1.46
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
```

### Comparing `unitsnet-py-0.1.45/README.md` & `unitsnet-py-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/pyproject.toml` & `unitsnet-py-0.1.46/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitsnet_py"
-version = "0.1.45"
+version = "0.1.46"
 description = "A better way to hold unit variables and easily convert to the destination unit"
 repository = "https://github.com/haimkastner/unitsnet-py"
 authors = ["Haim Kastner <haim.kastner@gmail.com>"]
 maintainers = [
     "Haim Kastner <haim.kastner@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `unitsnet-py-0.1.45/setup.py` & `unitsnet-py-0.1.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['unitsnet_py', 'unitsnet_py.units']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'unitsnet-py',
-    'version': '0.1.45',
+    'version': '0.1.46',
     'keywords': 'conversion, units-of-measure, units, quantities, unit-converter, converter, unit, measure, measures, measurement, measurements',
     'description': 'A better way to hold unit variables and easily convert to the destination unit',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Haim Kastner',
     'author_email': 'haim.kastner@gmail.com',
     'maintainer': 'Haim Kastner',
```

### Comparing `unitsnet-py-0.1.45/unitsnet_py/__init__.py` & `unitsnet-py-0.1.46/unitsnet_py/__init__.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py` & `unitsnet-py-0.1.46/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/acceleration.py` & `unitsnet-py-0.1.46/unitsnet_py/units/acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/amount_of_substance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/amount_of_substance.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,24 @@
         """
         
         PoundMole = 'pound_mole'
         """
             
         """
         
+        Femtomole = 'femtomole'
+        """
+            
+        """
+        
+        Picomole = 'picomole'
+        """
+            
+        """
+        
         Nanomole = 'nanomole'
         """
             
         """
         
         Micromole = 'micromole'
         """
@@ -97,14 +107,18 @@
             raise ValueError('Invalid unit: value is NaN')
         self.__value = self.__convert_to_base(value, from_unit)
         
         self.__moles = None
         
         self.__pound_moles = None
         
+        self.__femtomoles = None
+        
+        self.__picomoles = None
+        
         self.__nanomoles = None
         
         self.__micromoles = None
         
         self.__millimoles = None
         
         self.__centimoles = None
@@ -133,14 +147,20 @@
         
         if from_unit == AmountOfSubstanceUnits.Mole:
             return (value)
         
         if from_unit == AmountOfSubstanceUnits.PoundMole:
             return (value / 453.59237)
         
+        if from_unit == AmountOfSubstanceUnits.Femtomole:
+            return ((value) / 1e-15)
+        
+        if from_unit == AmountOfSubstanceUnits.Picomole:
+            return ((value) / 1e-12)
+        
         if from_unit == AmountOfSubstanceUnits.Nanomole:
             return ((value) / 1e-09)
         
         if from_unit == AmountOfSubstanceUnits.Micromole:
             return ((value) / 1e-06)
         
         if from_unit == AmountOfSubstanceUnits.Millimole:
@@ -183,14 +203,20 @@
         
         if to_unit == AmountOfSubstanceUnits.Mole:
             return (value)
         
         if to_unit == AmountOfSubstanceUnits.PoundMole:
             return (value * 453.59237)
         
+        if to_unit == AmountOfSubstanceUnits.Femtomole:
+            return ((value) * 1e-15)
+        
+        if to_unit == AmountOfSubstanceUnits.Picomole:
+            return ((value) * 1e-12)
+        
         if to_unit == AmountOfSubstanceUnits.Nanomole:
             return ((value) * 1e-09)
         
         if to_unit == AmountOfSubstanceUnits.Micromole:
             return ((value) * 1e-06)
         
         if to_unit == AmountOfSubstanceUnits.Millimole:
@@ -261,14 +287,44 @@
         :return: A new instance of AmountOfSubstance.
         :rtype: AmountOfSubstance
         """
         return AmountOfSubstance(pound_moles, AmountOfSubstanceUnits.PoundMole)
 
     
     @staticmethod
+    def from_femtomoles(femtomoles: float):
+        """
+        Create a new instance of AmountOfSubstance from a value in femtomoles.
+
+        
+
+        :param meters: The AmountOfSubstance value in femtomoles.
+        :type femtomoles: float
+        :return: A new instance of AmountOfSubstance.
+        :rtype: AmountOfSubstance
+        """
+        return AmountOfSubstance(femtomoles, AmountOfSubstanceUnits.Femtomole)
+
+    
+    @staticmethod
+    def from_picomoles(picomoles: float):
+        """
+        Create a new instance of AmountOfSubstance from a value in picomoles.
+
+        
+
+        :param meters: The AmountOfSubstance value in picomoles.
+        :type picomoles: float
+        :return: A new instance of AmountOfSubstance.
+        :rtype: AmountOfSubstance
+        """
+        return AmountOfSubstance(picomoles, AmountOfSubstanceUnits.Picomole)
+
+    
+    @staticmethod
     def from_nanomoles(nanomoles: float):
         """
         Create a new instance of AmountOfSubstance from a value in nanomoles.
 
         
 
         :param meters: The AmountOfSubstance value in nanomoles.
@@ -478,14 +534,36 @@
         if self.__pound_moles != None:
             return self.__pound_moles
         self.__pound_moles = self.__convert_from_base(AmountOfSubstanceUnits.PoundMole)
         return self.__pound_moles
 
     
     @property
+    def femtomoles(self) -> float:
+        """
+        
+        """
+        if self.__femtomoles != None:
+            return self.__femtomoles
+        self.__femtomoles = self.__convert_from_base(AmountOfSubstanceUnits.Femtomole)
+        return self.__femtomoles
+
+    
+    @property
+    def picomoles(self) -> float:
+        """
+        
+        """
+        if self.__picomoles != None:
+            return self.__picomoles
+        self.__picomoles = self.__convert_from_base(AmountOfSubstanceUnits.Picomole)
+        return self.__picomoles
+
+    
+    @property
     def nanomoles(self) -> float:
         """
         
         """
         if self.__nanomoles != None:
             return self.__nanomoles
         self.__nanomoles = self.__convert_from_base(AmountOfSubstanceUnits.Nanomole)
@@ -633,14 +711,20 @@
         
         if unit == AmountOfSubstanceUnits.Mole:
             return f"""{self.moles} mol"""
         
         if unit == AmountOfSubstanceUnits.PoundMole:
             return f"""{self.pound_moles} lbmol"""
         
+        if unit == AmountOfSubstanceUnits.Femtomole:
+            return f"""{self.femtomoles} """
+        
+        if unit == AmountOfSubstanceUnits.Picomole:
+            return f"""{self.picomoles} """
+        
         if unit == AmountOfSubstanceUnits.Nanomole:
             return f"""{self.nanomoles} """
         
         if unit == AmountOfSubstanceUnits.Micromole:
             return f"""{self.micromoles} """
         
         if unit == AmountOfSubstanceUnits.Millimole:
@@ -688,14 +772,20 @@
         
         if unit_abbreviation == AmountOfSubstanceUnits.Mole:
             return """mol"""
         
         if unit_abbreviation == AmountOfSubstanceUnits.PoundMole:
             return """lbmol"""
         
+        if unit_abbreviation == AmountOfSubstanceUnits.Femtomole:
+            return """"""
+        
+        if unit_abbreviation == AmountOfSubstanceUnits.Picomole:
+            return """"""
+        
         if unit_abbreviation == AmountOfSubstanceUnits.Nanomole:
             return """"""
         
         if unit_abbreviation == AmountOfSubstanceUnits.Micromole:
             return """"""
         
         if unit_abbreviation == AmountOfSubstanceUnits.Millimole:
```

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/amplitude_ratio.py` & `unitsnet-py-0.1.46/unitsnet_py/units/amplitude_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/angle.py` & `unitsnet-py-0.1.46/unitsnet_py/units/angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/apparent_energy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/apparent_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/apparent_power.py` & `unitsnet-py-0.1.46/unitsnet_py/units/apparent_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/area.py` & `unitsnet-py-0.1.46/unitsnet_py/units/area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/area_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/area_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/area_moment_of_inertia.py` & `unitsnet-py-0.1.46/unitsnet_py/units/area_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/bit_rate.py` & `unitsnet-py-0.1.46/unitsnet_py/units/bit_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/brake_specific_fuel_consumption.py` & `unitsnet-py-0.1.46/unitsnet_py/units/brake_specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/capacitance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/capacitance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/coefficient_of_thermal_expansion.py` & `unitsnet-py-0.1.46/unitsnet_py/units/coefficient_of_thermal_expansion.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/compressibility.py` & `unitsnet-py-0.1.46/unitsnet_py/units/compressibility.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/duration.py` & `unitsnet-py-0.1.46/unitsnet_py/units/duration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/dynamic_viscosity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/dynamic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_admittance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_admittance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_charge.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_charge.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_charge_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_conductance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_conductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_conductivity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_current.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_current.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_current_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_current_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_current_gradient.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_current_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_field.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_inductance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_inductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_potential.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_potential_ac.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_ac.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_potential_change_rate.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_potential_dc.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_dc.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_resistance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_resistivity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_resistivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/electric_surface_charge_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/electric_surface_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/energy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/energy_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/energy_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/entropy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/force.py` & `unitsnet-py-0.1.46/unitsnet_py/units/force.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/force_change_rate.py` & `unitsnet-py-0.1.46/unitsnet_py/units/force_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/force_per_length.py` & `unitsnet-py-0.1.46/unitsnet_py/units/force_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/frequency.py` & `unitsnet-py-0.1.46/unitsnet_py/units/frequency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/fuel_efficiency.py` & `unitsnet-py-0.1.46/unitsnet_py/units/fuel_efficiency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/heat_flux.py` & `unitsnet-py-0.1.46/unitsnet_py/units/heat_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/heat_transfer_coefficient.py` & `unitsnet-py-0.1.46/unitsnet_py/units/heat_transfer_coefficient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/illuminance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/illuminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/impulse.py` & `unitsnet-py-0.1.46/unitsnet_py/units/impulse.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/information.py` & `unitsnet-py-0.1.46/unitsnet_py/units/information.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/irradiance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/irradiance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/irradiation.py` & `unitsnet-py-0.1.46/unitsnet_py/units/irradiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/jerk.py` & `unitsnet-py-0.1.46/unitsnet_py/units/jerk.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/kinematic_viscosity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/kinematic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/leak_rate.py` & `unitsnet-py-0.1.46/unitsnet_py/units/leak_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/length.py` & `unitsnet-py-0.1.46/unitsnet_py/units/length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/level.py` & `unitsnet-py-0.1.46/unitsnet_py/units/level.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/linear_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/linear_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/linear_power_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/linear_power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/luminance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/luminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/luminosity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/luminosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/luminous_flux.py` & `unitsnet-py-0.1.46/unitsnet_py/units/luminous_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/luminous_intensity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/luminous_intensity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/magnetic_field.py` & `unitsnet-py-0.1.46/unitsnet_py/units/magnetic_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/magnetic_flux.py` & `unitsnet-py-0.1.46/unitsnet_py/units/magnetic_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/magnetization.py` & `unitsnet-py-0.1.46/unitsnet_py/units/magnetization.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/mass.py` & `unitsnet-py-0.1.46/unitsnet_py/units/mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/mass_concentration.py` & `unitsnet-py-0.1.46/unitsnet_py/units/mass_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/mass_flow.py` & `unitsnet-py-0.1.46/unitsnet_py/units/mass_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/mass_flux.py` & `unitsnet-py-0.1.46/unitsnet_py/units/mass_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/mass_fraction.py` & `unitsnet-py-0.1.46/unitsnet_py/units/mass_fraction.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/mass_moment_of_inertia.py` & `unitsnet-py-0.1.46/unitsnet_py/units/mass_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/molar_energy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/molar_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/molar_entropy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/molar_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/molar_flow.py` & `unitsnet-py-0.1.46/unitsnet_py/units/molar_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/molar_mass.py` & `unitsnet-py-0.1.46/unitsnet_py/units/molar_mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/molarity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/molarity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/permeability.py` & `unitsnet-py-0.1.46/unitsnet_py/units/permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/permittivity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/permittivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/porous_medium_permeability.py` & `unitsnet-py-0.1.46/unitsnet_py/units/porous_medium_permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/power.py` & `unitsnet-py-0.1.46/unitsnet_py/units/power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/power_density.py` & `unitsnet-py-0.1.46/unitsnet_py/units/power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/power_ratio.py` & `unitsnet-py-0.1.46/unitsnet_py/units/power_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/pressure.py` & `unitsnet-py-0.1.46/unitsnet_py/units/pressure.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/pressure_change_rate.py` & `unitsnet-py-0.1.46/unitsnet_py/units/pressure_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/ratio.py` & `unitsnet-py-0.1.46/unitsnet_py/units/ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/ratio_change_rate.py` & `unitsnet-py-0.1.46/unitsnet_py/units/ratio_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/reactive_energy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/reactive_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/reactive_power.py` & `unitsnet-py-0.1.46/unitsnet_py/units/reactive_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/reciprocal_area.py` & `unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/reciprocal_length.py` & `unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/relative_humidity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/relative_humidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/rotational_acceleration.py` & `unitsnet-py-0.1.46/unitsnet_py/units/rotational_acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/rotational_speed.py` & `unitsnet-py-0.1.46/unitsnet_py/units/rotational_speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/rotational_stiffness.py` & `unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/rotational_stiffness_per_length.py` & `unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/scalar.py` & `unitsnet-py-0.1.46/unitsnet_py/units/scalar.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/solid_angle.py` & `unitsnet-py-0.1.46/unitsnet_py/units/solid_angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/specific_energy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/specific_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/specific_entropy.py` & `unitsnet-py-0.1.46/unitsnet_py/units/specific_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/specific_fuel_consumption.py` & `unitsnet-py-0.1.46/unitsnet_py/units/specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/specific_volume.py` & `unitsnet-py-0.1.46/unitsnet_py/units/specific_volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/specific_weight.py` & `unitsnet-py-0.1.46/unitsnet_py/units/specific_weight.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/speed.py` & `unitsnet-py-0.1.46/unitsnet_py/units/speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/standard_volume_flow.py` & `unitsnet-py-0.1.46/unitsnet_py/units/standard_volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/temperature.py` & `unitsnet-py-0.1.46/unitsnet_py/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/temperature_change_rate.py` & `unitsnet-py-0.1.46/unitsnet_py/units/temperature_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/temperature_delta.py` & `unitsnet-py-0.1.46/unitsnet_py/units/temperature_delta.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/temperature_gradient.py` & `unitsnet-py-0.1.46/unitsnet_py/units/temperature_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/thermal_conductivity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/thermal_resistance.py` & `unitsnet-py-0.1.46/unitsnet_py/units/thermal_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/torque.py` & `unitsnet-py-0.1.46/unitsnet_py/units/torque.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/torque_per_length.py` & `unitsnet-py-0.1.46/unitsnet_py/units/torque_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/turbidity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/turbidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/vitamin_a.py` & `unitsnet-py-0.1.46/unitsnet_py/units/vitamin_a.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/volume.py` & `unitsnet-py-0.1.46/unitsnet_py/units/volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/volume_concentration.py` & `unitsnet-py-0.1.46/unitsnet_py/units/volume_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/volume_flow.py` & `unitsnet-py-0.1.46/unitsnet_py/units/volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/volume_flow_per_area.py` & `unitsnet-py-0.1.46/unitsnet_py/units/volume_flow_per_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/volume_per_length.py` & `unitsnet-py-0.1.46/unitsnet_py/units/volume_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/volumetric_heat_capacity.py` & `unitsnet-py-0.1.46/unitsnet_py/units/volumetric_heat_capacity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py/units/warping_moment_of_inertia.py` & `unitsnet-py-0.1.46/unitsnet_py/units/warping_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.45/unitsnet_py.egg-info/PKG-INFO` & `unitsnet-py-0.1.46/unitsnet_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.45
+Version: 0.1.46
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
```

### Comparing `unitsnet-py-0.1.45/unitsnet_py.egg-info/SOURCES.txt` & `unitsnet-py-0.1.46/unitsnet_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

