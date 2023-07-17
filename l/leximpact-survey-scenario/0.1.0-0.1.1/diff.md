# Comparing `tmp/leximpact_survey_scenario-0.1.0.tar.gz` & `tmp/leximpact_survey_scenario-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leximpact_survey_scenario-0.1.0.tar", max compression
+gzip compressed data, was "leximpact_survey_scenario-0.1.1.tar", max compression
```

## Comparing `leximpact_survey_scenario-0.1.0.tar` & `leximpact_survey_scenario-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-07-10 08:30:17.254774 leximpact_survey_scenario-0.1.0/LICENSE
--rw-r--r--   0        0        0      102 2023-07-10 15:42:38.559234 leximpact_survey_scenario-0.1.0/README.md
--rw-r--r--   0        0        0       54 2023-07-10 15:42:38.559234 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/__init__.py
--rw-r--r--   0        0        0    10764 2023-07-12 13:29:03.858158 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/leximpact_survey_scenario.py
--rw-r--r--   0        0        0     8177 2023-07-10 14:55:13.675184 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/leximpact_tax_and_benefit_system.py
--rw-r--r--   0        0        0       23 2023-07-10 08:30:17.258774 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/__init__.py
--rw-r--r--   0        0        0    11605 2023-07-12 14:27:26.922220 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/calmar_tools.py
--rw-r--r--   0        0        0    22810 2023-07-12 14:27:26.922220 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py
--rw-r--r--   0        0        0     9021 2023-07-12 14:27:26.922220 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py
--rw-r--r--   0        0        0     5233 2023-07-10 14:55:13.675184 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/inflator.py
--rw-r--r--   0        0        0     1561 2023-07-10 14:52:26.751181 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/leximpact_comparator.py
--rw-r--r--   0        0        0     9040 2023-07-10 08:30:17.258774 leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/plot.py
--rw-r--r--   0        0        0     1619 2023-07-12 14:27:26.922220 leximpact_survey_scenario-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 leximpact_survey_scenario-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/LICENSE
+-rw-r--r--   0        0        0      102 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/README.md
+-rw-r--r--   0        0        0       54 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/__init__.py
+-rw-r--r--   0        0        0    10764 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/leximpact_survey_scenario.py
+-rw-r--r--   0        0        0     6539 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/leximpact_tax_and_benefit_system.py
+-rw-r--r--   0        0        0       23 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/__init__.py
+-rw-r--r--   0        0        0    17584 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py
+-rw-r--r--   0        0        0     9021 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py
+-rw-r--r--   0        0        0     5233 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflator.py
+-rw-r--r--   0        0        0     1561 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/leximpact_comparator.py
+-rw-r--r--   0        0        0     9040 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/plot.py
+-rw-r--r--   0        0        0     1599 2023-07-17 11:12:26.581678 leximpact_survey_scenario-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 leximpact_survey_scenario-0.1.1/PKG-INFO
```

### Comparing `leximpact_survey_scenario-0.1.0/LICENSE` & `leximpact_survey_scenario-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/leximpact_survey_scenario.py` & `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/leximpact_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py` & `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import copy
 import unittest
 
-import matplotlib.pyplot as plt
 import pandas as pd
-import seaborn as sns
 from leximpact_aggregates.aggregate import AggregateManager
 from decouple import config
 
 
 tc = unittest.TestCase()
 
 # Import des années
@@ -581,160 +579,7 @@
             + " (en bleu) "
         )
 
     # Details
     title = title + title_suffix
 
     return title
