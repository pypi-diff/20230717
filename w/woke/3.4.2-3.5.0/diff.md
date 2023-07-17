# Comparing `tmp/woke-3.4.2.tar.gz` & `tmp/woke-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woke-3.4.2.tar", max compression
+gzip compressed data, was "woke-3.5.0.tar", max compression
```

## Comparing `woke-3.4.2.tar` & `woke-3.5.0.tar`

### file list

```diff
@@ -1,240 +1,240 @@
--rw-r--r--   0        0        0      751 2023-05-13 06:28:54.162344 woke-3.4.2/LICENSE
--rw-r--r--   0        0        0     3415 2023-05-13 06:29:36.852316 woke-3.4.2/README.md
--rw-r--r--   0        0        0     2720 2023-05-23 13:18:21.574662 woke-3.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.189011 woke-3.4.2/woke/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.189011 woke-3.4.2/woke/analysis/__init__.py
--rw-r--r--   0        0        0    20473 2023-05-23 12:59:50.604420 woke-3.4.2/woke/analysis/cfg.py
--rw-r--r--   0        0        0     1013 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/__init__.py
--rw-r--r--   0        0        0    21743 2023-05-23 12:59:50.607753 woke-3.4.2/woke/analysis/detectors/api.py
--rw-r--r--   0        0        0       61 2023-05-13 06:28:54.189011 woke-3.4.2/woke/analysis/detectors/axelar/__init__.py
--rw-r--r--   0        0        0    15183 2023-05-13 06:29:36.852316 woke-3.4.2/woke/analysis/detectors/axelar/proxy_contract_id.py
--rw-r--r--   0        0        0     6389 2023-05-13 06:29:36.852316 woke-3.4.2/woke/analysis/detectors/balance_state_var.py
--rw-r--r--   0        0        0     4759 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/bug_empty_byte_array_copy.py
--rw-r--r--   0        0        0     1777 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/call_options_not_called.py
--rw-r--r--   0        0        0     4162 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/missing_return.py
--rw-r--r--   0        0        0     3013 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/msg_value_nonpayable_function.py
--rw-r--r--   0        0        0     8723 2023-05-13 06:29:36.852316 woke-3.4.2/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
--rw-r--r--   0        0        0    17299 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/ownable.py
--rw-r--r--   0        0        0    23312 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/proxy_contract_selector_clashes.py
--rw-r--r--   0        0        0    13982 2023-05-23 12:59:50.607753 woke-3.4.2/woke/analysis/detectors/reentrancy.py
--rw-r--r--   0        0        0     2766 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/unchecked_return_value.py
--rw-r--r--   0        0        0     6242 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/unsafe_delegatecall.py
--rw-r--r--   0        0        0     1344 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/unsafe_selfdestruct.py
--rw-r--r--   0        0        0     5982 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/unsafe_tx_origin.py
--rw-r--r--   0        0        0     1397 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/unused_contract.py
--rw-r--r--   0        0        0    12233 2023-05-23 12:59:50.607753 woke-3.4.2/woke/analysis/detectors/utils.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/__init__.py
--rw-r--r--   0        0        0    10947 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/enums.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/__init__.py
--rw-r--r--   0        0        0     5941 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/abc.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/__init__.py
--rw-r--r--   0        0        0     5854 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/abc.py
--rw-r--r--   0        0        0    16974 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/contract_definition.py
--rw-r--r--   0        0        0     3079 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/enum_definition.py
--rw-r--r--   0        0        0     1361 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/enum_value.py
--rw-r--r--   0        0        0     4408 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/error_definition.py
--rw-r--r--   0        0        0     5162 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/event_definition.py
--rw-r--r--   0        0        0    18683 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/function_definition.py
--rw-r--r--   0        0        0    12891 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/modifier_definition.py
--rw-r--r--   0        0        0     3414 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/struct_definition.py
--rw-r--r--   0        0        0     2654 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/user_defined_value_type_definition.py
--rw-r--r--   0        0        0    19473 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/variable_declaration.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/__init__.py
--rw-r--r--   0        0        0     6583 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/abc.py
--rw-r--r--   0        0        0     4063 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/expression/assignment.py
--rw-r--r--   0        0        0     2959 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/binary_operation.py
--rw-r--r--   0        0        0     2087 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/conditional.py
--rw-r--r--   0        0        0     1361 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/elementary_type_name_expression.py
--rw-r--r--   0        0        0     8933 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/expression/function_call.py
--rw-r--r--   0        0        0     2142 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/expression/function_call_options.py
--rw-r--r--   0        0        0     5709 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/expression/identifier.py
--rw-r--r--   0        0        0     1996 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/index_access.py
--rw-r--r--   0        0        0     2661 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/index_range_access.py
--rw-r--r--   0        0        0     1437 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/literal.py
--rw-r--r--   0        0        0    19431 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/expression/member_access.py
--rw-r--r--   0        0        0     1376 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/new_expression.py
--rw-r--r--   0        0        0     2191 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/expression/tuple_expression.py
--rw-r--r--   0        0        0     3071 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/unary_operation.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/meta/__init__.py
--rw-r--r--   0        0        0    10965 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/identifier_path.py
--rw-r--r--   0        0        0     8998 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/import_directive.py
--rw-r--r--   0        0        0     3752 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/inheritance_specifier.py
--rw-r--r--   0        0        0     5700 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/modifier_invocation.py
--rw-r--r--   0        0        0     3462 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/override_specifier.py
--rw-r--r--   0        0        0     4311 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/parameter_list.py
--rw-r--r--   0        0        0     1534 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/pragma_directive.py
--rw-r--r--   0        0        0     9307 2023-05-23 12:59:50.607753 woke-3.4.2/woke/ast/ir/meta/source_unit.py
--rw-r--r--   0        0        0     2315 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/structured_documentation.py
--rw-r--r--   0        0        0     4541 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/meta/try_catch_clause.py
--rw-r--r--   0        0        0     5698 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/meta/using_for_directive.py
--rw-r--r--   0        0        0     4812 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/reference_resolver.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/__init__.py
--rw-r--r--   0        0        0     5608 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/abc.py
--rw-r--r--   0        0        0     3135 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/block.py
--rw-r--r--   0        0        0     1611 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/break_statement.py
--rw-r--r--   0        0        0     1635 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/continue_statement.py
--rw-r--r--   0        0        0     2563 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/do_while_statement.py
--rw-r--r--   0        0        0     2452 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/emit_statement.py
--rw-r--r--   0        0        0     6016 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/expression_statement.py
--rw-r--r--   0        0        0     5735 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/for_statement.py
--rw-r--r--   0        0        0     3423 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/if_statement.py
--rw-r--r--   0        0        0    10276 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/inline_assembly.py
--rw-r--r--   0        0        0     1583 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/placeholder_statement.py
--rw-r--r--   0        0        0     3336 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/return_statement.py
--rw-r--r--   0        0        0     2608 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/revert_statement.py
--rw-r--r--   0        0        0     3134 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/try_statement.py
--rw-r--r--   0        0        0     2454 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/unchecked_block.py
--rw-r--r--   0        0        0     4330 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/variable_declaration_statement.py
--rw-r--r--   0        0        0     2596 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/while_statement.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/type_name/__init__.py
--rw-r--r--   0        0        0     4932 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/type_name/abc.py
--rw-r--r--   0        0        0     4092 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/array_type_name.py
--rw-r--r--   0        0        0     5967 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/elementary_type_name.py
--rw-r--r--   0        0        0     3987 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/function_type_name.py
--rw-r--r--   0        0        0     3938 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/mapping.py
--rw-r--r--   0        0        0    11314 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/user_defined_type_name.py
--rw-r--r--   0        0        0       36 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/utils/__init__.py
--rw-r--r--   0        0        0      589 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/utils/init_tuple.py
--rw-r--r--   0        0        0      578 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/__init__.py
--rw-r--r--   0        0        0      705 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/abc.py
--rw-r--r--   0        0        0     1817 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/assignment.py
--rw-r--r--   0        0        0     4317 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/block.py
--rw-r--r--   0        0        0      301 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/break_statement.py
--rw-r--r--   0        0        0     1200 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/case_statement.py
--rw-r--r--   0        0        0      304 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/continue_statement.py
--rw-r--r--   0        0        0     1659 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/expression_statement.py
--rw-r--r--   0        0        0     1893 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/for_loop.py
--rw-r--r--   0        0        0     2323 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/function_call.py
--rw-r--r--   0        0        0     2298 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/function_definition.py
--rw-r--r--   0        0        0     1492 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/identifier.py
--rw-r--r--   0        0        0     1582 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/if_statement.py
--rw-r--r--   0        0        0      301 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/leave.py
--rw-r--r--   0        0        0     1781 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/literal.py
--rw-r--r--   0        0        0     1802 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/switch.py
--rw-r--r--   0        0        0      921 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/typed_name.py
--rw-r--r--   0        0        0     2097 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/variable_declaration.py
--rw-r--r--   0        0        0    37866 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/nodes.py
--rw-r--r--   0        0        0    47087 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/types.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/__init__.py
--rw-r--r--   0        0        0     3501 2023-05-13 06:29:36.855649 woke-3.4.2/woke/cli/__main__.py
--rw-r--r--   0        0        0     7942 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/accounts.py
--rw-r--r--   0        0        0     4650 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/compile.py
--rw-r--r--   0        0        0       54 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/console.py
--rw-r--r--   0        0        0     3838 2023-05-23 12:59:50.611086 woke-3.4.2/woke/cli/detect.py
--rw-r--r--   0        0        0     3791 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/fuzz.py
--rw-r--r--   0        0        0    11813 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/init.py
--rw-r--r--   0        0        0     1081 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/lsp.py
--rw-r--r--   0        0        0     3154 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/run.py
--rw-r--r--   0        0        0     4922 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/svm.py
--rw-r--r--   0        0        0     2258 2023-05-22 07:04:56.893614 woke-3.4.2/woke/cli/test.py
--rw-r--r--   0        0        0      187 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/__init__.py
--rw-r--r--   0        0        0     1814 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/build_data_model.py
--rw-r--r--   0        0        0     3120 2023-05-13 06:29:36.855649 woke-3.4.2/woke/compiler/compilation_unit.py
--rw-r--r--   0        0        0    41479 2023-05-23 12:59:50.614420 woke-3.4.2/woke/compiler/compiler.py
--rw-r--r--   0        0        0       97 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/exceptions.py
--rw-r--r--   0        0        0      103 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/__init__.py
--rw-r--r--   0        0        0       48 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/exceptions.py
--rw-r--r--   0        0        0     8554 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/input_data_model.py
--rw-r--r--   0        0        0     8728 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/output_data_model.py
--rw-r--r--   0        0        0     3571 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/solc_runner.py
--rw-r--r--   0        0        0     2455 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/source_path_resolver.py
--rw-r--r--   0        0        0     4813 2023-05-13 06:29:36.855649 woke-3.4.2/woke/compiler/source_unit_name_resolver.py
--rw-r--r--   0        0        0     1118 2023-05-13 06:28:54.199011 woke-3.4.2/woke/config/__init__.py
--rw-r--r--   0        0        0     6912 2023-05-23 12:59:50.614420 woke-3.4.2/woke/config/data_model.py
--rw-r--r--   0        0        0    12682 2023-05-13 06:29:36.855649 woke-3.4.2/woke/config/woke_config.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/contracts/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/contracts/woke/__init__.py
--rw-r--r--   0        0        0    64087 2023-05-13 06:28:54.199011 woke-3.4.2/woke/contracts/woke/console.sol
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/core/__init__.py
--rw-r--r--   0        0        0      386 2023-05-13 06:29:36.855649 woke-3.4.2/woke/core/enums.py
--rw-r--r--   0        0        0    24829 2023-05-13 06:29:36.855649 woke-3.4.2/woke/core/solidity_version.py
--rw-r--r--   0        0        0      678 2023-05-13 06:29:36.855649 woke-3.4.2/woke/deployment/__init__.py
--rw-r--r--   0        0        0    14848 2023-05-13 06:29:36.858982 woke-3.4.2/woke/deployment/core.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/development/__init__.py
--rw-r--r--   0        0        0     4552 2023-05-13 06:28:54.199011 woke-3.4.2/woke/development/blocks.py
--rw-r--r--   0        0        0    28963 2023-05-13 06:29:36.858982 woke-3.4.2/woke/development/call_trace.py
--rw-r--r--   0        0        0    25863 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/chain_interfaces.py
--rw-r--r--   0        0        0     1132 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/constants.py
--rw-r--r--   0        0        0    96441 2023-05-23 13:17:34.084931 woke-3.4.2/woke/development/core.py
--rw-r--r--   0        0        0     7270 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/globals.py
--rw-r--r--   0        0        0   161115 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/hardhat_console.py
--rw-r--r--   0        0        0     1093 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/internal.py
--rw-r--r--   0        0        0       39 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/__init__.py
--rw-r--r--   0        0        0      302 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/abc.py
--rw-r--r--   0        0        0     2070 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/communicator.py
--rw-r--r--   0        0        0      821 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/http.py
--rw-r--r--   0        0        0     2912 2023-05-13 06:29:36.858982 woke-3.4.2/woke/development/json_rpc/ipc.py
--rw-r--r--   0        0        0      625 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/websocket.py
--rw-r--r--   0        0        0     6572 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/primitive_types.py
--rw-r--r--   0        0        0    89995 2023-05-23 13:17:34.084931 woke-3.4.2/woke/development/pytypes_generator.py
--rw-r--r--   0        0        0    28061 2023-05-22 07:04:56.893614 woke-3.4.2/woke/development/transactions.py
--rw-r--r--   0        0        0     7389 2023-05-13 06:28:54.205678 woke-3.4.2/woke/development/utils.py
--rw-r--r--   0        0        0       47 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/__init__.py
--rw-r--r--   0        0        0      310 2023-05-22 07:04:56.893614 woke-3.4.2/woke/lsp/commands/__init__.py
--rw-r--r--   0        0        0     4033 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/commands/generate_control_flow_graph.py
--rw-r--r--   0        0        0     1097 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/commands/generate_imports_graph.py
--rw-r--r--   0        0        0     4247 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/commands/generate_inheritance_graph.py
--rw-r--r--   0        0        0     2163 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/commands/generate_linearized_inheritance_graph.py
--rw-r--r--   0        0        0    31491 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/common_structures.py
--rw-r--r--   0        0        0     1900 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/context.py
--rw-r--r--   0        0        0     2574 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/document_sync.py
--rw-r--r--   0        0        0      130 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/enums.py
--rw-r--r--   0        0        0      471 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/__init__.py
--rw-r--r--   0        0        0     6969 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/code_action.py
--rw-r--r--   0        0        0    10904 2023-05-22 07:04:56.893614 woke-3.4.2/woke/lsp/features/code_lens.py
--rw-r--r--   0        0        0    19824 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/completion.py
--rw-r--r--   0        0        0     9948 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/definition.py
--rw-r--r--   0        0        0     1446 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/diagnostic.py
--rw-r--r--   0        0        0     4305 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/document_link.py
--rw-r--r--   0        0        0     8407 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/document_symbol.py
--rw-r--r--   0        0        0    17901 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/hover.py
--rw-r--r--   0        0        0     3850 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/implementation.py
--rw-r--r--   0        0        0     5092 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/references.py
--rw-r--r--   0        0        0     8935 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/rename.py
--rw-r--r--   0        0        0     9505 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/type_definition.py
--rw-r--r--   0        0        0    11043 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/type_hierarchy.py
--rw-r--r--   0        0        0    39957 2023-05-23 12:59:50.614420 woke-3.4.2/woke/lsp/lsp_compiler.py
--rw-r--r--   0        0        0      328 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/lsp_data_model.py
--rw-r--r--   0        0        0     8941 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/lsp_parser.py
--rw-r--r--   0        0        0     5551 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/methods.py
--rw-r--r--   0        0        0     1897 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/protocol_structures.py
--rw-r--r--   0        0        0     2229 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/rpc_protocol.py
--rw-r--r--   0        0        0    37738 2023-05-22 07:04:56.893614 woke-3.4.2/woke/lsp/server.py
--rw-r--r--   0        0        0     6597 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/server_capabilities.py
--rw-r--r--   0        0        0       86 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/utils/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/utils/position.py
--rw-r--r--   0        0        0      459 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/utils/uri.py
--rw-r--r--   0        0        0       50 2023-05-13 06:28:54.205678 woke-3.4.2/woke/regex_parser/__init__.py
--rw-r--r--   0        0        0     1690 2023-05-13 06:28:54.205678 woke-3.4.2/woke/regex_parser/solidity_import.py
--rw-r--r--   0        0        0     6653 2023-05-23 12:59:50.617753 woke-3.4.2/woke/regex_parser/solidity_parser.py
--rw-r--r--   0        0        0       36 2023-05-13 06:28:54.205678 woke-3.4.2/woke/svm/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-13 06:29:36.858982 woke-3.4.2/woke/svm/abc.py
--rw-r--r--   0        0        0      270 2023-05-13 06:28:54.205678 woke-3.4.2/woke/svm/exceptions.py
--rw-r--r--   0        0        0    11721 2023-05-13 06:29:36.858982 woke-3.4.2/woke/svm/svm.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/scripts/__init__.py
--rw-r--r--   0        0        0      184 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/scripts/deploy.py
--rw-r--r--   0        0        0        0 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/tests/__init__.py
--rw-r--r--   0        0        0      140 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/tests/test_default.py
--rw-r--r--   0        0        0      678 2023-05-13 06:29:36.858982 woke-3.4.2/woke/testing/__init__.py
--rw-r--r--   0        0        0    10878 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/core.py
--rw-r--r--   0        0        0    24381 2023-05-13 06:29:36.858982 woke-3.4.2/woke/testing/coverage.py
--rw-r--r--   0        0        0      187 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/__init__.py
--rw-r--r--   0        0        0     4999 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/fuzz_test.py
--rw-r--r--   0        0        0    10795 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/fuzzer.py
--rw-r--r--   0        0        0     5780 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/generators.py
--rw-r--r--   0        0        0      298 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/pytest_plugin.py
--rw-r--r--   0        0        0      170 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/__init__.py
--rw-r--r--   0        0        0      560 2023-05-23 12:59:50.617753 woke-3.4.2/woke/utils/context_managers.py
--rw-r--r--   0        0        0      515 2023-05-23 12:59:50.617753 woke-3.4.2/woke/utils/decorators.py
--rw-r--r--   0        0        0      158 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/enums.py
--rw-r--r--   0        0        0     1699 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/file_utils.py
--rw-r--r--   0        0        0      384 2023-05-13 06:29:36.858982 woke-3.4.2/woke/utils/keyed_default_dict.py
--rw-r--r--   0        0        0      194 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/networking.py
--rw-r--r--   0        0        0     1017 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/openzeppelin.py
--rw-r--r--   0        0        0      630 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/string.py
--rw-r--r--   0        0        0     1747 2023-05-13 06:29:36.858982 woke-3.4.2/woke/utils/tee.py
--rw-r--r--   0        0        0     3765 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/threaded_child_watcher.py
--rw-r--r--   0        0        0      424 2023-05-13 06:29:36.858982 woke-3.4.2/woke/utils/version.py
--rw-r--r--   0        0        0     6129 1970-01-01 00:00:00.000000 woke-3.4.2/setup.py
--rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 woke-3.4.2/PKG-INFO
+-rw-r--r--   0        0        0      751 2023-05-24 10:43:30.470223 woke-3.5.0/LICENSE
+-rw-r--r--   0        0        0     3415 2023-05-24 10:43:30.470223 woke-3.5.0/README.md
+-rw-r--r--   0        0        0     2720 2023-07-17 12:10:52.083076 woke-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.496889 woke-3.5.0/woke/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/__init__.py
+-rw-r--r--   0        0        0    20473 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/cfg.py
+-rw-r--r--   0        0        0     1013 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/__init__.py
+-rw-r--r--   0        0        0    21743 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/api.py
+-rw-r--r--   0        0        0       61 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/axelar/__init__.py
+-rw-r--r--   0        0        0    15183 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/axelar/proxy_contract_id.py
+-rw-r--r--   0        0        0     6389 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/balance_state_var.py
+-rw-r--r--   0        0        0     4759 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/bug_empty_byte_array_copy.py
+-rw-r--r--   0        0        0     1777 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/call_options_not_called.py
+-rw-r--r--   0        0        0     4162 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/missing_return.py
+-rw-r--r--   0        0        0     3013 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/msg_value_nonpayable_function.py
+-rw-r--r--   0        0        0     8636 2023-07-17 12:10:25.583107 woke-3.5.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
+-rw-r--r--   0        0        0    17299 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/ownable.py
+-rw-r--r--   0        0        0    23312 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/proxy_contract_selector_clashes.py
+-rw-r--r--   0        0        0    13982 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/reentrancy.py
+-rw-r--r--   0        0        0     2766 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/unchecked_return_value.py
+-rw-r--r--   0        0        0     6242 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/unsafe_delegatecall.py
+-rw-r--r--   0        0        0     1344 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/unsafe_selfdestruct.py
+-rw-r--r--   0        0        0     5982 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/unsafe_tx_origin.py
+-rw-r--r--   0        0        0     1397 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/unused_contract.py
+-rw-r--r--   0        0        0    12233 2023-05-24 10:43:30.496889 woke-3.5.0/woke/analysis/detectors/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/__init__.py
+-rw-r--r--   0        0        0    10947 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/enums.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/__init__.py
+-rw-r--r--   0        0        0     5941 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/abc.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/__init__.py
+-rw-r--r--   0        0        0     5854 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/abc.py
+-rw-r--r--   0        0        0    16974 2023-06-02 07:10:21.578657 woke-3.5.0/woke/ast/ir/declaration/contract_definition.py
+-rw-r--r--   0        0        0     3079 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/enum_definition.py
+-rw-r--r--   0        0        0     1361 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/enum_value.py
+-rw-r--r--   0        0        0     4408 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/error_definition.py
+-rw-r--r--   0        0        0     5162 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/event_definition.py
+-rw-r--r--   0        0        0    18853 2023-07-17 12:10:25.583107 woke-3.5.0/woke/ast/ir/declaration/function_definition.py
+-rw-r--r--   0        0        0    12891 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/modifier_definition.py
+-rw-r--r--   0        0        0     3414 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/struct_definition.py
+-rw-r--r--   0        0        0     2654 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/user_defined_value_type_definition.py
+-rw-r--r--   0        0        0    19473 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/declaration/variable_declaration.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/__init__.py
+-rw-r--r--   0        0        0     6583 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/abc.py
+-rw-r--r--   0        0        0     5319 2023-07-17 12:10:25.583107 woke-3.5.0/woke/ast/ir/expression/assignment.py
+-rw-r--r--   0        0        0     2959 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/binary_operation.py
+-rw-r--r--   0        0        0     2087 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/conditional.py
+-rw-r--r--   0        0        0     1361 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/elementary_type_name_expression.py
+-rw-r--r--   0        0        0     8933 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/function_call.py
+-rw-r--r--   0        0        0     2142 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/function_call_options.py
+-rw-r--r--   0        0        0     5709 2023-07-08 06:51:16.698770 woke-3.5.0/woke/ast/ir/expression/identifier.py
+-rw-r--r--   0        0        0     1996 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/index_access.py
+-rw-r--r--   0        0        0     2661 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/index_range_access.py
+-rw-r--r--   0        0        0     1437 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/literal.py
+-rw-r--r--   0        0        0    19431 2023-07-08 06:51:17.098770 woke-3.5.0/woke/ast/ir/expression/member_access.py
+-rw-r--r--   0        0        0     1376 2023-05-24 10:43:30.496889 woke-3.5.0/woke/ast/ir/expression/new_expression.py
+-rw-r--r--   0        0        0     2191 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/expression/tuple_expression.py
+-rw-r--r--   0        0        0     3071 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/expression/unary_operation.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/__init__.py
+-rw-r--r--   0        0        0    10965 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/identifier_path.py
+-rw-r--r--   0        0        0     8998 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/import_directive.py
+-rw-r--r--   0        0        0     3752 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/inheritance_specifier.py
+-rw-r--r--   0        0        0     5700 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/modifier_invocation.py
+-rw-r--r--   0        0        0     3462 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/override_specifier.py
+-rw-r--r--   0        0        0     4311 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/parameter_list.py
+-rw-r--r--   0        0        0     1534 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/pragma_directive.py
+-rw-r--r--   0        0        0     9307 2023-07-17 10:19:52.075503 woke-3.5.0/woke/ast/ir/meta/source_unit.py
+-rw-r--r--   0        0        0     2315 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/structured_documentation.py
+-rw-r--r--   0        0        0     4541 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/try_catch_clause.py
+-rw-r--r--   0        0        0     5698 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/meta/using_for_directive.py
+-rw-r--r--   0        0        0     7286 2023-07-17 12:10:25.583107 woke-3.5.0/woke/ast/ir/reference_resolver.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/__init__.py
+-rw-r--r--   0        0        0     5608 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/abc.py
+-rw-r--r--   0        0        0     3135 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/block.py
+-rw-r--r--   0        0        0     1611 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/break_statement.py
+-rw-r--r--   0        0        0     1635 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/continue_statement.py
+-rw-r--r--   0        0        0     2563 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/do_while_statement.py
+-rw-r--r--   0        0        0     2452 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/emit_statement.py
+-rw-r--r--   0        0        0     6016 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/expression_statement.py
+-rw-r--r--   0        0        0     5735 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/for_statement.py
+-rw-r--r--   0        0        0     3423 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/if_statement.py
+-rw-r--r--   0        0        0    10276 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/inline_assembly.py
+-rw-r--r--   0        0        0     1583 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/placeholder_statement.py
+-rw-r--r--   0        0        0     3336 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/return_statement.py
+-rw-r--r--   0        0        0     2608 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/revert_statement.py
+-rw-r--r--   0        0        0     3134 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/try_statement.py
+-rw-r--r--   0        0        0     2454 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/unchecked_block.py
+-rw-r--r--   0        0        0     4330 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/variable_declaration_statement.py
+-rw-r--r--   0        0        0     2596 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/statement/while_statement.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/type_name/__init__.py
+-rw-r--r--   0        0        0     4932 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/type_name/abc.py
+-rw-r--r--   0        0        0     4092 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/type_name/array_type_name.py
+-rw-r--r--   0        0        0     5967 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/type_name/elementary_type_name.py
+-rw-r--r--   0        0        0     3987 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/type_name/function_type_name.py
+-rw-r--r--   0        0        0     3938 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/type_name/mapping.py
+-rw-r--r--   0        0        0    11314 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/type_name/user_defined_type_name.py
+-rw-r--r--   0        0        0       36 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/utils/__init__.py
+-rw-r--r--   0        0        0      589 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/utils/init_tuple.py
+-rw-r--r--   0        0        0      578 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/abc.py
+-rw-r--r--   0        0        0     1817 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/assignment.py
+-rw-r--r--   0        0        0     4317 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/block.py
+-rw-r--r--   0        0        0      301 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/break_statement.py
+-rw-r--r--   0        0        0     1200 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/case_statement.py
+-rw-r--r--   0        0        0      304 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/continue_statement.py
+-rw-r--r--   0        0        0     1659 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/expression_statement.py
+-rw-r--r--   0        0        0     1893 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/for_loop.py
+-rw-r--r--   0        0        0     2323 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/function_call.py
+-rw-r--r--   0        0        0     2298 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/function_definition.py
+-rw-r--r--   0        0        0     1492 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/identifier.py
+-rw-r--r--   0        0        0     1582 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/if_statement.py
+-rw-r--r--   0        0        0      301 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/leave.py
+-rw-r--r--   0        0        0     1781 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/literal.py
+-rw-r--r--   0        0        0     1802 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/switch.py
+-rw-r--r--   0        0        0      921 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/typed_name.py
+-rw-r--r--   0        0        0     2097 2023-05-24 10:43:30.500223 woke-3.5.0/woke/ast/ir/yul/variable_declaration.py
+-rw-r--r--   0        0        0    37885 2023-07-17 12:10:25.586440 woke-3.5.0/woke/ast/nodes.py
+-rw-r--r--   0        0        0    47087 2023-05-24 10:43:30.503556 woke-3.5.0/woke/ast/types.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.503556 woke-3.5.0/woke/cli/__init__.py
+-rw-r--r--   0        0        0     3491 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/__main__.py
+-rw-r--r--   0        0        0     8012 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/accounts.py
+-rw-r--r--   0        0        0     5097 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/compile.py
+-rw-r--r--   0        0        0       54 2023-05-24 10:43:30.503556 woke-3.5.0/woke/cli/console.py
+-rw-r--r--   0        0        0     3838 2023-07-17 10:07:36.767209 woke-3.5.0/woke/cli/detect.py
+-rw-r--r--   0        0        0     3779 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/fuzz.py
+-rw-r--r--   0        0        0    11949 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/init.py
+-rw-r--r--   0        0        0     1213 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/lsp.py
+-rw-r--r--   0        0        0     3154 2023-05-24 10:43:30.503556 woke-3.5.0/woke/cli/run.py
+-rw-r--r--   0        0        0     5495 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/svm.py
+-rw-r--r--   0        0        0     2711 2023-07-17 12:10:25.586440 woke-3.5.0/woke/cli/test.py
+-rw-r--r--   0        0        0      187 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/__init__.py
+-rw-r--r--   0        0        0     1836 2023-07-17 12:10:25.586440 woke-3.5.0/woke/compiler/build_data_model.py
+-rw-r--r--   0        0        0     3120 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/compilation_unit.py
+-rw-r--r--   0        0        0    44041 2023-07-17 12:10:25.586440 woke-3.5.0/woke/compiler/compiler.py
+-rw-r--r--   0        0        0       97 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/exceptions.py
+-rw-r--r--   0        0        0      103 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/solc_frontend/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/solc_frontend/exceptions.py
+-rw-r--r--   0        0        0     8554 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/solc_frontend/input_data_model.py
+-rw-r--r--   0        0        0     8728 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/solc_frontend/output_data_model.py
+-rw-r--r--   0        0        0     3571 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/solc_frontend/solc_runner.py
+-rw-r--r--   0        0        0     2455 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/source_path_resolver.py
+-rw-r--r--   0        0        0     4813 2023-05-24 10:43:30.503556 woke-3.5.0/woke/compiler/source_unit_name_resolver.py
+-rw-r--r--   0        0        0     1118 2023-05-24 10:43:30.503556 woke-3.5.0/woke/config/__init__.py
+-rw-r--r--   0        0        0     6912 2023-05-24 10:43:30.503556 woke-3.5.0/woke/config/data_model.py
+-rw-r--r--   0        0        0    12682 2023-05-24 10:43:30.503556 woke-3.5.0/woke/config/woke_config.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.503556 woke-3.5.0/woke/contracts/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.503556 woke-3.5.0/woke/contracts/woke/__init__.py
+-rw-r--r--   0        0        0    64087 2023-05-24 10:43:30.503556 woke-3.5.0/woke/contracts/woke/console.sol
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.503556 woke-3.5.0/woke/core/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-24 10:43:30.503556 woke-3.5.0/woke/core/enums.py
+-rw-r--r--   0        0        0    24829 2023-05-24 10:43:30.503556 woke-3.5.0/woke/core/solidity_version.py
+-rw-r--r--   0        0        0      678 2023-05-24 10:43:30.503556 woke-3.5.0/woke/deployment/__init__.py
+-rw-r--r--   0        0        0    14848 2023-05-24 10:43:30.503556 woke-3.5.0/woke/deployment/core.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.503556 woke-3.5.0/woke/development/__init__.py
+-rw-r--r--   0        0        0     4552 2023-05-24 10:43:30.503556 woke-3.5.0/woke/development/blocks.py
+-rw-r--r--   0        0        0    29041 2023-07-17 12:10:25.586440 woke-3.5.0/woke/development/call_trace.py
+-rw-r--r--   0        0        0    28478 2023-07-17 12:10:25.586440 woke-3.5.0/woke/development/chain_interfaces.py
+-rw-r--r--   0        0        0     1132 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/constants.py
+-rw-r--r--   0        0        0    98568 2023-07-17 12:10:25.586440 woke-3.5.0/woke/development/core.py
+-rw-r--r--   0        0        0     7270 2023-06-15 08:07:09.339852 woke-3.5.0/woke/development/globals.py
+-rw-r--r--   0        0        0   161115 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/hardhat_console.py
+-rw-r--r--   0        0        0     1093 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/internal.py
+-rw-r--r--   0        0        0       39 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/json_rpc/__init__.py
+-rw-r--r--   0        0        0      302 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/json_rpc/abc.py
+-rw-r--r--   0        0        0     2070 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/json_rpc/communicator.py
+-rw-r--r--   0        0        0      821 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/json_rpc/http.py
+-rw-r--r--   0        0        0     2912 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/json_rpc/ipc.py
+-rw-r--r--   0        0        0      668 2023-07-17 12:10:25.586440 woke-3.5.0/woke/development/json_rpc/websocket.py
+-rw-r--r--   0        0        0     6572 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/primitive_types.py
+-rw-r--r--   0        0        0    90215 2023-07-17 12:10:25.589774 woke-3.5.0/woke/development/pytypes_generator.py
+-rw-r--r--   0        0        0    29191 2023-07-17 12:10:25.589774 woke-3.5.0/woke/development/transactions.py
+-rw-r--r--   0        0        0     7389 2023-05-24 10:43:30.506889 woke-3.5.0/woke/development/utils.py
+-rw-r--r--   0        0        0       47 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/commands/__init__.py
+-rw-r--r--   0        0        0     4033 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/commands/generate_control_flow_graph.py
+-rw-r--r--   0        0        0     1097 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/commands/generate_imports_graph.py
+-rw-r--r--   0        0        0     4247 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/commands/generate_inheritance_graph.py
+-rw-r--r--   0        0        0     2163 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/commands/generate_linearized_inheritance_graph.py
+-rw-r--r--   0        0        0    31491 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/common_structures.py
+-rw-r--r--   0        0        0     1900 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/context.py
+-rw-r--r--   0        0        0     2574 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/document_sync.py
+-rw-r--r--   0        0        0      130 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/enums.py
+-rw-r--r--   0        0        0      471 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.506889 woke-3.5.0/woke/lsp/features/__init__.py
+-rw-r--r--   0        0        0     6969 2023-07-17 10:17:40.853056 woke-3.5.0/woke/lsp/features/code_action.py
+-rw-r--r--   0        0        0    10904 2023-07-17 10:17:40.853056 woke-3.5.0/woke/lsp/features/code_lens.py
+-rw-r--r--   0        0        0    19824 2023-07-17 10:17:40.853056 woke-3.5.0/woke/lsp/features/completion.py
+-rw-r--r--   0        0        0     9948 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/definition.py
+-rw-r--r--   0        0        0     1446 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/diagnostic.py
+-rw-r--r--   0        0        0     4305 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/document_link.py
+-rw-r--r--   0        0        0     8407 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/document_symbol.py
+-rw-r--r--   0        0        0    17901 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/hover.py
+-rw-r--r--   0        0        0     3850 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/implementation.py
+-rw-r--r--   0        0        0     5092 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/references.py
+-rw-r--r--   0        0        0     8935 2023-07-17 10:17:40.853056 woke-3.5.0/woke/lsp/features/rename.py
+-rw-r--r--   0        0        0     9505 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/type_definition.py
+-rw-r--r--   0        0        0    11043 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/features/type_hierarchy.py
+-rw-r--r--   0        0        0    43959 2023-07-17 12:10:25.589774 woke-3.5.0/woke/lsp/lsp_compiler.py
+-rw-r--r--   0        0        0      328 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/lsp_data_model.py
+-rw-r--r--   0        0        0     8941 2023-07-17 10:17:40.853056 woke-3.5.0/woke/lsp/lsp_parser.py
+-rw-r--r--   0        0        0     5551 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/methods.py
+-rw-r--r--   0        0        0     1897 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/protocol_structures.py
+-rw-r--r--   0        0        0     2229 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/rpc_protocol.py
+-rw-r--r--   0        0        0    37738 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/server.py
+-rw-r--r--   0        0        0     6597 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/server_capabilities.py
+-rw-r--r--   0        0        0       86 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/utils/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/utils/position.py
+-rw-r--r--   0        0        0      459 2023-05-24 10:43:30.510223 woke-3.5.0/woke/lsp/utils/uri.py
+-rw-r--r--   0        0        0       50 2023-05-24 10:43:30.510223 woke-3.5.0/woke/regex_parser/__init__.py
+-rw-r--r--   0        0        0     1690 2023-05-24 10:43:30.510223 woke-3.5.0/woke/regex_parser/solidity_import.py
+-rw-r--r--   0        0        0     6653 2023-05-24 10:43:30.510223 woke-3.5.0/woke/regex_parser/solidity_parser.py
+-rw-r--r--   0        0        0       36 2023-05-24 10:43:30.510223 woke-3.5.0/woke/svm/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-24 10:43:30.510223 woke-3.5.0/woke/svm/abc.py
+-rw-r--r--   0        0        0      270 2023-05-24 10:43:30.510223 woke-3.5.0/woke/svm/exceptions.py
+-rw-r--r--   0        0        0    11721 2023-05-24 10:43:30.510223 woke-3.5.0/woke/svm/svm.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.510223 woke-3.5.0/woke/templates/scripts/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-24 10:43:30.510223 woke-3.5.0/woke/templates/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:43:30.510223 woke-3.5.0/woke/templates/tests/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-24 10:43:30.510223 woke-3.5.0/woke/templates/tests/test_default.py
+-rw-r--r--   0        0        0      678 2023-05-24 10:43:30.510223 woke-3.5.0/woke/testing/__init__.py
+-rw-r--r--   0        0        0    10878 2023-05-24 10:43:30.510223 woke-3.5.0/woke/testing/core.py
+-rw-r--r--   0        0        0    24564 2023-07-17 12:10:25.589774 woke-3.5.0/woke/testing/coverage.py
+-rw-r--r--   0        0        0      187 2023-05-24 10:43:30.510223 woke-3.5.0/woke/testing/fuzzing/__init__.py
+-rw-r--r--   0        0        0     4997 2023-07-17 12:10:25.589774 woke-3.5.0/woke/testing/fuzzing/fuzz_test.py
+-rw-r--r--   0        0        0    10795 2023-05-24 10:43:30.510223 woke-3.5.0/woke/testing/fuzzing/fuzzer.py
+-rw-r--r--   0        0        0     5780 2023-05-24 10:43:30.510223 woke-3.5.0/woke/testing/fuzzing/generators.py
+-rw-r--r--   0        0        0      298 2023-05-24 10:43:30.510223 woke-3.5.0/woke/testing/pytest_plugin.py
+-rw-r--r--   0        0        0      170 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/context_managers.py
+-rw-r--r--   0        0        0      515 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/decorators.py
+-rw-r--r--   0        0        0      158 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/enums.py
+-rw-r--r--   0        0        0     1699 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/file_utils.py
+-rw-r--r--   0        0        0      384 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/keyed_default_dict.py
+-rw-r--r--   0        0        0      194 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/networking.py
+-rw-r--r--   0        0        0     1017 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/openzeppelin.py
+-rw-r--r--   0        0        0      630 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/string.py
+-rw-r--r--   0        0        0     1747 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/tee.py
+-rw-r--r--   0        0        0     3765 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/threaded_child_watcher.py
+-rw-r--r--   0        0        0      424 2023-05-24 10:43:30.510223 woke-3.5.0/woke/utils/version.py
+-rw-r--r--   0        0        0     6129 1970-01-01 00:00:00.000000 woke-3.5.0/setup.py
+-rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 woke-3.5.0/PKG-INFO
```

### Comparing `woke-3.4.2/LICENSE` & `woke-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/README.md` & `woke-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/pyproject.toml` & `woke-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woke"
-version = "3.4.2"
+version = "3.5.0"
 description = "Woke is a Python-based development and testing framework for Solidity."
 license = "ISC"
 authors = ["Ackee Blockchain"]
 readme = "README.md"
 homepage = "https://ackeeblockchain.com"
 repository = "https://github.com/Ackee-Blockchain/woke"
 documentation = "https://ackeeblockchain.com/woke/docs/latest"
