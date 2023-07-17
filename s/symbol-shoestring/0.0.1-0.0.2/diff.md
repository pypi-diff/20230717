# Comparing `tmp/symbol_shoestring-0.0.1.tar.gz` & `tmp/symbol_shoestring-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol_shoestring-0.0.1.tar", max compression
+gzip compressed data, was "symbol_shoestring-0.0.2.tar", max compression
```

## Comparing `symbol_shoestring-0.0.1.tar` & `symbol_shoestring-0.0.2.tar`

### file list

```diff
@@ -1,72 +1,79 @@
--rw-r--r--   0        0        0     9931 2023-07-12 01:51:37.859111 symbol_shoestring-0.0.1/README.md
--rw-r--r--   0        0        0      736 2023-07-14 17:23:57.684532 symbol_shoestring-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/__main__.py
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/commands/__init__.py
--rw-r--r--   0        0        0     1552 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/commands/announce_transaction.py
--rw-r--r--   0        0        0     2491 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/commands/health.py
--rw-r--r--   0        0        0     1262 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.1/shoestring/commands/import_bootstrap.py
--rw-r--r--   0        0        0     1025 2023-07-12 01:51:37.859111 symbol_shoestring-0.0.1/shoestring/commands/init.py
--rw-r--r--   0        0        0     1692 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.1/shoestring/commands/min_cosignatures_count.py
--rw-r--r--   0        0        0     1733 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/commands/pemtool.py
--rw-r--r--   0        0        0     1569 2023-07-04 16:02:45.782811 symbol_shoestring-0.0.1/shoestring/commands/renew_certificates.py
--rw-r--r--   0        0        0     5270 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/commands/renew_voting_keys.py
--rw-r--r--   0        0        0     3071 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.1/shoestring/commands/reset_data.py
--rw-r--r--   0        0        0     5330 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/commands/setup.py
--rw-r--r--   0        0        0     3367 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/commands/signer.py
--rw-r--r--   0        0        0     2246 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/commands/upgrade.py
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/healthagents/__init__.py
--rw-r--r--   0        0        0      594 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/healthagents/peer_api.py
--rw-r--r--   0        0        0     3586 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/healthagents/peer_certificate.py
--rw-r--r--   0        0        0      644 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/healthagents/rest_api.py
--rw-r--r--   0        0        0     1901 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/healthagents/rest_https_certificate.py
--rw-r--r--   0        0        0     1686 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/healthagents/voting_keys.py
--rw-r--r--   0        0        0     1573 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/healthagents/websockets.py
--rw-r--r--   0        0        0     5055 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/CertificateFactory.py
--rw-r--r--   0        0        0     3233 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/ConfigurationManager.py
--rw-r--r--   0        0        0     1656 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/FileDownloader.py
--rw-r--r--   0        0        0      360 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/FileTemplater.py
--rw-r--r--   0        0        0     1961 2023-07-04 16:02:45.782811 symbol_shoestring-0.0.1/shoestring/internal/HarvesterConfigurator.py
--rw-r--r--   0        0        0      830 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/HeightGrouping.py
--rw-r--r--   0        0        0     3089 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/LinkTransactionBuilder.py
--rw-r--r--   0        0        0      655 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/MultisigAnalyzer.py
--rw-r--r--   0        0        0     2789 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/NodeDownloader.py
--rw-r--r--   0        0        0      578 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/NodeFeatures.py
--rw-r--r--   0        0        0     1412 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/NodewatchClient.py
--rw-r--r--   0        0        0     1356 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/OpensslExecutor.py
--rw-r--r--   0        0        0     3050 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/PackageResolver.py
--rw-r--r--   0        0        0     2139 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/PeerDownloader.py
--rw-r--r--   0        0        0     2372 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/PemUtils.py
--rw-r--r--   0        0        0    12792 2023-07-04 16:02:45.782811 symbol_shoestring-0.0.1/shoestring/internal/Preparer.py
--rw-r--r--   0        0        0     3509 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.1/shoestring/internal/ShoestringConfiguration.py
--rw-r--r--   0        0        0      371 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/TransactionSerializer.py
--rw-r--r--   0        0        0     3947 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.1/shoestring/internal/VoterConfigurator.py
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.1/shoestring/internal/__init__.py
--rw-r--r--   0        0        0     1004 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/Screen.py
--rw-r--r--   0        0        0     2094 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/Screens.py
--rw-r--r--   0        0        0     1781 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/ShoestringOperation.py
--rw-r--r--   0        0        0     4647 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/TabbedView.py
--rw-r--r--   0        0        0      843 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/TitleBar.py
--rw-r--r--   0        0        0     2708 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/ValidatingTextBox.py
--rw-r--r--   0        0        0        0 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/__init__.py
--rw-r--r--   0        0        0     3575 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/__main__.py
--rw-r--r--   0        0        0     1970 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/buttons.py
--rw-r--r--   0        0        0      484 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/keybindings.py
--rw-r--r--   0        0        0     1553 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/navigation.py
--rw-r--r--   0        0        0     1635 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/screen_loader.py
--rw-r--r--   0        0        0        0 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/screens/__init__.py
--rw-r--r--   0        0        0     1890 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/screens/certificates.py
--rw-r--r--   0        0        0      652 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/screens/end_screen.py
--rw-r--r--   0        0        0     6536 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/screens/harvesting.py
--rw-r--r--   0        0        0     1625 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.1/shoestring/wizard/screens/modal.py
--rw-r--r--   0        0        0      799 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/screens/network_type.py
--rw-r--r--   0        0        0     2981 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/screens/node_settings.py
--rw-r--r--   0        0        0      757 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/screens/node_type.py
--rw-r--r--   0        0        0     6862 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/screens/obligatory.py
--rw-r--r--   0        0        0      827 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/screens/root_check.py
--rw-r--r--   0        0        0      799 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/screens/voting.py
--rw-r--r--   0        0        0     1835 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/screens/welcome.py
--rw-r--r--   0        0        0     3810 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/setup_file_generator.py
--rw-r--r--   0        0        0     1744 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/shoestring_dispatcher.py
--rw-r--r--   0        0        0     1095 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.1/shoestring/wizard/styles.py
--rw-r--r--   0        0        0    11183 1970-01-01 00:00:00.000000 symbol_shoestring-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9931 2023-07-12 01:51:37.859111 symbol_shoestring-0.0.2/README.md
+-rw-r--r--   0        0        0    25496 2023-07-17 14:34:37.741471 symbol_shoestring-0.0.2/lang/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    19551 2023-07-17 14:34:37.861482 symbol_shoestring-0.0.2/lang/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    18739 2023-07-17 14:34:37.601460 symbol_shoestring-0.0.2/lang/messages.pot
+-rw-r--r--   0        0        0      169 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/lang/po.header.txt
+-rw-r--r--   0        0        0      582 2023-07-17 15:25:15.924739 symbol_shoestring-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-17 15:22:51.737379 symbol_shoestring-0.0.2/shoestring/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/__init__.py
+-rw-r--r--   0        0        0     1552 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/announce_transaction.py
+-rw-r--r--   0        0        0     2491 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/health.py
+-rw-r--r--   0        0        0     1262 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/commands/import_bootstrap.py
+-rw-r--r--   0        0        0     1025 2023-07-12 01:51:37.859111 symbol_shoestring-0.0.2/shoestring/commands/init.py
+-rw-r--r--   0        0        0     1692 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/commands/min_cosignatures_count.py
+-rw-r--r--   0        0        0     1733 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/pemtool.py
+-rw-r--r--   0        0        0     1569 2023-07-04 16:02:45.782811 symbol_shoestring-0.0.2/shoestring/commands/renew_certificates.py
+-rw-r--r--   0        0        0     5270 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/renew_voting_keys.py
+-rw-r--r--   0        0        0     3071 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/commands/reset_data.py
+-rw-r--r--   0        0        0     5330 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/commands/setup.py
+-rw-r--r--   0        0        0     3367 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/signer.py
+-rw-r--r--   0        0        0     2246 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/upgrade.py
+-rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/__init__.py
+-rw-r--r--   0        0        0      594 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/peer_api.py
+-rw-r--r--   0        0        0     3586 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/peer_certificate.py
+-rw-r--r--   0        0        0      644 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/rest_api.py
+-rw-r--r--   0        0        0     1901 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/rest_https_certificate.py
+-rw-r--r--   0        0        0     1686 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/voting_keys.py
+-rw-r--r--   0        0        0     1573 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/websockets.py
+-rw-r--r--   0        0        0     5055 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/CertificateFactory.py
+-rw-r--r--   0        0        0     3233 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/ConfigurationManager.py
+-rw-r--r--   0        0        0     1656 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/FileDownloader.py
+-rw-r--r--   0        0        0      360 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/FileTemplater.py
+-rw-r--r--   0        0        0     1961 2023-07-04 16:02:45.782811 symbol_shoestring-0.0.2/shoestring/internal/HarvesterConfigurator.py
+-rw-r--r--   0        0        0      830 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/HeightGrouping.py
+-rw-r--r--   0        0        0     3089 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/LinkTransactionBuilder.py
+-rw-r--r--   0        0        0      655 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/MultisigAnalyzer.py
+-rw-r--r--   0        0        0     2789 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/NodeDownloader.py
+-rw-r--r--   0        0        0      578 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/NodeFeatures.py
+-rw-r--r--   0        0        0     1412 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/NodewatchClient.py
+-rw-r--r--   0        0        0     1356 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/OpensslExecutor.py
+-rw-r--r--   0        0        0     3050 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/PackageResolver.py
+-rw-r--r--   0        0        0     2139 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/PeerDownloader.py
+-rw-r--r--   0        0        0     2372 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/PemUtils.py
+-rw-r--r--   0        0        0    12610 2023-07-17 14:33:58.342037 symbol_shoestring-0.0.2/shoestring/internal/Preparer.py
+-rw-r--r--   0        0        0     3509 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/internal/ShoestringConfiguration.py
+-rw-r--r--   0        0        0      371 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/TransactionSerializer.py
+-rw-r--r--   0        0        0     3947 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/internal/VoterConfigurator.py
+-rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/__init__.py
+-rw-r--r--   0        0        0     1004 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/Screen.py
+-rw-r--r--   0        0        0     2094 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/Screens.py
+-rw-r--r--   0        0        0     1781 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/ShoestringOperation.py
+-rw-r--r--   0        0        0     4647 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/TabbedView.py
+-rw-r--r--   0        0        0      843 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/TitleBar.py
+-rw-r--r--   0        0        0     2708 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/ValidatingTextBox.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/__init__.py
+-rw-r--r--   0        0        0     3660 2023-07-17 15:22:51.737379 symbol_shoestring-0.0.2/shoestring/wizard/__main__.py
+-rw-r--r--   0        0        0     1970 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/buttons.py
+-rw-r--r--   0        0        0      484 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/keybindings.py
+-rw-r--r--   0        0        0     1553 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/navigation.py
+-rw-r--r--   0        0        0     1635 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screen_loader.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/__init__.py
+-rw-r--r--   0        0        0     1890 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/certificates.py
+-rw-r--r--   0        0        0      652 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/end_screen.py
+-rw-r--r--   0        0        0     6536 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/harvesting.py
+-rw-r--r--   0        0        0     1625 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/modal.py
+-rw-r--r--   0        0        0      799 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/network_type.py
+-rw-r--r--   0        0        0     2981 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/node_settings.py
+-rw-r--r--   0        0        0      757 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/node_type.py
+-rw-r--r--   0        0        0     6862 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/obligatory.py
+-rw-r--r--   0        0        0      827 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/root_check.py
+-rw-r--r--   0        0        0      799 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/voting.py
+-rw-r--r--   0        0        0     1835 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/welcome.py
+-rw-r--r--   0        0        0     3810 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/setup_file_generator.py
+-rw-r--r--   0        0        0     1744 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/shoestring_dispatcher.py
+-rw-r--r--   0        0        0     1095 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/styles.py
+-rw-r--r--   0        0        0     2830 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/templates/docker-compose-dual.yaml
+-rw-r--r--   0        0        0      629 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/templates/docker-compose-peer.yaml
+-rw-r--r--   0        0        0      299 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/templates/nginx.conf.erb
+-rw-r--r--   0        0        0    10861 1970-01-01 00:00:00.000000 symbol_shoestring-0.0.2/PKG-INFO
```

### Comparing `symbol_shoestring-0.0.1/README.md` & `symbol_shoestring-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/__main__.py` & `symbol_shoestring-0.0.2/shoestring/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import asyncio
 import gettext
 import importlib
 import os
 import sys
