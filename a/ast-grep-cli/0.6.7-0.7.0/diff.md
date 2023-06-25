# Comparing `tmp/ast_grep_cli-0.6.7.tar.gz` & `tmp/ast_grep_cli-0.7.0.tar.gz`

## Comparing `ast_grep_cli-0.6.7.tar` & `ast_grep_cli-0.7.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1911 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123     1815 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123     1515 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     2024 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123     8546 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123     2879 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     3114 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     2915 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6268 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11320 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    14850 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    10723 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11260 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15357 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2543 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11291 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7552 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 ast_grep_cli-0.6.7/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/config.rs
--rw-r--r--   0     1001      123     9325 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     3596 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     4996 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10196 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/new.rs
--rw-r--r--   0     1001      123    22359 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7258 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3046 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     7800 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/run.rs
--rw-r--r--   0     1001      123     8501 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     5935 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24629 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      901 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1046 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/pyproject.toml
--rw-r--r--   0     1001      123    59508 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4968 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/README.md
--rw-r--r--   0     1001      123     1077 2023-06-23 07:36:23.000000 ast_grep_cli-0.6.7/LICENSE
--rw-r--r--   0        0        0     6214 1970-01-01 00:00:00.000000 ast_grep_cli-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7552 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1911 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123     1815 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123     1515 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     2024 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123     8546 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123     2879 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     3114 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     2915 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3858 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    14850 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    10723 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    15431 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10936 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11291 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6268 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11320 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    11003 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10176 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     3596 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     4996 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10196 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123    22465 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7675 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123     9327 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3179 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     8424 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10361 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     6866 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24629 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      975 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1046 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      123    59913 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4980 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/README.md
+-rw-r--r--   0     1001      123     1077 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/PKG-INFO
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.6.7"
+version= "0.7.0"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
 
@@ -22,15 +22,15 @@
 tree-sitter-css = { version = "0.19.0", optional = true }
 tree-sitter-dart= { version = "0.0.3", optional = true }
 tree-sitter-go = { version = "0.19.1", optional = true }
 tree-sitter-html = { version = "0.19.0", optional = true }
 tree-sitter-java = { version = "0.20.0", optional = true }
 tree-sitter-javascript = { version = "0.20.0", optional = true }
 tree-sitter-kotlin = { version = "0.2.11", optional = true }
-tree-sitter-lua = { version = "0.0.17", optional = true }
+tree-sitter-lua = { version = "0.0.18", optional = true }
 tree-sitter-python = { version = "0.20.2", optional = true }
 tree-sitter-rust = { version = "0.20.3", optional = true }
 tree-sitter-swift = { version = "0.3.6", optional = true }
 tree-sitter-thrift = { version = "0.5.0", optional = true }
 tree-sitter-typescript= { version = "0.20.2", optional = true }
 
 [features]
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/cpp.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/csharp.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/css.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/go.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.6.7"
+version= "0.7.0"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 anyhow = "1.0"
 bit-set= { version = "0.5.3" }
 globset = "0.4.10"
 regex = { version = "1.8.4" , optional = true }
 serde= { version = "1.0", features = ["derive"] }
-serde_yaml = "0.9.21"
+serde_yaml = "0.9.22"
 thiserror= "1.0.40"
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.6.7"
+version= "0.7.0"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
 regex = { version = "1.8.4" , optional = true }
 thiserror= "1.0.40"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files 2% similar despite different names*

```diff
@@ -277,16 +277,16 @@
   if trimmed.starts_with('_') {
     Some(Anonymous(named))
   } else {
     Some(Named(trimmed.to_owned(), named))
   }
 }
 
-fn is_valid_meta_var_char(c: char) -> bool {
-  matches!(c, 'A'..='Z' | '_')
+pub(crate) fn is_valid_meta_var_char(c: char) -> bool {
+  matches!(c, 'A'..='Z' | '_' | '0'..='9')
 }
 
 impl<'tree, L: Language> From<MetaVarEnv<'tree, StrDoc<L>>> for HashMap<String, String> {
   fn from(env: MetaVarEnv<'tree, StrDoc<L>>) -> Self {
     let mut ret = HashMap::new();
     for (id, node) in env.single_matched {
       ret.insert(id, node.text().into());
@@ -317,14 +317,15 @@
   }
   #[test]
   fn test_match_var() {
     use MetaVariable::*;
     assert_eq!(extract_var("$$$"), Some(Ellipsis));
     assert_eq!(extract_var("$ABC"), Some(Named("ABC".into(), true)));
     assert_eq!(extract_var("$$ABC"), Some(Named("ABC".into(), false)));
+    assert_eq!(extract_var("$MATCH1"), Some(Named("MATCH1".into(), true)));
     assert_eq!(extract_var("$$$ABC"), Some(NamedEllipsis("ABC".into())));
     assert_eq!(extract_var("$_"), Some(Anonymous(true)));
     assert_eq!(extract_var("abc"), None);
     assert_eq!(extract_var("$abc"), None);
   }
 
   fn match_constraints(pattern: &str, node: &str) -> bool {
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/node.rs`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     while let Some(n) = node.parent() {
       node = n;
     }
     node == self.inner.root_node()
   }
 
   /// P.S. I am your father.
+  #[doc(hidden)]
   pub unsafe fn readopt<'a: 'b, 'b>(&'a self, node: &mut Node<'b, D>) {
     debug_assert!(self.check_lineage(&node.inner));
     node.root = self;
   }
 }
 
 /// 'r represents root lifetime
@@ -212,14 +213,18 @@
     DisplayContext {
       matched: self.text(),
       leading: &self.root.doc.get_source().as_str()[leading..start],
       trailing: &self.root.doc.get_source().as_str()[end..=trailing],
       start_line: self.inner.start_position().row() as usize + 1,
     }
   }
+
+  pub fn root(&self) -> Self {
+    self.root.root()
+  }
 }
 
 /**
  * Corresponds to inside/has/precedes/follows
  */
 impl<'r, D: Doc> Node<'r, D> {
   pub fn matches<M: Matcher<D::Lang>>(&self, m: M) -> bool {
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use crate::matcher::NodeMatch;
-use crate::meta_var::MetaVariableID;
+use crate::meta_var::{is_valid_meta_var_char, MetaVariableID};
 use crate::source::{Content, Edit as E};
 use crate::Pattern;
 use crate::{Doc, Node, Root};
 
 type Edit<D> = E<<D as Doc>::Source>;
 type Underlying<S> = Vec<<S as Content>::Underlying>;
 
@@ -80,15 +80,15 @@
     }
     if !src.starts_with(meta_char) {
       break (src, false);
     }
   };
   // no Anonymous meta var allowed, so _ is not allowed
   let i = trimmed