```

### Comparing `woke-3.4.2/woke/analysis/cfg.py` & `woke-3.5.0/woke/analysis/cfg.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/__init__.py` & `woke-3.5.0/woke/analysis/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/api.py` & `woke-3.5.0/woke/analysis/detectors/api.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/axelar/proxy_contract_id.py` & `woke-3.5.0/woke/analysis/detectors/axelar/proxy_contract_id.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/balance_state_var.py` & `woke-3.5.0/woke/analysis/detectors/balance_state_var.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/bug_empty_byte_array_copy.py` & `woke-3.5.0/woke/analysis/detectors/bug_empty_byte_array_copy.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/call_options_not_called.py` & `woke-3.5.0/woke/analysis/detectors/call_options_not_called.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/missing_return.py` & `woke-3.5.0/woke/analysis/detectors/missing_return.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/msg_value_nonpayable_function.py` & `woke-3.5.0/woke/analysis/detectors/msg_value_nonpayable_function.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py` & `woke-3.5.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,17 +171,16 @@
             ):
                 func_identifier = func_identifier.components[0]
             elif isinstance(func_identifier, FunctionCall):
                 t = func_identifier.type
                 if isinstance(t, types.Function) and (t.value_set or t.gas_set):
                     func_identifier = func_identifier.expression
                 else:
-                    logger.warning(
-                        f"Unexpected function call child node: {func_identifier} {func_identifier.source}"
-                    )
+                    # function returning a function
+                    break
             else:
                 logger.warning(
                     f"Unexpected function call child node: {func_identifier} {func_identifier.source if func_identifier else ''}"
                 )
                 return
 
         t = func_identifier.type
```

### Comparing `woke-3.4.2/woke/analysis/detectors/ownable.py` & `woke-3.5.0/woke/analysis/detectors/ownable.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/proxy_contract_selector_clashes.py` & `woke-3.5.0/woke/analysis/detectors/proxy_contract_selector_clashes.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/reentrancy.py` & `woke-3.5.0/woke/analysis/detectors/reentrancy.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/unchecked_return_value.py` & `woke-3.5.0/woke/analysis/detectors/unchecked_return_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/unsafe_delegatecall.py` & `woke-3.5.0/woke/analysis/detectors/unsafe_delegatecall.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/unsafe_selfdestruct.py` & `woke-3.5.0/woke/analysis/detectors/unsafe_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/unsafe_tx_origin.py` & `woke-3.5.0/woke/analysis/detectors/unsafe_tx_origin.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/unused_contract.py` & `woke-3.5.0/woke/analysis/detectors/unused_contract.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/analysis/detectors/utils.py` & `woke-3.5.0/woke/analysis/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/enums.py` & `woke-3.5.0/woke/ast/enums.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/abc.py` & `woke-3.5.0/woke/ast/ir/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/abc.py` & `woke-3.5.0/woke/ast/ir/declaration/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/contract_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/contract_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/enum_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/enum_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/enum_value.py` & `woke-3.5.0/woke/ast/ir/declaration/enum_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/error_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/error_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/event_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/event_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/function_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/function_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,16 +266,16 @@
 
     @property
     @lru_cache(maxsize=2048)
     def canonical_name(self) -> str:
         from .contract_definition import ContractDefinition
 
         if isinstance(self._parent, ContractDefinition):
-            return f"{self._parent.canonical_name}.{self._name}"
-        return self.name
+            return f"{self._parent.canonical_name}.{self._name}({','.join(param.type_name.type_string for param in self._parameters.parameters)})"
+        return f"{self._name}({','.join(param.type_name.type_string for param in self._parameters.parameters)})"
 
     @property
     @lru_cache(maxsize=2048)
     def declaration_string(self) -> str:
         if self.kind == FunctionKind.CONSTRUCTOR:
             ret = "constructor"
         elif self.kind == FunctionKind.FALLBACK:
```

### Comparing `woke-3.4.2/woke/ast/ir/declaration/modifier_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/modifier_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/struct_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/struct_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/user_defined_value_type_definition.py` & `woke-3.5.0/woke/ast/ir/declaration/user_defined_value_type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/declaration/variable_declaration.py` & `woke-3.5.0/woke/ast/ir/declaration/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/abc.py` & `woke-3.5.0/woke/ast/ir/expression/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/assignment.py` & `woke-3.5.0/woke/ast/ir/expression/assignment.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from functools import lru_cache
 from typing import Iterator, Optional, Set, Tuple, Union
 
 from typing_extensions import Literal
 
-from woke.ast.enums import AssignmentOperator, ModifiesStateFlag
+from woke.ast.enums import AssignmentOperator, GlobalSymbolsEnum, ModifiesStateFlag
 from woke.ast.ir.abc import IrAbc, SolidityAbc
 from woke.ast.ir.utils import IrInitTuple
 from woke.ast.nodes import SolcAssignment
 
 from ..declaration.abc import DeclarationAbc
+from ..declaration.function_definition import FunctionDefinition
+from ..declaration.struct_definition import StructDefinition
+from ..declaration.variable_declaration import VariableDeclaration
 from ..meta.source_unit import SourceUnit
 from .abc import ExpressionAbc
 from .conditional import Conditional