+from pathlib import Path
 
 
 def register_subcommand(subparsers, name, help_text):
 	parser = subparsers.add_parser(name, help=help_text)
 	module = importlib.import_module(f'shoestring.commands.{name.replace("-", "_")}')
 	module.add_arguments(parser)
 
@@ -29,15 +30,16 @@
 	register_subcommand(subparsers, 'signer', _('main-signer-help'))
 	register_subcommand(subparsers, 'upgrade', _('main-upgrade-help'))
 
 	return parser.parse_args(args)
 
 
 async def main(args):
-	lang = gettext.translation('messages', localedir='lang', languages=(os.environ.get('LC_MESSAGES', 'en'), 'en'))
+	lang_directory = Path(__file__).resolve().parent.parent / 'lang'
+	lang = gettext.translation('messages', localedir=lang_directory, languages=(os.environ.get('LC_MESSAGES', 'en'), 'en'))
 	lang.install()
 
 	args = parse_args(args)
 	possible_task = args.func(args)
 	if possible_task:
 		await possible_task
```

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/announce_transaction.py` & `symbol_shoestring-0.0.2/shoestring/commands/announce_transaction.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/health.py` & `symbol_shoestring-0.0.2/shoestring/commands/health.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/import_bootstrap.py` & `symbol_shoestring-0.0.2/shoestring/commands/import_bootstrap.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/init.py` & `symbol_shoestring-0.0.2/shoestring/commands/init.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/min_cosignatures_count.py` & `symbol_shoestring-0.0.2/shoestring/commands/min_cosignatures_count.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/pemtool.py` & `symbol_shoestring-0.0.2/shoestring/commands/pemtool.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/renew_certificates.py` & `symbol_shoestring-0.0.2/shoestring/commands/renew_certificates.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/renew_voting_keys.py` & `symbol_shoestring-0.0.2/shoestring/commands/renew_voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/reset_data.py` & `symbol_shoestring-0.0.2/shoestring/commands/reset_data.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/setup.py` & `symbol_shoestring-0.0.2/shoestring/commands/setup.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/signer.py` & `symbol_shoestring-0.0.2/shoestring/commands/signer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/commands/upgrade.py` & `symbol_shoestring-0.0.2/shoestring/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/healthagents/peer_api.py` & `symbol_shoestring-0.0.2/shoestring/healthagents/peer_api.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/healthagents/peer_certificate.py` & `symbol_shoestring-0.0.2/shoestring/healthagents/peer_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/healthagents/rest_api.py` & `symbol_shoestring-0.0.2/shoestring/healthagents/rest_api.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/healthagents/rest_https_certificate.py` & `symbol_shoestring-0.0.2/shoestring/healthagents/rest_https_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/healthagents/voting_keys.py` & `symbol_shoestring-0.0.2/shoestring/healthagents/voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/healthagents/websockets.py` & `symbol_shoestring-0.0.2/shoestring/healthagents/websockets.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/CertificateFactory.py` & `symbol_shoestring-0.0.2/shoestring/internal/CertificateFactory.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/ConfigurationManager.py` & `symbol_shoestring-0.0.2/shoestring/internal/ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/FileDownloader.py` & `symbol_shoestring-0.0.2/shoestring/internal/FileDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/HarvesterConfigurator.py` & `symbol_shoestring-0.0.2/shoestring/internal/HarvesterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/HeightGrouping.py` & `symbol_shoestring-0.0.2/shoestring/internal/HeightGrouping.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/LinkTransactionBuilder.py` & `symbol_shoestring-0.0.2/shoestring/internal/LinkTransactionBuilder.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/MultisigAnalyzer.py` & `symbol_shoestring-0.0.2/shoestring/internal/MultisigAnalyzer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/NodeDownloader.py` & `symbol_shoestring-0.0.2/shoestring/internal/NodeDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/NodeFeatures.py` & `symbol_shoestring-0.0.2/shoestring/internal/NodeFeatures.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/NodewatchClient.py` & `symbol_shoestring-0.0.2/shoestring/internal/NodewatchClient.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/OpensslExecutor.py` & `symbol_shoestring-0.0.2/shoestring/internal/OpensslExecutor.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/PackageResolver.py` & `symbol_shoestring-0.0.2/shoestring/internal/PackageResolver.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/PeerDownloader.py` & `symbol_shoestring-0.0.2/shoestring/internal/PeerDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/PemUtils.py` & `symbol_shoestring-0.0.2/shoestring/internal/PemUtils.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/Preparer.py` & `symbol_shoestring-0.0.2/shoestring/internal/Preparer.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,18 +331,14 @@
 
 			factory.package(self.directories.certificates)
 
 	def configure_docker(self, template_mapping):
 		"""Prepares docker-compose file."""
 
 		if NodeFeatures.API in self.config.node.features:
-			#
-			# TODO: where should those (startup + docker templates) be copied from?
-			# we can copy from within repo, but will shoestring be a separate installable (pypi) package?
-			#
 			self._copy_tree_readonly('startup', self.directories.startup)
 
 		compose_template_filename_postfix = 'dual' if NodeFeatures.API in self.config.node.features else 'peer'
 		compose_template_filename = f'templates/docker-compose-{compose_template_filename_postfix}.yaml'
 		compose_output_filepath = self.directory / 'docker-compose.yaml'
 		apply_template(compose_template_filename, template_mapping, compose_output_filepath)
 		compose_output_filepath.chmod(0o400)
```

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/ShoestringConfiguration.py` & `symbol_shoestring-0.0.2/shoestring/internal/ShoestringConfiguration.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/internal/VoterConfigurator.py` & `symbol_shoestring-0.0.2/shoestring/internal/VoterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/Screen.py` & `symbol_shoestring-0.0.2/shoestring/wizard/Screen.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/Screens.py` & `symbol_shoestring-0.0.2/shoestring/wizard/Screens.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/ShoestringOperation.py` & `symbol_shoestring-0.0.2/shoestring/wizard/ShoestringOperation.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/TabbedView.py` & `symbol_shoestring-0.0.2/shoestring/wizard/TabbedView.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/TitleBar.py` & `symbol_shoestring-0.0.2/shoestring/wizard/TitleBar.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/ValidatingTextBox.py` & `symbol_shoestring-0.0.2/shoestring/wizard/ValidatingTextBox.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/__main__.py` & `symbol_shoestring-0.0.2/shoestring/wizard/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import gettext
 import os
 from functools import partial
