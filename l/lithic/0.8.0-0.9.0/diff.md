# Comparing `tmp/lithic-0.8.0.tar.gz` & `tmp/lithic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lithic-0.8.0.tar", max compression
+gzip compressed data, was "lithic-0.9.0.tar", max compression
```

## Comparing `lithic-0.8.0.tar` & `lithic-0.9.0.tar`

### file list

```diff
@@ -1,95 +1,108 @@
--rw-r--r--   0        0        0    11336 2023-01-30 03:40:44.288103 lithic-0.8.0/LICENSE
--rw-r--r--   0        0        0    12068 2023-02-01 23:17:06.915127 lithic-0.8.0/README.md
--rw-r--r--   0        0        0     1530 2023-02-01 23:17:58.251660 lithic-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1760 2023-01-30 03:40:47.885253 lithic-0.8.0/src/lithic/__init__.py
--rw-r--r--   0        0        0    34762 2023-02-01 23:17:30.066528 lithic-0.8.0/src/lithic/_base_client.py
--rw-r--r--   0        0        0     3255 2023-01-30 03:40:44.294844 lithic-0.8.0/src/lithic/_base_exceptions.py
--rw-r--r--   0        0        0    13874 2023-01-30 03:40:47.887721 lithic-0.8.0/src/lithic/_client.py
--rw-r--r--   0        0        0      723 2023-01-30 03:40:47.892722 lithic-0.8.0/src/lithic/_exceptions.py
--rw-r--r--   0        0        0     6284 2023-01-30 03:40:47.890882 lithic-0.8.0/src/lithic/_models.py
--rw-r--r--   0        0        0     4781 2023-01-30 03:40:47.889118 lithic-0.8.0/src/lithic/_qs.py
--rw-r--r--   0        0        0      878 2023-01-30 03:40:47.883966 lithic-0.8.0/src/lithic/_resource.py
--rw-r--r--   0        0        0     3863 2023-01-30 03:40:47.878975 lithic-0.8.0/src/lithic/_types.py
--rw-r--r--   0        0        0     1028 2023-01-30 03:40:47.894008 lithic-0.8.0/src/lithic/_utils/__init__.py
--rw-r--r--   0        0        0     3810 2023-01-30 03:40:47.896731 lithic-0.8.0/src/lithic/_utils/_transform.py
--rw-r--r--   0        0        0     8566 2023-01-30 03:40:47.895524 lithic-0.8.0/src/lithic/_utils/_utils.py
--rw-r--r--   0        0        0       97 2023-02-01 23:19:20.500558 lithic-0.8.0/src/lithic/_version.py
--rw-r--r--   0        0        0     1225 2023-01-30 03:40:47.891776 lithic-0.8.0/src/lithic/pagination.py
--rw-r--r--   0        0        0        0 2023-01-30 03:40:44.289497 lithic-0.8.0/src/lithic/py.typed
--rw-r--r--   0        0        0      830 2023-01-30 03:40:47.970505 lithic-0.8.0/src/lithic/resources/__init__.py
--rw-r--r--   0        0        0    57836 2023-02-01 23:17:30.061617 lithic-0.8.0/src/lithic/resources/account_holders.py
--rw-r--r--   0        0        0    11980 2023-01-30 03:40:47.958839 lithic-0.8.0/src/lithic/resources/accounts.py
--rw-r--r--   0        0        0    25259 2023-01-30 03:40:47.973943 lithic-0.8.0/src/lithic/resources/auth_rules.py
--rw-r--r--   0        0        0     7429 2023-01-30 03:40:47.971605 lithic-0.8.0/src/lithic/resources/auth_stream_enrollment.py
--rw-r--r--   0        0        0    57210 2023-02-01 23:17:06.916259 lithic-0.8.0/src/lithic/resources/cards.py
--rw-r--r--   0        0        0    23292 2023-01-30 03:40:47.975870 lithic-0.8.0/src/lithic/resources/funding_sources.py
--rw-r--r--   0        0        0    35030 2023-02-01 23:17:30.062029 lithic-0.8.0/src/lithic/resources/transactions.py
--rw-r--r--   0        0        0     5946 2023-02-01 23:17:06.916544 lithic-0.8.0/src/lithic/types/__init__.py
--rw-r--r--   0        0        0     1419 2023-01-30 03:40:47.951636 lithic-0.8.0/src/lithic/types/account.py
--rw-r--r--   0        0        0     1270 2023-01-30 03:40:47.925033 lithic-0.8.0/src/lithic/types/account_holder.py
--rw-r--r--   0        0        0    10581 2023-02-01 23:17:30.062251 lithic-0.8.0/src/lithic/types/account_holder_create_params.py
--rw-r--r--   0        0        0      351 2023-01-30 03:40:46.460780 lithic-0.8.0/src/lithic/types/account_holder_create_webhook_params.py
--rw-r--r--   0        0        0      435 2023-01-30 03:40:47.941034 lithic-0.8.0/src/lithic/types/account_holder_create_webhook_response.py
--rw-r--r--   0        0        0     1554 2023-02-01 23:13:53.141306 lithic-0.8.0/src/lithic/types/account_holder_document.py
--rw-r--r--   0        0        0      342 2023-01-30 03:40:47.950585 lithic-0.8.0/src/lithic/types/account_holder_list_documents_response.py
--rw-r--r--   0        0        0     1994 2023-02-01 23:17:06.916887 lithic-0.8.0/src/lithic/types/account_holder_resubmit_params.py
--rw-r--r--   0        0        0      668 2023-01-30 03:40:46.500177 lithic-0.8.0/src/lithic/types/account_holder_update_params.py
--rw-r--r--   0        0        0      471 2023-01-30 03:40:47.899347 lithic-0.8.0/src/lithic/types/account_holder_update_response.py
--rw-r--r--   0        0        0      422 2023-01-30 03:40:46.524920 lithic-0.8.0/src/lithic/types/account_holder_upload_document_params.py
--rw-r--r--   0        0        0      604 2023-01-30 03:40:46.530718 lithic-0.8.0/src/lithic/types/account_list_params.py
--rw-r--r--   0        0        0     1790 2023-01-30 03:40:46.554220 lithic-0.8.0/src/lithic/types/account_update_params.py
--rw-r--r--   0        0        0      197 2023-01-30 03:40:47.924018 lithic-0.8.0/src/lithic/types/api_status.py
--rw-r--r--   0        0        0     2048 2023-01-30 03:40:47.946663 lithic-0.8.0/src/lithic/types/auth_rule.py
--rw-r--r--   0        0        0      786 2023-01-30 03:40:46.637203 lithic-0.8.0/src/lithic/types/auth_rule_apply_params.py
--rw-r--r--   0        0        0      263 2023-01-30 03:40:47.898499 lithic-0.8.0/src/lithic/types/auth_rule_apply_response.py
--rw-r--r--   0        0        0     2009 2023-01-30 03:40:46.581566 lithic-0.8.0/src/lithic/types/auth_rule_create_params.py
--rw-r--r--   0        0        0      265 2023-01-30 03:40:47.905816 lithic-0.8.0/src/lithic/types/auth_rule_create_response.py
--rw-r--r--   0        0        0      321 2023-01-30 03:40:46.631196 lithic-0.8.0/src/lithic/types/auth_rule_list_params.py
--rw-r--r--   0        0        0      788 2023-01-30 03:40:46.603049 lithic-0.8.0/src/lithic/types/auth_rule_remove_params.py
--rw-r--r--   0        0        0      367 2023-01-30 03:40:47.903543 lithic-0.8.0/src/lithic/types/auth_rule_remove_response.py
--rw-r--r--   0        0        0      281 2023-01-30 03:40:47.923228 lithic-0.8.0/src/lithic/types/auth_rule_retrieve_response.py
--rw-r--r--   0        0        0     1356 2023-01-30 03:40:46.626933 lithic-0.8.0/src/lithic/types/auth_rule_update_params.py
--rw-r--r--   0        0        0      265 2023-01-30 03:40:47.913789 lithic-0.8.0/src/lithic/types/auth_rule_update_response.py
--rw-r--r--   0        0        0      256 2023-01-30 03:40:47.928284 lithic-0.8.0/src/lithic/types/auth_stream_enrollment.py
--rw-r--r--   0        0        0      335 2023-01-30 03:40:46.638682 lithic-0.8.0/src/lithic/types/auth_stream_enrollment_enroll_params.py
--rw-r--r--   0        0        0     4569 2023-02-01 23:17:06.917237 lithic-0.8.0/src/lithic/types/card.py
--rw-r--r--   0        0        0     5089 2023-01-30 03:40:47.915748 lithic-0.8.0/src/lithic/types/card_create_params.py
--rw-r--r--   0        0        0      410 2023-01-30 03:40:46.683161 lithic-0.8.0/src/lithic/types/card_embed_params.py
--rw-r--r--   0        0        0      112 2023-01-30 03:40:46.658873 lithic-0.8.0/src/lithic/types/card_embed_response.py
--rw-r--r--   0        0        0     1333 2023-01-30 03:40:46.663442 lithic-0.8.0/src/lithic/types/card_get_embed_html_params.py
--rw-r--r--   0        0        0     1331 2023-01-30 03:40:46.670187 lithic-0.8.0/src/lithic/types/card_get_embed_url_params.py
--rw-r--r--   0        0        0      891 2023-01-30 03:40:46.696941 lithic-0.8.0/src/lithic/types/card_list_params.py
--rw-r--r--   0        0        0     1145 2023-01-30 03:40:46.668029 lithic-0.8.0/src/lithic/types/card_provision_params.py
--rw-r--r--   0        0        0      234 2023-01-30 03:40:47.941922 lithic-0.8.0/src/lithic/types/card_provision_response.py
--rw-r--r--   0        0        0     1115 2023-01-30 03:40:47.908130 lithic-0.8.0/src/lithic/types/card_reissue_params.py
--rw-r--r--   0        0        0      483 2023-01-30 03:40:46.675588 lithic-0.8.0/src/lithic/types/card_retrieve_params.py
--rw-r--r--   0        0        0     2918 2023-01-30 03:40:46.709937 lithic-0.8.0/src/lithic/types/card_update_params.py
--rw-r--r--   0        0        0     1317 2023-01-30 03:40:47.942723 lithic-0.8.0/src/lithic/types/embed_request_params.py
--rw-r--r--   0        0        0     1440 2023-01-30 03:40:47.914709 lithic-0.8.0/src/lithic/types/funding_source.py
--rw-r--r--   0        0        0     1566 2023-01-30 03:40:46.699524 lithic-0.8.0/src/lithic/types/funding_source_create_params.py
--rw-r--r--   0        0        0      355 2023-01-30 03:40:46.690960 lithic-0.8.0/src/lithic/types/funding_source_list_params.py
--rw-r--r--   0        0        0      944 2023-01-30 03:40:46.693676 lithic-0.8.0/src/lithic/types/funding_source_update_params.py
--rw-r--r--   0        0        0      715 2023-01-30 03:40:46.711604 lithic-0.8.0/src/lithic/types/funding_source_verify_params.py
--rw-r--r--   0        0        0      159 2023-02-01 23:17:06.917374 lithic-0.8.0/src/lithic/types/shared/__init__.py
--rw-r--r--   0        0        0      867 2023-02-01 23:17:06.917467 lithic-0.8.0/src/lithic/types/shared/address.py
--rw-r--r--   0        0        0     1534 2023-01-30 03:40:47.954699 lithic-0.8.0/src/lithic/types/shared/shipping_address.py
--rw-r--r--   0        0        0      159 2023-02-01 23:17:06.917593 lithic-0.8.0/src/lithic/types/shared_params/__init__.py
--rw-r--r--   0        0        0      908 2023-02-01 23:17:06.917671 lithic-0.8.0/src/lithic/types/shared_params/address.py
--rw-r--r--   0        0        0     1565 2023-01-30 03:40:47.956302 lithic-0.8.0/src/lithic/types/shared_params/shipping_address.py
--rw-r--r--   0        0        0      205 2023-02-01 23:17:06.917880 lithic-0.8.0/src/lithic/types/spend_limit_duration.py
--rw-r--r--   0        0        0    15766 2023-02-01 23:17:30.062506 lithic-0.8.0/src/lithic/types/transaction.py
--rw-r--r--   0        0        0      969 2023-01-30 03:40:46.708365 lithic-0.8.0/src/lithic/types/transaction_list_params.py
--rw-r--r--   0        0        0     2548 2023-02-01 23:17:30.062654 lithic-0.8.0/src/lithic/types/transaction_simulate_authorization_params.py
--rw-r--r--   0        0        0      486 2023-01-30 03:40:47.952827 lithic-0.8.0/src/lithic/types/transaction_simulate_authorization_response.py
--rw-r--r--   0        0        0      705 2023-01-30 03:40:46.713254 lithic-0.8.0/src/lithic/types/transaction_simulate_clearing_params.py
--rw-r--r--   0        0        0      328 2023-01-30 03:40:47.945714 lithic-0.8.0/src/lithic/types/transaction_simulate_clearing_response.py
--rw-r--r--   0        0        0      750 2023-02-01 23:17:30.062798 lithic-0.8.0/src/lithic/types/transaction_simulate_credit_authorization_params.py
--rw-r--r--   0        0        0      432 2023-01-30 03:40:47.939501 lithic-0.8.0/src/lithic/types/transaction_simulate_credit_authorization_response.py
--rw-r--r--   0        0        0      443 2023-01-30 03:40:46.722116 lithic-0.8.0/src/lithic/types/transaction_simulate_return_params.py
--rw-r--r--   0        0        0      406 2023-01-30 03:40:47.900122 lithic-0.8.0/src/lithic/types/transaction_simulate_return_response.py
--rw-r--r--   0        0        0      376 2023-01-30 03:40:46.720703 lithic-0.8.0/src/lithic/types/transaction_simulate_return_reversal_params.py
--rw-r--r--   0        0        0      340 2023-01-30 03:40:47.911877 lithic-0.8.0/src/lithic/types/transaction_simulate_return_reversal_response.py
--rw-r--r--   0        0        0      835 2023-01-30 03:40:46.724360 lithic-0.8.0/src/lithic/types/transaction_simulate_void_params.py
--rw-r--r--   0        0        0      320 2023-01-30 03:40:47.921933 lithic-0.8.0/src/lithic/types/transaction_simulate_void_response.py
--rw-r--r--   0        0        0    13410 1970-01-01 00:00:00.000000 lithic-0.8.0/setup.py
--rw-r--r--   0        0        0    12963 1970-01-01 00:00:00.000000 lithic-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2023-02-18 00:41:05.866324 lithic-0.9.0/LICENSE
+-rw-r--r--   0        0        0    12068 2023-02-18 00:41:07.950434 lithic-0.9.0/README.md
+-rw-r--r--   0        0        0     1530 2023-02-18 00:45:03.690332 lithic-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1760 2023-02-18 00:41:08.527432 lithic-0.9.0/src/lithic/__init__.py
+-rw-r--r--   0        0        0       22 2023-02-18 00:45:03.718660 lithic-0.9.0/src/lithic/__version.py
+-rw-r--r--   0        0        0    36010 2023-02-18 00:41:08.525836 lithic-0.9.0/src/lithic/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-02-18 00:41:07.065755 lithic-0.9.0/src/lithic/_base_exceptions.py
+-rw-r--r--   0        0        0    14032 2023-02-18 00:41:08.529577 lithic-0.9.0/src/lithic/_client.py
+-rw-r--r--   0        0        0      723 2023-02-18 00:41:08.533610 lithic-0.9.0/src/lithic/_exceptions.py
+-rw-r--r--   0        0        0     6284 2023-02-18 00:41:08.532064 lithic-0.9.0/src/lithic/_models.py
+-rw-r--r--   0        0        0     4781 2023-02-18 00:41:08.530675 lithic-0.9.0/src/lithic/_qs.py
+-rw-r--r--   0        0        0      878 2023-02-18 00:41:08.526569 lithic-0.9.0/src/lithic/_resource.py
+-rw-r--r--   0        0        0     3863 2023-02-18 00:41:08.522105 lithic-0.9.0/src/lithic/_types.py
+-rw-r--r--   0        0        0     1028 2023-02-18 00:41:08.535042 lithic-0.9.0/src/lithic/_utils/__init__.py
+-rw-r--r--   0        0        0     3810 2023-02-18 00:41:08.537581 lithic-0.9.0/src/lithic/_utils/_transform.py
+-rw-r--r--   0        0        0     8566 2023-02-18 00:41:08.536374 lithic-0.9.0/src/lithic/_utils/_utils.py
+-rw-r--r--   0        0        0       97 2023-02-18 00:41:07.036524 lithic-0.9.0/src/lithic/_version.py
+-rw-r--r--   0        0        0     3161 2023-02-18 00:41:08.532908 lithic-0.9.0/src/lithic/pagination.py
+-rw-r--r--   0        0        0        0 2023-02-18 00:41:05.863994 lithic-0.9.0/src/lithic/py.typed
+-rw-r--r--   0        0        0      903 2023-02-18 00:41:08.618074 lithic-0.9.0/src/lithic/resources/__init__.py
+-rw-r--r--   0        0        0    57824 2023-02-18 00:41:08.617085 lithic-0.9.0/src/lithic/resources/account_holders.py
+-rw-r--r--   0        0        0    11980 2023-02-18 00:41:08.607872 lithic-0.9.0/src/lithic/resources/accounts.py
+-rw-r--r--   0        0        0    25259 2023-02-18 00:41:08.621029 lithic-0.9.0/src/lithic/resources/auth_rules.py
+-rw-r--r--   0        0        0     7161 2023-02-18 00:41:33.482933 lithic-0.9.0/src/lithic/resources/auth_stream_enrollment.py
+-rw-r--r--   0        0        0    57210 2023-02-18 00:41:08.613669 lithic-0.9.0/src/lithic/resources/cards.py
+-rw-r--r--   0        0        0      231 2023-02-18 00:41:07.107833 lithic-0.9.0/src/lithic/resources/events/__init__.py
+-rw-r--r--   0        0        0     8165 2023-02-18 00:41:33.489556 lithic-0.9.0/src/lithic/resources/events/events.py
+-rw-r--r--   0        0        0    21305 2023-02-18 00:41:33.483484 lithic-0.9.0/src/lithic/resources/events/subscriptions.py
+-rw-r--r--   0        0        0    23292 2023-02-18 00:41:08.622748 lithic-0.9.0/src/lithic/resources/funding_sources.py
+-rw-r--r--   0        0        0    33672 2023-02-18 00:41:08.610194 lithic-0.9.0/src/lithic/resources/transactions.py
+-rw-r--r--   0        0        0     6189 2023-02-18 00:41:33.483689 lithic-0.9.0/src/lithic/types/__init__.py
+-rw-r--r--   0        0        0     1419 2023-02-18 00:41:08.589421 lithic-0.9.0/src/lithic/types/account.py
+-rw-r--r--   0        0        0     1270 2023-02-18 00:41:08.566475 lithic-0.9.0/src/lithic/types/account_holder.py
+-rw-r--r--   0        0        0    10572 2023-02-18 00:41:08.587223 lithic-0.9.0/src/lithic/types/account_holder_create_params.py
+-rw-r--r--   0        0        0      351 2023-02-18 00:41:08.578628 lithic-0.9.0/src/lithic/types/account_holder_create_webhook_params.py
+-rw-r--r--   0        0        0      435 2023-02-18 00:41:08.580702 lithic-0.9.0/src/lithic/types/account_holder_create_webhook_response.py
+-rw-r--r--   0        0        0     1551 2023-02-18 00:41:08.544075 lithic-0.9.0/src/lithic/types/account_holder_document.py
+-rw-r--r--   0        0        0      342 2023-02-18 00:41:08.588696 lithic-0.9.0/src/lithic/types/account_holder_list_documents_response.py
+-rw-r--r--   0        0        0     1994 2023-02-18 00:41:08.575468 lithic-0.9.0/src/lithic/types/account_holder_resubmit_params.py
+-rw-r--r--   0        0        0      668 2023-02-18 00:41:08.222743 lithic-0.9.0/src/lithic/types/account_holder_update_params.py
+-rw-r--r--   0        0        0      471 2023-02-18 00:41:08.541593 lithic-0.9.0/src/lithic/types/account_holder_update_response.py
+-rw-r--r--   0        0        0      422 2023-02-18 00:41:08.588066 lithic-0.9.0/src/lithic/types/account_holder_upload_document_params.py
+-rw-r--r--   0        0        0      604 2023-02-18 00:41:08.221458 lithic-0.9.0/src/lithic/types/account_list_params.py
+-rw-r--r--   0        0        0     1790 2023-02-18 00:41:08.217317 lithic-0.9.0/src/lithic/types/account_update_params.py
+-rw-r--r--   0        0        0      197 2023-02-18 00:41:08.565548 lithic-0.9.0/src/lithic/types/api_status.py
+-rw-r--r--   0        0        0     2048 2023-02-18 00:41:08.585629 lithic-0.9.0/src/lithic/types/auth_rule.py
+-rw-r--r--   0        0        0      786 2023-02-18 00:41:08.205389 lithic-0.9.0/src/lithic/types/auth_rule_apply_params.py
+-rw-r--r--   0        0        0      263 2023-02-18 00:41:08.540915 lithic-0.9.0/src/lithic/types/auth_rule_apply_response.py
+-rw-r--r--   0        0        0     2009 2023-02-18 00:41:08.218323 lithic-0.9.0/src/lithic/types/auth_rule_create_params.py
+-rw-r--r--   0        0        0      265 2023-02-18 00:41:08.547865 lithic-0.9.0/src/lithic/types/auth_rule_create_response.py
+-rw-r--r--   0        0        0      321 2023-02-18 00:41:08.220088 lithic-0.9.0/src/lithic/types/auth_rule_list_params.py
+-rw-r--r--   0        0        0      788 2023-02-18 00:41:08.222448 lithic-0.9.0/src/lithic/types/auth_rule_remove_params.py
+-rw-r--r--   0        0        0      367 2023-02-18 00:41:08.545676 lithic-0.9.0/src/lithic/types/auth_rule_remove_response.py
+-rw-r--r--   0        0        0      281 2023-02-18 00:41:08.564738 lithic-0.9.0/src/lithic/types/auth_rule_retrieve_response.py
+-rw-r--r--   0        0        0     1356 2023-02-18 00:41:08.218903 lithic-0.9.0/src/lithic/types/auth_rule_update_params.py
+-rw-r--r--   0        0        0      265 2023-02-18 00:41:08.555258 lithic-0.9.0/src/lithic/types/auth_rule_update_response.py
+-rw-r--r--   0        0        0      256 2023-02-18 00:41:08.569677 lithic-0.9.0/src/lithic/types/auth_stream_enrollment.py
+-rw-r--r--   0        0        0      335 2023-02-18 00:41:08.203606 lithic-0.9.0/src/lithic/types/auth_stream_enrollment_enroll_params.py
+-rw-r--r--   0        0        0     4569 2023-02-18 00:41:08.567632 lithic-0.9.0/src/lithic/types/card.py
+-rw-r--r--   0        0        0     5089 2023-02-18 00:41:08.557857 lithic-0.9.0/src/lithic/types/card_create_params.py
+-rw-r--r--   0        0        0      410 2023-02-18 00:41:08.218186 lithic-0.9.0/src/lithic/types/card_embed_params.py
+-rw-r--r--   0        0        0      112 2023-02-18 00:41:08.221369 lithic-0.9.0/src/lithic/types/card_embed_response.py
+-rw-r--r--   0        0        0     1333 2023-02-18 00:41:08.563378 lithic-0.9.0/src/lithic/types/card_get_embed_html_params.py
+-rw-r--r--   0        0        0     1331 2023-02-18 00:41:08.576276 lithic-0.9.0/src/lithic/types/card_get_embed_url_params.py
+-rw-r--r--   0        0        0      891 2023-02-18 00:41:08.218655 lithic-0.9.0/src/lithic/types/card_list_params.py
+-rw-r--r--   0        0        0     1145 2023-02-18 00:41:08.204500 lithic-0.9.0/src/lithic/types/card_provision_params.py
+-rw-r--r--   0        0        0      234 2023-02-18 00:41:08.581383 lithic-0.9.0/src/lithic/types/card_provision_response.py
+-rw-r--r--   0        0        0     1115 2023-02-18 00:41:08.550031 lithic-0.9.0/src/lithic/types/card_reissue_params.py
+-rw-r--r--   0        0        0      483 2023-02-18 00:41:08.206596 lithic-0.9.0/src/lithic/types/card_retrieve_params.py
+-rw-r--r--   0        0        0     2918 2023-02-18 00:41:08.205011 lithic-0.9.0/src/lithic/types/card_update_params.py
+-rw-r--r--   0        0        0     1317 2023-02-18 00:41:08.582064 lithic-0.9.0/src/lithic/types/embed_request_params.py
+-rw-r--r--   0        0        0      691 2023-02-18 00:41:08.544899 lithic-0.9.0/src/lithic/types/event.py
+-rw-r--r--   0        0        0      957 2023-02-18 00:41:33.489680 lithic-0.9.0/src/lithic/types/event_list_params.py
+-rw-r--r--   0        0        0     1323 2023-02-18 00:41:33.483791 lithic-0.9.0/src/lithic/types/event_resend_params.py
+-rw-r--r--   0        0        0      534 2023-02-18 00:41:08.562009 lithic-0.9.0/src/lithic/types/event_subscription.py
+-rw-r--r--   0        0        0      514 2023-02-18 00:41:08.604390 lithic-0.9.0/src/lithic/types/events/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-18 00:41:08.602995 lithic-0.9.0/src/lithic/types/events/subscription_create_params.py
+-rw-r--r--   0        0        0      561 2023-02-18 00:41:08.219780 lithic-0.9.0/src/lithic/types/events/subscription_list_params.py
+-rw-r--r--   0        0        0      244 2023-02-18 00:41:08.605138 lithic-0.9.0/src/lithic/types/events/subscription_retrieve_secret_response.py
+-rw-r--r--   0        0        0      741 2023-02-18 00:41:08.218668 lithic-0.9.0/src/lithic/types/events/subscription_update_params.py
+-rw-r--r--   0        0        0     1440 2023-02-18 00:41:08.556052 lithic-0.9.0/src/lithic/types/funding_source.py
+-rw-r--r--   0        0        0     1566 2023-02-18 00:41:08.546571 lithic-0.9.0/src/lithic/types/funding_source_create_params.py
+-rw-r--r--   0        0        0      355 2023-02-18 00:41:08.222708 lithic-0.9.0/src/lithic/types/funding_source_list_params.py
+-rw-r--r--   0        0        0      944 2023-02-18 00:41:08.220956 lithic-0.9.0/src/lithic/types/funding_source_update_params.py
+-rw-r--r--   0        0        0      715 2023-02-18 00:41:08.549311 lithic-0.9.0/src/lithic/types/funding_source_verify_params.py
+-rw-r--r--   0        0        0      159 2023-02-18 00:41:07.341708 lithic-0.9.0/src/lithic/types/shared/__init__.py
+-rw-r--r--   0        0        0      867 2023-02-18 00:41:08.592490 lithic-0.9.0/src/lithic/types/shared/address.py
+-rw-r--r--   0        0        0     1534 2023-02-18 00:41:08.593476 lithic-0.9.0/src/lithic/types/shared/shipping_address.py
+-rw-r--r--   0        0        0      159 2023-02-18 00:41:07.343383 lithic-0.9.0/src/lithic/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      908 2023-02-18 00:41:08.596278 lithic-0.9.0/src/lithic/types/shared_params/address.py
+-rw-r--r--   0        0        0     1565 2023-02-18 00:41:08.597353 lithic-0.9.0/src/lithic/types/shared_params/shipping_address.py
+-rw-r--r--   0        0        0      205 2023-02-18 00:41:08.219549 lithic-0.9.0/src/lithic/types/spend_limit_duration.py
+-rw-r--r--   0        0        0    13747 2023-02-18 00:41:08.553179 lithic-0.9.0/src/lithic/types/transaction.py
+-rw-r--r--   0        0        0      969 2023-02-18 00:41:08.218552 lithic-0.9.0/src/lithic/types/transaction_list_params.py
+-rw-r--r--   0        0        0     2548 2023-02-18 00:41:08.577106 lithic-0.9.0/src/lithic/types/transaction_simulate_authorization_params.py
+-rw-r--r--   0        0        0      486 2023-02-18 00:41:08.590123 lithic-0.9.0/src/lithic/types/transaction_simulate_authorization_response.py
+-rw-r--r--   0        0        0      705 2023-02-18 00:41:08.590880 lithic-0.9.0/src/lithic/types/transaction_simulate_clearing_params.py
+-rw-r--r--   0        0        0      328 2023-02-18 00:41:08.584746 lithic-0.9.0/src/lithic/types/transaction_simulate_clearing_response.py
+-rw-r--r--   0        0        0      750 2023-02-18 00:41:08.550784 lithic-0.9.0/src/lithic/types/transaction_simulate_credit_authorization_params.py
+-rw-r--r--   0        0        0      432 2023-02-18 00:41:08.579285 lithic-0.9.0/src/lithic/types/transaction_simulate_credit_authorization_response.py
+-rw-r--r--   0        0        0      443 2023-02-18 00:41:08.582752 lithic-0.9.0/src/lithic/types/transaction_simulate_return_params.py
+-rw-r--r--   0        0        0      406 2023-02-18 00:41:08.542376 lithic-0.9.0/src/lithic/types/transaction_simulate_return_response.py
+-rw-r--r--   0        0        0      376 2023-02-18 00:41:08.580036 lithic-0.9.0/src/lithic/types/transaction_simulate_return_reversal_params.py
+-rw-r--r--   0        0        0      340 2023-02-18 00:41:08.553868 lithic-0.9.0/src/lithic/types/transaction_simulate_return_reversal_response.py
+-rw-r--r--   0        0        0      835 2023-02-18 00:41:08.554543 lithic-0.9.0/src/lithic/types/transaction_simulate_void_params.py
+-rw-r--r--   0        0        0      320 2023-02-18 00:41:08.564038 lithic-0.9.0/src/lithic/types/transaction_simulate_void_response.py
+-rw-r--r--   0        0        0    13462 1970-01-01 00:00:00.000000 lithic-0.9.0/setup.py
+-rw-r--r--   0        0        0    12963 1970-01-01 00:00:00.000000 lithic-0.9.0/PKG-INFO
```

### Comparing `lithic-0.8.0/LICENSE` & `lithic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/README.md` & `lithic-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/pyproject.toml` & `lithic-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lithic"
-version = "0.8.0"
+version = "0.9.0"
 description = "Client library for the lithic API"
 readme = "README.md"
 authors = ["Lithic <sdk-feedback@lithic.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/lithic-com/lithic-python"
 packages = [
   { include = "lithic", from = "src" }
```

### Comparing `lithic-0.8.0/src/lithic/__init__.py` & `lithic-0.9.0/src/lithic/__init__.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_base_client.py` & `lithic-0.9.0/src/lithic/_base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Optional,
     Generator,
     AsyncIterator,
     cast,
     overload,
 )
 from functools import lru_cache
-from typing_extensions import Literal
+from typing_extensions import Literal, get_args, get_origin
 
 import anyio
 import httpx
 import distro
 import pydantic
 from httpx import URL
 from pydantic import PrivateAttr
@@ -289,36 +289,39 @@
         self._custom_headers = custom_headers or {}
         self._custom_query = custom_query or {}
         self._strict_response_validation = _strict_response_validation
         self._idempotency_header = None
 
     def _make_status_error(self, request: httpx.Request, response: httpx.Response) -> APIStatusError:
         err_text = response.text.strip()
+        body = err_text
+
         try:
-            err_msg = json.loads(err_text)
-        except:
-            err_msg = err_text or "Unknown"
+            body = json.loads(err_text)
+            err_msg = f"Error code: {response.status_code}"
+        except Exception:
+            err_msg = err_text or f"Error code: {response.status_code}"
 
         if response.status_code == 400:
-            return exceptions.BadRequestError(err_msg, request, response)
+            return exceptions.BadRequestError(err_msg, request=request, response=response, body=body)
         if response.status_code == 401:
-            return exceptions.AuthenticationError(err_msg, request, response)
+            return exceptions.AuthenticationError(err_msg, request=request, response=response, body=body)
         if response.status_code == 403:
-            return exceptions.PermissionDeniedError(err_msg, request, response)
+            return exceptions.PermissionDeniedError(err_msg, request=request, response=response, body=body)
         if response.status_code == 404:
-            return exceptions.NotFoundError(err_msg, request, response)
+            return exceptions.NotFoundError(err_msg, request=request, response=response, body=body)
         if response.status_code == 409:
-            return exceptions.ConflictError(err_msg, request, response)
+            return exceptions.ConflictError(err_msg, request=request, response=response, body=body)
         if response.status_code == 422:
-            return exceptions.UnprocessableEntityError(err_msg, request, response)
+            return exceptions.UnprocessableEntityError(err_msg, request=request, response=response, body=body)
         if response.status_code == 429:
-            return exceptions.RateLimitError(err_msg, request, response)
+            return exceptions.RateLimitError(err_msg, request=request, response=response, body=body)
         if response.status_code >= 500:
-            return exceptions.InternalServerError(err_msg, request, response)
-        return APIStatusError(err_msg, request, response)
+            return exceptions.InternalServerError(err_msg, request=request, response=response, body=body)
+        return APIStatusError(err_msg, request=request, response=response, body=body)
 
     def remaining_retries(
         self,
         remaining_retries: Optional[int],
         options: FinalRequestOptions,
     ) -> int:
         return remaining_retries if remaining_retries is not None else options.get_max_retries(self.max_retries)
@@ -402,21 +405,41 @@
 
     def process_response(
         self,
         *,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         response: httpx.Response,
+        _strict: bool = False,
     ) -> ResponseT:
         if cast_to is NoneType:
             return cast(ResponseT, None)
 
         if cast_to == str:
             return cast(ResponseT, response.text)
 
+        # TODO: try to handle Unions better…
+        if get_origin(cast_to) is Union:
+            members = get_args(cast_to)
+            for member in members:
+                try:
+                    return cast(
+                        ResponseT,
+                        self.process_response(cast_to=member, options=options, response=response, _strict=True),
+                    )
+                except:
+                    continue
+            # If nobody matches exactly, try again loosely.
+            for member in members:
+                try:
+                    return cast(ResponseT, self.process_response(cast_to=member, options=options, response=response))
+                except:
+                    continue
+            raise ValueError(f"Response did not match any type in union {members}")
+
         if issubclass(cast_to, httpx.Response):
             # Because of the invariance of our ResponseT TypeVar, users can subclass httpx.Response
             # and pass that class to our request functions. We cannot change the variance to be either
             # covariant or contravariant as that makes our usage of ResponseT illegal. We could construct
             # the response class ourselves but that is something that should be supported directly in httpx
             # as it would be easy to incorrectly construct the Response object due to the multitude of arguments.
             if cast_to != httpx.Response:
@@ -450,15 +473,15 @@
         if cast_to is UnknownResponse:
             return cast(ResponseT, data)
 
         if issubclass(cast_to, ModelBuilderProtocol):
             return cast(ResponseT, cast_to.build(response=response, data=data))
 
         model_cls = cast(Type[BaseModel], cast_to)
-        if self._strict_response_validation:
+        if _strict or self._strict_response_validation:
             return cast(ResponseT, model_cls(**data))
 
         return cast(ResponseT, model_cls.construct(**data))
 
     @property
     def qs(self) -> Querystring:
         return Querystring()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lithic-0.8.0/src/lithic/_base_exceptions.py` & `lithic-0.9.0/src/lithic/_base_exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,81 +25,89 @@
 
 class APIStatusError(APIError):
     """Raised when an API response has a status code of 4xx or 5xx."""
 
     response: Response
     status_code: int
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
+    body: object
+    """The API response body.
+
+    If the API responded with a valid JSON structure then this property will be the decoded result.
+    If it isn't a valid JSON structure then this will be the raw response.
+    """
+
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
         super().__init__(message, request)
         self.response = response
         self.status_code = response.status_code
+        self.body = body
 
 
 class BadRequestError(APIStatusError):
     status_code: Literal[400]
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = 400
 
 
 class AuthenticationError(APIStatusError):
     status_code: Literal[401]
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = 401
 
 
 class PermissionDeniedError(APIStatusError):
     status_code: Literal[403]
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = 403
 
 
 class NotFoundError(APIStatusError):
     status_code: Literal[404]
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = 404
 
 
 class ConflictError(APIStatusError):
     status_code: Literal[409]
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = 409
 
 
 class UnprocessableEntityError(APIStatusError):
     status_code: Literal[422]
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = 422
 
 
 class RateLimitError(APIStatusError):
     status_code: Literal[429]
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = 429
 
 
 class InternalServerError(APIStatusError):
     status_code: int
 
-    def __init__(self, message: str, request: Request, response: Response) -> None:
-        super().__init__(message, request, response)
+    def __init__(self, message: str, *, request: Request, response: Response, body: object) -> None:
+        super().__init__(message, request=request, response=response, body=body)
         self.status_code = response.status_code
 
 
 class APIConnectionError(APIError):
     def __init__(self, request: Request, message: str = "Connection error.") -> None:
         super().__init__(message, request)
```

### Comparing `lithic-0.8.0/src/lithic/_client.py` & `lithic-0.9.0/src/lithic/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 class Lithic(SyncAPIClient):
     accounts: resources.Accounts
     account_holders: resources.AccountHolders
     auth_rules: resources.AuthRules
     auth_stream_enrollment: resources.AuthStreamEnrollmentResource
     cards: resources.Cards
+    events: resources.Events
     funding_sources: resources.FundingSources
     transactions: resources.Transactions
 
     # client options
     api_key: str
 
     _environment: Literal["production", "sandbox"]
@@ -119,14 +120,15 @@
         self.api_key = api_key
 
         self.accounts = resources.Accounts(self)
         self.account_holders = resources.AccountHolders(self)
         self.auth_rules = resources.AuthRules(self)
         self.auth_stream_enrollment = resources.AuthStreamEnrollmentResource(self)
         self.cards = resources.Cards(self)
+        self.events = resources.Events(self)
         self.funding_sources = resources.FundingSources(self)
         self.transactions = resources.Transactions(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
@@ -205,14 +207,15 @@
 
 class AsyncLithic(AsyncAPIClient):
     accounts: resources.AsyncAccounts
     account_holders: resources.AsyncAccountHolders
     auth_rules: resources.AsyncAuthRules
     auth_stream_enrollment: resources.AsyncAuthStreamEnrollmentResource
     cards: resources.AsyncCards
+    events: resources.AsyncEvents
     funding_sources: resources.AsyncFundingSources
     transactions: resources.AsyncTransactions
 
     # client options
     api_key: str
 
     _environment: Literal["production", "sandbox"]
@@ -274,14 +277,15 @@
         self.api_key = api_key
 
         self.accounts = resources.AsyncAccounts(self)
         self.account_holders = resources.AsyncAccountHolders(self)
         self.auth_rules = resources.AsyncAuthRules(self)
         self.auth_stream_enrollment = resources.AsyncAuthStreamEnrollmentResource(self)
         self.cards = resources.AsyncCards(self)
+        self.events = resources.AsyncEvents(self)
         self.funding_sources = resources.AsyncFundingSources(self)
         self.transactions = resources.AsyncTransactions(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
```

### Comparing `lithic-0.8.0/src/lithic/_exceptions.py` & `lithic-0.9.0/src/lithic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_models.py` & `lithic-0.9.0/src/lithic/_models.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_qs.py` & `lithic-0.9.0/src/lithic/_qs.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_resource.py` & `lithic-0.9.0/src/lithic/_resource.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_types.py` & `lithic-0.9.0/src/lithic/_types.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_utils/__init__.py` & `lithic-0.9.0/src/lithic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_utils/_transform.py` & `lithic-0.9.0/src/lithic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/_utils/_utils.py` & `lithic-0.9.0/src/lithic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/resources/__init__.py` & `lithic-0.9.0/src/lithic/resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from .cards import Cards, AsyncCards
+from .events import Events, AsyncEvents
 from .accounts import Accounts, AsyncAccounts
 from .auth_rules import AuthRules, AsyncAuthRules
 from .transactions import Transactions, AsyncTransactions
 from .account_holders import AccountHolders, AsyncAccountHolders
 from .funding_sources import FundingSources, AsyncFundingSources
 from .auth_stream_enrollment import (
     AuthStreamEnrollmentResource,
@@ -18,12 +19,14 @@
     "AsyncAccountHolders",
     "AuthRules",
     "AsyncAuthRules",
     "AuthStreamEnrollmentResource",
     "AsyncAuthStreamEnrollmentResource",
     "Cards",
     "AsyncCards",
+    "Events",
+    "AsyncEvents",
     "FundingSources",
     "AsyncFundingSources",
     "Transactions",
     "AsyncTransactions",
 ]
```

### Comparing `lithic-0.8.0/src/lithic/resources/account_holders.py` & `lithic-0.9.0/src/lithic/resources/account_holders.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 class AccountHolders(SyncAPIResource):
     @overload
     def create(
         self,
         *,
         business_entity: account_holder_create_params.KYBBusinessEntity,
-        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntities],
-        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividuals],
+        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntity],
+        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividual],
         control_person: account_holder_create_params.KYBControlPerson,
         kyb_passed_timestamp: str | NotGiven = NOT_GIVEN,
         nature_of_business: str,
         tos_timestamp: str,
         website_url: str,
         workflow: Literal["KYB_BASIC", "KYB_BYO"],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -215,16 +215,16 @@
         ["individual", "tos_timestamp", "workflow"],
         ["workflow", "kyc_exemption_type", "first_name", "last_name", "email", "phone_number"],
     )
     def create(
         self,
         *,
         business_entity: account_holder_create_params.KYBBusinessEntity | NotGiven = NOT_GIVEN,
-        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntities] | NotGiven = NOT_GIVEN,
-        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividuals]
+        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntity] | NotGiven = NOT_GIVEN,
+        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividual]
         | NotGiven = NOT_GIVEN,
         control_person: account_holder_create_params.KYBControlPerson | NotGiven = NOT_GIVEN,
         kyb_passed_timestamp: str | NotGiven = NOT_GIVEN,
         nature_of_business: str | NotGiven = NOT_GIVEN,
         tos_timestamp: str | str | NotGiven = NOT_GIVEN,
         website_url: str | NotGiven = NOT_GIVEN,
         workflow: Literal["KYB_BASIC", "KYB_BYO"]