+from .function_call import FunctionCall
 from .identifier import Identifier
 from .index_access import IndexAccess
 from .member_access import MemberAccess
 from .tuple_expression import TupleExpression
 
 AssignedVariablePath = Tuple[
     Union[DeclarationAbc, SourceUnit, Literal["IndexAccess"]], ...
@@ -100,14 +104,32 @@
             elif isinstance(node, MemberAccess):
                 referenced_declaration = node.referenced_declaration
                 assert isinstance(referenced_declaration, (DeclarationAbc, SourceUnit))
                 return {
                     path + (referenced_declaration,)
                     for path in resolve_node(node.expression)
                 }
+            elif isinstance(node, FunctionCall):
+                function_called = node.function_called
+                if function_called is None:
+                    return set()
+                elif isinstance(
+                    function_called, (GlobalSymbolsEnum, VariableDeclaration)
+                ):
+                    # global function or variable getter called
+                    # variable getter may return different type than variable declaration (structs with arrays and mappings)
+                    # return empty set for now
+                    return set()
+                elif isinstance(function_called, FunctionDefinition):
+                    # cannot be handled in the current implementation, return empty set for now
+                    return set()
+                elif isinstance(function_called, StructDefinition):
+                    return {(function_called,)}
+                else:
+                    assert False, f"Unexpected node type: {type(node)}\n{self.source}"
             else:
                 assert False, f"Unexpected node type: {type(node)}\n{self.source}"
 
         node = self.left_expression
         if isinstance(node, TupleExpression):
             return tuple(
                 resolve_node(expression) if expression is not None else None
```

### Comparing `woke-3.4.2/woke/ast/ir/expression/binary_operation.py` & `woke-3.5.0/woke/ast/ir/expression/binary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/conditional.py` & `woke-3.5.0/woke/ast/ir/expression/conditional.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/elementary_type_name_expression.py` & `woke-3.5.0/woke/ast/ir/expression/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/function_call.py` & `woke-3.5.0/woke/ast/ir/expression/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/function_call_options.py` & `woke-3.5.0/woke/ast/ir/expression/function_call_options.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/identifier.py` & `woke-3.5.0/woke/ast/ir/expression/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/index_access.py` & `woke-3.5.0/woke/ast/ir/expression/index_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/index_range_access.py` & `woke-3.5.0/woke/ast/ir/expression/index_range_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/literal.py` & `woke-3.5.0/woke/ast/ir/expression/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/member_access.py` & `woke-3.5.0/woke/ast/ir/expression/member_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/new_expression.py` & `woke-3.5.0/woke/ast/ir/expression/new_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/tuple_expression.py` & `woke-3.5.0/woke/ast/ir/expression/tuple_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/expression/unary_operation.py` & `woke-3.5.0/woke/ast/ir/expression/unary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/identifier_path.py` & `woke-3.5.0/woke/ast/ir/meta/identifier_path.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/import_directive.py` & `woke-3.5.0/woke/ast/ir/meta/import_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/inheritance_specifier.py` & `woke-3.5.0/woke/ast/ir/meta/inheritance_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/modifier_invocation.py` & `woke-3.5.0/woke/ast/ir/meta/modifier_invocation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/override_specifier.py` & `woke-3.5.0/woke/ast/ir/meta/override_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/parameter_list.py` & `woke-3.5.0/woke/ast/ir/meta/parameter_list.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/pragma_directive.py` & `woke-3.5.0/woke/ast/ir/meta/pragma_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/source_unit.py` & `woke-3.5.0/woke/ast/ir/meta/source_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/structured_documentation.py` & `woke-3.5.0/woke/ast/ir/meta/structured_documentation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/try_catch_clause.py` & `woke-3.5.0/woke/ast/ir/meta/try_catch_clause.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/meta/using_for_directive.py` & `woke-3.5.0/woke/ast/ir/meta/using_for_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/abc.py` & `woke-3.5.0/woke/ast/ir/statement/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/block.py` & `woke-3.5.0/woke/ast/ir/statement/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/break_statement.py` & `woke-3.5.0/woke/ast/ir/statement/break_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/continue_statement.py` & `woke-3.5.0/woke/ast/ir/statement/continue_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/do_while_statement.py` & `woke-3.5.0/woke/ast/ir/statement/do_while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/emit_statement.py` & `woke-3.5.0/woke/ast/ir/statement/emit_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/expression_statement.py` & `woke-3.5.0/woke/ast/ir/statement/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/for_statement.py` & `woke-3.5.0/woke/ast/ir/statement/for_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/if_statement.py` & `woke-3.5.0/woke/ast/ir/statement/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/inline_assembly.py` & `woke-3.5.0/woke/ast/ir/statement/inline_assembly.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/placeholder_statement.py` & `woke-3.5.0/woke/ast/ir/statement/placeholder_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/return_statement.py` & `woke-3.5.0/woke/ast/ir/statement/return_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/revert_statement.py` & `woke-3.5.0/woke/ast/ir/statement/revert_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/try_statement.py` & `woke-3.5.0/woke/ast/ir/statement/try_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/unchecked_block.py` & `woke-3.5.0/woke/ast/ir/statement/unchecked_block.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/variable_declaration_statement.py` & `woke-3.5.0/woke/ast/ir/statement/variable_declaration_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/statement/while_statement.py` & `woke-3.5.0/woke/ast/ir/statement/while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/type_name/abc.py` & `woke-3.5.0/woke/ast/ir/type_name/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/type_name/array_type_name.py` & `woke-3.5.0/woke/ast/ir/type_name/array_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/type_name/elementary_type_name.py` & `woke-3.5.0/woke/ast/ir/type_name/elementary_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/type_name/function_type_name.py` & `woke-3.5.0/woke/ast/ir/type_name/function_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/type_name/mapping.py` & `woke-3.5.0/woke/ast/ir/type_name/mapping.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/type_name/user_defined_type_name.py` & `woke-3.5.0/woke/ast/ir/type_name/user_defined_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/utils/init_tuple.py` & `woke-3.5.0/woke/ast/ir/utils/init_tuple.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/__init__.py` & `woke-3.5.0/woke/ast/ir/yul/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/abc.py` & `woke-3.5.0/woke/ast/ir/yul/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/assignment.py` & `woke-3.5.0/woke/ast/ir/yul/assignment.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/block.py` & `woke-3.5.0/woke/ast/ir/yul/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/case_statement.py` & `woke-3.5.0/woke/ast/ir/yul/case_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/expression_statement.py` & `woke-3.5.0/woke/ast/ir/yul/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/for_loop.py` & `woke-3.5.0/woke/ast/ir/yul/for_loop.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/function_call.py` & `woke-3.5.0/woke/ast/ir/yul/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/function_definition.py` & `woke-3.5.0/woke/ast/ir/yul/function_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/identifier.py` & `woke-3.5.0/woke/ast/ir/yul/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/if_statement.py` & `woke-3.5.0/woke/ast/ir/yul/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/literal.py` & `woke-3.5.0/woke/ast/ir/yul/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/switch.py` & `woke-3.5.0/woke/ast/ir/yul/switch.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/typed_name.py` & `woke-3.5.0/woke/ast/ir/yul/typed_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/ir/yul/variable_declaration.py` & `woke-3.5.0/woke/ast/ir/yul/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/ast/nodes.py` & `woke-3.5.0/woke/ast/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,14 +316,15 @@
 
 class SolcOrYulNode(AstModel):
     src: Src
 
 
 class SolcNode(SolcOrYulNode):
     id: AstNodeId
+    node_type: str
 
     def __iter__(self):
         def iter_list(l: List):
             for item in l:
                 if isinstance(item, SolcNode):
                     yield item
                     yield from item
```

### Comparing `woke-3.4.2/woke/ast/types.py` & `woke-3.5.0/woke/ast/types.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/cli/__main__.py` & `woke-3.5.0/woke/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import asyncio
 import logging
 import os
 import platform
-from pathlib import Path
-from typing import Optional
 
 import rich.traceback
 import rich_click as click
 from click.core import Context
 from rich.logging import RichHandler
 
-from woke.config import WokeConfig
-
 from .accounts import run_accounts
 from .compile import run_compile
 from .console import console
 from .detect import run_detect
 from .fuzz import run_fuzz
 from .init import run_init
 from .lsp import run_lsp
@@ -82,23 +78,26 @@
 main.add_command(run_test)
 
 
 @main.command(name="config")
 @click.pass_context
 def config(ctx: Context) -> None:
     """Print loaded config options in JSON format."""
+    from woke.config import WokeConfig
+
     config = WokeConfig()
     config.load_configs()
     console.print_json(str(config))
 
 
 def woke_solc() -> None:
     import subprocess
     import sys
 
+    from woke.config import WokeConfig
     from woke.core.solidity_version import SolidityVersion
     from woke.svm import SolcVersionManager
 
     logging.basicConfig(level=logging.CRITICAL)
     config = WokeConfig()
     config.load_configs()
     svm = SolcVersionManager(config)
```

### Comparing `woke-3.4.2/woke/cli/accounts.py` & `woke-3.5.0/woke/cli/accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import json
 from pathlib import Path
 from typing import List, Optional
 
 import rich_click as click
 from click.core import Context
 from rich_click.rich_group import RichGroup
 
-from woke.cli.console import console
-from woke.config import WokeConfig
+from .console import console
 
 
 class NewCommandAlias(RichGroup):
     def get_command(self, ctx: Context, cmd_name: str):
         rv = click.Group.get_command(self, ctx, cmd_name)
         if rv is not None:
             return rv
@@ -30,14 +28,16 @@
 @click.pass_context
 def run_accounts(ctx: Context):
     """
     Run Woke accounts manager.
     """
     from eth_account import Account
 
+    from woke.config import WokeConfig
+
     config = WokeConfig()
     config.load_configs()
     ctx.obj["config"] = config
 
     Account.enable_unaudited_hdwallet_features()
 
 
@@ -70,14 +70,16 @@
     hd_path: str,
     keystore: Optional[str],
     alias: str,
 ):
     """
     Create a new account.
     """
+    import json
+
     from eth_account import Account
     from eth_utils.address import to_checksum_address
 
     if keystore is None:
         path = Path(ctx.obj["config"].global_data_path) / "keystore"
     else:
         path = Path(keystore)
@@ -119,14 +121,16 @@
 )
 @click.argument("alias")
 @click.pass_context
 def accounts_remove(ctx: Context, keystore: Optional[str], alias: str):
     """
     Remove an account.
     """
+    import json
+
     from eth_utils.address import to_checksum_address
 
     if keystore is None:
         path = Path(ctx.obj["config"].global_data_path) / "keystore"
     else:
         path = Path(keystore)
     if not path.is_dir():
@@ -148,14 +152,16 @@
     "--keystore", type=click.Path(exists=True, file_okay=False), help="Keystore path"
 )
 @click.pass_context
 def accounts_list(ctx: Context, keystore: Optional[str]):
     """
     List all accounts.
     """
+    import json
+
     from eth_utils.address import to_checksum_address
 
     if keystore is None:
         path = Path(ctx.obj["config"].global_data_path) / "keystore"
     else:
         path = Path(keystore)
     if not path.is_dir():
@@ -191,14 +197,16 @@
     hd_path: str,
     keystore: Optional[str],
     alias: str,
 ):
     """
     Import an account from a private key or mnemonic.
     """
+    import json
+
     from eth_account import Account
     from eth_utils.address import to_checksum_address
 
     if keystore is None:
         path = Path(ctx.obj["config"].global_data_path) / "keystore"
     else:
         path = Path(keystore)
@@ -248,14 +256,16 @@
 )
 @click.argument("alias")
 @click.pass_context
 def accounts_export(ctx: Context, keystore: Optional[str], alias: str):
     """
     Export an account's private key.
     """
+    import json
+
     from eth_account import Account
     from eth_utils.address import to_checksum_address
 
     if keystore is None:
         path = Path(ctx.obj["config"].global_data_path) / "keystore"
     else:
         path = Path(keystore)
```

### Comparing `woke-3.4.2/woke/cli/compile.py` & `woke-3.5.0/woke/cli/compile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+from __future__ import annotations
+
 import asyncio
 import sys
 import time
 from pathlib import Path
-from typing import Set, Tuple
+from typing import TYPE_CHECKING, Optional, Set, Tuple
 
 import rich_click as click
 from click.core import Context
 
-from woke.config import WokeConfig
+if TYPE_CHECKING:
+    from woke.config import WokeConfig
 
 
 async def compile(
     config: WokeConfig,
     paths: Tuple[str],
     no_artifacts: bool,
     no_warnings: bool,
     force: bool,
     watch: bool,
+    incremental: Optional[bool],
 ):
     from watchdog.observers import Observer
 
     from woke.compiler.compiler import (
         CompilationFileSystemEventHandler,
         SolidityCompiler,
     )
@@ -28,36 +32,14 @@
 
     from ..compiler.solc_frontend import SolcOutputErrorSeverityEnum
     from ..utils.file_utils import is_relative_to
     from .console import console
 
     compiler = SolidityCompiler(config)
 
-    if watch:
-        fs_handler = CompilationFileSystemEventHandler(
-            config,
-            asyncio.get_event_loop(),
-            compiler,
-            [SolcOutputSelectionEnum.ALL],
-            write_artifacts=not no_artifacts,
-            console=console,
-            no_warnings=no_warnings,
-        )
-
-        observer = Observer()
-        observer.schedule(
-            fs_handler,
-            str(config.project_root_path),
-            recursive=True,
-        )
-        observer.start()
-    else:
-        fs_handler = None
-        observer = None
-
     sol_files: Set[Path] = set()
     start = time.perf_counter()
     with console.status("[bold green]Searching for *.sol files...[/]"):
         if len(paths) == 0:
             for file in config.project_root_path.rglob("**/*.sol"):
                 if (
                     not any(
@@ -87,25 +69,49 @@
                 else:
                     raise ValueError(f"Argument `{p}` is not a file or directory.")
     end = time.perf_counter()
     console.log(
         f"[green]Found {len(sol_files)} *.sol files in [bold green]{end - start:.2f} s[/bold green][/]"
     )
 
+    if watch:
+        fs_handler = CompilationFileSystemEventHandler(
+            config,
+            sol_files,
+            asyncio.get_event_loop(),
+            compiler,
+            [SolcOutputSelectionEnum.ALL],
+            write_artifacts=not no_artifacts,
+            console=console,
+            no_warnings=no_warnings,
+        )
+
+        observer = Observer()
+        observer.schedule(
+            fs_handler,
+            str(config.project_root_path),
+            recursive=True,
+        )
+        observer.start()
+    else:
+        fs_handler = None
+        observer = None
+
     if not force:
         compiler.load(console=console)
 
     # TODO Allow choosing build artifacts subset in compile subcommand
     _, errors = await compiler.compile(
         sol_files,
         [SolcOutputSelectionEnum.ALL],
         write_artifacts=not no_artifacts,
         force_recompile=force,
         console=console,
         no_warnings=no_warnings,
+        incremental=incremental,
     )
 
     if watch:
         assert fs_handler is not None
         assert observer is not None
         try:
             await fs_handler.run()
@@ -143,21 +149,33 @@
 @click.option(
     "--watch",
     "-w",
     is_flag=True,
     default=False,
     help="Watch for changes in the project and recompile on change.",
 )
+@click.option(
+    "--incremental/--no-incremental",
+    is_flag=True,
+    required=False,
+    default=None,
+    help="Enforce incremental or non-incremental compilation.",
+)
 @click.pass_context
 def run_compile(
     ctx: Context,
     paths: Tuple[str],
     no_artifacts: bool,
     no_warnings: bool,
     force: bool,
     watch: bool,
+    incremental: Optional[bool],
 ) -> None:
     """Compile the project."""
+    from woke.config import WokeConfig
+
     config = WokeConfig()
     config.load_configs()  # load ~/.woke/config.toml and ./woke.toml
 
-    asyncio.run(compile(config, paths, no_artifacts, no_warnings, force, watch))
+    asyncio.run(
+        compile(config, paths, no_artifacts, no_warnings, force, watch, incremental)
+    )
```

### Comparing `woke-3.4.2/woke/cli/detect.py` & `woke-3.5.0/woke/cli/detect.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/cli/fuzz.py` & `woke-3.5.0/woke/cli/fuzz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-import importlib.resources
-import importlib.util
-import inspect
 import multiprocessing
-import shutil
 import sys
 from pathlib import Path
 from typing import Callable, Iterable, Tuple
 
 import rich_click as click
 
-from woke.config import WokeConfig
-
 from .console import console
 
 
 def _get_module_name(path: Path, root: Path) -> str:
     path = path.with_suffix("")
     return ".".join(path.relative_to(root).parts)
 
@@ -48,15 +42,19 @@
     paths: Tuple[str],
     process_count: int,
     coverage: int,
     seeds: Tuple[str],
     passive: bool,
 ) -> None:
     """Run a Woke test using multiple processes."""
+    import importlib.util
+    import inspect
+    import shutil
 
+    from woke.config import WokeConfig
     from woke.testing.fuzzing.fuzzer import fuzz
 
     if coverage == -1:
         coverage = process_count
 
     if process_count < coverage:
         raise ValueError("Coverage must be less than or equal to process count.")
```

### Comparing `woke-3.4.2/woke/cli/init.py` & `woke-3.5.0/woke/cli/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations
+
 import asyncio
 import sys
 import time
 from pathlib import Path
-from typing import Set
+from typing import TYPE_CHECKING, Set
 
 import rich_click as click
 from click.core import Context
 
-from woke.config import WokeConfig
+if TYPE_CHECKING:
+    from woke.config import WokeConfig
 
 
 def write_config(config: WokeConfig) -> None:
     with config.project_root_path.joinpath("woke.toml").open("w") as f:
         f.write("[compiler.solc]\n")
         f.write('ignore_paths = ["node_modules", ".woke-build", "venv", "lib"]\n')
         f.write('include_paths = ["node_modules"]\n')
@@ -78,14 +81,16 @@
 @click.group(name="init", invoke_without_command=True)
 @click.option(
     "--force", "-f", is_flag=True, default=False, help="Force overwrite existing files."
 )
 @click.pass_context
 def run_init(ctx: Context, force: bool):
     """Initialize project."""
+    from woke.config import WokeConfig
+
     config = WokeConfig()
     config.load_configs()
     ctx.obj["config"] = config
 
     if ctx.invoked_subcommand is None:
         import subprocess
 
@@ -246,17 +251,34 @@
             type_generator = TypeGenerator(config, return_tx)
             type_generator.generate_types(compiler)
         end = time.perf_counter()
         console.log(f"[green]Generated pytypes in [bold green]{end - start:.2f} s[/]")
 
     compiler = SolidityCompiler(config)
 
+    sol_files: Set[Path] = set()
+    start = time.perf_counter()
+    with console.status("[bold green]Searching for *.sol files...[/]"):
+        for file in config.project_root_path.rglob("**/*.sol"):
+            if (
+                not any(
+                    is_relative_to(file, p) for p in config.compiler.solc.ignore_paths
+                )
+                and file.is_file()
+            ):
+                sol_files.add(file)
+    end = time.perf_counter()
+    console.log(
+        f"[green]Found {len(sol_files)} *.sol files in [bold green]{end - start:.2f} s[/bold green][/]"
+    )
+
     if watch:
         fs_handler = CompilationFileSystemEventHandler(
             config,
+            sol_files,
             asyncio.get_event_loop(),
             compiler,
             [SolcOutputSelectionEnum.ALL],
             write_artifacts=True,
             console=console,
             no_warnings=not warnings,
         )
@@ -269,30 +291,14 @@
             recursive=True,
         )
         observer.start()
     else:
         fs_handler = None
         observer = None
 
-    sol_files: Set[Path] = set()
-    start = time.perf_counter()
-    with console.status("[bold green]Searching for *.sol files...[/]"):
-        for file in config.project_root_path.rglob("**/*.sol"):
-            if (
-                not any(
-                    is_relative_to(file, p) for p in config.compiler.solc.ignore_paths
-                )
-                and file.is_file()
-            ):
-                sol_files.add(file)
-    end = time.perf_counter()
-    console.log(
-        f"[green]Found {len(sol_files)} *.sol files in [bold green]{end - start:.2f} s[/bold green][/]"
-    )
-
     compiler.load(console=console)
 
     _, errors = await compiler.compile(
         sol_files,
         [SolcOutputSelectionEnum.ALL],
         write_artifacts=True,
         force_recompile=False,
```

### Comparing `woke-3.4.2/woke/cli/lsp.py` & `woke-3.5.0/woke/cli/lsp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from __future__ import annotations
+
 import asyncio
 import logging
+from typing import TYPE_CHECKING
 
 import rich_click as click
 
-from woke.config import WokeConfig
+if TYPE_CHECKING:
+    from woke.config import WokeConfig
+
 
 logger = logging.getLogger(__name__)
 
 
 async def run_server(config: WokeConfig, port: int) -> None:
     from woke.lsp.server import LspServer
 
@@ -30,11 +35,13 @@
 @click.command(name="lsp")
 @click.option("--port", default=65432, type=int, help="Port to listen on.")
 @click.pass_context
 def run_lsp(context: click.Context, port: int):
     """
     Start the LSP server.
     """
+    from woke.config import WokeConfig
+
     config = WokeConfig()
     config.load_configs()  # load ~/.woke/config.toml and ./woke.toml
 
     asyncio.run(run_server(config, port))
```

### Comparing `woke-3.4.2/woke/cli/run.py` & `woke-3.5.0/woke/cli/run.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/cli/svm.py` & `woke-3.5.0/woke/cli/svm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+from __future__ import annotations
+
 import asyncio
-from typing import Tuple
+from typing import TYPE_CHECKING, Tuple
 
 import rich_click as click
 from click import Context
 from rich.progress import Progress
 
-from woke.config import WokeConfig
-from woke.core.solidity_version import SolidityVersion, SolidityVersionExpr
-from woke.svm import SolcVersionManager
-
 from .console import console
 
+if TYPE_CHECKING:
+    from woke.config import WokeConfig
+    from woke.core.solidity_version import SolidityVersionExpr
+    from woke.svm import SolcVersionManager
+
 
 @click.group(name="svm")
 @click.pass_context
 def run_svm(ctx: Context):
     """Run Woke Solc Version Manager."""
+    from woke.config import WokeConfig
+
     config = WokeConfig()
     config.load_configs()
     ctx.obj["config"] = config
 
 
 @run_svm.command(name="install")
 @click.argument("version_range", nargs=-1)
@@ -28,14 +33,17 @@
     "-f",
     is_flag=True,
     help="Reinstall the target version if already installed.",
 )
 @click.pass_context
 def svm_install(ctx: Context, version_range: Tuple[str], force: bool) -> None:
     """Install the latest solc version matching the given version range."""
