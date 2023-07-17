# Comparing `tmp/increase-0.8.1.tar.gz` & `tmp/increase-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increase-0.8.1.tar", max compression
+gzip compressed data, was "increase-0.9.0.tar", max compression
```

## Comparing `increase-0.8.1.tar` & `increase-0.9.0.tar`

### file list

```diff
@@ -1,210 +1,211 @@
--rw-r--r--   0        0        0    11338 2023-07-01 00:24:38.031246 increase-0.8.1/LICENSE
--rw-r--r--   0        0        0     8418 2023-07-01 00:24:38.031246 increase-0.8.1/README.md
--rw-r--r--   0        0        0     1881 2023-07-01 00:24:38.031246 increase-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2587 2023-07-01 00:24:38.031246 increase-0.8.1/src/increase/__init__.py
--rw-r--r--   0        0        0    46808 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_base_client.py
--rw-r--r--   0        0        0     3889 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_base_exceptions.py
--rw-r--r--   0        0        0    26762 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_client.py
--rw-r--r--   0        0        0    10875 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_models.py
--rw-r--r--   0        0        0     4846 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_qs.py
--rw-r--r--   0        0        0      890 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_resource.py
--rw-r--r--   0        0        0     5884 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_streaming.py
--rw-r--r--   0        0        0     4229 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_types.py
--rw-r--r--   0        0        0     1277 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_utils/_utils.py
--rw-r--r--   0        0        0      127 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_version.py
--rw-r--r--   0        0        0     1109 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/pagination.py
--rw-r--r--   0        0        0        0 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/py.typed
--rw-r--r--   0        0        0     4478 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/__init__.py
--rw-r--r--   0        0        0    15065 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/account_numbers.py
--rw-r--r--   0        0        0     7400 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/account_statements.py
--rw-r--r--   0        0        0    18102 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/account_transfers.py
--rw-r--r--   0        0        0    18476 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/accounts.py
--rw-r--r--   0        0        0    15600 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/ach_prenotifications.py
--rw-r--r--   0        0        0    26071 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/ach_transfers.py
--rw-r--r--   0        0        0     4285 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/balance_lookups.py
--rw-r--r--   0        0        0     8651 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/bookkeeping_accounts.py
--rw-r--r--   0        0        0     4122 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/bookkeeping_entries.py
--rw-r--r--   0        0        0     4842 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/bookkeeping_entry_sets.py
--rw-r--r--   0        0        0    10707 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/card_disputes.py
--rw-r--r--   0        0        0    10597 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/card_profiles.py
--rw-r--r--   0        0        0    19120 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/cards.py
--rw-r--r--   0        0        0    11757 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/check_deposits.py
--rw-r--r--   0        0        0    23188 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/check_transfers.py
--rw-r--r--   0        0        0     7771 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/declined_transactions.py
--rw-r--r--   0        0        0     7353 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/digital_wallet_tokens.py
--rw-r--r--   0        0        0     7177 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/documents.py
--rw-r--r--   0        0        0      282 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/entities/__init__.py
--rw-r--r--   0        0        0    14010 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/entities/entities.py
--rw-r--r--   0        0        0     8071 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/entities/supplemental_documents.py
--rw-r--r--   0        0        0    18799 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/event_subscriptions.py
--rw-r--r--   0        0        0     7154 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/events.py
--rw-r--r--   0        0        0    10548 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/exports.py
--rw-r--r--   0        0        0    15315 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/external_accounts.py
--rw-r--r--   0        0        0    12929 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/files.py
--rw-r--r--   0        0        0     2040 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/groups.py
--rw-r--r--   0        0        0    12035 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/inbound_ach_transfer_returns.py
--rw-r--r--   0        0        0     7075 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0    14231 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/limits.py
--rw-r--r--   0        0        0     6593 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/oauth_connections.py
--rw-r--r--   0        0        0     8344 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/pending_transactions.py
--rw-r--r--   0        0        0     6300 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/programs.py
--rw-r--r--   0        0        0     8536 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/real_time_decisions.py
--rw-r--r--   0        0        0    14968 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4951 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/routing_numbers.py
--rw-r--r--   0        0        0     1989 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/__init__.py
--rw-r--r--   0        0        0     4026 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/account_statements.py
--rw-r--r--   0        0        0     4024 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/account_transfers.py
--rw-r--r--   0        0        0    21871 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/ach_transfers.py
--rw-r--r--   0        0        0     5051 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/card_disputes.py
--rw-r--r--   0        0        0     3967 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/card_refunds.py
--rw-r--r--   0        0        0    11463 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/cards.py
--rw-r--r--   0        0        0    10125 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/check_deposits.py
--rw-r--r--   0        0        0    11013 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/check_transfers.py
--rw-r--r--   0        0        0     4085 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/digital_wallet_token_requests.py
--rw-r--r--   0        0        0     3639 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/documents.py
--rw-r--r--   0        0        0    13466 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0     4411 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/interest_payments.py
--rw-r--r--   0        0        0     3919 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/programs.py
--rw-r--r--   0        0        0    11257 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4588 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/simulations.py
--rw-r--r--   0        0        0    12351 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/wire_transfers.py
--rw-r--r--   0        0        0     7800 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/transactions.py
--rw-r--r--   0        0        0    13338 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/wire_drawdown_requests.py
--rw-r--r--   0        0        0    27583 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/wire_transfers.py
--rw-r--r--   0        0        0     8739 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/types/__init__.py
--rw-r--r--   0        0        0     1666 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/types/account.py
--rw-r--r--   0        0        0      747 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_create_params.py
--rw-r--r--   0        0        0     1693 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_list_params.py
--rw-r--r--   0        0        0     1026 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number.py
--rw-r--r--   0        0        0      408 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number_create_params.py
--rw-r--r--   0        0        0     1598 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number_list_params.py
--rw-r--r--   0        0        0      435 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number_update_params.py
--rw-r--r--   0        0        0     1347 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_statement.py
--rw-r--r--   0        0        0     1534 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_statement_list_params.py
--rw-r--r--   0        0        0     2648 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_transfer.py
--rw-r--r--   0        0        0      814 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_transfer_create_params.py
--rw-r--r--   0        0        0     1494 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_transfer_list_params.py
--rw-r--r--   0        0        0      271 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_update_params.py
--rw-r--r--   0        0        0     2152 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_prenotification.py
--rw-r--r--   0        0        0     1847 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_prenotification_create_params.py
--rw-r--r--   0        0        0     1391 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_prenotification_list_params.py
--rw-r--r--   0        0        0     8882 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_transfer.py
--rw-r--r--   0        0        0     3388 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_transfer_create_params.py
--rw-r--r--   0        0        0     1592 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_transfer_list_params.py
--rw-r--r--   0        0        0      585 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/balance_lookup_lookup_params.py
--rw-r--r--   0        0        0      780 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/balance_lookup_lookup_response.py
--rw-r--r--   0        0        0      823 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_account.py
--rw-r--r--   0        0        0      626 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_account_create_params.py
--rw-r--r--   0        0        0      428 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_account_list_params.py
--rw-r--r--   0        0        0      698 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry.py
--rw-r--r--   0        0        0      424 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry_list_params.py
--rw-r--r--   0        0        0      895 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry_set.py
--rw-r--r--   0        0        0     1133 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry_set_create_params.py
--rw-r--r--   0        0        0     2342 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card.py
--rw-r--r--   0        0        0     1767 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_create_params.py
--rw-r--r--   0        0        0      907 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_details.py
--rw-r--r--   0        0        0     2011 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_dispute.py
--rw-r--r--   0        0        0      483 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_dispute_create_params.py
--rw-r--r--   0        0        0     1661 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_dispute_list_params.py
--rw-r--r--   0        0        0     1451 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_list_params.py
--rw-r--r--   0        0        0     2186 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_profile.py
--rw-r--r--   0        0        0     1820 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_profile_create_params.py
--rw-r--r--   0        0        0      716 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_profile_list_params.py
--rw-r--r--   0        0        0     1611 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_update_params.py
--rw-r--r--   0        0        0     4894 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_deposit.py
--rw-r--r--   0        0        0      748 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_deposit_create_params.py
--rw-r--r--   0        0        0     1477 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_deposit_list_params.py
--rw-r--r--   0        0        0     6750 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_transfer.py
--rw-r--r--   0        0        0     1939 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_transfer_create_params.py
--rw-r--r--   0        0        0     1488 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_transfer_list_params.py
--rw-r--r--   0        0        0    13068 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/declined_transaction.py
--rw-r--r--   0        0        0     1598 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/declined_transaction_list_params.py
--rw-r--r--   0        0        0      950 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/digital_wallet_token.py
--rw-r--r--   0        0        0     1489 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/digital_wallet_token_list_params.py
--rw-r--r--   0        0        0      883 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/document.py
--rw-r--r--   0        0        0     1780 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/document_list_params.py
--rw-r--r--   0        0        0      418 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/__init__.py
--rw-r--r--   0        0        0      634 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/supplemental_document.py
--rw-r--r--   0        0        0      343 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/supplemental_document_create_params.py
--rw-r--r--   0        0        0      547 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/supplemental_document_list_params.py
--rw-r--r--   0        0        0    11893 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entity.py
--rw-r--r--   0        0        0    25685 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entity_create_params.py
--rw-r--r--   0        0        0     1367 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entity_list_params.py
--rw-r--r--   0        0        0     2724 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event.py
--rw-r--r--   0        0        0     4044 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_list_params.py
--rw-r--r--   0        0        0     3124 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription.py
--rw-r--r--   0        0        0     2526 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription_create_params.py
--rw-r--r--   0        0        0      426 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription_list_params.py
--rw-r--r--   0        0        0      360 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription_update_params.py
--rw-r--r--   0        0        0     1147 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/export.py
--rw-r--r--   0        0        0     2946 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/export_create_params.py
--rw-r--r--   0        0        0      404 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/export_list_params.py
--rw-r--r--   0        0        0     1205 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account.py
--rw-r--r--   0        0        0      706 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account_create_params.py
--rw-r--r--   0        0        0      701 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account_list_params.py
--rw-r--r--   0        0        0      420 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account_update_params.py
--rw-r--r--   0        0        0     1612 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/file.py
--rw-r--r--   0        0        0     1115 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/file_create_params.py
--rw-r--r--   0        0        0     2202 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/file_list_params.py
--rw-r--r--   0        0        0      738 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/group.py
--rw-r--r--   0        0        0     1693 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_ach_transfer_return.py
--rw-r--r--   0        0        0     1109 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_ach_transfer_return_create_params.py
--rw-r--r--   0        0        0      440 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_ach_transfer_return_list_params.py
--rw-r--r--   0        0        0     2916 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_wire_drawdown_request.py
--rw-r--r--   0        0        0      444 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     1041 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit.py
--rw-r--r--   0        0        0      696 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit_create_params.py
--rw-r--r--   0        0        0      527 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit_list_params.py
--rw-r--r--   0        0        0      332 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit_update_params.py
--rw-r--r--   0        0        0      779 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/oauth_connection.py
--rw-r--r--   0        0        0      422 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/oauth_connection_list_params.py
--rw-r--r--   0        0        0    12078 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/pending_transaction.py
--rw-r--r--   0        0        0     1956 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/pending_transaction_list_params.py
--rw-r--r--   0        0        0      735 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/program.py
--rw-r--r--   0        0        0      406 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/program_list_params.py
--rw-r--r--   0        0        0     6113 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_decision.py
--rw-r--r--   0        0        0     2451 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_decision_action_params.py
--rw-r--r--   0        0        0     5096 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_payments_transfer.py
--rw-r--r--   0        0        0     1283 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_payments_transfer_create_params.py
--rw-r--r--   0        0        0     1664 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_payments_transfer_list_params.py
--rw-r--r--   0        0        0      895 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/routing_number.py
--rw-r--r--   0        0        0      522 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/routing_number_list_params.py
--rw-r--r--   0        0        0      155 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared/__init__.py
--rw-r--r--   0        0        0      489 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared/point_of_service_entry_mode.py
--rw-r--r--   0        0        0      155 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared_params/__init__.py
--rw-r--r--   0        0        0      525 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared_params/point_of_service_entry_mode.py
--rw-r--r--   0        0        0     2608 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/__init__.py
--rw-r--r--   0        0        0      338 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/account_statement_create_params.py
--rw-r--r--   0        0        0     1027 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     3303 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/ach_transfer_return_params.py
--rw-r--r--   0        0        0    51481 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/ach_transfer_simulation.py
--rw-r--r--   0        0        0    26885 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_authorization_simulation.py
--rw-r--r--   0        0        0      823 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_authorize_params.py
--rw-r--r--   0        0        0      443 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_dispute_action_params.py
--rw-r--r--   0        0        0      400 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_refund_create_params.py
--rw-r--r--   0        0        0      610 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_settlement_params.py
--rw-r--r--   0        0        0      425 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/check_transfer_return_params.py
--rw-r--r--   0        0        0      346 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/digital_wallet_token_request_create_params.py
--rw-r--r--   0        0        0      953 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py
--rw-r--r--   0        0        0      325 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/document_create_params.py
--rw-r--r--   0        0        0    51652 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
--rw-r--r--   0        0        0     2648 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      435 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/interest_payment_create_params.py
--rw-r--r--   0        0        0    37747 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/interest_payment_simulation_result.py
--rw-r--r--   0        0        0      299 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/program_create_params.py
--rw-r--r--   0        0        0     1362 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
--rw-r--r--   0        0        0     1020 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     2591 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py
--rw-r--r--   0        0        0    37791 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/wire_transfer_simulation.py
--rw-r--r--   0        0        0    36238 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/transaction.py
--rw-r--r--   0        0        0     3293 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/transaction_list_params.py
--rw-r--r--   0        0        0     2239 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_drawdown_request.py
--rw-r--r--   0        0        0     1148 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      430 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     5343 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_transfer.py
--rw-r--r--   0        0        0     1367 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_transfer_create_params.py
--rw-r--r--   0        0        0     1588 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_transfer_list_params.py
--rw-r--r--   0        0        0     9328 1970-01-01 00:00:00.000000 increase-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-07-07 14:37:14.963685 increase-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8418 2023-07-07 14:37:14.963685 increase-0.9.0/README.md
+-rw-r--r--   0        0        0     1881 2023-07-07 14:37:14.963685 increase-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2587 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/__init__.py
+-rw-r--r--   0        0        0    46808 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_base_exceptions.py
+-rw-r--r--   0        0        0    26762 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_client.py
+-rw-r--r--   0        0        0    10875 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_models.py
+-rw-r--r--   0        0        0     4846 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_qs.py
+-rw-r--r--   0        0        0      890 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_resource.py
+-rw-r--r--   0        0        0     5884 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_streaming.py
+-rw-r--r--   0        0        0     4229 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_types.py
+-rw-r--r--   0        0        0     1277 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_utils/_utils.py
+-rw-r--r--   0        0        0      127 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/_version.py
+-rw-r--r--   0        0        0     1109 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/pagination.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/py.typed
+-rw-r--r--   0        0        0     4478 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/__init__.py
+-rw-r--r--   0        0        0    15881 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/account_numbers.py
+-rw-r--r--   0        0        0     7400 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/account_statements.py
+-rw-r--r--   0        0        0    18102 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/account_transfers.py
+-rw-r--r--   0        0        0    18760 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/accounts.py
+-rw-r--r--   0        0        0    16386 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/ach_prenotifications.py
+-rw-r--r--   0        0        0    26745 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/ach_transfers.py
+-rw-r--r--   0        0        0     4285 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/balance_lookups.py
+-rw-r--r--   0        0        0     8923 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/bookkeeping_accounts.py
+-rw-r--r--   0        0        0     4122 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/bookkeeping_entries.py
+-rw-r--r--   0        0        0     4842 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/bookkeeping_entry_sets.py
+-rw-r--r--   0        0        0    10707 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/card_disputes.py
+-rw-r--r--   0        0        0    10597 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/card_profiles.py
+-rw-r--r--   0        0        0    19468 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/cards.py
+-rw-r--r--   0        0        0    11757 2023-07-07 14:37:14.963685 increase-0.9.0/src/increase/resources/check_deposits.py
+-rw-r--r--   0        0        0    24661 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/check_transfers.py
+-rw-r--r--   0        0        0     7771 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/declined_transactions.py
+-rw-r--r--   0        0        0     7353 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/digital_wallet_tokens.py
+-rw-r--r--   0        0        0     7177 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/documents.py
+-rw-r--r--   0        0        0      282 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/entities/__init__.py
+-rw-r--r--   0        0        0    14966 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/entities/entities.py
+-rw-r--r--   0        0        0     8071 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/entities/supplemental_documents.py
+-rw-r--r--   0        0        0    30003 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/event_subscriptions.py
+-rw-r--r--   0        0        0     7154 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/events.py
+-rw-r--r--   0        0        0    10962 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/exports.py
+-rw-r--r--   0        0        0    15967 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/external_accounts.py
+-rw-r--r--   0        0        0    15719 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/files.py
+-rw-r--r--   0        0        0     2040 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/groups.py
+-rw-r--r--   0        0        0    14659 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/inbound_ach_transfer_returns.py
+-rw-r--r--   0        0        0     7075 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0    15965 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/limits.py
+-rw-r--r--   0        0        0     6593 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/oauth_connections.py
+-rw-r--r--   0        0        0     8344 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/pending_transactions.py
+-rw-r--r--   0        0        0     6300 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/programs.py
+-rw-r--r--   0        0        0     8536 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/real_time_decisions.py
+-rw-r--r--   0        0        0    14968 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4951 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/routing_numbers.py
+-rw-r--r--   0        0        0     2093 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/__init__.py
+-rw-r--r--   0        0        0     4026 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/account_statements.py
+-rw-r--r--   0        0        0     4024 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/account_transfers.py
+-rw-r--r--   0        0        0    43813 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/ach_transfers.py
+-rw-r--r--   0        0        0     5413 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/card_disputes.py
+-rw-r--r--   0        0        0     4068 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/card_profiles.py
+-rw-r--r--   0        0        0     3967 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/card_refunds.py
+-rw-r--r--   0        0        0    11463 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/cards.py
+-rw-r--r--   0        0        0    10125 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/check_deposits.py
+-rw-r--r--   0        0        0     7058 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/check_transfers.py
+-rw-r--r--   0        0        0     4085 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/digital_wallet_token_requests.py
+-rw-r--r--   0        0        0     3639 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/documents.py
+-rw-r--r--   0        0        0    13466 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0     4411 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/interest_payments.py
+-rw-r--r--   0        0        0     3919 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/programs.py
+-rw-r--r--   0        0        0    11257 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4821 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/simulations.py
+-rw-r--r--   0        0        0    12351 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/simulations/wire_transfers.py
+-rw-r--r--   0        0        0     7800 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/transactions.py
+-rw-r--r--   0        0        0    13338 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/wire_drawdown_requests.py
+-rw-r--r--   0        0        0    27583 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/resources/wire_transfers.py
+-rw-r--r--   0        0        0     8861 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/__init__.py
+-rw-r--r--   0        0        0     1984 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account.py
+-rw-r--r--   0        0        0      747 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_create_params.py
+-rw-r--r--   0        0        0     1820 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_list_params.py
+-rw-r--r--   0        0        0     1205 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_number.py
+-rw-r--r--   0        0        0      408 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_number_create_params.py
+-rw-r--r--   0        0        0     1777 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_number_list_params.py
+-rw-r--r--   0        0        0      614 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_number_update_params.py
+-rw-r--r--   0        0        0     1347 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_statement.py
+-rw-r--r--   0        0        0     1534 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_statement_list_params.py
+-rw-r--r--   0        0        0     3009 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_transfer.py
+-rw-r--r--   0        0        0      814 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_transfer_create_params.py
+-rw-r--r--   0        0        0     1494 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_transfer_list_params.py
+-rw-r--r--   0        0        0      271 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/account_update_params.py
+-rw-r--r--   0        0        0     2547 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/ach_prenotification.py
+-rw-r--r--   0        0        0     2200 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/ach_prenotification_create_params.py
+-rw-r--r--   0        0        0     1391 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/ach_prenotification_list_params.py
+-rw-r--r--   0        0        0    19432 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/ach_transfer.py
+-rw-r--r--   0        0        0     3685 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/ach_transfer_create_params.py
+-rw-r--r--   0        0        0     1592 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/ach_transfer_list_params.py
+-rw-r--r--   0        0        0      585 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/balance_lookup_lookup_params.py
+-rw-r--r--   0        0        0      780 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/balance_lookup_lookup_response.py
+-rw-r--r--   0        0        0      944 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/bookkeeping_account.py
+-rw-r--r--   0        0        0      747 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/bookkeeping_account_create_params.py
+-rw-r--r--   0        0        0      428 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/bookkeeping_account_list_params.py
+-rw-r--r--   0        0        0      698 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/bookkeeping_entry.py
+-rw-r--r--   0        0        0      424 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/bookkeeping_entry_list_params.py
+-rw-r--r--   0        0        0      895 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/bookkeeping_entry_set.py
+-rw-r--r--   0        0        0     1133 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/bookkeeping_entry_set_create_params.py
+-rw-r--r--   0        0        0     2491 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card.py
+-rw-r--r--   0        0        0     1767 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_create_params.py
+-rw-r--r--   0        0        0      907 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_details.py
+-rw-r--r--   0        0        0     2231 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_dispute.py
+-rw-r--r--   0        0        0      483 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_dispute_create_params.py
+-rw-r--r--   0        0        0     1661 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_dispute_list_params.py
+-rw-r--r--   0        0        0     1451 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_list_params.py
+-rw-r--r--   0        0        0     2502 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_profile.py
+-rw-r--r--   0        0        0     1820 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_profile_create_params.py
+-rw-r--r--   0        0        0      716 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_profile_list_params.py
+-rw-r--r--   0        0        0     1760 2023-07-07 14:37:14.967685 increase-0.9.0/src/increase/types/card_update_params.py
+-rw-r--r--   0        0        0     7284 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/check_deposit.py
+-rw-r--r--   0        0        0      748 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/check_deposit_create_params.py
+-rw-r--r--   0        0        0     1477 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/check_deposit_list_params.py
+-rw-r--r--   0        0        0     6987 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/check_transfer.py
+-rw-r--r--   0        0        0     2091 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/check_transfer_create_params.py
+-rw-r--r--   0        0        0     1488 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/check_transfer_list_params.py
+-rw-r--r--   0        0        0      493 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/check_transfer_stop_payment_params.py
+-rw-r--r--   0        0        0    20551 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/declined_transaction.py
+-rw-r--r--   0        0        0     1598 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/declined_transaction_list_params.py
+-rw-r--r--   0        0        0     1363 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/digital_wallet_token.py
+-rw-r--r--   0        0        0     1489 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/digital_wallet_token_list_params.py
+-rw-r--r--   0        0        0     1224 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/document.py
+-rw-r--r--   0        0        0     1780 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/document_list_params.py
+-rw-r--r--   0        0        0      418 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/entities/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/entities/supplemental_document.py
+-rw-r--r--   0        0        0      343 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/entities/supplemental_document_create_params.py
+-rw-r--r--   0        0        0      547 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/entities/supplemental_document_list_params.py
+-rw-r--r--   0        0        0    14241 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/entity.py
+-rw-r--r--   0        0        0    28028 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/entity_create_params.py
+-rw-r--r--   0        0        0     1367 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/entity_list_params.py
+-rw-r--r--   0        0        0     7263 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/event.py
+-rw-r--r--   0        0        0     4044 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/event_list_params.py
+-rw-r--r--   0        0        0     8084 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/event_subscription.py
+-rw-r--r--   0        0        0     7065 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/event_subscription_create_params.py
+-rw-r--r--   0        0        0      426 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/event_subscription_list_params.py
+-rw-r--r--   0        0        0      648 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/event_subscription_update_params.py
+-rw-r--r--   0        0        0     1446 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/export.py
+-rw-r--r--   0        0        0     3128 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/export_create_params.py
+-rw-r--r--   0        0        0      404 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/export_list_params.py
+-rw-r--r--   0        0        0     1681 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/external_account.py
+-rw-r--r--   0        0        0      833 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/external_account_create_params.py
+-rw-r--r--   0        0        0      701 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/external_account_list_params.py
+-rw-r--r--   0        0        0      569 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/external_account_update_params.py
+-rw-r--r--   0        0        0     3124 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/file.py
+-rw-r--r--   0        0        0     2315 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/file_create_params.py
+-rw-r--r--   0        0        0     2202 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/file_list_params.py
+-rw-r--r--   0        0        0      946 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/group.py
+-rw-r--r--   0        0        0     3018 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/inbound_ach_transfer_return.py
+-rw-r--r--   0        0        0     2251 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/inbound_ach_transfer_return_create_params.py
+-rw-r--r--   0        0        0      440 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/inbound_ach_transfer_return_list_params.py
+-rw-r--r--   0        0        0     2916 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/inbound_wire_drawdown_request.py
+-rw-r--r--   0        0        0      444 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/inbound_wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     1988 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/limit.py
+-rw-r--r--   0        0        0     1355 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/limit_create_params.py
+-rw-r--r--   0        0        0      527 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/limit_list_params.py
+-rw-r--r--   0        0        0      425 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/limit_update_params.py
+-rw-r--r--   0        0        0      902 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/oauth_connection.py
+-rw-r--r--   0        0        0      422 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/oauth_connection_list_params.py
+-rw-r--r--   0        0        0    17395 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/pending_transaction.py
+-rw-r--r--   0        0        0     1956 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/pending_transaction_list_params.py
+-rw-r--r--   0        0        0      735 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/program.py
+-rw-r--r--   0        0        0      406 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/program_list_params.py
+-rw-r--r--   0        0        0     9425 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/real_time_decision.py
+-rw-r--r--   0        0        0     2758 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/real_time_decision_action_params.py
+-rw-r--r--   0        0        0     9089 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/real_time_payments_transfer.py
+-rw-r--r--   0        0        0     1283 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/real_time_payments_transfer_create_params.py
+-rw-r--r--   0        0        0     1664 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/real_time_payments_transfer_list_params.py
+-rw-r--r--   0        0        0     1360 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/routing_number.py
+-rw-r--r--   0        0        0      522 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/routing_number_list_params.py
+-rw-r--r--   0        0        0      155 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/shared/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/shared/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0      155 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/shared_params/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0     2502 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/account_statement_create_params.py
+-rw-r--r--   0        0        0     1027 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0    12834 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/ach_transfer_return_params.py
+-rw-r--r--   0        0        0    76942 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/ach_transfer_simulation.py
+-rw-r--r--   0        0        0    39685 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/card_authorization_simulation.py
+-rw-r--r--   0        0        0      823 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/card_authorize_params.py
+-rw-r--r--   0        0        0      599 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/card_dispute_action_params.py
+-rw-r--r--   0        0        0      400 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/card_refund_create_params.py
+-rw-r--r--   0        0        0      610 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/card_settlement_params.py
+-rw-r--r--   0        0        0      346 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/digital_wallet_token_request_create_params.py
+-rw-r--r--   0        0        0     1288 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py
+-rw-r--r--   0        0        0      325 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/document_create_params.py
+-rw-r--r--   0        0        0    77113 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
+-rw-r--r--   0        0        0     2648 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      435 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/interest_payment_create_params.py
+-rw-r--r--   0        0        0    55725 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/interest_payment_simulation_result.py
+-rw-r--r--   0        0        0      299 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/program_create_params.py
+-rw-r--r--   0        0        0     4590 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
+-rw-r--r--   0        0        0     1020 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     2591 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0    55769 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/simulations/wire_transfer_simulation.py
+-rw-r--r--   0        0        0    54249 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/transaction.py
+-rw-r--r--   0        0        0     3252 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/transaction_list_params.py
+-rw-r--r--   0        0        0     2605 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/wire_drawdown_request.py
+-rw-r--r--   0        0        0     1148 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      430 2023-07-07 14:37:14.971685 increase-0.9.0/src/increase/types/wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     5954 2023-07-07 14:37:14.975685 increase-0.9.0/src/increase/types/wire_transfer.py
+-rw-r--r--   0        0        0     1367 2023-07-07 14:37:14.975685 increase-0.9.0/src/increase/types/wire_transfer_create_params.py
+-rw-r--r--   0        0        0     1588 2023-07-07 14:37:14.975685 increase-0.9.0/src/increase/types/wire_transfer_list_params.py
+-rw-r--r--   0        0        0     9328 1970-01-01 00:00:00.000000 increase-0.9.0/PKG-INFO
```

### Comparing `increase-0.8.1/LICENSE` & `increase-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/README.md` & `increase-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/pyproject.toml` & `increase-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "increase"
-version = "0.8.1"
+version = "0.9.0"
 description = "Client library for the increase API"
 readme = "README.md"
 authors = ["Increase <dev-feedback@increase.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/increase/increase-python"
 packages = [
   { include = "increase", from = "src" }
```

### Comparing `increase-0.8.1/src/increase/__init__.py` & `increase-0.9.0/src/increase/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_base_client.py` & `increase-0.9.0/src/increase/_base_client.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_base_exceptions.py` & `increase-0.9.0/src/increase/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_client.py` & `increase-0.9.0/src/increase/_client.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_exceptions.py` & `increase-0.9.0/src/increase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_models.py` & `increase-0.9.0/src/increase/_models.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_qs.py` & `increase-0.9.0/src/increase/_qs.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_resource.py` & `increase-0.9.0/src/increase/_resource.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_streaming.py` & `increase-0.9.0/src/increase/_streaming.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_types.py` & `increase-0.9.0/src/increase/_types.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_utils/__init__.py` & `increase-0.9.0/src/increase/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_utils/_transform.py` & `increase-0.9.0/src/increase/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/_utils/_utils.py` & `increase-0.9.0/src/increase/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/pagination.py` & `increase-0.9.0/src/increase/pagination.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/__init__.py` & `increase-0.9.0/src/increase/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/account_numbers.py` & `increase-0.9.0/src/increase/resources/account_numbers.py`

 * *Files 14% similar despite different names*

```diff
@@ -123,14 +123,18 @@
         Args:
           account_number_id: The identifier of the Account Number.
 
           name: The name you choose for the Account Number.
 
           status: This indicates if transfers can be made to the Account Number.
 
+              - `active` - The account number is active.
+              - `disabled` - The account number is temporarily disabled.
+              - `canceled` - The account number is permanently disabled.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -180,14 +184,18 @@
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           status: The status to retrieve Account Numbers for.
 
+              - `active` - The account number is active.
+              - `disabled` - The account number is temporarily disabled.
+              - `canceled` - The account number is permanently disabled.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -319,14 +327,18 @@
         Args:
           account_number_id: The identifier of the Account Number.
 
           name: The name you choose for the Account Number.
 
           status: This indicates if transfers can be made to the Account Number.
 
+              - `active` - The account number is active.
+              - `disabled` - The account number is temporarily disabled.
+              - `canceled` - The account number is permanently disabled.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -376,14 +388,18 @@
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           status: The status to retrieve Account Numbers for.
 
+              - `active` - The account number is active.
+              - `disabled` - The account number is temporarily disabled.
+              - `canceled` - The account number is permanently disabled.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
```

### Comparing `increase-0.8.1/src/increase/resources/account_statements.py` & `increase-0.9.0/src/increase/resources/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/account_transfers.py` & `increase-0.9.0/src/increase/resources/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/accounts.py` & `increase-0.9.0/src/increase/resources/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,17 @@
           informational_entity_id: Filter Accounts for those belonging to the specified Entity as informational.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           status: Filter Accounts for those with the specified status.
 
+              - `open` - Open Accounts that are ready to use.
+              - `closed` - Closed Accounts on which no new activity can occur.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -425,14 +428,17 @@
           informational_entity_id: Filter Accounts for those belonging to the specified Entity as informational.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           status: Filter Accounts for those with the specified status.
 
+              - `open` - Open Accounts that are ready to use.
+              - `closed` - Closed Accounts on which no new activity can occur.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
```

### Comparing `increase-0.8.1/src/increase/resources/ach_prenotifications.py` & `increase-0.9.0/src/increase/resources/ach_prenotifications.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,24 +64,31 @@
 
           company_entry_description: The description of the transfer you wish to be shown to the recipient.
 
           company_name: The name by which the recipient knows you.
 
           credit_debit_indicator: Whether the Prenotification is for a future debit or credit.
 
+              - `credit` - The Prenotification is for an anticipated credit.
+              - `debit` - The Prenotification is for an anticipated debit.
+
           effective_date: The transfer effective date in
               [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
 
           individual_id: Your identifer for the transfer recipient.
 
           individual_name: The name of the transfer recipient. This value is information and not verified
               by the recipient's bank.
 
           standard_entry_class_code: The Standard Entry Class (SEC) code to use for the ACH Prenotification.
 
+              - `corporate_credit_or_debit` - Corporate Credit and Debit (CCD).
+              - `prearranged_payments_and_deposit` - Prearranged Payments and Deposits (PPD).
+              - `internet_initiated` - Internet Initiated (WEB).
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -245,24 +252,31 @@
 
           company_entry_description: The description of the transfer you wish to be shown to the recipient.
 
           company_name: The name by which the recipient knows you.
 
           credit_debit_indicator: Whether the Prenotification is for a future debit or credit.
 
+              - `credit` - The Prenotification is for an anticipated credit.
+              - `debit` - The Prenotification is for an anticipated debit.
+
           effective_date: The transfer effective date in
               [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
 
           individual_id: Your identifer for the transfer recipient.
 
           individual_name: The name of the transfer recipient. This value is information and not verified
               by the recipient's bank.
 
           standard_entry_class_code: The Standard Entry Class (SEC) code to use for the ACH Prenotification.
 
+              - `corporate_credit_or_debit` - Corporate Credit and Debit (CCD).
+              - `prearranged_payments_and_deposit` - Prearranged Payments and Deposits (PPD).
+              - `internet_initiated` - Internet Initiated (WEB).
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
```

### Comparing `increase-0.8.1/src/increase/resources/ach_transfers.py` & `increase-0.9.0/src/increase/resources/ach_transfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,26 +86,33 @@
               [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
 
           external_account_id: The ID of an External Account to initiate a transfer to. If this parameter is
               provided, `account_number`, `routing_number`, and `funding` must be absent.
 
           funding: The type of the account to which the transfer will be sent.
 
+              - `checking` - A checking account.
+              - `savings` - A savings account.
+
           individual_id: Your identifer for the transfer recipient.
 
           individual_name: The name of the transfer recipient. This value is informational and not verified
               by the recipient's bank.
 
           require_approval: Whether the transfer requires explicit approval via the dashboard or API.
 
           routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
               destination account.
 
           standard_entry_class_code: The Standard Entry Class (SEC) code to use for the transfer.
 
+              - `corporate_credit_or_debit` - Corporate Credit and Debit (CCD).
+              - `prearranged_payments_and_deposit` - Prearranged Payments and Deposits (PPD).
+              - `internet_initiated` - Internet Initiated (WEB).
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -388,26 +395,33 @@
               [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
 
           external_account_id: The ID of an External Account to initiate a transfer to. If this parameter is
               provided, `account_number`, `routing_number`, and `funding` must be absent.
 
           funding: The type of the account to which the transfer will be sent.
 
+              - `checking` - A checking account.
+              - `savings` - A savings account.
+
           individual_id: Your identifer for the transfer recipient.
 
           individual_name: The name of the transfer recipient. This value is informational and not verified
               by the recipient's bank.
 
           require_approval: Whether the transfer requires explicit approval via the dashboard or API.
 
           routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
               destination account.
 
           standard_entry_class_code: The Standard Entry Class (SEC) code to use for the transfer.
 
+              - `corporate_credit_or_debit` - Corporate Credit and Debit (CCD).
+              - `prearranged_payments_and_deposit` - Prearranged Payments and Deposits (PPD).
+              - `internet_initiated` - Internet Initiated (WEB).
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
```

### Comparing `increase-0.8.1/src/increase/resources/balance_lookups.py` & `increase-0.9.0/src/increase/resources/balance_lookups.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/bookkeeping_accounts.py` & `increase-0.9.0/src/increase/resources/bookkeeping_accounts.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,17 @@
         Args:
           name: The name you choose for the account.
 
           account_id: The entity, if `compliance_category` is `commingled_cash`.
 
           compliance_category: The account compliance category.
 
+              - `commingled_cash` - A cash in an commingled Increase Account.
+              - `customer_balance` - A customer balance.
+
           entity_id: The entity, if `compliance_category` is `customer_balance`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -148,14 +151,17 @@
         Args:
           name: The name you choose for the account.
 
           account_id: The entity, if `compliance_category` is `commingled_cash`.
 
           compliance_category: The account compliance category.
 
+              - `commingled_cash` - A cash in an commingled Increase Account.
+              - `customer_balance` - A customer balance.
+
           entity_id: The entity, if `compliance_category` is `customer_balance`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
```

### Comparing `increase-0.8.1/src/increase/resources/bookkeeping_entries.py` & `increase-0.9.0/src/increase/resources/bookkeeping_entries.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/bookkeeping_entry_sets.py` & `increase-0.9.0/src/increase/resources/bookkeeping_entry_sets.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/card_disputes.py` & `increase-0.9.0/src/increase/resources/card_disputes.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/card_profiles.py` & `increase-0.9.0/src/increase/resources/card_profiles.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/cards.py` & `increase-0.9.0/src/increase/resources/cards.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,14 +144,18 @@
 
           digital_wallet: The contact information used in the two-factor steps for digital wallet card
               creation. At least one field must be present to complete the digital wallet
               steps.
 
           status: The status to update the Card with.
 
+              - `active` - The card is active.
+              - `disabled` - The card is temporarily disabled.
+              - `canceled` - The card is permanently canceled.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -391,14 +395,18 @@
 
           digital_wallet: The contact information used in the two-factor steps for digital wallet card
               creation. At least one field must be present to complete the digital wallet
               steps.
 
           status: The status to update the Card with.
 
+              - `active` - The card is active.
+              - `disabled` - The card is temporarily disabled.
+              - `canceled` - The card is permanently canceled.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
```

### Comparing `increase-0.8.1/src/increase/resources/check_deposits.py` & `increase-0.9.0/src/increase/resources/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/check_transfers.py` & `increase-0.9.0/src/increase/resources/check_transfers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
+from typing_extensions import Literal
+
 from ..types import (
     CheckTransfer,
     check_transfer_list_params,
     check_transfer_create_params,
+    check_transfer_stop_payment_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
@@ -28,14 +31,15 @@
         amount: int,
         message: str,
         recipient_name: str,
         address_line2: str | NotGiven = NOT_GIVEN,
         note: str | NotGiven = NOT_GIVEN,
         require_approval: bool | NotGiven = NOT_GIVEN,
         return_address: check_transfer_create_params.ReturnAddress | NotGiven = NOT_GIVEN,
+        source_account_number_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -65,14 +69,17 @@
           note: The descriptor that will be printed on the letter included with the check.
 
           require_approval: Whether the transfer requires explicit approval via the dashboard or API.
 
           return_address: The return address to be printed on the check. If omitted this will default to
               the address of the Entity of the Account used to make the Check Transfer.
 
+          source_account_number_id: The identifier of the Account Number from which to send the transfer and print
+              on the check.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -91,14 +98,15 @@
                     "amount": amount,
                     "message": message,
                     "recipient_name": recipient_name,
                     "address_line2": address_line2,
                     "note": note,
                     "require_approval": require_approval,
                     "return_address": return_address,
+                    "source_account_number_id": source_account_number_id,
                 },
                 check_transfer_create_params.CheckTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -275,40 +283,47 @@
             cast_to=CheckTransfer,
         )
 
     def stop_payment(
         self,
         check_transfer_id: str,
         *,
+        reason: Literal["mail_delivery_failed", "unknown"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Request a stop payment on a Check Transfer
 
         Args:
           check_transfer_id: The identifier of the Check Transfer.
 
+          reason: The reason why this transfer should be stopped.
+
+              - `mail_delivery_failed` - The check could not be delivered.
+              - `unknown` - The check was stopped for another reason.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/check_transfers/{check_transfer_id}/stop_payment",
+            body=maybe_transform({"reason": reason}, check_transfer_stop_payment_params.CheckTransferStopPaymentParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
@@ -328,14 +343,15 @@
         amount: int,
         message: str,
         recipient_name: str,
         address_line2: str | NotGiven = NOT_GIVEN,
         note: str | NotGiven = NOT_GIVEN,
         require_approval: bool | NotGiven = NOT_GIVEN,
         return_address: check_transfer_create_params.ReturnAddress | NotGiven = NOT_GIVEN,
+        source_account_number_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -365,14 +381,17 @@
           note: The descriptor that will be printed on the letter included with the check.
 
           require_approval: Whether the transfer requires explicit approval via the dashboard or API.
 
           return_address: The return address to be printed on the check. If omitted this will default to
               the address of the Entity of the Account used to make the Check Transfer.
 
+          source_account_number_id: The identifier of the Account Number from which to send the transfer and print
+              on the check.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -391,14 +410,15 @@
                     "amount": amount,
                     "message": message,
                     "recipient_name": recipient_name,
                     "address_line2": address_line2,
                     "note": note,
                     "require_approval": require_approval,
                     "return_address": return_address,
+                    "source_account_number_id": source_account_number_id,
                 },
                 check_transfer_create_params.CheckTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -575,40 +595,47 @@
             cast_to=CheckTransfer,
         )
 
     async def stop_payment(
         self,
         check_transfer_id: str,
         *,
+        reason: Literal["mail_delivery_failed", "unknown"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Request a stop payment on a Check Transfer
 
         Args:
           check_transfer_id: The identifier of the Check Transfer.
 
+          reason: The reason why this transfer should be stopped.
+
+              - `mail_delivery_failed` - The check could not be delivered.
+              - `unknown` - The check was stopped for another reason.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/check_transfers/{check_transfer_id}/stop_payment",
+            body=maybe_transform({"reason": reason}, check_transfer_stop_payment_params.CheckTransferStopPaymentParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
```

### Comparing `increase-0.8.1/src/increase/resources/declined_transactions.py` & `increase-0.9.0/src/increase/resources/declined_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/digital_wallet_tokens.py` & `increase-0.9.0/src/increase/resources/digital_wallet_tokens.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/documents.py` & `increase-0.9.0/src/increase/resources/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/entities/entities.py` & `increase-0.9.0/src/increase/resources/entities/entities.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,16 +47,26 @@
     ) -> Entity:
         """
         Create an Entity
 
         Args:
           relationship: The relationship between your group and the entity.
 
+              - `affiliated` - The entity is controlled by your group.
+              - `informational` - The entity is for informational purposes only.
+              - `unaffiliated` - The entity is not controlled by your group, but can still
+                directly open accounts.
+
           structure: The type of Entity to create.
 
+              - `corporation` - A corporation.
+              - `natural_person` - An individual person.
+              - `joint` - Multiple individual people.
+              - `trust` - A trust.
+
           corporation: Details of the corporation entity to create. Required if `structure` is equal to
               `corporation`.
 
           description: The description you choose to give the entity.
 
           joint: Details of the joint entity to create. Required if `structure` is equal to
               `joint`.
@@ -218,16 +228,26 @@
     ) -> Entity:
         """
         Create an Entity
 
         Args:
           relationship: The relationship between your group and the entity.
 
+              - `affiliated` - The entity is controlled by your group.
+              - `informational` - The entity is for informational purposes only.
+              - `unaffiliated` - The entity is not controlled by your group, but can still
+                directly open accounts.
+
           structure: The type of Entity to create.
 
+              - `corporation` - A corporation.
+              - `natural_person` - An individual person.
+              - `joint` - Multiple individual people.
+              - `trust` - A trust.
+
           corporation: Details of the corporation entity to create. Required if `structure` is equal to
               `corporation`.
 
           description: The description you choose to give the entity.
 
           joint: Details of the joint entity to create. Required if `structure` is equal to
               `joint`.
```

### Comparing `increase-0.8.1/src/increase/resources/entities/supplemental_documents.py` & `increase-0.9.0/src/increase/resources/entities/supplemental_documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/events.py` & `increase-0.9.0/src/increase/resources/events.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/exports.py` & `increase-0.9.0/src/increase/resources/exports.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     ) -> Export:
         """
         Create an Export
 
         Args:
           category: The type of Export to create.
 
+              - `transaction_csv` - Export a CSV of all transactions for a given time range.
+              - `balance_csv` - Export a CSV of account balances for the dates in a given
+                range.
+
           balance_csv: Options for the created export. Required if `category` is equal to
               `balance_csv`.
 
           transaction_csv: Options for the created export. Required if `category` is equal to
               `transaction_csv`.
 
           extra_headers: Send extra headers
@@ -170,14 +174,18 @@
     ) -> Export:
         """
         Create an Export
 
         Args:
           category: The type of Export to create.
 
+              - `transaction_csv` - Export a CSV of all transactions for a given time range.
+              - `balance_csv` - Export a CSV of account balances for the dates in a given
+                range.
+
           balance_csv: Options for the created export. Required if `category` is equal to
               `balance_csv`.
 
           transaction_csv: Options for the created export. Required if `category` is equal to
               `transaction_csv`.
 
           extra_headers: Send extra headers
```

### Comparing `increase-0.8.1/src/increase/resources/external_accounts.py` & `increase-0.9.0/src/increase/resources/external_accounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,18 @@
           description: The name you choose for the Account.
 
           routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
               destination account.
 
           funding: The type of the destination account. Defaults to `checking`.
 
+              - `checking` - A checking account.
+              - `savings` - A savings account.
+              - `other` - A different type of account.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -132,14 +136,18 @@
         Args:
           external_account_id: The external account identifier.
 
           description: The description you choose to give the external account.
 
           status: The status of the External Account.
 
+              - `active` - The External Acccount is active.
+              - `archived` - The External Account is archived and won't appear in the
+                dashboard.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -241,14 +249,18 @@
           description: The name you choose for the Account.
 
           routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
               destination account.
 
           funding: The type of the destination account. Defaults to `checking`.
 
+              - `checking` - A checking account.
+              - `savings` - A savings account.
+              - `other` - A different type of account.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -329,14 +341,18 @@
         Args:
           external_account_id: The external account identifier.
 
           description: The description you choose to give the external account.
 
           status: The status of the External Account.
 
+              - `active` - The External Acccount is active.
+              - `archived` - The External Account is archived and won't appear in the
+                dashboard.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
```

### Comparing `increase-0.8.1/src/increase/resources/files.py` & `increase-0.9.0/src/increase/resources/files.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,14 +51,35 @@
         Args:
           file: The file contents. This should follow the specifications of
               [RFC 7578](https://datatracker.ietf.org/doc/html/rfc7578) which defines file
               transfers for the multipart/form-data protocol.
 
           purpose: What the File will be used for in Increase's systems.
 
+              - `check_image_front` - An image of the front of a check, used for check
+                deposits.
+              - `check_image_back` - An image of the back of a check, used for check deposits.
+              - `form_ss_4` - IRS Form SS-4.
+              - `identity_document` - An image of a government-issued ID.
+              - `other` - A file purpose not covered by any of the other cases.
+              - `trust_formation_document` - A legal document forming a trust.
+              - `digital_wallet_artwork` - A card image to be rendered inside digital wallet
+                apps. This must be a 1536x969 pixel PNG.
+              - `digital_wallet_app_icon` - An icon for you app to be rendered inside digital
+                wallet apps. This must be a 100x100 pixel PNG.
+              - `physical_card_artwork` - A card image to be printed on the front of a
+                physical card. This must be a 2100x1340 pixel PNG with no other color but
+                black.
+              - `physical_card_carrier` - An image representing the entirety of the carrier
+                used for a physical card. This must be a 2550x3300 pixel PNG with no other
+                color but black.
+              - `document_request` - A document requested by Increase.
+              - `entity_supplemental_document` - A supplemental document associated an an
+                Entity.
+
           description: The description you choose to give the File.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -217,14 +238,35 @@
         Args:
           file: The file contents. This should follow the specifications of
               [RFC 7578](https://datatracker.ietf.org/doc/html/rfc7578) which defines file
               transfers for the multipart/form-data protocol.
 
           purpose: What the File will be used for in Increase's systems.
 
+              - `check_image_front` - An image of the front of a check, used for check
+                deposits.
+              - `check_image_back` - An image of the back of a check, used for check deposits.
+              - `form_ss_4` - IRS Form SS-4.
+              - `identity_document` - An image of a government-issued ID.
+              - `other` - A file purpose not covered by any of the other cases.
+              - `trust_formation_document` - A legal document forming a trust.
+              - `digital_wallet_artwork` - A card image to be rendered inside digital wallet
+                apps. This must be a 1536x969 pixel PNG.
+              - `digital_wallet_app_icon` - An icon for you app to be rendered inside digital
+                wallet apps. This must be a 100x100 pixel PNG.
+              - `physical_card_artwork` - A card image to be printed on the front of a
+                physical card. This must be a 2100x1340 pixel PNG with no other color but
+                black.
+              - `physical_card_carrier` - An image representing the entirety of the carrier
+                used for a physical card. This must be a 2550x3300 pixel PNG with no other
+                color but black.
+              - `document_request` - A document requested by Increase.
+              - `entity_supplemental_document` - A supplemental document associated an an
+                Entity.
+
           description: The description you choose to give the File.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
```

### Comparing `increase-0.8.1/src/increase/resources/groups.py` & `increase-0.9.0/src/increase/resources/groups.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/inbound_ach_transfer_returns.py` & `increase-0.9.0/src/increase/resources/simulations/real_time_payments_transfers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,306 +1,264 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing_extensions import Literal
-
-from ..types import (
-    InboundACHTransferReturn,
-    inbound_ach_transfer_return_list_params,
-    inbound_ach_transfer_return_create_params,
+from ...types import RealTimePaymentsTransfer
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
+from ..._resource import SyncAPIResource, AsyncAPIResource
+from ..._base_client import make_request_options
+from ...types.simulations import (
+    InboundRealTimePaymentsTransferSimulationResult,
+    real_time_payments_transfer_complete_params,
+    real_time_payments_transfer_create_inbound_params,
 )
-from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from .._utils import maybe_transform
-from .._resource import SyncAPIResource, AsyncAPIResource
-from ..pagination import SyncPage, AsyncPage
-from .._base_client import AsyncPaginator, make_request_options
 
-__all__ = ["InboundACHTransferReturns", "AsyncInboundACHTransferReturns"]
+__all__ = ["RealTimePaymentsTransfers", "AsyncRealTimePaymentsTransfers"]
 
 
-class InboundACHTransferReturns(SyncAPIResource):
-    def create(
+class RealTimePaymentsTransfers(SyncAPIResource):
+    def complete(
         self,
+        real_time_payments_transfer_id: str,
         *,
-        reason: Literal[
-            "authorization_revoked_by_customer",
-            "payment_stopped",
-            "customer_advised_unauthorized_improper_ineligible_or_incomplete",
-            "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
-            "beneficiary_or_account_holder_deceased",
-            "credit_entry_refused_by_receiver",
-            "duplicate_entry",
-            "corporate_customer_advised_not_authorized",
-        ],
-        transaction_id: str,
+        rejection: real_time_payments_transfer_complete_params.Rejection | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> InboundACHTransferReturn:
+    ) -> RealTimePaymentsTransfer:
         """
-        Create an ACH Return
+        Simulates submission of a Real Time Payments transfer and handling the response
+        from the destination financial institution. This transfer must first have a
+        `status` of `pending_submission`.
 
         Args:
-          reason: The reason why this transfer will be returned. The most usual return codes are
-              `payment_stopped` for debits and `credit_entry_refused_by_receiver` for credits.
+          real_time_payments_transfer_id: The identifier of the Real Time Payments Transfer you wish to complete.
 
-          transaction_id: The transaction identifier of the Inbound ACH Transfer to return to the
-              originating financial institution.
+          rejection: If set, the simulation will reject the transfer.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            "/inbound_ach_transfer_returns",
+            f"/simulations/real_time_payments_transfers/{real_time_payments_transfer_id}/complete",
             body=maybe_transform(
-                {
-                    "reason": reason,
-                    "transaction_id": transaction_id,
-                },
-                inbound_ach_transfer_return_create_params.InboundACHTransferReturnCreateParams,
+                {"rejection": rejection},
+                real_time_payments_transfer_complete_params.RealTimePaymentsTransferCompleteParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=InboundACHTransferReturn,
+            cast_to=RealTimePaymentsTransfer,
         )
 
-    def retrieve(
+    def create_inbound(
         self,
-        inbound_ach_transfer_return_id: str,
         *,
+        account_number_id: str,
+        amount: int,
+        debtor_account_number: str | NotGiven = NOT_GIVEN,
+        debtor_name: str | NotGiven = NOT_GIVEN,
+        debtor_routing_number: str | NotGiven = NOT_GIVEN,
+        remittance_information: str | NotGiven = NOT_GIVEN,
+        request_for_payment_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> InboundACHTransferReturn:
-        """
-        Retrieve an Inbound ACH Transfer Return
+        idempotency_key: str | None = None,
+    ) -> InboundRealTimePaymentsTransferSimulationResult:
+        """Simulates an inbound Real Time Payments transfer to your account.
+
+        Real Time
+        Payments are a beta feature.
 
         Args:
-          inbound_ach_transfer_return_id: The identifier of the Inbound ACH Transfer Return to retrieve.
+          account_number_id: The identifier of the Account Number the inbound Real Time Payments Transfer is
+              for.
 
-          extra_headers: Send extra headers
+          amount: The transfer amount in USD cents. Must be positive.
 
-          extra_query: Add additional query parameters to the request
+          debtor_account_number: The account number of the account that sent the transfer.
 
-          extra_body: Add additional JSON properties to the request
+          debtor_name: The name provided by the sender of the transfer.
 
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return self._get(
-            f"/inbound_ach_transfer_returns/{inbound_ach_transfer_return_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=InboundACHTransferReturn,
-        )
+          debtor_routing_number: The routing number of the account that sent the transfer.
 
-    def list(
-        self,
-        *,
-        cursor: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> SyncPage[InboundACHTransferReturn]:
-        """
-        List Inbound ACH Transfer Returns
-
-        Args:
-          cursor: Return the page of entries after this one.
+          remittance_information: Additional information included with the transfer.
 
-          limit: Limit the size of the list that is returned. The default (and maximum) is 100
-              objects.
+          request_for_payment_id: The identifier of a pending Request for Payment that this transfer will fulfill.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
-        return self._get_api_list(
-            "/inbound_ach_transfer_returns",
-            page=SyncPage[InboundACHTransferReturn],
+        return self._post(
+            "/simulations/inbound_real_time_payments_transfers",
+            body=maybe_transform(
+                {
+                    "account_number_id": account_number_id,
+                    "amount": amount,
+                    "debtor_account_number": debtor_account_number,
+                    "debtor_name": debtor_name,
+                    "debtor_routing_number": debtor_routing_number,
+                    "remittance_information": remittance_information,
+                    "request_for_payment_id": request_for_payment_id,
+                },
+                real_time_payments_transfer_create_inbound_params.RealTimePaymentsTransferCreateInboundParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=maybe_transform(
-                    {
-                        "cursor": cursor,
-                        "limit": limit,
-                    },
-                    inbound_ach_transfer_return_list_params.InboundACHTransferReturnListParams,
-                ),
+                idempotency_key=idempotency_key,
             ),
-            model=InboundACHTransferReturn,
+            cast_to=InboundRealTimePaymentsTransferSimulationResult,
         )
 
 
-class AsyncInboundACHTransferReturns(AsyncAPIResource):
-    async def create(
+class AsyncRealTimePaymentsTransfers(AsyncAPIResource):
+    async def complete(
         self,
+        real_time_payments_transfer_id: str,
         *,
-        reason: Literal[
-            "authorization_revoked_by_customer",
-            "payment_stopped",
-            "customer_advised_unauthorized_improper_ineligible_or_incomplete",
-            "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
-            "beneficiary_or_account_holder_deceased",
-            "credit_entry_refused_by_receiver",
-            "duplicate_entry",
-            "corporate_customer_advised_not_authorized",
-        ],
-        transaction_id: str,
+        rejection: real_time_payments_transfer_complete_params.Rejection | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> InboundACHTransferReturn:
+    ) -> RealTimePaymentsTransfer:
         """
-        Create an ACH Return
+        Simulates submission of a Real Time Payments transfer and handling the response
+        from the destination financial institution. This transfer must first have a
+        `status` of `pending_submission`.
 
         Args:
-          reason: The reason why this transfer will be returned. The most usual return codes are
-              `payment_stopped` for debits and `credit_entry_refused_by_receiver` for credits.
+          real_time_payments_transfer_id: The identifier of the Real Time Payments Transfer you wish to complete.
 
-          transaction_id: The transaction identifier of the Inbound ACH Transfer to return to the
-              originating financial institution.
+          rejection: If set, the simulation will reject the transfer.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            "/inbound_ach_transfer_returns",
+            f"/simulations/real_time_payments_transfers/{real_time_payments_transfer_id}/complete",
             body=maybe_transform(
-                {
-                    "reason": reason,
-                    "transaction_id": transaction_id,
-                },
-                inbound_ach_transfer_return_create_params.InboundACHTransferReturnCreateParams,
+                {"rejection": rejection},
+                real_time_payments_transfer_complete_params.RealTimePaymentsTransferCompleteParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=InboundACHTransferReturn,
+            cast_to=RealTimePaymentsTransfer,
         )
 
-    async def retrieve(
+    async def create_inbound(
         self,
-        inbound_ach_transfer_return_id: str,
         *,
+        account_number_id: str,
+        amount: int,
+        debtor_account_number: str | NotGiven = NOT_GIVEN,
+        debtor_name: str | NotGiven = NOT_GIVEN,
+        debtor_routing_number: str | NotGiven = NOT_GIVEN,
+        remittance_information: str | NotGiven = NOT_GIVEN,
+        request_for_payment_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> InboundACHTransferReturn:
-        """
-        Retrieve an Inbound ACH Transfer Return
+        idempotency_key: str | None = None,
+    ) -> InboundRealTimePaymentsTransferSimulationResult:
+        """Simulates an inbound Real Time Payments transfer to your account.
 
-        Args:
-          inbound_ach_transfer_return_id: The identifier of the Inbound ACH Transfer Return to retrieve.
+        Real Time
+        Payments are a beta feature.
 
-          extra_headers: Send extra headers
+        Args:
+          account_number_id: The identifier of the Account Number the inbound Real Time Payments Transfer is
+              for.
 
-          extra_query: Add additional query parameters to the request
+          amount: The transfer amount in USD cents. Must be positive.
 
-          extra_body: Add additional JSON properties to the request
+          debtor_account_number: The account number of the account that sent the transfer.
 
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return await self._get(
-            f"/inbound_ach_transfer_returns/{inbound_ach_transfer_return_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=InboundACHTransferReturn,
-        )
+          debtor_name: The name provided by the sender of the transfer.
 
-    def list(
-        self,
-        *,
-        cursor: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[InboundACHTransferReturn, AsyncPage[InboundACHTransferReturn]]:
-        """
-        List Inbound ACH Transfer Returns
+          debtor_routing_number: The routing number of the account that sent the transfer.
 
-        Args:
-          cursor: Return the page of entries after this one.
+          remittance_information: Additional information included with the transfer.
 
-          limit: Limit the size of the list that is returned. The default (and maximum) is 100
-              objects.
+          request_for_payment_id: The identifier of a pending Request for Payment that this transfer will fulfill.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
-        return self._get_api_list(
-            "/inbound_ach_transfer_returns",
-            page=AsyncPage[InboundACHTransferReturn],
+        return await self._post(
+            "/simulations/inbound_real_time_payments_transfers",
+            body=maybe_transform(
+                {
+                    "account_number_id": account_number_id,
+                    "amount": amount,
+                    "debtor_account_number": debtor_account_number,
+                    "debtor_name": debtor_name,
+                    "debtor_routing_number": debtor_routing_number,
+                    "remittance_information": remittance_information,
+                    "request_for_payment_id": request_for_payment_id,
+                },
+                real_time_payments_transfer_create_inbound_params.RealTimePaymentsTransferCreateInboundParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=maybe_transform(
-                    {
-                        "cursor": cursor,
-                        "limit": limit,
-                    },
-                    inbound_ach_transfer_return_list_params.InboundACHTransferReturnListParams,
-                ),
+                idempotency_key=idempotency_key,
             ),
-            model=InboundACHTransferReturn,
+            cast_to=InboundRealTimePaymentsTransferSimulationResult,
         )
```

### Comparing `increase-0.8.1/src/increase/resources/inbound_wire_drawdown_requests.py` & `increase-0.9.0/src/increase/resources/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/limits.py` & `increase-0.9.0/src/increase/resources/limits.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,21 +32,34 @@
     ) -> Limit:
         """
         Create a Limit
 
         Args:
           metric: The metric for the limit.
 
+              - `count` - The maximum number of debits allowed.
+              - `volume` - The maximum volume of debits allowed in the minor unit of the
+                model's currency.
+
           model_id: The identifier of the Account or Account Number you wish to associate the limit
               with.
 
           value: The value to test the limit against.
 
           interval: The interval for the metric. Required if `metric` is `count` or `volume`.
 
+              - `transaction` - Enforce the limit per-transaction.
+              - `day` - Enforce the limit based on the previous 24 hour period.
+              - `week` - Enforce the limit based on the previous seven days.
+              - `month` - Enforce the limit based on the previous month, going back to the
+                current day in the previous month, or as close as possible given month length
+                differences.
+              - `year` - Enforce the limit based on the previous year.
+              - `all_time` - Enforce the limit for all time.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -124,14 +137,17 @@
         Update a Limit
 
         Args:
           limit_id: The limit to update.
 
           status: The status to update the limit with.
 
+              - `inactive` - Disable the limit temporarily.
+              - `active` - Activate the limit.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -226,21 +242,34 @@
     ) -> Limit:
         """
         Create a Limit
 
         Args:
           metric: The metric for the limit.
 
+              - `count` - The maximum number of debits allowed.
+              - `volume` - The maximum volume of debits allowed in the minor unit of the
+                model's currency.
+
           model_id: The identifier of the Account or Account Number you wish to associate the limit
               with.
 
           value: The value to test the limit against.
 
           interval: The interval for the metric. Required if `metric` is `count` or `volume`.
 
+              - `transaction` - Enforce the limit per-transaction.
+              - `day` - Enforce the limit based on the previous 24 hour period.
+              - `week` - Enforce the limit based on the previous seven days.
+              - `month` - Enforce the limit based on the previous month, going back to the
+                current day in the previous month, or as close as possible given month length
+                differences.
+              - `year` - Enforce the limit based on the previous year.
+              - `all_time` - Enforce the limit for all time.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -318,14 +347,17 @@
         Update a Limit
 
         Args:
           limit_id: The limit to update.
 
           status: The status to update the limit with.
 
+              - `inactive` - Disable the limit temporarily.
+              - `active` - Activate the limit.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
```

### Comparing `increase-0.8.1/src/increase/resources/oauth_connections.py` & `increase-0.9.0/src/increase/resources/oauth_connections.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/pending_transactions.py` & `increase-0.9.0/src/increase/resources/pending_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/programs.py` & `increase-0.9.0/src/increase/resources/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/real_time_decisions.py` & `increase-0.9.0/src/increase/resources/real_time_decisions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/real_time_payments_transfers.py` & `increase-0.9.0/src/increase/resources/real_time_payments_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/routing_numbers.py` & `increase-0.9.0/src/increase/resources/routing_numbers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/__init__.py` & `increase-0.9.0/src/increase/resources/simulations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .cards import Cards, AsyncCards
 from .programs import Programs, AsyncPrograms
 from .documents import Documents, AsyncDocuments
 from .simulations import Simulations, AsyncSimulations
 from .card_refunds import CardRefunds, AsyncCardRefunds
 from .ach_transfers import ACHTransfers, AsyncACHTransfers
 from .card_disputes import CardDisputes, AsyncCardDisputes
+from .card_profiles import CardProfiles, AsyncCardProfiles
 from .check_deposits import CheckDeposits, AsyncCheckDeposits
 from .wire_transfers import WireTransfers, AsyncWireTransfers
 from .check_transfers import CheckTransfers, AsyncCheckTransfers
 from .account_transfers import AccountTransfers, AsyncAccountTransfers
 from .interest_payments import InterestPayments, AsyncInterestPayments
 from .account_statements import AccountStatements, AsyncAccountStatements
 from .real_time_payments_transfers import (
@@ -31,14 +32,16 @@
     "AsyncAccountTransfers",
     "AccountStatements",
     "AsyncAccountStatements",
     "ACHTransfers",
     "AsyncACHTransfers",
     "CardDisputes",
     "AsyncCardDisputes",
+    "CardProfiles",
+    "AsyncCardProfiles",
     "CardRefunds",
     "AsyncCardRefunds",
     "CheckTransfers",
     "AsyncCheckTransfers",
     "Documents",
     "AsyncDocuments",
     "DigitalWalletTokenRequests",
```

### Comparing `increase-0.8.1/src/increase/resources/simulations/account_statements.py` & `increase-0.9.0/src/increase/resources/simulations/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/account_transfers.py` & `increase-0.9.0/src/increase/resources/simulations/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/card_disputes.py` & `increase-0.9.0/src/increase/resources/simulations/card_disputes.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,14 +36,18 @@
         be actioned one time and must have a status of `pending_reviewing`.
 
         Args:
           card_dispute_id: The dispute you would like to action.
 
           status: The status to move the dispute to.
 
+              - `accepted` - The Card Dispute has been accepted and your funds have been
+                returned.
+              - `rejected` - The Card Dispute has been rejected.
+
           explanation: Why the dispute was rejected. Not required for accepting disputes.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -94,14 +98,18 @@
         be actioned one time and must have a status of `pending_reviewing`.
 
         Args:
           card_dispute_id: The dispute you would like to action.
 
           status: The status to move the dispute to.
 
+              - `accepted` - The Card Dispute has been accepted and your funds have been
+                returned.
+              - `rejected` - The Card Dispute has been rejected.
+
           explanation: Why the dispute was rejected. Not required for accepting disputes.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
```

### Comparing `increase-0.8.1/src/increase/resources/simulations/card_refunds.py` & `increase-0.9.0/src/increase/resources/simulations/card_refunds.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/cards.py` & `increase-0.9.0/src/increase/resources/simulations/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/check_deposits.py` & `increase-0.9.0/src/increase/resources/simulations/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/check_transfers.py` & `increase-0.9.0/src/increase/resources/simulations/check_transfers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing_extensions import Literal
-
 from ...types import CheckTransfer
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
-from ...types.simulations import check_transfer_return_params
 
 __all__ = ["CheckTransfers", "AsyncCheckTransfers"]
 
 
 class CheckTransfers(SyncAPIResource):
     def deposit(
         self,
@@ -95,59 +91,14 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
-    def return_(
-        self,
-        check_transfer_id: str,
-        *,
-        reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"],
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
-        idempotency_key: str | None = None,
-    ) -> CheckTransfer:
-        """
-        Simulates a [Check Transfer](#check-transfers) being returned via USPS to
-        Increase. This transfer must first have a `status` of `mailed`.
-
-        Args:
-          check_transfer_id: The identifier of the Check Transfer you wish to mark returned.
-
-          reason: The reason why the Check Transfer was returned to Increase.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-
-          idempotency_key: Specify a custom idempotency key for this request
-        """
-        return self._post(
-            f"/simulations/check_transfers/{check_transfer_id}/return",
-            body=maybe_transform({"reason": reason}, check_transfer_return_params.CheckTransferReturnParams),
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                timeout=timeout,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=CheckTransfer,
-        )
-
 
 class AsyncCheckTransfers(AsyncAPIResource):
     async def deposit(
         self,
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -223,54 +174,9 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=CheckTransfer,
-        )
-
-    async def return_(
-        self,
-        check_transfer_id: str,
-        *,
-        reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"],
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
-        idempotency_key: str | None = None,
-    ) -> CheckTransfer:
-        """
-        Simulates a [Check Transfer](#check-transfers) being returned via USPS to
-        Increase. This transfer must first have a `status` of `mailed`.
-
-        Args:
-          check_transfer_id: The identifier of the Check Transfer you wish to mark returned.
-
-          reason: The reason why the Check Transfer was returned to Increase.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-
-          idempotency_key: Specify a custom idempotency key for this request
-        """
-        return await self._post(
-            f"/simulations/check_transfers/{check_transfer_id}/return",
-            body=maybe_transform({"reason": reason}, check_transfer_return_params.CheckTransferReturnParams),
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                timeout=timeout,
-                idempotency_key=idempotency_key,
-            ),
             cast_to=CheckTransfer,
         )
```

### Comparing `increase-0.8.1/src/increase/resources/simulations/digital_wallet_token_requests.py` & `increase-0.9.0/src/increase/resources/simulations/digital_wallet_token_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/documents.py` & `increase-0.9.0/src/increase/resources/simulations/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py` & `increase-0.9.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/interest_payments.py` & `increase-0.9.0/src/increase/resources/simulations/interest_payments.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/programs.py` & `increase-0.9.0/src/increase/resources/simulations/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/simulations/simulations.py` & `increase-0.9.0/src/increase/resources/simulations/simulations.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .cards import Cards, AsyncCards
 from .programs import Programs, AsyncPrograms
 from .documents import Documents, AsyncDocuments
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from .card_refunds import CardRefunds, AsyncCardRefunds
 from .ach_transfers import ACHTransfers, AsyncACHTransfers
 from .card_disputes import CardDisputes, AsyncCardDisputes
+from .card_profiles import CardProfiles, AsyncCardProfiles
 from .check_deposits import CheckDeposits, AsyncCheckDeposits
 from .wire_transfers import WireTransfers, AsyncWireTransfers
 from .check_transfers import CheckTransfers, AsyncCheckTransfers
 from .account_transfers import AccountTransfers, AsyncAccountTransfers
 from .interest_payments import InterestPayments, AsyncInterestPayments
 from .account_statements import AccountStatements, AsyncAccountStatements
 from .real_time_payments_transfers import (
@@ -37,14 +38,15 @@
 
 
 class Simulations(SyncAPIResource):
     account_transfers: AccountTransfers
     account_statements: AccountStatements
     ach_transfers: ACHTransfers
     card_disputes: CardDisputes
+    card_profiles: CardProfiles
     card_refunds: CardRefunds
     check_transfers: CheckTransfers
     documents: Documents
     digital_wallet_token_requests: DigitalWalletTokenRequests
     check_deposits: CheckDeposits
     programs: Programs
     inbound_wire_drawdown_requests: InboundWireDrawdownRequests
@@ -55,14 +57,15 @@
 
     def __init__(self, client: Increase) -> None:
         super().__init__(client)
         self.account_transfers = AccountTransfers(client)
         self.account_statements = AccountStatements(client)
         self.ach_transfers = ACHTransfers(client)
         self.card_disputes = CardDisputes(client)
+        self.card_profiles = CardProfiles(client)
         self.card_refunds = CardRefunds(client)
         self.check_transfers = CheckTransfers(client)
         self.documents = Documents(client)
         self.digital_wallet_token_requests = DigitalWalletTokenRequests(client)
         self.check_deposits = CheckDeposits(client)
         self.programs = Programs(client)
         self.inbound_wire_drawdown_requests = InboundWireDrawdownRequests(client)
@@ -73,14 +76,15 @@
 
 
 class AsyncSimulations(AsyncAPIResource):
     account_transfers: AsyncAccountTransfers
     account_statements: AsyncAccountStatements
     ach_transfers: AsyncACHTransfers
     card_disputes: AsyncCardDisputes
+    card_profiles: AsyncCardProfiles
     card_refunds: AsyncCardRefunds
     check_transfers: AsyncCheckTransfers
     documents: AsyncDocuments
     digital_wallet_token_requests: AsyncDigitalWalletTokenRequests
     check_deposits: AsyncCheckDeposits
     programs: AsyncPrograms
     inbound_wire_drawdown_requests: AsyncInboundWireDrawdownRequests
@@ -91,14 +95,15 @@
 
     def __init__(self, client: AsyncIncrease) -> None:
         super().__init__(client)
         self.account_transfers = AsyncAccountTransfers(client)
         self.account_statements = AsyncAccountStatements(client)
         self.ach_transfers = AsyncACHTransfers(client)
         self.card_disputes = AsyncCardDisputes(client)
+        self.card_profiles = AsyncCardProfiles(client)
         self.card_refunds = AsyncCardRefunds(client)
         self.check_transfers = AsyncCheckTransfers(client)
         self.documents = AsyncDocuments(client)
         self.digital_wallet_token_requests = AsyncDigitalWalletTokenRequests(client)
         self.check_deposits = AsyncCheckDeposits(client)
         self.programs = AsyncPrograms(client)
         self.inbound_wire_drawdown_requests = AsyncInboundWireDrawdownRequests(client)
```

### Comparing `increase-0.8.1/src/increase/resources/simulations/wire_transfers.py` & `increase-0.9.0/src/increase/resources/simulations/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/transactions.py` & `increase-0.9.0/src/increase/resources/transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/wire_drawdown_requests.py` & `increase-0.9.0/src/increase/resources/wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/resources/wire_transfers.py` & `increase-0.9.0/src/increase/resources/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/__init__.py` & `increase-0.9.0/src/increase/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,17 @@
 )
 from .bookkeeping_account_create_params import (
     BookkeepingAccountCreateParams as BookkeepingAccountCreateParams,
 )
 from .wire_drawdown_request_list_params import (
     WireDrawdownRequestListParams as WireDrawdownRequestListParams,
 )
+from .check_transfer_stop_payment_params import (
+    CheckTransferStopPaymentParams as CheckTransferStopPaymentParams,
+)
 from .bookkeeping_entry_set_create_params import (
     BookkeepingEntrySetCreateParams as BookkeepingEntrySetCreateParams,
 )
 from .wire_drawdown_request_create_params import (
     WireDrawdownRequestCreateParams as WireDrawdownRequestCreateParams,
 )
 from .inbound_ach_transfer_return_list_params import (
```

### Comparing `increase-0.8.1/src/increase/types/account.py` & `increase-0.9.0/src/increase/types/account.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,14 +19,21 @@
     was created.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Account
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     entity_id: Optional[str]
     """The identifier for the Entity the Account belongs to."""
 
     informational_entity_id: Optional[str]
     """
@@ -53,14 +60,18 @@
     "0.01".
     """
 
     name: str
     """The name you choose for the Account."""
 
     status: Literal["open", "closed"]
-    """The status of the Account."""
+    """The status of the Account.
+
+    - `open` - Open Accounts that are ready to use.
+    - `closed` - Closed Accounts on which no new activity can occur.
+    """
 
     type: Literal["account"]
     """A constant representing the object's type.
 
     For this resource it will always be `account`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/account_create_params.py` & `increase-0.9.0/src/increase/types/account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/account_list_params.py` & `increase-0.9.0/src/increase/types/card_list_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Union
 from datetime import datetime
-from typing_extensions import Literal, Annotated, TypedDict
+from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["AccountListParams", "CreatedAt"]
+__all__ = ["CardListParams", "CreatedAt"]
 
 
-class AccountListParams(TypedDict, total=False):
+class CardListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Cards to ones belonging to the specified Account."""
+
     created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
-    entity_id: str
-    """Filter Accounts for those belonging to the specified Entity."""
-
-    informational_entity_id: str
-    """Filter Accounts for those belonging to the specified Entity as informational."""
-
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
-    status: Literal["open", "closed"]
-    """Filter Accounts for those with the specified status."""
-
 
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
```

### Comparing `increase-0.8.1/src/increase/types/account_number.py` & `increase-0.9.0/src/increase/types/account_number.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     name: str
     """The name you choose for the Account Number."""
 
     routing_number: str
     """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     status: Literal["active", "disabled", "canceled"]
-    """This indicates if payments can be made to the Account Number."""
+    """This indicates if payments can be made to the Account Number.
+
+    - `active` - The account number is active.
+    - `disabled` - The account number is temporarily disabled.
+    - `canceled` - The account number is permanently disabled.
+    """
 
     type: Literal["account_number"]
     """A constant representing the object's type.
 
     For this resource it will always be `account_number`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/account_number_list_params.py` & `increase-0.9.0/src/increase/types/account_statement_list_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Union
 from datetime import datetime
-from typing_extensions import Literal, Annotated, TypedDict
+from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["AccountNumberListParams", "CreatedAt"]
+__all__ = ["AccountStatementListParams", "StatementPeriodStart"]
 
 
-class AccountNumberListParams(TypedDict, total=False):
+class AccountStatementListParams(TypedDict, total=False):
     account_id: str
-    """Filter Account Numbers to those belonging to the specified Account."""
-
-    created_at: CreatedAt
+    """Filter Account Statements to those belonging to the specified Account."""
 
     cursor: str
     """Return the page of entries after this one."""
 
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
-    status: Literal["active", "disabled", "canceled"]
-    """The status to retrieve Account Numbers for."""
+    statement_period_start: StatementPeriodStart
 
 
-class CreatedAt(TypedDict, total=False):
+class StatementPeriodStart(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
     before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
```

### Comparing `increase-0.8.1/src/increase/types/account_statement.py` & `increase-0.9.0/src/increase/types/account_statement.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/account_statement_list_params.py` & `increase-0.9.0/src/increase/types/ach_transfer_list_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,37 @@
 
 from typing import Union
 from datetime import datetime
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["AccountStatementListParams", "StatementPeriodStart"]
+__all__ = ["ACHTransferListParams", "CreatedAt"]
 
 
-class AccountStatementListParams(TypedDict, total=False):
+class ACHTransferListParams(TypedDict, total=False):
     account_id: str
-    """Filter Account Statements to those belonging to the specified Account."""
+    """Filter ACH Transfers to those that originated from the specified Account."""
+
+    created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
+    external_account_id: str
+    """Filter ACH Transfers to those made to the specified External Account."""
+
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
-    statement_period_start: StatementPeriodStart
-
 
-class StatementPeriodStart(TypedDict, total=False):
+class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
     before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
```

### Comparing `increase-0.8.1/src/increase/types/account_transfer.py` & `increase-0.9.0/src/increase/types/account_transfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,14 +68,21 @@
     the transfer was created.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
     account currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
     """The description that will show on the transactions."""
 
     destination_account_id: str
     """The destination account's identifier."""
@@ -83,15 +90,20 @@
     destination_transaction_id: Optional[str]
     """The ID for the transaction receiving the transfer."""
 
     network: Literal["account"]
     """The transfer's network."""
 
     status: Literal["pending_approval", "canceled", "complete"]
-    """The lifecycle status of the transfer."""
+    """The lifecycle status of the transfer.
+
+    - `pending_approval` - The transfer is pending approval.
+    - `canceled` - The transfer has been canceled.
+    - `complete` - The transfer has been completed.
+    """
 
     transaction_id: Optional[str]
     """The ID for the transaction funding the transfer."""
 
     type: Literal["account_transfer"]
     """A constant representing the object's type.
```

### Comparing `increase-0.8.1/src/increase/types/account_transfer_create_params.py` & `increase-0.9.0/src/increase/types/account_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/account_transfer_list_params.py` & `increase-0.9.0/src/increase/types/account_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/ach_prenotification.py` & `increase-0.9.0/src/increase/types/ach_prenotification.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,28 +45,38 @@
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the prenotification was created.
     """
 
     credit_debit_indicator: Optional[Literal["credit", "debit"]]
-    """If the notification is for a future credit or debit."""
+    """If the notification is for a future credit or debit.
+
+    - `credit` - The Prenotification is for an anticipated credit.
+    - `debit` - The Prenotification is for an anticipated debit.
+    """
 
     effective_date: Optional[datetime]
     """
     The effective date in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     """
 
     prenotification_return: Optional[PrenotificationReturn]
     """If your prenotification is returned, this will contain details of the return."""
 
     routing_number: str
     """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     status: Literal["pending_submitting", "requires_attention", "returned", "submitted"]
-    """The lifecycle status of the ACH Prenotification."""
+    """The lifecycle status of the ACH Prenotification.
+
+    - `pending_submitting` - The Prenotification is pending submission.
+    - `requires_attention` - The Prenotification requires attention.
+    - `returned` - The Prenotification has been returned.
+    - `submitted` - The Prentification is complete.
+    """
 
     type: Literal["ach_prenotification"]
     """A constant representing the object's type.
 
     For this resource it will always be `ach_prenotification`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/ach_prenotification_create_params.py` & `increase-0.9.0/src/increase/types/ach_prenotification_create_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,15 +33,19 @@
     company_entry_description: str
     """The description of the transfer you wish to be shown to the recipient."""
 
     company_name: str
     """The name by which the recipient knows you."""
 
     credit_debit_indicator: Literal["credit", "debit"]
-    """Whether the Prenotification is for a future debit or credit."""
+    """Whether the Prenotification is for a future debit or credit.
+
+    - `credit` - The Prenotification is for an anticipated credit.
+    - `debit` - The Prenotification is for an anticipated debit.
+    """
 
     effective_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """
     The transfer effective date in
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     """
 
@@ -53,8 +57,13 @@
 
     This value is information and not verified by the recipient's bank.
     """
 
     standard_entry_class_code: Literal[
         "corporate_credit_or_debit", "prearranged_payments_and_deposit", "internet_initiated"
     ]
-    """The Standard Entry Class (SEC) code to use for the ACH Prenotification."""
+    """The Standard Entry Class (SEC) code to use for the ACH Prenotification.
+
+    - `corporate_credit_or_debit` - Corporate Credit and Debit (CCD).
+    - `prearranged_payments_and_deposit` - Prearranged Payments and Deposits (PPD).
+    - `internet_initiated` - Internet Initiated (WEB).
+    """
```

### Comparing `increase-0.8.1/src/increase/types/ach_prenotification_list_params.py` & `increase-0.9.0/src/increase/types/ach_prenotification_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/ach_transfer.py` & `increase-0.9.0/src/increase/types/real_time_decision.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,281 +1,268 @@
 # File generated from our OpenAPI spec by Stainless.
 
-from typing import List, Optional
-from datetime import date, datetime
+from typing import Optional
+from datetime import datetime
 from typing_extensions import Literal
 
-from pydantic import Field as FieldInfo
-
+from ..types import shared
 from .._models import BaseModel
 
-__all__ = ["ACHTransfer", "Approval", "Cancellation", "NotificationsOfChange", "Return", "Submission"]
-
-
-class Approval(BaseModel):
-    approved_at: datetime
+__all__ = [
+    "RealTimeDecision",
+    "CardAuthorization",
+    "CardAuthorizationNetworkDetails",
+    "CardAuthorizationNetworkDetailsVisa",
+    "DigitalWalletAuthentication",
+    "DigitalWalletToken",
+]
+
+
+class CardAuthorizationNetworkDetailsVisa(BaseModel):
+    electronic_commerce_indicator: Optional[
+        Literal[
+            "mail_phone_order",
+            "recurring",
+            "installment",
+            "unknown_mail_phone_order",
+            "secure_electronic_commerce",
+            "non_authenticated_security_transaction_at_3ds_capable_merchant",
+            "non_authenticated_security_transaction",
+            "non_secure_transaction",
+        ]
+    ]
     """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the transfer was approved.
+    For electronic commerce transactions, this identifies the level of security used
+    in obtaining the customer's payment credential. For mail or telephone order
+    transactions, identifies the type of mail or telephone order.
+
+    - `mail_phone_order` - Single transaction of a mail/phone order: Use to indicate
+      that the transaction is a mail/phone order purchase, not a recurring
+      transaction or installment payment. For domestic transactions in the US
+      region, this value may also indicate one bill payment transaction in the
+      card-present or card-absent environments.
+    - `recurring` - Recurring transaction: Payment indicator used to indicate a
+      recurring transaction that originates from an acquirer in the US region.
+    - `installment` - Installment payment: Payment indicator used to indicate one
+      purchase of goods or services that is billed to the account in multiple
+      charges over a period of time agreed upon by the cardholder and merchant from
+      transactions that originate from an acquirer in the US region.
+    - `unknown_mail_phone_order` - Unknown classification: other mail order: Use to
+      indicate that the type of mail/telephone order is unknown.
+    - `secure_electronic_commerce` - Secure electronic commerce transaction: Use to
+      indicate that the electronic commerce transaction has been authenticated using
+      e.g., 3-D Secure
+    - `non_authenticated_security_transaction_at_3ds_capable_merchant` -
+      Non-authenticated security transaction at a 3-D Secure-capable merchant, and
+      merchant attempted to authenticate the cardholder using 3-D Secure: Use to
+      identify an electronic commerce transaction where the merchant attempted to
+      authenticate the cardholder using 3-D Secure, but was unable to complete the
+      authentication because the issuer or cardholder does not participate in the
+      3-D Secure program.
+    - `non_authenticated_security_transaction` - Non-authenticated security
+      transaction: Use to identify an electronic commerce transaction that uses data
+      encryption for security however , cardholder authentication is not performed
+      using 3-D Secure.
+    - `non_secure_transaction` - Non-secure transaction: Use to identify an
+      electronic commerce transaction that has no data protection.
+    """
+
+    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
+    """
+    The method used to enter the cardholder's primary account number and card
+    expiration date
     """
 
-    approved_by: Optional[str]
-    """
-    If the Transfer was approved by a user in the dashboard, the email address of
-    that user.
-    """
 
+class CardAuthorizationNetworkDetails(BaseModel):
+    visa: CardAuthorizationNetworkDetailsVisa
+    """Fields specific to the `visa` network"""
 
-class Cancellation(BaseModel):
-    canceled_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the Transfer was canceled.
-    """
 
-    canceled_by: Optional[str]
-    """
-    If the Transfer was canceled by a user in the dashboard, the email address of
-    that user.
-    """
+class CardAuthorization(BaseModel):
+    account_id: str
+    """The identifier of the Account the authorization will debit."""
 
+    card_id: str
+    """The identifier of the Card that is being authorized."""
 
-class NotificationsOfChange(BaseModel):
-    change_code: str
-    """The type of change that occurred."""
+    decision: Optional[Literal["approve", "decline"]]
+    """Whether or not the authorization was approved.
 
-    corrected_data: str
-    """The corrected data."""
+    - `approve` - Approve the authorization.
+    - `decline` - Decline the authorization.
+    """
 
-    created_at: datetime
+    merchant_acceptor_id: str
     """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the notification occurred.
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
     """
 
-
-class Return(BaseModel):
-    created_at: datetime
+    merchant_category_code: Optional[str]
     """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the transfer was created.
+    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
+    card is transacting with.
     """
 
-    raw_return_reason_code: str
-    """The three character ACH return code, in the range R01 to R85."""
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
 
-    return_reason_code: Literal[
-        "insufficient_fund",
-        "no_account",
-        "account_closed",
-        "invalid_account_number_structure",
-        "account_frozen_entry_returned_per_ofac_instruction",
-        "credit_entry_refused_by_receiver",
-        "unauthorized_debit_to_consumer_account_using_corporate_sec_code",
-        "corporate_customer_advised_not_authorized",
-        "payment_stopped",
-        "non_transaction_account",
-        "uncollected_funds",
-        "routing_number_check_digit_error",
-        "customer_advised_unauthorized_improper_ineligible_or_incomplete",
-        "amount_field_error",
-        "authorization_revoked_by_customer",
-        "invalid_ach_routing_number",
-        "file_record_edit_criteria",
-        "enr_invalid_individual_name",
-        "returned_per_odfi_request",
-        "limited_participation_dfi",
-        "incorrectly_coded_outbound_international_payment",
-        "account_sold_to_another_dfi",
-        "addenda_error",
-        "beneficiary_or_account_holder_deceased",
-        "customer_advised_not_within_authorization_terms",
-        "corrected_return",
-        "duplicate_entry",
-        "duplicate_return",
-        "enr_duplicate_enrollment",
-        "enr_invalid_dfi_account_number",
-        "enr_invalid_individual_id_number",
-        "enr_invalid_representative_payee_indicator",
-        "enr_invalid_transaction_code",
-        "enr_return_of_enr_entry",
-        "enr_routing_number_check_digit_error",
-        "entry_not_processed_by_gateway",
-        "field_error",
-        "foreign_receiving_dfi_unable_to_settle",
-        "iat_entry_coding_error",
-        "improper_effective_entry_date",
-        "improper_source_document_source_document_presented",
-        "invalid_company_id",
-        "invalid_foreign_receiving_dfi_identification",
-        "invalid_individual_id_number",
-        "item_and_rck_entry_presented_for_payment",
-        "item_related_to_rck_entry_is_ineligible",
-        "mandatory_field_error",
-        "misrouted_dishonored_return",
-        "misrouted_return",
-        "no_errors_found",
-        "non_acceptance_of_r62_dishonored_return",
-        "non_participant_in_iat_program",
-        "permissible_return_entry",
-        "permissible_return_entry_not_accepted",
-        "rdfi_non_settlement",
-        "rdfi_participant_in_check_truncation_program",
-        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
-        "return_not_a_duplicate",
-        "return_of_erroneous_or_reversing_debit",
-        "return_of_improper_credit_entry",
-        "return_of_improper_debit_entry",
-        "return_of_xck_entry",
-        "source_document_presented_for_payment",
-        "state_law_affecting_rck_acceptance",
-        "stop_payment_on_item_related_to_rck_entry",
-        "stop_payment_on_source_document",
-        "timely_original_return",
-        "trace_number_error",
-        "untimely_dishonored_return",
-        "untimely_return",
-    ]
-    """Why the ACH Transfer was returned."""
+    merchant_country: Optional[str]
+    """The country the merchant resides in."""
 
-    transaction_id: str
-    """The identifier of the Tranasaction associated with this return."""
+    merchant_descriptor: str
+    """The merchant descriptor of the merchant the card is transacting with."""
 
-    transfer_id: str
-    """The identifier of the ACH Transfer associated with this return."""
+    network: Literal["visa"]
+    """The payment network used to process this card authorization
 
+    - `visa` - Visa
+    """
 
-class Submission(BaseModel):
-    submitted_at: datetime
-    """When the ACH transfer was sent to FedACH."""
+    network_details: CardAuthorizationNetworkDetails
+    """Fields specific to the `network`"""
 
-    trace_number: str
-    """The trace number for the submission."""
+    presentment_amount: int
+    """
+    The amount of the attempted authorization in the currency the card user sees at
+    the time of purchase, in the minor unit of that currency. For dollars, for
+    example, this is cents.
+    """
 
+    presentment_currency: str
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the currency the
+    user sees at the time of purchase.
+    """
 
-class ACHTransfer(BaseModel):
-    id: str
-    """The ACH transfer's identifier."""
+    settlement_amount: int
+    """The amount of the attempted authorization in the currency it will be settled in.
 
-    account_id: str
-    """The Account to which the transfer belongs."""
+    This currency is the same as that of the Account the card belongs to.
+    """
 
-    account_number: str
-    """The destination account number."""
+    settlement_currency: str
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the currency the
+    transaction will be settled in.
+    """
 
-    addendum: Optional[str]
-    """Additional information that will be sent to the recipient."""
 
-    amount: int
-    """The transfer amount in USD cents.
+class DigitalWalletAuthentication(BaseModel):
+    card_id: str
+    """The identifier of the Card that is being tokenized."""
 
-    A positive amount indicates a credit transfer pushing funds to the receiving
-    account. A negative amount indicates a debit transfer pulling funds from the
-    receiving account.
-    """
+    channel: Literal["sms", "email"]
+    """The channel to send the card user their one-time passcode.
 
-    approval: Optional[Approval]
+    - `sms` - Send one-time passcodes over SMS.
+    - `email` - Send one-time passcodes over email.
     """
-    If your account requires approvals for transfers and the transfer was approved,
-    this will contain details of the approval.
+
+    digital_wallet: Literal["apple_pay", "google_pay"]
+    """The digital wallet app being used.
+
+    - `apple_pay` - Apple Pay
+    - `google_pay` - Google Pay
     """
 
-    cancellation: Optional[Cancellation]
+    email: Optional[str]
+    """The email to send the one-time passcode to if `channel` is equal to `email`."""
+
+    one_time_passcode: str
+    """The one-time passcode to send the card user."""
+
+    phone: Optional[str]
     """
-    If your account requires approvals for transfers and the transfer was not
-    approved, this will contain details of the cancellation.
+    The phone number to send the one-time passcode to if `channel` is equal to
+    `sms`.
     """
 
-    company_descriptive_date: Optional[str]
-    """The description of the date of the transfer."""
+    result: Optional[Literal["success", "failure"]]
+    """Whether your application successfully delivered the one-time passcode.
 
-    company_discretionary_data: Optional[str]
-    """The data you chose to associate with the transfer."""
+    - `success` - Your application successfully delivered the one-time passcode to
+      the cardholder.
+    - `failure` - Your application failed to deliver the one-time passcode to the
+      cardholder.
+    """
 
-    company_entry_description: Optional[str]
-    """The description of the transfer you set to be shown to the recipient."""
 
-    company_name: Optional[str]
-    """The name by which the recipient knows you."""
+class DigitalWalletToken(BaseModel):
+    card_id: str
+    """The identifier of the Card that is being tokenized."""
 
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the transfer was created.
-    """
+    card_profile_id: Optional[str]
+    """The identifier of the Card Profile that was set via the real time decision.
 
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transfer's
-    currency. For ACH transfers this is always equal to `usd`.
+    This will be null until the real time decision is responded to or if the real
+    time decision did not set a card profile.
     """
 
-    effective_date: Optional[date]
+    decision: Optional[Literal["approve", "decline"]]
+    """Whether or not the provisioning request was approved.
+
+    This will be null until the real time decision is responded to.
+
+    - `approve` - Approve the provisioning request.
+    - `decline` - Decline the provisioning request.
     """
-    The transfer effective date in
-    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
+
+    digital_wallet: Literal["apple_pay", "google_pay"]
+    """The digital wallet app being used.
+
+    - `apple_pay` - Apple Pay
+    - `google_pay` - Google Pay
     """
 
-    external_account_id: Optional[str]
-    """The identifier of the External Account the transfer was made to, if any."""
 
-    funding: Literal["checking", "savings"]
-    """The type of the account to which the transfer will be sent."""
+class RealTimeDecision(BaseModel):
+    id: str
+    """The Real-Time Decision identifier."""
 
-    individual_id: Optional[str]
-    """Your identifer for the transfer recipient."""
+    card_authorization: Optional[CardAuthorization]
+    """Fields related to a card authorization."""
 
-    individual_name: Optional[str]
-    """The name of the transfer recipient.
+    category: Literal[
+        "card_authorization_requested", "digital_wallet_token_requested", "digital_wallet_authentication_requested"
+    ]
+    """The category of the Real-Time Decision.
 
-    This value is information and not verified by the recipient's bank.
+    - `card_authorization_requested` - A card is being authorized.
+    - `digital_wallet_token_requested` - A card is being loaded into a digital
+      wallet.
+    - `digital_wallet_authentication_requested` - A card is being loaded into a
+      digital wallet and requires cardholder authentication.
     """
 
-    network: Literal["ach"]
-    """The transfer's network."""
-
-    notifications_of_change: List[NotificationsOfChange]
+    created_at: datetime
     """
-    If the receiving bank accepts the transfer but notifies that future transfers
-    should use different details, this will contain those details.
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the Real-Time Decision was created.
     """
 
-    return_: Optional[Return] = FieldInfo(alias="return")
-    """If your transfer is returned, this will contain details of the return."""
-
-    routing_number: str
-    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
+    digital_wallet_authentication: Optional[DigitalWalletAuthentication]
+    """Fields related to a digital wallet authentication attempt."""
 
-    standard_entry_class_code: Literal[
-        "corporate_credit_or_debit", "prearranged_payments_and_deposit", "internet_initiated"
-    ]
-    """The Standard Entry Class (SEC) code to use for the transfer."""
+    digital_wallet_token: Optional[DigitalWalletToken]
+    """Fields related to a digital wallet token provisioning attempt."""
 
-    statement_descriptor: str
-    """The descriptor that will show on the recipient's bank statement."""
+    status: Literal["pending", "responded", "timed_out"]
+    """The status of the Real-Time Decision.
 
-    status: Literal[
-        "pending_approval",
-        "canceled",
-        "pending_reviewing",
-        "pending_submission",
-        "submitted",
-        "returned",
-        "requires_attention",
-        "rejected",
-    ]
-    """The lifecycle status of the transfer."""
+    - `pending` - The decision is pending action via real-time webhook.
+    - `responded` - Your webhook actioned the real-time decision.
+    - `timed_out` - Your webhook failed to respond to the authorization in time.
+    """
 
-    submission: Optional[Submission]
+    timeout_at: datetime
     """
-    After the transfer is submitted to FedACH, this will contain supplemental
-    details.
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    your application can no longer respond to the Real-Time Decision.
     """
 
-    transaction_id: Optional[str]
-    """The ID for the transaction funding the transfer."""
-
-    type: Literal["ach_transfer"]
+    type: Literal["real_time_decision"]
     """A constant representing the object's type.
 
-    For this resource it will always be `ach_transfer`.
+    For this resource it will always be `real_time_decision`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/ach_transfer_create_params.py` & `increase-0.9.0/src/increase/types/ach_transfer_create_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,15 +77,19 @@
     """The ID of an External Account to initiate a transfer to.
 
     If this parameter is provided, `account_number`, `routing_number`, and `funding`
     must be absent.
     """
 
     funding: Literal["checking", "savings"]
-    """The type of the account to which the transfer will be sent."""
+    """The type of the account to which the transfer will be sent.
+
+    - `checking` - A checking account.
+    - `savings` - A savings account.
+    """
 
     individual_id: str
     """Your identifer for the transfer recipient."""
 
     individual_name: str
     """The name of the transfer recipient.
 
@@ -100,8 +104,13 @@
     The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
     destination account.
     """
 
     standard_entry_class_code: Literal[
         "corporate_credit_or_debit", "prearranged_payments_and_deposit", "internet_initiated"
     ]
-    """The Standard Entry Class (SEC) code to use for the transfer."""
+    """The Standard Entry Class (SEC) code to use for the transfer.
+
+    - `corporate_credit_or_debit` - Corporate Credit and Debit (CCD).
+    - `prearranged_payments_and_deposit` - Prearranged Payments and Deposits (PPD).
+    - `internet_initiated` - Internet Initiated (WEB).
+    """
```

### Comparing `increase-0.8.1/src/increase/types/ach_transfer_list_params.py` & `increase-0.9.0/src/increase/types/wire_transfer_list_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 from typing import Union
 from datetime import datetime
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["ACHTransferListParams", "CreatedAt"]
+__all__ = ["WireTransferListParams", "CreatedAt"]
 
 
-class ACHTransferListParams(TypedDict, total=False):
+class WireTransferListParams(TypedDict, total=False):
     account_id: str
-    """Filter ACH Transfers to those that originated from the specified Account."""
+    """Filter Wire Transfers to those belonging to the specified Account."""
 
     created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
     external_account_id: str
-    """Filter ACH Transfers to those made to the specified External Account."""
+    """Filter Wire Transfers to those made to the specified External Account."""
 
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
```

### Comparing `increase-0.8.1/src/increase/types/balance_lookup_lookup_params.py` & `increase-0.9.0/src/increase/types/balance_lookup_lookup_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/balance_lookup_lookup_response.py` & `increase-0.9.0/src/increase/types/balance_lookup_lookup_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/bookkeeping_account.py` & `increase-0.9.0/src/increase/types/bookkeeping_account.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,19 @@
     id: str
     """The account identifier."""
 
     account_id: Optional[str]
     """The API Account associated with this bookkeeping account."""
 
     compliance_category: Optional[Literal["commingled_cash", "customer_balance"]]
-    """The compliance category of the account."""
+    """The compliance category of the account.
+
+    - `commingled_cash` - A cash in an commingled Increase Account.
+    - `customer_balance` - A customer balance.
+    """
 
     entity_id: Optional[str]
     """The Entity associated with this bookkeeping account."""
 
     name: str
     """The name you choose for the account."""
```

### Comparing `increase-0.8.1/src/increase/types/bookkeeping_account_create_params.py` & `increase-0.9.0/src/increase/types/bookkeeping_account_create_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,11 +11,15 @@
     name: Required[str]
     """The name you choose for the account."""
 
     account_id: str
     """The entity, if `compliance_category` is `commingled_cash`."""
 
     compliance_category: Literal["commingled_cash", "customer_balance"]
-    """The account compliance category."""
+    """The account compliance category.
+
+    - `commingled_cash` - A cash in an commingled Increase Account.
+    - `customer_balance` - A customer balance.
+    """
 
     entity_id: str
     """The entity, if `compliance_category` is `customer_balance`."""
```

### Comparing `increase-0.8.1/src/increase/types/bookkeeping_entry.py` & `increase-0.9.0/src/increase/types/bookkeeping_entry.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/bookkeeping_entry_set.py` & `increase-0.9.0/src/increase/types/bookkeeping_entry_set.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/bookkeeping_entry_set_create_params.py` & `increase-0.9.0/src/increase/types/bookkeeping_entry_set_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/card.py` & `increase-0.9.0/src/increase/types/card.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,19 @@
     expiration_year: int
     """The year the card expires in YYYY format (e.g., 2025)."""
 
     last4: str
     """The last 4 digits of the Card's Primary Account Number."""
 
     status: Literal["active", "disabled", "canceled"]
-    """This indicates if payments can be made with the card."""
+    """This indicates if payments can be made with the card.
+
+    - `active` - The card is active.
+    - `disabled` - The card is temporarily disabled.
+    - `canceled` - The card is permanently canceled.
+    """
 
     type: Literal["card"]
     """A constant representing the object's type.
 
     For this resource it will always be `card`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/card_create_params.py` & `increase-0.9.0/src/increase/types/card_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/card_details.py` & `increase-0.9.0/src/increase/types/card_details.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/card_dispute.py` & `increase-0.9.0/src/increase/types/card_dispute.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,14 +65,20 @@
     rejection: Optional[Rejection]
     """
     If the Card Dispute's status is `rejected`, this will contain details of the
     unsuccessful dispute.
     """
 
     status: Literal["pending_reviewing", "accepted", "rejected"]
-    """The results of the Dispute investigation."""
+    """The results of the Dispute investigation.
+
+    - `pending_reviewing` - The Card Dispute is pending review.
+    - `accepted` - The Card Dispute has been accepted and your funds have been
+      returned.
+    - `rejected` - The Card Dispute has been rejected.
+    """
 
     type: Literal["card_dispute"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_dispute`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/card_dispute_list_params.py` & `increase-0.9.0/src/increase/types/card_dispute_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/card_list_params.py` & `increase-0.9.0/src/increase/types/check_transfer_list_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from typing import Union
 from datetime import datetime
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["CardListParams", "CreatedAt"]
+__all__ = ["CheckTransferListParams", "CreatedAt"]
 
 
-class CardListParams(TypedDict, total=False):
+class CheckTransferListParams(TypedDict, total=False):
     account_id: str
-    """Filter Cards to ones belonging to the specified Account."""
+    """Filter Check Transfers to those that originated from the specified Account."""
 
     created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
     limit: int
```

### Comparing `increase-0.8.1/src/increase/types/card_profile.py` & `increase-0.9.0/src/increase/types/card_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,14 +63,21 @@
     """How Cards should appear in digital wallets such as Apple Pay.
 
     Different wallets will use these values to render card artwork appropriately for
     their app.
     """
 
     status: Literal["pending", "rejected", "active", "archived"]
-    """The status of the Card Profile."""
+    """The status of the Card Profile.
+
+    - `pending` - The Card Profile is awaiting review from Increase and/or
+      processing by card networks.
+    - `rejected` - There is an issue with the Card Profile preventing it from use.
+    - `active` - The Card Profile can be assigned to Cards.
+    - `archived` - The Card Profile is no longer in use.
+    """
 
     type: Literal["card_profile"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_profile`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/card_profile_create_params.py` & `increase-0.9.0/src/increase/types/card_profile_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/card_profile_list_params.py` & `increase-0.9.0/src/increase/types/card_profile_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/card_update_params.py` & `increase-0.9.0/src/increase/types/card_update_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,20 @@
     """
     The contact information used in the two-factor steps for digital wallet card
     creation. At least one field must be present to complete the digital wallet
     steps.
     """
 
     status: Literal["active", "disabled", "canceled"]
-    """The status to update the Card with."""
+    """The status to update the Card with.
+
+    - `active` - The card is active.
+    - `disabled` - The card is temporarily disabled.
+    - `canceled` - The card is permanently canceled.
+    """
 
 
 class BillingAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the billing address."""
 
     line1: Required[str]
```

### Comparing `increase-0.8.1/src/increase/types/check_deposit_create_params.py` & `increase-0.9.0/src/increase/types/check_deposit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/check_deposit_list_params.py` & `increase-0.9.0/src/increase/types/check_deposit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/check_transfer.py` & `increase-0.9.0/src/increase/types/check_transfer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,15 @@
 
 from typing import Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = [
-    "CheckTransfer",
-    "Approval",
-    "Cancellation",
-    "Deposit",
-    "ReturnAddress",
-    "ReturnDetails",
-    "StopPaymentRequest",
-    "Submission",
-]
+__all__ = ["CheckTransfer", "Approval", "Cancellation", "Deposit", "ReturnAddress", "StopPaymentRequest", "Submission"]
 
 
 class Approval(BaseModel):
     approved_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was approved.
@@ -58,14 +49,17 @@
 
     front_image_file_id: Optional[str]
     """
     The identifier of the API File object containing an image of the front of the
     deposited check.
     """
 
+    transaction_id: Optional[str]
+    """The identifier of the Transaction object created when the check was deposited."""
+
     type: Literal["check_transfer_deposit"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_deposit`.
     """
 
 
@@ -85,69 +79,50 @@
     state: Optional[str]
     """The US state of the address."""
 
     zip: Optional[str]
     """The postal code of the address."""
 
 
-class ReturnDetails(BaseModel):
-    file_id: Optional[str]
-    """If available, a document with additional information about the return."""
-
-    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
-    """The reason why the check was returned."""
-
-    returned_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the check was returned.
-    """
+class StopPaymentRequest(BaseModel):
+    reason: Literal["mail_delivery_failed", "unknown"]
+    """The reason why this transfer was stopped.
 
-    transaction_id: Optional[str]
-    """
-    The identifier of the Transaction that was created to credit you for the
-    returned check.
+    - `mail_delivery_failed` - The check could not be delivered.
+    - `unknown` - The check was stopped for another reason.
     """
 
-    transfer_id: str
-    """The identifier of the returned Check Transfer."""
-
-
-class StopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
-    transaction_id: str
-    """The transaction ID of the corresponding credit transaction."""
-
     transfer_id: str
     """The ID of the check transfer that was stopped."""
 
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
     """
 
 
 class Submission(BaseModel):
-    check_number: str
-    """The identitying number of the check."""
-
     submitted_at: datetime
     """When this check transfer was submitted to our check printer."""
 
 
 class CheckTransfer(BaseModel):
     id: str
     """The Check transfer's identifier."""
 
     account_id: str
     """The identifier of the Account from which funds will be transferred."""
 
+    account_number: str
+    """The account number printed on the check."""
+
     address_city: Optional[str]
     """The city of the check's destination."""
 
     address_line1: Optional[str]
     """The street address of the check's destination."""
 
     address_line2: Optional[str]
@@ -170,24 +145,34 @@
 
     cancellation: Optional[Cancellation]
     """
     If your account requires approvals for transfers and the transfer was not
     approved, this will contain details of the cancellation.
     """
 
+    check_number: str
+    """The check number printed on the check."""
+
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     deposit: Optional[Deposit]
     """After a check transfer is deposited, this will contain supplemental details."""
 
     mailed_at: Optional[datetime]
     """
@@ -197,58 +182,66 @@
 
     message: Optional[str]
     """The descriptor that will be printed on the memo field on the check."""
 
     note: Optional[str]
     """The descriptor that will be printed on the letter included with the check."""
 
+    pending_transaction_id: Optional[str]
+    """The identifier of the Pending Transaction associated with the check's creation."""
+
     recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     return_address: Optional[ReturnAddress]
     """The return address to be printed on the check."""
 
-    return_details: Optional[ReturnDetails]
-    """After a check transfer is returned, this will contain supplemental details.
+    routing_number: str
+    """The routing number printed on the check."""
 
-    A check transfer is returned when the receiver mails a never deposited check
-    back to the bank printed on the check.
+    source_account_number_id: Optional[str]
+    """
+    The identifier of the Account Number from which to send the transfer and print
+    on the check.
     """
 
     status: Literal[
         "pending_approval",
         "pending_submission",
         "submitted",
         "pending_mailing",
         "mailed",
         "canceled",
         "deposited",
         "stopped",
-        "returned",
         "rejected",
         "requires_attention",
     ]
-    """The lifecycle status of the transfer."""
+    """The lifecycle status of the transfer.
+
+    - `pending_approval` - The transfer is awaiting approval.
+    - `pending_submission` - The transfer is pending submission.
+    - `submitted` - The transfer is complete.
+    - `pending_mailing` - The check is queued for mailing.
+    - `mailed` - The check has been mailed.
+    - `canceled` - The transfer has been canceled.
+    - `deposited` - The check has been deposited.
+    - `stopped` - A stop-payment was requested for this check.
+    - `rejected` - The transfer has been rejected.
+    - `requires_attention` - The transfer requires attention from an Increase
+      operator.
+    """
 
     stop_payment_request: Optional[StopPaymentRequest]
     """
     After a stop-payment is requested on the check, this will contain supplemental
     details.
     """
 
     submission: Optional[Submission]
     """After the transfer is submitted, this will contain supplemental details."""
 
-    submitted_at: Optional[datetime]
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the check was submitted.
-    """
-
-    transaction_id: Optional[str]
-    """The ID for the transaction caused by the transfer."""
-
     type: Literal["check_transfer"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/check_transfer_create_params.py` & `increase-0.9.0/src/increase/types/check_transfer_create_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,14 +44,20 @@
     return_address: ReturnAddress
     """The return address to be printed on the check.
 
     If omitted this will default to the address of the Entity of the Account used to
     make the Check Transfer.
     """
 
+    source_account_number_id: str
+    """
+    The identifier of the Account Number from which to send the transfer and print
+    on the check.
+    """
+
 
 class ReturnAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the return address."""
 
     line1: Required[str]
     """The first line of the return address."""
```

### Comparing `increase-0.8.1/src/increase/types/check_transfer_list_params.py` & `increase-0.9.0/src/increase/types/entity_list_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 
 from typing import Union
 from datetime import datetime
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["CheckTransferListParams", "CreatedAt"]
+__all__ = ["EntityListParams", "CreatedAt"]
 
 
-class CheckTransferListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Check Transfers to those that originated from the specified Account."""
-
+class EntityListParams(TypedDict, total=False):
     created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
     limit: int
     """Limit the size of the list that is returned.
```

### Comparing `increase-0.8.1/src/increase/types/declined_transaction_list_params.py` & `increase-0.9.0/src/increase/types/declined_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/digital_wallet_token.py` & `increase-0.9.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # File generated from our OpenAPI spec by Stainless.
 
-from datetime import datetime
+from typing import Optional
 from typing_extensions import Literal
 
-from .._models import BaseModel
+from ..._models import BaseModel
 
-__all__ = ["DigitalWalletToken"]
+__all__ = ["DigitalWalletTokenRequestCreateResponse"]
 
 
-class DigitalWalletToken(BaseModel):
-    id: str
-    """The Digital Wallet Token identifier."""
+class DigitalWalletTokenRequestCreateResponse(BaseModel):
+    decline_reason: Optional[
+        Literal["card_not_active", "no_verification_method", "webhook_timed_out", "webhook_declined"]
+    ]
+    """
+    If the simulated tokenization attempt was declined, this field contains details
+    as to why.
 
-    card_id: str
-    """The identifier for the Card this Digital Wallet Token belongs to."""
+    - `card_not_active` - The card is not active.
+    - `no_verification_method` - The card does not have a two-factor authentication
+      method.
+    - `webhook_timed_out` - Your webhook timed out when evaluating the token
+      provisioning attempt.
+    - `webhook_declined` - Your webhook declined the token provisioning attempt.
+    """
 
-    created_at: datetime
+    digital_wallet_token_id: Optional[str]
     """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the Card was created.
+    If the simulated tokenization attempt was accepted, this field contains the id
+    of the Digital Wallet Token that was created.
     """
 
-    status: Literal["active", "inactive", "suspended", "deactivated"]
-    """This indicates if payments can be made with the Digital Wallet Token."""
-
-    token_requestor: Literal["apple_pay", "google_pay"]
-    """The digital wallet app being used."""
-
-    type: Literal["digital_wallet_token"]
+    type: Literal["inbound_digital_wallet_token_request_simulation_result"]
     """A constant representing the object's type.
 
-    For this resource it will always be `digital_wallet_token`.
+    For this resource it will always be
+    `inbound_digital_wallet_token_request_simulation_result`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/digital_wallet_token_list_params.py` & `increase-0.9.0/src/increase/types/digital_wallet_token_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/document.py` & `increase-0.9.0/src/increase/types/document.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,22 @@
 
 
 class Document(BaseModel):
     id: str
     """The Document identifier."""
 
     category: Literal["form_1099_int", "proof_of_authorization", "company_information"]
-    """The type of document."""
+    """The type of document.
+
+    - `form_1099_int` - Internal Revenue Service Form 1099-INT.
+    - `proof_of_authorization` - A document submitted in response to a proof of
+      authorization request for an ACH transfer.
+    - `company_information` - Company information, such a policies or procedures,
+      typically submitted during our due diligence process.
+    """
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the
     Document was created.
     """
```

### Comparing `increase-0.8.1/src/increase/types/document_list_params.py` & `increase-0.9.0/src/increase/types/document_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/entities/supplemental_document.py` & `increase-0.9.0/src/increase/types/entities/supplemental_document.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/entities/supplemental_document_list_params.py` & `increase-0.9.0/src/increase/types/entities/supplemental_document_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/entity.py` & `increase-0.9.0/src/increase/types/entity.py`

 * *Files 19% similar despite different names*

```diff
@@ -74,15 +74,23 @@
     """The ZIP code of the address."""
 
 
 class CorporationBeneficialOwnerIndividualIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
@@ -105,15 +113,21 @@
     company_title: Optional[str]
     """This person's role or title within the entity."""
 
     individual: CorporationBeneficialOwnerIndividual
     """Personal details for the beneficial owner."""
 
     prong: Literal["ownership", "control"]
-    """Why this person is considered a beneficial owner of the entity."""
+    """Why this person is considered a beneficial owner of the entity.
+
+    - `ownership` - A person with 25% or greater direct or indirect ownership of the
+      entity.
+    - `control` - A person who manages, directs, or has significant control of the
+      entity.
+    """
 
 
 class Corporation(BaseModel):
     address: CorporationAddress
     """The corporation's address."""
 
     beneficial_owners: List[CorporationBeneficialOwner]
@@ -158,15 +172,23 @@
     """The ZIP code of the address."""
 
 
 class JointIndividualIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
@@ -213,15 +235,23 @@
     """The ZIP code of the address."""
 
 
 class NaturalPersonIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
@@ -297,15 +327,23 @@
     """The ZIP code of the address."""
 
 
 class TrustGrantorIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
@@ -344,15 +382,23 @@
     """The ZIP code of the address."""
 
 
 class TrustTrusteeIndividualIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
@@ -375,23 +421,30 @@
     individual: Optional[TrustTrusteeIndividual]
     """The individual trustee of the trust.
 
     Will be present if the trustee's `structure` is equal to `individual`.
     """
 
     structure: Literal["individual"]
-    """The structure of the trustee. Will always be equal to `individual`."""
+    """The structure of the trustee. Will always be equal to `individual`.
+
+    - `individual` - The trustee is an individual.
+    """
 
 
 class Trust(BaseModel):
     address: TrustAddress
     """The trust's address."""
 
     category: Literal["revocable", "irrevocable"]
-    """Whether the trust is `revocable` or `irrevocable`."""
+    """Whether the trust is `revocable` or `irrevocable`.
+
+    - `revocable` - The trust is revocable by the grantor.
+    - `irrevocable` - The trust cannot be revoked.
+    """
 
     formation_document_file_id: Optional[str]
     """The ID for the File containing the formation document of the trust."""
 
     formation_state: Optional[str]
     """
     The two-letter United States Postal Service (USPS) abbreviation for the state in
@@ -433,18 +486,30 @@
     natural_person: Optional[NaturalPerson]
     """Details of the natural person entity.
 
     Will be present if `structure` is equal to `natural_person`.
     """
 
     relationship: Literal["affiliated", "informational", "unaffiliated"]
-    """The relationship between your group and the entity."""
+    """The relationship between your group and the entity.
+
+    - `affiliated` - The entity is controlled by your group.
+    - `informational` - The entity is for informational purposes only.
+    - `unaffiliated` - The entity is not controlled by your group, but can still
+      directly open accounts.
+    """
 
     structure: Literal["corporation", "natural_person", "joint", "trust"]
-    """The entity's legal structure."""
+    """The entity's legal structure.
+
+    - `corporation` - A corporation.
+    - `natural_person` - An individual person.
+    - `joint` - Multiple individual people.
+    - `trust` - A trust.
+    """
 
     supplemental_documents: List[SupplementalDocument]
     """Additional documentation associated with the entity.
 
     This is limited to the first 10 documents for an entity. If an entity has more
     than 10 documents, use the GET /entity_supplemental_documents list endpoint to
     retrieve them.
```

### Comparing `increase-0.8.1/src/increase/types/entity_create_params.py` & `increase-0.9.0/src/increase/types/entity_create_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,30 @@
     "TrustGrantorIdentificationOther",
     "TrustGrantorIdentificationPassport",
 ]
 
 
 class EntityCreateParams(TypedDict, total=False):
     relationship: Required[Literal["affiliated", "informational", "unaffiliated"]]
-    """The relationship between your group and the entity."""
+    """The relationship between your group and the entity.
+
+    - `affiliated` - The entity is controlled by your group.
+    - `informational` - The entity is for informational purposes only.
+    - `unaffiliated` - The entity is not controlled by your group, but can still
+      directly open accounts.
+    """
 
     structure: Required[Literal["corporation", "natural_person", "joint", "trust"]]
-    """The type of Entity to create."""
+    """The type of Entity to create.
+
+    - `corporation` - A corporation.
+    - `natural_person` - An individual person.
+    - `joint` - Multiple individual people.
+    - `trust` - A trust.
+    """
 
     corporation: Corporation
     """Details of the corporation entity to create.
 
     Required if `structure` is equal to `corporation`.
     """
 
@@ -176,15 +188,23 @@
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
             "other",
         ]
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number: Required[str]
     """
     An identification number that can be used to verify the individual's identity,
     such as a social security number.
     """
 
@@ -230,15 +250,21 @@
 
 
 class CorporationBeneficialOwner(TypedDict, total=False):
     individual: Required[CorporationBeneficialOwnerIndividual]
     """Personal details for the beneficial owner."""
 
     prong: Required[Literal["ownership", "control"]]
-    """Why this person is considered a beneficial owner of the entity."""
+    """Why this person is considered a beneficial owner of the entity.
+
+    - `ownership` - A person with 25% or greater direct or indirect ownership of the
+      entity.
+    - `control` - A person who manages, directs, or has significant control of the
+      entity.
+    """
 
     company_title: str
     """This person's role or title within the entity."""
 
 
 class Corporation(TypedDict, total=False):
     address: Required[CorporationAddress]
@@ -331,15 +357,23 @@
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
             "other",
         ]
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number: Required[str]
     """
     An identification number that can be used to verify the individual's identity,
     such as a social security number.
     """
 
@@ -457,15 +491,23 @@
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
             "other",
         ]
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number: Required[str]
     """
     An identification number that can be used to verify the individual's identity,
     such as a social security number.
     """
 
@@ -600,15 +642,23 @@
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
             "other",
         ]
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number: Required[str]
     """
     An identification number that can be used to verify the individual's identity,
     such as a social security number.
     """
 
@@ -651,15 +701,18 @@
     tax id (either a Social Security Number or Individual Taxpayer Identification
     Number).
     """
 
 
 class TrustTrustee(TypedDict, total=False):
     structure: Required[Literal["individual"]]
-    """The structure of the trustee."""
+    """The structure of the trustee.
+
+    - `individual` - The trustee is an individual.
+    """
 
     individual: TrustTrusteeIndividual
     """Details of the individual trustee.
 
     Required when the trustee `structure` is equal to `individual`.
     """
 
@@ -729,15 +782,23 @@
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
             "other",
         ]
     ]
-    """A method that can be used to verify the individual's identity."""
+    """A method that can be used to verify the individual's identity.
+
+    - `social_security_number` - A social security number.
+    - `individual_taxpayer_identification_number` - An individual taxpayer
+      identification number (ITIN).
+    - `passport` - A passport number.
+    - `drivers_license` - A driver's license number.
+    - `other` - Another identifying document.
+    """
 
     number: Required[str]
     """
     An identification number that can be used to verify the individual's identity,
     such as a social security number.
     """
 
@@ -787,14 +848,17 @@
     """The trust's address."""
 
     category: Required[Literal["revocable", "irrevocable"]]
     """Whether the trust is `revocable` or `irrevocable`.
 
     Irrevocable trusts require their own Employer Identification Number. Revocable
     trusts require information about the individual `grantor` who created the trust.
+
+    - `revocable` - The trust is revocable by the grantor.
+    - `irrevocable` - The trust cannot be revoked.
     """
 
     name: Required[str]
     """The legal name of the trust."""
 
     trustees: Required[List[TrustTrustee]]
     """The trustees of the trust."""
```

### Comparing `increase-0.8.1/src/increase/types/entity_list_params.py` & `increase-0.9.0/src/increase/types/account_number_list_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Union
 from datetime import datetime
-from typing_extensions import Annotated, TypedDict
+from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["EntityListParams", "CreatedAt"]
+__all__ = ["AccountNumberListParams", "CreatedAt"]
 
 
-class EntityListParams(TypedDict, total=False):
+class AccountNumberListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Account Numbers to those belonging to the specified Account."""
+
     created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
+    status: Literal["active", "disabled", "canceled"]
+    """The status to retrieve Account Numbers for.
+
+    - `active` - The account number is active.
+    - `disabled` - The account number is temporarily disabled.
+    - `canceled` - The account number is permanently disabled.
+    """
+
 
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
```

### Comparing `increase-0.8.1/src/increase/types/event_list_params.py` & `increase-0.9.0/src/increase/types/event_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/export.py` & `increase-0.9.0/src/increase/types/export.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     """The Export identifier."""
 
     category: Literal["transaction_csv", "balance_csv"]
     """The category of the Export.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle that gracefully.
+
+    - `transaction_csv` - Export a CSV of all transactions for a given time range.
+    - `balance_csv` - Export a CSV of account balances for the dates in a given
+      range.
     """
 
     created_at: datetime
     """The time the Export was created."""
 
     file_download_url: Optional[str]
     """A URL at which the Export's file can be downloaded.
@@ -32,14 +36,18 @@
     file_id: Optional[str]
     """The File containing the contents of the Export.
 
     This will be present when the Export's status transitions to `complete`.
     """
 
     status: Literal["pending", "complete"]
-    """The status of the Export."""
+    """The status of the Export.
+
+    - `pending` - Increase is generating the export.
+    - `complete` - The export has been successfully generated.
+    """
 
     type: Literal["export"]
     """A constant representing the object's type.
 
     For this resource it will always be `export`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/export_create_params.py` & `increase-0.9.0/src/increase/types/export_create_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 from .._utils import PropertyInfo
 
 __all__ = ["ExportCreateParams", "BalanceCsv", "BalanceCsvCreatedAt", "TransactionCsv", "TransactionCsvCreatedAt"]
 
 
 class ExportCreateParams(TypedDict, total=False):
     category: Required[Literal["transaction_csv", "balance_csv"]]
-    """The type of Export to create."""
+    """The type of Export to create.
+
+    - `transaction_csv` - Export a CSV of all transactions for a given time range.
+    - `balance_csv` - Export a CSV of account balances for the dates in a given
+      range.
+    """
 
     balance_csv: BalanceCsv
     """Options for the created export.
 
     Required if `category` is equal to `balance_csv`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/external_account.py` & `increase-0.9.0/src/increase/types/external_account.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,23 +21,38 @@
     the External Account was created.
     """
 
     description: str
     """The External Account's description for display purposes."""
 
     funding: Literal["checking", "savings", "other"]
-    """The type of the account to which the transfer will be sent."""
+    """The type of the account to which the transfer will be sent.
+
+    - `checking` - A checking account.
+    - `savings` - A savings account.
+    - `other` - A different type of account.
+    """
 
     routing_number: str
     """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     status: Literal["active", "archived"]
-    """The External Account's status."""
+    """The External Account's status.
+
+    - `active` - The External Acccount is active.
+    - `archived` - The External Account is archived and won't appear in the
+      dashboard.
+    """
 
     type: Literal["external_account"]
     """A constant representing the object's type.
 
     For this resource it will always be `external_account`.
     """
 
     verification_status: Literal["unverified", "pending", "verified"]
-    """If you have verified ownership of the External Account."""
+    """If you have verified ownership of the External Account.
+
+    - `unverified` - The External Account has not been verified.
+    - `pending` - The External Account is in the process of being verified.
+    - `verified` - The External Account is verified.
+    """
```

### Comparing `increase-0.8.1/src/increase/types/external_account_list_params.py` & `increase-0.9.0/src/increase/types/external_account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/file_list_params.py` & `increase-0.9.0/src/increase/types/file_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/inbound_wire_drawdown_request.py` & `increase-0.9.0/src/increase/types/inbound_wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/limit_create_params.py` & `increase-0.9.0/src/increase/types/routing_number_list_params.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing_extensions import Literal, Required, TypedDict
+from typing_extensions import Required, TypedDict
 
-__all__ = ["LimitCreateParams"]
+__all__ = ["RoutingNumberListParams"]
 
 
-class LimitCreateParams(TypedDict, total=False):
-    metric: Required[Literal["count", "volume"]]
-    """The metric for the limit."""
+class RoutingNumberListParams(TypedDict, total=False):
+    routing_number: Required[str]
+    """Filter financial institutions by routing number."""
 
-    model_id: Required[str]
-    """
-    The identifier of the Account or Account Number you wish to associate the limit
-    with.
-    """
+    cursor: str
+    """Return the page of entries after this one."""
 
-    value: Required[int]
-    """The value to test the limit against."""
+    limit: int
+    """Limit the size of the list that is returned.
 
-    interval: Literal["transaction", "day", "week", "month", "year", "all_time"]
-    """The interval for the metric. Required if `metric` is `count` or `volume`."""
+    The default (and maximum) is 100 objects.
+    """
```

### Comparing `increase-0.8.1/src/increase/types/limit_list_params.py` & `increase-0.9.0/src/increase/types/limit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/oauth_connection.py` & `increase-0.9.0/src/increase/types/oauth_connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     Connection was created.
     """
 
     group_id: str
     """The identifier of the Group that has authorized your OAuth application."""
 
     status: Literal["active", "inactive"]
-    """Whether the connection is active."""
+    """Whether the connection is active.
+
+    - `active` - The OAuth connection is active.
+    - `inactive` - The OAuth connection is permanently deactivated.
+    """
 
     type: Literal["oauth_connection"]
     """A constant representing the object's type.
 
     For this resource it will always be `oauth_connection`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/pending_transaction.py` & `increase-0.9.0/src/increase/types/pending_transaction.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,14 +30,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
     account currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     transfer_id: str
     """The identifier of the Account Transfer that led to this Pending Transaction."""
 
 
 class SourceACHTransferInstruction(BaseModel):
@@ -64,14 +71,44 @@
             "non_secure_transaction",
         ]
     ]
     """
     For electronic commerce transactions, this identifies the level of security used
     in obtaining the customer's payment credential. For mail or telephone order
     transactions, identifies the type of mail or telephone order.
+
+    - `mail_phone_order` - Single transaction of a mail/phone order: Use to indicate
+      that the transaction is a mail/phone order purchase, not a recurring
+      transaction or installment payment. For domestic transactions in the US
+      region, this value may also indicate one bill payment transaction in the
+      card-present or card-absent environments.
+    - `recurring` - Recurring transaction: Payment indicator used to indicate a
+      recurring transaction that originates from an acquirer in the US region.
+    - `installment` - Installment payment: Payment indicator used to indicate one
+      purchase of goods or services that is billed to the account in multiple
+      charges over a period of time agreed upon by the cardholder and merchant from
+      transactions that originate from an acquirer in the US region.
+    - `unknown_mail_phone_order` - Unknown classification: other mail order: Use to
+      indicate that the type of mail/telephone order is unknown.
+    - `secure_electronic_commerce` - Secure electronic commerce transaction: Use to
+      indicate that the electronic commerce transaction has been authenticated using
+      e.g., 3-D Secure
+    - `non_authenticated_security_transaction_at_3ds_capable_merchant` -
+      Non-authenticated security transaction at a 3-D Secure-capable merchant, and
+      merchant attempted to authenticate the cardholder using 3-D Secure: Use to
+      identify an electronic commerce transaction where the merchant attempted to
+      authenticate the cardholder using 3-D Secure, but was unable to complete the
+      authentication because the issuer or cardholder does not participate in the
+      3-D Secure program.
+    - `non_authenticated_security_transaction` - Non-authenticated security
+      transaction: Use to identify an electronic commerce transaction that uses data
+      encryption for security however , cardholder authentication is not performed
+      using 3-D Secure.
+    - `non_secure_transaction` - Non-secure transaction: Use to identify an
+      electronic commerce transaction that has no data protection.
     """
 
     point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
     """
     The method used to enter the cardholder's primary account number and card
     expiration date
     """
@@ -92,14 +129,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     digital_wallet_token_id: Optional[str]
     """
     If the authorization was made via a Digital Wallet Token (such as an Apple Pay
     purchase), the identifier of the token that was used.
     """
@@ -128,15 +172,18 @@
     merchant_country: Optional[str]
     """The country the merchant resides in."""
 
     merchant_descriptor: str
     """The merchant descriptor of the merchant the card is transacting with."""
 
     network: Literal["visa"]
-    """The payment network used to process this card authorization"""
+    """The payment network used to process this card authorization
+
+    - `visa` - Visa
+    """
 
     network_details: SourceCardAuthorizationNetworkDetails
     """Fields specific to the `network`"""
 
     pending_transaction_id: Optional[str]
     """The identifier of the Pending Transaction associated with this Transaction."""
 
@@ -169,14 +216,21 @@
     check_deposit_id: Optional[str]
     """The identifier of the Check Deposit."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     front_image_file_id: str
     """
     The identifier of the File containing the image of the front of the check that
     was deposited.
     """
@@ -189,14 +243,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     transfer_id: str
     """The identifier of the Check Transfer that led to this Pending Transaction."""
 
 
 class SourceInboundFundsHold(BaseModel):
@@ -218,27 +279,38 @@
     was created.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the hold's
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     held_transaction_id: Optional[str]
     """The ID of the Transaction for which funds were held."""
 
     pending_transaction_id: Optional[str]
     """The ID of the Pending Transaction representing the held funds."""
 
     released_at: Optional[datetime]
     """When the hold was released (if it has been released)."""
 
     status: Literal["held", "complete"]
-    """The status of the hold."""
+    """The status of the hold.
+
+    - `held` - Funds are still being held.
+    - `complete` - Funds have been released.
+    """
 
 
 class SourceRealTimePaymentsTransferInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -300,14 +372,39 @@
         "wire_transfer_instruction",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
+
+    - `account_transfer_instruction` - The Pending Transaction was created by a
+      Account Transfer Instruction object. Details will be under the
+      `account_transfer_instruction` object.
+    - `ach_transfer_instruction` - The Pending Transaction was created by a ACH
+      Transfer Instruction object. Details will be under the
+      `ach_transfer_instruction` object.
+    - `card_authorization` - The Pending Transaction was created by a Card
+      Authorization object. Details will be under the `card_authorization` object.
+    - `check_deposit_instruction` - The Pending Transaction was created by a Check
+      Deposit Instruction object. Details will be under the
+      `check_deposit_instruction` object.
+    - `check_transfer_instruction` - The Pending Transaction was created by a Check
+      Transfer Instruction object. Details will be under the
+      `check_transfer_instruction` object.
+    - `inbound_funds_hold` - The Pending Transaction was created by a Inbound Funds
+      Hold object. Details will be under the `inbound_funds_hold` object.
+    - `real_time_payments_transfer_instruction` - The Pending Transaction was
+      created by a Real Time Payments Transfer Instruction object. Details will be
+      under the `real_time_payments_transfer_instruction` object.
+    - `wire_transfer_instruction` - The Pending Transaction was created by a Wire
+      Transfer Instruction object. Details will be under the
+      `wire_transfer_instruction` object.
+    - `other` - The Pending Transaction was made for an undocumented or deprecated
+      reason.
     """
 
     check_deposit_instruction: Optional[SourceCheckDepositInstruction]
     """A Check Deposit Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_instruction`.
@@ -368,14 +465,21 @@
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Pending
     Transaction's currency. This will match the currency on the Pending
     Transcation's Account.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
     """
     For a Pending Transaction related to a transfer, this is the description you
     provide. For a Pending Transaction related to a payment, this is the description
     the vendor provides.
@@ -384,27 +488,36 @@
     route_id: Optional[str]
     """The identifier for the route this Pending Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Pending Transaction came through."""
+    """The type of the route this Pending Transaction came through.
+
+    - `account_number` - An Account Number.
+    - `card` - A Card.
+    """
 
     source: Source
     """
     This is an object giving more details on the network-level event that caused the
     Pending Transaction. For example, for a card transaction this lists the
     merchant's industry and location.
     """
 
     status: Literal["pending", "complete"]
     """
     Whether the Pending Transaction has been confirmed and has an associated
     Transaction.
+
+    - `pending` - The Pending Transaction is still awaiting confirmation.
+    - `complete` - The Pending Transaction is confirmed. An associated Transaction
+      exists for this object. The Pending Transaction will no longer count against
+      your balance and can generally be hidden from UIs, etc.
     """
 
     type: Literal["pending_transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `pending_transaction`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/pending_transaction_list_params.py` & `increase-0.9.0/src/increase/types/pending_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/program.py` & `increase-0.9.0/src/increase/types/program.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/real_time_decision_action_params.py` & `increase-0.9.0/src/increase/types/real_time_decision_action_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,30 @@
     If the Real-Time Decision relates to a digital wallet token provisioning
     attempt, this object contains your response to the attempt.
     """
 
 
 class CardAuthorization(TypedDict, total=False):
     decision: Required[Literal["approve", "decline"]]
-    """Whether the card authorization should be approved or declined."""
+    """Whether the card authorization should be approved or declined.
+
+    - `approve` - Approve the authorization.
+    - `decline` - Decline the authorization.
+    """
 
 
 class DigitalWalletAuthentication(TypedDict, total=False):
     result: Required[Literal["success", "failure"]]
-    """Whether your application was able to deliver the one-time passcode."""
+    """Whether your application was able to deliver the one-time passcode.
+
+    - `success` - Your application successfully delivered the one-time passcode to
+      the cardholder.
+    - `failure` - Your application failed to deliver the one-time passcode to the
+      cardholder.
+    """
 
 
 class DigitalWalletTokenApproval(TypedDict, total=False):
     card_profile_id: Required[str]
     """The identifier of the Card Profile to assign to the Digital Wallet token."""
 
     email: str
```

### Comparing `increase-0.8.1/src/increase/types/real_time_payments_transfer.py` & `increase-0.9.0/src/increase/types/wire_transfer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
-from datetime import datetime
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["RealTimePaymentsTransfer", "Approval", "Cancellation", "Rejection", "Submission"]
+__all__ = ["WireTransfer", "Approval", "Cancellation", "Reversal", "Submission"]
 
 
 class Approval(BaseModel):
     approved_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was approved.
@@ -33,140 +33,168 @@
     canceled_by: Optional[str]
     """
     If the Transfer was canceled by a user in the dashboard, the email address of
     that user.
     """
 
 
-class Rejection(BaseModel):
-    reject_reason_additional_information: Optional[str]
-    """
-    Additional information about the rejection provided by the recipient bank when
-    the `reject_reason_code` is `NARRATIVE`.
-    """
+class Reversal(BaseModel):
+    amount: int
+    """The amount that was reversed."""
 
-    reject_reason_code: Literal[
-        "account_closed",
-        "account_blocked",
-        "invalid_creditor_account_type",
-        "invalid_creditor_account_number",
-        "invalid_creditor_financial_institution_identifier",
-        "end_customer_deceased",
-        "narrative",
-        "transaction_forbidden",
-        "transaction_type_not_supported",
-        "unexpected_amount",
-        "amount_exceeds_bank_limits",
-        "invalid_creditor_address",
-        "unknown_end_customer",
-        "invalid_debtor_address",
-        "timeout",
-        "unsupported_message_for_recipient",
-        "recipient_connection_not_available",
-        "real_time_payments_suspended",
-        "instructed_agent_signed_off",
-        "processing_error",
-        "other",
-    ]
+    created_at: datetime
     """
-    The reason the transfer was rejected as provided by the recipient bank or the
-    Real Time Payments network.
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the reversal was created.
     """
 
-    rejected_at: Optional[datetime]
+    description: str
+    """The description on the reversal message from Fedwire."""
+
+    financial_institution_to_financial_institution_information: Optional[str]
+    """Additional financial institution information included in the wire reversal."""
+
+    input_cycle_date: date
+    """The Fedwire cycle date for the wire reversal."""
+
+    input_message_accountability_data: str
+    """The Fedwire transaction identifier."""
+
+    input_sequence_number: str
+    """The Fedwire sequence number."""
+
+    input_source: str
+    """The Fedwire input source identifier."""
+
+    previous_message_input_cycle_date: date
+    """The Fedwire cycle date for the wire transfer that was reversed."""
+
+    previous_message_input_message_accountability_data: str
+    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+
+    previous_message_input_sequence_number: str
+    """The Fedwire sequence number for the wire transfer that was reversed."""
+
+    previous_message_input_source: str
+    """The Fedwire input source identifier for the wire transfer that was reversed."""
+
+    receiver_financial_institution_information: Optional[str]
     """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the transfer was rejected.
+    Information included in the wire reversal for the receiving financial
+    institution.
     """
 
+    transaction_id: Optional[str]
+    """The ID for the Transaction associated with the transfer reversal."""
+
+    wire_transfer_id: str
+    """The ID for the Wire Transfer that is being reversed."""
+
 
 class Submission(BaseModel):
-    submitted_at: Optional[datetime]
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the transfer was submitted to The Clearing House.
-    """
+    input_message_accountability_data: str
+    """The accountability data for the submission."""
 
-    transaction_identification: str
-    """The Real Time Payments network identification of the transfer."""
+    submitted_at: datetime
+    """When this wire transfer was submitted to Fedwire."""
 
 
-class RealTimePaymentsTransfer(BaseModel):
+class WireTransfer(BaseModel):
     id: str
-    """The Real Time Payments Transfer's identifier."""
+    """The wire transfer's identifier."""
 
     account_id: str
-    """The Account from which the transfer was sent."""
+    """The Account to which the transfer belongs."""
+
+    account_number: str
+    """The destination account number."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     approval: Optional[Approval]
     """
     If your account requires approvals for transfers and the transfer was approved,
     this will contain details of the approval.
     """
 
+    beneficiary_address_line1: Optional[str]
+    """The beneficiary's address line 1."""
+
+    beneficiary_address_line2: Optional[str]
+    """The beneficiary's address line 2."""
+
+    beneficiary_address_line3: Optional[str]
+    """The beneficiary's address line 3."""
+
+    beneficiary_name: Optional[str]
+    """The beneficiary's name."""
+
     cancellation: Optional[Cancellation]
     """
     If your account requires approvals for transfers and the transfer was not
     approved, this will contain details of the cancellation.
     """
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
-    creditor_name: str
-    """The name of the transfer's recipient as provided by the sender."""
-
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transfer's
-    currency. For real time payments transfers this is always equal to `USD`.
-    """
-
-    destination_account_number: str
-    """The destination account number."""
+    currency. For wire transfers this is always equal to `usd`.
 
-    destination_routing_number: str
-    """
-    The destination American Bankers' Association (ABA) Routing Transit Number
-    (RTN).
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     external_account_id: Optional[str]
     """The identifier of the External Account the transfer was made to, if any."""
 
-    rejection: Optional[Rejection]
-    """
-    If the transfer is rejected by Real Time Payments or the destination financial
-    institution, this will contain supplemental details.
-    """
+    message_to_recipient: Optional[str]
+    """The message that will show on the recipient's bank statement."""
+
+    network: Literal["wire"]
+    """The transfer's network."""
 
-    remittance_information: str
-    """Unstructured information that will show on the recipient's bank statement."""
+    reversal: Optional[Reversal]
+    """If your transfer is reversed, this will contain details of the reversal."""
 
-    source_account_number_id: str
-    """The Account Number the recipient will see as having sent the transfer."""
+    routing_number: str
+    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     status: Literal[
-        "pending_approval", "canceled", "pending_submission", "submitted", "complete", "rejected", "requires_attention"
+        "canceled", "requires_attention", "pending_approval", "rejected", "reversed", "complete", "pending_creating"
     ]
-    """The lifecycle status of the transfer."""
+    """The lifecycle status of the transfer.
+
+    - `canceled` - The transfer has been canceled.
+    - `requires_attention` - The transfer requires attention from an Increase
+      operator.
+    - `pending_approval` - The transfer is pending approval.
+    - `rejected` - The transfer has been rejected.
+    - `reversed` - The transfer has been reversed.
+    - `complete` - The transfer is complete.
+    - `pending_creating` - The transfer is pending creation.
+    """
 
     submission: Optional[Submission]
     """
-    After the transfer is submitted to Real Time Payments, this will contain
-    supplemental details.
+    After the transfer is submitted to Fedwire, this will contain supplemental
+    details.
     """
 
     transaction_id: Optional[str]
-    """The Transaction funding the transfer once it is complete."""
+    """The ID for the transaction funding the transfer."""
 
-    type: Literal["real_time_payments_transfer"]
+    type: Literal["wire_transfer"]
     """A constant representing the object's type.
 
-    For this resource it will always be `real_time_payments_transfer`.
+    For this resource it will always be `wire_transfer`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/real_time_payments_transfer_create_params.py` & `increase-0.9.0/src/increase/types/real_time_payments_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/real_time_payments_transfer_list_params.py` & `increase-0.9.0/src/increase/types/real_time_payments_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/shared_params/point_of_service_entry_mode.py` & `increase-0.9.0/src/increase/types/shared_params/point_of_service_entry_mode.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/simulations/__init__.py` & `increase-0.9.0/src/increase/types/simulations/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 from .card_refund_create_params import CardRefundCreateParams as CardRefundCreateParams
 from .ach_transfer_return_params import (
     ACHTransferReturnParams as ACHTransferReturnParams,
 )
 from .card_dispute_action_params import (
     CardDisputeActionParams as CardDisputeActionParams,
 )
-from .check_transfer_return_params import (
-    CheckTransferReturnParams as CheckTransferReturnParams,
-)
 from .card_authorization_simulation import (
     CardAuthorizationSimulation as CardAuthorizationSimulation,
 )
 from .interest_payment_create_params import (
     InterestPaymentCreateParams as InterestPaymentCreateParams,
 )
 from .account_statement_create_params import (
```

### Comparing `increase-0.8.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py` & `increase-0.9.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/simulations/ach_transfer_simulation.py` & `increase-0.9.0/src/increase/types/simulations/interest_payment_simulation_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
 from datetime import date, datetime
 from typing_extensions import Literal
 
-from ...types import shared
 from ..._models import BaseModel
 
 __all__ = [
-    "ACHTransferSimulation",
-    "DeclinedTransaction",
-    "DeclinedTransactionSource",
-    "DeclinedTransactionSourceACHDecline",
-    "DeclinedTransactionSourceCardDecline",
-    "DeclinedTransactionSourceCardDeclineNetworkDetails",
-    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
-    "DeclinedTransactionSourceCheckDecline",
-    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
-    "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceWireDecline",
+    "InterestPaymentSimulationResult",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
@@ -30,15 +19,14 @@
     "TransactionSourceCardRevenuePayment",
     "TransactionSourceCardSettlement",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferDeposit",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferRejection",
-    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPayment",
@@ -50,480 +38,32 @@
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
 ]
 
 
-class DeclinedTransactionSourceACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    originator_company_descriptive_date: Optional[str]
-
-    originator_company_discretionary_data: Optional[str]
-
-    originator_company_id: str
-
-    originator_company_name: str
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "credit_entry_refused_by_receiver",
-        "duplicate_return",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "misrouted_return",
-        "no_ach_route",
-        "originator_request",
-        "transaction_not_allowed",
-    ]
-    """Why the ACH transfer was declined."""
-
-    receiver_id_number: Optional[str]
-
-    receiver_name: Optional[str]
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
-    electronic_commerce_indicator: Optional[
-        Literal[
-            "mail_phone_order",
-            "recurring",
-            "installment",
-            "unknown_mail_phone_order",
-            "secure_electronic_commerce",
-            "non_authenticated_security_transaction_at_3ds_capable_merchant",
-            "non_authenticated_security_transaction",
-            "non_secure_transaction",
-        ]
-    ]
-    """
-    For electronic commerce transactions, this identifies the level of security used
-    in obtaining the customer's payment credential. For mail or telephone order
-    transactions, identifies the type of mail or telephone order.
-    """
-
-    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
-    """
-    The method used to enter the cardholder's primary account number and card
-    expiration date
-    """
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
-    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
-    """Fields specific to the `visa` network"""
-
-
-class DeclinedTransactionSourceCardDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    digital_wallet_token_id: Optional[str]
-    """
-    If the authorization was attempted using a Digital Wallet Token (such as an
-    Apple Pay purchase), the identifier of the token that was used.
-    """
-
-    merchant_acceptor_id: str
-    """
-    The merchant identifier (commonly abbreviated as MID) of the merchant the card
-    is transacting with.
-    """
-
-    merchant_category_code: Optional[str]
-    """
-    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
-    card is transacting with.
-    """
-
-    merchant_city: Optional[str]
-    """The city the merchant resides in."""
-
-    merchant_country: Optional[str]
-    """The country the merchant resides in."""
-
-    merchant_descriptor: str
-    """The merchant descriptor of the merchant the card is transacting with."""
-
-    merchant_state: Optional[str]
-    """The state the merchant resides in."""
-
-    network: Literal["visa"]
-    """The payment network used to process this card authorization"""
-
-    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
-    """Fields specific to the `network`"""
-
-    real_time_decision_id: Optional[str]
-    """
-    The identifier of the Real-Time Decision sent to approve or decline this
-    transaction.
-    """
-
-    reason: Literal[
-        "card_not_active",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "cvv2_mismatch",
-        "transaction_not_allowed",
-        "breaches_internal_limit",
-        "breaches_limit",
-        "webhook_declined",
-        "webhook_timed_out",
-        "declined_by_stand_in_processing",
-        "invalid_physical_card",
-        "missing_original_authorization",
-    ]
-    """Why the transaction was declined."""
-
-
-class DeclinedTransactionSourceCheckDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    auxiliary_on_us: Optional[str]
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "unable_to_locate_account",
-        "not_our_item",
-        "unable_to_process",
-        "refer_to_image",
-        "stop_payment_requested",
-        "returned",
-        "duplicate_presentment",
-        "not_authorized",
-        "altered_or_fictitious",
-    ]
-    """Why the check was declined."""
-
-
-class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    creditor_name: str
-    """The name the sender of the transfer specified as the recipient of the transfer."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
-    transfer's currency. This will always be "USD" for a Real Time Payments
-    transfer.
-    """
-
-    debtor_account_number: str
-    """The account number of the account that sent the transfer."""
-
-    debtor_name: str
-    """The name provided by the sender of the transfer."""
-
-    debtor_routing_number: str
-    """The routing number of the account that sent the transfer."""
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "account_restricted",
-        "group_locked",
-        "entity_not_active",
-        "real_time_payments_not_enabled",
-    ]
-    """Why the transfer was declined."""
-
-    remittance_information: Optional[str]
-    """Additional information included with the transfer."""
-
-    transaction_identification: str
-    """The Real Time Payments network identification of the declined transfer."""
-
-
-class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    destination_country_code: str
-
-    destination_currency_code: str
-
-    foreign_exchange_indicator: str
-
-    foreign_exchange_reference: Optional[str]
-
-    foreign_exchange_reference_indicator: str
-
-    foreign_payment_amount: int
-
-    foreign_trace_number: Optional[str]
-
-    international_transaction_type_code: str
-
-    originating_currency_code: str
-
-    originating_depository_financial_institution_branch_country: str
-
-    originating_depository_financial_institution_id: str
-
-    originating_depository_financial_institution_id_qualifier: str
-
-    originating_depository_financial_institution_name: str
-
-    originator_city: str
-
-    originator_company_entry_description: str
-
-    originator_country: str
-
-    originator_identification: str
-
-    originator_name: str
-
-    originator_postal_code: Optional[str]
-
-    originator_state_or_province: Optional[str]
-
-    originator_street_address: str
-
-    payment_related_information: Optional[str]
-
-    payment_related_information2: Optional[str]
-
-    receiver_city: str
-
-    receiver_country: str
-
-    receiver_identification_number: Optional[str]
-
-    receiver_postal_code: Optional[str]
-
-    receiver_state_or_province: Optional[str]
-
-    receiver_street_address: str
-
-    receiving_company_or_individual_name: str
-
-    receiving_depository_financial_institution_country: str
-
-    receiving_depository_financial_institution_id: str
-
-    receiving_depository_financial_institution_id_qualifier: str
-
-    receiving_depository_financial_institution_name: str
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceWireDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    beneficiary_address_line1: Optional[str]
-
-    beneficiary_address_line2: Optional[str]
-
-    beneficiary_address_line3: Optional[str]
-
-    beneficiary_name: Optional[str]
-
-    beneficiary_reference: Optional[str]
-
-    description: str
-
-    input_message_accountability_data: Optional[str]
-
-    originator_address_line1: Optional[str]
-
-    originator_address_line2: Optional[str]
-
-    originator_address_line3: Optional[str]
-
-    originator_name: Optional[str]
-
-    originator_to_beneficiary_information_line1: Optional[str]
-
-    originator_to_beneficiary_information_line2: Optional[str]
-
-    originator_to_beneficiary_information_line3: Optional[str]
-
-    originator_to_beneficiary_information_line4: Optional[str]
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "entity_not_active",
-        "group_locked",
-        "no_account_number",
-        "transaction_not_allowed",
-    ]
-    """Why the wire transfer was declined."""
-
-
-class DeclinedTransactionSource(BaseModel):
-    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
-    """A ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_decline`.
-    """
-
-    card_decline: Optional[DeclinedTransactionSourceCardDecline]
-    """A Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_decline`.
-    """
-
-    category: Literal[
-        "ach_decline",
-        "card_decline",
-        "check_decline",
-        "inbound_real_time_payments_transfer_decline",
-        "international_ach_decline",
-        "wire_decline",
-        "other",
-    ]
-    """The type of decline that took place.
-
-    We may add additional possible values for this enum over time; your application
-    should be able to handle such additions gracefully.
-    """
-
-    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
-    """A Check Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_decline`.
-    """
-
-    inbound_real_time_payments_transfer_decline: Optional[
-        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
-    ]
-    """A Inbound Real Time Payments Transfer Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_real_time_payments_transfer_decline`.
-    """
-
-    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
-    """A International ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `international_ach_decline`.
-    """
-
-    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
-    """A Wire Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_decline`.
-    """
-
-
-class DeclinedTransaction(BaseModel):
-    id: str
-    """The Declined Transaction identifier."""
-
-    account_id: str
-    """The identifier for the Account the Declined Transaction belongs to."""
-
-    amount: int
-    """The Declined Transaction amount in the minor unit of its currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
-    Transaction occured.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
-    Transaction's currency. This will match the currency on the Declined
-    Transcation's Account.
-    """
-
-    description: str
-    """This is the description the vendor provides."""
-
-    route_id: Optional[str]
-    """The identifier for the route this Declined Transaction came through.
-
-    Routes are things like cards and ACH details.
-    """
-
-    route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Declined Transaction came through."""
-
-    source: DeclinedTransactionSource
-    """
-    This is an object giving more details on the network-level event that caused the
-    Declined Transaction. For example, for a card transaction this lists the
-    merchant's industry and location. Note that for backwards compatibility reasons,
-    additional undocumented keys may appear in this object. These should be treated
-    as deprecated and will be removed in the future.
-    """
-
-    type: Literal["declined_transaction"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `declined_transaction`.
-    """
-
-
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
     account currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
     """The description you chose to give the transfer."""
 
     destination_account_id: str
     """The identifier of the Account to where the Account Transfer was sent."""
@@ -635,15 +175,161 @@
         "stop_payment_on_item_related_to_rck_entry",
         "stop_payment_on_source_document",
         "timely_original_return",
         "trace_number_error",
         "untimely_dishonored_return",
         "untimely_return",
     ]
-    """Why the ACH Transfer was returned."""
+    """Why the ACH Transfer was returned.
+
+    - `insufficient_fund` - Code R01. Insufficient funds in the source account.
+    - `no_account` - Code R03. The account does not exist or the receiving bank was
+      unable to locate it.
+    - `account_closed` - Code R02. The account is closed.
+    - `invalid_account_number_structure` - Code R04. The account number is invalid
+      at the receiving bank.
+    - `account_frozen_entry_returned_per_ofac_instruction` - Code R16. The account
+      was frozen per the Office of Foreign Assets Control.
+    - `credit_entry_refused_by_receiver` - Code R23. The receiving bank account
+      refused a credit transfer.
+    - `unauthorized_debit_to_consumer_account_using_corporate_sec_code` - Code R05.
+      The receiving bank rejected because of an incorrect Standard Entry Class code.
+    - `corporate_customer_advised_not_authorized` - Code R29. The corporate customer
+      reversed the transfer.
+    - `payment_stopped` - Code R08. The receiving bank stopped payment on this
+      transfer.
+    - `non_transaction_account` - Code R20. The receiving bank account does not
+      perform transfers.
+    - `uncollected_funds` - Code R09. The receiving bank account does not have
+      enough available balance for the transfer.
+    - `routing_number_check_digit_error` - Code R28. The routing number is
+      incorrect.
+    - `customer_advised_unauthorized_improper_ineligible_or_incomplete` - Code R10.
+      The customer reversed the transfer.
+    - `amount_field_error` - Code R19. The amount field is incorrect or too large.
+    - `authorization_revoked_by_customer` - Code R07. The customer who initiated the
+      transfer revoked authorization.
+    - `invalid_ach_routing_number` - Code R13. The routing number is invalid.
+    - `file_record_edit_criteria` - Code R17. The receiving bank is unable to
+      process a field in the transfer.
+    - `enr_invalid_individual_name` - Code R45. The individual name field was
+      invalid.
+    - `returned_per_odfi_request` - Code R06. The originating financial institution
+      reversed the transfer.
+    - `limited_participation_dfi` - Code R34. The receiving bank's regulatory
+      supervisor has limited their participation.
+    - `incorrectly_coded_outbound_international_payment` - Code R85. The outbound
+      international ACH transfer was incorrect.
+    - `account_sold_to_another_dfi` - Code R12. A rare return reason. The account
+      was sold to another bank.
+    - `addenda_error` - Code R25. The addenda record is incorrect or missing.
+    - `beneficiary_or_account_holder_deceased` - Code R15. A rare return reason. The
+      account holder is deceased.
+    - `customer_advised_not_within_authorization_terms` - Code R11. A rare return
+      reason. The customer authorized some payment to the sender, but this payment
+      was not in error.
+    - `corrected_return` - Code R74. A rare return reason. Sent in response to a
+      return that was returned with code `field_error`. The latest return should
+      include the corrected field(s).
+    - `duplicate_entry` - Code R24. A rare return reason. The receiving bank
+      received an exact duplicate entry with the same trace number and amount.
+    - `duplicate_return` - Code R67. A rare return reason. The return this message
+      refers to was a duplicate.
+    - `enr_duplicate_enrollment` - Code R47. A rare return reason. Only used for US
+      Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_dfi_account_number` - Code R43. A rare return reason. Only used
+      for US Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_individual_id_number` - Code R44. A rare return reason. Only used
+      for US Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_representative_payee_indicator` - Code R46. A rare return reason.
+      Only used for US Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_transaction_code` - Code R41. A rare return reason. Only used for
+      US Government agency non-monetary automatic enrollment messages.
+    - `enr_return_of_enr_entry` - Code R40. A rare return reason. Only used for US
+      Government agency non-monetary automatic enrollment messages.
+    - `enr_routing_number_check_digit_error` - Code R42. A rare return reason. Only
+      used for US Government agency non-monetary automatic enrollment messages.
+    - `entry_not_processed_by_gateway` - Code R84. A rare return reason. The
+      International ACH Transfer cannot be processed by the gateway.
+    - `field_error` - Code R69. A rare return reason. One or more of the fields in
+      the ACH were malformed.
+    - `foreign_receiving_dfi_unable_to_settle` - Code R83. A rare return reason. The
+      Foreign receiving bank was unable to settle this ACH transfer.
+    - `iat_entry_coding_error` - Code R80. A rare return reason. The International
+      ACH Transfer is malformed.
+    - `improper_effective_entry_date` - Code R18. A rare return reason. The ACH has
+      an improper effective entry date field.
+    - `improper_source_document_source_document_presented` - Code R39. A rare return
+      reason. The source document related to this ACH, usually an ACH check
+      conversion, was presented to the bank.
+    - `invalid_company_id` - Code R21. A rare return reason. The Company ID field of
+      the ACH was invalid.
+    - `invalid_foreign_receiving_dfi_identification` - Code R82. A rare return
+      reason. The foreign receiving bank identifier for an International ACH
+      Transfer was invalid.
+    - `invalid_individual_id_number` - Code R22. A rare return reason. The
+      Individual ID number field of the ACH was invalid.
+    - `item_and_rck_entry_presented_for_payment` - Code R53. A rare return reason.
+      Both the Represented Check ("RCK") entry and the original check were presented
+      to the bank.
+    - `item_related_to_rck_entry_is_ineligible` - Code R51. A rare return reason.
+      The Represented Check ("RCK") entry is ineligible.
+    - `mandatory_field_error` - Code R26. A rare return reason. The ACH is missing a
+      required field.
+    - `misrouted_dishonored_return` - Code R71. A rare return reason. The receiving
+      bank does not recognize the routing number in a dishonored return entry.
+    - `misrouted_return` - Code R61. A rare return reason. The receiving bank does
+      not recognize the routing number in a return entry.
+    - `no_errors_found` - Code R76. A rare return reason. Sent in response to a
+      return, the bank does not find the errors alleged by the returning bank.
+    - `non_acceptance_of_r62_dishonored_return` - Code R77. A rare return reason.
+      The receiving bank does not accept the return of the erroneous debit. The
+      funds are not available at the receiving bank.
+    - `non_participant_in_iat_program` - Code R81. A rare return reason. The
+      receiving bank does not accept International ACH Transfers.
+    - `permissible_return_entry` - Code R31. A rare return reason. A return that has
+      been agreed to be accepted by the receiving bank, despite falling outside of
+      the usual return timeframe.
+    - `permissible_return_entry_not_accepted` - Code R70. A rare return reason. The
+      receiving bank had not approved this return.
+    - `rdfi_non_settlement` - Code R32. A rare return reason. The receiving bank
+      could not settle this transaction.
+    - `rdfi_participant_in_check_truncation_program` - Code R30. A rare return
+      reason. The receiving bank does not accept Check Truncation ACH transfers.
+    - `representative_payee_deceased_or_unable_to_continue_in_that_capacity` - Code
+      R14. A rare return reason. The payee is deceased.
+    - `return_not_a_duplicate` - Code R75. A rare return reason. The originating
+      bank disputes that an earlier `duplicate_entry` return was actually a
+      duplicate.
+    - `return_of_erroneous_or_reversing_debit` - Code R62. A rare return reason. The
+      originating bank made a mistake earlier and this return corrects it.
+    - `return_of_improper_credit_entry` - Code R36. A rare return reason. Return of
+      a malformed credit entry.
+    - `return_of_improper_debit_entry` - Code R35. A rare return reason. Return of a
+      malformed debit entry.
+    - `return_of_xck_entry` - Code R33. A rare return reason. Return of a Destroyed
+      Check ("XKC") entry.
+    - `source_document_presented_for_payment` - Code R37. A rare return reason. The
+      source document related to this ACH, usually an ACH check conversion, was
+      presented to the bank.
+    - `state_law_affecting_rck_acceptance` - Code R50. A rare return reason. State
+      law prevents the bank from accepting the Represented Check ("RCK") entry.
+    - `stop_payment_on_item_related_to_rck_entry` - Code R52. A rare return reason.
+      A stop payment was issued on a Represented Check ("RCK") entry.
+    - `stop_payment_on_source_document` - Code R38. A rare return reason. The source
+      attached to the ACH, usually an ACH check conversion, includes a stop payment.
+    - `timely_original_return` - Code R73. A rare return reason. The bank receiving
+      an `untimely_return` believes it was on time.
+    - `trace_number_error` - Code R27. A rare return reason. An ACH Return's trace
+      number does not match an originated ACH.
+    - `untimely_dishonored_return` - Code R72. A rare return reason. The dishonored
+      return was sent too late.
+    - `untimely_return` - Code R68. A rare return reason. The return was sent too
+      late.
+    """
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
     """The identifier of the ACH Transfer associated with this return."""
 
@@ -675,14 +361,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
@@ -698,14 +391,17 @@
 
     merchant_name: Optional[str]
     """The name of the merchant."""
 
     merchant_state: Optional[str]
     """The state the merchant resides in."""
 
+    transaction_id: str
+    """The identifier of the Transaction associated with this Transaction."""
+
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
@@ -716,14 +412,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     period_end: datetime
     """The end of the period for which this transaction paid interest."""
 
     period_start: datetime
     """The start of the period for which this transaction paid interest."""
@@ -748,14 +451,21 @@
     exists.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
@@ -783,14 +493,17 @@
 
     presentment_currency: str
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's presentment currency.
     """
 
+    transaction_id: str
+    """The identifier of the Transaction associated with this Transaction."""
+
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
@@ -813,14 +526,21 @@
     check_deposit_id: str
     """The ID of the Check Deposit that was accepted."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     routing_number: str
     """The routing number printed on the check."""
 
     serial_number: Optional[str]
     """The check serial number, if present, for consumer checks.
@@ -840,14 +560,21 @@
     check_deposit_id: str
     """The identifier of the Check Deposit that was returned."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     return_reason: Literal[
         "ach_conversion_not_supported",
         "closed_account",
         "duplicate_submission",
         "insufficient_funds",
@@ -856,14 +583,28 @@
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
         "endorsement_irregular",
     ]
+    """
+    - `ach_conversion_not_supported` - The check doesn't allow ACH conversion.
+    - `closed_account` - The account is closed.
+    - `duplicate_submission` - The check has already been deposited.
+    - `insufficient_funds` - Insufficient funds
+    - `no_account` - No account was found matching the check details.
+    - `not_authorized` - The check was not authorized.
+    - `stale_dated` - The check is too old.
+    - `stop_payment` - The payment has been stopped by the account holder.
+    - `unknown_reason` - The reason for the return is unknown.
+    - `unmatched_details` - The image doesn't match the details submitted.
+    - `unreadable_image` - The image could not be read.
+    - `endorsement_irregular` - The check endorsement was irregular.
+    """
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
 
@@ -886,14 +627,17 @@
 
     front_image_file_id: Optional[str]
     """
     The identifier of the API File object containing an image of the front of the
     deposited check.
     """
 
+    transaction_id: Optional[str]
+    """The identifier of the Transaction object created when the check was deposited."""
+
     type: Literal["check_transfer_deposit"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_deposit`.
     """
 
 
@@ -916,58 +660,46 @@
     amount: int
     """The transfer amount in USD cents."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     transfer_id: str
     """The identifier of the Check Transfer with which this is associated."""
 
 
 class TransactionSourceCheckTransferRejection(BaseModel):
     transfer_id: str
     """The identifier of the Check Transfer that led to this Transaction."""
 
 
-class TransactionSourceCheckTransferReturn(BaseModel):
-    file_id: Optional[str]
-    """If available, a document with additional information about the return."""
-
-    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
-    """The reason why the check was returned."""
-
-    returned_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the check was returned.
-    """
+class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
+    reason: Literal["mail_delivery_failed", "unknown"]
+    """The reason why this transfer was stopped.
 
-    transaction_id: Optional[str]
-    """
-    The identifier of the Transaction that was created to credit you for the
-    returned check.
+    - `mail_delivery_failed` - The check could not be delivered.
+    - `unknown` - The check was stopped for another reason.
     """
 
-    transfer_id: str
-    """The identifier of the returned Check Transfer."""
-
-
-class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
-    transaction_id: str
-    """The transaction ID of the corresponding credit transaction."""
-
     transfer_id: str
     """The ID of the check transfer that was stopped."""
 
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
@@ -981,14 +713,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
 
 class TransactionSourceInboundACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
@@ -1025,14 +764,21 @@
 
     check_rear_image_file_id: Optional[str]
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
 
 class TransactionSourceInboundInternationalACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
@@ -1120,14 +866,21 @@
     creditor_name: str
     """The name the sender of the transfer specified as the recipient of the transfer."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the transfer's
     currency. This will always be "USD" for a Real Time Payments transfer.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     debtor_account_number: str
     """The account number of the account that sent the transfer."""
 
     debtor_name: str
     """The name provided by the sender of the transfer."""
@@ -1309,14 +1062,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     period_end: datetime
     """The end of the period for which this transaction paid interest."""
 
     period_start: datetime
     """The start of the period for which this transaction paid interest."""
@@ -1329,14 +1089,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     reason: Literal[
         "account_closure",
         "bank_migration",
         "cashback",
         "collection_receivable",
@@ -1345,14 +1112,28 @@
         "error_correction",
         "fees",
         "interest",
         "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
+    """
+    - `account_closure` - Account closure
+    - `bank_migration` - Bank migration
+    - `cashback` - Cashback
+    - `collection_receivable` - Collection receivable
+    - `empyreal_adjustment` - Empyreal adjustment
+    - `error` - Error
+    - `error_correction` - Error correction
+    - `fees` - Fees
+    - `interest` - Interest
+    - `negative_balance_forgiveness` - Negative balance forgiveness
+    - `sample_funds` - Sample funds
+    - `sample_funds_return` - Sample funds return
+    """
 
 
 class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
     amount: int
     """The transfer amount in USD cents."""
 
     destination_account_number: str
@@ -1460,15 +1241,14 @@
         "card_revenue_payment",
         "card_settlement",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_deposit",
         "check_transfer_intention",
         "check_transfer_rejection",
-        "check_transfer_return",
         "check_transfer_stop_payment_request",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
@@ -1484,14 +1264,85 @@
         "wire_transfer_rejection",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
+
+    - `account_transfer_intention` - The Transaction was created by a Account
+      Transfer Intention object. Details will be under the
+      `account_transfer_intention` object.
+    - `ach_transfer_intention` - The Transaction was created by a ACH Transfer
+      Intention object. Details will be under the `ach_transfer_intention` object.
+    - `ach_transfer_rejection` - The Transaction was created by a ACH Transfer
+      Rejection object. Details will be under the `ach_transfer_rejection` object.
+    - `ach_transfer_return` - The Transaction was created by a ACH Transfer Return
+      object. Details will be under the `ach_transfer_return` object.
+    - `card_dispute_acceptance` - The Transaction was created by a Card Dispute
+      Acceptance object. Details will be under the `card_dispute_acceptance` object.
+    - `card_refund` - The Transaction was created by a Card Refund object. Details
+      will be under the `card_refund` object.
+    - `card_revenue_payment` - The Transaction was created by a Card Revenue Payment
+      object. Details will be under the `card_revenue_payment` object.
+    - `card_settlement` - The Transaction was created by a Card Settlement object.
+      Details will be under the `card_settlement` object.
+    - `check_deposit_acceptance` - The Transaction was created by a Check Deposit
+      Acceptance object. Details will be under the `check_deposit_acceptance`
+      object.
+    - `check_deposit_return` - The Transaction was created by a Check Deposit Return
+      object. Details will be under the `check_deposit_return` object.
+    - `check_transfer_deposit` - The Transaction was created by a Check Transfer
+      Deposit object. Details will be under the `check_transfer_deposit` object.
+    - `check_transfer_intention` - The Transaction was created by a Check Transfer
+      Intention object. Details will be under the `check_transfer_intention` object.
+    - `check_transfer_rejection` - The Transaction was created by a Check Transfer
+      Rejection object. Details will be under the `check_transfer_rejection` object.
+    - `check_transfer_stop_payment_request` - The Transaction was created by a Check
+      Transfer Stop Payment Request object. Details will be under the
+      `check_transfer_stop_payment_request` object.
+    - `fee_payment` - The Transaction was created by a Fee Payment object. Details
+      will be under the `fee_payment` object.
+    - `inbound_ach_transfer` - The Transaction was created by a Inbound ACH Transfer
+      object. Details will be under the `inbound_ach_transfer` object.
+    - `inbound_ach_transfer_return_intention` - The Transaction was created by a
+      Inbound ACH Transfer Return Intention object. Details will be under the
+      `inbound_ach_transfer_return_intention` object.
+    - `inbound_check` - The Transaction was created by a Inbound Check object.
+      Details will be under the `inbound_check` object.
+    - `inbound_international_ach_transfer` - The Transaction was created by a
+      Inbound International ACH Transfer object. Details will be under the
+      `inbound_international_ach_transfer` object.
+    - `inbound_real_time_payments_transfer_confirmation` - The Transaction was
+      created by a Inbound Real Time Payments Transfer Confirmation object. Details
+      will be under the `inbound_real_time_payments_transfer_confirmation` object.
+    - `inbound_wire_drawdown_payment` - The Transaction was created by a Inbound
+      Wire Drawdown Payment object. Details will be under the
+      `inbound_wire_drawdown_payment` object.
+    - `inbound_wire_drawdown_payment_reversal` - The Transaction was created by a
+      Inbound Wire Drawdown Payment Reversal object. Details will be under the
+      `inbound_wire_drawdown_payment_reversal` object.
+    - `inbound_wire_reversal` - The Transaction was created by a Inbound Wire
+      Reversal object. Details will be under the `inbound_wire_reversal` object.
+    - `inbound_wire_transfer` - The Transaction was created by a Inbound Wire
+      Transfer object. Details will be under the `inbound_wire_transfer` object.
+    - `interest_payment` - The Transaction was created by a Interest Payment object.
+      Details will be under the `interest_payment` object.
+    - `internal_source` - The Transaction was created by a Internal Source object.
+      Details will be under the `internal_source` object.
+    - `real_time_payments_transfer_acknowledgement` - The Transaction was created by
+      a Real Time Payments Transfer Acknowledgement object. Details will be under
+      the `real_time_payments_transfer_acknowledgement` object.
+    - `sample_funds` - The Transaction was created by a Sample Funds object. Details
+      will be under the `sample_funds` object.
+    - `wire_transfer_intention` - The Transaction was created by a Wire Transfer
+      Intention object. Details will be under the `wire_transfer_intention` object.
+    - `wire_transfer_rejection` - The Transaction was created by a Wire Transfer
+      Rejection object. Details will be under the `wire_transfer_rejection` object.
+    - `other` - The Transaction was made for an undocumented or deprecated reason.
     """
 
     check_deposit_acceptance: Optional[TransactionSourceCheckDepositAcceptance]
     """A Check Deposit Acceptance object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_acceptance`.
@@ -1521,21 +1372,14 @@
     check_transfer_rejection: Optional[TransactionSourceCheckTransferRejection]
     """A Check Transfer Rejection object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_rejection`.
     """
 
-    check_transfer_return: Optional[TransactionSourceCheckTransferReturn]
-    """A Check Transfer Return object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_return`.
-    """
-
     check_transfer_stop_payment_request: Optional[TransactionSourceCheckTransferStopPaymentRequest]
     """A Check Transfer Stop Payment Request object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_stop_payment_request`.
     """
 
@@ -1667,31 +1511,42 @@
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     Transaction's currency. This will match the currency on the Transcation's
     Account.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
-    """For a Transaction related to a transfer, this is the description you provide.
+    """An informational message describing this transaction.
 
-    For a Transaction related to a payment, this is the description the vendor
-    provides.
+    Use the fields in `source` to get more detailed information. This field appears
+    as the line-item on the statement.
     """
 
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Transaction came through."""
+    """The type of the route this Transaction came through.
+
+    - `account_number` - An Account Number.
+    - `card` - A Card.
+    """
 
     source: TransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Transaction. Note that for backwards compatibility reasons, additional
     undocumented keys may appear in this object. These should be treated as
     deprecated and will be removed in the future.
@@ -1700,27 +1555,19 @@
     type: Literal["transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `transaction`.
     """
 
 
-class ACHTransferSimulation(BaseModel):
-    declined_transaction: Optional[DeclinedTransaction]
-    """
-    If the ACH Transfer attempt fails, this will contain the resulting
-    [Declined Transaction](#declined-transactions) object. The Declined
-    Transaction's `source` will be of `category: inbound_ach_transfer`.
-    """
+class InterestPaymentSimulationResult(BaseModel):
+    transaction: Transaction
+    """This will contain the resulting [Transaction](#transactions) object.
 
-    transaction: Optional[Transaction]
-    """
-    If the ACH Transfer attempt succeeds, this will contain the resulting
-    [Transaction](#transactions) object. The Transaction's `source` will be of
-    `category: inbound_ach_transfer`.
+    The Transaction's `source` will be of `category: interest_payment`.
     """
 
-    type: Literal["inbound_ach_transfer_simulation_result"]
+    type: Literal["interest_payment_simulation_result"]
     """A constant representing the object's type.
 
-    For this resource it will always be `inbound_ach_transfer_simulation_result`.
+    For this resource it will always be `interest_payment_simulation_result`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/simulations/card_authorization_simulation.py` & `increase-0.9.0/src/increase/types/declined_transaction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
 from datetime import datetime
 from typing_extensions import Literal
 
-from ...types import shared
-from ..._models import BaseModel
+from ..types import shared
+from .._models import BaseModel
 
 __all__ = [
-    "CardAuthorizationSimulation",
     "DeclinedTransaction",
-    "DeclinedTransactionSource",
-    "DeclinedTransactionSourceACHDecline",
-    "DeclinedTransactionSourceCardDecline",
-    "DeclinedTransactionSourceCardDeclineNetworkDetails",
-    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
-    "DeclinedTransactionSourceCheckDecline",
-    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
-    "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceWireDecline",
-    "PendingTransaction",
-    "PendingTransactionSource",
-    "PendingTransactionSourceAccountTransferInstruction",
-    "PendingTransactionSourceACHTransferInstruction",
-    "PendingTransactionSourceCardAuthorization",
-    "PendingTransactionSourceCardAuthorizationNetworkDetails",
-    "PendingTransactionSourceCardAuthorizationNetworkDetailsVisa",
-    "PendingTransactionSourceCheckDepositInstruction",
-    "PendingTransactionSourceCheckTransferInstruction",
-    "PendingTransactionSourceInboundFundsHold",
-    "PendingTransactionSourceRealTimePaymentsTransferInstruction",
-    "PendingTransactionSourceWireTransferInstruction",
+    "Source",
+    "SourceACHDecline",
+    "SourceCardDecline",
+    "SourceCardDeclineNetworkDetails",
+    "SourceCardDeclineNetworkDetailsVisa",
+    "SourceCheckDecline",
+    "SourceInboundRealTimePaymentsTransferDecline",
+    "SourceInternationalACHDecline",
+    "SourceWireDecline",
 ]
 
 
-class DeclinedTransactionSourceACHDecline(BaseModel):
+class SourceACHDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     originator_company_descriptive_date: Optional[str]
@@ -59,24 +46,39 @@
         "group_locked",
         "insufficient_funds",
         "misrouted_return",
         "no_ach_route",
         "originator_request",
         "transaction_not_allowed",
     ]
-    """Why the ACH transfer was declined."""
+    """Why the ACH transfer was declined.
+
+    - `ach_route_canceled` - The account number is canceled.
+    - `ach_route_disabled` - The account number is disabled.
+    - `breaches_limit` - The transaction would cause a limit to be exceeded.
+    - `credit_entry_refused_by_receiver` - A credit was refused.
+    - `duplicate_return` - Other.
+    - `entity_not_active` - The account's entity is not active.
+    - `group_locked` - Your account is inactive.
+    - `insufficient_funds` - Your account contains insufficient funds.
+    - `misrouted_return` - Other.
+    - `no_ach_route` - The account number that was debited does not exist.
+    - `originator_request` - Other.
+    - `transaction_not_allowed` - The transaction is not allowed per Increase's
+      terms.
+    """
 
     receiver_id_number: Optional[str]
 
     receiver_name: Optional[str]
 
     trace_number: str
 
 
-class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
+class SourceCardDeclineNetworkDetailsVisa(BaseModel):
     electronic_commerce_indicator: Optional[
         Literal[
             "mail_phone_order",
             "recurring",
             "installment",
             "unknown_mail_phone_order",
             "secure_electronic_commerce",
@@ -85,39 +87,76 @@
             "non_secure_transaction",
         ]
     ]
     """
     For electronic commerce transactions, this identifies the level of security used
     in obtaining the customer's payment credential. For mail or telephone order
     transactions, identifies the type of mail or telephone order.
+
+    - `mail_phone_order` - Single transaction of a mail/phone order: Use to indicate
+      that the transaction is a mail/phone order purchase, not a recurring
+      transaction or installment payment. For domestic transactions in the US
+      region, this value may also indicate one bill payment transaction in the
+      card-present or card-absent environments.
+    - `recurring` - Recurring transaction: Payment indicator used to indicate a
+      recurring transaction that originates from an acquirer in the US region.
+    - `installment` - Installment payment: Payment indicator used to indicate one
+      purchase of goods or services that is billed to the account in multiple
+      charges over a period of time agreed upon by the cardholder and merchant from
+      transactions that originate from an acquirer in the US region.
+    - `unknown_mail_phone_order` - Unknown classification: other mail order: Use to
+      indicate that the type of mail/telephone order is unknown.
+    - `secure_electronic_commerce` - Secure electronic commerce transaction: Use to
+      indicate that the electronic commerce transaction has been authenticated using
+      e.g., 3-D Secure
+    - `non_authenticated_security_transaction_at_3ds_capable_merchant` -
+      Non-authenticated security transaction at a 3-D Secure-capable merchant, and
+      merchant attempted to authenticate the cardholder using 3-D Secure: Use to
+      identify an electronic commerce transaction where the merchant attempted to
+      authenticate the cardholder using 3-D Secure, but was unable to complete the
+      authentication because the issuer or cardholder does not participate in the
+      3-D Secure program.
+    - `non_authenticated_security_transaction` - Non-authenticated security
+      transaction: Use to identify an electronic commerce transaction that uses data
+      encryption for security however , cardholder authentication is not performed
+      using 3-D Secure.
+    - `non_secure_transaction` - Non-secure transaction: Use to identify an
+      electronic commerce transaction that has no data protection.
     """
 
     point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
     """
     The method used to enter the cardholder's primary account number and card
     expiration date
     """
 
 
-class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
-    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
+class SourceCardDeclineNetworkDetails(BaseModel):
+    visa: SourceCardDeclineNetworkDetailsVisa
     """Fields specific to the `visa` network"""
 
 
-class DeclinedTransactionSourceCardDecline(BaseModel):
+class SourceCardDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
     account currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     digital_wallet_token_id: Optional[str]
     """
     If the authorization was attempted using a Digital Wallet Token (such as an
     Apple Pay purchase), the identifier of the token that was used.
     """
@@ -143,17 +182,20 @@
     merchant_descriptor: str
     """The merchant descriptor of the merchant the card is transacting with."""
 
     merchant_state: Optional[str]
     """The state the merchant resides in."""
 
     network: Literal["visa"]
-    """The payment network used to process this card authorization"""
+    """The payment network used to process this card authorization
 
-    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
+    - `visa` - Visa
+    """
+
+    network_details: SourceCardDeclineNetworkDetails
     """Fields specific to the `network`"""
 
     real_time_decision_id: Optional[str]
     """
     The identifier of the Real-Time Decision sent to approve or decline this
     transaction.
     """
@@ -169,18 +211,39 @@
         "breaches_limit",
         "webhook_declined",
         "webhook_timed_out",
         "declined_by_stand_in_processing",
         "invalid_physical_card",
         "missing_original_authorization",
     ]
-    """Why the transaction was declined."""
+    """Why the transaction was declined.
+
+    - `card_not_active` - The Card was not active.
+    - `entity_not_active` - The account's entity was not active.
+    - `group_locked` - The account was inactive.
+    - `insufficient_funds` - The Card's Account did not have a sufficient available
+      balance.
+    - `cvv2_mismatch` - The given CVV2 did not match the card's value.
+    - `transaction_not_allowed` - The attempted card transaction is not allowed per
+      Increase's terms.
+    - `breaches_internal_limit` - The transaction was blocked by an internal limit
+      for new Increase accounts.
+    - `breaches_limit` - The transaction was blocked by a Limit.
+    - `webhook_declined` - Your application declined the transaction via webhook.
+    - `webhook_timed_out` - Your application webhook did not respond without the
+      required timeout.
+    - `declined_by_stand_in_processing` - Declined by stand-in processing.
+    - `invalid_physical_card` - The card read had an invalid CVV, dCVV, or
+      authorization request cryptogram.
+    - `missing_original_authorization` - The original card authorization for this
+      incremental authorization does not exist.
+    """
 
 
-class DeclinedTransactionSourceCheckDecline(BaseModel):
+class SourceCheckDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     auxiliary_on_us: Optional[str]
@@ -198,32 +261,56 @@
         "refer_to_image",
         "stop_payment_requested",
         "returned",
         "duplicate_presentment",
         "not_authorized",
         "altered_or_fictitious",
     ]
-    """Why the check was declined."""
+    """Why the check was declined.
+
+    - `ach_route_canceled` - The account number is canceled.
+    - `ach_route_disabled` - The account number is disabled.
+    - `breaches_limit` - The transaction would cause a limit to be exceeded.
+    - `entity_not_active` - The account's entity is not active.
+    - `group_locked` - Your account is inactive.
+    - `insufficient_funds` - Your account contains insufficient funds.
+    - `unable_to_locate_account` - Unable to locate account.
+    - `not_our_item` - Routing number on the check is not ours.
+    - `unable_to_process` - Unable to process.
+    - `refer_to_image` - Refer to image.
+    - `stop_payment_requested` - Stop payment requested for this check.
+    - `returned` - Check was returned to sender.
+    - `duplicate_presentment` - The check was a duplicate deposit.
+    - `not_authorized` - The transaction is not allowed.
+    - `altered_or_fictitious` - The check was altered or fictitious.
+    """
 
 
-class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
+class SourceInboundRealTimePaymentsTransferDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     creditor_name: str
     """The name the sender of the transfer specified as the recipient of the transfer."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
     transfer's currency. This will always be "USD" for a Real Time Payments
     transfer.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     debtor_account_number: str
     """The account number of the account that sent the transfer."""
 
     debtor_name: str
     """The name provided by the sender of the transfer."""
@@ -235,24 +322,33 @@
         "account_number_canceled",
         "account_number_disabled",
         "account_restricted",
         "group_locked",
         "entity_not_active",
         "real_time_payments_not_enabled",
     ]
-    """Why the transfer was declined."""
+    """Why the transfer was declined.
+
+    - `account_number_canceled` - The account number is canceled.
+    - `account_number_disabled` - The account number is disabled.
+    - `account_restricted` - Your account is restricted.
+    - `group_locked` - Your account is inactive.
+    - `entity_not_active` - The account's entity is not active.
+    - `real_time_payments_not_enabled` - Your account is not enabled to receive Real
+      Time Payments transfers.
+    """
 
     remittance_information: Optional[str]
     """Additional information included with the transfer."""
 
     transaction_identification: str
     """The Real Time Payments network identification of the declined transfer."""
 
 
-class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
+class SourceInternationalACHDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     destination_country_code: str
@@ -322,15 +418,15 @@
     receiving_depository_financial_institution_id_qualifier: str
 
     receiving_depository_financial_institution_name: str
 
     trace_number: str
 
 
-class DeclinedTransactionSourceWireDecline(BaseModel):
+class SourceWireDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     beneficiary_address_line1: Optional[str]
@@ -367,26 +463,35 @@
         "account_number_canceled",
         "account_number_disabled",
         "entity_not_active",
         "group_locked",
         "no_account_number",
         "transaction_not_allowed",
     ]
-    """Why the wire transfer was declined."""
+    """Why the wire transfer was declined.
 
+    - `account_number_canceled` - The account number is canceled.
+    - `account_number_disabled` - The account number is disabled.
+    - `entity_not_active` - The account's entity is not active.
+    - `group_locked` - Your account is inactive.
+    - `no_account_number` - The beneficiary account number does not exist.
+    - `transaction_not_allowed` - The transaction is not allowed per Increase's
+      terms.
+    """
 
-class DeclinedTransactionSource(BaseModel):
-    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
+
+class Source(BaseModel):
+    ach_decline: Optional[SourceACHDecline]
     """A ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_decline`.
     """
 
-    card_decline: Optional[DeclinedTransactionSourceCardDecline]
+    card_decline: Optional[SourceCardDecline]
     """A Card Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_decline`.
     """
 
     category: Literal[
@@ -398,40 +503,55 @@
         "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
+
+    - `ach_decline` - The Declined Transaction was created by a ACH Decline object.
+      Details will be under the `ach_decline` object.
+    - `card_decline` - The Declined Transaction was created by a Card Decline
+      object. Details will be under the `card_decline` object.
+    - `check_decline` - The Declined Transaction was created by a Check Decline
+      object. Details will be under the `check_decline` object.
+    - `inbound_real_time_payments_transfer_decline` - The Declined Transaction was
+      created by a Inbound Real Time Payments Transfer Decline object. Details will
+      be under the `inbound_real_time_payments_transfer_decline` object.
+    - `international_ach_decline` - The Declined Transaction was created by a
+      International ACH Decline object. Details will be under the
+      `international_ach_decline` object.
+    - `wire_decline` - The Declined Transaction was created by a Wire Decline
+      object. Details will be under the `wire_decline` object.
+    - `other` - The Declined Transaction was made for an undocumented or deprecated
+      reason.
     """
 
-    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
+    check_decline: Optional[SourceCheckDecline]
     """A Check Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_decline`.
     """
 
-    inbound_real_time_payments_transfer_decline: Optional[
-        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
-    ]
+    inbound_real_time_payments_transfer_decline: Optional[SourceInboundRealTimePaymentsTransferDecline]
     """A Inbound Real Time Payments Transfer Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `inbound_real_time_payments_transfer_decline`.
     """
 
-    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
+    international_ach_decline: Optional[SourceInternationalACHDecline]
     """A International ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `international_ach_decline`.
     """
 
-    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
+    wire_decline: Optional[SourceWireDecline]
     """A Wire Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_decline`.
     """
 
 
@@ -455,445 +575,46 @@
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
     Transaction's currency. This will match the currency on the Declined
     Transcation's Account.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
     """This is the description the vendor provides."""
 
     route_id: Optional[str]
     """The identifier for the route this Declined Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Declined Transaction came through."""
+    """The type of the route this Declined Transaction came through.
 
-    source: DeclinedTransactionSource
+    - `account_number` - An Account Number.
+    - `card` - A Card.
+    """
+
+    source: Source
     """
     This is an object giving more details on the network-level event that caused the
     Declined Transaction. For example, for a card transaction this lists the
     merchant's industry and location. Note that for backwards compatibility reasons,
     additional undocumented keys may appear in this object. These should be treated
     as deprecated and will be removed in the future.
     """
 
     type: Literal["declined_transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `declined_transaction`.
     """
-
-
-class PendingTransactionSourceAccountTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    transfer_id: str
-    """The identifier of the Account Transfer that led to this Pending Transaction."""
-
-
-class PendingTransactionSourceACHTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    transfer_id: str
-    """The identifier of the ACH Transfer that led to this Pending Transaction."""
-
-
-class PendingTransactionSourceCardAuthorizationNetworkDetailsVisa(BaseModel):
-    electronic_commerce_indicator: Optional[
-        Literal[
-            "mail_phone_order",
-            "recurring",
-            "installment",
-            "unknown_mail_phone_order",
-            "secure_electronic_commerce",
-            "non_authenticated_security_transaction_at_3ds_capable_merchant",
-            "non_authenticated_security_transaction",
-            "non_secure_transaction",
-        ]
-    ]
-    """
-    For electronic commerce transactions, this identifies the level of security used
-    in obtaining the customer's payment credential. For mail or telephone order
-    transactions, identifies the type of mail or telephone order.
-    """
-
-    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
-    """
-    The method used to enter the cardholder's primary account number and card
-    expiration date
-    """
-
-
-class PendingTransactionSourceCardAuthorizationNetworkDetails(BaseModel):
-    visa: PendingTransactionSourceCardAuthorizationNetworkDetailsVisa
-    """Fields specific to the `visa` network"""
-
-
-class PendingTransactionSourceCardAuthorization(BaseModel):
-    id: str
-    """The Card Authorization identifier."""
-
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    digital_wallet_token_id: Optional[str]
-    """
-    If the authorization was made via a Digital Wallet Token (such as an Apple Pay
-    purchase), the identifier of the token that was used.
-    """
-
-    expires_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) when this authorization
-    will expire and the pending transaction will be released.
-    """
-
-    merchant_acceptor_id: str
-    """
-    The merchant identifier (commonly abbreviated as MID) of the merchant the card
-    is transacting with.
-    """
-
-    merchant_category_code: Optional[str]
-    """
-    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
-    card is transacting with.
-    """
-
-    merchant_city: Optional[str]
-    """The city the merchant resides in."""
-
-    merchant_country: Optional[str]
-    """The country the merchant resides in."""
-
-    merchant_descriptor: str
-    """The merchant descriptor of the merchant the card is transacting with."""
-
-    network: Literal["visa"]
-    """The payment network used to process this card authorization"""
-
-    network_details: PendingTransactionSourceCardAuthorizationNetworkDetails
-    """Fields specific to the `network`"""
-
-    pending_transaction_id: Optional[str]
-    """The identifier of the Pending Transaction associated with this Transaction."""
-
-    real_time_decision_id: Optional[str]
-    """
-    The identifier of the Real-Time Decision sent to approve or decline this
-    transaction.
-    """
-
-    type: Literal["card_authorization"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `card_authorization`.
-    """
-
-
-class PendingTransactionSourceCheckDepositInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    back_image_file_id: Optional[str]
-    """
-    The identifier of the File containing the image of the back of the check that
-    was deposited.
-    """
-
-    check_deposit_id: Optional[str]
-    """The identifier of the Check Deposit."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    front_image_file_id: str
-    """
-    The identifier of the File containing the image of the front of the check that
-    was deposited.
-    """
-
-
-class PendingTransactionSourceCheckTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
-    currency.
-    """
-
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Pending Transaction."""
-
-
-class PendingTransactionSourceInboundFundsHold(BaseModel):
-    amount: int
-    """The held amount in the minor unit of the account's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    automatically_releases_at: datetime
-    """When the hold will be released automatically.
-
-    Certain conditions may cause it to be released before this time.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the hold
-    was created.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the hold's
-    currency.
-    """
-
-    held_transaction_id: Optional[str]
-    """The ID of the Transaction for which funds were held."""
-
-    pending_transaction_id: Optional[str]
-    """The ID of the Pending Transaction representing the held funds."""
-
-    released_at: Optional[datetime]
-    """When the hold was released (if it has been released)."""
-
-    status: Literal["held", "complete"]
-    """The status of the hold."""
-
-
-class PendingTransactionSourceRealTimePaymentsTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    transfer_id: str
-    """
-    The identifier of the Real Time Payments Transfer that led to this Pending
-    Transaction.
-    """
-
-
-class PendingTransactionSourceWireTransferInstruction(BaseModel):
-    account_number: str
-
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    message_to_recipient: str
-
-    routing_number: str
-
-    transfer_id: str
-
-
-class PendingTransactionSource(BaseModel):
-    account_transfer_instruction: Optional[PendingTransactionSourceAccountTransferInstruction]
-    """A Account Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `account_transfer_instruction`.
-    """
-
-    ach_transfer_instruction: Optional[PendingTransactionSourceACHTransferInstruction]
-    """A ACH Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_transfer_instruction`.
-    """
-
-    card_authorization: Optional[PendingTransactionSourceCardAuthorization]
-    """A Card Authorization object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_authorization`.
-    """
-
-    category: Literal[
-        "account_transfer_instruction",
-        "ach_transfer_instruction",
-        "card_authorization",
-        "check_deposit_instruction",
-        "check_transfer_instruction",
-        "inbound_funds_hold",
-        "real_time_payments_transfer_instruction",
-        "wire_transfer_instruction",
-        "other",
-    ]
-    """The type of transaction that took place.
-
-    We may add additional possible values for this enum over time; your application
-    should be able to handle such additions gracefully.
-    """
-
-    check_deposit_instruction: Optional[PendingTransactionSourceCheckDepositInstruction]
-    """A Check Deposit Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_deposit_instruction`.
-    """
-
-    check_transfer_instruction: Optional[PendingTransactionSourceCheckTransferInstruction]
-    """A Check Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_instruction`.
-    """
-
-    inbound_funds_hold: Optional[PendingTransactionSourceInboundFundsHold]
-    """A Inbound Funds Hold object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_funds_hold`.
-    """
-
-    real_time_payments_transfer_instruction: Optional[PendingTransactionSourceRealTimePaymentsTransferInstruction]
-    """A Real Time Payments Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `real_time_payments_transfer_instruction`.
-    """
-
-    wire_transfer_instruction: Optional[PendingTransactionSourceWireTransferInstruction]
-    """A Wire Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_transfer_instruction`.
-    """
-
-
-class PendingTransaction(BaseModel):
-    id: str
-    """The Pending Transaction identifier."""
-
-    account_id: str
-    """The identifier for the account this Pending Transaction belongs to."""
-
-    amount: int
-    """The Pending Transaction amount in the minor unit of its currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    completed_at: Optional[datetime]
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
-    Transaction was completed.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
-    Transaction occured.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Pending
-    Transaction's currency. This will match the currency on the Pending
-    Transcation's Account.
-    """
-
-    description: str
-    """
-    For a Pending Transaction related to a transfer, this is the description you
-    provide. For a Pending Transaction related to a payment, this is the description
-    the vendor provides.
-    """
-
-    route_id: Optional[str]
-    """The identifier for the route this Pending Transaction came through.
-
-    Routes are things like cards and ACH details.
-    """
-
-    route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Pending Transaction came through."""
-
-    source: PendingTransactionSource
-    """
-    This is an object giving more details on the network-level event that caused the
-    Pending Transaction. For example, for a card transaction this lists the
-    merchant's industry and location.
-    """
-
-    status: Literal["pending", "complete"]
-    """
-    Whether the Pending Transaction has been confirmed and has an associated
-    Transaction.
-    """
-
-    type: Literal["pending_transaction"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `pending_transaction`.
-    """
-
-
-class CardAuthorizationSimulation(BaseModel):
-    declined_transaction: Optional[DeclinedTransaction]
-    """
-    If the authorization attempt fails, this will contain the resulting
-    [Declined Transaction](#declined-transactions) object. The Declined
-    Transaction's `source` will be of `category: card_decline`.
-    """
-
-    pending_transaction: Optional[PendingTransaction]
-    """
-    If the authorization attempt succeeds, this will contain the resulting Pending
-    Transaction object. The Pending Transaction's `source` will be of
-    `category: card_authorization`.
-    """
-
-    type: Literal["inbound_card_authorization_simulation_result"]
-    """A constant representing the object's type.
-
-    For this resource it will always be
-    `inbound_card_authorization_simulation_result`.
-    """
```

### Comparing `increase-0.8.1/src/increase/types/simulations/card_authorize_params.py` & `increase-0.9.0/src/increase/types/simulations/card_authorize_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/simulations/card_settlement_params.py` & `increase-0.9.0/src/increase/types/simulations/card_settlement_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py` & `increase-0.9.0/src/increase/types/simulations/wire_transfer_simulation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
 from datetime import date, datetime
 from typing_extensions import Literal
 
-from ...types import shared
 from ..._models import BaseModel
 
 __all__ = [
-    "InboundRealTimePaymentsTransferSimulationResult",
-    "DeclinedTransaction",
-    "DeclinedTransactionSource",
-    "DeclinedTransactionSourceACHDecline",
-    "DeclinedTransactionSourceCardDecline",
-    "DeclinedTransactionSourceCardDeclineNetworkDetails",
-    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
-    "DeclinedTransactionSourceCheckDecline",
-    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
-    "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceWireDecline",
+    "WireTransferSimulation",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
@@ -30,15 +19,14 @@
     "TransactionSourceCardRevenuePayment",
     "TransactionSourceCardSettlement",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferDeposit",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferRejection",
-    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPayment",
@@ -50,480 +38,32 @@
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
 ]
 
 
-class DeclinedTransactionSourceACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    originator_company_descriptive_date: Optional[str]
-
-    originator_company_discretionary_data: Optional[str]
-
-    originator_company_id: str
-
-    originator_company_name: str
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "credit_entry_refused_by_receiver",
-        "duplicate_return",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "misrouted_return",
-        "no_ach_route",
-        "originator_request",
-        "transaction_not_allowed",
-    ]
-    """Why the ACH transfer was declined."""
-
-    receiver_id_number: Optional[str]
-
-    receiver_name: Optional[str]
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
-    electronic_commerce_indicator: Optional[
-        Literal[
-            "mail_phone_order",
-            "recurring",
-            "installment",
-            "unknown_mail_phone_order",
-            "secure_electronic_commerce",
-            "non_authenticated_security_transaction_at_3ds_capable_merchant",
-            "non_authenticated_security_transaction",
-            "non_secure_transaction",
-        ]
-    ]
-    """
-    For electronic commerce transactions, this identifies the level of security used
-    in obtaining the customer's payment credential. For mail or telephone order
-    transactions, identifies the type of mail or telephone order.
-    """
-
-    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
-    """
-    The method used to enter the cardholder's primary account number and card
-    expiration date
-    """
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
-    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
-    """Fields specific to the `visa` network"""
-
-
-class DeclinedTransactionSourceCardDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    digital_wallet_token_id: Optional[str]
-    """
-    If the authorization was attempted using a Digital Wallet Token (such as an
-    Apple Pay purchase), the identifier of the token that was used.
-    """
-
-    merchant_acceptor_id: str
-    """
-    The merchant identifier (commonly abbreviated as MID) of the merchant the card
-    is transacting with.
-    """
-
-    merchant_category_code: Optional[str]
-    """
-    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
-    card is transacting with.
-    """
-
-    merchant_city: Optional[str]
-    """The city the merchant resides in."""
-
-    merchant_country: Optional[str]
-    """The country the merchant resides in."""
-
-    merchant_descriptor: str
-    """The merchant descriptor of the merchant the card is transacting with."""
-
-    merchant_state: Optional[str]
-    """The state the merchant resides in."""
-
-    network: Literal["visa"]
-    """The payment network used to process this card authorization"""
-
-    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
-    """Fields specific to the `network`"""
-
-    real_time_decision_id: Optional[str]
-    """
-    The identifier of the Real-Time Decision sent to approve or decline this
-    transaction.
-    """
-
-    reason: Literal[
-        "card_not_active",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "cvv2_mismatch",
-        "transaction_not_allowed",
-        "breaches_internal_limit",
-        "breaches_limit",
-        "webhook_declined",
-        "webhook_timed_out",
-        "declined_by_stand_in_processing",
-        "invalid_physical_card",
-        "missing_original_authorization",
-    ]
-    """Why the transaction was declined."""
-
-
-class DeclinedTransactionSourceCheckDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    auxiliary_on_us: Optional[str]
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "unable_to_locate_account",
-        "not_our_item",
-        "unable_to_process",
-        "refer_to_image",
-        "stop_payment_requested",
-        "returned",
-        "duplicate_presentment",
-        "not_authorized",
-        "altered_or_fictitious",
-    ]
-    """Why the check was declined."""
-
-
-class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    creditor_name: str
-    """The name the sender of the transfer specified as the recipient of the transfer."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
-    transfer's currency. This will always be "USD" for a Real Time Payments
-    transfer.
-    """
-
-    debtor_account_number: str
-    """The account number of the account that sent the transfer."""
-
-    debtor_name: str
-    """The name provided by the sender of the transfer."""
-
-    debtor_routing_number: str
-    """The routing number of the account that sent the transfer."""
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "account_restricted",
-        "group_locked",
-        "entity_not_active",
-        "real_time_payments_not_enabled",
-    ]
-    """Why the transfer was declined."""
-
-    remittance_information: Optional[str]
-    """Additional information included with the transfer."""
-
-    transaction_identification: str
-    """The Real Time Payments network identification of the declined transfer."""
-
-
-class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    destination_country_code: str
-
-    destination_currency_code: str
-
-    foreign_exchange_indicator: str
-
-    foreign_exchange_reference: Optional[str]
-
-    foreign_exchange_reference_indicator: str
-
-    foreign_payment_amount: int
-
-    foreign_trace_number: Optional[str]
-
-    international_transaction_type_code: str
-
-    originating_currency_code: str
-
-    originating_depository_financial_institution_branch_country: str
-
-    originating_depository_financial_institution_id: str
-
-    originating_depository_financial_institution_id_qualifier: str
-
-    originating_depository_financial_institution_name: str
-
-    originator_city: str
-
-    originator_company_entry_description: str
-
-    originator_country: str
-
-    originator_identification: str
-
-    originator_name: str
-
-    originator_postal_code: Optional[str]
-
-    originator_state_or_province: Optional[str]
-
-    originator_street_address: str
-
-    payment_related_information: Optional[str]
-
-    payment_related_information2: Optional[str]
-
-    receiver_city: str
-
-    receiver_country: str
-
-    receiver_identification_number: Optional[str]
-
-    receiver_postal_code: Optional[str]
-
-    receiver_state_or_province: Optional[str]
-
-    receiver_street_address: str
-
-    receiving_company_or_individual_name: str
-
-    receiving_depository_financial_institution_country: str
-
-    receiving_depository_financial_institution_id: str
-
-    receiving_depository_financial_institution_id_qualifier: str
-
-    receiving_depository_financial_institution_name: str
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceWireDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    beneficiary_address_line1: Optional[str]
-
-    beneficiary_address_line2: Optional[str]
-
-    beneficiary_address_line3: Optional[str]
-
-    beneficiary_name: Optional[str]
-
-    beneficiary_reference: Optional[str]
-
-    description: str
-
-    input_message_accountability_data: Optional[str]
-
-    originator_address_line1: Optional[str]
-
-    originator_address_line2: Optional[str]
-
-    originator_address_line3: Optional[str]
-
-    originator_name: Optional[str]
-
-    originator_to_beneficiary_information_line1: Optional[str]
-
-    originator_to_beneficiary_information_line2: Optional[str]
-
-    originator_to_beneficiary_information_line3: Optional[str]
-
-    originator_to_beneficiary_information_line4: Optional[str]
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "entity_not_active",
-        "group_locked",
-        "no_account_number",
-        "transaction_not_allowed",
-    ]
-    """Why the wire transfer was declined."""
-
-
-class DeclinedTransactionSource(BaseModel):
-    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
-    """A ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_decline`.
-    """
-
-    card_decline: Optional[DeclinedTransactionSourceCardDecline]
-    """A Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_decline`.
-    """
-
-    category: Literal[
-        "ach_decline",
-        "card_decline",
-        "check_decline",
-        "inbound_real_time_payments_transfer_decline",
-        "international_ach_decline",
-        "wire_decline",
-        "other",
-    ]
-    """The type of decline that took place.
-
-    We may add additional possible values for this enum over time; your application
-    should be able to handle such additions gracefully.
-    """
-
-    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
-    """A Check Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_decline`.
-    """
-
-    inbound_real_time_payments_transfer_decline: Optional[
-        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
-    ]
-    """A Inbound Real Time Payments Transfer Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_real_time_payments_transfer_decline`.
-    """
-
-    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
-    """A International ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `international_ach_decline`.
-    """
-
-    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
-    """A Wire Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_decline`.
-    """
-
-
-class DeclinedTransaction(BaseModel):
-    id: str
-    """The Declined Transaction identifier."""
-
-    account_id: str
-    """The identifier for the Account the Declined Transaction belongs to."""
-
-    amount: int
-    """The Declined Transaction amount in the minor unit of its currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
-    Transaction occured.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
-    Transaction's currency. This will match the currency on the Declined
-    Transcation's Account.
-    """
-
-    description: str
-    """This is the description the vendor provides."""
-
-    route_id: Optional[str]
-    """The identifier for the route this Declined Transaction came through.
-
-    Routes are things like cards and ACH details.
-    """
-
-    route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Declined Transaction came through."""
-
-    source: DeclinedTransactionSource
-    """
-    This is an object giving more details on the network-level event that caused the
-    Declined Transaction. For example, for a card transaction this lists the
-    merchant's industry and location. Note that for backwards compatibility reasons,
-    additional undocumented keys may appear in this object. These should be treated
-    as deprecated and will be removed in the future.
-    """
-
-    type: Literal["declined_transaction"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `declined_transaction`.
-    """
-
-
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
     account currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
     """The description you chose to give the transfer."""
 
     destination_account_id: str
     """The identifier of the Account to where the Account Transfer was sent."""
@@ -635,15 +175,161 @@
         "stop_payment_on_item_related_to_rck_entry",
         "stop_payment_on_source_document",
         "timely_original_return",
         "trace_number_error",
         "untimely_dishonored_return",
         "untimely_return",
     ]
-    """Why the ACH Transfer was returned."""
+    """Why the ACH Transfer was returned.
+
+    - `insufficient_fund` - Code R01. Insufficient funds in the source account.
+    - `no_account` - Code R03. The account does not exist or the receiving bank was
+      unable to locate it.
+    - `account_closed` - Code R02. The account is closed.
+    - `invalid_account_number_structure` - Code R04. The account number is invalid
+      at the receiving bank.
+    - `account_frozen_entry_returned_per_ofac_instruction` - Code R16. The account
+      was frozen per the Office of Foreign Assets Control.
+    - `credit_entry_refused_by_receiver` - Code R23. The receiving bank account
+      refused a credit transfer.
+    - `unauthorized_debit_to_consumer_account_using_corporate_sec_code` - Code R05.
+      The receiving bank rejected because of an incorrect Standard Entry Class code.
+    - `corporate_customer_advised_not_authorized` - Code R29. The corporate customer
+      reversed the transfer.
+    - `payment_stopped` - Code R08. The receiving bank stopped payment on this
+      transfer.
+    - `non_transaction_account` - Code R20. The receiving bank account does not
+      perform transfers.
+    - `uncollected_funds` - Code R09. The receiving bank account does not have
+      enough available balance for the transfer.
+    - `routing_number_check_digit_error` - Code R28. The routing number is
+      incorrect.
+    - `customer_advised_unauthorized_improper_ineligible_or_incomplete` - Code R10.
+      The customer reversed the transfer.
+    - `amount_field_error` - Code R19. The amount field is incorrect or too large.
+    - `authorization_revoked_by_customer` - Code R07. The customer who initiated the
+      transfer revoked authorization.
+    - `invalid_ach_routing_number` - Code R13. The routing number is invalid.
+    - `file_record_edit_criteria` - Code R17. The receiving bank is unable to
+      process a field in the transfer.
+    - `enr_invalid_individual_name` - Code R45. The individual name field was
+      invalid.
+    - `returned_per_odfi_request` - Code R06. The originating financial institution
+      reversed the transfer.
+    - `limited_participation_dfi` - Code R34. The receiving bank's regulatory
+      supervisor has limited their participation.
+    - `incorrectly_coded_outbound_international_payment` - Code R85. The outbound
+      international ACH transfer was incorrect.
+    - `account_sold_to_another_dfi` - Code R12. A rare return reason. The account
+      was sold to another bank.
+    - `addenda_error` - Code R25. The addenda record is incorrect or missing.
+    - `beneficiary_or_account_holder_deceased` - Code R15. A rare return reason. The
+      account holder is deceased.
+    - `customer_advised_not_within_authorization_terms` - Code R11. A rare return
+      reason. The customer authorized some payment to the sender, but this payment
+      was not in error.
+    - `corrected_return` - Code R74. A rare return reason. Sent in response to a
+      return that was returned with code `field_error`. The latest return should
+      include the corrected field(s).
+    - `duplicate_entry` - Code R24. A rare return reason. The receiving bank
+      received an exact duplicate entry with the same trace number and amount.
+    - `duplicate_return` - Code R67. A rare return reason. The return this message
+      refers to was a duplicate.
+    - `enr_duplicate_enrollment` - Code R47. A rare return reason. Only used for US
+      Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_dfi_account_number` - Code R43. A rare return reason. Only used
+      for US Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_individual_id_number` - Code R44. A rare return reason. Only used
+      for US Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_representative_payee_indicator` - Code R46. A rare return reason.
+      Only used for US Government agency non-monetary automatic enrollment messages.
+    - `enr_invalid_transaction_code` - Code R41. A rare return reason. Only used for
+      US Government agency non-monetary automatic enrollment messages.
+    - `enr_return_of_enr_entry` - Code R40. A rare return reason. Only used for US
+      Government agency non-monetary automatic enrollment messages.
+    - `enr_routing_number_check_digit_error` - Code R42. A rare return reason. Only
+      used for US Government agency non-monetary automatic enrollment messages.
+    - `entry_not_processed_by_gateway` - Code R84. A rare return reason. The
+      International ACH Transfer cannot be processed by the gateway.
+    - `field_error` - Code R69. A rare return reason. One or more of the fields in
+      the ACH were malformed.
+    - `foreign_receiving_dfi_unable_to_settle` - Code R83. A rare return reason. The
+      Foreign receiving bank was unable to settle this ACH transfer.
+    - `iat_entry_coding_error` - Code R80. A rare return reason. The International
+      ACH Transfer is malformed.
+    - `improper_effective_entry_date` - Code R18. A rare return reason. The ACH has
+      an improper effective entry date field.
+    - `improper_source_document_source_document_presented` - Code R39. A rare return
+      reason. The source document related to this ACH, usually an ACH check
+      conversion, was presented to the bank.
+    - `invalid_company_id` - Code R21. A rare return reason. The Company ID field of
+      the ACH was invalid.
+    - `invalid_foreign_receiving_dfi_identification` - Code R82. A rare return
+      reason. The foreign receiving bank identifier for an International ACH
+      Transfer was invalid.
+    - `invalid_individual_id_number` - Code R22. A rare return reason. The
+      Individual ID number field of the ACH was invalid.
+    - `item_and_rck_entry_presented_for_payment` - Code R53. A rare return reason.
+      Both the Represented Check ("RCK") entry and the original check were presented
+      to the bank.
+    - `item_related_to_rck_entry_is_ineligible` - Code R51. A rare return reason.
+      The Represented Check ("RCK") entry is ineligible.
+    - `mandatory_field_error` - Code R26. A rare return reason. The ACH is missing a
+      required field.
+    - `misrouted_dishonored_return` - Code R71. A rare return reason. The receiving
+      bank does not recognize the routing number in a dishonored return entry.
+    - `misrouted_return` - Code R61. A rare return reason. The receiving bank does
+      not recognize the routing number in a return entry.
+    - `no_errors_found` - Code R76. A rare return reason. Sent in response to a
+      return, the bank does not find the errors alleged by the returning bank.
+    - `non_acceptance_of_r62_dishonored_return` - Code R77. A rare return reason.
+      The receiving bank does not accept the return of the erroneous debit. The
+      funds are not available at the receiving bank.
+    - `non_participant_in_iat_program` - Code R81. A rare return reason. The
+      receiving bank does not accept International ACH Transfers.
+    - `permissible_return_entry` - Code R31. A rare return reason. A return that has
+      been agreed to be accepted by the receiving bank, despite falling outside of
+      the usual return timeframe.
+    - `permissible_return_entry_not_accepted` - Code R70. A rare return reason. The
+      receiving bank had not approved this return.
+    - `rdfi_non_settlement` - Code R32. A rare return reason. The receiving bank
+      could not settle this transaction.
+    - `rdfi_participant_in_check_truncation_program` - Code R30. A rare return
+      reason. The receiving bank does not accept Check Truncation ACH transfers.
+    - `representative_payee_deceased_or_unable_to_continue_in_that_capacity` - Code
+      R14. A rare return reason. The payee is deceased.
+    - `return_not_a_duplicate` - Code R75. A rare return reason. The originating
+      bank disputes that an earlier `duplicate_entry` return was actually a
+      duplicate.
+    - `return_of_erroneous_or_reversing_debit` - Code R62. A rare return reason. The
+      originating bank made a mistake earlier and this return corrects it.
+    - `return_of_improper_credit_entry` - Code R36. A rare return reason. Return of
+      a malformed credit entry.
+    - `return_of_improper_debit_entry` - Code R35. A rare return reason. Return of a
+      malformed debit entry.
+    - `return_of_xck_entry` - Code R33. A rare return reason. Return of a Destroyed
+      Check ("XKC") entry.
+    - `source_document_presented_for_payment` - Code R37. A rare return reason. The
+      source document related to this ACH, usually an ACH check conversion, was
+      presented to the bank.
+    - `state_law_affecting_rck_acceptance` - Code R50. A rare return reason. State
+      law prevents the bank from accepting the Represented Check ("RCK") entry.
+    - `stop_payment_on_item_related_to_rck_entry` - Code R52. A rare return reason.
+      A stop payment was issued on a Represented Check ("RCK") entry.
+    - `stop_payment_on_source_document` - Code R38. A rare return reason. The source
+      attached to the ACH, usually an ACH check conversion, includes a stop payment.
+    - `timely_original_return` - Code R73. A rare return reason. The bank receiving
+      an `untimely_return` believes it was on time.
+    - `trace_number_error` - Code R27. A rare return reason. An ACH Return's trace
+      number does not match an originated ACH.
+    - `untimely_dishonored_return` - Code R72. A rare return reason. The dishonored
+      return was sent too late.
+    - `untimely_return` - Code R68. A rare return reason. The return was sent too
+      late.
+    """
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
     """The identifier of the ACH Transfer associated with this return."""
 
@@ -675,14 +361,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
@@ -698,14 +391,17 @@
 
     merchant_name: Optional[str]
     """The name of the merchant."""
 
     merchant_state: Optional[str]
     """The state the merchant resides in."""
 
+    transaction_id: str
+    """The identifier of the Transaction associated with this Transaction."""
+
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
@@ -716,14 +412,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     period_end: datetime
     """The end of the period for which this transaction paid interest."""
 
     period_start: datetime
     """The start of the period for which this transaction paid interest."""
@@ -748,14 +451,21 @@
     exists.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
@@ -783,14 +493,17 @@
 
     presentment_currency: str
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's presentment currency.
     """
 
+    transaction_id: str
+    """The identifier of the Transaction associated with this Transaction."""
+
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
@@ -813,14 +526,21 @@
     check_deposit_id: str
     """The ID of the Check Deposit that was accepted."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     routing_number: str
     """The routing number printed on the check."""
 
     serial_number: Optional[str]
     """The check serial number, if present, for consumer checks.
@@ -840,14 +560,21 @@
     check_deposit_id: str
     """The identifier of the Check Deposit that was returned."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     return_reason: Literal[
         "ach_conversion_not_supported",
         "closed_account",
         "duplicate_submission",
         "insufficient_funds",
@@ -856,14 +583,28 @@
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
         "endorsement_irregular",
     ]
+    """
+    - `ach_conversion_not_supported` - The check doesn't allow ACH conversion.
+    - `closed_account` - The account is closed.
+    - `duplicate_submission` - The check has already been deposited.
+    - `insufficient_funds` - Insufficient funds
+    - `no_account` - No account was found matching the check details.
+    - `not_authorized` - The check was not authorized.
+    - `stale_dated` - The check is too old.
+    - `stop_payment` - The payment has been stopped by the account holder.
+    - `unknown_reason` - The reason for the return is unknown.
+    - `unmatched_details` - The image doesn't match the details submitted.
+    - `unreadable_image` - The image could not be read.
+    - `endorsement_irregular` - The check endorsement was irregular.
+    """
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
 
@@ -886,14 +627,17 @@
 
     front_image_file_id: Optional[str]
     """
     The identifier of the API File object containing an image of the front of the
     deposited check.
     """
 
+    transaction_id: Optional[str]
+    """The identifier of the Transaction object created when the check was deposited."""
+
     type: Literal["check_transfer_deposit"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_deposit`.
     """
 
 
@@ -916,58 +660,46 @@
     amount: int
     """The transfer amount in USD cents."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     transfer_id: str
     """The identifier of the Check Transfer with which this is associated."""
 
 
 class TransactionSourceCheckTransferRejection(BaseModel):
     transfer_id: str
     """The identifier of the Check Transfer that led to this Transaction."""
 
 
-class TransactionSourceCheckTransferReturn(BaseModel):
-    file_id: Optional[str]
-    """If available, a document with additional information about the return."""
-
-    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
-    """The reason why the check was returned."""
-
-    returned_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the check was returned.
-    """
+class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
+    reason: Literal["mail_delivery_failed", "unknown"]
+    """The reason why this transfer was stopped.
 
-    transaction_id: Optional[str]
-    """
-    The identifier of the Transaction that was created to credit you for the
-    returned check.
+    - `mail_delivery_failed` - The check could not be delivered.
+    - `unknown` - The check was stopped for another reason.
     """
 
-    transfer_id: str
-    """The identifier of the returned Check Transfer."""
-
-
-class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
-    transaction_id: str
-    """The transaction ID of the corresponding credit transaction."""
-
     transfer_id: str
     """The ID of the check transfer that was stopped."""
 
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
@@ -981,14 +713,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
 
 class TransactionSourceInboundACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
@@ -1025,14 +764,21 @@
 
     check_rear_image_file_id: Optional[str]
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
 
 class TransactionSourceInboundInternationalACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
@@ -1120,14 +866,21 @@
     creditor_name: str
     """The name the sender of the transfer specified as the recipient of the transfer."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the transfer's
     currency. This will always be "USD" for a Real Time Payments transfer.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     debtor_account_number: str
     """The account number of the account that sent the transfer."""
 
     debtor_name: str
     """The name provided by the sender of the transfer."""
@@ -1309,14 +1062,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     period_end: datetime
     """The end of the period for which this transaction paid interest."""
 
     period_start: datetime
     """The start of the period for which this transaction paid interest."""
@@ -1329,14 +1089,21 @@
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     reason: Literal[
         "account_closure",
         "bank_migration",
         "cashback",
         "collection_receivable",
@@ -1345,14 +1112,28 @@
         "error_correction",
         "fees",
         "interest",
         "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
+    """
+    - `account_closure` - Account closure
+    - `bank_migration` - Bank migration
+    - `cashback` - Cashback
+    - `collection_receivable` - Collection receivable
+    - `empyreal_adjustment` - Empyreal adjustment
+    - `error` - Error
+    - `error_correction` - Error correction
+    - `fees` - Fees
+    - `interest` - Interest
+    - `negative_balance_forgiveness` - Negative balance forgiveness
+    - `sample_funds` - Sample funds
+    - `sample_funds_return` - Sample funds return
+    """
 
 
 class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
     amount: int
     """The transfer amount in USD cents."""
 
     destination_account_number: str
@@ -1460,15 +1241,14 @@
         "card_revenue_payment",
         "card_settlement",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_deposit",
         "check_transfer_intention",
         "check_transfer_rejection",
-        "check_transfer_return",
         "check_transfer_stop_payment_request",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
@@ -1484,14 +1264,85 @@
         "wire_transfer_rejection",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
+
+    - `account_transfer_intention` - The Transaction was created by a Account
+      Transfer Intention object. Details will be under the
+      `account_transfer_intention` object.
+    - `ach_transfer_intention` - The Transaction was created by a ACH Transfer
+      Intention object. Details will be under the `ach_transfer_intention` object.
+    - `ach_transfer_rejection` - The Transaction was created by a ACH Transfer
+      Rejection object. Details will be under the `ach_transfer_rejection` object.
+    - `ach_transfer_return` - The Transaction was created by a ACH Transfer Return
+      object. Details will be under the `ach_transfer_return` object.
+    - `card_dispute_acceptance` - The Transaction was created by a Card Dispute
+      Acceptance object. Details will be under the `card_dispute_acceptance` object.
+    - `card_refund` - The Transaction was created by a Card Refund object. Details
+      will be under the `card_refund` object.
+    - `card_revenue_payment` - The Transaction was created by a Card Revenue Payment
+      object. Details will be under the `card_revenue_payment` object.
+    - `card_settlement` - The Transaction was created by a Card Settlement object.
+      Details will be under the `card_settlement` object.
+    - `check_deposit_acceptance` - The Transaction was created by a Check Deposit
+      Acceptance object. Details will be under the `check_deposit_acceptance`
+      object.
+    - `check_deposit_return` - The Transaction was created by a Check Deposit Return
+      object. Details will be under the `check_deposit_return` object.
+    - `check_transfer_deposit` - The Transaction was created by a Check Transfer
+      Deposit object. Details will be under the `check_transfer_deposit` object.
+    - `check_transfer_intention` - The Transaction was created by a Check Transfer
+      Intention object. Details will be under the `check_transfer_intention` object.
+    - `check_transfer_rejection` - The Transaction was created by a Check Transfer
+      Rejection object. Details will be under the `check_transfer_rejection` object.
+    - `check_transfer_stop_payment_request` - The Transaction was created by a Check
+      Transfer Stop Payment Request object. Details will be under the
+      `check_transfer_stop_payment_request` object.
+    - `fee_payment` - The Transaction was created by a Fee Payment object. Details
+      will be under the `fee_payment` object.
+    - `inbound_ach_transfer` - The Transaction was created by a Inbound ACH Transfer
+      object. Details will be under the `inbound_ach_transfer` object.
+    - `inbound_ach_transfer_return_intention` - The Transaction was created by a
+      Inbound ACH Transfer Return Intention object. Details will be under the
+      `inbound_ach_transfer_return_intention` object.
+    - `inbound_check` - The Transaction was created by a Inbound Check object.
+      Details will be under the `inbound_check` object.
+    - `inbound_international_ach_transfer` - The Transaction was created by a
+      Inbound International ACH Transfer object. Details will be under the
+      `inbound_international_ach_transfer` object.
+    - `inbound_real_time_payments_transfer_confirmation` - The Transaction was
+      created by a Inbound Real Time Payments Transfer Confirmation object. Details
+      will be under the `inbound_real_time_payments_transfer_confirmation` object.
+    - `inbound_wire_drawdown_payment` - The Transaction was created by a Inbound
+      Wire Drawdown Payment object. Details will be under the
+      `inbound_wire_drawdown_payment` object.
+    - `inbound_wire_drawdown_payment_reversal` - The Transaction was created by a
+      Inbound Wire Drawdown Payment Reversal object. Details will be under the
+      `inbound_wire_drawdown_payment_reversal` object.
+    - `inbound_wire_reversal` - The Transaction was created by a Inbound Wire
+      Reversal object. Details will be under the `inbound_wire_reversal` object.
+    - `inbound_wire_transfer` - The Transaction was created by a Inbound Wire
+      Transfer object. Details will be under the `inbound_wire_transfer` object.
+    - `interest_payment` - The Transaction was created by a Interest Payment object.
+      Details will be under the `interest_payment` object.
+    - `internal_source` - The Transaction was created by a Internal Source object.
+      Details will be under the `internal_source` object.
+    - `real_time_payments_transfer_acknowledgement` - The Transaction was created by
+      a Real Time Payments Transfer Acknowledgement object. Details will be under
+      the `real_time_payments_transfer_acknowledgement` object.
+    - `sample_funds` - The Transaction was created by a Sample Funds object. Details
+      will be under the `sample_funds` object.
+    - `wire_transfer_intention` - The Transaction was created by a Wire Transfer
+      Intention object. Details will be under the `wire_transfer_intention` object.
+    - `wire_transfer_rejection` - The Transaction was created by a Wire Transfer
+      Rejection object. Details will be under the `wire_transfer_rejection` object.
+    - `other` - The Transaction was made for an undocumented or deprecated reason.
     """
 
     check_deposit_acceptance: Optional[TransactionSourceCheckDepositAcceptance]
     """A Check Deposit Acceptance object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_acceptance`.
@@ -1521,21 +1372,14 @@
     check_transfer_rejection: Optional[TransactionSourceCheckTransferRejection]
     """A Check Transfer Rejection object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_rejection`.
     """
 
-    check_transfer_return: Optional[TransactionSourceCheckTransferReturn]
-    """A Check Transfer Return object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_return`.
-    """
-
     check_transfer_stop_payment_request: Optional[TransactionSourceCheckTransferStopPaymentRequest]
     """A Check Transfer Stop Payment Request object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_stop_payment_request`.
     """
 
@@ -1667,31 +1511,42 @@
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     Transaction's currency. This will match the currency on the Transcation's
     Account.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
-    """For a Transaction related to a transfer, this is the description you provide.
+    """An informational message describing this transaction.
 
-    For a Transaction related to a payment, this is the description the vendor
-    provides.
+    Use the fields in `source` to get more detailed information. This field appears
+    as the line-item on the statement.
     """
 
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Transaction came through."""
+    """The type of the route this Transaction came through.
+
+    - `account_number` - An Account Number.
+    - `card` - A Card.
+    """
 
     source: TransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Transaction. Note that for backwards compatibility reasons, additional
     undocumented keys may appear in this object. These should be treated as
     deprecated and will be removed in the future.
@@ -1700,29 +1555,20 @@
     type: Literal["transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `transaction`.
     """
 
 
-class InboundRealTimePaymentsTransferSimulationResult(BaseModel):
-    declined_transaction: Optional[DeclinedTransaction]
-    """
-    If the Real Time Payments Transfer attempt fails, this will contain the
-    resulting [Declined Transaction](#declined-transactions) object. The Declined
-    Transaction's `source` will be of
-    `category: inbound_real_time_payments_transfer_decline`.
-    """
-
-    transaction: Optional[Transaction]
+class WireTransferSimulation(BaseModel):
+    transaction: Transaction
     """
-    If the Real Time Payments Transfer attempt succeeds, this will contain the
-    resulting [Transaction](#transactions) object. The Transaction's `source` will
-    be of `category: inbound_real_time_payments_transfer_confirmation`.
+    If the Wire Transfer attempt succeeds, this will contain the resulting
+    [Transaction](#transactions) object. The Transaction's `source` will be of
+    `category: inbound_wire_transfer`.
     """
 
-    type: Literal["inbound_real_time_payments_transfer_simulation_result"]
+    type: Literal["inbound_wire_transfer_simulation_result"]
     """A constant representing the object's type.
 
-    For this resource it will always be
-    `inbound_real_time_payments_transfer_simulation_result`.
+    For this resource it will always be `inbound_wire_transfer_simulation_result`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py` & `increase-0.9.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/simulations/interest_payment_simulation_result.py` & `increase-0.9.0/src/increase/types/simulations/card_authorization_simulation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,578 +1,369 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
-from datetime import date, datetime
+from datetime import datetime
 from typing_extensions import Literal
 
+from ...types import shared
 from ..._models import BaseModel
 
 __all__ = [
-    "InterestPaymentSimulationResult",
-    "Transaction",
-    "TransactionSource",
-    "TransactionSourceAccountTransferIntention",
-    "TransactionSourceACHTransferIntention",
-    "TransactionSourceACHTransferRejection",
-    "TransactionSourceACHTransferReturn",
-    "TransactionSourceCardDisputeAcceptance",
-    "TransactionSourceCardRefund",
-    "TransactionSourceCardRevenuePayment",
-    "TransactionSourceCardSettlement",
-    "TransactionSourceCheckDepositAcceptance",
-    "TransactionSourceCheckDepositReturn",
-    "TransactionSourceCheckTransferDeposit",
-    "TransactionSourceCheckTransferIntention",
-    "TransactionSourceCheckTransferRejection",
-    "TransactionSourceCheckTransferReturn",
-    "TransactionSourceCheckTransferStopPaymentRequest",
-    "TransactionSourceFeePayment",
-    "TransactionSourceInboundACHTransfer",
-    "TransactionSourceInboundCheck",
-    "TransactionSourceInboundInternationalACHTransfer",
-    "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
-    "TransactionSourceInboundWireDrawdownPayment",
-    "TransactionSourceInboundWireDrawdownPaymentReversal",
-    "TransactionSourceInboundWireReversal",
-    "TransactionSourceInboundWireTransfer",
-    "TransactionSourceInterestPayment",
-    "TransactionSourceInternalSource",
-    "TransactionSourceRealTimePaymentsTransferAcknowledgement",
-    "TransactionSourceSampleFunds",
-    "TransactionSourceWireTransferIntention",
-    "TransactionSourceWireTransferRejection",
+    "CardAuthorizationSimulation",
+    "DeclinedTransaction",
+    "DeclinedTransactionSource",
+    "DeclinedTransactionSourceACHDecline",
+    "DeclinedTransactionSourceCardDecline",
+    "DeclinedTransactionSourceCardDeclineNetworkDetails",
+    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
+    "DeclinedTransactionSourceCheckDecline",
+    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
+    "DeclinedTransactionSourceInternationalACHDecline",
+    "DeclinedTransactionSourceWireDecline",
+    "PendingTransaction",
+    "PendingTransactionSource",
+    "PendingTransactionSourceAccountTransferInstruction",
+    "PendingTransactionSourceACHTransferInstruction",
+    "PendingTransactionSourceCardAuthorization",
+    "PendingTransactionSourceCardAuthorizationNetworkDetails",
+    "PendingTransactionSourceCardAuthorizationNetworkDetailsVisa",
+    "PendingTransactionSourceCheckDepositInstruction",
+    "PendingTransactionSourceCheckTransferInstruction",
+    "PendingTransactionSourceInboundFundsHold",
+    "PendingTransactionSourceRealTimePaymentsTransferInstruction",
+    "PendingTransactionSourceWireTransferInstruction",
 ]
 
 
-class TransactionSourceAccountTransferIntention(BaseModel):
+class DeclinedTransactionSourceACHDecline(BaseModel):
     amount: int
-    """The pending amount in the minor unit of the transaction's currency.
+    """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    description: str
-    """The description you chose to give the transfer."""
-
-    destination_account_id: str
-    """The identifier of the Account to where the Account Transfer was sent."""
-
-    source_account_id: str
-    """The identifier of the Account from where the Account Transfer was sent."""
-
-    transfer_id: str
-    """The identifier of the Account Transfer that led to this Pending Transaction."""
-
-
-class TransactionSourceACHTransferIntention(BaseModel):
-    account_number: str
-
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    routing_number: str
-
-    statement_descriptor: str
-
-    transfer_id: str
-    """The identifier of the ACH Transfer that led to this Transaction."""
-
-
-class TransactionSourceACHTransferRejection(BaseModel):
-    transfer_id: str
-    """The identifier of the ACH Transfer that led to this Transaction."""
+    originator_company_descriptive_date: Optional[str]
 
+    originator_company_discretionary_data: Optional[str]
 
-class TransactionSourceACHTransferReturn(BaseModel):
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the transfer was created.
-    """
+    originator_company_id: str
 
-    raw_return_reason_code: str
-    """The three character ACH return code, in the range R01 to R85."""
+    originator_company_name: str
 
-    return_reason_code: Literal[
-        "insufficient_fund",
-        "no_account",
-        "account_closed",
-        "invalid_account_number_structure",
-        "account_frozen_entry_returned_per_ofac_instruction",
+    reason: Literal[
+        "ach_route_canceled",
+        "ach_route_disabled",
+        "breaches_limit",
         "credit_entry_refused_by_receiver",
-        "unauthorized_debit_to_consumer_account_using_corporate_sec_code",
-        "corporate_customer_advised_not_authorized",
-        "payment_stopped",
-        "non_transaction_account",
-        "uncollected_funds",
-        "routing_number_check_digit_error",
-        "customer_advised_unauthorized_improper_ineligible_or_incomplete",
-        "amount_field_error",
-        "authorization_revoked_by_customer",
-        "invalid_ach_routing_number",
-        "file_record_edit_criteria",
-        "enr_invalid_individual_name",
-        "returned_per_odfi_request",
-        "limited_participation_dfi",
-        "incorrectly_coded_outbound_international_payment",
-        "account_sold_to_another_dfi",
-        "addenda_error",
-        "beneficiary_or_account_holder_deceased",
-        "customer_advised_not_within_authorization_terms",
-        "corrected_return",
-        "duplicate_entry",
         "duplicate_return",
-        "enr_duplicate_enrollment",
-        "enr_invalid_dfi_account_number",
-        "enr_invalid_individual_id_number",
-        "enr_invalid_representative_payee_indicator",
-        "enr_invalid_transaction_code",
-        "enr_return_of_enr_entry",
-        "enr_routing_number_check_digit_error",
-        "entry_not_processed_by_gateway",
-        "field_error",
-        "foreign_receiving_dfi_unable_to_settle",
-        "iat_entry_coding_error",
-        "improper_effective_entry_date",
-        "improper_source_document_source_document_presented",
-        "invalid_company_id",
-        "invalid_foreign_receiving_dfi_identification",
-        "invalid_individual_id_number",
-        "item_and_rck_entry_presented_for_payment",
-        "item_related_to_rck_entry_is_ineligible",
-        "mandatory_field_error",
-        "misrouted_dishonored_return",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
         "misrouted_return",
-        "no_errors_found",
-        "non_acceptance_of_r62_dishonored_return",
-        "non_participant_in_iat_program",
-        "permissible_return_entry",
-        "permissible_return_entry_not_accepted",
-        "rdfi_non_settlement",
-        "rdfi_participant_in_check_truncation_program",
-        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
-        "return_not_a_duplicate",
-        "return_of_erroneous_or_reversing_debit",
-        "return_of_improper_credit_entry",
-        "return_of_improper_debit_entry",
-        "return_of_xck_entry",
-        "source_document_presented_for_payment",
-        "state_law_affecting_rck_acceptance",
-        "stop_payment_on_item_related_to_rck_entry",
-        "stop_payment_on_source_document",
-        "timely_original_return",
-        "trace_number_error",
-        "untimely_dishonored_return",
-        "untimely_return",
+        "no_ach_route",
+        "originator_request",
+        "transaction_not_allowed",
     ]
-    """Why the ACH Transfer was returned."""
-
-    transaction_id: str
-    """The identifier of the Tranasaction associated with this return."""
+    """Why the ACH transfer was declined.
 
-    transfer_id: str
-    """The identifier of the ACH Transfer associated with this return."""
-
-
-class TransactionSourceCardDisputeAcceptance(BaseModel):
-    accepted_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the Card Dispute was accepted.
-    """
-
-    card_dispute_id: str
-    """The identifier of the Card Dispute that was accepted."""
-
-    transaction_id: str
-    """
-    The identifier of the Transaction that was created to return the disputed funds
-    to your account.
+    - `ach_route_canceled` - The account number is canceled.
+    - `ach_route_disabled` - The account number is disabled.
+    - `breaches_limit` - The transaction would cause a limit to be exceeded.
+    - `credit_entry_refused_by_receiver` - A credit was refused.
+    - `duplicate_return` - Other.
+    - `entity_not_active` - The account's entity is not active.
+    - `group_locked` - Your account is inactive.
+    - `insufficient_funds` - Your account contains insufficient funds.
+    - `misrouted_return` - Other.
+    - `no_ach_route` - The account number that was debited does not exist.
+    - `originator_request` - Other.
+    - `transaction_not_allowed` - The transaction is not allowed per Increase's
+      terms.
     """
 
+    receiver_id_number: Optional[str]
 
-class TransactionSourceCardRefund(BaseModel):
-    id: str
-    """The Card Refund identifier."""
-
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
+    receiver_name: Optional[str]
 
-    For dollars, for example, this is cents.
-    """
+    trace_number: str
 
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
 
-    merchant_acceptor_id: Optional[str]
+class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
+    electronic_commerce_indicator: Optional[
+        Literal[
+            "mail_phone_order",
+            "recurring",
+            "installment",
+            "unknown_mail_phone_order",
+            "secure_electronic_commerce",
+            "non_authenticated_security_transaction_at_3ds_capable_merchant",
+            "non_authenticated_security_transaction",
+            "non_secure_transaction",
+        ]
+    ]
     """
-    The merchant identifier (commonly abbreviated as MID) of the merchant the card
-    is transacting with.
+    For electronic commerce transactions, this identifies the level of security used
+    in obtaining the customer's payment credential. For mail or telephone order
+    transactions, identifies the type of mail or telephone order.
+
+    - `mail_phone_order` - Single transaction of a mail/phone order: Use to indicate
+      that the transaction is a mail/phone order purchase, not a recurring
+      transaction or installment payment. For domestic transactions in the US
+      region, this value may also indicate one bill payment transaction in the
+      card-present or card-absent environments.
+    - `recurring` - Recurring transaction: Payment indicator used to indicate a
+      recurring transaction that originates from an acquirer in the US region.
+    - `installment` - Installment payment: Payment indicator used to indicate one
+      purchase of goods or services that is billed to the account in multiple
+      charges over a period of time agreed upon by the cardholder and merchant from
+      transactions that originate from an acquirer in the US region.
+    - `unknown_mail_phone_order` - Unknown classification: other mail order: Use to
+      indicate that the type of mail/telephone order is unknown.
+    - `secure_electronic_commerce` - Secure electronic commerce transaction: Use to
+      indicate that the electronic commerce transaction has been authenticated using
+      e.g., 3-D Secure
+    - `non_authenticated_security_transaction_at_3ds_capable_merchant` -
+      Non-authenticated security transaction at a 3-D Secure-capable merchant, and
+      merchant attempted to authenticate the cardholder using 3-D Secure: Use to
+      identify an electronic commerce transaction where the merchant attempted to
+      authenticate the cardholder using 3-D Secure, but was unable to complete the
+      authentication because the issuer or cardholder does not participate in the
+      3-D Secure program.
+    - `non_authenticated_security_transaction` - Non-authenticated security
+      transaction: Use to identify an electronic commerce transaction that uses data
+      encryption for security however , cardholder authentication is not performed
+      using 3-D Secure.
+    - `non_secure_transaction` - Non-secure transaction: Use to identify an
+      electronic commerce transaction that has no data protection.
+    """
+
+    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
+    """
+    The method used to enter the cardholder's primary account number and card
+    expiration date
     """
 
-    merchant_category_code: str
-    """The 4-digit MCC describing the merchant's business."""
-
-    merchant_city: Optional[str]
-    """The city the merchant resides in."""
-
-    merchant_country: str
-    """The country the merchant resides in."""
-
-    merchant_name: Optional[str]
-    """The name of the merchant."""
 
-    merchant_state: Optional[str]
-    """The state the merchant resides in."""
-
-    type: Literal["card_refund"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `card_refund`.
-    """
+class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
+    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
+    """Fields specific to the `visa` network"""
 
 
-class TransactionSourceCardRevenuePayment(BaseModel):
+class DeclinedTransactionSourceCardDecline(BaseModel):
     amount: int
-    """The amount in the minor unit of the transaction's currency.
+    """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
-
-    period_end: datetime
-    """The end of the period for which this transaction paid interest."""
-
-    period_start: datetime
-    """The start of the period for which this transaction paid interest."""
-
-    transacted_on_account_id: Optional[str]
-    """The account the card belonged to."""
-
-
-class TransactionSourceCardSettlement(BaseModel):
-    id: str
-    """The Card Settlement identifier."""
-
-    amount: int
-    """The amount in the minor unit of the transaction's settlement currency.
-
-    For dollars, for example, this is cents.
-    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
+    account currency.
 
-    card_authorization: Optional[str]
-    """
-    The Card Authorization that was created prior to this Card Settlement, if on
-    exists.
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    digital_wallet_token_id: Optional[str]
     """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's settlement currency.
+    If the authorization was attempted using a Digital Wallet Token (such as an
+    Apple Pay purchase), the identifier of the token that was used.
     """
 
-    merchant_acceptor_id: Optional[str]
+    merchant_acceptor_id: str
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
-    merchant_category_code: str
-    """The 4-digit MCC describing the merchant's business."""
+    merchant_category_code: Optional[str]
+    """
+    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
+    card is transacting with.
+    """
 
     merchant_city: Optional[str]
     """The city the merchant resides in."""
 
-    merchant_country: str
+    merchant_country: Optional[str]
     """The country the merchant resides in."""
 
-    merchant_name: Optional[str]
-    """The name of the merchant."""
+    merchant_descriptor: str
+    """The merchant descriptor of the merchant the card is transacting with."""
 
     merchant_state: Optional[str]
     """The state the merchant resides in."""
 
-    pending_transaction_id: Optional[str]
-    """The identifier of the Pending Transaction associated with this Transaction."""
-
-    presentment_amount: int
-    """The amount in the minor unit of the transaction's presentment currency."""
+    network: Literal["visa"]
+    """The payment network used to process this card authorization
 
-    presentment_currency: str
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's presentment currency.
+    - `visa` - Visa
     """
 
-    type: Literal["card_settlement"]
-    """A constant representing the object's type.
+    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
+    """Fields specific to the `network`"""
 
-    For this resource it will always be `card_settlement`.
+    real_time_decision_id: Optional[str]
     """
-
-
-class TransactionSourceCheckDepositAcceptance(BaseModel):
-    account_number: str
-    """The account number printed on the check."""
-
-    amount: int
-    """The amount to be deposited in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    auxiliary_on_us: Optional[str]
-    """An additional line of metadata printed on the check.
-
-    This typically includes the check number for business checks.
-    """
-
-    check_deposit_id: str
-    """The ID of the Check Deposit that was accepted."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
+    The identifier of the Real-Time Decision sent to approve or decline this
+    transaction.
     """
 
-    routing_number: str
-    """The routing number printed on the check."""
-
-    serial_number: Optional[str]
-    """The check serial number, if present, for consumer checks.
+    reason: Literal[
+        "card_not_active",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
+        "cvv2_mismatch",
+        "transaction_not_allowed",
+        "breaches_internal_limit",
+        "breaches_limit",
+        "webhook_declined",
+        "webhook_timed_out",
+        "declined_by_stand_in_processing",
+        "invalid_physical_card",
+        "missing_original_authorization",
+    ]
+    """Why the transaction was declined.
 
-    For business checks, the serial number is usually in the `auxiliary_on_us`
-    field.
+    - `card_not_active` - The Card was not active.
+    - `entity_not_active` - The account's entity was not active.
+    - `group_locked` - The account was inactive.
+    - `insufficient_funds` - The Card's Account did not have a sufficient available
+      balance.
+    - `cvv2_mismatch` - The given CVV2 did not match the card's value.
+    - `transaction_not_allowed` - The attempted card transaction is not allowed per
+      Increase's terms.
+    - `breaches_internal_limit` - The transaction was blocked by an internal limit
+      for new Increase accounts.
+    - `breaches_limit` - The transaction was blocked by a Limit.
+    - `webhook_declined` - Your application declined the transaction via webhook.
+    - `webhook_timed_out` - Your application webhook did not respond without the
+      required timeout.
+    - `declined_by_stand_in_processing` - Declined by stand-in processing.
+    - `invalid_physical_card` - The card read had an invalid CVV, dCVV, or
+      authorization request cryptogram.
+    - `missing_original_authorization` - The original card authorization for this
+      incremental authorization does not exist.
     """
 
 
-class TransactionSourceCheckDepositReturn(BaseModel):
+class DeclinedTransactionSourceCheckDecline(BaseModel):
     amount: int
-    """The amount in the minor unit of the transaction's currency.
+    """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
-    check_deposit_id: str
-    """The identifier of the Check Deposit that was returned."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
+    auxiliary_on_us: Optional[str]
 
-    return_reason: Literal[
-        "ach_conversion_not_supported",
-        "closed_account",
-        "duplicate_submission",
+    reason: Literal[
+        "ach_route_canceled",
+        "ach_route_disabled",
+        "breaches_limit",
+        "entity_not_active",
+        "group_locked",
         "insufficient_funds",
-        "no_account",
+        "unable_to_locate_account",
+        "not_our_item",
+        "unable_to_process",
+        "refer_to_image",
+        "stop_payment_requested",
+        "returned",
+        "duplicate_presentment",
         "not_authorized",
-        "stale_dated",
-        "stop_payment",
-        "unknown_reason",
-        "unmatched_details",
-        "unreadable_image",
-        "endorsement_irregular",
+        "altered_or_fictitious",
     ]
+    """Why the check was declined.
 
-    returned_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the check deposit was returned.
-    """
-
-    transaction_id: str
-    """
-    The identifier of the transaction that reversed the original check deposit
-    transaction.
-    """
-
-
-class TransactionSourceCheckTransferDeposit(BaseModel):
-    back_image_file_id: Optional[str]
-    """
-    The identifier of the API File object containing an image of the back of the
-    deposited check.
-    """
-
-    deposited_at: datetime
-    """When the check was deposited."""
-
-    front_image_file_id: Optional[str]
-    """
-    The identifier of the API File object containing an image of the front of the
-    deposited check.
-    """
-
-    type: Literal["check_transfer_deposit"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `check_transfer_deposit`.
-    """
-
-
-class TransactionSourceCheckTransferIntention(BaseModel):
-    address_city: Optional[str]
-    """The city of the check's destination."""
-
-    address_line1: Optional[str]
-    """The street address of the check's destination."""
-
-    address_line2: Optional[str]
-    """The second line of the address of the check's destination."""
-
-    address_state: Optional[str]
-    """The state of the check's destination."""
-
-    address_zip: Optional[str]
-    """The postal code of the check's destination."""
-
-    amount: int
-    """The transfer amount in USD cents."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
-    currency.
-    """
-
-    recipient_name: Optional[str]
-    """The name that will be printed on the check."""
-
-    transfer_id: str
-    """The identifier of the Check Transfer with which this is associated."""
-
-
-class TransactionSourceCheckTransferRejection(BaseModel):
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Transaction."""
-
-
-class TransactionSourceCheckTransferReturn(BaseModel):
-    file_id: Optional[str]
-    """If available, a document with additional information about the return."""
-
-    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
-    """The reason why the check was returned."""
-
-    returned_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the check was returned.
-    """
-
-    transaction_id: Optional[str]
-    """
-    The identifier of the Transaction that was created to credit you for the
-    returned check.
-    """
-
-    transfer_id: str
-    """The identifier of the returned Check Transfer."""
-
-
-class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
-    requested_at: datetime
-    """The time the stop-payment was requested."""
-
-    transaction_id: str
-    """The transaction ID of the corresponding credit transaction."""
-
-    transfer_id: str
-    """The ID of the check transfer that was stopped."""
-
-    type: Literal["check_transfer_stop_payment_request"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `check_transfer_stop_payment_request`.
+    - `ach_route_canceled` - The account number is canceled.
+    - `ach_route_disabled` - The account number is disabled.
+    - `breaches_limit` - The transaction would cause a limit to be exceeded.
+    - `entity_not_active` - The account's entity is not active.
+    - `group_locked` - Your account is inactive.
+    - `insufficient_funds` - Your account contains insufficient funds.
+    - `unable_to_locate_account` - Unable to locate account.
+    - `not_our_item` - Routing number on the check is not ours.
+    - `unable_to_process` - Unable to process.
+    - `refer_to_image` - Refer to image.
+    - `stop_payment_requested` - Stop payment requested for this check.
+    - `returned` - Check was returned to sender.
+    - `duplicate_presentment` - The check was a duplicate deposit.
+    - `not_authorized` - The transaction is not allowed.
+    - `altered_or_fictitious` - The check was altered or fictitious.
     """
 
 
-class TransactionSourceFeePayment(BaseModel):
+class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
     amount: int
-    """The amount in the minor unit of the transaction's currency.
+    """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
+    creditor_name: str
+    """The name the sender of the transfer specified as the recipient of the transfer."""
+
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
-
-
-class TransactionSourceInboundACHTransfer(BaseModel):
-    amount: int
-    """The amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
+    transfer's currency. This will always be "USD" for a Real Time Payments
+    transfer.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
-    originator_company_descriptive_date: Optional[str]
-
-    originator_company_discretionary_data: Optional[str]
-
-    originator_company_entry_description: str
-
-    originator_company_id: str
-
-    originator_company_name: str
-
-    receiver_id_number: Optional[str]
-
-    receiver_name: Optional[str]
+    debtor_account_number: str
+    """The account number of the account that sent the transfer."""
 
-    trace_number: str
+    debtor_name: str
+    """The name provided by the sender of the transfer."""
 
+    debtor_routing_number: str
+    """The routing number of the account that sent the transfer."""
 
-class TransactionSourceInboundCheck(BaseModel):
-    amount: int
-    """The amount in the minor unit of the destination account currency.
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "account_restricted",
+        "group_locked",
+        "entity_not_active",
+        "real_time_payments_not_enabled",
+    ]
+    """Why the transfer was declined.
 
-    For dollars, for example, this is cents.
+    - `account_number_canceled` - The account number is canceled.
+    - `account_number_disabled` - The account number is disabled.
+    - `account_restricted` - Your account is restricted.
+    - `group_locked` - Your account is inactive.
+    - `entity_not_active` - The account's entity is not active.
+    - `real_time_payments_not_enabled` - Your account is not enabled to receive Real
+      Time Payments transfers.
     """
 
-    check_front_image_file_id: Optional[str]
-
-    check_number: Optional[str]
-
-    check_rear_image_file_id: Optional[str]
+    remittance_information: Optional[str]
+    """Additional information included with the transfer."""
 
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
+    transaction_identification: str
+    """The Real Time Payments network identification of the declined transfer."""
 
 
-class TransactionSourceInboundInternationalACHTransfer(BaseModel):
+class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
     amount: int
-    """The amount in the minor unit of the destination account currency.
+    """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     destination_country_code: str
 
     destination_currency_code: str
@@ -640,49 +431,17 @@
     receiving_depository_financial_institution_id_qualifier: str
 
     receiving_depository_financial_institution_name: str
 
     trace_number: str
 
 
-class TransactionSourceInboundRealTimePaymentsTransferConfirmation(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transfer's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    creditor_name: str
-    """The name the sender of the transfer specified as the recipient of the transfer."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the transfer's
-    currency. This will always be "USD" for a Real Time Payments transfer.
-    """
-
-    debtor_account_number: str
-    """The account number of the account that sent the transfer."""
-
-    debtor_name: str
-    """The name provided by the sender of the transfer."""
-
-    debtor_routing_number: str
-    """The routing number of the account that sent the transfer."""
-
-    remittance_information: Optional[str]
-    """Additional information included with the transfer."""
-
-    transaction_identification: str
-    """The Real Time Payments network identification of the transfer"""
-
-
-class TransactionSourceInboundWireDrawdownPayment(BaseModel):
+class DeclinedTransactionSourceWireDecline(BaseModel):
     amount: int
-    """The amount in the minor unit of the transaction's currency.
+    """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
     beneficiary_address_line1: Optional[str]
 
     beneficiary_address_line2: Optional[str]
@@ -701,552 +460,699 @@
 
     originator_address_line2: Optional[str]
 
     originator_address_line3: Optional[str]
 
     originator_name: Optional[str]
 
-    originator_to_beneficiary_information: Optional[str]
-
-
-class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
-    amount: int
-    """The amount that was reversed."""
-
-    description: str
-    """The description on the reversal message from Fedwire."""
-
-    input_cycle_date: date
-    """The Fedwire cycle date for the wire reversal."""
+    originator_to_beneficiary_information_line1: Optional[str]
 
-    input_message_accountability_data: str
-    """The Fedwire transaction identifier."""
+    originator_to_beneficiary_information_line2: Optional[str]
 
-    input_sequence_number: str
-    """The Fedwire sequence number."""
+    originator_to_beneficiary_information_line3: Optional[str]
 
-    input_source: str
-    """The Fedwire input source identifier."""
+    originator_to_beneficiary_information_line4: Optional[str]
 
-    previous_message_input_cycle_date: date
-    """The Fedwire cycle date for the wire transfer that was reversed."""
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "entity_not_active",
+        "group_locked",
+        "no_account_number",
+        "transaction_not_allowed",
+    ]
+    """Why the wire transfer was declined.
 
-    previous_message_input_message_accountability_data: str
-    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+    - `account_number_canceled` - The account number is canceled.
+    - `account_number_disabled` - The account number is disabled.
+    - `entity_not_active` - The account's entity is not active.
+    - `group_locked` - Your account is inactive.
+    - `no_account_number` - The beneficiary account number does not exist.
+    - `transaction_not_allowed` - The transaction is not allowed per Increase's
+      terms.
+    """
 
-    previous_message_input_sequence_number: str
-    """The Fedwire sequence number for the wire transfer that was reversed."""
 
-    previous_message_input_source: str
-    """The Fedwire input source identifier for the wire transfer that was reversed."""
+class DeclinedTransactionSource(BaseModel):
+    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
+    """A ACH Decline object.
 
+    This field will be present in the JSON response if and only if `category` is
+    equal to `ach_decline`.
+    """
 
-class TransactionSourceInboundWireReversal(BaseModel):
-    amount: int
-    """The amount that was reversed."""
+    card_decline: Optional[DeclinedTransactionSourceCardDecline]
+    """A Card Decline object.
 
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the reversal was created.
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_decline`.
     """
 
-    description: str
-    """The description on the reversal message from Fedwire."""
-
-    financial_institution_to_financial_institution_information: Optional[str]
-    """Additional financial institution information included in the wire reversal."""
+    category: Literal[
+        "ach_decline",
+        "card_decline",
+        "check_decline",
+        "inbound_real_time_payments_transfer_decline",
+        "international_ach_decline",
+        "wire_decline",
+        "other",
+    ]
+    """The type of decline that took place.
 
-    input_cycle_date: date
-    """The Fedwire cycle date for the wire reversal."""
+    We may add additional possible values for this enum over time; your application
+    should be able to handle such additions gracefully.
 
-    input_message_accountability_data: str
-    """The Fedwire transaction identifier."""
+    - `ach_decline` - The Declined Transaction was created by a ACH Decline object.
+      Details will be under the `ach_decline` object.
+    - `card_decline` - The Declined Transaction was created by a Card Decline
+      object. Details will be under the `card_decline` object.
+    - `check_decline` - The Declined Transaction was created by a Check Decline
+      object. Details will be under the `check_decline` object.
+    - `inbound_real_time_payments_transfer_decline` - The Declined Transaction was
+      created by a Inbound Real Time Payments Transfer Decline object. Details will
+      be under the `inbound_real_time_payments_transfer_decline` object.
+    - `international_ach_decline` - The Declined Transaction was created by a
+      International ACH Decline object. Details will be under the
+      `international_ach_decline` object.
+    - `wire_decline` - The Declined Transaction was created by a Wire Decline
+      object. Details will be under the `wire_decline` object.
+    - `other` - The Declined Transaction was made for an undocumented or deprecated
+      reason.
+    """
+
+    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
+    """A Check Decline object.
 
-    input_sequence_number: str
-    """The Fedwire sequence number."""
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_decline`.
+    """
 
-    input_source: str
-    """The Fedwire input source identifier."""
+    inbound_real_time_payments_transfer_decline: Optional[
+        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
+    ]
+    """A Inbound Real Time Payments Transfer Decline object.
 
-    previous_message_input_cycle_date: date
-    """The Fedwire cycle date for the wire transfer that was reversed."""
+    This field will be present in the JSON response if and only if `category` is
+    equal to `inbound_real_time_payments_transfer_decline`.
+    """
 
-    previous_message_input_message_accountability_data: str
-    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
+    """A International ACH Decline object.
 
-    previous_message_input_sequence_number: str
-    """The Fedwire sequence number for the wire transfer that was reversed."""
+    This field will be present in the JSON response if and only if `category` is
+    equal to `international_ach_decline`.
+    """
 
-    previous_message_input_source: str
-    """The Fedwire input source identifier for the wire transfer that was reversed."""
+    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
+    """A Wire Decline object.
 
-    receiver_financial_institution_information: Optional[str]
-    """
-    Information included in the wire reversal for the receiving financial
-    institution.
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_decline`.
     """
 
-    transaction_id: Optional[str]
-    """The ID for the Transaction associated with the transfer reversal."""
 
-    wire_transfer_id: str
-    """The ID for the Wire Transfer that is being reversed."""
+class DeclinedTransaction(BaseModel):
+    id: str
+    """The Declined Transaction identifier."""
 
+    account_id: str
+    """The identifier for the Account the Declined Transaction belongs to."""
 
-class TransactionSourceInboundWireTransfer(BaseModel):
     amount: int
-    """The amount in the minor unit of the transaction's currency.
+    """The Declined Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
     """
 
-    beneficiary_address_line1: Optional[str]
-
-    beneficiary_address_line2: Optional[str]
-
-    beneficiary_address_line3: Optional[str]
-
-    beneficiary_name: Optional[str]
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
+    Transaction occured.
+    """
 
-    beneficiary_reference: Optional[str]
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
+    Transaction's currency. This will match the currency on the Declined
+    Transcation's Account.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
+    """
 
     description: str
+    """This is the description the vendor provides."""
 
-    input_message_accountability_data: Optional[str]
-
-    originator_address_line1: Optional[str]
-
-    originator_address_line2: Optional[str]
-
-    originator_address_line3: Optional[str]
-
-    originator_name: Optional[str]
+    route_id: Optional[str]
+    """The identifier for the route this Declined Transaction came through.
 
-    originator_to_beneficiary_information: Optional[str]
+    Routes are things like cards and ACH details.
+    """
 
-    originator_to_beneficiary_information_line1: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
+    """The type of the route this Declined Transaction came through.
 
-    originator_to_beneficiary_information_line2: Optional[str]
+    - `account_number` - An Account Number.
+    - `card` - A Card.
+    """
 
-    originator_to_beneficiary_information_line3: Optional[str]
+    source: DeclinedTransactionSource
+    """
+    This is an object giving more details on the network-level event that caused the
+    Declined Transaction. For example, for a card transaction this lists the
+    merchant's industry and location. Note that for backwards compatibility reasons,
+    additional undocumented keys may appear in this object. These should be treated
+    as deprecated and will be removed in the future.
+    """
 
-    originator_to_beneficiary_information_line4: Optional[str]
+    type: Literal["declined_transaction"]
+    """A constant representing the object's type.
 
+    For this resource it will always be `declined_transaction`.
+    """
 
-class TransactionSourceInterestPayment(BaseModel):
-    accrued_on_account_id: Optional[str]
-    """The account on which the interest was accrued."""
 
+class PendingTransactionSourceAccountTransferInstruction(BaseModel):
     amount: int
-    """The amount in the minor unit of the transaction's currency.
+    """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
+    account currency.
 
-    period_end: datetime
-    """The end of the period for which this transaction paid interest."""
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
+    """
 
-    period_start: datetime
-    """The start of the period for which this transaction paid interest."""
+    transfer_id: str
+    """The identifier of the Account Transfer that led to this Pending Transaction."""
 
 
-class TransactionSourceInternalSource(BaseModel):
+class PendingTransactionSourceACHTransferInstruction(BaseModel):
     amount: int
-    """The amount in the minor unit of the transaction's currency.
+    """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    transfer_id: str
+    """The identifier of the ACH Transfer that led to this Pending Transaction."""
+
+
+class PendingTransactionSourceCardAuthorizationNetworkDetailsVisa(BaseModel):
+    electronic_commerce_indicator: Optional[
+        Literal[
+            "mail_phone_order",
+            "recurring",
+            "installment",
+            "unknown_mail_phone_order",
+            "secure_electronic_commerce",
+            "non_authenticated_security_transaction_at_3ds_capable_merchant",
+            "non_authenticated_security_transaction",
+            "non_secure_transaction",
+        ]
+    ]
     """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
+    For electronic commerce transactions, this identifies the level of security used
+    in obtaining the customer's payment credential. For mail or telephone order
+    transactions, identifies the type of mail or telephone order.
+
+    - `mail_phone_order` - Single transaction of a mail/phone order: Use to indicate
+      that the transaction is a mail/phone order purchase, not a recurring
+      transaction or installment payment. For domestic transactions in the US
+      region, this value may also indicate one bill payment transaction in the
+      card-present or card-absent environments.
+    - `recurring` - Recurring transaction: Payment indicator used to indicate a
+      recurring transaction that originates from an acquirer in the US region.
+    - `installment` - Installment payment: Payment indicator used to indicate one
+      purchase of goods or services that is billed to the account in multiple
+      charges over a period of time agreed upon by the cardholder and merchant from
+      transactions that originate from an acquirer in the US region.
+    - `unknown_mail_phone_order` - Unknown classification: other mail order: Use to
+      indicate that the type of mail/telephone order is unknown.
+    - `secure_electronic_commerce` - Secure electronic commerce transaction: Use to
+      indicate that the electronic commerce transaction has been authenticated using
+      e.g., 3-D Secure
+    - `non_authenticated_security_transaction_at_3ds_capable_merchant` -
+      Non-authenticated security transaction at a 3-D Secure-capable merchant, and
+      merchant attempted to authenticate the cardholder using 3-D Secure: Use to
+      identify an electronic commerce transaction where the merchant attempted to
+      authenticate the cardholder using 3-D Secure, but was unable to complete the
+      authentication because the issuer or cardholder does not participate in the
+      3-D Secure program.
+    - `non_authenticated_security_transaction` - Non-authenticated security
+      transaction: Use to identify an electronic commerce transaction that uses data
+      encryption for security however , cardholder authentication is not performed
+      using 3-D Secure.
+    - `non_secure_transaction` - Non-secure transaction: Use to identify an
+      electronic commerce transaction that has no data protection.
+    """
+
+    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
+    """
+    The method used to enter the cardholder's primary account number and card
+    expiration date
     """
 
-    reason: Literal[
-        "account_closure",
-        "bank_migration",
-        "cashback",
-        "collection_receivable",
-        "empyreal_adjustment",
-        "error",
-        "error_correction",
-        "fees",
-        "interest",
-        "negative_balance_forgiveness",
-        "sample_funds",
-        "sample_funds_return",
-    ]
 
+class PendingTransactionSourceCardAuthorizationNetworkDetails(BaseModel):
+    visa: PendingTransactionSourceCardAuthorizationNetworkDetailsVisa
+    """Fields specific to the `visa` network"""
 
-class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
-    amount: int
-    """The transfer amount in USD cents."""
 
-    destination_account_number: str
-    """The destination account number."""
+class PendingTransactionSourceCardAuthorization(BaseModel):
+    id: str
+    """The Card Authorization identifier."""
 
-    destination_routing_number: str
-    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
 
-    remittance_information: str
-    """Unstructured information that will show on the recipient's bank statement."""
+    For dollars, for example, this is cents.
+    """
 
-    transfer_id: str
-    """The identifier of the Real Time Payments Transfer that led to this Transaction."""
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
+    transaction's currency.
 
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
+    """
 
-class TransactionSourceSampleFunds(BaseModel):
-    originator: str
-    """Where the sample funds came from."""
+    digital_wallet_token_id: Optional[str]
+    """
+    If the authorization was made via a Digital Wallet Token (such as an Apple Pay
+    purchase), the identifier of the token that was used.
+    """
 
+    expires_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) when this authorization
+    will expire and the pending transaction will be released.
+    """
 
-class TransactionSourceWireTransferIntention(BaseModel):
-    account_number: str
-    """The destination account number."""
+    merchant_acceptor_id: str
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
 
-    amount: int
-    """The transfer amount in USD cents."""
+    merchant_category_code: Optional[str]
+    """
+    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
+    card is transacting with.
+    """
 
-    message_to_recipient: str
-    """The message that will show on the recipient's bank statement."""
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
 
-    routing_number: str
-    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
+    merchant_country: Optional[str]
+    """The country the merchant resides in."""
 
-    transfer_id: str
+    merchant_descriptor: str
+    """The merchant descriptor of the merchant the card is transacting with."""
 
+    network: Literal["visa"]
+    """The payment network used to process this card authorization
 
-class TransactionSourceWireTransferRejection(BaseModel):
-    transfer_id: str
+    - `visa` - Visa
+    """
 
+    network_details: PendingTransactionSourceCardAuthorizationNetworkDetails
+    """Fields specific to the `network`"""
 
-class TransactionSource(BaseModel):
-    account_transfer_intention: Optional[TransactionSourceAccountTransferIntention]
-    """A Account Transfer Intention object.
+    pending_transaction_id: Optional[str]
+    """The identifier of the Pending Transaction associated with this Transaction."""
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `account_transfer_intention`.
+    real_time_decision_id: Optional[str]
     """
-
-    ach_transfer_intention: Optional[TransactionSourceACHTransferIntention]
-    """A ACH Transfer Intention object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_transfer_intention`.
+    The identifier of the Real-Time Decision sent to approve or decline this
+    transaction.
     """
 
-    ach_transfer_rejection: Optional[TransactionSourceACHTransferRejection]
-    """A ACH Transfer Rejection object.
+    type: Literal["card_authorization"]
+    """A constant representing the object's type.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_transfer_rejection`.
+    For this resource it will always be `card_authorization`.
     """
 
-    ach_transfer_return: Optional[TransactionSourceACHTransferReturn]
-    """A ACH Transfer Return object.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_transfer_return`.
-    """
+class PendingTransactionSourceCheckDepositInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
 
-    card_dispute_acceptance: Optional[TransactionSourceCardDisputeAcceptance]
-    """A Card Dispute Acceptance object.
+    For dollars, for example, this is cents.
+    """
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_dispute_acceptance`.
+    back_image_file_id: Optional[str]
+    """
+    The identifier of the File containing the image of the back of the check that
+    was deposited.
     """
 
-    card_refund: Optional[TransactionSourceCardRefund]
-    """A Card Refund object.
+    check_deposit_id: Optional[str]
+    """The identifier of the Check Deposit."""
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_refund`.
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
+    transaction's currency.
 
-    card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
-    """A Card Revenue Payment object.
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
+    """
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_revenue_payment`.
+    front_image_file_id: str
+    """
+    The identifier of the File containing the image of the front of the check that
+    was deposited.
     """
 
-    card_settlement: Optional[TransactionSourceCardSettlement]
-    """A Card Settlement object.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_settlement`.
+class PendingTransactionSourceCheckTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
     """
 
-    category: Literal[
-        "account_transfer_intention",
-        "ach_transfer_intention",
-        "ach_transfer_rejection",
-        "ach_transfer_return",
-        "card_dispute_acceptance",
-        "card_refund",
-        "card_revenue_payment",
-        "card_settlement",
-        "check_deposit_acceptance",
-        "check_deposit_return",
-        "check_transfer_deposit",
-        "check_transfer_intention",
-        "check_transfer_rejection",
-        "check_transfer_return",
-        "check_transfer_stop_payment_request",
-        "fee_payment",
-        "inbound_ach_transfer",
-        "inbound_ach_transfer_return_intention",
-        "inbound_check",
-        "inbound_international_ach_transfer",
-        "inbound_real_time_payments_transfer_confirmation",
-        "inbound_wire_drawdown_payment",
-        "inbound_wire_drawdown_payment_reversal",
-        "inbound_wire_reversal",
-        "inbound_wire_transfer",
-        "interest_payment",
-        "internal_source",
-        "real_time_payments_transfer_acknowledgement",
-        "sample_funds",
-        "wire_transfer_intention",
-        "wire_transfer_rejection",
-        "other",
-    ]
-    """The type of transaction that took place.
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
+    currency.
 
-    We may add additional possible values for this enum over time; your application
-    should be able to handle such additions gracefully.
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
-    check_deposit_acceptance: Optional[TransactionSourceCheckDepositAcceptance]
-    """A Check Deposit Acceptance object.
+    transfer_id: str
+    """The identifier of the Check Transfer that led to this Pending Transaction."""
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_deposit_acceptance`.
-    """
 
-    check_deposit_return: Optional[TransactionSourceCheckDepositReturn]
-    """A Check Deposit Return object.
+class PendingTransactionSourceInboundFundsHold(BaseModel):
+    amount: int
+    """The held amount in the minor unit of the account's currency.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_deposit_return`.
+    For dollars, for example, this is cents.
     """
 
-    check_transfer_deposit: Optional[TransactionSourceCheckTransferDeposit]
-    """A Check Transfer Deposit object.
+    automatically_releases_at: datetime
+    """When the hold will be released automatically.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_deposit`.
+    Certain conditions may cause it to be released before this time.
     """
 
-    check_transfer_intention: Optional[TransactionSourceCheckTransferIntention]
-    """A Check Transfer Intention object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_intention`.
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the hold
+    was created.
     """
 
-    check_transfer_rejection: Optional[TransactionSourceCheckTransferRejection]
-    """A Check Transfer Rejection object.
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the hold's
+    currency.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_rejection`.
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
-    check_transfer_return: Optional[TransactionSourceCheckTransferReturn]
-    """A Check Transfer Return object.
+    held_transaction_id: Optional[str]
+    """The ID of the Transaction for which funds were held."""
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_return`.
-    """
+    pending_transaction_id: Optional[str]
+    """The ID of the Pending Transaction representing the held funds."""
 
-    check_transfer_stop_payment_request: Optional[TransactionSourceCheckTransferStopPaymentRequest]
-    """A Check Transfer Stop Payment Request object.
+    released_at: Optional[datetime]
+    """When the hold was released (if it has been released)."""
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_stop_payment_request`.
+    status: Literal["held", "complete"]
+    """The status of the hold.
+
+    - `held` - Funds are still being held.
+    - `complete` - Funds have been released.
     """
 
-    fee_payment: Optional[TransactionSourceFeePayment]
-    """A Fee Payment object.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `fee_payment`.
-    """
+class PendingTransactionSourceRealTimePaymentsTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
 
-    inbound_ach_transfer: Optional[TransactionSourceInboundACHTransfer]
-    """A Inbound ACH Transfer object.
+    For dollars, for example, this is cents.
+    """
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_ach_transfer`.
+    transfer_id: str
+    """
+    The identifier of the Real Time Payments Transfer that led to this Pending
+    Transaction.
     """
 
-    inbound_check: Optional[TransactionSourceInboundCheck]
-    """A Inbound Check object.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_check`.
-    """
+class PendingTransactionSourceWireTransferInstruction(BaseModel):
+    account_number: str
 
-    inbound_international_ach_transfer: Optional[TransactionSourceInboundInternationalACHTransfer]
-    """A Inbound International ACH Transfer object.
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_international_ach_transfer`.
+    For dollars, for example, this is cents.
     """
 
-    inbound_real_time_payments_transfer_confirmation: Optional[
-        TransactionSourceInboundRealTimePaymentsTransferConfirmation
-    ]
-    """A Inbound Real Time Payments Transfer Confirmation object.
+    message_to_recipient: str
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_real_time_payments_transfer_confirmation`.
-    """
+    routing_number: str
 
-    inbound_wire_drawdown_payment: Optional[TransactionSourceInboundWireDrawdownPayment]
-    """A Inbound Wire Drawdown Payment object.
+    transfer_id: str
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_wire_drawdown_payment`.
-    """
 
-    inbound_wire_drawdown_payment_reversal: Optional[TransactionSourceInboundWireDrawdownPaymentReversal]
-    """A Inbound Wire Drawdown Payment Reversal object.
+class PendingTransactionSource(BaseModel):
+    account_transfer_instruction: Optional[PendingTransactionSourceAccountTransferInstruction]
+    """A Account Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_wire_drawdown_payment_reversal`.
+    equal to `account_transfer_instruction`.
     """
 
-    inbound_wire_reversal: Optional[TransactionSourceInboundWireReversal]
-    """A Inbound Wire Reversal object.
+    ach_transfer_instruction: Optional[PendingTransactionSourceACHTransferInstruction]
+    """A ACH Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_wire_reversal`.
+    equal to `ach_transfer_instruction`.
     """
 
-    inbound_wire_transfer: Optional[TransactionSourceInboundWireTransfer]
-    """A Inbound Wire Transfer object.
+    card_authorization: Optional[PendingTransactionSourceCardAuthorization]
+    """A Card Authorization object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_wire_transfer`.
+    equal to `card_authorization`.
     """
 
-    interest_payment: Optional[TransactionSourceInterestPayment]
-    """A Interest Payment object.
+    category: Literal[
+        "account_transfer_instruction",
+        "ach_transfer_instruction",
+        "card_authorization",
+        "check_deposit_instruction",
+        "check_transfer_instruction",
+        "inbound_funds_hold",
+        "real_time_payments_transfer_instruction",
+        "wire_transfer_instruction",
+        "other",
+    ]
+    """The type of transaction that took place.
+
+    We may add additional possible values for this enum over time; your application
+    should be able to handle such additions gracefully.
 
-    This field will be present in the JSON response if and only if `category` is
-    equal to `interest_payment`.
+    - `account_transfer_instruction` - The Pending Transaction was created by a
+      Account Transfer Instruction object. Details will be under the
+      `account_transfer_instruction` object.
+    - `ach_transfer_instruction` - The Pending Transaction was created by a ACH
+      Transfer Instruction object. Details will be under the
+      `ach_transfer_instruction` object.
+    - `card_authorization` - The Pending Transaction was created by a Card
+      Authorization object. Details will be under the `card_authorization` object.
+    - `check_deposit_instruction` - The Pending Transaction was created by a Check
+      Deposit Instruction object. Details will be under the
+      `check_deposit_instruction` object.
+    - `check_transfer_instruction` - The Pending Transaction was created by a Check
+      Transfer Instruction object. Details will be under the
+      `check_transfer_instruction` object.
+    - `inbound_funds_hold` - The Pending Transaction was created by a Inbound Funds
+      Hold object. Details will be under the `inbound_funds_hold` object.
+    - `real_time_payments_transfer_instruction` - The Pending Transaction was
+      created by a Real Time Payments Transfer Instruction object. Details will be
+      under the `real_time_payments_transfer_instruction` object.
+    - `wire_transfer_instruction` - The Pending Transaction was created by a Wire
+      Transfer Instruction object. Details will be under the
+      `wire_transfer_instruction` object.
+    - `other` - The Pending Transaction was made for an undocumented or deprecated
+      reason.
     """
 
-    internal_source: Optional[TransactionSourceInternalSource]
-    """A Internal Source object.
+    check_deposit_instruction: Optional[PendingTransactionSourceCheckDepositInstruction]
+    """A Check Deposit Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `internal_source`.
+    equal to `check_deposit_instruction`.
     """
 
-    real_time_payments_transfer_acknowledgement: Optional[TransactionSourceRealTimePaymentsTransferAcknowledgement]
-    """A Real Time Payments Transfer Acknowledgement object.
+    check_transfer_instruction: Optional[PendingTransactionSourceCheckTransferInstruction]
+    """A Check Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `real_time_payments_transfer_acknowledgement`.
+    equal to `check_transfer_instruction`.
     """
 
-    sample_funds: Optional[TransactionSourceSampleFunds]
-    """A Sample Funds object.
+    inbound_funds_hold: Optional[PendingTransactionSourceInboundFundsHold]
+    """A Inbound Funds Hold object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `sample_funds`.
+    equal to `inbound_funds_hold`.
     """
 
-    wire_transfer_intention: Optional[TransactionSourceWireTransferIntention]
-    """A Wire Transfer Intention object.
+    real_time_payments_transfer_instruction: Optional[PendingTransactionSourceRealTimePaymentsTransferInstruction]
+    """A Real Time Payments Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `wire_transfer_intention`.
+    equal to `real_time_payments_transfer_instruction`.
     """
 
-    wire_transfer_rejection: Optional[TransactionSourceWireTransferRejection]
-    """A Wire Transfer Rejection object.
+    wire_transfer_instruction: Optional[PendingTransactionSourceWireTransferInstruction]
+    """A Wire Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
-    equal to `wire_transfer_rejection`.
+    equal to `wire_transfer_instruction`.
     """
 
 
-class Transaction(BaseModel):
+class PendingTransaction(BaseModel):
     id: str
-    """The Transaction identifier."""
+    """The Pending Transaction identifier."""
 
     account_id: str
-    """The identifier for the Account the Transaction belongs to."""
+    """The identifier for the account this Pending Transaction belongs to."""
 
     amount: int
-    """The Transaction amount in the minor unit of its currency.
+    """The Pending Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
     """
 
+    completed_at: Optional[datetime]
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
+    Transaction was completed.
+    """
+
     created_at: datetime
     """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
     Transaction occured.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    Transaction's currency. This will match the currency on the Transcation's
-    Account.
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Pending
+    Transaction's currency. This will match the currency on the Pending
+    Transcation's Account.
+
+    - `CAD` - Canadian Dollar (CAD)
+    - `CHF` - Swiss Franc (CHF)
+    - `EUR` - Euro (EUR)
+    - `GBP` - British Pound (GBP)
+    - `JPY` - Japanese Yen (JPY)
+    - `USD` - US Dollar (USD)
     """
 
     description: str
-    """For a Transaction related to a transfer, this is the description you provide.
-
-    For a Transaction related to a payment, this is the description the vendor
-    provides.
+    """
+    For a Pending Transaction related to a transfer, this is the description you
+    provide. For a Pending Transaction related to a payment, this is the description
+    the vendor provides.
     """
 
     route_id: Optional[str]
-    """The identifier for the route this Transaction came through.
+    """The identifier for the route this Pending Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Transaction came through."""
+    """The type of the route this Pending Transaction came through.
+
+    - `account_number` - An Account Number.
+    - `card` - A Card.
+    """
 
-    source: TransactionSource
+    source: PendingTransactionSource
     """
     This is an object giving more details on the network-level event that caused the
-    Transaction. Note that for backwards compatibility reasons, additional
-    undocumented keys may appear in this object. These should be treated as
-    deprecated and will be removed in the future.
+    Pending Transaction. For example, for a card transaction this lists the
+    merchant's industry and location.
     """
 
-    type: Literal["transaction"]
+    status: Literal["pending", "complete"]
+    """
+    Whether the Pending Transaction has been confirmed and has an associated
+    Transaction.
+
+    - `pending` - The Pending Transaction is still awaiting confirmation.
+    - `complete` - The Pending Transaction is confirmed. An associated Transaction
+      exists for this object. The Pending Transaction will no longer count against
+      your balance and can generally be hidden from UIs, etc.
+    """
+
+    type: Literal["pending_transaction"]
     """A constant representing the object's type.
 
-    For this resource it will always be `transaction`.
+    For this resource it will always be `pending_transaction`.
     """
 
 
-class InterestPaymentSimulationResult(BaseModel):
-    transaction: Transaction
-    """This will contain the resulting [Transaction](#transactions) object.
+class CardAuthorizationSimulation(BaseModel):
+    declined_transaction: Optional[DeclinedTransaction]
+    """
+    If the authorization attempt fails, this will contain the resulting
+    [Declined Transaction](#declined-transactions) object. The Declined
+    Transaction's `source` will be of `category: card_decline`.
+    """
 
-    The Transaction's `source` will be of `category: interest_payment`.
+    pending_transaction: Optional[PendingTransaction]
+    """
+    If the authorization attempt succeeds, this will contain the resulting Pending
+    Transaction object. The Pending Transaction's `source` will be of
+    `category: card_authorization`.
     """
 
-    type: Literal["interest_payment_simulation_result"]
+    type: Literal["inbound_card_authorization_simulation_result"]
     """A constant representing the object's type.
 
-    For this resource it will always be `interest_payment_simulation_result`.
+    For this resource it will always be
+    `inbound_card_authorization_simulation_result`.
     """
```

### Comparing `increase-0.8.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py` & `increase-0.9.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py` & `increase-0.9.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/transaction_list_params.py` & `increase-0.9.0/src/increase/types/transaction_list_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,14 @@
                 "card_revenue_payment",
                 "card_settlement",
                 "check_deposit_acceptance",
                 "check_deposit_return",
                 "check_transfer_deposit",
                 "check_transfer_intention",
                 "check_transfer_rejection",
-                "check_transfer_return",
                 "check_transfer_stop_payment_request",
                 "fee_payment",
                 "inbound_ach_transfer",
                 "inbound_ach_transfer_return_intention",
                 "inbound_check",
                 "inbound_international_ach_transfer",
                 "inbound_real_time_payments_transfer_confirmation",
```

### Comparing `increase-0.8.1/src/increase/types/wire_drawdown_request.py` & `increase-0.9.0/src/increase/types/wire_drawdown_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,15 +59,23 @@
     recipient_name: Optional[str]
     """The drawdown request's recipient's name."""
 
     recipient_routing_number: str
     """The drawdown request's recipient's routing number."""
 
     status: Literal["pending_submission", "pending_response", "fulfilled", "refused"]
-    """The lifecycle status of the drawdown request."""
+    """The lifecycle status of the drawdown request.
+
+    - `pending_submission` - The drawdown request is queued to be submitted to
+      Fedwire.
+    - `pending_response` - The drawdown request has been sent and the recipient
+      should respond in some way.
+    - `fulfilled` - The drawdown request has been fulfilled by the recipient.
+    - `refused` - The drawdown request has been refused by the recipient.
+    """
 
     submission: Optional[Submission]
     """
     After the drawdown request is submitted to Fedwire, this will contain
     supplemental details.
     """
```

### Comparing `increase-0.8.1/src/increase/types/wire_drawdown_request_create_params.py` & `increase-0.9.0/src/increase/types/wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/wire_transfer_create_params.py` & `increase-0.9.0/src/increase/types/wire_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.1/src/increase/types/wire_transfer_list_params.py` & `increase-0.9.0/src/increase/types/account_list_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Union
 from datetime import datetime
-from typing_extensions import Annotated, TypedDict
+from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["WireTransferListParams", "CreatedAt"]
+__all__ = ["AccountListParams", "CreatedAt"]
 
 
-class WireTransferListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Wire Transfers to those belonging to the specified Account."""
-
+class AccountListParams(TypedDict, total=False):
     created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
-    external_account_id: str
-    """Filter Wire Transfers to those made to the specified External Account."""
+    entity_id: str
+    """Filter Accounts for those belonging to the specified Entity."""
+
+    informational_entity_id: str
+    """Filter Accounts for those belonging to the specified Entity as informational."""
 
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
+    status: Literal["open", "closed"]
+    """Filter Accounts for those with the specified status.
+
+    - `open` - Open Accounts that are ready to use.
+    - `closed` - Closed Accounts on which no new activity can occur.
+    """
+
 
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
```

### Comparing `increase-0.8.1/PKG-INFO` & `increase-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increase
-Version: 0.8.1
+Version: 0.9.0
 Summary: Client library for the increase API
 Home-page: https://github.com/increase/increase-python
 License: Apache-2.0
 Author: Increase
 Author-email: dev-feedback@increase.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