+from pathlib import Path
 
 from prompt_toolkit import Application
 from prompt_toolkit.filters.base import Condition
 from prompt_toolkit.formatted_text import HTML
 from prompt_toolkit.layout.containers import ConditionalContainer, FloatContainer, HSplit, Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
@@ -21,16 +22,17 @@
 from .buttons import create_next_clicked_handler, create_operation_button_handler, create_prev_clicked_handler
 from .screen_loader import load_screens
 from .Screens import Screens
 from .shoestring_dispatcher import dispatch_shoestring_command
 from .TitleBar import TitleBar
 
 
-async def main():  # pylint: disable=too-many-locals, too-many-statements
-	lang = gettext.translation('messages', localedir='lang', languages=(os.environ.get('LC_MESSAGES', 'en'), 'en'))
+async def main():  # pylint: disable=too-many-locals
+	lang_directory = Path(__file__).resolve().parent.parent.parent / 'lang'
+	lang = gettext.translation('messages', localedir=lang_directory, languages=(os.environ.get('LC_MESSAGES', 'en'), 'en'))
 	lang.install()
 
 	message_box_float = create_message_box_float()
 
 	key_bindings = keybindings.initialize(lambda: message_box_float.visible)
 	app_styles = styles.initialize()
 	navbar = navigation.initialize()