+    from woke.core.solidity_version import SolidityVersionExpr
+    from woke.svm import SolcVersionManager
+
     config: WokeConfig = ctx.obj["config"]
     svm = SolcVersionManager(config)
     version_expr = SolidityVersionExpr(" ".join(version_range))
 
     asyncio.run(run_solc_install(svm, version_expr, force))
 
 
@@ -64,14 +72,17 @@
 
 
 @run_svm.command(name="switch")
 @click.argument("version", nargs=1)
 @click.pass_context
 def svm_switch(ctx: Context, version: str) -> None:
     """Switch to the target version of solc. Raise an exception if the version is not installed."""
+    from woke.core.solidity_version import SolidityVersion
+    from woke.svm import SolcVersionManager
+
     config: WokeConfig = ctx.obj["config"]
     svm = SolcVersionManager(config)
     parsed_version = SolidityVersion.fromstring(version)
 
     if not svm.installed(parsed_version):
         raise ValueError(f"solc version {parsed_version} is not installed.")
 
@@ -86,14 +97,17 @@
     "-f",
     is_flag=True,
     help="Reinstall the target version if already installed.",
 )
 @click.pass_context
 def svm_use(ctx: Context, version_range: Tuple[str], force: bool) -> None:
     """Install the target solc version and use it as the global version."""
+    from woke.core.solidity_version import SolidityVersionExpr
+    from woke.svm import SolcVersionManager
+
     config: WokeConfig = ctx.obj["config"]
     svm = SolcVersionManager(config)
     version_expr = SolidityVersionExpr(" ".join(version_range))
     version = next(
         version for version in reversed(svm.list_all()) if version in version_expr
     )
 
@@ -107,14 +121,16 @@
 @run_svm.command(name="list")  # TODO alias `ls`
 @click.option(
     "--all", is_flag=True, help="List all versions including non-installed ones."
 )
 @click.pass_context
 def svm_list(ctx: Context, all: bool) -> None:
     """List installed solc versions."""
+    from woke.svm import SolcVersionManager
+
     config: WokeConfig = ctx.obj["config"]
     svm = SolcVersionManager(config)
     if all:
         installed = set(svm.list_installed())
         output = "\n".join(
             f"- {version} {'([green]installed[/green])' if version in installed else ''}"
             for version in svm.list_all()
@@ -130,14 +146,17 @@
     "--ignore-missing",
     is_flag=True,
     help="do not raise an exception if version to be removed is not installed",
 )
 @click.pass_context
 def svm_remove(ctx: Context, version: str, ignore_missing: bool) -> None:
     """Remove the target solc version."""
+    from woke.core.solidity_version import SolidityVersion
+    from woke.svm import SolcVersionManager
+
     config: WokeConfig = ctx.obj["config"]
     svm = SolcVersionManager(config)
     parsed_version = SolidityVersion.fromstring(version)
 
     if ignore_missing:
         try:
             svm.remove(parsed_version)
```

### Comparing `woke-3.4.2/woke/cli/test.py` & `woke-3.5.0/woke/cli/test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,32 @@
-import json
 import sys
-from typing import Tuple
+from typing import List, Tuple
 
+import click.shell_completion as shell_completion
 import rich_click as click
 
 
-@click.command(name="test")
+class FileAndPassParamType(click.ParamType):
+    name = "file_and_pass"
+
+    def convert(self, value, param, ctx):
+        return value
+
+    def shell_complete(
+        self, ctx: click.Context, param: click.Parameter, incomplete: str
+    ) -> List:
+        return [shell_completion.CompletionItem(incomplete, type="file")]
+
+
+@click.command(
+    name="test",
+    context_settings=dict(
+        ignore_unknown_options=True,
+    ),
+)
 @click.option(
     "--debug", "-d", is_flag=True, default=False, help="Attach debugger on exception."
 )
 @click.option(
     "--s/--no-s",
     "-s",
     is_flag=True,
@@ -18,15 +35,15 @@
 )
 @click.option(
     "--coverage/--no-coverage",
     is_flag=True,
     default=False,
     help="Create coverage report.",
 )
-@click.argument("pytest_args", nargs=-1, type=click.UNPROCESSED)
+@click.argument("pytest_args", nargs=-1, type=FileAndPassParamType())
 @click.pass_context
 def run_test(
     context: click.Context,
     debug: bool,
     s: bool,
     coverage: bool,
     pytest_args: Tuple[str, ...],
```

### Comparing `woke-3.4.2/woke/compiler/build_data_model.py` & `woke-3.5.0/woke/compiler/build_data_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,13 +50,14 @@
     source_units_info: Dict[str, SourceUnitInfo]
     allow_paths: FrozenSet[Path]
     ignore_paths: FrozenSet[Path]
     include_paths: FrozenSet[Path]
     settings: SolcInputSettings
     target_solidity_version: Optional[SolidityVersion]
     woke_version: str
+    incremental: bool
 
 
 class ProjectBuild(NamedTuple):
     interval_trees: Dict[Path, IntervalTree]
     reference_resolver: ReferenceResolver
     source_units: Dict[Path, SourceUnit]
```

### Comparing `woke-3.4.2/woke/compiler/compilation_unit.py` & `woke-3.5.0/woke/compiler/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/compiler/compiler.py` & `woke-3.5.0/woke/compiler/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import pickle
 import time
 from collections import defaultdict, deque
 from contextlib import nullcontext
 from json import JSONDecodeError
 from pathlib import Path
+from types import MappingProxyType
 from typing import (
     Callable,
     Collection,
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
@@ -77,14 +78,15 @@
 # pyright: reportGeneralTypeIssues=false
 
 logger = logging.getLogger(__name__)
 
 
 class CompilationFileSystemEventHandler(FileSystemEventHandler):
     _config: WokeConfig
+    _files: Set[Path]
     _config_path: Path
     _compiler: SolidityCompiler
     _output_types: Collection[SolcOutputSelectionEnum]
     _write_artifacts: bool
     _console: Optional[rich.console.Console]
     _no_warnings: bool
     _created_files: Set[Path]
@@ -96,23 +98,25 @@
     _callbacks: List[Callable[[ProjectBuild, ProjectBuildInfo], None]]
 
     TIMEOUT_INTERVAL = 1.0
 
     def __init__(
         self,
         config: WokeConfig,
+        files: Iterable[Path],
         loop: asyncio.AbstractEventLoop,
         compiler: SolidityCompiler,
         output_types: Collection[SolcOutputSelectionEnum],
         *,
         write_artifacts: bool = True,
         console: Optional[rich.console.Console] = None,
         no_warnings: bool = False,
     ):
         self._config = config
+        self._files = set(files)
         self._loop = loop
         self._config_path = config.project_root_path / "woke.toml"
         self._compiler = compiler
         self._output_types = output_types
         self._write_artifacts = write_artifacts
         self._console = console
         self._no_warnings = no_warnings
@@ -181,16 +185,14 @@
                 self._loop.call_soon_threadsafe(self._queue.put_nowait, event)
         else:
             file = Path(event.src_path)
             if file == self._config_path or file.suffix == ".sol":
                 self._loop.call_soon_threadsafe(self._queue.put_nowait, event)
 
     async def _compile(self):
-        assert self._compiler.latest_build_info is not None
-
         if self._config_changed:
             self._config.load_configs()
 
             # find files that were previously ignored but are now included
             ctx_manager = (
                 self._console.status("[bold green]Searching for *.sol files...[/]")
                 if self._console
@@ -212,18 +214,15 @@
             if self._console is not None:
                 self._console.log(
                     f"[green]Found {len(files)} *.sol files in [bold green]{end - start:.2f} s[/bold green][/]"
                 )
 
             deleted_files = self._deleted_files
         else:
-            files = {
-                unit_info.fs_path
-                for unit_info in self._compiler.latest_build_info.source_units_info.values()
-            }
+            files = self._files.copy()
             files.update(self._created_files)
             files.update(self._modified_files)
             ignored_files = {
                 f
                 for f in files
                 if any(
                     is_relative_to(f, p)
@@ -249,14 +248,15 @@
         self._deleted_files.clear()
         self._config_changed = False
 
     def _on_created(self, file: Path):
         if file == self._config_path:
             self._config_changed = True
         elif file.suffix == ".sol":
+            self._files.add(file)
             if file in self._deleted_files:
                 self._deleted_files.remove(file)
                 self._modified_files.add(file)
             else:
                 logger.debug(f"File {file} created")
                 self._created_files.add(file)
 
@@ -267,14 +267,18 @@
             logger.debug(f"File {file} modified")
             self._modified_files.add(file)
 
     def _on_deleted(self, file: Path):
         if file == self._config_path:
             self._config_changed = True
         elif file.suffix == ".sol":
+            try:
+                self._files.remove(file)
+            except KeyError:
+                pass
             if file in self._modified_files:
                 self._modified_files.remove(file)
 
             if file in self._created_files:
                 self._created_files.remove(file)
             else:
                 logger.debug(f"File {file} deleted")
@@ -287,38 +291,44 @@
     __solc_frontend: SolcFrontend
     __source_unit_name_resolver: SourceUnitNameResolver
     __source_path_resolver: SourcePathResolver
 
     _latest_build_info: Optional[ProjectBuildInfo]
     _latest_build: Optional[ProjectBuild]
     _latest_graph: Optional[nx.DiGraph]
+    _latest_source_units_to_paths: Optional[Dict[str, Path]]
 
     def __init__(self, woke_config: WokeConfig):
         self.__config = woke_config
         self.__svm = SolcVersionManager(woke_config)
         self.__solc_frontend = SolcFrontend(woke_config)
         self.__source_unit_name_resolver = SourceUnitNameResolver(woke_config)
         self.__source_path_resolver = SourcePathResolver(woke_config)
 
         self._latest_build_info = None
         self._latest_build = None
         self._latest_graph = None
+        self._latest_source_units_to_paths = None
 
     @property
     def latest_build_info(self) -> Optional[ProjectBuildInfo]:
         return self._latest_build_info
 
     @property
     def latest_build(self) -> Optional[ProjectBuild]:
         return self._latest_build
 
     @property
     def latest_graph(self) -> Optional[nx.DiGraph]:
         return self._latest_graph
 
+    @property
+    def latest_source_units_to_paths(self) -> Optional[MappingProxyType[str, Path]]:
+        return MappingProxyType(self._latest_source_units_to_paths)
+
     def build_graph(
         self,
         files: Iterable[Path],
         modified_files: Mapping[Path, str],
         ignore_errors: bool = False,
     ) -> Tuple[nx.DiGraph, Dict[str, Path]]:
         # source unit name, full path, file content
@@ -714,21 +724,27 @@
         force_recompile: bool = False,
         modified_files: Optional[Mapping[Path, str]] = None,
         deleted_files: Optional[
             Set[Path]
         ] = None,  # files that should be treated as deleted even if they exist
         console: Optional[rich.console.Console] = None,
         no_warnings: bool = False,
-        merge_compilation_units: bool = False,
+        incremental: Optional[bool] = None,
     ) -> Tuple[ProjectBuild, Set[SolcOutputError]]:
         if modified_files is None:
             modified_files = {}
         if deleted_files is None:
             deleted_files = set()
 
+        if incremental is None:
+            if force_recompile or self._latest_build_info is None:
+                incremental = True
+            else:
+                incremental = self._latest_build_info.incremental
+
         # validate target solc version (if set)
         target_version = self.__config.compiler.solc.target_version
         min_version = self.__config.min_solidity_version
         max_version = self.__config.max_solidity_version
         if target_version is not None and target_version < min_version:
             raise CompilationError(
                 f"Target configured version {target_version} is lower than minimum supported version {min_version}"
@@ -741,27 +757,29 @@
         graph, source_units_to_paths = self.build_graph(
             files, modified_files, ignore_errors=True
         )
         compilation_units = self.build_compilation_units_maximize(graph)
         build_settings = self.create_build_settings(output_types)
 
         self._latest_graph = graph
+        self._latest_source_units_to_paths = source_units_to_paths
 
         build_settings_changed = False
         if self._latest_build_info is not None:
             if (
                 self._latest_build_info.allow_paths
                 != self.__config.compiler.solc.allow_paths
                 or self._latest_build_info.ignore_paths
                 != self.__config.compiler.solc.ignore_paths
                 or self._latest_build_info.include_paths
                 != self.__config.compiler.solc.include_paths
                 or self._latest_build_info.settings != build_settings
                 or self._latest_build_info.target_solidity_version
                 != self.__config.compiler.solc.target_version
+                or self._latest_build_info.incremental != incremental
             ):
                 logger.debug("Build settings changed")
                 build_settings_changed = True
 
         errors_per_cu: DefaultDict[bytes, Set[SolcOutputError]] = defaultdict(set)
 
         if (
@@ -776,15 +794,15 @@
                 reference_resolver=ReferenceResolver(),
                 source_units={},
             )
             files_to_compile = set(
                 source_units_to_paths[source_unit] for source_unit in graph.nodes
             )
 
-            if merge_compilation_units:
+            if not incremental:
                 compilation_units = self._merge_compilation_units(
                     compilation_units, graph
                 )
         else:
             # TODO this is not needed? graph contains hash of modified files
             # files_to_compile = set(modified_files.keys())
             files_to_compile = set()
@@ -799,15 +817,15 @@
                 ):
                     files_to_compile.add(source_units_to_paths[source_unit])
 
             for source_unit, info in self._latest_build_info.source_units_info.items():
                 if source_unit not in graph.nodes:
                     deleted_files.add(info.fs_path)
 
-            if merge_compilation_units:
+            if not incremental:
                 compilation_units = self._merge_compilation_units(
                     compilation_units, graph
                 )
 
             for cu_hash, cu_data in self._latest_build_info.compilation_units.items():
                 if any(cu.hash.hex() == cu_hash for cu in compilation_units):
                     errors_per_cu[bytes.fromhex(cu_hash)] = set(cu_data.errors)
@@ -873,18 +891,19 @@
 
         ctx_manager = (
             console.status(f"[bold green]Processing compilation results...[/]")
             if console
             else nullcontext()
         )
         start = time.perf_counter()
-        processed_files: Set[Path] = set()
 
         with ctx_manager:
             successful_compilation_units = []
+            all_errored_files: Set[Path] = set()
+
             for cu, solc_output in zip(compilation_units, ret):
                 errored_files: Set[Path] = set()
                 errors_per_cu[cu.hash] = set()
 
                 for error in solc_output.errors:
                     errors_per_cu[cu.hash].add(error)
                     if error.severity == SolcOutputErrorSeverityEnum.ERROR:
@@ -894,31 +913,74 @@
                             )
                             errored_files.add(path)
                         else:
                             # whole compilation unit errored
                             errored_files |= cu.files
 
                 self._out_edge_bfs(cu, errored_files, errored_files)
+                all_errored_files |= errored_files
 
                 for file in errored_files:
                     if file in build.source_units:
                         build.reference_resolver.run_destroy_callbacks(file)
                         build.source_units.pop(file)
                     if file in build.interval_trees:
                         build.interval_trees.pop(file)
 
                 if len(errored_files) == 0:
                     successful_compilation_units.append((cu, solc_output))
 
+            # files_to_compile and files importing them
+            files_to_recompile = set(
+                graph.nodes[n[1]]["path"]  # pyright: ignore reportGeneralTypeIssues
+                for n in nx.edge_bfs(
+                    graph,
+                    [
+                        source_unit_name
+                        for source_unit_name in graph.nodes  # pyright: ignore reportGeneralTypeIssues
+                        if graph.nodes[source_unit_name]["path"]
+                        in files_to_compile  # pyright: ignore reportGeneralTypeIssues
+                    ],
+                )
+            ) | set(files_to_compile)
+
+            # destroy callbacks for IR nodes that will be replaced by new ones must be executed before
+            # new IR nodes are created
+            for file in files_to_recompile:
+                if file in build.source_units:
+                    build.reference_resolver.run_destroy_callbacks(file)
+                    build.source_units.pop(file)
+                if file in build.interval_trees:
+                    build.interval_trees.pop(file)
+
+            # clear indexed node types responsible for handling multiple structurally different ASTs for the same file
+            build.reference_resolver.clear_indexed_nodes(files_to_recompile)
+
+            source_units_info = {
+                str(source_unit): SourceUnitInfo(
+                    graph.nodes[source_unit]["path"], graph.nodes[source_unit]["hash"]
+                )
+                for source_unit in graph.nodes
+                if graph.nodes[source_unit]["path"] not in deleted_files
+                and graph.nodes[source_unit]["path"] not in all_errored_files
+                and graph.nodes[source_unit]["path"] not in files_to_recompile
+            }
+
+            processed_files: Set[Path] = set()
             for cu, solc_output in successful_compilation_units:
                 # files requested to be compiled and files that import these files (even indirectly)
                 recompiled_files: Set[Path] = set()
                 self._out_edge_bfs(cu, files_to_compile & cu.files, recompiled_files)
 
                 for source_unit_name, raw_ast in solc_output.sources.items():
+                    source_units_info[source_unit_name] = SourceUnitInfo(
+                        graph.nodes[source_unit_name]["path"],
+                        graph.nodes[source_unit_name]["hash"],
+                    )
+
                     path = cu.source_unit_name_to_path(source_unit_name)
                     ast = AstSolc.parse_obj(raw_ast.ast)
 
                     build.reference_resolver.register_source_file_id(
                         raw_ast.id, path, cu.hash
                     )
                     build.reference_resolver.index_nodes(ast, path, cu.hash)
@@ -939,15 +1001,14 @@
                         cu,
                         interval_tree,
                         build.reference_resolver,
                         solc_output.contracts[source_unit_name]
                         if source_unit_name in solc_output.contracts
                         else None,
                     )
-                    build.reference_resolver.run_destroy_callbacks(path)
                     build.source_units[path] = SourceUnit(init, ast)
                     build.interval_trees[path] = interval_tree
 
                 build.reference_resolver.run_post_process_callbacks(
                     CallbackParams(
                         interval_trees=build.interval_trees,
                         source_units=build.source_units,
@@ -965,22 +1026,18 @@
                 cu_hash.hex(): CompilationUnitBuildInfo(errors=list(errors))
                 for cu_hash, errors in errors_per_cu.items()
             },
             allow_paths=self.__config.compiler.solc.allow_paths,
             ignore_paths=self.__config.compiler.solc.ignore_paths,
             include_paths=self.__config.compiler.solc.include_paths,
             settings=build_settings,
-            source_units_info={
-                str(source_unit): SourceUnitInfo(
-                    graph.nodes[source_unit]["path"], graph.nodes[source_unit]["hash"]
-                )
-                for source_unit in graph.nodes
-            },
+            source_units_info=source_units_info,
             target_solidity_version=self.__config.compiler.solc.target_version,
             woke_version=get_package_version("woke"),
+            incremental=incremental,
         )
         self._latest_build = build
 
         if write_artifacts and (
             len(compilation_units) > 0 or len(deleted_files) > 0 or force_recompile
         ):
             logger.debug("Writing artifacts")
```

### Comparing `woke-3.4.2/woke/compiler/solc_frontend/input_data_model.py` & `woke-3.5.0/woke/compiler/solc_frontend/input_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/compiler/solc_frontend/output_data_model.py` & `woke-3.5.0/woke/compiler/solc_frontend/output_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/compiler/solc_frontend/solc_runner.py` & `woke-3.5.0/woke/compiler/solc_frontend/solc_runner.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/compiler/source_path_resolver.py` & `woke-3.5.0/woke/compiler/source_path_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/compiler/source_unit_name_resolver.py` & `woke-3.5.0/woke/compiler/source_unit_name_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/config/__init__.py` & `woke-3.5.0/woke/config/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/config/data_model.py` & `woke-3.5.0/woke/config/data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/config/woke_config.py` & `woke-3.5.0/woke/config/woke_config.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/contracts/woke/console.sol` & `woke-3.5.0/woke/contracts/woke/console.sol`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/core/solidity_version.py` & `woke-3.5.0/woke/core/solidity_version.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/deployment/__init__.py` & `woke-3.5.0/woke/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/deployment/core.py` & `woke-3.5.0/woke/deployment/core.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/blocks.py` & `woke-3.5.0/woke/development/blocks.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/call_trace.py` & `woke-3.5.0/woke/development/call_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import importlib
-import reprlib
 from collections import ChainMap
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, cast
 
 import eth_abi
 import eth_abi.abi
 import eth_abi.exceptions
 import eth_utils
@@ -226,15 +225,15 @@
                 )
             )
 
         if self.kind != CallTraceKind.INTERNAL:
             if self.arguments is not None:
                 ret.append("(")
                 for i, arg in enumerate(self.arguments):
-                    t = Text(reprlib.repr(arg))
+                    t = Text(repr(arg))
                     ReprHighlighter().highlight(t)
                     ret.append_text(t)
                     if i < len(self.arguments) - 1:
                         ret.append(", ")
                 ret.append(")")
             else:
                 ret.append("(???)")
@@ -715,28 +714,31 @@
 
                 current_trace._subtraces.append(call_trace)
                 call_trace._parent = current_trace
                 current_trace = call_trace
                 contracts.append(fqn)
                 values.append(value)
                 fqn_overrides.maps.insert(0, {})
-            elif log["op"] in {"RETURN", "REVERT", "STOP", "SELFDESTRUCT"}:
-                if log["op"] == "REVERT":
+            elif log["op"] in {"INVALID", "RETURN", "REVERT", "STOP", "SELFDESTRUCT"}:
+                if log["op"] in {"INVALID", "REVERT"}:
                     status = False
                 else:
                     status = True
 
                 assert current_trace is not None
                 while current_trace._kind == CallTraceKind.INTERNAL:
                     current_trace._status = status
                     current_trace = current_trace._parent
                     assert current_trace is not None
 
                 assert current_trace is not None
-                if log["op"] != "REVERT" and len(fqn_overrides.maps) > 1:
+                if (
+                    log["op"] not in {"INVALID", "REVERT"}
+                    and len(fqn_overrides.maps) > 1
+                ):
                     fqn_overrides.maps[1].update(fqn_overrides.maps[0])
                 fqn_overrides.maps.pop(0)
 
                 if current_trace.kind in {CallTraceKind.CREATE, CallTraceKind.CREATE2}:
                     try:
                         address = Address(
                             int(trace["structLogs"][i + 1]["stack"][-1], 16)
```

### Comparing `woke-3.4.2/woke/development/chain_interfaces.py` & `woke-3.5.0/woke/development/chain_interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -421,14 +421,28 @@
                 self._encode_block_identifier(block_identifier),
             ],
         )
 
     def trace_transaction(self, tx_hash: str) -> List:
         return self._communicator.send_request("trace_transaction", [tx_hash])
 