@@ -615,16 +615,16 @@
 
 class AsyncAccountHolders(AsyncAPIResource):
     @overload
     async def create(
         self,
         *,
         business_entity: account_holder_create_params.KYBBusinessEntity,
-        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntities],
-        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividuals],
+        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntity],
+        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividual],
         control_person: account_holder_create_params.KYBControlPerson,
         kyb_passed_timestamp: str | NotGiven = NOT_GIVEN,
         nature_of_business: str,
         tos_timestamp: str,
         website_url: str,
         workflow: Literal["KYB_BASIC", "KYB_BYO"],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -805,16 +805,16 @@
         ["individual", "tos_timestamp", "workflow"],
         ["workflow", "kyc_exemption_type", "first_name", "last_name", "email", "phone_number"],
     )
     async def create(
         self,
         *,
         business_entity: account_holder_create_params.KYBBusinessEntity | NotGiven = NOT_GIVEN,
-        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntities] | NotGiven = NOT_GIVEN,
-        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividuals]
+        beneficial_owner_entities: List[account_holder_create_params.KYBBeneficialOwnerEntity] | NotGiven = NOT_GIVEN,
+        beneficial_owner_individuals: List[account_holder_create_params.KYBBeneficialOwnerIndividual]
         | NotGiven = NOT_GIVEN,
         control_person: account_holder_create_params.KYBControlPerson | NotGiven = NOT_GIVEN,
         kyb_passed_timestamp: str | NotGiven = NOT_GIVEN,
         nature_of_business: str | NotGiven = NOT_GIVEN,
         tos_timestamp: str | str | NotGiven = NOT_GIVEN,
         website_url: str | NotGiven = NOT_GIVEN,
         workflow: Literal["KYB_BASIC", "KYB_BYO"]