-    .find(|c: char| !c.is_ascii_uppercase())
+    .find(|c: char| !is_valid_meta_var_char(c))
     .unwrap_or(trimmed.len());
   // no name found
   if i == 0 {
     return None;
   }
   let name = trimmed[..i].to_string();
   let var = if is_multi {
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.6.7"
+version= "0.7.0"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 ast-grep-config.path = "../ast-grep-config"
 
 dashmap = "5.4.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.97"
+serde_json = "1.0.99"
 tower-lsp = "0.19.0"
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.6.7"
+version= "0.7.0"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.6.7/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/Cargo.toml` & `ast_grep_cli-0.7.0/crates/cli/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 name = "ast-grep"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
+license-file = "../../LICENSE"
 
-version= "0.6.7"
+version= "0.7.0"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 homepage= "https://ast-grep.github.io/"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
@@ -30,18 +31,18 @@
 ast-grep-dynamic.path = "../../local_dependencies/ast-grep-dynamic"
 ast-grep-language.path = "../../local_dependencies/ast-grep-language"
 ast-grep-lsp.path = "../../local_dependencies/ast-grep-lsp"
 
 ansi_term = "0.12"
 anyhow = "1.0"
 atty = "0.2.14"
-clap = { version = "4.3.4", features = ["derive"] }
+clap = { version = "4.3.8", features = ["derive"] }
 codespan-reporting = "0.11.1"
 crossterm = "0.26.1"
 ignore= { version = "0.4.20" }
 inquire = "0.6.2"
 num_cpus = "1.15.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.97"
-serde_yaml = "0.9.21"
+serde_json = "1.0.99"
+serde_yaml = "0.9.22"
 similar = { version = "2.2.1", features = ["inline"] }
 tokio = { version = "1", features = ["rt-multi-thread", "io-std"] }
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/config.rs` & `ast_grep_cli-0.7.0/crates/cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/error.rs` & `ast_grep_cli-0.7.0/crates/cli/src/error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use std::path::PathBuf;
 
 use crate::utils::ansi_link;
 
 const DOC_SITE_HOST: &str = "https://ast-grep.github.io";
 const PATTERN_GUIDE: Option<&str> = Some("/guide/pattern-syntax.html");
 const CONFIG_GUIDE: Option<&str> = Some("/guide/rule-config.html");
+const TOOL_OVERVIEW: Option<&str> = Some("/guide/tooling-overview.html");
 const CLI_USAGE: Option<&str> = Some("/reference/cli.html");
 const TEST_GUIDE: Option<&str> = Some("/guide/test-rule.html");
 const UTIL_GUIDE: Option<&str> = Some("/guide/rule-config/utility-rule.html");
 const EDITOR_INTEGRATION: Option<&str> = Some("/guide/editor-integration.html");
 const PLAYGROUND: Option<&str> = Some("/playground.html");
 
 /// AppError stands for ast-grep command line usage.
@@ -26,16 +27,19 @@
   WalkRuleDir(PathBuf),
   ReadRule(PathBuf),
   ParseRule(PathBuf),
   ParseTest(PathBuf),
   GlobPattern,
   // Run
   ParsePattern,
+  LanguageNotSpecified,
+  StdInIsNotInteractive,
   // Scan
   DiagnosticError(usize),
+  RuleNotSpecified,
   // LSP
   StartLanguageServer,
   // Edit
   OpenEditor,
   WriteFile(PathBuf),
   // Test
   TestFail(String),
@@ -50,18 +54,19 @@
 
 impl ErrorContext {
   fn exit_code(&self) -> i32 {
     use ErrorContext::*;
     // reference: https://mariadb.com/kb/en/operating-system-error-codes/
     match self {
       DiagnosticError(_) => 1,
-      ProjectNotExist => 2,
+      ProjectNotExist | LanguageNotSpecified | RuleNotSpecified => 2,
       TestFail(_) => 3,
       NoTestDirConfigured | NoUtilDirConfigured => 4,
       ReadConfiguration | ReadRule(_) | WalkRuleDir(_) | WriteFile(_) => 5,
+      StdInIsNotInteractive => 6,
       ParseTest(_) | ParseRule(_) | ParseConfiguration | GlobPattern | ParsePattern => 8,
       ProjectAlreadyExist | FileAlreadyExist(_) => 17,
       InsufficientCLIArgument(_) => 22,
       OpenEditor | StartLanguageServer => 126,
     }
   }
 }
@@ -133,18 +138,33 @@
       ),
       DiagnosticError(num) => Self::new(
         format!("{num} error(s) found in code."),
         "Scan succeeded and found error level diagnostics in the codebase.",
         None,
       ),
       ParsePattern => Self::new(
-        "Cannot parse query as a valid pattern",
+        "Cannot parse query as a valid pattern.",
         "The pattern either fails to parse or contains error. Please refer to pattern syntax guide.",
         PATTERN_GUIDE,
       ),
+      LanguageNotSpecified => Self::new(
+        "Language must be specified for code from StdIn.",
+        "Please use `--language` to specify the code language.",
+        TOOL_OVERVIEW,
+      ),
+      StdInIsNotInteractive => Self::new(
+        "Interactive mode is incompatible with parsing code from StdIn.",
+        "`--interactive` needs StdIn, but it is used as source code. Please use files as input.",
+        TOOL_OVERVIEW,
+      ),
+      RuleNotSpecified => Self::new(
+        "Only one rule can scan code from StdIn.",
+        "Please use `--rule path/to/rule.yml` to choose the rule.",
+        TOOL_OVERVIEW,
+      ),
       StartLanguageServer => Self::new(
         "Cannot start language server.",
         "Please see language server logging file.",
         EDITOR_INTEGRATION,
       ),
       OpenEditor => Self::new(
         "Cannot open file in editor.",
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/lang.rs` & `ast_grep_cli-0.7.0/crates/cli/src/lang.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/lib.rs` & `ast_grep_cli-0.7.0/crates/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/lsp.rs` & `ast_grep_cli-0.7.0/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/new.rs` & `ast_grep_cli-0.7.0/crates/cli/src/new.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.7.0/crates/cli/src/print/colored_print.rs`

 * *Files 3% similar despite different names*

```diff
@@ -277,95 +277,90 @@
   styles: &PrintStyles,
   writer: &mut W,
 ) -> Result<()> {
   print_prelude(path, styles, writer)?;
   let Some(first_match) = matches.next() else {
     return Ok(())
   };
-  let source = first_match
-    .ancestors()
-    .last()
-    .map_or_else(|| first_match.text(), |n| n.text());
+  let source = first_match.root().text();
   let display = first_match.display_context(0);
 
   let mut merger = MatchMerger::new(&first_match);
   let mut ret = display.leading.to_string();
-  ret.push_str(&format!("{}", styles.matched.paint(&*display.matched)));
+  styles.push_matched_to_ret(&mut ret, &display.matched)?;
 
   for nm in matches {
     if merger.check_overlapping(&nm) {
       continue;
     }
     let display = nm.display_context(0);
     // merge adjacent matches
     if let Some(last_end_offset) = merger.merge_adjacent(&nm) {
       ret.push_str(&source[last_end_offset..nm.range().start]);
-      ret.push_str(&format!("{}", styles.matched.paint(&*display.matched)));
+      styles.push_matched_to_ret(&mut ret, &display.matched)?;
       continue;
     }
     ret.push_str(merger.last_trailing);
     let lines = ret.lines().count();
     let mut num = merger.last_start_line;
     let width = (lines + num).to_string().chars().count();
     write!(writer, "{num:>width$}│")?; // initial line num
-    print_highlight(ret.lines(), Style::new(), width, &mut num, writer)?;
+    print_highlight(ret.lines(), width, &mut num, writer)?;
     writeln!(writer)?; // end match new line
                        //
     merger.conclude_match(&nm);
     ret = display.leading.to_string();
-    ret.push_str(&format!("{}", styles.matched.paint(&*display.matched)));
+    styles.push_matched_to_ret(&mut ret, &display.matched)?;
   }
   ret.push_str(merger.last_trailing);
   let lines = ret.lines().count();
   let mut num = merger.last_start_line;
   let width = (lines + num).to_string().chars().count();
   write!(writer, "{num:>width$}│")?; // initial line num
-  print_highlight(ret.lines(), Style::new(), width, &mut num, writer)?;
+  print_highlight(ret.lines(), width, &mut num, writer)?;
   writeln!(writer)?; // end match new line
+  writeln!(writer)?; // end
   Ok(())
 }
 
 fn print_matches_with_prefix<'a, W: WriteColor>(
   mut matches: Matches!('a),
   path: &Path,
   styles: &PrintStyles,
   writer: &mut W,
 ) -> Result<()> {
   let path = path.display();
   let Some(first_match) = matches.next() else {
     return Ok(())
   };
-  let source = first_match
-    .ancestors()
-    .last()
-    .map_or_else(|| first_match.text(), |n| n.text());
+  let source = first_match.root().text();
   let display = first_match.display_context(0);
 
   let mut merger = MatchMerger::new(&first_match);
   let mut ret = display.leading.to_string();
-  ret.push_str(&format!("{}", styles.matched.paint(&*display.matched)));
+  styles.push_matched_to_ret(&mut ret, &display.matched)?;
   for nm in matches {
     if merger.check_overlapping(&nm) {
       continue;
     }
     // merge adjacent matches
     if let Some(last_end_offset) = merger.merge_adjacent(&nm) {
       ret.push_str(&source[last_end_offset..nm.range().start]);
-      ret.push_str(&format!("{}", styles.matched.paint(nm.text())));
+      styles.push_matched_to_ret(&mut ret, &display.matched)?;
       continue;
     }
     ret.push_str(merger.last_trailing);
     for (n, line) in ret.lines().enumerate() {
       let num = merger.last_start_line + n;
       writeln!(writer, "{path}:{num}:{line}")?;
     }
     merger.conclude_match(&nm);
     let display = nm.display_context(0);
     ret = display.leading.to_string();
-    ret.push_str(&format!("{}", styles.matched.paint(&*display.matched)));
+    styles.push_matched_to_ret(&mut ret, &display.matched)?;
   }
   ret.push_str(merger.last_trailing);
   for (n, line) in ret.lines().enumerate() {
     let num = merger.last_start_line + n;
     writeln!(writer, "{path}:{num}:{line}")?;
   }
   Ok(())
@@ -378,15 +373,15 @@
   writer: &mut W,
 ) -> Result<()> {
   print_prelude(path, styles, writer)?;
   let Some(first_diff) = diffs.next() else {
     return Ok(());
   };
   let range = first_diff.node_match.range();
-  let source = first_diff.node_match.ancestors().last().unwrap().text();
+  let source = first_diff.node_match.root().text();
   let mut start = range.end;
   let mut new_str = format!("{}{}", &source[..range.start], first_diff.replacement);
   for diff in diffs {
     let range = diff.node_match.range();
     // skip overlapping diff
     if range.start < start {
       continue;
@@ -398,27 +393,24 @@
   new_str.push_str(&source[start..]);
   print_diff(&source, &new_str, styles, writer)?;
   Ok(())
 }
 
 fn print_highlight<'a, W: Write>(
   mut lines: impl Iterator<Item = &'a str>,
-  style: Style,
   width: usize,
   num: &mut usize,
   writer: &mut W,
 ) -> Result<()> {
   if let Some(line) = lines.next() {
-    let line = style.paint(line);
     write!(writer, "{line}")?;
   }
   for line in lines {
     writeln!(writer)?;
     *num += 1;
-    let line = style.paint(line);
     write!(writer, "{num:>width$}│{line}")?;
   }
   Ok(())
 }
 
 fn index_display(index: Option<usize>, style: Style, width: usize) -> impl Display {
   let index_str = match index {
@@ -534,14 +526,30 @@
         message: Style::new().bold(),
       },
     }
   }
   fn no_color() -> Self {
     Self::default()
   }