+    def get_storage_at(
+        self, address: str, position: int, block_identifier: Union[int, str] = "latest"
+    ) -> bytes:
+        return bytes.fromhex(
+            self._communicator.send_request(
+                "eth_getStorageAt",
+                [
+                    address,
+                    hex(position),
+                    self._encode_block_identifier(block_identifier),
+                ],
+            )[2:]
+        )
+
     @abstractmethod
     def get_accounts(self) -> List[str]:
         ...
 
     @abstractmethod
     def get_automine(self) -> bool:
         ...
@@ -473,14 +487,22 @@
     def set_next_block_base_fee_per_gas(self, value: int) -> None:
         ...
 
     @abstractmethod
     def set_min_gas_price(self, value: int) -> None:
         ...
 
+    @abstractmethod
+    def set_storage_at(self, address: str, position: int, value: bytes) -> None:
+        ...
+
+    @abstractmethod
+    def mine_many(self, num_blocks: int, timestamp_change: Optional[int]) -> None:
+        ...
+
 
 class HardhatChainInterface(ChainInterfaceAbc):
     def get_accounts(self) -> List[str]:
         return self._communicator.send_request("eth_accounts")
 
     def set_balance(self, address: str, value: int) -> None:
         self._communicator.send_request("hardhat_setBalance", [address, hex(value)])
@@ -528,14 +550,27 @@
         self._communicator.send_request(
             "hardhat_setNextBlockBaseFeePerGas", [hex(value)]
         )
 
     def set_min_gas_price(self, value: int) -> None:
         self._communicator.send_request("hardhat_setMinGasPrice", [hex(value)])
 
+    def set_storage_at(self, address: str, position: int, value: bytes) -> None:
+        self._communicator.send_request(
+            "hardhat_setStorageAt", [address, hex(position), "0x" + value.hex()]
+        )
+
+    def mine_many(self, num_blocks: int, timestamp_change: Optional[int]) -> None:
+        self._communicator.send_request(
+            "hardhat_mine",
+            [hex(num_blocks), hex(timestamp_change)]
+            if timestamp_change is not None
+            else [hex(num_blocks)],
+        )
+
 
 class AnvilChainInterface(ChainInterfaceAbc):
     def get_accounts(self) -> List[str]:
         return self._communicator.send_request("eth_accounts")
 
     def set_balance(self, address: str, value: int) -> None:
         self._communicator.send_request("anvil_setBalance", [address, hex(value)])
@@ -579,17 +614,30 @@
 
     def set_next_block_base_fee_per_gas(self, value: int) -> None:
         self._communicator.send_request("anvil_setNextBlockBaseFeePerGas", [hex(value)])
 
     def set_min_gas_price(self, value: int) -> None:
         self._communicator.send_request("anvil_setMinGasPrice", [hex(value)])
 
+    def set_storage_at(self, address: str, position: int, value: bytes) -> None:
+        self._communicator.send_request(
+            "anvil_setStorageAt", [address, hex(position), "0x" + value.hex()]
+        )
+
     def node_info(self) -> Dict[str, Any]:
         return self._communicator.send_request("anvil_nodeInfo")
 
+    def mine_many(self, num_blocks: int, timestamp_change: Optional[int]) -> None:
+        self._communicator.send_request(
+            "anvil_mine",
+            [hex(num_blocks), hex(timestamp_change)]
+            if timestamp_change is not None
+            else [hex(num_blocks)],
+        )
+
 
 class GanacheChainInterface(ChainInterfaceAbc):
     def get_accounts(self) -> List[str]:
         return self._communicator.send_request("eth_accounts")
 
     def set_balance(self, address: str, value: int) -> None:
         self._communicator.send_request("evm_setAccountBalance", [address, hex(value)])
@@ -638,14 +686,29 @@
         raise NotImplementedError(
             "Ganache does not support setting next block base fee per gas"
         )
 
     def set_min_gas_price(self, value: int) -> None:
         self._communicator.send_request("miner_setGasPrice", [hex(value)])
 
+    def set_storage_at(self, address: str, position: int, value: bytes) -> None:
+        self._communicator.send_request(
+            "evm_setAccountStorageAt", [address, hex(position), "0x" + value.hex()]
+        )
+
+    def mine_many(self, num_blocks: int, timestamp_change: Optional[int]) -> None:
+        if timestamp_change is not None:
+            raise NotImplementedError(
+                "Ganache does not support timestamp intervals when mining multiple blocks"
+            )
+        self._communicator.send_request(
+            "evm_mine",
+            [{"blocks": num_blocks}],
+        )
+
 
 class GethLikeChainInterfaceAbc(ChainInterfaceAbc, ABC):
     @property
     @abstractmethod
     def _name(self) -> str:
         ...
 
@@ -694,14 +757,20 @@
         )
 
     def set_min_gas_price(self, value: int) -> None:
         raise NotImplementedError(
             f"{self._name} does not support setting min gas price"
         )
 
+    def set_storage_at(self, address: str, position: int, value: bytes) -> None:
+        raise NotImplementedError(f"{self._name} does not support setting storage")
+
+    def mine_many(self, num_blocks: int, timestamp_change: Optional[int]) -> None:
+        raise NotImplementedError(f"{self._name} does not support mining blocks")
+
 
 class GethChainInterface(GethLikeChainInterfaceAbc):
     @property
     def _name(self) -> str:
         return "Geth"
 
     def get_accounts(self) -> List[str]:
```

### Comparing `woke-3.4.2/woke/development/constants.py` & `woke-3.5.0/woke/development/constants.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/core.py` & `woke-3.5.0/woke/development/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,26 @@
     Any,
     Callable,
     DefaultDict,
     Dict,
     Iterable,
     List,
     Optional,
+    Sequence,
     Set,
     Tuple,
     Type,
     Union,
     cast,
 )
 from urllib.error import HTTPError
 
 import eth_abi
 import eth_abi.abi
+import eth_abi.grammar
 import eth_abi.packed
 import eth_account
 import eth_account.messages
 import eth_utils
 from Crypto.Hash import BLAKE2b, keccak
 from typing_extensions import (
     Annotated,
@@ -124,42 +126,76 @@
 
 def fix_library_abi(args: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
     ret = []
     for arg in args:
         arg = deepcopy(arg)
         if arg["type"] == "tuple":
             fix_library_abi(arg["components"])
-        elif arg["internalType"].startswith("contract "):
-            arg["type"] = "address"
-        elif arg["internalType"].startswith("enum "):
-            arg["type"] = "uint8"
+        elif "internalType" in arg:
+            # internalType was added in 0.5.11
+            # versions before 0.5.11 are not supported by Woke anyway
+            # but we may fetch ABIs generated by an older version of solc through Etherscan
+            if arg["internalType"].startswith("contract "):
+                # replace contract type with "address" but keep array suffix (if any)
+                arg["type"] = arg["type"].replace(
+                    arg["type"].split("[", 1)[0], "address"
+                )
+            elif arg["internalType"].startswith("enum "):
+                # replace enum type with "uint8" but keep array suffix (if any)
+                arg["type"] = arg["type"].replace(arg["type"].split("[", 1)[0], "uint8")
         ret.append(arg)
     return ret
 
 
 class Abi:
     @staticmethod
-    def _normalize_arguments(arguments: Iterable) -> List:
+    def _normalize_input(arguments: Iterable) -> List:
         ret = []
         for arg in arguments:
             if isinstance(arg, Address):
                 ret.append(str(arg))
             elif isinstance(arg, Account):
                 ret.append(str(arg.address))
+            elif isinstance(arg, (list, tuple)):
+                ret.append(Abi._normalize_input(arg))
             else:
                 ret.append(arg)
         return ret
 
+    @staticmethod
+    def _normalize_output(types: Sequence[str], arguments: Sequence) -> Tuple:
+        ret = []
+        assert len(types) == len(arguments)
+        for type, arg in zip(types, arguments):
+            type = type.strip()
+            if type == "address":
+                ret.append(Address(arg))
+            elif type.endswith("]"):
+                args_type = type[: type.rfind("[")]
+                assert isinstance(arg, (list, tuple))
+                ret.append(Abi._normalize_output([args_type] * len(arg), arg))
+            elif type.startswith("(") and type.endswith(")"):
+                abi_type = eth_abi.grammar.parse(type)
+                assert isinstance(abi_type, eth_abi.grammar.TupleType)
+                ret.append(
+                    Abi._normalize_output(
+                        [c.to_type_str() for c in abi_type.components], arg
+                    )
+                )
+            else:
+                ret.append(arg)
+        return tuple(ret)
+
     @classmethod
     def encode(cls, types: Iterable, arguments: Iterable) -> bytes:
-        return eth_abi.abi.encode(types, cls._normalize_arguments(arguments))
+        return eth_abi.abi.encode(types, cls._normalize_input(arguments))
 
     @classmethod
     def encode_packed(cls, types: Iterable, arguments: Iterable) -> bytes:
-        return eth_abi.packed.encode_packed(types, cls._normalize_arguments(arguments))
+        return eth_abi.packed.encode_packed(types, cls._normalize_input(arguments))
 
     @classmethod
     def encode_with_selector(
         cls, selector: bytes, types: Iterable, arguments: Iterable
     ) -> bytes:
         return selector + cls.encode(types, arguments)
 
@@ -206,16 +242,16 @@
                     "inputs"
                 ]
             )
         ]
         return cls.encode_with_selector(selector, types, arguments)
 
     @classmethod
-    def decode(cls, types: Iterable, data: bytes) -> Any:
-        return eth_abi.abi.decode(types, data)
+    def decode(cls, types: Sequence[str], data: bytes) -> Any:
+        return cls._normalize_output(types, eth_abi.abi.decode(types, data))
 
 
 class Wei(int):
     def to_ether(self) -> float:
         return self / 10**18
 
     def to_gwei(self) -> float:
@@ -1490,14 +1526,18 @@
     @check_connected
     def set_next_block_base_fee_per_gas(self, value: Union[int, str]) -> None:
         if isinstance(value, str):
             value = Wei.from_str(value)
         self._chain_interface.set_next_block_base_fee_per_gas(value)
 
     @check_connected