```

### Comparing `lithic-0.8.0/src/lithic/resources/accounts.py` & `lithic-0.9.0/src/lithic/resources/accounts.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/resources/auth_rules.py` & `lithic-0.9.0/src/lithic/resources/auth_rules.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/resources/auth_stream_enrollment.py` & `lithic-0.9.0/src/lithic/resources/auth_stream_enrollment.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> None:
         """Disenroll Authorization Stream Access (ASA) in Sandbox."""
-        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
         return self._delete(
             "/auth_stream",
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=NoneType,
         )
 
     def enroll(
@@ -76,15 +75,14 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
-        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
         return self._post(
             "/auth_stream",
             body={"webhook_url": webhook_url},
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=NoneType,
         )
 
@@ -115,15 +113,14 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> None:
         """Disenroll Authorization Stream Access (ASA) in Sandbox."""
-        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
         return await self._delete(
             "/auth_stream",
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=NoneType,
         )
 
     async def enroll(
@@ -155,14 +152,13 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
-        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
         return await self._post(
             "/auth_stream",
             body={"webhook_url": webhook_url},
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=NoneType,
         )
```

### Comparing `lithic-0.8.0/src/lithic/resources/cards.py` & `lithic-0.9.0/src/lithic/resources/cards.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/resources/funding_sources.py` & `lithic-0.9.0/src/lithic/resources/funding_sources.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/resources/transactions.py` & `lithic-0.9.0/src/lithic/resources/transactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,15 @@
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> Transaction:
-        """
-        Get specific transaction.
-
-        _Note that the transaction object returned via this endpoint will be changing in
-        Sandbox on January 4, 2023 and in Production on February 8, 2023. Please refer
-        to [this page](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes)
-        for more information._
-        """
+        """Get specific transaction."""
         return self._get(
             f"/transactions/{transaction_token}",
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Transaction,
         )
 
     def list(
@@ -61,19 +54,14 @@
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[Transaction]:
         """
         List transactions.
 
-        _Note that the transaction object returned via this endpoint will be changing in
-        Sandbox on January 4, 2023 and in Production on February 8, 2023. Please refer
-        to [this page](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes)
-        for more information._
-
         Args:
           account_token: Filters for transactions associated with a specific account.
 
           card_token: Filters for transactions associated with a specific card.
 
           result: Filters for transactions using transaction result field. Can filter by
               `APPROVED`, and `DECLINED`.
@@ -352,16 +340,15 @@
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> TransactionSimulateReturnReversalResponse:
         """
         Voids a settled credit transaction – i.e., a transaction with a negative amount
         and `SETTLED` status. These can be credit authorizations that have already
-        cleared or financial credit authorizations. This endpoint will be available
-        beginning January 4, 2023.
+        cleared or financial credit authorizations.
 
         Args:
           token: The transaction token returned from the /v1/simulate/authorize response.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -432,22 +419,15 @@
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> Transaction:
-        """
-        Get specific transaction.
-
-        _Note that the transaction object returned via this endpoint will be changing in
-        Sandbox on January 4, 2023 and in Production on February 8, 2023. Please refer
-        to [this page](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes)
-        for more information._
-        """
+        """Get specific transaction."""
         return await self._get(
             f"/transactions/{transaction_token}",
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Transaction,
         )
 
     def list(
@@ -465,19 +445,14 @@
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[Transaction, AsyncPage[Transaction]]:
         """
         List transactions.
 
-        _Note that the transaction object returned via this endpoint will be changing in
-        Sandbox on January 4, 2023 and in Production on February 8, 2023. Please refer
-        to [this page](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes)
-        for more information._
-
         Args:
           account_token: Filters for transactions associated with a specific account.
 
           card_token: Filters for transactions associated with a specific card.
 
           result: Filters for transactions using transaction result field. Can filter by
               `APPROVED`, and `DECLINED`.
@@ -756,16 +731,15 @@
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> TransactionSimulateReturnReversalResponse:
         """
         Voids a settled credit transaction – i.e., a transaction with a negative amount
         and `SETTLED` status. These can be credit authorizations that have already
-        cleared or financial credit authorizations. This endpoint will be available
-        beginning January 4, 2023.
+        cleared or financial credit authorizations.
 
         Args:
           token: The transaction token returned from the /v1/simulate/authorize response.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
```

### Comparing `lithic-0.8.0/src/lithic/types/__init__.py` & `lithic-0.9.0/src/lithic/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from .card import Card as Card
+from .event import Event as Event
 from .shared import Address as Address
 from .shared import ShippingAddress as ShippingAddress
 from .account import Account as Account
 from .auth_rule import AuthRule as AuthRule
 from .api_status import APIStatus as APIStatus
 from .transaction import Transaction as Transaction
 from .account_holder import AccountHolder as AccountHolder
 from .funding_source import FundingSource as FundingSource
 from .card_list_params import CardListParams as CardListParams
 from .card_embed_params import CardEmbedParams as CardEmbedParams
+from .event_list_params import EventListParams as EventListParams
 from .card_create_params import CardCreateParams as CardCreateParams
 from .card_update_params import CardUpdateParams as CardUpdateParams
+from .event_subscription import EventSubscription as EventSubscription
 from .account_list_params import AccountListParams as AccountListParams
 from .card_embed_response import CardEmbedResponse as CardEmbedResponse
 from .card_reissue_params import CardReissueParams as CardReissueParams
+from .event_resend_params import EventResendParams as EventResendParams
 from .card_retrieve_params import CardRetrieveParams as CardRetrieveParams
 from .embed_request_params import EmbedRequestParams as EmbedRequestParams
 from .spend_limit_duration import SpendLimitDuration as SpendLimitDuration
 from .account_update_params import AccountUpdateParams as AccountUpdateParams
 from .auth_rule_list_params import AuthRuleListParams as AuthRuleListParams
 from .card_provision_params import CardProvisionParams as CardProvisionParams
 from .auth_rule_apply_params import AuthRuleApplyParams as AuthRuleApplyParams
```

### Comparing `lithic-0.8.0/src/lithic/types/account.py` & `lithic-0.9.0/src/lithic/types/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import List, Optional
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["SpendLimit", "Account"]
+__all__ = ["Account", "SpendLimit"]
 
 
 class SpendLimit(BaseModel):
     daily: int
     """Daily spend limit (in cents)."""
 
     lifetime: int
```

### Comparing `lithic-0.8.0/src/lithic/types/account_holder.py` & `lithic-0.9.0/src/lithic/types/account_holder.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/account_holder_create_params.py` & `lithic-0.9.0/src/lithic/types/account_holder_create_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from typing import List, Union
 from typing_extensions import Literal, Required, TypedDict
 
 from ..types import shared_params
 
 __all__ = [
+    "AccountHolderCreateParams",
+    "KYB",
     "KYBBusinessEntity",
-    "KYBBeneficialOwnerEntities",
-    "KYBBeneficialOwnerIndividuals",
+    "KYBBeneficialOwnerEntity",
+    "KYBBeneficialOwnerIndividual",
     "KYBControlPerson",
-    "KYB",
-    "KYCIndividual",
     "KYC",
+    "KYCIndividual",
     "KYCExempt",
-    "AccountHolderCreateParams",
 ]
 
 
 class KYBBusinessEntity(TypedDict, total=False):
     address: Required[shared_params.Address]
     """
     Business's physical address - PO boxes, UPS drops, and FedEx drops are not
@@ -49,15 +49,15 @@
     (if applicable).
     """
 
     parent_company: str
     """Parent company name (if applicable)."""
 
 
-class KYBBeneficialOwnerEntities(TypedDict, total=False):
+class KYBBeneficialOwnerEntity(TypedDict, total=False):
     address: Required[shared_params.Address]
     """
     Business's physical address - PO boxes, UPS drops, and FedEx drops are not
     acceptable; APO/FPO are acceptable.
     """
 
     government_id: Required[str]
@@ -82,15 +82,15 @@
     (if applicable).
     """
 
     parent_company: str
     """Parent company name (if applicable)."""
 
 
-class KYBBeneficialOwnerIndividuals(TypedDict, total=False):
+class KYBBeneficialOwnerIndividual(TypedDict, total=False):
     address: Required[shared_params.Address]
     """
     Individual's current address - PO boxes, UPS drops, and FedEx drops are not
     acceptable; APO/FPO are acceptable. Only USA addresses are currently supported.
     """
 
     dob: Required[str]
@@ -151,26 +151,26 @@
     """Individual's last name, as it appears on government-issued identity documents."""
 
     phone_number: Required[str]
     """Individual's phone number, entered in E.164 format."""
 
 
 class KYB(TypedDict, total=False):
-    beneficial_owner_entities: Required[List[KYBBeneficialOwnerEntities]]
+    beneficial_owner_entities: Required[List[KYBBeneficialOwnerEntity]]
     """List of all entities with >25% ownership in the company.
 
     If no entity or individual owns >25% of the company, and the largest shareholder
     is an entity, please identify them in this field. See
     [FinCEN requirements](https://www.fincen.gov/sites/default/files/shared/CDD_Rev6.7_Sept_2017_Certificate.pdf)
     (Section I) for more background. If no business owner is an entity, pass in an
     empty list. However, either this parameter or `beneficial_owner_individuals`
     must be populated. on entities that should be included.
     """
 
-    beneficial_owner_individuals: Required[List[KYBBeneficialOwnerIndividuals]]
+    beneficial_owner_individuals: Required[List[KYBBeneficialOwnerIndividual]]
     """List of all individuals with >25% ownership in the company.
 
     If no entity or individual owns >25% of the company, and the largest shareholder
     is an individual, please identify them in this field. See
     [FinCEN requirements](https://www.fincen.gov/sites/default/files/shared/CDD_Rev6.7_Sept_2017_Certificate.pdf)
     (Section I) for more background on individuals that should be included. If no
     individual is an entity, pass in an empty list. However, either this parameter
```

### Comparing `lithic-0.8.0/src/lithic/types/account_holder_document.py` & `lithic-0.9.0/src/lithic/types/account_holder_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import List, Optional
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["RequiredDocumentUploads", "AccountHolderDocument"]
+__all__ = ["AccountHolderDocument", "RequiredDocumentUpload"]
 
 
-class RequiredDocumentUploads(BaseModel):
+class RequiredDocumentUpload(BaseModel):
     image_type: Optional[Literal["back", "front"]]
     """Type of image to upload."""
 
     status: Optional[Literal["COMPLETED", "FAILED", "PENDING", "UPLOADED"]]
     """Status of document image upload."""
 
     status_reasons: Optional[
@@ -40,11 +40,11 @@
 class AccountHolderDocument(BaseModel):
     account_holder_token: Optional[str]
     """Globally unique identifier for the account holder."""
 
     document_type: Optional[Literal["commercial_license", "drivers_license", "passport", "passport_card", "visa"]]
     """Type of documentation to be submitted for verification."""
 
-    required_document_uploads: Optional[List[RequiredDocumentUploads]]
+    required_document_uploads: Optional[List[RequiredDocumentUpload]]
 
     token: Optional[str]
     """Globally unique identifier for the document."""
```

### Comparing `lithic-0.8.0/src/lithic/types/account_holder_resubmit_params.py` & `lithic-0.9.0/src/lithic/types/account_holder_resubmit_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from typing_extensions import Literal, Required, TypedDict
 
 from ..types import shared_params
 
-__all__ = ["Individual", "AccountHolderResubmitParams"]
+__all__ = ["AccountHolderResubmitParams", "Individual"]
 
 
 class Individual(TypedDict, total=False):
     address: Required[shared_params.Address]
     """
     Individual's current address - PO boxes, UPS drops, and FedEx drops are not
     acceptable; APO/FPO are acceptable. Only USA addresses are currently supported.
```

### Comparing `lithic-0.8.0/src/lithic/types/account_holder_update_params.py` & `lithic-0.9.0/src/lithic/types/account_holder_update_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/account_list_params.py` & `lithic-0.9.0/src/lithic/types/account_list_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/account_update_params.py` & `lithic-0.9.0/src/lithic/types/account_update_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing_extensions import Literal, TypedDict
 
-__all__ = ["VerificationAddress", "AccountUpdateParams"]
+__all__ = ["AccountUpdateParams", "VerificationAddress"]
 
 
 class VerificationAddress(TypedDict, total=False):
     address1: str
 
     address2: str
```

### Comparing `lithic-0.8.0/src/lithic/types/auth_rule.py` & `lithic-0.9.0/src/lithic/types/auth_rule.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/auth_rule_apply_params.py` & `lithic-0.9.0/src/lithic/types/auth_rule_apply_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/auth_rule_create_params.py` & `lithic-0.9.0/src/lithic/types/auth_rule_create_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/auth_rule_remove_params.py` & `lithic-0.9.0/src/lithic/types/auth_rule_remove_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/auth_rule_update_params.py` & `lithic-0.9.0/src/lithic/types/auth_rule_update_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card.py` & `lithic-0.9.0/src/lithic/types/card.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card_create_params.py` & `lithic-0.9.0/src/lithic/types/card_create_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card_get_embed_html_params.py` & `lithic-0.9.0/src/lithic/types/card_get_embed_html_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card_get_embed_url_params.py` & `lithic-0.9.0/src/lithic/types/card_get_embed_url_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card_list_params.py` & `lithic-0.9.0/src/lithic/types/card_list_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card_provision_params.py` & `lithic-0.9.0/src/lithic/types/card_provision_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card_reissue_params.py` & `lithic-0.9.0/src/lithic/types/card_reissue_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/card_update_params.py` & `lithic-0.9.0/src/lithic/types/card_update_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/embed_request_params.py` & `lithic-0.9.0/src/lithic/types/embed_request_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/funding_source.py` & `lithic-0.9.0/src/lithic/types/funding_source.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/funding_source_create_params.py` & `lithic-0.9.0/src/lithic/types/funding_source_create_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Union
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["Bank", "Plaid", "FundingSourceCreateParams"]
+__all__ = ["FundingSourceCreateParams", "Bank", "Plaid"]
 
 
 class Bank(TypedDict, total=False):
     account_number: Required[str]
     """The account number of the bank account."""
 
     routing_number: Required[str]
```

### Comparing `lithic-0.8.0/src/lithic/types/funding_source_update_params.py` & `lithic-0.9.0/src/lithic/types/funding_source_update_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/funding_source_verify_params.py` & `lithic-0.9.0/src/lithic/types/funding_source_verify_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/shared/address.py` & `lithic-0.9.0/src/lithic/types/shared/address.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/shared/shipping_address.py` & `lithic-0.9.0/src/lithic/types/shared/shipping_address.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/shared_params/address.py` & `lithic-0.9.0/src/lithic/types/shared_params/address.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/shared_params/shipping_address.py` & `lithic-0.9.0/src/lithic/types/shared_params/shipping_address.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/transaction.py` & `lithic-0.9.0/src/lithic/types/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import List, Optional
 from typing_extensions import Literal
 
 from pydantic import Field
 
-from ..types import card
 from .._models import BaseModel
 
-__all__ = ["CardholderAuthentication", "Events", "Funding", "Merchant", "Transaction"]
+__all__ = ["Transaction", "CardholderAuthentication", "Event", "Merchant"]
 
 
 class CardholderAuthentication(BaseModel):
     three_ds_version: Optional[str] = Field(alias="3ds_version")
     """3-D Secure Protocol version. Possible values:
 
     - `1`: 3-D Secure Protocol version 1.x applied to the transaction.
@@ -111,15 +110,15 @@
     - `C`: Challenge Required
     - `D`: Challenge Required; decoupled authentication confirmed
     - `I`: Informational only
     - `S`: Challenge using Secure Payment Confirmation (SPC)
     """
 
 
-class Events(BaseModel):
+class Event(BaseModel):
     amount: int
     """Amount of the transaction event (in cents), including any acquirer fees."""
 
     created: str
     """ISO 8601 date and time this event entered the system. UTC time zone."""
 
     result: Literal[
@@ -214,33 +213,14 @@
     - `FINANCIAL_AUTHORIZATION` - A request from a merchant to debit funds without
       additional clearing.
     - `FINANCIAL_CREDIT_AUTHORIZATION` - A request from a merchant to refund or
       credit funds without additional clearing.
     - `RETURN` - A refund has been processed on the transaction.
     - `RETURN_REVERSAL` - A refund has been reversed (e.g., when a merchant reverses
       an incorrect refund).
-    - `VOID` - Note this value will be removed with the February API changes (see
-      https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes). A
-      transaction has been voided (e.g., when a merchant reverses an incorrect
-      authorization).
-    """
-
-
-class Funding(BaseModel):
-    amount: Optional[int]
-    """Amount of the transaction event, including any acquirer fees."""
-
-    token: Optional[str]
-    """Funding account token."""
-
-    type: Optional[Literal["DEPOSITORY_CHECKING", "DEPOSITORY_SAVINGS"]]
-    """Types of funding:
-
-    - `DEPOSITORY_CHECKING` - Bank checking account.
-    - `DEPOSITORY_SAVINGS` - Bank savings account.
     """
 
 
 class Merchant(BaseModel):
     acceptor_id: Optional[str]
     """Unique identifier to identify the payment card acceptor."""
 
@@ -288,47 +268,25 @@
 
     authorization_code: Optional[str]
     """
     A fixed-width 6-digit numeric identifier that can be used to identify a
     transaction with networks.
     """
 
-    card: Optional[card.Card]
-    """
-    Note this field will be removed with the
-    [February API changes](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes).
-    Card used in this transaction.
-    """
-
     card_token: Optional[str]
-    """Token for the card used in this transaction. Note this field is not yet
-    included.
-
-    It will be added as part of the
-    [February API changes](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes).
-    """
+    """Token for the card used in this transaction."""
 
     cardholder_authentication: Optional[CardholderAuthentication]
 
     created: Optional[str]
     """Date and time when the transaction first occurred. UTC time zone."""
 
-    events: Optional[List[Events]]
+    events: Optional[List[Event]]
     """A list of all events that have modified this transaction."""
 
-    funding: Optional[List[Funding]]
-    """
-    Note this field will be removed with the
-    [February API changes](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes).
-    A list of objects that describe how this transaction was funded, with the
-    `amount` represented in cents. A reference to the funding account for the `card`
-    that made this transaction may appear here and the `token` will match the
-    `token` for the funding account in the `card` field.
-    """
-
     merchant: Optional[Merchant]
 
     merchant_amount: Optional[int]
     """
     Analogous to the "amount" property, but will represent the amount in the
     transaction's local currency (smallest unit), including any acquirer fees.
     """
@@ -382,23 +340,17 @@
     Amount of the transaction that has been settled (in cents), including any
     acquirer fees. This may change over time.
     """
 
     status: Optional[Literal["BOUNCED", "DECLINED", "EXPIRED", "PENDING", "SETTLED", "SETTLING", "VOIDED"]]
     """Status types:
 
-    - `BOUNCED` - The transaction was bounced. Note this value will be removed with
-      the
-      [February API changes](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes).
     - `DECLINED` - The transaction was declined.
     - `EXPIRED` - Lithic reversed the authorization as it has passed its expiration
       time.
     - `PENDING` - Authorization is pending completion from the merchant.
     - `SETTLED` - The transaction is complete.
-    - `SETTLING` - The merchant has completed the transaction and the funding source
-      is being debited. Note this value will be removed with the
-      [February API changes](https://docs.lithic.com/docs/guide-to-q1-2023-lithic-api-changes).
     - `VOIDED` - The merchant has voided the previously pending authorization.
     """
 
     token: Optional[str]
     """Globally unique identifier."""
```

### Comparing `lithic-0.8.0/src/lithic/types/transaction_list_params.py` & `lithic-0.9.0/src/lithic/types/transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/transaction_simulate_authorization_params.py` & `lithic-0.9.0/src/lithic/types/transaction_simulate_authorization_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/transaction_simulate_clearing_params.py` & `lithic-0.9.0/src/lithic/types/transaction_simulate_clearing_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/transaction_simulate_credit_authorization_params.py` & `lithic-0.9.0/src/lithic/types/transaction_simulate_credit_authorization_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/src/lithic/types/transaction_simulate_void_params.py` & `lithic-0.9.0/src/lithic/types/transaction_simulate_void_params.py`

 * *Files identical despite different names*

### Comparing `lithic-0.8.0/setup.py` & `lithic-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['lithic',
  'lithic._utils',
  'lithic.resources',
+ 'lithic.resources.events',
  'lithic.types',
+ 'lithic.types.events',
  'lithic.types.shared',
  'lithic.types.shared_params']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -20,15 +22,15 @@
  'distro>=1.7.0',
  'httpx>=0.23.0',
  'pydantic>=1.9.0',
  'typing-extensions>=4.1.1']
 
 setup_kwargs = {
     'name': 'lithic',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Client library for the lithic API',
     'long_description': '# Lithic Python API Library\n\n> **Migration Guide**\n>\n> We\'ve made some major improvements to how you pass arguments to methods which will require migrating your existing code.\n>\n> If you want to migrate to the new patterns incrementally you can do so by installing `v0.5.0`. This release contains both\n> the new and old patterns with a backwards compatibility layer.\n>\n> You can find a guide to migrating in [this document](#migration-guide).\n\n[![PyPI version](https://img.shields.io/pypi/v/lithic.svg)](https://pypi.org/project/lithic/)\n\nThe Lithic Python library provides convenient access to the Lithic REST API from any Python 3.7+\napplication. It includes type definitions for all request params and response fields,\nand offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).\n\n## Documentation\n\nThe API documentation can be found [here](https://docs.lithic.com).\n\n## Installation\n\n```sh\npip install lithic\n```\n\n## Usage\n\n```python\nfrom lithic import Lithic\n\nlithic = Lithic(\n    # defaults to os.environ.get("LITHIC_API_KEY")\n    api_key="my api key",\n    # defaults to "production".\n    environment="sandbox",\n)\n\ncard = lithic.cards.create(\n    type="SINGLE_USE",\n)\nprint(card.token)\n```\n\nWhile you can provide an `api_key` keyword argument, we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)\nand adding `LITHIC_API_KEY="my api key"` to your `.env` file so that your API Key is not stored in source control.\n\n## Async Usage\n\nSimply import `AsyncLithic` instead of `Lithic` and use `await` with each API call:\n\n```python\nfrom lithic import AsyncLithic\n\nlithic = AsyncLithic(\n    # defaults to os.environ.get("LITHIC_API_KEY")\n    api_key="my api key",\n    # defaults to "production".\n    environment="sandbox",\n)\n\n\nasync def main():\n    card = await lithic.cards.create(\n        type="SINGLE_USE",\n    )\n    print(card.token)\n\n\nasyncio.run(main())\n```\n\nFunctionality between the synchronous and asynchronous clients is otherwise identical.\n\n## Using Types\n\nNested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict), while responses are [Pydantic](https://pydantic-docs.helpmanual.io/) models. This helps provide autocomplete and documentation within your editor.\n\nIf you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `"basic"`.\n\n## Pagination\n\nList methods in the Lithic API are paginated.\n\nThis library provides auto-paginating iterators with each list response, so you do not have to request successive pages manually:\n\n```python\nimport lithic\n\nlithic = Lithic()\n\nall_cards = []\n# Automatically fetches more pages as needed.\nfor card in lithic.cards.list():\n    # Do something with card here\n    all_cards.append(card)\nprint(all_cards)\n```\n\nOr, asynchronously:\n\n```python\nimport asyncio\nimport lithic\n\nlithic = AsyncLithic()\n\n\nasync def main() -> None:\n    all_cards = []\n    # Iterate through items across all pages, issuing requests as needed.\n    async for card in lithic.cards.list():\n        all_cards.append(card)\n    print(all_cards)\n\n\nasyncio.run(main())\n```\n\nAlternatively, you can use the `.has_next_page()`, `.next_page_info()`, or `.get_next_page()` methods for more granular control working with pages:\n\n```python\nfirst_page = await lithic.cards.list()\nif first_page.has_next_page():\n    print(f"will fetch next page using these details: {first_page.next_page_info()}")\n    next_page = await first_page.get_next_page()\n    print(f"number of items we just fetched: {len(next_page.data)}")\n\n# Remove `await` for non-async usage.\n```\n\nOr just work directly with the returned data:\n\n```python\nfirst_page = await lithic.cards.list()\n\nprint(f"page number: {first_page.page}")  # => "page number: 1"\nfor card in first_page.data:\n    print(card.created)\n\n# Remove `await` for non-async usage.\n```\n\n## Nested params\n\nNested parameters are dictionaries, typed using `TypedDict`, for example:\n\n```py\nfrom lithic import Lithic\n\nlithic = Lithic()\n\nlithic.cards.create(\n    foo={\n        "bar": True\n    },\n)\n```\n\n## Handling errors\n\nWhen the library is unable to connect to the API (e.g., due to network connection problems or a timeout), a subclass of `lithic.APIConnectionError` is raised.\n\nWhen the API returns a non-success status code (i.e., 4xx or 5xx\nresponse), a subclass of `lithic.APIStatusError` will be raised, containing `status_code` and `response` properties.\n\nAll errors inherit from `lithic.APIError`.\n\n```python\nfrom lithic import Lithic\n\nlithic = Lithic()\n\ntry:\n    lithic.cards.create(\n        type="an_incorrect_type",\n    )\nexcept lithic.APIConnectionError as e:\n    print("The server could not be reached")\n    print(e.__cause__)  # an underlying Exception, likely raised within httpx.\nexcept lithic.RateLimitError as e:\n    print("A 429 status code was received; we should back off a bit.")\nexcept lithic.APIStatusError as e:\n    print("Another non-200-range status code was received")\n    print(e.status_code)\n    print(e.response)\n```\n\nError codes are as followed:\n\n| Status Code | Error Type                 |\n| ----------- | -------------------------- |\n| 400         | `BadRequestError`          |\n| 401         | `AuthenticationError`      |\n| 403         | `PermissionDeniedError`    |\n| 404         | `NotFoundError`            |\n| 422         | `UnprocessableEntityError` |\n| 429         | `RateLimitError`           |\n| >=500       | `InternalServerError`      |\n| N/A         | `APIConnectionError`       |\n\n### Retries\n\nCertain errors will be automatically retried 2 times by default, with a short exponential backoff.\nConnection errors (for example, due to a network connectivity problem), 409 Conflict, 429 Rate Limit,\nand >=500 Internal errors will all be retried by default.\n\nYou can use the `max_retries` option to configure or disable this:\n\n```python\nfrom lithic import Lithic\n\n# Configure the default for all requests:\nlithic = Lithic(\n    # default is 2\n    max_retries=0,\n)\n\n# Or, configure per-request:\nlithic.with_options(max_retries=5).cards.list(\n    page_size=10,\n)\n```\n\n### Timeouts\n\nRequests time out after 60 seconds by default. You can configure this with a `timeout` option,\nwhich accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):\n\n```python\nfrom lithic import Lithic\n\n# Configure the default for all requests:\nlithic = Lithic(\n    # default is 60s\n    timeout=20.0,\n)\n\n# More granular control:\nlithic = Lithic(\n    timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),\n)\n\n# Override per-request:\nlithic.with_options(timeout=5 * 1000).cards.list(\n    page_size=10,\n)\n```\n\nOn timeout, an `APITimeoutError` is thrown.\n\nNote that requests which time out will be [retried twice by default](#retries).\n\n## Advanced: Configuring custom URLs, proxies, and transports\n\nYou can configure the following keyword arguments when instantiating the client:\n\n```python\nimport httpx\nfrom lithic import Lithic\n\nlithic = Lithic(\n    # Use a custom base URL\n    base_url="http://my.test.server.example.com:8083",\n    proxies="http://my.test.proxy.example.com",\n    transport=httpx.HTTPTransport(local_address="0.0.0.0"),\n)\n```\n\nSee the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.\n\n# Migration guide\n\nThis section outlines the features that were deprecated in `v0.5.0`, and subsequently removed in `v0.6.0` and how to migrate your code.\n\n## Breaking changes\n\n### TypedDict → keyword arguments\n\nThe way you pass arguments to methods has been changed from a single `TypedDict` to individual arguments. For example, this snippet:\n\n```python\ncard = await client.cards.create({"type": "VIRTUAL"})\n```\n\nNow becomes:\n\n```python\ncard = await client.cards.create(type="VIRTUAL")\n```\n\n#### Migrating\n\nThe easiest way to make your code compatible with this change is to add `**{`, for example:\n\n```diff\n- card = await client.cards.create({\'type\': \'VIRTUAL\'})\n+ card = await client.cards.create(**{\'type\': \'VIRTUAL\'})\n```\n\nHowever, it is highly recommended to completely switch to explicit keyword arguments:\n\n```diff\n- card = await client.cards.create({\'type\': \'VIRTUAL\'})\n+ card = await client.cards.create(type=\'VIRTUAL\')\n```\n\n### Named path arguments\n\nAll but the last path parameter must now be passed as named arguments instead of positional arguments, for example, for a method that calls the endpoint `/account_holders/{account_holder_token}/documents/{document_token}` you would\'ve been able to call the method like this:\n\n```python\ncard = await client.account_holders.retrieve(\n    "account_holder_token", "my_document_token"\n)\n```\n\nBut now you must call the method like this:\n\n```python\ncard = await client.account_holders.retrieve(\n    "my_document_token", account_holder_token="account_holder_token"\n)\n```\n\nIf you have type checking enabled in your IDE it will tell you which parts of your code need to be updated.\n\n### Request options\n\nYou used to be able to set request options on a per-method basis, now you can only set them on the client. There are two methods that you can use to make this easy, `with_options` and `copy`.\n\nIf you need to make multiple requests with changed options, you can use `.copy()` to get a new client object with those options. This can be useful if you need to set a custom header for multiple requests, for example:\n\n```python\ncopied = client.copy(default_headers={"X-My-Header": "Foo"})\ncard = await copied.cards.create(type="VIRTUAL")\nawait copied.cards.provision(card.token, digital_wallet="GOOGLE_PAY")\n```\n\nIf you just need to override one of the client options for one request, you can use `.with_options()`, for example:\n\n```python\nawait client.with_options(timeout=None).cards.create(type="VIRTUAL")\n```\n\nIt should be noted that the `.with_options()` method is simply an alias to `.copy()`, you can use them interchangeably.\n\nYou can pass nearly every argument that is supported by the Client `__init__` method to the `.copy()` method, except for `proxies` and `transport`.\n\n```python\ncopied = client.copy(\n    api_key="...",\n    environment="sandbox",\n    timeout=httpx.Timeout(read=10),\n    max_retries=5,\n    default_headers={\n        "X-My-Header": "value",\n    },\n    default_query={\n        "my_default_param": "value",\n    },\n)\n```\n\n## New features\n\n### Pass custom headers\n\nIf you need to add additional headers to a request you can easily do so with the `extra_headers` argument:\n\n```python\ncard = await client.cards.create(\n    type="VIRTUAL",\n    extra_headers={\n        "X-Foo": "my header",\n    },\n)\n```\n\n### Pass custom JSON properties\n\nYou can add additional properties to the JSON request body that are not included directly in the method definition through the `extra_body` argument. This can be useful when there are in new properties in the API that are in beta and aren\'t in the SDK yet.\n\n```python\ncard = await client.cards.create(\n    type="VIRTUAL",\n    extra_body={\n        "special_prop": "foo",\n    },\n)\n# sends this to the API:\n# {"type": "VIRTUAL", "special_prop": "foo"}\n```\n\n### Pass custom query parameters\n\nYou can add additional query parameters that aren\'t specified in the method definition through the `extra_query` argument. This can be useful when there are any new/beta query parameters that are not yet in the SDK.\n\n```python\ncard = await client.cards.create(\n    type="VIRTUAL",\n    extra_query={\n        "special_param": "bar",\n    },\n)\n# makes the request to this URL:\n# https://api.lithic.com/v1/cards?special_param=bar\n```\n\n## Status\n\nThis package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;\nplease reach out if you rely on any undocumented behavior.\n\nWe are keen for your feedback; please email us at [sdk-feedback@lithic.com](mailto:sdk-feedback@lithic.com) or open an issue with questions,\nbugs, or suggestions.\n\n## Requirements\n\nPython 3.7 or higher.',
     'author': 'Lithic',
     'author_email': 'sdk-feedback@lithic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lithic-com/lithic-python',
```

### Comparing `lithic-0.8.0/PKG-INFO` & `lithic-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lithic
-Version: 0.8.0
+Version: 0.9.0
 Summary: Client library for the lithic API
 Home-page: https://github.com/lithic-com/lithic-python
 License: Apache-2.0
 Author: Lithic
 Author-email: sdk-feedback@lithic.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

