# Comparing `tmp/vit-2.3.0.tar.gz` & `tmp/vit-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-2.3.0.tar", last modified: Fri Apr 14 04:27:09 2023, max compression
+gzip compressed data, was "vit-2.3.1.tar", last modified: Sun Jun 25 00:59:42 2023, max compression
```

## Comparing `vit-2.3.0.tar` & `vit-2.3.1.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.157355 vit-2.3.0/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      856 2020-12-24 03:52:45.000000 vit-2.3.0/AUTHORS.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2034 2020-12-24 03:52:45.000000 vit-2.3.0/COLOR.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     9309 2023-04-14 04:10:49.000000 vit-2.3.0/CUSTOMIZE.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3048 2022-04-28 02:43:50.000000 vit-2.3.0/DEVELOPMENT.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1763 2020-12-24 03:52:45.000000 vit-2.3.0/INSTALL.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1070 2020-12-24 03:52:45.000000 vit-2.3.0/LICENSE
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      299 2020-12-24 03:52:45.000000 vit-2.3.0/MANIFEST.in
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2911 2023-04-14 04:27:09.153355 vit-2.3.0/PKG-INFO
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1985 2022-05-09 14:29:06.000000 vit-2.3.0/README.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      104 2021-02-28 21:10:00.000000 vit-2.3.0/pyproject.toml
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2022-04-17 22:57:32.000000 vit-2.3.0/requirements.txt
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.101356 vit-2.3.0/scripts/
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.109356 vit-2.3.0/scripts/bash/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      153 2020-12-24 03:52:45.000000 vit-2.3.0/scripts/bash/vit.bash_completion
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       38 2023-04-14 04:27:09.157355 vit-2.3.0/setup.cfg
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1823 2023-04-14 04:10:49.000000 vit-2.3.0/setup.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.109356 vit-2.3.0/test/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.3.0/test/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2934 2021-11-04 13:51:45.000000 vit-2.3.0/test/test_list_batcher.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.117355 vit-2.3.0/vit/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      194 2020-12-24 03:52:45.000000 vit-2.3.0/vit/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2491 2023-04-14 04:10:49.000000 vit-2.3.0/vit/action_manager.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3834 2023-04-14 04:10:49.000000 vit-2.3.0/vit/actions.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    45170 2023-04-14 04:10:49.000000 vit-2.3.0/vit/application.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    11394 2023-04-14 04:10:49.000000 vit-2.3.0/vit/autocomplete.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5154 2022-10-26 13:33:43.000000 vit-2.3.0/vit/base_list_box.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    12121 2023-04-14 04:10:49.000000 vit-2.3.0/vit/color.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2491 2020-12-24 03:52:45.000000 vit-2.3.0/vit/color_mappings.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5466 2023-04-14 04:10:49.000000 vit-2.3.0/vit/command_bar.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      168 2022-04-28 01:54:06.000000 vit-2.3.0/vit/command_line.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.121355 vit-2.3.0/vit/config/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     9749 2022-10-21 16:59:04.000000 vit-2.3.0/vit/config/config.sample.ini
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    16940 2023-04-14 04:10:49.000000 vit-2.3.0/vit/config_parser.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      296 2020-12-24 03:52:45.000000 vit-2.3.0/vit/debug.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6442 2020-12-24 03:52:45.000000 vit-2.3.0/vit/denotation.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       73 2022-04-28 19:54:53.000000 vit-2.3.0/vit/env.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      495 2023-04-14 04:10:49.000000 vit-2.3.0/vit/event.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       92 2020-12-24 03:52:45.000000 vit-2.3.0/vit/exception.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.153355 vit-2.3.0/vit/formatter/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6781 2023-04-14 04:10:49.000000 vit-2.3.0/vit/formatter/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      342 2021-02-02 03:24:52.000000 vit-2.3.0/vit/formatter/depends.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      206 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/depends_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      224 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/depends_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/depends_list.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2493 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      100 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/description_combined.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      895 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      357 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_desc.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      637 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/description_oneline.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      483 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_truncated.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      718 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_truncated_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      253 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      129 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       69 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      131 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       66 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      120 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      138 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       61 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/id.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       62 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/id_number.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6424 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/markers.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       71 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      150 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      156 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/parent.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/parent_long.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      190 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/parent_short.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1143 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/project.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/project_full.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      162 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/project_indented.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      342 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/project_parent.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/recur.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/recur_duration.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      178 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/recur_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      307 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      165 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       93 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      167 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      171 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      202 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_active.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      312 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/status.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/status_long.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      139 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/status_short.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      785 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/tags.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      440 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/tags_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/tags_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/tags_list.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      812 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_date.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      385 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_duration.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      471 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      404 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_numeric.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      369 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_string.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      271 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/urgency.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/urgency_integer.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/urgency_real.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       63 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/uuid.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/uuid_long.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/uuid_short.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       67 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5402 2023-04-14 04:10:49.000000 vit-2.3.0/vit/formatter_base.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     7345 2023-04-14 04:10:49.000000 vit-2.3.0/vit/help.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2300 2023-04-14 04:10:49.000000 vit-2.3.0/vit/key_cache.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.153355 vit-2.3.0/vit/keybinding/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1573 2020-12-30 18:53:00.000000 vit-2.3.0/vit/keybinding/vi.ini
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6801 2023-04-14 04:10:49.000000 vit-2.3.0/vit/keybinding_parser.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1662 2023-04-14 04:10:49.000000 vit-2.3.0/vit/list_batcher.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1182 2023-04-14 04:10:49.000000 vit-2.3.0/vit/loader.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3187 2023-04-14 04:10:49.000000 vit-2.3.0/vit/markers.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2050 2020-12-24 03:52:45.000000 vit-2.3.0/vit/multi_widget.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2692 2023-01-06 12:19:59.000000 vit-2.3.0/vit/option_parser.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1491 2023-04-14 04:10:49.000000 vit-2.3.0/vit/pid_manager.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2087 2023-04-14 04:10:49.000000 vit-2.3.0/vit/process.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5606 2023-04-14 04:10:49.000000 vit-2.3.0/vit/readline.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1978 2023-04-14 04:10:49.000000 vit-2.3.0/vit/registry.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5214 2023-04-14 04:10:49.000000 vit-2.3.0/vit/task.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    23608 2023-04-14 04:10:49.000000 vit-2.3.0/vit/task_list.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.153355 vit-2.3.0/vit/theme/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.3.0/vit/theme/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      842 2020-12-24 03:52:45.000000 vit-2.3.0/vit/theme/classic.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      926 2020-12-24 03:52:45.000000 vit-2.3.0/vit/theme/default.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      410 2020-12-24 03:52:45.000000 vit-2.3.0/vit/uda.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1529 2022-12-25 20:06:26.000000 vit-2.3.0/vit/util.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       14 2023-04-14 04:10:49.000000 vit-2.3.0/vit/version.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      483 2021-11-04 13:51:45.000000 vit-2.3.0/vit/xdg.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.117355 vit-2.3.0/vit.egg-info/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2911 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/PKG-INFO
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     4454 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/SOURCES.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/dependency_links.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       46 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/entry_points.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2019-09-28 15:34:44.000000 vit-2.3.0/vit.egg-info/not-zip-safe
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       74 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/requires.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        4 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/top_level.txt
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.065125 vit-2.3.1/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      856 2020-12-24 03:52:45.000000 vit-2.3.1/AUTHORS.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2034 2020-12-24 03:52:45.000000 vit-2.3.1/COLOR.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     9309 2023-04-14 04:10:49.000000 vit-2.3.1/CUSTOMIZE.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3048 2022-04-28 02:43:50.000000 vit-2.3.1/DEVELOPMENT.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1763 2020-12-24 03:52:45.000000 vit-2.3.1/INSTALL.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1070 2020-12-24 03:52:45.000000 vit-2.3.1/LICENSE
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      299 2020-12-24 03:52:45.000000 vit-2.3.1/MANIFEST.in
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2911 2023-06-25 00:59:42.065125 vit-2.3.1/PKG-INFO
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1985 2022-05-09 14:29:06.000000 vit-2.3.1/README.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      104 2021-02-28 21:10:00.000000 vit-2.3.1/pyproject.toml
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2022-04-17 22:57:32.000000 vit-2.3.1/requirements.txt
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.033125 vit-2.3.1/scripts/
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.037125 vit-2.3.1/scripts/bash/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      153 2020-12-24 03:52:45.000000 vit-2.3.1/scripts/bash/vit.bash_completion
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       38 2023-06-25 00:59:42.065125 vit-2.3.1/setup.cfg
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1823 2023-04-14 04:10:49.000000 vit-2.3.1/setup.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.045125 vit-2.3.1/test/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.3.1/test/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2934 2021-11-04 13:51:45.000000 vit-2.3.1/test/test_list_batcher.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.049125 vit-2.3.1/vit/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      194 2020-12-24 03:52:45.000000 vit-2.3.1/vit/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2491 2023-04-14 04:10:49.000000 vit-2.3.1/vit/action_manager.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3834 2023-04-14 04:10:49.000000 vit-2.3.1/vit/actions.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    45170 2023-04-14 04:10:49.000000 vit-2.3.1/vit/application.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    11394 2023-04-14 04:10:49.000000 vit-2.3.1/vit/autocomplete.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5154 2022-10-26 13:33:43.000000 vit-2.3.1/vit/base_list_box.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    12121 2023-04-14 04:10:49.000000 vit-2.3.1/vit/color.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2491 2020-12-24 03:52:45.000000 vit-2.3.1/vit/color_mappings.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5466 2023-04-14 04:10:49.000000 vit-2.3.1/vit/command_bar.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      168 2022-04-28 01:54:06.000000 vit-2.3.1/vit/command_line.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.049125 vit-2.3.1/vit/config/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     9749 2022-10-21 16:59:04.000000 vit-2.3.1/vit/config/config.sample.ini
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    16940 2023-04-14 04:10:49.000000 vit-2.3.1/vit/config_parser.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      296 2020-12-24 03:52:45.000000 vit-2.3.1/vit/debug.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6442 2020-12-24 03:52:45.000000 vit-2.3.1/vit/denotation.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       73 2022-04-28 19:54:53.000000 vit-2.3.1/vit/env.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      495 2023-04-14 04:10:49.000000 vit-2.3.1/vit/event.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       92 2020-12-24 03:52:45.000000 vit-2.3.1/vit/exception.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.061125 vit-2.3.1/vit/formatter/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6781 2023-04-14 04:10:49.000000 vit-2.3.1/vit/formatter/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      342 2021-02-02 03:24:52.000000 vit-2.3.1/vit/formatter/depends.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      206 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/depends_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      224 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/depends_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/depends_list.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2493 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/description.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      100 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/description_combined.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      895 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/description_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      357 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/description_desc.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      637 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/description_oneline.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      483 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/description_truncated.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      718 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/description_truncated_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      253 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      129 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       69 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      131 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/due_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       66 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      120 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/end_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      138 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/entry_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       61 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/id.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       62 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/id_number.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6424 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/markers.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       71 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      150 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      156 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/modified_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/parent.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/parent_long.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      190 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/parent_short.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1143 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/project.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/project_full.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      162 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/project_indented.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      342 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/project_parent.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/recur.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/recur_duration.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      178 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/recur_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      307 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      165 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       93 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      167 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      171 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/scheduled_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      202 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_active.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/start_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      312 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/status.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/status_long.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      139 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/status_short.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      785 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/tags.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      440 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/tags_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/tags_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/tags_list.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      812 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/uda_date.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      385 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/uda_duration.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      471 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/uda_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      404 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/uda_numeric.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      369 2022-10-14 23:05:54.000000 vit-2.3.1/vit/formatter/uda_string.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      271 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/until_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/urgency.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/urgency_integer.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/urgency_real.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       63 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/uuid.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/uuid_long.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/uuid_short.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       67 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.1/vit/formatter/wait_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5402 2023-04-14 04:10:49.000000 vit-2.3.1/vit/formatter_base.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     7345 2023-04-14 04:10:49.000000 vit-2.3.1/vit/help.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2300 2023-04-14 04:10:49.000000 vit-2.3.1/vit/key_cache.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.061125 vit-2.3.1/vit/keybinding/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1573 2020-12-30 18:53:00.000000 vit-2.3.1/vit/keybinding/vi.ini
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6801 2023-04-14 04:10:49.000000 vit-2.3.1/vit/keybinding_parser.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1662 2023-04-14 04:10:49.000000 vit-2.3.1/vit/list_batcher.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1182 2023-04-14 04:10:49.000000 vit-2.3.1/vit/loader.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3187 2023-04-14 04:10:49.000000 vit-2.3.1/vit/markers.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2050 2020-12-24 03:52:45.000000 vit-2.3.1/vit/multi_widget.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2692 2023-01-06 12:19:59.000000 vit-2.3.1/vit/option_parser.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1491 2023-04-14 04:10:49.000000 vit-2.3.1/vit/pid_manager.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2087 2023-04-14 04:10:49.000000 vit-2.3.1/vit/process.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5606 2023-04-14 04:10:49.000000 vit-2.3.1/vit/readline.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1978 2023-04-14 04:10:49.000000 vit-2.3.1/vit/registry.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5214 2023-04-14 04:10:49.000000 vit-2.3.1/vit/task.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    23608 2023-04-14 04:10:49.000000 vit-2.3.1/vit/task_list.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.065125 vit-2.3.1/vit/theme/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.3.1/vit/theme/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      842 2020-12-24 03:52:45.000000 vit-2.3.1/vit/theme/classic.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      926 2020-12-24 03:52:45.000000 vit-2.3.1/vit/theme/default.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      410 2020-12-24 03:52:45.000000 vit-2.3.1/vit/uda.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1496 2023-06-22 13:35:29.000000 vit-2.3.1/vit/util.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       14 2023-06-25 00:58:01.000000 vit-2.3.1/vit/version.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      483 2021-11-04 13:51:45.000000 vit-2.3.1/vit/xdg.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-06-25 00:59:42.049125 vit-2.3.1/vit.egg-info/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2911 2023-06-25 00:59:42.000000 vit-2.3.1/vit.egg-info/PKG-INFO
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     4454 2023-06-25 00:59:42.000000 vit-2.3.1/vit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2023-06-25 00:59:42.000000 vit-2.3.1/vit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       46 2023-06-25 00:59:42.000000 vit-2.3.1/vit.egg-info/entry_points.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2019-09-28 15:34:44.000000 vit-2.3.1/vit.egg-info/not-zip-safe
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       74 2023-06-25 00:59:42.000000 vit-2.3.1/vit.egg-info/requires.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        4 2023-06-25 00:59:42.000000 vit-2.3.1/vit.egg-info/top_level.txt
```

### Comparing `vit-2.3.0/AUTHORS.md` & `vit-2.3.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/COLOR.md` & `vit-2.3.1/COLOR.md`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/CUSTOMIZE.md` & `vit-2.3.1/CUSTOMIZE.md`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/DEVELOPMENT.md` & `vit-2.3.1/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/INSTALL.md` & `vit-2.3.1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/LICENSE` & `vit-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/PKG-INFO` & `vit-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit
-Version: 2.3.0
+Version: 2.3.1
 Summary: Visual Interactive Taskwarrior full-screen terminal interface
 Home-page: https://github.com/vit-project/vit
 Author: Chad Phillips
 Author-email: chad@apartmentlines.com
 Keywords: taskwarrior,console,tui,text-user-interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vit-2.3.0/README.md` & `vit-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/setup.py` & `vit-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/test/test_list_batcher.py` & `vit-2.3.1/test/test_list_batcher.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/action_manager.py` & `vit-2.3.1/vit/action_manager.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/actions.py` & `vit-2.3.1/vit/actions.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/application.py` & `vit-2.3.1/vit/application.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/autocomplete.py` & `vit-2.3.1/vit/autocomplete.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/base_list_box.py` & `vit-2.3.1/vit/base_list_box.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/color.py` & `vit-2.3.1/vit/color.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/color_mappings.py` & `vit-2.3.1/vit/color_mappings.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/command_bar.py` & `vit-2.3.1/vit/command_bar.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/config/config.sample.ini` & `vit-2.3.1/vit/config/config.sample.ini`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/config_parser.py` & `vit-2.3.1/vit/config_parser.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/denotation.py` & `vit-2.3.1/vit/denotation.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/__init__.py` & `vit-2.3.1/vit/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/description.py` & `vit-2.3.1/vit/formatter/description.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/description_count.py` & `vit-2.3.1/vit/formatter/description_count.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/description_oneline.py` & `vit-2.3.1/vit/formatter/description_oneline.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/description_truncated_count.py` & `vit-2.3.1/vit/formatter/description_truncated_count.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/markers.py` & `vit-2.3.1/vit/formatter/markers.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/project.py` & `vit-2.3.1/vit/formatter/project.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/tags.py` & `vit-2.3.1/vit/formatter/tags.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter/uda_date.py` & `vit-2.3.1/vit/formatter/uda_date.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/formatter_base.py` & `vit-2.3.1/vit/formatter_base.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/help.py` & `vit-2.3.1/vit/help.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/key_cache.py` & `vit-2.3.1/vit/key_cache.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/keybinding/vi.ini` & `vit-2.3.1/vit/keybinding/vi.ini`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/keybinding_parser.py` & `vit-2.3.1/vit/keybinding_parser.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/list_batcher.py` & `vit-2.3.1/vit/list_batcher.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/loader.py` & `vit-2.3.1/vit/loader.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/markers.py` & `vit-2.3.1/vit/markers.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/multi_widget.py` & `vit-2.3.1/vit/multi_widget.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/option_parser.py` & `vit-2.3.1/vit/option_parser.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/pid_manager.py` & `vit-2.3.1/vit/pid_manager.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/process.py` & `vit-2.3.1/vit/process.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/readline.py` & `vit-2.3.1/vit/readline.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/registry.py` & `vit-2.3.1/vit/registry.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/task.py` & `vit-2.3.1/vit/task.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/task_list.py` & `vit-2.3.1/vit/task_list.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/theme/classic.py` & `vit-2.3.1/vit/theme/classic.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/theme/default.py` & `vit-2.3.1/vit/theme/default.py`

 * *Files identical despite different names*

### Comparing `vit-2.3.0/vit/util.py` & `vit-2.3.1/vit/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import sys
 import curses
 import shlex
-from functools import reduce
 
-from urwid.str_util import calc_width
+from urwid.util import calc_width
 
 curses.setupterm()
 e3_seq = curses.tigetstr('E3') or b''
 clear_screen_seq = curses.tigetstr('clear') or b''
 
 def clear_screen():
     os.write(sys.stdout.fileno(), e3_seq + clear_screen_seq)
```

### Comparing `vit-2.3.0/vit.egg-info/PKG-INFO` & `vit-2.3.1/vit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit
-Version: 2.3.0
+Version: 2.3.1
 Summary: Visual Interactive Taskwarrior full-screen terminal interface
 Home-page: https://github.com/vit-project/vit
 Author: Chad Phillips
 Author-email: chad@apartmentlines.com
 Keywords: taskwarrior,console,tui,text-user-interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vit-2.3.0/vit.egg-info/SOURCES.txt` & `vit-2.3.1/vit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