+    def set_next_block_timestamp(self, timestamp: int) -> None:
+        self._chain_interface.set_next_block_timestamp(timestamp)
+
+    @check_connected
     def set_min_gas_price(self, value: Union[int, str]) -> None:
         if isinstance(value, str):
             value = Wei.from_str(value)
         self._chain_interface.set_min_gas_price(value)
         self.gas_price = value
 
     @check_connected
@@ -1532,14 +1572,20 @@
             last_timestamp = int(block_info["timestamp"], 16)
             timestamp = timestamp_change(last_timestamp)
         else:
             timestamp = None
 
         self._chain_interface.mine(timestamp)
 
+    @check_connected
+    def mine_many(
+        self, num_blocks: int, timestamp_change: Optional[int] = None
+    ) -> None:
+        self._chain_interface.mine_many(num_blocks, timestamp_change)
+
     @contextmanager
     def snapshot_and_revert(self):
         snapshot_id = self.snapshot()
         try:
             yield
         except Exception as e:
             if not isinstance(e, BdbQuit):
@@ -1650,16 +1696,14 @@
             ]
             return expected_type(*converted_values)
         elif isinstance(expected_type, type):
             if issubclass(expected_type, Contract):
                 return expected_type(value, self)
             elif issubclass(expected_type, Account):
                 return Account(value, self)