```

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/buttons.py` & `symbol_shoestring-0.0.2/shoestring/wizard/buttons.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/navigation.py` & `symbol_shoestring-0.0.2/shoestring/wizard/navigation.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screen_loader.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screen_loader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/certificates.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/certificates.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/end_screen.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/end_screen.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/harvesting.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/harvesting.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/modal.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/modal.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/network_type.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/network_type.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/node_settings.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/node_settings.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/node_type.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/node_type.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/obligatory.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/obligatory.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/root_check.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/root_check.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/voting.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/voting.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/screens/welcome.py` & `symbol_shoestring-0.0.2/shoestring/wizard/screens/welcome.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/setup_file_generator.py` & `symbol_shoestring-0.0.2/shoestring/wizard/setup_file_generator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/shoestring_dispatcher.py` & `symbol_shoestring-0.0.2/shoestring/wizard/shoestring_dispatcher.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/shoestring/wizard/styles.py` & `symbol_shoestring-0.0.2/shoestring/wizard/styles.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.1/PKG-INFO` & `symbol_shoestring-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbol-shoestring
-Version: 0.0.1
+Version: 0.0.2
 Summary: Symbol Shoestring Deployment Tool
 Home-page: https://github.com/symbol/product/tree/main/tools/shoestring
 License: MIT
 Keywords: symbol,shoestring,deployment,node
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
@@ -14,23 +14,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Requires-Dist: Jinja2 (==3.1.2)
-Requires-Dist: PyYAML (==6.0)
-Requires-Dist: aiohttp (==3.8.4)
-Requires-Dist: prompt-toolkit (==3.0.38)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: symbol-lightapi (==0.0.4)
-Requires-Dist: symbol-sdk-python (==3.0.7)
-Requires-Dist: websockets (==11.0.3)
-Requires-Dist: zenlog (==1.1)
 Project-URL: Repository, https://github.com/symbol/product/tree/main/tools/shoestring
 Description-Content-Type: text/markdown
 
 # shoestring
 
 # CLI Commands
```