+
+  fn push_matched_to_ret(&self, ret: &mut String, matched: &str) -> Result<()> {
+    use std::fmt::Write;
+    // TODO: use intersperse
+    let mut lines = matched.lines();
+    if let Some(line) = lines.next() {
+      write!(ret, "{}", self.matched.paint(line))?;
+    } else {
+      return Ok(());
+    }
+    for line in lines {
+      ret.push('\n');
+      write!(ret, "{}", self.matched.paint(line))?;
+    }
+    Ok(())
+  }
 }
 impl From<ColorChoice> for PrintStyles {
   fn from(color: ColorChoice) -> Self {
     if choose_color::should_use_color(&color) {
       Self::colored()
     } else {
       Self::no_color()
@@ -682,15 +690,15 @@
       printer.print_matches(matches, "test.tsx".as_ref()).unwrap();
       let expected: String = source
         .lines()
         .enumerate()
         .map(|(i, l)| format!("{}│{l}\n", i + 1))
         .collect();
       // append heading to expected
-      let output = format!("test.tsx\n{expected}");
+      let output = format!("test.tsx\n{expected}\n");
       assert_eq!(get_text(&printer), output, "{note}");
     }
   }
 
   #[test]
   fn test_print_matches_without_heading() {
     for &(source, pattern, note) in MATCHES_CASES {
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.7.0/crates/cli/src/print/interactive_print.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-use std::sync::atomic::{AtomicBool, Ordering};
-
-use anyhow::{Context, Result};
-use ast_grep_config::RuleConfig;
-
 use super::{Diff, Printer};
 use crate::error::ErrorContext as EC;
 use crate::lang::SgLang;
 use crate::utils;
 
+use anyhow::{Context, Result};
+use ast_grep_config::RuleConfig;
+use ast_grep_core::{NodeMatch as SgNodeMatch, StrDoc};
 pub use codespan_reporting::{files::SimpleFile, term::ColorArg};
 
-use ast_grep_core::{NodeMatch as SgNodeMatch, StrDoc};
+use std::sync::atomic::{AtomicBool, Ordering};
+
 type NodeMatch<'a, L> = SgNodeMatch<'a, StrDoc<L>>;
 
 use std::borrow::Cow;
 use std::path::{Path, PathBuf};
 
 // add this macro because neither trait_alias nor type_alias_impl is supported.
 macro_rules! Matches {
@@ -22,27 +21,50 @@
 }
 macro_rules! Diffs {
   ($lt: lifetime) => { impl Iterator<Item = Diff<$lt>> };
 }
 
 pub struct InteractivePrinter<P: Printer> {
   accept_all: AtomicBool,
+  from_stdin: bool,
   inner: P,
 }
+
 impl<P: Printer> InteractivePrinter<P> {
-  pub fn new(inner: P) -> Self {
-    Self {
-      accept_all: AtomicBool::new(false),
-      inner,
+  pub fn new(inner: P, accept_all: bool) -> Result<Self> {
+    let from_stdin = utils::is_from_stdin();
+    if from_stdin && !accept_all {
+      Err(anyhow::anyhow!(EC::StdInIsNotInteractive))
+    } else {
+      Ok(Self {
+        accept_all: AtomicBool::new(accept_all),
+        from_stdin,
+        inner,
+      })
     }
   }
 
-  pub fn accept_all(self, accept_all: bool) -> Self {
-    self.accept_all.store(accept_all, Ordering::SeqCst);
-    self
+  fn prompt_edit(&self) -> char {
+    const EDIT_PROMPT: &str = "Accept change? (Yes[y], No[n], Accept All[a], Quit[q], Edit[e])";
+    utils::prompt(EDIT_PROMPT, "ynaqe", Some('n')).expect("Error happened during prompt")
+  }
+
+  fn prompt_view(&self) -> char {
+    const VIEW_PROMPT: &str = "Next[enter], Quit[q], Edit[e]";
+    utils::prompt(VIEW_PROMPT, "qe", Some('\n')).expect("cannot fail")
+  }
+
+  fn rewrite_action(&self, diffs: Vec<Diff<'_>>, path: &PathBuf) -> Result<()> {
+    let new_content = apply_rewrite(diffs);
+    if self.from_stdin {
+      println!("{new_content}");
+      Ok(())
+    } else {
+      std::fs::write(path, new_content).with_context(|| EC::WriteFile(path.clone()))
+    }
   }
 }
 
 impl<P: Printer> Printer for InteractivePrinter<P> {
   fn print_rule<'a>(
     &self,
     matches: Matches!('a),
@@ -53,121 +75,113 @@
       let matches: Vec<_> = matches.collect();
       let first_match = match matches.first() {
         Some(n) => n.start_pos().0,
         None => return Ok(()),
       };
       let file_path = PathBuf::from(file.name().to_string());
       self.inner.print_rule(matches.into_iter(), file, rule)?;
-      let resp = utils::prompt(VIEW_PROMPT, "qe", Some('\n')).expect("cannot fail");
+      let resp = self.prompt_view();
       if resp == 'q' {
         Err(anyhow::anyhow!("Exit interactive editing"))
       } else if resp == 'e' {
         utils::open_in_editor(&file_path, first_match)?;
         Ok(())
       } else {
         Ok(())
       }
     })
   }
 
   fn print_matches<'a>(&self, matches: Matches!('a), path: &Path) -> Result<()> {
-    utils::run_in_alternate_screen(|| print_matches_and_confirm_next(&self.inner, matches, path))
+    utils::run_in_alternate_screen(|| print_matches_and_confirm_next(self, matches, path))
   }
 
   fn print_diffs<'a>(&self, diffs: Diffs!('a), path: &Path) -> Result<()> {
     let path = path.to_path_buf();
     if self.accept_all.load(Ordering::SeqCst) {
-      return rewrite_action(diffs.collect(), &path);
+      return self.rewrite_action(diffs.collect(), &path);
     }
     utils::run_in_alternate_screen(|| {
-      let all = print_diffs_and_prompt_action(&self.inner, &path, diffs, None)?;
+      let all = print_diffs_and_prompt_action(self, &path, diffs, None)?;
       if all {
         self.accept_all.store(true, Ordering::SeqCst);
       }
       Ok(())
     })
   }
   fn print_rule_diffs<'a>(
     &self,
     diffs: Diffs!('a),
     path: &Path,
     rule: &RuleConfig<SgLang>,
   ) -> Result<()> {
     let path = path.to_path_buf();
     if self.accept_all.load(Ordering::SeqCst) {
-      return rewrite_action(diffs.collect(), &path);
+      return self.rewrite_action(diffs.collect(), &path);
     }
     utils::run_in_alternate_screen(|| {
-      let all = print_diffs_and_prompt_action(&self.inner, &path, diffs, Some(rule))?;
+      let all = print_diffs_and_prompt_action(self, &path, diffs, Some(rule))?;
       if all {
         self.accept_all.store(true, Ordering::SeqCst);
       }
       Ok(())
     })
   }
 }
 