-            elif issubclass(expected_type, Address):
-                return expected_type(value)
             elif issubclass(expected_type, IntEnum):
                 return expected_type(value)
         return value
 
     def _process_revert_data(
         self,
         tx: Optional[TransactionAbc],
@@ -2254,20 +2298,20 @@
             length = int(trace["stack"][-3], 16)
             creation_code = read_from_memory(offset, length, trace["memory"])
 
             trace_is_create.append(True)
             addresses.append(None)
             fqns.append(get_fqn_from_creation_code(creation_code)[0])
             fqn_overrides.maps.insert(0, {})
-        elif trace["op"] in {"RETURN", "REVERT", "STOP", "SELFDESTRUCT"}:
+        elif trace["op"] in {"INVALID", "RETURN", "REVERT", "STOP", "SELFDESTRUCT"}:
             if trace["op"] == "SELFDESTRUCT":
                 if addresses[-1] is not None:
                     fqn_overrides.maps[0][addresses[-1]] = None
 
-            if trace["op"] != "REVERT" and len(fqn_overrides.maps) > 1:
+            if trace["op"] not in {"INVALID", "REVERT"} and len(fqn_overrides.maps) > 1:
                 fqn_overrides.maps[1].update(fqn_overrides.maps[0])
             fqn_overrides.maps.pop(0)
             addresses.pop()
 
             if trace_is_create.pop():
                 try:
                     addr = Address(
@@ -2326,22 +2370,26 @@
             length = int(trace["stack"][-3], 16)
             creation_code = read_from_memory(offset, length, trace["memory"])
 
             trace_is_create.append(True)
             addresses.append(None)
             fqns.append(get_fqn_from_creation_code(creation_code)[0])
             fqn_overrides.maps.insert(0, {})
-        elif trace["op"] == "REVERT":
+        elif trace["op"] in {"INVALID", "REVERT"}:
             pc = trace["pc"]
             fqn_overrides.maps.pop(0)
             fqn = fqns.pop()
             addresses.pop()
             trace_is_create.pop()
 
-            if fqn in contracts_revert_index and pc in contracts_revert_index[fqn]:
+            if (
+                trace["op"] == "REVERT"
+                and fqn in contracts_revert_index
+                and pc in contracts_revert_index[fqn]
+            ):
                 last_revert_origin = fqn
         elif trace["op"] in {"RETURN", "STOP", "SELFDESTRUCT"}:
             if len(fqn_overrides.maps) > 1:
                 fqn_overrides.maps[1].update(fqn_overrides.maps[0])
             fqn_overrides.maps.pop(0)
             addresses.pop()
 
@@ -2407,16 +2455,16 @@
             length = int(trace["stack"][-3], 16)
             creation_code = read_from_memory(offset, length, trace["memory"])
 
             trace_is_create.append(True)
             addresses.append(None)
             fqns.append(get_fqn_from_creation_code(creation_code)[0])
             fqn_overrides.maps.insert(0, {})
-        elif trace["op"] in {"RETURN", "REVERT", "STOP", "SELFDESTRUCT"}:
-            if trace["op"] != "REVERT" and len(fqn_overrides.maps) > 1:
+        elif trace["op"] in {"INVALID", "RETURN", "REVERT", "STOP", "SELFDESTRUCT"}:
+            if trace["op"] not in {"INVALID", "REVERT"} and len(fqn_overrides.maps) > 1:
                 fqn_overrides.maps[1].update(fqn_overrides.maps[0])
             fqn_overrides.maps.pop(0)
             addresses.pop()
 
             if trace_is_create.pop():
                 try:
                     addr = Address(
```

### Comparing `woke-3.4.2/woke/development/globals.py` & `woke-3.5.0/woke/development/globals.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/hardhat_console.py` & `woke-3.5.0/woke/development/hardhat_console.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/internal.py` & `woke-3.5.0/woke/development/internal.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/json_rpc/communicator.py` & `woke-3.5.0/woke/development/json_rpc/communicator.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/json_rpc/http.py` & `woke-3.5.0/woke/development/json_rpc/http.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/json_rpc/ipc.py` & `woke-3.5.0/woke/development/json_rpc/ipc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/primitive_types.py` & `woke-3.5.0/woke/development/primitive_types.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/development/pytypes_generator.py` & `woke-3.5.0/woke/development/pytypes_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,21 +539,26 @@
 
         for item in compilation_info.abi:
             if item["type"] == "function":
                 if contract.kind == ContractKind.LIBRARY:
                     item_copy = deepcopy(item)
                     for arg in item_copy["inputs"]:
                         if arg["internalType"].startswith("contract "):
-                            arg["type"] = arg["internalType"][9:]
+                            arg["internalType"] = arg["internalType"][9:]
                         elif arg["internalType"].startswith("struct "):
-                            arg["type"] = arg["internalType"][7:]
+                            arg["internalType"] = arg["internalType"][7:]
                         elif arg["internalType"].startswith("enum "):
-                            arg["type"] = arg["internalType"][5:]
+                            arg["internalType"] = arg["internalType"][5:]
 
-                    selector = eth_utils.abi.function_abi_to_4byte_selector(item_copy)
+                    selector = keccak.new(
+                        data=f"{item['name']}({','.join(arg['internalType'] for arg in item_copy['inputs'])})".encode(
+                            "utf-8"
+                        ),
+                        digest_bits=256,
+                    ).digest()[:4]
                 else:
                     selector = eth_utils.abi.function_abi_to_4byte_selector(item)
                 abi_by_selector[selector] = item
             elif item["type"] == "error":
                 selector = eth_utils.abi.function_abi_to_4byte_selector(item)
 
                 if selector not in self.__errors_index:
@@ -1579,32 +1584,32 @@
             self.__current_source_unit = source_unit.source_unit_name
             self.generate_types_source_unit(source_unit)
             self.write_source_unit_to_file(source_unit.source_unit_name)
             self.cleanup_source_unit()
             self.__name_sanitizer.clear_global_renames()
 
         build = compiler.latest_build
-        build_info = compiler.latest_build_info
         assert build is not None
-        assert build_info is not None
         self.__interval_trees = build.interval_trees
         self.__source_units = build.source_units
         self.__reference_resolver = build.reference_resolver
 
         self.clean_type_dir()
 
         # generate source units in import order, source units with no imports are generated first
         # also handle cyclic imports
         assert compiler.latest_graph is not None
+        assert compiler.latest_source_units_to_paths
         graph: nx.DiGraph = (
             compiler.latest_graph.copy()
         )  # pyright: ignore reportGeneralTypeIssues
+        source_units_to_paths = compiler.latest_source_units_to_paths
         paths_to_source_unit_names: DefaultDict[Path, Set[str]] = defaultdict(set)
-        for source_unit_name, info in build_info.source_units_info.items():
-            paths_to_source_unit_names[info.fs_path].add(source_unit_name)
+        for source_unit, path in source_units_to_paths.items():
+            paths_to_source_unit_names[path].add(source_unit)
 
         previous_len = len(graph)
         cycles_detected = False
         cycles: Set[FrozenSet[str]] = set()
 
         for cycle in nx.simple_cycles(graph):
             for source_unit_name in cycle:
@@ -1620,15 +1625,15 @@
                 if in_degree == 0
             ]
             heapq.heapify(sources)
             visited: Set[str] = set(sources)
 
             while len(sources) > 0:
                 source = heapq.heappop(sources)
-                path = build_info.source_units_info[source].fs_path
+                path = source_units_to_paths[source]
                 if path in self.__source_units:
                     generate_source_unit(self.__source_units[path])
 
                 for source_unit_name in paths_to_source_unit_names[path]:
                     visited.add(source_unit_name)
                     for (
                         _,
@@ -1666,15 +1671,15 @@
                         break
 
                 if is_closed_cycle:
                     generated_cycles.add(frozenset(cycle))
 
             for cycle in sorted(generated_cycles):
                 for source in cycle:
-                    path = build_info.source_units_info[source].fs_path
+                    path = source_units_to_paths[source]
                     if path in self.__source_units:
                         generate_source_unit(self.__source_units[path])
                     graph.remove_nodes_from(paths_to_source_unit_names[path])
 
             if len(graph) == previous_len:
                 break
             previous_len = len(graph)
```

### Comparing `woke-3.4.2/woke/development/transactions.py` & `woke-3.5.0/woke/development/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -765,18 +765,36 @@
 class ExceptionWrapper:
     value: Optional[Exception] = None
 
 
 @contextmanager
 def must_revert(
     exceptions: Union[
-        Exception, Type[Exception], Tuple[Union[Exception, Type[Exception]], ...]
+        str,
+        int,
+        Exception,
+        Type[Exception],
+        Tuple[Union[str, int, Exception, Type[Exception]], ...],
     ] = TransactionRevertedError,
 ) -> Iterator[ExceptionWrapper]:
+    if isinstance(exceptions, str):
+        exceptions = Error(exceptions)
+    elif isinstance(exceptions, int):
+        exceptions = Panic(PanicCodeEnum(exceptions))
+
     if isinstance(exceptions, (tuple, list)):
+        tmp: List[Union[str, int, Exception, Type[Exception]]] = []
+        for ex in exceptions:
+            if isinstance(ex, str):
+                tmp.append(Error(ex))
+            elif isinstance(ex, int):
+                tmp.append(Panic(PanicCodeEnum(ex)))
+            else:
+                tmp.append(ex)
+        exceptions = tuple(tmp)
         types = tuple(type(x) if not inspect.isclass(x) else x for x in exceptions)
     else:
         types = type(exceptions) if not inspect.isclass(exceptions) else exceptions
 
     wrapper = ExceptionWrapper()
 
     try:
@@ -796,18 +814,36 @@
             if not inspect.isclass(exceptions):
                 assert e == exceptions, f"Expected {e} but got {exceptions}"
 
 
 @contextmanager
 def may_revert(
     exceptions: Union[
-        Exception, Type[Exception], Tuple[Union[Exception, Type[Exception]], ...]
+        str,
+        int,
+        Exception,
+        Type[Exception],
+        Tuple[Union[str, int, Exception, Type[Exception]], ...],
     ] = TransactionRevertedError,
 ) -> Iterator[ExceptionWrapper]:
+    if isinstance(exceptions, str):
+        exceptions = Error(exceptions)
+    elif isinstance(exceptions, int):
+        exceptions = Panic(PanicCodeEnum(exceptions))
+
     if isinstance(exceptions, (tuple, list)):
+        tmp: List[Union[str, int, Exception, Type[Exception]]] = []
+        for ex in exceptions:
+            if isinstance(ex, str):
+                tmp.append(Error(ex))
+            elif isinstance(ex, int):
+                tmp.append(Panic(PanicCodeEnum(ex)))
+            else:
+                tmp.append(ex)
+        exceptions = tuple(tmp)
         types = tuple(type(x) if not inspect.isclass(x) else x for x in exceptions)
     else:
         types = type(exceptions) if not inspect.isclass(exceptions) else exceptions
 
     wrapper = ExceptionWrapper()
 
     try:
```

### Comparing `woke-3.4.2/woke/development/utils.py` & `woke-3.5.0/woke/development/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/commands/generate_control_flow_graph.py` & `woke-3.5.0/woke/lsp/commands/generate_control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/commands/generate_imports_graph.py` & `woke-3.5.0/woke/lsp/commands/generate_imports_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/commands/generate_inheritance_graph.py` & `woke-3.5.0/woke/lsp/commands/generate_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/commands/generate_linearized_inheritance_graph.py` & `woke-3.5.0/woke/lsp/commands/generate_linearized_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/common_structures.py` & `woke-3.5.0/woke/lsp/common_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/context.py` & `woke-3.5.0/woke/lsp/context.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/document_sync.py` & `woke-3.5.0/woke/lsp/document_sync.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/code_action.py` & `woke-3.5.0/woke/lsp/features/code_action.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/code_lens.py` & `woke-3.5.0/woke/lsp/features/code_lens.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/completion.py` & `woke-3.5.0/woke/lsp/features/completion.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/definition.py` & `woke-3.5.0/woke/lsp/features/definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/diagnostic.py` & `woke-3.5.0/woke/lsp/features/diagnostic.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/document_link.py` & `woke-3.5.0/woke/lsp/features/document_link.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/document_symbol.py` & `woke-3.5.0/woke/lsp/features/document_symbol.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/hover.py` & `woke-3.5.0/woke/lsp/features/hover.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/implementation.py` & `woke-3.5.0/woke/lsp/features/implementation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/references.py` & `woke-3.5.0/woke/lsp/features/references.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/rename.py` & `woke-3.5.0/woke/lsp/features/rename.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/type_definition.py` & `woke-3.5.0/woke/lsp/features/type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/features/type_hierarchy.py` & `woke-3.5.0/woke/lsp/features/type_hierarchy.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/lsp_compiler.py` & `woke-3.5.0/woke/lsp/lsp_compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -626,16 +626,19 @@
                 else:
                     await self.__svm.install(version)
 
         for compilation_unit in skipped_compilation_units:
             for file in compilation_unit.files:
                 # clear diagnostics
                 await self.__diagnostic_queue.put((file, set()))
-                self.__interval_trees.pop(file, None)
-                self.__source_units.pop(file, None)
+                if file in self.__interval_trees:
+                    self.__interval_trees.pop(file)
+                if file in self.__source_units:
+                    self.__ir_reference_resolver.run_destroy_callbacks(file)
+                    self.__source_units.pop(file)
             compilation_units.remove(compilation_unit)
 
         progress_token = await self.__server.progress_begin(
             "Compiling", f"0/{len(compilation_units)}", 0
         )
 
         tasks = []
@@ -703,110 +706,148 @@
             for file in self.__discovered_files:
                 # clear diagnostics
                 await self.__diagnostic_queue.put((file, set()))
             self.__interval_trees.clear()
             self.__source_units.clear()
             return
 
-        files_to_recompile = set(files_to_compile)
-        processed_files: Set[Path] = set()
+        # files passed as files_to_compile and files importing them
+        files_to_recompile = set(
+            graph.nodes[n[1]]["path"]  # pyright: ignore reportGeneralTypeIssues
+            for n in nx.edge_bfs(
+                graph,
+                [
+                    source_unit_name
+                    for source_unit_name in graph.nodes  # pyright: ignore reportGeneralTypeIssues
+                    if graph.nodes[  # pyright: ignore reportGeneralTypeIssues
+                        source_unit_name
+                    ][  # pyright: ignore reportGeneralTypeIssues
+                        "path"
+                    ]
+                    in files_to_compile  # pyright: ignore reportGeneralTypeIssues
+                ],
+            )
+        ) | set(files_to_compile)
 
         for deleted_file in self.__deleted_files:
             await self.__diagnostic_queue.put((deleted_file, []))
             if deleted_file in self.__source_units:
                 self.__ir_reference_resolver.run_destroy_callbacks(deleted_file)
                 self.__source_units.pop(deleted_file)
 
-        for cu_index, (cu, solc_output) in enumerate(zip(compilation_units, ret)):
+        successful_compilation_units = []
+        for cu, solc_output in zip(compilation_units, ret):
             for file in cu.files:
                 if file in self.__line_indexes:
                     self.__line_indexes.pop(file)
                 if file in self.__opened_files:
                     self.__output_contents[file] = self.__opened_files[file]
 
             errored_files: Set[Path] = set()
 
             for error in solc_output.errors:
                 if error.source_location is not None:
                     path = cu.source_unit_name_to_path(error.source_location.file)
                     errors_per_file[path].add(
-                        self.__solc_error_to_diagnostic(error, path)
+                        self.__solc_error_to_diagnostic(error, path, cu)
                     )
                     if error.severity == SolcOutputErrorSeverityEnum.ERROR:
                         errored_files.add(path)
+                else:
+                    # whole compilation unit errored
+                    if error.severity == SolcOutputErrorSeverityEnum.ERROR:
+                        errored_files.update(cu.files)
 
             _out_edge_bfs(cu, errored_files, errored_files)
 
-            # files requested to be compiled and files that import these files (even indirectly)
-            recompiled_files: Set[Path] = set()
-            _out_edge_bfs(cu, files_to_compile & cu.files, recompiled_files)
-
             for file in errored_files:
                 files_to_recompile.discard(file)
                 # an error occurred during compilation
                 # AST still may be provided, but it must NOT be parsed (pydantic model is not defined for this case)
                 if file in self.__source_units:
                     self.__ir_reference_resolver.run_destroy_callbacks(file)
                     self.__source_units.pop(file)
                 if file in self.__interval_trees:
                     self.__interval_trees.pop(file)
 
             if len(errored_files) == 0:
-                for source_unit_name, raw_ast in solc_output.sources.items():
-                    path = cu.source_unit_name_to_path(source_unit_name)
-                    if path in errored_files or raw_ast.ast is None:
-                        continue
-                    ast = AstSolc.parse_obj(raw_ast.ast)
+                successful_compilation_units.append((cu, solc_output))
 
-                    self.__ir_reference_resolver.index_nodes(ast, path, cu.hash)
+        # destroy callbacks for IR nodes that will be replaced by new ones must be executed before
+        # new IR nodes are created
+        callback_processed_files: Set[Path] = set()
+        for cu, solc_output in successful_compilation_units:
+            # files requested to be compiled and files that import these files (even indirectly)
+            recompiled_files: Set[Path] = set()
+            _out_edge_bfs(cu, files_to_compile & cu.files, recompiled_files)
 
-                    files_to_recompile.discard(path)
+            # run destroy callbacks for files that were recompiled and their IR nodes will be replaced
+            for source_unit_name in solc_output.sources.keys():
+                path = cu.source_unit_name_to_path(source_unit_name)
+                if (
+                    path in self.__source_units and path not in recompiled_files
+                ) or path in callback_processed_files:
+                    continue
+                callback_processed_files.add(path)
+                self.__ir_reference_resolver.run_destroy_callbacks(path)
 
-                    # give a chance to other tasks (LSP requests) to be processed
-                    await asyncio.sleep(0)
+        # clear indexed node types responsible for handling multiple structurally different ASTs for the same file
+        self.__ir_reference_resolver.clear_indexed_nodes(files_to_recompile)
 
-                    if (
-                        path in self.__source_units and path not in recompiled_files
-                    ) or path in processed_files:
-                        continue
-                    processed_files.add(path)
-
-                    interval_tree = IntervalTree()
-                    init = IrInitTuple(
-                        path,
-                        self.get_compiled_file(path).text.encode("utf-8"),
-                        cu,
-                        interval_tree,
-                        self.__ir_reference_resolver,
-                        None,
-                    )
-                    self.__ir_reference_resolver.run_destroy_callbacks(path)
-                    self.__source_units[path] = SourceUnit(init, ast)
-                    self.__interval_trees[path] = interval_tree
+        processed_files: Set[Path] = set()
+        for cu_index, (cu, solc_output) in enumerate(successful_compilation_units):
+            # files requested to be compiled and files that import these files (even indirectly)
+            recompiled_files: Set[Path] = set()
+            _out_edge_bfs(cu, files_to_compile & cu.files, recompiled_files)
 
-                    self.__last_compilation_source_units[path] = self.__source_units[
-                        path
-                    ]
-                    self.__last_compilation_interval_trees[
-                        path
-                    ] = self.__interval_trees[path]
+            for source_unit_name, raw_ast in solc_output.sources.items():
+                path: Path = cu.source_unit_name_to_path(source_unit_name)
+                ast = AstSolc.parse_obj(raw_ast.ast)
+
+                self.__ir_reference_resolver.index_nodes(ast, path, cu.hash)
+
+                files_to_recompile.discard(path)
+
+                # give a chance to other tasks (LSP requests) to be processed
+                await asyncio.sleep(0)
+
+                if (
+                    path in self.__source_units and path not in recompiled_files
+                ) or path in processed_files:
+                    continue
+                processed_files.add(path)
+
+                interval_tree = IntervalTree()
+                init = IrInitTuple(
+                    path,
+                    self.get_compiled_file(path).text.encode("utf-8"),
+                    cu,
+                    interval_tree,
+                    self.__ir_reference_resolver,
+                    None,
+                )
+                self.__source_units[path] = SourceUnit(init, ast)
+                self.__interval_trees[path] = interval_tree
 
-                    if path in self.__opened_files:
-                        self.__last_successful_compilation_contents[
-                            path
-                        ] = self.__opened_files[path]
-                    else:
-                        self.__last_successful_compilation_contents[
-                            path
-                        ] = VersionedFile(
-                            cu.graph.nodes[  # pyright: ignore reportGeneralTypeIssues
-                                source_unit_name
-                            ]["content"],
-                            None,
-                        )
+                self.__last_compilation_source_units[path] = self.__source_units[path]
+                self.__last_compilation_interval_trees[path] = self.__interval_trees[
+                    path
+                ]
+
+                if path in self.__opened_files:
+                    self.__last_successful_compilation_contents[
+                        path
+                    ] = self.__opened_files[path]
+                else:
+                    self.__last_successful_compilation_contents[path] = VersionedFile(
+                        cu.graph.nodes[  # pyright: ignore reportGeneralTypeIssues
+                            source_unit_name
+                        ]["content"],
+                        None,
+                    )
 
             self.__ir_reference_resolver.run_post_process_callbacks(
                 CallbackParams(
                     interval_trees=self.__interval_trees,
                     source_units=self.__source_units,
                 )
             )
@@ -992,15 +1033,15 @@
         for line in lines:
             encoded_line = line.encode("utf-8")
             encoded_lines.append((encoded_line, prefix_sum))
             prefix_sum += len(encoded_line)
         self.__line_indexes[file] = encoded_lines
 
     def __solc_error_to_diagnostic(
-        self, error: SolcOutputError, path: Path
+        self, error: SolcOutputError, path: Path, cu: CompilationUnit
     ) -> Diagnostic:
         assert error.source_location is not None
         if error.severity == SolcOutputErrorSeverityEnum.ERROR:
             severity = DiagnosticSeverity.ERROR
         elif error.severity == SolcOutputErrorSeverityEnum.WARNING:
             severity = DiagnosticSeverity.WARNING
         else:
@@ -1012,19 +1053,66 @@
             )
         else:
             range_ = Range(
                 start=Position(line=0, character=0),
                 end=Position(line=0, character=0),
             )
 
-        return Diagnostic(
+        diag = Diagnostic(
             range=range_,
             severity=severity,
             code=error.error_code,
             source="Woke(solc)",
             message=error.message,
         )
+        if (
+            error.secondary_source_locations is not None
+            and len(error.secondary_source_locations) > 0
+        ):
+            related_info = []
+            for secondary_source_location in error.secondary_source_locations:
+                if (
+                    secondary_source_location.file is None
+                    or secondary_source_location.start is None
+                    or secondary_source_location.end is None
+                ):
+                    continue
+
+                if (
+                    secondary_source_location.start >= 0
+                    and secondary_source_location.end >= 0
+                ):
+                    range_ = self.get_range_from_byte_offsets(
+                        cu.source_unit_name_to_path(secondary_source_location.file),
+                        (
+                            secondary_source_location.start,
+                            secondary_source_location.end,
+                        ),
+                    )
+                else:
+                    range_ = Range(
+                        start=Position(line=0, character=0),
+                        end=Position(line=0, character=0),
+                    )
+
+                related_info.append(
+                    DiagnosticRelatedInformation(
+                        location=Location(
+                            uri=DocumentUri(
+                                path_to_uri(
+                                    cu.source_unit_name_to_path(
+                                        secondary_source_location.file
+                                    )
+                                )
+                            ),
+                            range=range_,
+                        ),
+                        message=secondary_source_location.message,
+                    )
+                )
+            diag.related_information = related_info
+        return diag
 
     def __file_ignored(self, path: Path) -> bool:
         return any(
             is_relative_to(path, p) for p in self.__config.compiler.solc.ignore_paths
         )
```

### Comparing `woke-3.4.2/woke/lsp/lsp_parser.py` & `woke-3.5.0/woke/lsp/lsp_parser.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/methods.py` & `woke-3.5.0/woke/lsp/methods.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/protocol_structures.py` & `woke-3.5.0/woke/lsp/protocol_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/rpc_protocol.py` & `woke-3.5.0/woke/lsp/rpc_protocol.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/server.py` & `woke-3.5.0/woke/lsp/server.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/server_capabilities.py` & `woke-3.5.0/woke/lsp/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/lsp/utils/position.py` & `woke-3.5.0/woke/lsp/utils/position.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/regex_parser/solidity_import.py` & `woke-3.5.0/woke/regex_parser/solidity_import.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/regex_parser/solidity_parser.py` & `woke-3.5.0/woke/regex_parser/solidity_parser.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/svm/abc.py` & `woke-3.5.0/woke/svm/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/svm/svm.py` & `woke-3.5.0/woke/svm/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/testing/__init__.py` & `woke-3.5.0/woke/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/testing/core.py` & `woke-3.5.0/woke/testing/core.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/testing/coverage.py` & `woke-3.5.0/woke/testing/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,17 +556,26 @@
                 except ValueError:
                     logger.warning(f"Failed to get contract FQN for {creation_code}")
                     new_fqn = None
 
                 contract_fqn_stack.append(new_fqn)
                 is_deployment_stack.append(True)
                 fqn_overrides.maps.insert(0, {})
-            elif struct_log["op"] in ("RETURN", "STOP", "REVERT", "SELFDESTRUCT"):
+            elif struct_log["op"] in {
+                "INVALID",
+                "RETURN",
+                "STOP",
+                "REVERT",
+                "SELFDESTRUCT",
+            }:
                 logger.debug(f"{pc} {struct_log['op']} before pop {contract_fqn_stack}")
-                if struct_log["op"] != "REVERT" and len(fqn_overrides.maps) > 1:
+                if (
+                    struct_log["op"] not in {"INVALID", "REVERT"}
+                    and len(fqn_overrides.maps) > 1
+                ):
                     fqn_overrides.maps[1].update(fqn_overrides.maps[0])
                 fqn_overrides.maps.pop(0)
 
                 if is_deployment_stack.pop():
                     try:
                         addr = Address(int(trace["structLogs"][i + 1]["stack"][-1], 16))
                         if addr != Address(0):
```

### Comparing `woke-3.4.2/woke/testing/fuzzing/fuzz_test.py` & `woke-3.5.0/woke/testing/fuzzing/fuzz_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import random
 from collections import defaultdict
-from typing import Callable, DefaultDict, List, Optional, Set
+from typing import Callable, DefaultDict, List, Optional
 
 from typing_extensions import get_type_hints
 
 from ..core import get_connected_chains
 from .generators import generate
 
 
@@ -45,34 +45,34 @@
     def sequence_num(self):
         return self._sequence_num
 
     @property
     def flow_num(self):
         return self._flow_num
 
-    def __get_methods(self, attr: str) -> Set[Callable]:
-        ret = set()
+    def __get_methods(self, attr: str) -> List[Callable]:
+        ret = []
         for x in dir(self):
             if hasattr(self.__class__, x):
                 m = getattr(self.__class__, x)
                 if hasattr(m, attr) and getattr(m, attr):
-                    ret.add(m)
+                    ret.append(m)
         return ret
 
     def run(
         self,
         sequences_count: int,
         flows_count: int,
         *,
         dry_run: bool = False,
     ):
         chains = get_connected_chains()
 
-        flows: Set[Callable] = self.__get_methods("flow")
-        invariants: Set[Callable] = self.__get_methods("invariant")
+        flows: List[Callable] = self.__get_methods("flow")
+        invariants: List[Callable] = self.__get_methods("invariant")
 
         for i in range(sequences_count):
             flows_counter: DefaultDict[Callable, int] = defaultdict(int)
             invariant_periods: DefaultDict[Callable[[None], None], int] = defaultdict(
                 int
             )
```

### Comparing `woke-3.4.2/woke/testing/fuzzing/fuzzer.py` & `woke-3.5.0/woke/testing/fuzzing/fuzzer.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/testing/fuzzing/generators.py` & `woke-3.5.0/woke/testing/fuzzing/generators.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/utils/context_managers.py` & `woke-3.5.0/woke/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/utils/decorators.py` & `woke-3.5.0/woke/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/utils/file_utils.py` & `woke-3.5.0/woke/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/utils/openzeppelin.py` & `woke-3.5.0/woke/utils/openzeppelin.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/utils/string.py` & `woke-3.5.0/woke/utils/string.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/utils/tee.py` & `woke-3.5.0/woke/utils/tee.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/woke/utils/threaded_child_watcher.py` & `woke-3.5.0/woke/utils/threaded_child_watcher.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.2/setup.py` & `woke-3.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 entry_points = \
 {'console_scripts': ['woke = woke.cli.__main__:main',
                      'woke-solc = woke.cli.__main__:woke_solc']}
 
 setup_kwargs = {
     'name': 'woke',
-    'version': '3.4.2',
+    'version': '3.5.0',
     'description': 'Woke is a Python-based development and testing framework for Solidity.',
     'long_description': '# Woke\n\nWoke is a Python-based development and testing framework for Solidity.\n\nFeatures:\n\n- **Testing framework** - a testing framework for Solidity smart contracts with Python-native equivalents of Solidity types and blazing fast execution.\n\n- **Fuzzer** - a property-based fuzzer for Solidity smart contracts that allows testers to write their fuzz tests in Python.\n\n- **Vulnerability detectors**\n\n- **LSP server**\n\n## Dependencies\n\n- [Python](https://www.python.org/downloads/release/python-3910/) (version 3.7 or higher)\n\n> :warning: Python 3.11 is experimentally supported.\n\n## Installation\n\nvia `pip`\n\n```shell\npip3 install woke\n```\n\n## Documentation & Contribution\n\nWoke documentation can be found [here](https://ackeeblockchain.com/woke/docs/latest).\n\nThere you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).\n\n## Features\n\n### Testing framework\n\nSee [examples](examples) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.\n\nWriting tests is as simple as:\n\n```python\nfrom woke.testing import *\nfrom pytypes.contracts.Counter import Counter\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n\n    counter = Counter.deploy()\n    assert counter.count() == 0\n\n    counter.increment()\n    assert counter.count() == 1\n```\n\n### Fuzzer\n\nFuzzer builds on top of the testing framework and allows efficient fuzz testing of Solidity smart contracts.\n\n```python\nfrom woke.testing import *\nfrom woke.testing.fuzzing import *\nfrom pytypes.contracts.Counter import Counter\n\nclass CounterTest(FuzzTest):\n    def pre_sequence(self) -> None:\n        self.counter = Counter.deploy()\n        self.count = 0\n\n    @flow()\n    def increment(self) -> None:\n        self.counter.increment()\n        self.count += 1\n\n    @flow()\n    def decrement(self) -> None:\n        with may_revert(Panic(PanicCodeEnum.UNDERFLOW_OVERFLOW)) as e:\n            self.counter.decrement()\n\n        if e.value is not None:\n            assert self.count == 0\n        else:\n            self.count -= 1\n\n    @invariant(period=10)\n    def count(self) -> None:\n        assert self.counter.count() == self.count\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n    CounterTest().run(sequences_count=30, flows_count=100)\n```\n\n### Vulnerability detectors\n\nVulnerability detectors can be run using:\n```shell\nwoke detect\n```\n\n### LSP server\n\nWoke implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.\n\nWoke LSP server can be run using:\n\n```shell\nwoke lsp\n```\n\nOr with an optional --port argument:\n\n```shell\nwoke lsp --port 1234\n```\n\nAll LSP server features can be found in the [documentation](https://ackeeblockchain.com/woke/docs/latest/language-server/).\n\n## License\n\nThis project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/woke/blob/main/LICENSE).\n\n## Partners\n\nRockawayX             |  Coinbase\n:-------------------------:|:-------------------------:\n[![](https://github.com/Ackee-Blockchain/woke/blob/main/images/rockawayx.jpg?raw=true)](https://rockawayx.com/)  |  [![](https://github.com/Ackee-Blockchain/woke/blob/main/images/coinbase.png?raw=true)](https://www.coinbase.com/)\n\n\n\n\n\n\n',
     'author': 'Ackee Blockchain',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ackeeblockchain.com',
```

### Comparing `woke-3.4.2/PKG-INFO` & `woke-3.5.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woke
-Version: 3.4.2
+Version: 3.5.0
 Summary: Woke is a Python-based development and testing framework for Solidity.
 Home-page: https://ackeeblockchain.com
 License: ISC
 Keywords: ethereum,solidity,security,testing,development,framework,audit
 Author: Ackee Blockchain
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved
```

