# Comparing `tmp/robotcode_language_server-0.47.1.tar.gz` & `tmp/robotcode_language_server-0.47.2.tar.gz`

## Comparing `robotcode_language_server-0.47.1.tar` & `robotcode_language_server-0.47.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    58866 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    71453 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    89225 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    58866 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    71453 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    89230 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.2/PKG-INFO
```

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 
     with RobotLanguageServer(
         mode=mode, tcp_params=TcpParams(addresses or "127.0.0.1", port), pipe_name=pipe_name, profile=profile
     ) as server:
         server.run()
 
 
-# mypy: disable-error-code="misc, arg-type, attr-defined"
-
-
 @click.command(
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
 @add_options(
     *server_options(
         ServerMode.STDIO,
```

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
             if (
                 self.config.filter_default_language
                 and len(self.namespace.languages.languages) > 1
                 and self.config.filter_default_language
             ):
                 languages = [v for v in languages if v.code != "en"]
 
-            headers = itertools.chain(*(lang.headers.keys() for lang in languages))
+            headers = set(itertools.chain(*(lang.headers.keys() for lang in languages)))
 
         return [
             CompletionItem(
                 label=s[0],
                 kind=CompletionItemKind.CLASS,
                 detail="Header",
                 # this is to get the english version in the documentation
```

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Optional
 
 from robotcode.core.async_itertools import async_next
-from robotcode.core.async_tools import run_coroutine_in_thread, threaded
+from robotcode.core.async_tools import threaded
 from robotcode.core.dataclasses import CamelSnakeMixin
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.core.lsp.types import Position, Range, TextDocumentIdentifier
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.language_server.robotframework.utils.ast_utils import (
     HasTokens,
     get_nodes_at_position,
@@ -49,59 +49,56 @@
         text_document: TextDocumentIdentifier,
         position: Position,
         *args: Any,
         **kwargs: Any,
     ) -> Optional[EvaluatableExpression]:
         from robot.parsing.lexer.tokens import Token as RobotToken
 
-        async def run() -> Optional[EvaluatableExpression]:
-            document = await self.parent.documents.get(text_document.uri)
-            if document is None:
-                return None
-
-            namespace = await self.parent.documents_cache.get_namespace(document)
-            model = await self.parent.documents_cache.get_model(document, False)
-
-            nodes = await get_nodes_at_position(model, position)
-            node = nodes[-1]
-
-            if not isinstance(node, HasTokens):
-                return None
-
-            token = get_tokens_at_position(node, position)[-1]
-
+        document = await self.parent.documents.get(text_document.uri)
+        if document is None:
+            return None
+
+        namespace = await self.parent.documents_cache.get_namespace(document)
+        model = await self.parent.documents_cache.get_model(document, False)
+
+        nodes = await get_nodes_at_position(model, position)
+        node = nodes[-1]
+
+        if not isinstance(node, HasTokens):
+            return None
+
+        token = get_tokens_at_position(node, position)[-1]
+
+        token_and_var = await async_next(
+            (
+                (t, v)
+                async for t, v in self.iter_variables_from_token(token, namespace, nodes, position)
+                if position in range_from_token(t)
+            ),
+            None,
+        )
+
+        if (
+            token_and_var is None
+            and isinstance(node, self.get_expression_statement_types())
+            and (token := node.get_token(RobotToken.ARGUMENT)) is not None
+            and position in range_from_token(token)
+        ):
             token_and_var = await async_next(
                 (
-                    (t, v)
-                    async for t, v in self.iter_variables_from_token(token, namespace, nodes, position)
-                    if position in range_from_token(t)
+                    (var_token, var)
+                    async for var_token, var in self.iter_expression_variables_from_token(
+                        token, namespace, nodes, position
+                    )
+                    if position in range_from_token(var_token)
                 ),
                 None,
             )
 
-            if (
-                token_and_var is None
-                and isinstance(node, self.get_expression_statement_types())
-                and (token := node.get_token(RobotToken.ARGUMENT)) is not None
-                and position in range_from_token(token)
-            ):
-                token_and_var = await async_next(
-                    (
-                        (var_token, var)
-                        async for var_token, var in self.iter_expression_variables_from_token(
-                            token, namespace, nodes, position
-                        )
-                        if position in range_from_token(var_token)
-                    ),
-                    None,
-                )
-
-            if token_and_var is None:
-                return None
-
-            var_token, var = token_and_var
-            if var.name == "${CURDIR}":
-                return None
+        if token_and_var is None:
+            return None
 
-            return EvaluatableExpression(range_from_token(var_token), var.name)
+        var_token, var = token_and_var
+        if var.name == "${CURDIR}":
+            return None
 
-        return await run_coroutine_in_thread(run)
+        return EvaluatableExpression(range_from_token(var_token), var.name)
```

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         sender: Any,
         document: TextDocument,
         range: Range,
         context: InlineValueContext,
     ) -> Optional[List[InlineValue]]:
         from robot.parsing.lexer import Token as RobotToken
 
+        # TODO make this configurable
+
         namespace = await self.parent.documents_cache.get_namespace(document)
 
         model = await self.parent.documents_cache.get_model(document, False)
 
         real_range = Range(range.start, min(range.end, context.stopped_location.end))
 
         nodes = await get_nodes_at_position(model, context.stopped_location.start)
```

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.47.2/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/.gitignore` & `robotcode_language_server-0.47.2/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/LICENSE.txt` & `robotcode_language_server-0.47.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/README.md` & `robotcode_language_server-0.47.2/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.47.1/pyproject.toml` & `robotcode_language_server-0.47.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.47.1",
-  "robotcode==0.47.1",
+  "robotcode-jsonrpc2==0.47.2",
+  "robotcode==0.47.2",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.47.1/PKG-INFO` & `robotcode_language_server-0.47.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.47.1
+Version: 0.47.2
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.47.1
-Requires-Dist: robotcode==0.47.1
+Requires-Dist: robotcode-jsonrpc2==0.47.2
+Requires-Dist: robotcode==0.47.2
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

