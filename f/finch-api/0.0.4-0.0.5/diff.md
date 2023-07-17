# Comparing `tmp/finch_api-0.0.4.tar.gz` & `tmp/finch_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finch_api-0.0.4.tar", max compression
+gzip compressed data, was "finch_api-0.0.5.tar", max compression
```

## Comparing `finch_api-0.0.4.tar` & `finch_api-0.0.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11335 2023-07-12 11:39:59.195564 finch_api-0.0.4/LICENSE
--rw-r--r--   0        0        0     7466 2023-07-12 11:39:59.195564 finch_api-0.0.4/README.md
--rw-r--r--   0        0        0     1891 2023-07-12 11:39:59.199564 finch_api-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1834 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/__init__.py
--rw-r--r--   0        0        0    46805 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_base_client.py
--rw-r--r--   0        0        0     3889 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_base_exceptions.py
--rw-r--r--   0        0        0    17881 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_client.py
--rw-r--r--   0        0        0     1285 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_models.py
--rw-r--r--   0        0        0     4846 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_qs.py
--rw-r--r--   0        0        0      872 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_resource.py
--rw-r--r--   0        0        0     5884 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_streaming.py
--rw-r--r--   0        0        0     4226 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_types.py
--rw-r--r--   0        0        0     1277 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_utils/_utils.py
--rw-r--r--   0        0        0      124 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/_version.py
--rw-r--r--   0        0        0    10630 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/pagination.py
--rw-r--r--   0        0        0        0 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/py.typed
--rw-r--r--   0        0        0      321 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/account.py
--rw-r--r--   0        0        0      532 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/ats/__init__.py
--rw-r--r--   0        0        0     6374 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/ats/applications.py
--rw-r--r--   0        0        0     1409 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/ats/ats.py
--rw-r--r--   0        0        0     6638 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/ats/candidates.py
--rw-r--r--   0        0        0     6044 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/ats/jobs.py
--rw-r--r--   0        0        0     6148 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/ats/offers.py
--rw-r--r--   0        0        0     2703 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/ats/stages.py
--rw-r--r--   0        0        0      703 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/__init__.py
--rw-r--r--   0        0        0      231 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/benefits/__init__.py
--rw-r--r--   0        0        0    14280 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/benefits/benefits.py
--rw-r--r--   0        0        0    14347 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/benefits/individuals.py
--rw-r--r--   0        0        0     2021 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/company.py
--rw-r--r--   0        0        0     4175 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/directory.py
--rw-r--r--   0        0        0     1760 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/hris.py
--rw-r--r--   0        0        0      262 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/individuals/__init__.py
--rw-r--r--   0        0        0     4278 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/individuals/employment_data.py
--rw-r--r--   0        0        0     4552 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/individuals/individuals.py
--rw-r--r--   0        0        0     3963 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/pay_statements.py
--rw-r--r--   0        0        0     4247 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/hris/payments.py
--rw-r--r--   0        0        0     2256 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/resources/providers.py
--rw-r--r--   0        0        0      416 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/__init__.py
--rw-r--r--   0        0        0      572 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/__init__.py
--rw-r--r--   0        0        0      512 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/application.py
--rw-r--r--   0        0        0      361 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/application_list_params.py
--rw-r--r--   0        0        0      726 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/candidate.py
--rw-r--r--   0        0        0      355 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/candidate_list_params.py
--rw-r--r--   0        0        0      889 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/job.py
--rw-r--r--   0        0        0      337 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/job_list_params.py
--rw-r--r--   0        0        0      474 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/offer.py
--rw-r--r--   0        0        0      343 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/offer_list_params.py
--rw-r--r--   0        0        0      362 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/ats/stage.py
--rw-r--r--   0        0        0      266 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/disconnect_response.py
--rw-r--r--   0        0        0     1761 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/__init__.py
--rw-r--r--   0        0        0      902 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefit_create_params.py
--rw-r--r--   0        0        0      220 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefit_frequency.py
--rw-r--r--   0        0        0      598 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefit_type.py
--rw-r--r--   0        0        0      278 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefit_update_params.py
--rw-r--r--   0        0        0      784 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/__init__.py
--rw-r--r--   0        0        0      723 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/enrolled_individual.py
--rw-r--r--   0        0        0      969 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/individual_benefit.py
--rw-r--r--   0        0        0      550 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/individual_enroll_many_params.py
--rw-r--r--   0        0        0      259 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
--rw-r--r--   0        0        0      398 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
--rw-r--r--   0        0        0      329 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/individual_unenroll_params.py
--rw-r--r--   0        0        0      647 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benefits/unenrolled_individual.py
--rw-r--r--   0        0        0      415 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/benfit_contribution.py
--rw-r--r--   0        0        0     2209 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/company.py
--rw-r--r--   0        0        0      596 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/company_benefit.py
--rw-r--r--   0        0        0      202 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/create_company_benefits_response.py
--rw-r--r--   0        0        0      376 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/directory_list_individuals_params.py
--rw-r--r--   0        0        0     1361 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individual.py
--rw-r--r--   0        0        0     1025 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individual_in_directory.py
--rw-r--r--   0        0        0      327 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individual_response.py
--rw-r--r--   0        0        0      480 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individual_retrieve_many_params.py
--rw-r--r--   0        0        0      367 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individuals/__init__.py
--rw-r--r--   0        0        0     2985 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individuals/employment_data.py
--rw-r--r--   0        0        0      363 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individuals/employment_data_response.py
--rw-r--r--   0        0        0      703 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py
--rw-r--r--   0        0        0     3320 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/pay_statement.py
--rw-r--r--   0        0        0      376 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/pay_statement_response.py
--rw-r--r--   0        0        0      438 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/pay_statement_response_body.py
--rw-r--r--   0        0        0      616 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/pay_statement_retrieve_many_params.py
--rw-r--r--   0        0        0      791 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/payment.py
--rw-r--r--   0        0        0      709 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/payment_list_params.py
--rw-r--r--   0        0        0     1411 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/supported_benefit.py
--rw-r--r--   0        0        0      200 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/hris/update_company_benefit_response.py
--rw-r--r--   0        0        0      724 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/income.py
--rw-r--r--   0        0        0      881 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/introspection.py
--rw-r--r--   0        0        0      631 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/location.py
--rw-r--r--   0        0        0      262 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/money.py
--rw-r--r--   0        0        0      369 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/paging.py
--rw-r--r--   0        0        0      959 2023-07-12 11:39:59.199564 finch_api-0.0.4/src/finch/types/provider.py
--rw-r--r--   0        0        0     8383 1970-01-01 00:00:00.000000 finch_api-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-17 16:52:36.629876 finch_api-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7466 2023-07-17 16:52:36.629876 finch_api-0.0.5/README.md
+-rw-r--r--   0        0        0     1891 2023-07-17 16:52:36.629876 finch_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1834 2023-07-17 16:52:36.629876 finch_api-0.0.5/src/finch/__init__.py
+-rw-r--r--   0        0        0    46805 2023-07-17 16:52:36.629876 finch_api-0.0.5/src/finch/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-07-17 16:52:36.629876 finch_api-0.0.5/src/finch/_base_exceptions.py
+-rw-r--r--   0        0        0    17881 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_client.py
+-rw-r--r--   0        0        0     1285 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_models.py
+-rw-r--r--   0        0        0     4846 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_qs.py
+-rw-r--r--   0        0        0      872 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_resource.py
+-rw-r--r--   0        0        0     5884 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_streaming.py
+-rw-r--r--   0        0        0     4226 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_types.py
+-rw-r--r--   0        0        0     1277 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_utils/_utils.py
+-rw-r--r--   0        0        0      124 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/_version.py
+-rw-r--r--   0        0        0    10630 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/pagination.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/py.typed
+-rw-r--r--   0        0        0      321 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/account.py
+-rw-r--r--   0        0        0      532 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/ats/__init__.py
+-rw-r--r--   0        0        0     6374 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/ats/applications.py
+-rw-r--r--   0        0        0     1409 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/ats/ats.py
+-rw-r--r--   0        0        0     6638 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/ats/candidates.py
+-rw-r--r--   0        0        0     6044 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/ats/jobs.py
+-rw-r--r--   0        0        0     6148 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/ats/offers.py
+-rw-r--r--   0        0        0     2703 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/ats/stages.py
+-rw-r--r--   0        0        0      703 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/__init__.py
+-rw-r--r--   0        0        0      231 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/benefits/__init__.py
+-rw-r--r--   0        0        0    14280 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/benefits/benefits.py
+-rw-r--r--   0        0        0    14347 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/benefits/individuals.py
+-rw-r--r--   0        0        0     2021 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/company.py
+-rw-r--r--   0        0        0     4175 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/directory.py
+-rw-r--r--   0        0        0     1760 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/hris.py
+-rw-r--r--   0        0        0      262 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     4278 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0     4552 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/individuals/individuals.py
+-rw-r--r--   0        0        0     3963 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/pay_statements.py
+-rw-r--r--   0        0        0     4247 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/hris/payments.py
+-rw-r--r--   0        0        0     2256 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/resources/providers.py
+-rw-r--r--   0        0        0      416 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/__init__.py
+-rw-r--r--   0        0        0      512 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/application.py
+-rw-r--r--   0        0        0      361 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/application_list_params.py
+-rw-r--r--   0        0        0      726 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/candidate.py
+-rw-r--r--   0        0        0      355 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/candidate_list_params.py
+-rw-r--r--   0        0        0      889 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/job.py
+-rw-r--r--   0        0        0      337 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/job_list_params.py
+-rw-r--r--   0        0        0      474 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/offer.py
+-rw-r--r--   0        0        0      343 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/offer_list_params.py
+-rw-r--r--   0        0        0      362 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/ats/stage.py
+-rw-r--r--   0        0        0      266 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/disconnect_response.py
+-rw-r--r--   0        0        0     1761 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefit_create_params.py
+-rw-r--r--   0        0        0      220 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefit_frequency.py
+-rw-r--r--   0        0        0      598 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefit_type.py
+-rw-r--r--   0        0        0      278 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefit_update_params.py
+-rw-r--r--   0        0        0      784 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/enrolled_individual.py
+-rw-r--r--   0        0        0      969 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/individual_benefit.py
+-rw-r--r--   0        0        0      550 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/individual_enroll_many_params.py
+-rw-r--r--   0        0        0      259 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
+-rw-r--r--   0        0        0      398 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
+-rw-r--r--   0        0        0      329 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/individual_unenroll_params.py
+-rw-r--r--   0        0        0      647 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benefits/unenrolled_individual.py
+-rw-r--r--   0        0        0      415 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/benfit_contribution.py
+-rw-r--r--   0        0        0     2209 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/company.py
+-rw-r--r--   0        0        0      596 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/company_benefit.py
+-rw-r--r--   0        0        0      202 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/create_company_benefits_response.py
+-rw-r--r--   0        0        0      376 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/directory_list_individuals_params.py
+-rw-r--r--   0        0        0     1361 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individual.py
+-rw-r--r--   0        0        0     1025 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individual_in_directory.py
+-rw-r--r--   0        0        0      327 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individual_response.py
+-rw-r--r--   0        0        0      480 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individual_retrieve_many_params.py
+-rw-r--r--   0        0        0      367 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     2985 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0      363 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individuals/employment_data_response.py
+-rw-r--r--   0        0        0      703 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py
+-rw-r--r--   0        0        0     3320 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/pay_statement.py
+-rw-r--r--   0        0        0      376 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/pay_statement_response.py
+-rw-r--r--   0        0        0      438 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/pay_statement_response_body.py
+-rw-r--r--   0        0        0      616 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/pay_statement_retrieve_many_params.py
+-rw-r--r--   0        0        0      791 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/payment.py
+-rw-r--r--   0        0        0      709 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/payment_list_params.py
+-rw-r--r--   0        0        0     1411 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/supported_benefit.py
+-rw-r--r--   0        0        0      200 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/hris/update_company_benefit_response.py
+-rw-r--r--   0        0        0      724 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/income.py
+-rw-r--r--   0        0        0      881 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/introspection.py
+-rw-r--r--   0        0        0      631 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/location.py
+-rw-r--r--   0        0        0      262 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/money.py
+-rw-r--r--   0        0        0      369 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/paging.py
+-rw-r--r--   0        0        0      959 2023-07-17 16:52:36.633877 finch_api-0.0.5/src/finch/types/provider.py
+-rw-r--r--   0        0        0     8383 1970-01-01 00:00:00.000000 finch_api-0.0.5/PKG-INFO
```

### Comparing `finch_api-0.0.4/LICENSE` & `finch_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/README.md` & `finch_api-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/pyproject.toml` & `finch_api-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finch-api"
-version = "0.0.4"
+version = "0.0.5"
 description = "Client library for the Finch API"
 readme = "README.md"
 authors = ["Finch <founders@tryfinch.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/Finch-API/finch-api-python"
 packages = [
   { include = "finch", from = "src" }
```

### Comparing `finch_api-0.0.4/src/finch/__init__.py` & `finch_api-0.0.5/src/finch/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_base_client.py` & `finch_api-0.0.5/src/finch/_base_client.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_base_exceptions.py` & `finch_api-0.0.5/src/finch/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_client.py` & `finch_api-0.0.5/src/finch/_client.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_exceptions.py` & `finch_api-0.0.5/src/finch/_exceptions.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_models.py` & `finch_api-0.0.5/src/finch/_models.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_qs.py` & `finch_api-0.0.5/src/finch/_qs.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_resource.py` & `finch_api-0.0.5/src/finch/_resource.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_streaming.py` & `finch_api-0.0.5/src/finch/_streaming.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_types.py` & `finch_api-0.0.5/src/finch/_types.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_utils/__init__.py` & `finch_api-0.0.5/src/finch/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_utils/_transform.py` & `finch_api-0.0.5/src/finch/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/_utils/_utils.py` & `finch_api-0.0.5/src/finch/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/pagination.py` & `finch_api-0.0.5/src/finch/pagination.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/account.py` & `finch_api-0.0.5/src/finch/resources/account.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/ats/__init__.py` & `finch_api-0.0.5/src/finch/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/ats/applications.py` & `finch_api-0.0.5/src/finch/resources/ats/applications.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/ats/ats.py` & `finch_api-0.0.5/src/finch/resources/ats/ats.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/ats/candidates.py` & `finch_api-0.0.5/src/finch/resources/ats/candidates.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/ats/jobs.py` & `finch_api-0.0.5/src/finch/resources/ats/jobs.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/ats/offers.py` & `finch_api-0.0.5/src/finch/resources/ats/offers.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/ats/stages.py` & `finch_api-0.0.5/src/finch/resources/ats/stages.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/__init__.py` & `finch_api-0.0.5/src/finch/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/benefits/benefits.py` & `finch_api-0.0.5/src/finch/resources/hris/benefits/benefits.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/benefits/individuals.py` & `finch_api-0.0.5/src/finch/resources/hris/benefits/individuals.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/company.py` & `finch_api-0.0.5/src/finch/resources/hris/company.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/directory.py` & `finch_api-0.0.5/src/finch/resources/hris/directory.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/hris.py` & `finch_api-0.0.5/src/finch/resources/hris/hris.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/individuals/employment_data.py` & `finch_api-0.0.5/src/finch/resources/hris/individuals/employment_data.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/individuals/individuals.py` & `finch_api-0.0.5/src/finch/resources/hris/individuals/individuals.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/pay_statements.py` & `finch_api-0.0.5/src/finch/resources/hris/pay_statements.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/hris/payments.py` & `finch_api-0.0.5/src/finch/resources/hris/payments.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/resources/providers.py` & `finch_api-0.0.5/src/finch/resources/providers.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/ats/__init__.py` & `finch_api-0.0.5/src/finch/types/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/ats/application.py` & `finch_api-0.0.5/src/finch/types/ats/application.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/ats/candidate.py` & `finch_api-0.0.5/src/finch/types/ats/candidate.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/ats/job.py` & `finch_api-0.0.5/src/finch/types/ats/job.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/__init__.py` & `finch_api-0.0.5/src/finch/types/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/benefit_create_params.py` & `finch_api-0.0.5/src/finch/types/hris/benefit_create_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/benefit_type.py` & `finch_api-0.0.5/src/finch/types/hris/benefit_type.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/benefits/__init__.py` & `finch_api-0.0.5/src/finch/types/hris/benefits/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/benefits/enrolled_individual.py` & `finch_api-0.0.5/src/finch/types/hris/benefits/enrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/benefits/individual_benefit.py` & `finch_api-0.0.5/src/finch/types/hris/benefits/individual_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/benefits/individual_enroll_many_params.py` & `finch_api-0.0.5/src/finch/types/hris/benefits/individual_enroll_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/benefits/unenrolled_individual.py` & `finch_api-0.0.5/src/finch/types/hris/benefits/unenrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/company.py` & `finch_api-0.0.5/src/finch/types/hris/company.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/company_benefit.py` & `finch_api-0.0.5/src/finch/types/hris/company_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/individual.py` & `finch_api-0.0.5/src/finch/types/hris/individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/individual_in_directory.py` & `finch_api-0.0.5/src/finch/types/hris/individual_in_directory.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/individuals/employment_data.py` & `finch_api-0.0.5/src/finch/types/hris/individuals/employment_data.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py` & `finch_api-0.0.5/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/pay_statement.py` & `finch_api-0.0.5/src/finch/types/hris/pay_statement.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/pay_statement_retrieve_many_params.py` & `finch_api-0.0.5/src/finch/types/hris/pay_statement_retrieve_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/payment.py` & `finch_api-0.0.5/src/finch/types/hris/payment.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/payment_list_params.py` & `finch_api-0.0.5/src/finch/types/hris/payment_list_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/hris/supported_benefit.py` & `finch_api-0.0.5/src/finch/types/hris/supported_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/income.py` & `finch_api-0.0.5/src/finch/types/income.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/introspection.py` & `finch_api-0.0.5/src/finch/types/introspection.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/location.py` & `finch_api-0.0.5/src/finch/types/location.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/src/finch/types/provider.py` & `finch_api-0.0.5/src/finch/types/provider.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.4/PKG-INFO` & `finch_api-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finch-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Client library for the Finch API
 Home-page: https://github.com/Finch-API/finch-api-python
 License: Apache-2.0
 Author: Finch
 Author-email: founders@tryfinch.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