-
-
-def compare_distributions(
-    df_erfs,
-    df_pote,
-    var_name,
-    annee_erfs,
-    annee_pote,
-    title_suffix,
-    log=None,
-    df_cal=[],
-):
-    """Plot et compare les distributions de l'ERFS et de POTE"""
-    annee_erfs = str(annee_erfs)
-    annee_pote = str(annee_pote)
-
-    # Pour traiter le cas des buckets vides, on remplace les NaN par zéro
-    df_pote["mean"] = df_pote["mean"].fillna(0)
-    df_erfs["mean"] = df_erfs["mean"].fillna(0)
-    if len(df_cal) != 0:
-        df_cal["mean"] = df_cal["mean"].fillna(0)
-
-    # Création d'une figure
-    fig = plt.figure(figsize=(18, 8), facecolor="white", clear=True)
-    ax = sns.barplot(data=df_pote, y="sum", x=df_pote.index, alpha=0.5, color="blue")
-    ax = sns.barplot(data=df_erfs, y="sum", x=df_erfs.index, alpha=0.5, color="red")
-    outname = (
-        var_name
-        + "_ERFS_"
-        + str(annee_erfs)
-        + "_POTE_"
-        + str(annee_pote)
-        + "_"
-        + title_suffix
-    )
-
-    # S'il y a une calibration
-    if len(df_cal) != 0:
-        ax = sns.barplot(data=df_cal, y="sum", x=df_cal.index, alpha=0.5, color="green")
-        title = generate_title(var_name, annee_erfs, annee_pote, title_suffix, cal=True)
-        outname = "Distributions_de_" + outname
-        df_base = df_cal.copy()
-
-    else:
-        title = generate_title(
-            var_name, annee_erfs, annee_pote, title_suffix, cal=False
-        )
-        outname = "Calibration_de_" + outname
-        df_base = df_erfs.copy()
-
-    # Si échelle logarithmique
-    if log:
-        _ = ax.set_yscale("log")
-        _ = ax.set_title(
-            (title + "\n Echelle de population logarithmique"), fontsize=18
-        )
-    else:
-        _ = ax.set_title(title, fontsize=18)
-
-    # Axis Setup
-    xticks = [i for i in range(len(df_pote["middle"]))]
-    xlabels = [f"{str(round(j / (10 ** 3), 2))} k€" for j in df_pote["mean"]]
-    _ = ax.set_xticks(xticks)
-    _ = ax.set_xticklabels(xlabels, rotation=75)
-    _ = ax.set_xlabel(
-        " ' " + var_name + " ' " + " moyen pour chaque quantile (POTE)", fontsize=16
-    )
-    _ = ax.set_ylabel("Somme de " + var_name + " dans chaque quantile", fontsize=16)
-
-    # Plotting the sum on top of the bars
-    # ax.margins(y=0.1)
-    # for bars in ax.containers:
-    #    ax.bar_label(bars, fmt='%.1f')
-
-    # Saving the figure
-    figpath = config.get("PLOTS")
-    plt.savefig((figpath + outname), bbox_inches="tight")
-
-    # On calcule l'erreur comme la moyenne des erreurs de chaque bucket
-    error_df = 100 * pd.Series(abs(df_pote["sum"] - df_base["sum"]) / df_pote["sum"])
-    # Pour le premier bucket, les sommes sont à zéro donc on mesure l'erreur en Nb de foyers
-    error_df[0] = (
-        100 * abs(df_pote["nb_ff"][0] - df_base["nb_ff"][0]) / df_pote["nb_ff"][0]
-    )
-    # On exclut les quantiles nuls du calcul d'erreur
-    final_error = (error_df.sum()) / (len(df_base))
-    print("Erreur moyenne des buckets de ", var_name, " : ", final_error, " %")
-    print("Erreur min : ", min(error_df), "erreur max: ", max(error_df))
-
-    return fig, error_df, final_error
-
-
-def pote_comparison(base_ff, variable, title_suffix=None, log=None, base_ff_cal=None):
-    # Obtention des quantiles de POTE
-    quantiles = get_quantiles_casd(variable)
-    assert quantiles is not None
-    print(base_ff.keys())
-    # On garde les notations utilisées pour le calcul
-    base_ff["wprm"] = base_ff["weight_foyers"]
-    base_ff["idfoy"] = base_ff["foyer_fiscal_id"]
-
-    # Distribution de la base sur les quantiles de POTE
-    Distrib_BASE, Distrib_POTE, quantiles = distrib_to_quantiles(
-        base_ff, variable, quantiles
-    )
-    poids_avant = base_ff["weight_foyers"].copy()
-    print("Somme des poids avant calibration", poids_avant.sum())
-
-    if base_ff_cal is not None:
-        print("Somme des poids après calibration", base_ff_cal["weight_foyers"].sum())
-        # On garde les notations utilisées pour le calcul
-        base_ff_cal["wprm"] = base_ff_cal["weight_foyers"]
-        base_ff_cal["idfoy"] = base_ff_cal["foyer_fiscal_id"]
-
-        # Distribution de la base sur les quantiles de POTE
-        Distrib_BASE_CAL, Distrib_POTE_2, quantiles = distrib_to_quantiles(
-            base_ff_cal, variable, quantiles
-        )
-
-        # Comparaison des distributions
-        fig, error_df, final_error = compare_distributions(
-            Distrib_BASE.df,
-            Distrib_POTE.df,
-            variable,
-            annee_erfs,
-            annee_pote,
-            title_suffix,
-            log,
-            df_cal=Distrib_BASE_CAL.df,
-        )
-
-        print(
-            "Total de ",
-            variable,
-            "avant :",
-            (base_ff[variable] * poids_avant).sum(),
-            "et après calibration :",
-            (base_ff_cal["weight_foyers"] * base_ff_cal[variable]).sum(),
-        )
-    else:
-        # Comparaison des distributions
-        fig, error_df, final_error = compare_distributions(
-            Distrib_BASE.df,
-            Distrib_POTE.df,
-            variable,
-            annee_erfs,
-            annee_pote,
-            title_suffix,
-            log,
-            df_cal=[],
-        )
-
-    return fig, error_df, final_error
```

### Comparing `leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py` & `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/inflator.py` & `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflator.py`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/leximpact_comparator.py` & `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/leximpact_comparator.py`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.0/leximpact_survey_scenario/scenario_tools/plot.py` & `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/plot.py`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.0/pyproject.toml` & `leximpact_survey_scenario-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "leximpact-survey-scenario"
-version = "0.1.0"
+version = "0.1.1"
 description = "OpenFisca Survey Scenario for LexImpact"
 authors = ["LexImapct"]
 license = "LGPLv3"
 readme = "README.md"
 packages = [{include = "leximpact_survey_scenario"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 OpenFisca-France-Data = "^1.2.0"
 ipykernel = "^6.24.0"
 scikit-learn = "^1.3.0"
-seaborn = "^0.12.2"
 python-decouple = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.17.0"
 ruff = "^0.0.277"
 black = "^23.3.0"
 pytest = "^7.4.0"
```

### Comparing `leximpact_survey_scenario-0.1.0/PKG-INFO` & `leximpact_survey_scenario-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: leximpact-survey-scenario
-Version: 0.1.0
+Version: 0.1.1
 Summary: OpenFisca Survey Scenario for LexImpact
 License: LGPLv3
 Author: LexImapct
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: OpenFisca-France-Data (>=1.2.0,<2.0.0)
 Requires-Dist: ipykernel (>=6.24.0,<7.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
-Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Description-Content-Type: text/markdown
 
 # leximpact-survey-scenario
 
 This project is for internal use at [LexImpact](http://LexImpact.an.fr).
```