-const EDIT_PROMPT: &str = "Accept change? (Yes[y], No[n], Accept All[a], Quit[q], Edit[e])";
-const VIEW_PROMPT: &str = "Next[enter], Quit[q], Edit[e]";
-
-fn rewrite_action(diffs: Vec<Diff<'_>>, path: &PathBuf) -> Result<()> {
-  let new_content = apply_rewrite(diffs);
-  std::fs::write(path, new_content).with_context(|| EC::WriteFile(path.clone()))
-}
-
 /// returns if accept_all is chosen
 fn print_diffs_and_prompt_action<'a>(
-  printer: &impl Printer,
+  interactive: &InteractivePrinter<impl Printer>,
   path: &PathBuf,
   diffs: Diffs!('a),
   rule: Option<&RuleConfig<SgLang>>,
 ) -> Result<bool> {
+  let printer = &interactive.inner;
   let diffs: Vec<_> = diffs.collect();
   let first_match = match diffs.first() {
     Some(n) => n.node_match.start_pos().0,
     None => return Ok(false),
   };
   if let Some(rule) = rule {
     printer.print_rule_diffs(diffs.clone().into_iter(), path, rule)?;
   } else {
     printer.print_diffs(diffs.clone().into_iter(), path)?;
   }
-  let response =
-    utils::prompt(EDIT_PROMPT, "ynaqe", Some('n')).expect("Error happened during prompt");
-  match response {
+  match interactive.prompt_edit() {
     'y' => {
-      rewrite_action(diffs, path)?;
+      interactive.rewrite_action(diffs, path)?;
       Ok(false)
     }
     'a' => {
-      rewrite_action(diffs, path)?;
+      interactive.rewrite_action(diffs, path)?;
       Ok(true)
     }
     'n' => Ok(false),
     'e' => {
       utils::open_in_editor(path, first_match)?;
       Ok(false)
     }
     'q' => Err(anyhow::anyhow!("Exit interactive editing")),
     _ => Ok(false),
   }
 }
 
 fn print_matches_and_confirm_next<'a>(
-  printer: &impl Printer,
+  interactive: &InteractivePrinter<impl Printer>,
   matches: Matches!('a),
   path: &Path,
 ) -> Result<()> {
+  let printer = &interactive.inner;
   let matches: Vec<_> = matches.collect();
   let first_match = match matches.first() {
     Some(n) => n.start_pos().0,
     None => return Ok(()),
   };
   printer.print_matches(matches.into_iter(), path)?;
-  let resp = utils::prompt(VIEW_PROMPT, "qe", Some('\n')).expect("cannot fail");
+  let resp = interactive.prompt_view();
   if resp == 'q' {
     Err(anyhow::anyhow!("Exit interactive editing"))
   } else if resp == 'e' {
     utils::open_in_editor(&path.to_path_buf(), first_match)?;
     Ok(())
   } else {
     Ok(())
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.7.0/crates/cli/src/print/json_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.7.0/crates/cli/src/print/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -40,18 +40,20 @@
   fn print_diffs<'a>(&self, diffs: Diffs!('a), path: &Path) -> Result<()>;
   fn print_rule_diffs<'a>(
     &self,
     diffs: Diffs!('a),
     path: &Path,
     rule: &RuleConfig<SgLang>,
   ) -> Result<()>;
+  /// Run before all printing. One CLI will run this exactly once.
   #[inline]
   fn before_print(&self) -> Result<()> {
     Ok(())
   }
+  /// Run after all printing. One CLI will run this exactly once.
   #[inline]
   fn after_print(&self) -> Result<()> {
     Ok(())
   }
 }
 
 #[derive(Clone)]
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/run.rs` & `ast_grep_cli-0.7.0/crates/cli/src/run.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 use crate::config::{register_custom_language, IgnoreFile, NoIgnore};
 use crate::error::ErrorContext as EC;
 use crate::lang::SgLang;
 use crate::print::{
   ColorArg, ColoredPrinter, Diff, Heading, InteractivePrinter, JSONPrinter, Printer,
 };
-use crate::utils::{filter_file_interactive, MatchUnit};
+use crate::utils::{filter_file_interactive, is_from_stdin, MatchUnit};
+use crate::utils::{run_std_in, StdInWorker};
 use crate::utils::{run_worker, Items, Worker};
 
 type Pattern<L> = SgPattern<StrDoc<L>>;
 
 // NOTE: have to register custom lang before clap read arg
 // RunArg has a field of SgLang
 pub fn register_custom_language_if_is_run(args: &[String]) {
@@ -83,23 +84,25 @@
 pub fn run_with_pattern(arg: RunArg) -> Result<()> {
   if arg.json {
     return run_pattern_with_printer(arg, JSONPrinter::stdout());
   }
   let printer = ColoredPrinter::stdout(arg.color).heading(arg.heading);
   let interactive = arg.interactive || arg.accept_all;
   if interactive {
-    let printer = InteractivePrinter::new(printer).accept_all(arg.accept_all);
+    let printer = InteractivePrinter::new(printer, arg.accept_all)?;
     run_pattern_with_printer(arg, printer)
   } else {
     run_pattern_with_printer(arg, printer)
   }
 }
 
 fn run_pattern_with_printer(arg: RunArg, printer: impl Printer + Sync) -> Result<()> {
-  if arg.lang.is_some() {
+  if is_from_stdin() {
+    run_std_in(RunWithSpecificLang::new(arg, printer)?)
+  } else if arg.lang.is_some() {
     run_worker(RunWithSpecificLang::new(arg, printer)?)
   } else {
     run_worker(RunWithInferredLang { arg, printer })
   }
 }
 
 struct RunWithInferredLang<Printer> {
@@ -153,15 +156,15 @@
   printer: Printer,
   pattern: Pattern<SgLang>,
 }
 
 impl<Printer> RunWithSpecificLang<Printer> {
   fn new(arg: RunArg, printer: Printer) -> Result<Self> {
     let pattern = &arg.pattern;
-    let lang = arg.lang.expect("must present");
+    let lang = arg.lang.ok_or(anyhow::anyhow!(EC::LanguageNotSpecified))?;
     let pattern = Pattern::try_new(pattern, lang).context(EC::ParsePattern)?;
     Ok(Self {
       arg,
       printer,
       pattern,
     })
   }
@@ -202,14 +205,27 @@
       match_one_file(printer, &match_unit, &rewrite)?;
     }
     printer.after_print()?;
     Ok(())
   }
 }
 
+impl<P: Printer + Sync> StdInWorker for RunWithSpecificLang<P> {
+  fn parse_stdin(&self, src: String) -> Option<Self::Item> {
+    let lang = self.arg.lang.expect("must present");
+    let grep = lang.ast_grep(src);
+    let has_match = grep.root().find(&self.pattern).is_some();
+    has_match.then(|| MatchUnit {
+      path: PathBuf::from("STDIN"),
+      matcher: self.pattern.clone(),
+      grep,
+    })
+  }
+}
+
 fn match_one_file(
   printer: &impl Printer,
   match_unit: &MatchUnit<impl Matcher<SgLang>>,
   rewrite: &Option<Fixer<String>>,
 ) -> Result<()> {
   let MatchUnit {
     path,
@@ -228,14 +244,15 @@
 
 #[cfg(test)]
 mod test {
   use super::*;
   use ast_grep_language::SupportLang;
   #[test]
   fn test_run_with_pattern() {
+    std::env::set_var("AST_GREP_ALWAYS_TTY", "1");
     let arg = RunArg {
       pattern: "console.log".to_string(),
       rewrite: None,
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
       lang: None,
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/scan.rs` & `ast_grep_cli-0.7.0/crates/cli/src/scan.rs`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 use crate::config::{find_rules, read_rule_file, register_custom_language, IgnoreFile, NoIgnore};
 use crate::error::ErrorContext as EC;
 use crate::lang::SgLang;
 use crate::print::{
   ColorArg, ColoredPrinter, Diff, InteractivePrinter, JSONPrinter, Printer, ReportStyle, SimpleFile,
 };
 use crate::utils::filter_file_interactive;
+use crate::utils::{is_from_stdin, run_std_in, StdInWorker};
 use crate::utils::{run_worker, Items, Worker};
 
 type AstGrep = ast_grep_core::AstGrep<StrDoc<SgLang>>;
 
 #[derive(Args)]
 pub struct ScanArg {
   /// Path to ast-grep root config, default is sgconfig.yml.
@@ -41,38 +42,46 @@
 
   /// Output matches in structured JSON text. This is useful for tools like jq.
   /// Conflicts with color and report-style.
   #[clap(long, conflicts_with = "color", conflicts_with = "report_style")]
   json: bool,
 
   /// Apply all rewrite without confirmation if true.
-  #[clap(long)]
+  #[clap(short = 'A', long)]
   accept_all: bool,
 
   /// The paths to search. You can provide multiple paths separated by spaces.
   #[clap(value_parser, default_value = ".")]
   paths: Vec<PathBuf>,
 
   /// Do not respect ignore files. You can suppress multiple ignore files by passing `no-ignore` multiple times.
   #[clap(long, action = clap::ArgAction::Append)]
   no_ignore: Vec<IgnoreFile>,
 }
 
 pub fn run_with_config(arg: ScanArg) -> Result<()> {
   register_custom_language(arg.config.clone());
   if arg.json {
-    let worker = ScanWithConfig::try_new(arg, JSONPrinter::stdout())?;
-    return run_worker(worker);
+    let printer = JSONPrinter::stdout();
+    return run_scan(arg, printer);
   }
   let printer = ColoredPrinter::stdout(arg.color).style(arg.report_style);
   let interactive = arg.interactive || arg.accept_all;
   if interactive {
-    let printer = InteractivePrinter::new(printer).accept_all(arg.accept_all);
-    let worker = ScanWithConfig::try_new(arg, printer)?;
-    run_worker(worker)
+    let printer = InteractivePrinter::new(printer, arg.accept_all)?;
+    run_scan(arg, printer)
+  } else {
+    run_scan(arg, printer)
+  }
+}
+
+fn run_scan<P: Printer + Sync>(arg: ScanArg, printer: P) -> Result<()> {
+  if is_from_stdin() {
+    let worker = ScanWithRule::try_new(arg, printer)?;
+    run_std_in(worker)
   } else {
     let worker = ScanWithConfig::try_new(arg, printer)?;
     run_worker(worker)
   }
 }
 
 struct ScanWithConfig<Printer> {
@@ -141,14 +150,68 @@
       Err(anyhow::anyhow!(EC::DiagnosticError(has_error)))
     } else {
       Ok(())
     }
   }
 }
 
+struct ScanWithRule<Printer> {
+  printer: Printer,
+  rule: RuleConfig<SgLang>,
+}
+impl<P: Printer> ScanWithRule<P> {
+  fn try_new(arg: ScanArg, printer: P) -> Result<Self> {
+    let rule = if let Some(path) = &arg.rule {
+      read_rule_file(path, None)?.pop().unwrap()
+    } else {
+      return Err(anyhow::anyhow!(EC::RuleNotSpecified));
+    };
+    Ok(Self { printer, rule })
+  }
+}
+
+impl<P: Printer + Sync> Worker for ScanWithRule<P> {
+  type Item = (PathBuf, AstGrep);
+  fn build_walk(&self) -> WalkParallel {
+    unreachable!()
+  }
+  fn produce_item(&self, _p: &Path) -> Option<Self::Item> {
+    unreachable!()
+  }
+  fn consume_items(&self, items: Items<Self::Item>) -> Result<()> {
+    self.printer.before_print()?;
+    let mut has_error = 0;
+    for (path, grep) in items {
+      let file_content = grep.root().text().to_string();
+      let rule = &self.rule;
+      let matches = grep.root().find_all(&rule.matcher).collect();
+      if matches!(rule.severity, Severity::Error) {
+        has_error += 1;
+      }
+      match_rule_on_file(&path, matches, rule, &file_content, &self.printer)?;
+    }
+    self.printer.after_print()?;
+    if has_error > 0 {
+      Err(anyhow::anyhow!(EC::DiagnosticError(has_error)))
+    } else {
+      Ok(())
+    }
+  }
+}
+
+impl<P: Printer + Sync> StdInWorker for ScanWithRule<P> {
+  fn parse_stdin(&self, src: String) -> Option<Self::Item> {
+    use ast_grep_core::Language;
+    let lang = self.rule.language;
+    let grep = lang.ast_grep(src);
+    let has_match = grep.root().find(&self.rule.matcher).is_some();
+    has_match.then(|| (PathBuf::from("STDIN"), grep))
+  }
+}
+
 fn match_rule_on_file(
   path: &Path,
   matches: Vec<NodeMatch<StrDoc<SgLang>>>,
   rule: &RuleConfig<SgLang>,
   file_content: &String,
   reporter: &impl Printer,
 ) -> Result<()> {
@@ -263,14 +326,15 @@
     let mut file = File::create(dir.path().join("rules/test.yml")).unwrap();
     file.write_all(RULE.as_bytes()).unwrap();
     let mut file = File::create(dir.path().join("test.rs")).unwrap();
     file
       .write_all("fn test() { Some(123) }".as_bytes())
       .unwrap();
     file.sync_all().unwrap();
+    std::env::set_var("AST_GREP_ALWAYS_TTY", "1");
     let arg = ScanArg {
       config: Some(dir.path().join("sgconfig.yml")),
       rule: None,
       report_style: ReportStyle::Rich,
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/utils.rs` & `ast_grep_cli-0.7.0/crates/cli/src/utils.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   terminal::{self, EnterAlternateScreen, LeaveAlternateScreen},
 };
 use ignore::{DirEntry, WalkParallel, WalkState};
 
 use ast_grep_core::{AstGrep, Matcher, StrDoc};
 use ast_grep_language::Language;
 
+use std::env;
 use std::fs::read_to_string;
 use std::io::stdout;
 use std::io::Write;
 use std::path::{Path, PathBuf};
 use std::sync::mpsc;
 
 fn read_char() -> Result<char> {
@@ -73,37 +74,61 @@
 pub trait Worker: Sync {
   type Item: Send;
   fn build_walk(&self) -> WalkParallel;
   fn produce_item(&self, path: &Path) -> Option<Self::Item>;
   fn consume_items(&self, items: Items<Self::Item>) -> Result<()>;
 }
 
+pub trait StdInWorker: Worker {
+  fn parse_stdin(&self, src: String) -> Option<Self::Item>;
+}
+
 pub struct Items<T>(mpsc::Receiver<T>);
 impl<T> Iterator for Items<T> {
   type Item = T;
   fn next(&mut self) -> Option<Self::Item> {
     if let Ok(match_result) = self.0.recv() {
       Some(match_result)
     } else {
       None
     }
   }
 }
+impl<T> Items<T> {
+  pub fn once(t: T) -> Result<Self> {
+    let (tx, rx) = mpsc::channel();
+    // use write to avoid send/sync trait bound
+    match tx.send(t) {
+      Ok(_) => (),
+      Err(e) => return Err(anyhow!(e.to_string())),
+    };
+    Ok(Items(rx))
+  }
+}
 
 fn filter_result(result: Result<DirEntry, ignore::Error>) -> Option<PathBuf> {
   let entry = match result {
     Ok(entry) => entry,
     Err(err) => {
       eprintln!("ERROR: {}", err);
       return None;
     }
   };
   entry.file_type()?.is_file().then(|| entry.into_path())
 }
 
+pub fn run_std_in<MW: StdInWorker>(worker: MW) -> Result<()> {
+  let source = std::io::read_to_string(std::io::stdin())?;
+  if let Some(item) = worker.parse_stdin(source) {
+    worker.consume_items(Items::once(item)?)
+  } else {
+    Ok(())
+  }
+}
+
 pub fn run_worker<MW: Worker>(worker: MW) -> Result<()> {
   let producer = |path: PathBuf| worker.produce_item(&path);
   let (tx, rx) = mpsc::channel();
   let walker = worker.build_walk();
   walker.run(|| {
     let tx = tx.clone();
     Box::new(move |result| {
@@ -185,14 +210,25 @@
 /// An analogy to compilation unit in C programming language.
 pub struct MatchUnit<M: Matcher<SgLang>> {
   pub path: PathBuf,
   pub grep: AstGrep<StrDoc<SgLang>>,
   pub matcher: M,
 }
 
+#[inline]
+pub fn is_from_stdin() -> bool {
+  // disable stdin if tty env presents or is_atty == true
+  // env is used for testing purpose only
+  if cfg!(debug_assertions) {
+    env::var_os("AST_GREP_ALWAYS_TTY").is_none() && !atty::is(atty::Stream::Stdin)
+  } else {
+    !atty::is(atty::Stream::Stdin)
+  }
+}
+
 #[cfg(test)]
 mod test {
   use super::*;
 
   #[test]
   fn test_open_editor() {
     // these two tests must run in sequence
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/src/verify.rs` & `ast_grep_cli-0.7.0/crates/cli/src/verify.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.7.0/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.7.0/crates/cli/tests/run_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 use predicates::prelude::*;
 use predicates::str::contains;
 
 #[test]
 fn test_simple_infer_lang() -> Result<()> {
   let dir = create_test_files([("a.ts", "console.log(123)"), ("b.rs", "console.log(456)")])?;
   Command::cargo_bin("sg")?
+    .env("AST_GREP_ALWAYS_TTY", "1")
     .current_dir(dir.path())
     .args(["-p", "console.log($A)"])
     .assert()
     .success()
     .stdout(contains("console.log(123)"))
     .stdout(contains("console.log(456)"));
   Ok(())
 }
 
 #[test]
 fn test_simple_specific_lang() -> Result<()> {
   let dir = create_test_files([("a.ts", "console.log(123)"), ("b.rs", "console.log(456)")])?;
   Command::cargo_bin("sg")?
+    .env("AST_GREP_ALWAYS_TTY", "1")
     .current_dir(dir.path())
     .args(["-p", "console.log($A)", "-l", "rs"])
     .assert()
     .success()
     .stdout(contains("console.log(123)").not())
     .stdout(contains("console.log(456)"));
   Ok(())
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.7.0/crates/cli/tests/verify_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/pyproject.toml` & `ast_grep_cli-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.6.7"
+version = "0.7.0"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.6.7/crates/cli/Cargo.lock` & `ast_grep_cli-0.7.0/crates/cli/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -131,15 +131,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -147,38 +147,38 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading 0.8.0",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
@@ -195,27 +195,27 @@
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "dashmap",
  "serde",
  "serde_json",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -276,15 +276,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -382,28 +382,28 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.4"
+version = "4.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80672091db20273a15cf9fdd4e47ed43b5091ec9841bf4c6145c9dfbbcae09ed"
+checksum = "d9394150f5b4273a1763355bd1c2ec54cc5a2593f790587bcd6b2c947cfa9211"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.4"
+version = "4.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1458a1df40e1e2afebb7ab60ce55c1fa8f431146205aa5f4887e0b111c27636"
+checksum = "9a78fbdd3cc2914ddf37ba444114bc7765bbdcb55ec9cbe6fa054f0137400717"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags 1.3.2",
  "clap_lex",
  "strsim",
 ]
@@ -584,15 +584,15 @@
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
- "hashbrown",
+ "hashbrown 0.12.3",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "difflib"
@@ -615,14 +615,20 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
+name = "equivalent"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88bffebc5d80432c9b140ee17875ff173a8ab62faad5b257da912bd2f6c1c0a1"
+
+[[package]]
 name = "errno"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
 dependencies = [
  "errno-dragonfly",
  "libc",
@@ -769,14 +775,20 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+
+[[package]]
 name = "heck"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2540771e65fc8cb83cd6e8a237f70c319bd5c29f78ed1084ba5d50eeac86f7f9"
 
 [[package]]
 name = "hermit-abi"
@@ -834,20 +846,20 @@
  "thread_local",
  "walkdir",
  "winapi-util",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.1"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10a35a97730320ffe8e2d410b5d3b69279b98d2c14bdb8b70ea89ecf7888d41e"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
 dependencies = [
- "autocfg",
- "hashbrown",
+ "equivalent",
+ "hashbrown 0.14.0",
 ]
 
 [[package]]
 name = "inquire"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c33e7c1ddeb15c9abcbfef6029d8e29f69b52b6d6c891031b88ed91b5065803b"
@@ -1438,17 +1450,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.98",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.97"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -1461,17 +1473,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.98",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.21"
+version = "0.9.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
+checksum = "452e67b9c20c37fa79df53201dc03839651086ed9bbe92b3ca585ca9fdaa7d85"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -1658,23 +1670,23 @@
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.2"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
+checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
 
 [[package]]
 name = "toml_edit"
-version = "0.19.10"
+version = "0.19.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
+checksum = "266f016b7f039eec8a1a80dfe6156b633d208b9fccca5e4db1d6775b0c4e34a7"
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
@@ -1880,17 +1892,17 @@
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-lua"
-version = "0.0.17"
+version = "0.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78370a81245067b381587508ceadde7a327aa9884a7c5ff8becaf437d6912f60"
+checksum = "81c1b8887a3a3d9bf10087f490d53563e665598c460c60fc7208869ec10f225a"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-python"
```

### Comparing `ast_grep_cli-0.6.7/README.md` & `ast_grep_cli-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,19 @@
 Try the [online playground](https://ast-grep.github.io/playground.html) for a taste!
 
 ## Demo
 
 ![output](https://user-images.githubusercontent.com/2883231/183275066-8d9c342f-46cb-4fa5-aa4e-b98aac011869.gif)
 
 ## Installation
-You can install it from [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
+You can install it from [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip](https://pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
 
 ```bash
-# install via npm
 npm install --global @ast-grep/cli
-
-# install via cargo
+pip install ast-grep-cli
 cargo install ast-grep
 
 # install via homebrew, thank @henryhchchc
 brew install ast-grep
 
 # install via scoop, thank @brian6932
 scoop install main/ast-grep
```

#### html2text {}

```diff
@@ -8,51 +8,51 @@
 writing ordinary code. It will match all code that has the same syntactical
 structure. You can use `$` sign + upper case letters as wildcard, e.g.
 `$MATCH`, to match any single AST node. Think it as REGEX dot `.`, except it is
 not textual. Try the [online playground](https://ast-grep.github.io/
 playground.html) for a taste! ## Demo ![output](https://user-
 images.githubusercontent.com/2883231/183275066-8d9c342f-46cb-4fa5-aa4e-
 b98aac011869.gif) ## Installation You can install it from [npm](https://
-docs.npmjs.com/downloading-and-installing-node-js-and-npm), [cargo](https://
-doc.rust-lang.org/cargo/getting-started/installation.html), [homebrew](https://
-brew.sh/) or [scoop](https://scoop.sh/)! ```bash # install via npm npm install
---global @ast-grep/cli # install via cargo cargo install ast-grep # install via
-homebrew, thank @henryhchchc brew install ast-grep # install via scoop, thank
-@brian6932 scoop install main/ast-grep ``` Or you can build ast-grep from
-source. You need install rustup, clone the repository and then ```bash cargo
-install --path ./crates/cli ``` [Packages](https://repology.org/project/ast-
-grep/versions) are available on other platforms too. ## Command line usage
-example ast-grep has following form. ``` sg --pattern 'var code = $PATTERN' --
-rewrite 'let code = new $PATTERN' --lang ts ``` ### Example * [Rewrite code in
-null coalescing operator](https://twitter.com/Hchan_mgn/status/
-1547061516993699841?s=20&t=ldDoj4U2nq-FRKQkU5GWXA) ```bash sg -p '$A && $A()' -
-l ts -r '$A?.()' ``` * [Rewrite](https://twitter.com/Hchan_mgn/status/
-1561802312846278657) [Zodios](https://github.com/ecyrbe/zodios#migrate-to-v8)
-```bash sg -p 'new Zodios($URL, $CONF as const,)' -l ts -r 'new Zodios($URL,
-$CONF)' -i ``` * [Implement eslint rule using YAML.](https://twitter.com/
-Hchan_mgn/status/1560108625460355073) ## Sponsor ![Sponsors](https://
-raw.githubusercontent.com/HerringtonDarkholme/sponsors/main/sponsorkit/
-sponsors.svg) If you find ast-grep interesting and useful for your work, please
-[buy me a coffee](https://github.com/sponsors/HerringtonDarkholme) so I can
-spend more time on the project! ## Feature Highlight ast-grep's core is an
-algorithm to search and replace code based on abstract syntax tree produced by
-tree-sitter. It can help you to do lightweight static analysis and massive
-scale code manipulation in an intuitive way. Key highlights: * An intuitive
-pattern to find and replace AST. ast-grep's pattern looks like ordinary code
-you would write every day. (You can call the pattern is isomorphic to code). *
-jQuery like API for AST traversal and manipulation. * YAML configuration to
-write new linting rules or code modification. * Written in compiled language,
-with tree-sitter based parsing and utilizing multiple cores. * Beautiful
-command line interface :) ast-grep's vision is to democratize abstract syntax
-tree magic and to liberate one from cumbersome AST programming! * If you are an
-open source library author, ast-grep can help your library users adopt breaking
-changes more easily. * if you are a tech lead in your team, ast-grep can help
-you enforce code best practice tailored to your business need. * If you are a
-security researcher, ast-grep can help you write rules much faster. ## CLI
-Screenshot ### Search | Feature | Command | Screenshot | | ------- | ------- |
----------- | | Search | `sg -p 'Some($A)' -l rs` | ![image](https://github.com/
-ast-grep/ast-grep/assets/2883231/002db3a2-8a79-4838-ad5c-563634183c3f) | |
-Rewrite | `sg -p '$F && $F($$$ARGS)' -r '$F?.($$$ARGS)' -l ts` | ![image]
-(https://github.com/ast-grep/ast-grep/assets/2883231/ad9394d8-3aea-4b96-8d54-
-6e01f06174d2)| | Report | `sg scan` | ![image](https://user-
-images.githubusercontent.com/2883231/187094977-fd544d4b-64de-4bba-8bea-
-8c0de047b352.png) |
+docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip](https://
+pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/
+installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
+```bash npm install --global @ast-grep/cli pip install ast-grep-cli cargo
+install ast-grep # install via homebrew, thank @henryhchchc brew install ast-
+grep # install via scoop, thank @brian6932 scoop install main/ast-grep ``` Or
+you can build ast-grep from source. You need install rustup, clone the
+repository and then ```bash cargo install --path ./crates/cli ``` [Packages]
+(https://repology.org/project/ast-grep/versions) are available on other
+platforms too. ## Command line usage example ast-grep has following form. ```
+sg --pattern 'var code = $PATTERN' --rewrite 'let code = new $PATTERN' --lang
+ts ``` ### Example * [Rewrite code in null coalescing operator](https://
+twitter.com/Hchan_mgn/status/1547061516993699841?s=20&t=ldDoj4U2nq-FRKQkU5GWXA)
+```bash sg -p '$A && $A()' -l ts -r '$A?.()' ``` * [Rewrite](https://
+twitter.com/Hchan_mgn/status/1561802312846278657) [Zodios](https://github.com/
+ecyrbe/zodios#migrate-to-v8) ```bash sg -p 'new Zodios($URL, $CONF as const,)'
+-l ts -r 'new Zodios($URL, $CONF)' -i ``` * [Implement eslint rule using YAML.]
+(https://twitter.com/Hchan_mgn/status/1560108625460355073) ## Sponsor !
+[Sponsors](https://raw.githubusercontent.com/HerringtonDarkholme/sponsors/main/
+sponsorkit/sponsors.svg) If you find ast-grep interesting and useful for your
+work, please [buy me a coffee](https://github.com/sponsors/HerringtonDarkholme)
+so I can spend more time on the project! ## Feature Highlight ast-grep's core
+is an algorithm to search and replace code based on abstract syntax tree
+produced by tree-sitter. It can help you to do lightweight static analysis and
+massive scale code manipulation in an intuitive way. Key highlights: * An
+intuitive pattern to find and replace AST. ast-grep's pattern looks like
+ordinary code you would write every day. (You can call the pattern is
+isomorphic to code). * jQuery like API for AST traversal and manipulation. *
+YAML configuration to write new linting rules or code modification. * Written
+in compiled language, with tree-sitter based parsing and utilizing multiple
+cores. * Beautiful command line interface :) ast-grep's vision is to
+democratize abstract syntax tree magic and to liberate one from cumbersome AST
+programming! * If you are an open source library author, ast-grep can help your
+library users adopt breaking changes more easily. * if you are a tech lead in
+your team, ast-grep can help you enforce code best practice tailored to your
+business need. * If you are a security researcher, ast-grep can help you write
+rules much faster. ## CLI Screenshot ### Search | Feature | Command |
+Screenshot | | ------- | ------- | ---------- | | Search | `sg -p 'Some($A)' -
+l rs` | ![image](https://github.com/ast-grep/ast-grep/assets/2883231/002db3a2-
+8a79-4838-ad5c-563634183c3f) | | Rewrite | `sg -p '$F && $F($$$ARGS)' -r '$F?.
+($$$ARGS)' -l ts` | ![image](https://github.com/ast-grep/ast-grep/assets/
+2883231/ad9394d8-3aea-4b96-8d54-6e01f06174d2)| | Report | `sg scan` | ![image]
+(https://user-images.githubusercontent.com/2883231/187094977-fd544d4b-64de-
+4bba-8bea-8c0de047b352.png) |
```

### Comparing `ast_grep_cli-0.6.7/LICENSE` & `ast_grep_cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.6.7/PKG-INFO` & `ast_grep_cli-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.6.7
+Version: 0.7.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 License-File: LICENSE
+License-File: LICENSE
 Summary: Structural Search and Rewrite code at large scale using precise AST pattern.
 Keywords: ast,pattern,codemod,structural search,rewrite
 Home-Page: https://ast-grep.github.io/
 Author: Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>
 Author-email: Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>
 Maintainer-email: Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>
 License: MIT
@@ -50,21 +51,19 @@
 Try the [online playground](https://ast-grep.github.io/playground.html) for a taste!
 
 ## Demo
 
 ![output](https://user-images.githubusercontent.com/2883231/183275066-8d9c342f-46cb-4fa5-aa4e-b98aac011869.gif)
 
 ## Installation
-You can install it from [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
+You can install it from [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip](https://pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
 
 ```bash
-# install via npm
 npm install --global @ast-grep/cli
-
-# install via cargo
+pip install ast-grep-cli
 cargo install ast-grep
 
 # install via homebrew, thank @henryhchchc
 brew install ast-grep
 
 # install via scoop, thank @brian6932
 scoop install main/ast-grep
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.6.7 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.7.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
-Topic :: Text Processing License-File: LICENSE Summary: Structural Search and
-Rewrite code at large scale using precise AST pattern. Keywords:
-ast,pattern,codemod,structural search,rewrite Home-Page: https://ast-
+Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
+Structural Search and Rewrite code at large scale using precise AST pattern.
+Keywords: ast,pattern,codemod,structural search,rewrite Home-Page: https://ast-
 grep.github.io/ Author: Herrington Darkholme
 <2883231+HerringtonDarkholme@users.noreply.github.com> Author-email: Herrington
 Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com> Maintainer-
 email: Herrington Darkholme
 <2883231+HerringtonDarkholme@users.noreply.github.com> License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-
 URL: Repository, https://github.com/ast-grep/ast-grep Project-URL:
@@ -26,51 +26,51 @@
 writing ordinary code. It will match all code that has the same syntactical
 structure. You can use `$` sign + upper case letters as wildcard, e.g.
 `$MATCH`, to match any single AST node. Think it as REGEX dot `.`, except it is
 not textual. Try the [online playground](https://ast-grep.github.io/
 playground.html) for a taste! ## Demo ![output](https://user-
 images.githubusercontent.com/2883231/183275066-8d9c342f-46cb-4fa5-aa4e-
 b98aac011869.gif) ## Installation You can install it from [npm](https://
-docs.npmjs.com/downloading-and-installing-node-js-and-npm), [cargo](https://
-doc.rust-lang.org/cargo/getting-started/installation.html), [homebrew](https://
-brew.sh/) or [scoop](https://scoop.sh/)! ```bash # install via npm npm install
---global @ast-grep/cli # install via cargo cargo install ast-grep # install via
-homebrew, thank @henryhchchc brew install ast-grep # install via scoop, thank
-@brian6932 scoop install main/ast-grep ``` Or you can build ast-grep from
-source. You need install rustup, clone the repository and then ```bash cargo
-install --path ./crates/cli ``` [Packages](https://repology.org/project/ast-
-grep/versions) are available on other platforms too. ## Command line usage
-example ast-grep has following form. ``` sg --pattern 'var code = $PATTERN' --
-rewrite 'let code = new $PATTERN' --lang ts ``` ### Example * [Rewrite code in
-null coalescing operator](https://twitter.com/Hchan_mgn/status/
-1547061516993699841?s=20&t=ldDoj4U2nq-FRKQkU5GWXA) ```bash sg -p '$A && $A()' -
-l ts -r '$A?.()' ``` * [Rewrite](https://twitter.com/Hchan_mgn/status/
-1561802312846278657) [Zodios](https://github.com/ecyrbe/zodios#migrate-to-v8)
-```bash sg -p 'new Zodios($URL, $CONF as const,)' -l ts -r 'new Zodios($URL,
-$CONF)' -i ``` * [Implement eslint rule using YAML.](https://twitter.com/
-Hchan_mgn/status/1560108625460355073) ## Sponsor ![Sponsors](https://
-raw.githubusercontent.com/HerringtonDarkholme/sponsors/main/sponsorkit/
-sponsors.svg) If you find ast-grep interesting and useful for your work, please
-[buy me a coffee](https://github.com/sponsors/HerringtonDarkholme) so I can
-spend more time on the project! ## Feature Highlight ast-grep's core is an
-algorithm to search and replace code based on abstract syntax tree produced by
-tree-sitter. It can help you to do lightweight static analysis and massive
-scale code manipulation in an intuitive way. Key highlights: * An intuitive
-pattern to find and replace AST. ast-grep's pattern looks like ordinary code
-you would write every day. (You can call the pattern is isomorphic to code). *
-jQuery like API for AST traversal and manipulation. * YAML configuration to
-write new linting rules or code modification. * Written in compiled language,
-with tree-sitter based parsing and utilizing multiple cores. * Beautiful
-command line interface :) ast-grep's vision is to democratize abstract syntax
-tree magic and to liberate one from cumbersome AST programming! * If you are an
-open source library author, ast-grep can help your library users adopt breaking
-changes more easily. * if you are a tech lead in your team, ast-grep can help
-you enforce code best practice tailored to your business need. * If you are a
-security researcher, ast-grep can help you write rules much faster. ## CLI
-Screenshot ### Search | Feature | Command | Screenshot | | ------- | ------- |
----------- | | Search | `sg -p 'Some($A)' -l rs` | ![image](https://github.com/
-ast-grep/ast-grep/assets/2883231/002db3a2-8a79-4838-ad5c-563634183c3f) | |
-Rewrite | `sg -p '$F && $F($$$ARGS)' -r '$F?.($$$ARGS)' -l ts` | ![image]
-(https://github.com/ast-grep/ast-grep/assets/2883231/ad9394d8-3aea-4b96-8d54-
-6e01f06174d2)| | Report | `sg scan` | ![image](https://user-
-images.githubusercontent.com/2883231/187094977-fd544d4b-64de-4bba-8bea-
-8c0de047b352.png) |
+docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip](https://
+pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/
+installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
+```bash npm install --global @ast-grep/cli pip install ast-grep-cli cargo
+install ast-grep # install via homebrew, thank @henryhchchc brew install ast-
+grep # install via scoop, thank @brian6932 scoop install main/ast-grep ``` Or
+you can build ast-grep from source. You need install rustup, clone the
+repository and then ```bash cargo install --path ./crates/cli ``` [Packages]
+(https://repology.org/project/ast-grep/versions) are available on other
+platforms too. ## Command line usage example ast-grep has following form. ```
+sg --pattern 'var code = $PATTERN' --rewrite 'let code = new $PATTERN' --lang
+ts ``` ### Example * [Rewrite code in null coalescing operator](https://
+twitter.com/Hchan_mgn/status/1547061516993699841?s=20&t=ldDoj4U2nq-FRKQkU5GWXA)
+```bash sg -p '$A && $A()' -l ts -r '$A?.()' ``` * [Rewrite](https://
+twitter.com/Hchan_mgn/status/1561802312846278657) [Zodios](https://github.com/
+ecyrbe/zodios#migrate-to-v8) ```bash sg -p 'new Zodios($URL, $CONF as const,)'
+-l ts -r 'new Zodios($URL, $CONF)' -i ``` * [Implement eslint rule using YAML.]
+(https://twitter.com/Hchan_mgn/status/1560108625460355073) ## Sponsor !
+[Sponsors](https://raw.githubusercontent.com/HerringtonDarkholme/sponsors/main/
+sponsorkit/sponsors.svg) If you find ast-grep interesting and useful for your
+work, please [buy me a coffee](https://github.com/sponsors/HerringtonDarkholme)
+so I can spend more time on the project! ## Feature Highlight ast-grep's core
+is an algorithm to search and replace code based on abstract syntax tree
+produced by tree-sitter. It can help you to do lightweight static analysis and
+massive scale code manipulation in an intuitive way. Key highlights: * An
+intuitive pattern to find and replace AST. ast-grep's pattern looks like
+ordinary code you would write every day. (You can call the pattern is
+isomorphic to code). * jQuery like API for AST traversal and manipulation. *
+YAML configuration to write new linting rules or code modification. * Written
+in compiled language, with tree-sitter based parsing and utilizing multiple
+cores. * Beautiful command line interface :) ast-grep's vision is to
+democratize abstract syntax tree magic and to liberate one from cumbersome AST
+programming! * If you are an open source library author, ast-grep can help your
+library users adopt breaking changes more easily. * if you are a tech lead in
+your team, ast-grep can help you enforce code best practice tailored to your
+business need. * If you are a security researcher, ast-grep can help you write
+rules much faster. ## CLI Screenshot ### Search | Feature | Command |
+Screenshot | | ------- | ------- | ---------- | | Search | `sg -p 'Some($A)' -
+l rs` | ![image](https://github.com/ast-grep/ast-grep/assets/2883231/002db3a2-
+8a79-4838-ad5c-563634183c3f) | | Rewrite | `sg -p '$F && $F($$$ARGS)' -r '$F?.
+($$$ARGS)' -l ts` | ![image](https://github.com/ast-grep/ast-grep/assets/
+2883231/ad9394d8-3aea-4b96-8d54-6e01f06174d2)| | Report | `sg scan` | ![image]
+(https://user-images.githubusercontent.com/2883231/187094977-fd544d4b-64de-
+4bba-8bea-8c0de047b352.png) |
```

