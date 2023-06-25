# Comparing `tmp/endplay-0.4.8b0.tar.gz` & `tmp/endplay-0.4.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endplay-0.4.8b0.tar", last modified: Sat Sep 17 13:02:33 2022, max compression
+gzip compressed data, was "endplay-0.4.9b0.tar", last modified: Sun Jan 29 22:13:09 2023, max compression
```

## Comparing `endplay-0.4.8b0.tar` & `endplay-0.4.9b0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.623748 endplay-0.4.8b0/
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-09-17 13:02:16.000000 endplay-0.4.8b0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-09-17 13:02:16.000000 endplay-0.4.8b0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-17 13:02:16.000000 endplay-0.4.8b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    55314 2022-09-17 13:02:33.623748 endplay-0.4.8b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    54388 2022-09-17 13:02:16.000000 endplay-0.4.8b0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-17 13:02:16.000000 endplay-0.4.8b0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.611748 endplay-0.4.8b0/libs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.611748 endplay-0.4.8b0/libs/dds/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.611748 endplay-0.4.8b0/libs/dds/include/
--rw-r--r--   0 runner    (1001) docker     (121)    12250 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/include/dll.h
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/include/portab.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.615748 endplay-0.4.8b0/libs/dds/src/
--rw-r--r--   0 runner    (1001) docker     (121)    24774 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/ABsearch.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/ABsearch.h
--rw-r--r--   0 runner    (1001) docker     (121)     7780 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/ABstats.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/ABstats.h
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/COMMENT
--rw-r--r--   0 runner    (1001) docker     (121)     7701 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/CalcTables.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/CalcTables.h
--rw-r--r--   0 runner    (1001) docker     (121)    15750 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/DealerPar.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Exports.def
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/File.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/File.h
--rw-r--r--   0 runner    (1001) docker     (121)    16905 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Init.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Init.h
--rw-r--r--   0 runner    (1001) docker     (121)     7457 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/LaterTricks.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/LaterTricks.h
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Makefile_Win_clang_static
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Memory.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Memory.h
--rw-r--r--   0 runner    (1001) docker     (121)    68184 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Moves.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5421 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Moves.h
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/PBN.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/PBN.h
--rw-r--r--   0 runner    (1001) docker     (121)    38509 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Par.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9692 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/PlayAnalyser.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/PlayAnalyser.h
--rw-r--r--   0 runner    (1001) docker     (121)    29161 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/QuickTricks.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/QuickTricks.h
--rw-r--r--   0 runner    (1001) docker     (121)    21901 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Scheduler.h
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/SolveBoard.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/SolveBoard.h
--rw-r--r--   0 runner    (1001) docker     (121)    29045 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/SolverIF.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/SolverIF.h
--rw-r--r--   0 runner    (1001) docker     (121)    18777 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/System.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/System.h
--rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/ThreadMgr.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/ThreadMgr.h
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimeStat.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimeStat.h
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimeStatList.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimeStatList.h
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Timer.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/Timer.h
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimerGroup.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimerGroup.h
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimerList.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TimerList.h
--rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TransTable.h
--rw-r--r--   0 runner    (1001) docker     (121)    46485 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TransTableL.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7960 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TransTableL.h
--rw-r--r--   0 runner    (1001) docker     (121)    20351 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TransTableS.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/TransTableS.h
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/dds.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/dds.h
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/dds.rc
--rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/debug.h
--rw-r--r--   0 runner    (1001) docker     (121)     8355 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/dump.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/dump.h
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-09-17 13:02:20.000000 endplay-0.4.8b0/libs/dds/src/parallel.h
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-17 13:02:16.000000 endplay-0.4.8b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-09-17 13:02:33.623748 endplay-0.4.8b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-09-17 13:02:16.000000 endplay-0.4.8b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.611748 endplay-0.4.8b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.615748 endplay-0.4.8b0/src/endplay/
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/_dds/
--rw-r--r--   0 runner    (1001) docker     (121)    15992 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/_dds/__init__.py.in
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/config.py.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/dds/
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5888 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dds/analyse.py
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dds/ddtable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dds/parscore.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dds/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/dealer/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/dealer/actions/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/latex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/dealer/actions/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/templates/postamble.html
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/templates/postamble.tex
--rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/templates/preamble.html
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/templates/preamble.tex
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/actions/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)    11054 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/constraint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7974 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     8826 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/dealer/runscript.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/evaluate/
--rw-r--r--   0 runner    (1001) docker     (121)    12497 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/evaluate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/experimental/playdetect.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/interact/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/interact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/interact/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/interact/frontends/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/interact/frontends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6750 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/interact/frontends/cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/interact/frontends/curses.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/interact/frontends/tk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/interact/interactivedeal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15039 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/parsers/dealer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6857 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/parsers/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/parsers/lin.py
--rw-r--r--   0 runner    (1001) docker     (121)    16151 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/parsers/pbn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay/stats/
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.623748 endplay-0.4.8b0/src/endplay/types/
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/bid.py
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/board.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/card.py
--rw-r--r--   0 runner    (1001) docker     (121)     7088 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/contract.py
--rw-r--r--   0 runner    (1001) docker     (121)    14453 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/deal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/denom.py
--rw-r--r--   0 runner    (1001) docker     (121)     6388 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/hand.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/penalty.py
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/player.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/rank.py
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/suitholding.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/types/vul.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.623748 endplay-0.4.8b0/src/endplay/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     3233 2022-09-17 13:02:16.000000 endplay-0.4.8b0/src/endplay/utils/play.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 13:02:33.619748 endplay-0.4.8b0/src/endplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    55314 2022-09-17 13:02:33.000000 endplay-0.4.8b0/src/endplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-09-17 13:02:33.000000 endplay-0.4.8b0/src/endplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-17 13:02:33.000000 endplay-0.4.8b0/src/endplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-09-17 13:02:33.000000 endplay-0.4.8b0/src/endplay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-17 13:02:33.000000 endplay-0.4.8b0/src/endplay.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-17 13:02:33.000000 endplay-0.4.8b0/src/endplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-17 13:02:33.000000 endplay-0.4.8b0/src/endplay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.024398 endplay-0.4.9b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-01-29 22:12:52.000000 endplay-0.4.9b0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-01-29 22:12:52.000000 endplay-0.4.9b0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-01-29 22:12:52.000000 endplay-0.4.9b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    55314 2023-01-29 22:13:09.024398 endplay-0.4.9b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54388 2023-01-29 22:12:52.000000 endplay-0.4.9b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-29 22:12:52.000000 endplay-0.4.9b0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.004398 endplay-0.4.9b0/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.004398 endplay-0.4.9b0/libs/dds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.008398 endplay-0.4.9b0/libs/dds/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/include/dll.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/include/portab.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.016398 endplay-0.4.9b0/libs/dds/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/ABsearch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/ABsearch.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/ABstats.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/ABstats.h
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/COMMENT
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/CalcTables.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/CalcTables.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/DealerPar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Exports.def
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/File.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/File.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Init.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Init.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/LaterTricks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/LaterTricks.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Makefile_Win_clang_static
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)    68184 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Moves.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Moves.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/PBN.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/PBN.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38509 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Par.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/PlayAnalyser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/PlayAnalyser.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/QuickTricks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/QuickTricks.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21901 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/SolveBoard.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/SolveBoard.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/SolverIF.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/SolverIF.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/System.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/System.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/ThreadMgr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/ThreadMgr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimeStat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimeStat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimeStatList.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimeStatList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Timer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/Timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimerGroup.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimerGroup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimerList.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TimerList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TransTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46485 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TransTableL.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TransTableL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TransTableS.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/TransTableS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/dds.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/dds.h
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/dds.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/dump.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/dump.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-29 22:12:56.000000 endplay-0.4.9b0/libs/dds/src/parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-29 22:12:52.000000 endplay-0.4.9b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-01-29 22:13:09.024398 endplay-0.4.9b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-01-29 22:12:52.000000 endplay-0.4.9b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.004398 endplay-0.4.9b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.016398 endplay-0.4.9b0/src/endplay/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.016398 endplay-0.4.9b0/src/endplay/_dds/
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/_dds/__init__.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/config.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.016398 endplay-0.4.9b0/src/endplay/dds/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dds/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dds/ddtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dds/parscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dds/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/dealer/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/dealer/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/latex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/dealer/actions/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/templates/postamble.html
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/templates/postamble.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/templates/preamble.html
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/templates/preamble.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/actions/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/dealer/runscript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/evaluate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/experimental/playdetect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/interact/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/interact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/interact/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/interact/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/interact/frontends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/interact/frontends/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/interact/frontends/curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/interact/frontends/tk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/interact/interactivedeal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/parsers/dealer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/parsers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/parsers/lin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/parsers/pbn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.020398 endplay-0.4.9b0/src/endplay/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.024398 endplay-0.4.9b0/src/endplay/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/deal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/denom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/penalty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/suitholding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/types/vul.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.024398 endplay-0.4.9b0/src/endplay/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-01-29 22:12:52.000000 endplay-0.4.9b0/src/endplay/utils/play.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:13:09.016398 endplay-0.4.9b0/src/endplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55314 2023-01-29 22:13:08.000000 endplay-0.4.9b0/src/endplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-01-29 22:13:09.000000 endplay-0.4.9b0/src/endplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 22:13:08.000000 endplay-0.4.9b0/src/endplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-29 22:13:08.000000 endplay-0.4.9b0/src/endplay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 22:13:08.000000 endplay-0.4.9b0/src/endplay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-29 22:13:08.000000 endplay-0.4.9b0/src/endplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-29 22:13:08.000000 endplay-0.4.9b0/src/endplay.egg-info/top_level.txt
```

### Comparing `endplay-0.4.8b0/CMakeLists.txt` & `endplay-0.4.9b0/CMakeLists.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-cmake_minimum_required(VERSION 3.13)
-project(endplay)
-
-# Global settings
-# ===============
-
-if (NOT CMAKE_BUILD_TYPE)
-	message(WARNING "CMAKE_BUILD_TYPE not specified; defaulting to 'Release'")
-	set(CMAKE_BUILD_TYPE Release)
-endif()
-set(CMAKE_CXX_STANDARD 17)
-
-set(ENDPLAY_ROOT_DIR "${CMAKE_CURRENT_SOURCE_DIR}/src/endplay")
-file(READ "${CMAKE_CURRENT_SOURCE_DIR}/VERSION" ENDPLAY_VERSION)
-string(REGEX REPLACE "\n$" "" ENDPLAY_VERSION "${ENDPLAY_VERSION}")
-string(TIMESTAMP ENDPLAY_BUILD_TIME)
-
-# Detect compiler
-if (CMAKE_CXX_COMPILER_ID STREQUAL "Clang")
-	set(CC_CLANG 1)
-elseif (CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
-	set(CC_GCC 1)
-elseif (CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
-	set(CC_MSVC 1)
-else()
-	message(WARNING "The compiler you are using hasn't been tested for building this library.")
-endif()
-
-# Pretend to use SETUPTOOLS_BUILD variable to stop it complaining
-if (SETUPTOOLS_BUILD)
-	message(STATUS "Call to CMake was invocated by setuptools")
-endif()
-
-if (COMPILE_32_BITS)
-	add_compile_options("-m32")
-	add_link_options("-m32")
-endif()
-
-# Configure config.py with version number
-# =======================================
-configure_file("${ENDPLAY_ROOT_DIR}/config.py.in" "config.py" @ONLY)
-install(FILES "${CMAKE_CURRENT_BINARY_DIR}/config.py" DESTINATION "endplay")
-
-
-# _dds library
-# ============
-
-# Compile the source files for the DDS library together into a shared library file
-set(DDS_ROOT_DIR "${CMAKE_CURRENT_SOURCE_DIR}/libs/dds/")
-set(DDS_SOURCE
-	dds.cpp             dump.cpp            ABsearch.cpp
-	ABstats.cpp         CalcTables.cpp      DealerPar.cpp
-	File.cpp            Init.cpp            LaterTricks.cpp
-	Memory.cpp          Moves.cpp           Par.cpp
-	PlayAnalyser.cpp    PBN.cpp             QuickTricks.cpp
-	Scheduler.cpp       SolveBoard.cpp      SolverIF.cpp
-	System.cpp          ThreadMgr.cpp       Timer.cpp
-	TimerGroup.cpp      TimerList.cpp       TimeStat.cpp
-	TimeStatList.cpp    TransTableS.cpp     TransTableL.cpp)
-if (CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
-	set(DDS_SOURCE ${DDS_SOURCE} exports.def dds.rc)
-endif()
-list(TRANSFORM DDS_SOURCE PREPEND "${DDS_ROOT_DIR}/src/")
-
-add_library(dds SHARED ${DDS_SOURCE})
-target_compile_definitions(dds PRIVATE "DDS_THREADS_STL")
-target_include_directories(dds PRIVATE "${DDS_ROOT_DIR}/src")
-# Compiler specific flags
-if (CC_GCC)
-	target_compile_options(dds PRIVATE "-Wno-format-overflow")
-elseif (CC_MSVC)
-	target_compile_definitions(dds PRIVATE "_CRT_SECURE_NO_WARNINGS")
-	target_compile_options(dds PRIVATE "/wd4267")
-endif()
-
-# Copy some macro definitions from the c header file into the
-# __init__.py for the package
-file(READ "${DDS_ROOT_DIR}/include/dll.h" DDS_DLL_H)
-string(REGEX MATCH "#define MAXNOOFBOARDS [0-9]+" DDS_MAXNOOFBOARDS "${DDS_DLL_H}")
-string(REGEX MATCH "[0-9]+" DDS_MAXNOOFBOARDS "${DDS_MAXNOOFBOARDS}")
-string(REGEX MATCH "#define MAXNOOFTABLES [0-9]+" DDS_MAXNOOFTABLES "${DDS_DLL_H}")
-string(REGEX MATCH "[0-9]+" DDS_MAXNOOFTABLES "${DDS_MAXNOOFTABLES}")
-set(DDS_LIBRARY_NAME "${CMAKE_SHARED_LIBRARY_PREFIX}dds${CMAKE_SHARED_LIBRARY_SUFFIX}")
-configure_file("${ENDPLAY_ROOT_DIR}/_dds/__init__.py.in" "_dds/__init__.py" @ONLY)
-
-# Install both bits into the right places in the package  
-if (CC_MSVC)
-	# .dll is a runtime component
-	install(TARGETS dds RUNTIME DESTINATION "endplay/_dds")
-else()
-	install(TARGETS dds DESTINATION "endplay/_dds")
-endif()
-
+cmake_minimum_required(VERSION 3.13)
+project(endplay)
+
+# Global settings
+# ===============
+
+if (NOT CMAKE_BUILD_TYPE)
+	message(WARNING "CMAKE_BUILD_TYPE not specified; defaulting to 'Release'")
+	set(CMAKE_BUILD_TYPE Release)
+endif()
+set(CMAKE_CXX_STANDARD 17)
+
+set(ENDPLAY_ROOT_DIR "${CMAKE_CURRENT_SOURCE_DIR}/src/endplay")
+file(READ "${CMAKE_CURRENT_SOURCE_DIR}/VERSION" ENDPLAY_VERSION)
+string(REGEX REPLACE "\n$" "" ENDPLAY_VERSION "${ENDPLAY_VERSION}")
+string(TIMESTAMP ENDPLAY_BUILD_TIME)
+
+# Detect compiler
+if (CMAKE_CXX_COMPILER_ID STREQUAL "Clang")
+	set(CC_CLANG 1)
+elseif (CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
+	set(CC_GCC 1)
+elseif (CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
+	set(CC_MSVC 1)
+else()
+	message(WARNING "The compiler you are using hasn't been tested for building this library.")
+endif()
+
+# Pretend to use SETUPTOOLS_BUILD variable to stop it complaining
+if (SETUPTOOLS_BUILD)
+	message(STATUS "Call to CMake was invocated by setuptools")
+endif()
+
+if (COMPILE_32_BITS)
+	add_compile_options("-m32")
+	add_link_options("-m32")
+endif()
+
+# Configure config.py with version number
+# =======================================
+configure_file("${ENDPLAY_ROOT_DIR}/config.py.in" "config.py" @ONLY)
+install(FILES "${CMAKE_CURRENT_BINARY_DIR}/config.py" DESTINATION "endplay")
+
+
+# _dds library
+# ============
+
+# Compile the source files for the DDS library together into a shared library file
+set(DDS_ROOT_DIR "${CMAKE_CURRENT_SOURCE_DIR}/libs/dds/")
+set(DDS_SOURCE
+	dds.cpp             dump.cpp            ABsearch.cpp
+	ABstats.cpp         CalcTables.cpp      DealerPar.cpp
+	File.cpp            Init.cpp            LaterTricks.cpp
+	Memory.cpp          Moves.cpp           Par.cpp
+	PlayAnalyser.cpp    PBN.cpp             QuickTricks.cpp
+	Scheduler.cpp       SolveBoard.cpp      SolverIF.cpp
+	System.cpp          ThreadMgr.cpp       Timer.cpp
+	TimerGroup.cpp      TimerList.cpp       TimeStat.cpp
+	TimeStatList.cpp    TransTableS.cpp     TransTableL.cpp)
+if (CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
+	set(DDS_SOURCE ${DDS_SOURCE} exports.def dds.rc)
+endif()
+list(TRANSFORM DDS_SOURCE PREPEND "${DDS_ROOT_DIR}/src/")
+
+add_library(dds SHARED ${DDS_SOURCE})
+target_compile_definitions(dds PRIVATE "DDS_THREADS_STL")
+target_include_directories(dds PRIVATE "${DDS_ROOT_DIR}/src")
+# Compiler specific flags
+if (CC_GCC)
+	target_compile_options(dds PRIVATE "-Wno-format-overflow")
+elseif (CC_MSVC)
+	target_compile_definitions(dds PRIVATE "_CRT_SECURE_NO_WARNINGS")
+	target_compile_options(dds PRIVATE "/wd4267")
+endif()
+
+# Copy some macro definitions from the c header file into the
+# __init__.py for the package
+file(READ "${DDS_ROOT_DIR}/include/dll.h" DDS_DLL_H)
+string(REGEX MATCH "#define MAXNOOFBOARDS [0-9]+" DDS_MAXNOOFBOARDS "${DDS_DLL_H}")
+string(REGEX MATCH "[0-9]+" DDS_MAXNOOFBOARDS "${DDS_MAXNOOFBOARDS}")
+string(REGEX MATCH "#define MAXNOOFTABLES [0-9]+" DDS_MAXNOOFTABLES "${DDS_DLL_H}")
+string(REGEX MATCH "[0-9]+" DDS_MAXNOOFTABLES "${DDS_MAXNOOFTABLES}")
+set(DDS_LIBRARY_NAME "${CMAKE_SHARED_LIBRARY_PREFIX}dds${CMAKE_SHARED_LIBRARY_SUFFIX}")
+configure_file("${ENDPLAY_ROOT_DIR}/_dds/__init__.py.in" "_dds/__init__.py" @ONLY)
+
+# Install both bits into the right places in the package  
+if (CC_MSVC)
+	# .dll is a runtime component
+	install(TARGETS dds RUNTIME DESTINATION "endplay/_dds")
+else()
+	install(TARGETS dds DESTINATION "endplay/_dds")
+endif()
+
 install(FILES "${CMAKE_CURRENT_BINARY_DIR}/_dds/__init__.py" DESTINATION "endplay/_dds/")
```

### Comparing `endplay-0.4.8b0/LICENCE` & `endplay-0.4.9b0/LICENCE`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/PKG-INFO` & `endplay-0.4.9b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endplay
-Version: 0.4.8b0
+Version: 0.4.9b0
 Summary: A suite of tools for generation and analysis of bridge deals
 Home-page: https://github.com/dominicprice/endplay
 Author: Dominic Price
 Author-email: dominicprice@outlook.com
 Project-URL: Documentation, https://endplay.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/dominicprice/endplay/issues
 Keywords: bridge,cards,games,double dummy,dds,analysis,stats,deal,dealer
```

### Comparing `endplay-0.4.8b0/README.md` & `endplay-0.4.9b0/README.md`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/include/dll.h` & `endplay-0.4.9b0/libs/dds/include/dll.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/include/portab.h` & `endplay-0.4.9b0/libs/dds/include/portab.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/ABsearch.cpp` & `endplay-0.4.9b0/libs/dds/src/ABsearch.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/ABsearch.h` & `endplay-0.4.9b0/libs/dds/src/ABsearch.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/ABstats.cpp` & `endplay-0.4.9b0/libs/dds/src/ABstats.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/ABstats.h` & `endplay-0.4.9b0/libs/dds/src/ABstats.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/CalcTables.cpp` & `endplay-0.4.9b0/libs/dds/src/CalcTables.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/CalcTables.h` & `endplay-0.4.9b0/libs/dds/src/CalcTables.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/DealerPar.cpp` & `endplay-0.4.9b0/libs/dds/src/DealerPar.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Exports.def` & `endplay-0.4.9b0/libs/dds/src/Exports.def`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/File.cpp` & `endplay-0.4.9b0/libs/dds/src/File.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/File.h` & `endplay-0.4.9b0/libs/dds/src/File.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Init.cpp` & `endplay-0.4.9b0/libs/dds/src/Init.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/LaterTricks.cpp` & `endplay-0.4.9b0/libs/dds/src/LaterTricks.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/LaterTricks.h` & `endplay-0.4.9b0/libs/dds/src/LaterTricks.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Makefile_Win_clang_static` & `endplay-0.4.9b0/libs/dds/src/Makefile_Win_clang_static`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Memory.cpp` & `endplay-0.4.9b0/libs/dds/src/Memory.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Memory.h` & `endplay-0.4.9b0/libs/dds/src/Memory.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Moves.cpp` & `endplay-0.4.9b0/libs/dds/src/Moves.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Moves.h` & `endplay-0.4.9b0/libs/dds/src/Moves.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/PBN.cpp` & `endplay-0.4.9b0/libs/dds/src/PBN.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Par.cpp` & `endplay-0.4.9b0/libs/dds/src/Par.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/PlayAnalyser.cpp` & `endplay-0.4.9b0/libs/dds/src/PlayAnalyser.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/PlayAnalyser.h` & `endplay-0.4.9b0/libs/dds/src/PlayAnalyser.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/QuickTricks.cpp` & `endplay-0.4.9b0/libs/dds/src/QuickTricks.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/QuickTricks.h` & `endplay-0.4.9b0/libs/dds/src/QuickTricks.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Scheduler.cpp` & `endplay-0.4.9b0/libs/dds/src/Scheduler.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Scheduler.h` & `endplay-0.4.9b0/libs/dds/src/Scheduler.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/SolveBoard.cpp` & `endplay-0.4.9b0/libs/dds/src/SolveBoard.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/SolveBoard.h` & `endplay-0.4.9b0/libs/dds/src/SolveBoard.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/SolverIF.cpp` & `endplay-0.4.9b0/libs/dds/src/SolverIF.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/SolverIF.h` & `endplay-0.4.9b0/libs/dds/src/SolverIF.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/System.cpp` & `endplay-0.4.9b0/libs/dds/src/System.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/System.h` & `endplay-0.4.9b0/libs/dds/src/System.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/ThreadMgr.cpp` & `endplay-0.4.9b0/libs/dds/src/ThreadMgr.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/ThreadMgr.h` & `endplay-0.4.9b0/libs/dds/src/ThreadMgr.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimeStat.cpp` & `endplay-0.4.9b0/libs/dds/src/TimeStat.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimeStat.h` & `endplay-0.4.9b0/libs/dds/src/TimeStat.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimeStatList.cpp` & `endplay-0.4.9b0/libs/dds/src/TimeStatList.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimeStatList.h` & `endplay-0.4.9b0/libs/dds/src/TimeStatList.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Timer.cpp` & `endplay-0.4.9b0/libs/dds/src/Timer.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/Timer.h` & `endplay-0.4.9b0/libs/dds/src/Timer.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimerGroup.cpp` & `endplay-0.4.9b0/libs/dds/src/TimerGroup.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimerGroup.h` & `endplay-0.4.9b0/libs/dds/src/TimerGroup.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimerList.cpp` & `endplay-0.4.9b0/libs/dds/src/TimerList.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TimerList.h` & `endplay-0.4.9b0/libs/dds/src/TimerList.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TransTable.h` & `endplay-0.4.9b0/libs/dds/src/TransTable.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TransTableL.cpp` & `endplay-0.4.9b0/libs/dds/src/TransTableL.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TransTableL.h` & `endplay-0.4.9b0/libs/dds/src/TransTableL.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TransTableS.cpp` & `endplay-0.4.9b0/libs/dds/src/TransTableS.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/TransTableS.h` & `endplay-0.4.9b0/libs/dds/src/TransTableS.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/dds.cpp` & `endplay-0.4.9b0/libs/dds/src/dds.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/dds.h` & `endplay-0.4.9b0/libs/dds/src/dds.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/dds.rc` & `endplay-0.4.9b0/libs/dds/src/dds.rc`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/debug.h` & `endplay-0.4.9b0/libs/dds/src/debug.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/dump.cpp` & `endplay-0.4.9b0/libs/dds/src/dump.cpp`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/dump.h` & `endplay-0.4.9b0/libs/dds/src/dump.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/libs/dds/src/parallel.h` & `endplay-0.4.9b0/libs/dds/src/parallel.h`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/setup.cfg` & `endplay-0.4.9b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/setup.py` & `endplay-0.4.9b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿#!/usr/bin/env python3
+#!/usr/bin/env python3
 
 import os
 import pathlib
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 
 class CMakeExtension(Extension):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/_dds/__init__.py.in` & `endplay-0.4.9b0/src/endplay/_dds/__init__.py.in`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/config.py.in` & `endplay-0.4.9b0/src/endplay/config.py.in`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-﻿"""
-Configuration and versioning information
-"""
-
-__all__ = ["__version__", "__version_info__", "__author__", "use_unicode", "suppress_unicode"]
-
-from contextlib import ContextDecorator
-
-# Packages metadata, used by setuptools etc
-__version__ = """@ENDPLAY_VERSION@""".strip()
-"""Version of the library as a string"""
-
-__version_info__ = tuple(int(i) if i.isdigit() else i for i in __version__.replace("-", ".").split("."))
-"""Version of the library as a tuple of integers"""
-
-__author__ = "Dominic Price"
-"""Author of the library"""
-
-__buildtime__ = """@ENDPLAY_BUILD_TIME@""".strip()
-
-use_unicode = True 
-"""If set to False, the library will only print characters in the ASCII range"""
-
-class suppress_unicode(ContextDecorator):
-	"""
-	Context manager to temporarily ensure that unicode output is turned off,
-	for example when writing to a file which expects suit symbols to be
-	SDHC.
-
-	Example usage::
-
-		print(Denom.hearts.abbr) # prints ♥ (assuming config.use_unicode=True)
-		with suppress_unicode():
-			print(Denom.hearts.abbr) # prints H
-		print(Denom.hearts.abbr) # prints ♥
-	"""
-	def __enter__(self):
-		global use_unicode
-		self.use_unicode = use_unicode
-		use_unicode = False
-		return self
-
-	def __exit__(self, *exc):
-		global use_unicode
-		use_unicode = self.use_unicode
-		return False
+"""
+Configuration and versioning information
+"""
+
+__all__ = ["__version__", "__version_info__", "__author__", "use_unicode", "suppress_unicode"]
+
+from contextlib import ContextDecorator
+
+# Packages metadata, used by setuptools etc
+__version__ = """@ENDPLAY_VERSION@""".strip()
+"""Version of the library as a string"""
+
+__version_info__ = tuple(int(i) if i.isdigit() else i for i in __version__.replace("-", ".").split("."))
+"""Version of the library as a tuple of integers"""
+
+__author__ = "Dominic Price"
+"""Author of the library"""
+
+__buildtime__ = """@ENDPLAY_BUILD_TIME@""".strip()
+
+use_unicode = True 
+"""If set to False, the library will only print characters in the ASCII range"""
+
+class suppress_unicode(ContextDecorator):
+	"""
+	Context manager to temporarily ensure that unicode output is turned off,
+	for example when writing to a file which expects suit symbols to be
+	SDHC.
+
+	Example usage::
+
+		print(Denom.hearts.abbr) # prints ♥ (assuming config.use_unicode=True)
+		with suppress_unicode():
+			print(Denom.hearts.abbr) # prints H
+		print(Denom.hearts.abbr) # prints ♥
+	"""
+	def __enter__(self):
+		global use_unicode
+		self.use_unicode = use_unicode
+		use_unicode = False
+		return self
+
+	def __exit__(self, *exc):
+		global use_unicode
+		use_unicode = self.use_unicode
+		return False
```

### Comparing `endplay-0.4.8b0/src/endplay/dds/analyse.py` & `endplay-0.4.9b0/src/endplay/dds/analyse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Analysis functions from the DDS library, which calculate the double dummy
 number of tricks available given a play history.
 """
 
 from __future__ import annotations
 
 __all__ = [
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dds/ddtable.py` & `endplay-0.4.9b0/src/endplay/dds/ddtable.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/dds/parscore.py` & `endplay-0.4.9b0/src/endplay/dds/parscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Par contract and scoring function
 """
 
 from __future__ import annotations
 
 __all__ = ["ParList", "par"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dds/solve.py` & `endplay-0.4.9b0/src/endplay/dds/solve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Solving functions from the DDS library, which calculate the double dummy
 results for playing each card in a player's hand.
 """
 
 from __future__ import annotations
 
 __all__ = ["SolvedBoard", "SolvedBoardList", "solve_board", "solve_all_boards"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dealer/__init__.py` & `endplay-0.4.9b0/src/endplay/dealer/__init__.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/dealer/__main__.py` & `endplay-0.4.9b0/src/endplay/dealer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 The endplay.dealer program is a reimplementation of Hans van Staveren's dealer program
 which can be used to generate hands for partnerships bidding training or for
 generating statistics that can be used to design conventions, or win postmortems.
 
 While compatibility with the original has been a design goal, the precise format of the
 output is not expected to correspond 1:1 with the original program. Furthermore, several
 extra options including the ability to specify actions and constraints at the command line
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dealer/actions/__init__.py` & `endplay-0.4.9b0/src/endplay/dealer/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 The Actions classes provide a common interface for producing different
 types of output from a dealer script. When a script is run, an appropriate
 Actions object is constructed, and any time output is requested one of the
 methods is called to format it correctly.
 """
 
 __all__ = ["BaseActions", "TerminalActions", "LaTeXActions", "HTMLActions"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dealer/actions/base.py` & `endplay-0.4.9b0/src/endplay/dealer/actions/base.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/dealer/actions/html.py` & `endplay-0.4.9b0/src/endplay/dealer/actions/html.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/dealer/actions/latex.py` & `endplay-0.4.9b0/src/endplay/dealer/actions/latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Actions class for producing LaTeX output.
 """
 
 __all__ = ["LaTeXActions"]
 
 from endplay.dealer.actions.base import BaseActions
 from endplay.types import Denom, Player
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dealer/actions/templates/preamble.html` & `endplay-0.4.9b0/src/endplay/dealer/actions/templates/preamble.html`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/dealer/actions/terminal.py` & `endplay-0.4.9b0/src/endplay/dealer/actions/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Actions class for producing plaintext output.
 """
 
 __all__ = ["TerminalActions"]
 
 from io import StringIO
 from endplay.dealer.actions.base import BaseActions
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dealer/constraint.py` & `endplay-0.4.9b0/src/endplay/dealer/constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Engine for converting dealer-syntax expressions into evaluatable
 Python functions. You should not need to use this directly unless
 you are developing your own functions, as most functions accept
 strings as well as functions and automatically compile them using
 the machinery in this module.
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dealer/generate.py` & `endplay-0.4.9b0/src/endplay/dealer/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Generic routines for generating deals based on a set of constraints
 """
 
 from __future__ import annotations
 
 __all__ = ['generate_deal', 'generate_deals']
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/dealer/runscript.py` & `endplay-0.4.9b0/src/endplay/dealer/runscript.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 All-purpose routine for executing a dealer script file. This can be
 called directly from within Python to convert a dealer file into a 
 list of deals, but its main purpose is as the entry point for the
 main module.
 """
 
 from __future__ import annotations
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/evaluate/__init__.py` & `endplay-0.4.9b0/src/endplay/evaluate/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,326 +1,326 @@
-"""
-Functions for evaluating bridge hands using a variety of different metrics.
-"""
-
-from __future__ import annotations
-
-__all__ = [
-	"standard_hcp_scale", "bergen_hcp_scale", "hcp", "shortage_nofit_dist_scale", 
-	"shortage_fit_dist_scale", "length_dist_scale", "mixed_fit_dist_scale", 
-	"mixed_nofit_dist_scale", "dist_points", "total_points",
-	"top_honours", "losers", "cccc", "quality", "controls", "rule_of_n",
-	"exact_shape", "shape", "major_shape", "minor_shape", "is_balanced",
-	"is_semibalanced", "is_minor_semibalanced", "is_single_suited",
-	"is_two_suited", "is_three_suited"]
-
-from typing import Union, Optional
-from collections.abc import Iterable
-from endplay.types import Hand, SuitHolding, Card, Rank, AlternateRank, Denom
-
-# Points for each rank in order [A, K, Q, J, ...]
-standard_hcp_scale: list[int] = [4, 3, 2, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0]
-"""Classic HCP scale with A=4, K=3, Q=2, J=1"""
-bergen_hcp_scale: list[int] = [4.5, 3, 1.5, 0.75, 0.25, 0, 0, 0, 0, 0, 0, 0, 0]
-"""Bergen HCP scale with A=4.5, K=3, Q=1.5, J=0.75, T=0.25"""
-
-def hcp(
-	obj: Union[Iterable[Union[Card, Rank, AlternateRank]], Card, Rank, AlternateRank], 
-	scale: list[int] = standard_hcp_scale) -> float:
-	"""
-	Return the high card points of a hand or suit holding using a given scale. Two
-	scales are predefined: `standard_hcp_scale` which uses the traditional 4321
-	point scale, and `bergen_hcp_scale` which uses the Bergen scale.
-
-	:param obj: A (possibly iterable of) card or rank type to evaluate
-	:param scale: A list of 13 numbers which assign points to each rank in descending
-		order, e.g. [4,3,2,1,0,...] is used for the standard HCP scale where an ace is
-		worth 4 points, a king 3 etc...
-	"""
-	if len(scale) < 13:
-		scale = list(scale) + [0] * (13 - len(scale))
-	if isinstance(obj, Card):
-		return scale[14 - obj.rank.to_alternate()]
-	elif isinstance(obj, Rank):
-		return scale[14 - obj.to_alternate()]
-	elif isinstance(obj, AlternateRank):
-		return scale[14 - obj]
-	else:
-		return sum(hcp(card, scale) for card in obj)
-
-# Points for each suit length in order [0/void, 1/singleton, 2/doubleton, 3, ...]
-shortage_nofit_dist_scale: list[int] = [3, 2, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
-"""Distribution point scale with void=3, singleton=2, doubleton=1"""
-shortage_fit_dist_scale: list[int] = [5, 3, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
-"""Distribution point scale when a trump fit is found with void=5, singleton=3, doubleton=1"""
-length_dist_scale: list[int] = [0, 0, 0, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
-"""Distribution point scale which awards a point for each extra card in a suit over 4"""
-mixed_nofit_dist_scale: list[int] = [3, 2, 1, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
-"""Combined scale using `shortage_nofit_dist_scale` and `length_dist_scale`"""
-mixed_fit_dist_scale: list[int] = [5, 3, 1, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
-"""Combined scale using `shortage_fit_dist_scale` and `length_dist_scale`"""
-
-def dist_points(obj: Union[Hand, SuitHolding], scale: list[int] = shortage_nofit_dist_scale, exclude: Iterable[Denom] = []) -> float:
-	"""
-	Return the extra points for distribution for a hand or suit holding using the given scale.
-	Five scales are predefined: 
-
-	* `shortage_nofit_dist_scale`: Standard evaluation of shortage points if no trump fit is agreed, 
-	  void=3, singleton=2, doubleton=1
-
-	* `shortage_fit_dist_scale`: Standard evaluation of shortage points if trump fit is agreed, 
-	  void=5, singleton=3, doubleton=1
-
-	* `length_dist_scale`: Standard evaluation of length points, one point for each extra card in a 
-	  suit with more than four cards in it, i.e. 5 cards=1, 6 cards=2, etc...
-
-	:param obj: Hand or suit holding to evaluate
-	:param scale: A list of 14 numbers which assign points to each suit length in ascending order,
-		e.g. [3,2,1,0,...] is used for the standard shortage points where void=3, singleton=2 etc...
-	:param exclude: List of suits to be excluded from distribution calculations if a `Hand` object
-		is passed, in order to e.g. exclude the trump suit from the calculation
-	"""
-	if len(scale) < 14:
-		scale = list(scale) + [0] * (14 - len(scale))
-	if isinstance(obj, SuitHolding):
-		return scale[len(obj)]
-	return sum(dist_points(obj[suit], scale) if suit not in exclude else 0 for suit in Denom.suits())
-
-def total_points(
-	obj: Union[Hand, SuitHolding], 
-	hcp_scale: list[int] = standard_hcp_scale, 
-	dist_scale: list[int] = shortage_nofit_dist_scale,
-	trump: Optional[Denom] = None,
-	protect_honours: bool = False):
-	"""
-	Return the sum of high card points and distribution points in a hand.
-
-	:param obj: Hand or suit holding to evaluate
-	:param hcp_scale: The HCP scale to use, as for the `hcp` function
-	:param dist_scale: The distribution points scale, as for the `dist_scale` function
-	:param trump: If set then distribution points for the given suit are excluded from 
-		the calculation
-	:param protect_honours: If `True`, then honours must be protected for their HCP
-		to be included, i.e. king singleton, queen doubleton etc do not contribute to
-		total points
-	"""
-	if isinstance(obj, SuitHolding):
-		points = dist_points(obj, dist_scale, [trump] if trump is not None else [])
-		if protect_honours:
-			obj = obj.copy()
-			ncards = len(obj)
-			if ncards < 4: obj.remove(Rank.RJ)
-			if ncards < 3: obj.remove(Rank.RQ)
-			if ncards < 2: obj.remove(Rank.RK)
-		return hcp(obj, hcp_scale) + points
-	else:
-		return sum(total_points(obj[suit], hcp_scale, dist_scale, trump, protect_honours) for suit in Denom.suits())
-
-def top_honours(hand: Union[Hand, SuitHolding], lowest_honour: Union[Rank, int] = Rank.RJ) -> int:
-	"""
-	Return the number of top honors in a suit
-
-	:param suit: The suit holding to evaluate
-	:param lowest_honour: The lowest rank to be treated as an honour, or an
-		integer for how many top cards are honours
-	"""
-	if not isinstance(lowest_honour, Rank):
-		lowest_honour = AlternateRank(15 - lowest_honour).to_standard()
-	if isinstance(hand, SuitHolding):
-		return sum(1 for rank in hand if rank >= lowest_honour)
-	else:
-		return sum(1 for card in hand if card.rank >= lowest_honour)
-
-def losers(hand: Union[Hand, SuitHolding]) -> int:
-	"""
-	Returns the number of losers in a hand. The number of losers in each
-	suit is calculated as: (a) 3 or more cards in a suit: 3 - 1 per AKQ
-	(b) Doubleton: AK=0, Ax/Kx=1, else 2 (c) Singleton: A=0, else 1 (d) Void: 0
-	"""
-	if isinstance(hand, SuitHolding):
-		a, k, q = Rank.RA in hand, Rank.RK in hand, Rank.RQ in hand
-		if len(hand) == 0: return 0
-		if len(hand) == 1: return 1 - a
-		if len(hand) == 2: return 2 - a - k
-		return 3 - a - k - q
-	else:
-		return sum(losers(hand[suit]) for suit in Denom.suits())
-
-def cccc(hand: Union[Hand, SuitHolding]) -> float:
-	"""
-	Uses the Kaplan four cs algorithm from the October 1982 issue of Bridge world
-	magazine. This implementation is based on the interpretation of the algorithm
-	described on http://www.rpbridge.net/8j19.htm
-	"""
-	if isinstance(hand, Hand):
-		return sum(cccc(hand[suit]) for suit in Denom.suits())
-	l = len(hand)
-	score = 0
-	# 1-5: Count point values A=4,K=3,Q=2,J=1,T=0.5
-	if Rank.RA in hand: score += 4
-	if Rank.RK in hand: score += 3
-	if Rank.RQ in hand: score += 2
-	if Rank.RJ in hand: score += 1
-	if Rank.RT in hand: score += 0.5
-	# 6-7: if between 2-6 cards, count points for supported T and 9
-	if l >= 2 and l <= 6:
-		if (Rank.RT in hand) and ((Rank.RJ in hand) or top_honours(hand, 4) >= 2):
-			score += 0.5
-		if (Rank.R9 in hand) and ((Rank.R8 in hand or Rank.RT in hand) or top_honours(hand, 5) == 2):
-			score += 0.5
-	# 8: if between 4-6 cards, count 9 without any touching cards and exactly three higher honours
-	if l >= 4 and l <= 6:
-		if (Rank.R9 in hand) and not (Rank.R8 in hand and Rank.RT in hand) and top_honours(hand, 4) == 3:
-			score += 0.5
-	# 9: 7+ cards missing queen or jack (or both)
-	if l >= 7 and (Rank.RQ not in hand or Rank.RJ not in hand):
-		score += 1
-	# 10: 8+ cards missing queen
-	if l >= 8 and Rank.RQ not in hand:
-		score += 1
-	# 11: 9+ cards missing queen and jack
-	if l >= 9 and (Rank.RQ not in hand and Rank.RJ not in hand):
-		score += 1
-	# 12: Multiply current total by suit length, divide by 10, then continue
-	score *= l / 10
-	# 13: Add 3 for an ace
-	if Rank.RA in hand:
-		score += 3
-	# 14-15: Add 2 for guarded king and 0.5 for king singleton
-	if Rank.RK in hand:
-		if l > 1: score += 2
-		else: score += 0.5
-	# 16-19: Add values for queen
-	if Rank.RQ in hand:
-		if l >= 3:
-			# 16-17: 3+ cards, +1 if has higher honour else +0.75
-			if Rank.RK in hand or Rank.RA in hand:
-				score += 1
-			else:
-				score += 0.75
-		elif l == 2:
-			# 18-19: doubleton, +0.5 if has higher honour else +0.25
-			if Rank.RK in hand or Rank.RA in hand:
-				score += 0.5
-			else:
-				score += 0.25
-	# 20-21: Jack with two higher honours=0.5, one higher honour=0.25
-	if Rank.RJ in hand:
-		hh = top_honours(hand, 3)
-		if hh == 2:
-			score += 0.5
-		elif hh == 1:
-			score += 0.25
-	# 22-23: Ten with two higher honours=0.25, T9 with one higher honour=0.25
-	if Rank.RT in hand:
-		hh = top_honours(hand, 4)
-		if hh == 2:
-			score += 0.25
-		if Rank.R9 in hand and hh == 1:
-			score += 0.25
-	# 24-26: void=3, singleton=2, doubleton=1
-	if l == 0:
-		score += 3
-	elif l == 1:
-		score += 2
-	elif l == 2:
-		score += 1
-	return score
-
-def quality(hand: SuitHolding) -> float:
-	"Uses the quality algorithm (from the October 1982 issue of Bridge World magazine)"
-	raise NotImplementedError
-
-def controls(hand: Union[Iterable, Card, Rank]) -> int:
-	"Return the number of controls in a sequence, using A=2 and K=1"
-	if isinstance(hand, Rank):
-		if hand == Rank.RA: return 2
-		elif hand == Rank.RK: return 1
-		else: return 0
-	elif isinstance(hand, Card):
-		return controls(hand.rank)
-	else:
-		return sum(controls(card) for card in hand)
-
-def rule_of_n(hand: Hand) -> int:
-	"Returns the hcp of the hand added to the length of the two longest suits"
-	s = shape(hand)
-	return hcp(hand) + s[0] + s[1]
-
-def exact_shape(hand: Hand) -> list[int]:
-	"Return the shape of a hand as a list starting from spades, e.g. (5, 2, 3, 3)"
-	return [len(hand[suit]) for suit in Denom.suits()]
-
-def shape(hand: Hand) -> list[int]:
-	"""
-	Return the shape of a hand as a list from longest to shortest, e.g. a 3424 would
-	return (4, 4, 3, 2)
-	"""
-	return sorted(exact_shape(hand), reverse=True)
-
-def major_shape(hand: Hand) -> list[int]:
-	"Return the shape of a hand's major holding from longest to shortest"
-	return sorted((len(hand[Denom.spades]), len(hand[Denom.hearts])), reverse=True)
-
-def minor_shape(hand: Hand) -> list[int]:
-	"""
-	Return the shape of a hand's minor holding from longest to shortest
-	"""
-	return sorted((len(hand[Denom.diamonds]), len(hand[Denom.clubs])), reverse=True)
-
-def is_balanced(hand: Hand) -> bool:
-	"""
-	Returns True if the hand shape is 4333, 4432 or 5332
-	"""
-	s = shape(hand)
-	return s in ([4,3,3,3],[4,4,3,2],[5,3,3,2])
-
-def is_semibalanced(hand: Hand) -> bool:
-	"""
-	Returns True if the hand shape is balanced or 5422
-	"""
-	s = shape(hand)
-	return is_balanced(hand) or s == [5, 4, 2, 2]
-
-def is_minor_semibalanced(hand: Hand) -> bool:
-	"""
-	Returns True if the hand shape is balanced or contains 
-	doubletons in both minors
-	"""
-	return is_balanced(hand) or minor_shape(hand) == [2, 2]
-
-def is_single_suited(hand: Hand, min_length: int = 6, no_side_suit: bool = False) -> bool:
-	"""
-	Returns True if the hand is singled suited
-
-	:param min_length: The minimum number of cards to hold in the suit
-	:param no_side_suit: If True, the hand cannot contain another 4 card suit
-	"""
-	s = shape(hand)
-	if no_side_suit:
-		return s[0] >= min_length and s[1] < 4
-	else:
-		return s[0] >= min_length
-
-def is_two_suited(hand: Hand, strict: bool = False) -> bool:
-	"""
-	Returns True if the hand contains at least 10 cards in two suits.
-
-	:param strict: Hand must be at least 5-5
-	"""
-	s = shape(hand)
-	if strict:
-		return s[0] + s[1] >= 10 and s[1] >= 5
-	else:
-		return s[0] + s[1] >= 10
-
-def is_three_suited(hand: Hand, strict: bool = False) -> bool:
-	"""
-	Returns True if the hand has three suits with at least four cards in them.
-
-	:param strict: Only return true if the hand is 4441
-	"""
-	s = shape(hand)
-	if strict:
-		return s == [4, 4, 4, 1]
-	else:
-		return s[0] >= 4 and s[1] >= 4 and s[2] >= 4
+"""
+Functions for evaluating bridge hands using a variety of different metrics.
+"""
+
+from __future__ import annotations
+
+__all__ = [
+	"standard_hcp_scale", "bergen_hcp_scale", "hcp", "shortage_nofit_dist_scale",
+	"shortage_fit_dist_scale", "length_dist_scale", "mixed_fit_dist_scale",
+	"mixed_nofit_dist_scale", "dist_points", "total_points",
+	"top_honours", "losers", "cccc", "quality", "controls", "rule_of_n",
+	"exact_shape", "shape", "major_shape", "minor_shape", "is_balanced",
+	"is_semibalanced", "is_minor_semibalanced", "is_single_suited",
+	"is_two_suited", "is_three_suited"]
+
+from typing import Union, Optional
+from collections.abc import Iterable
+from endplay.types import Hand, SuitHolding, Card, Rank, AlternateRank, Denom
+
+# Points for each rank in order [A, K, Q, J, ...]
+standard_hcp_scale: list[float] = [4, 3, 2, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+"""Classic HCP scale with A=4, K=3, Q=2, J=1"""
+bergen_hcp_scale: list[float] = [4.5, 3, 1.5, 0.75, 0.25, 0, 0, 0, 0, 0, 0, 0, 0]
+"""Bergen HCP scale with A=4.5, K=3, Q=1.5, J=0.75, T=0.25"""
+
+def hcp(
+	obj: Union[Iterable[Union[Card, Rank, AlternateRank]], Card, Rank, AlternateRank],
+	scale: list[float] = standard_hcp_scale) -> float:
+	"""
+	Return the high card points of a hand or suit holding using a given scale. Two
+	scales are predefined: `standard_hcp_scale` which uses the traditional 4321
+	point scale, and `bergen_hcp_scale` which uses the Bergen scale.
+
+	:param obj: A (possibly iterable of) card or rank type to evaluate
+	:param scale: A list of 13 numbers which assign points to each rank in descending
+		order, e.g. [4,3,2,1,0,...] is used for the standard HCP scale where an ace is
+		worth 4 points, a king 3 etc...
+	"""
+	if len(scale) < 13:
+		scale += [0] * (13 - len(scale))
+	if isinstance(obj, Card):
+		return scale[14 - obj.rank.to_alternate()]
+	elif isinstance(obj, Rank):
+		return scale[14 - obj.to_alternate()]
+	elif isinstance(obj, AlternateRank):
+		return scale[14 - obj]
+	else:
+		return sum(hcp(card, scale) for card in obj)
+
+# Points for each suit length in order [0/void, 1/singleton, 2/doubleton, 3, ...]
+shortage_nofit_dist_scale: list[float] = [3, 2, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+"""Distribution point scale with void=3, singleton=2, doubleton=1"""
+shortage_fit_dist_scale: list[float] = [5, 3, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+"""Distribution point scale when a trump fit is found with void=5, singleton=3, doubleton=1"""
+length_dist_scale: list[float] = [0, 0, 0, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
+"""Distribution point scale which awards a point for each extra card in a suit over 4"""
+mixed_nofit_dist_scale: list[float] = [3, 2, 1, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
+"""Combined scale using `shortage_nofit_dist_scale` and `length_dist_scale`"""
+mixed_fit_dist_scale: list[float] = [5, 3, 1, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
+"""Combined scale using `shortage_fit_dist_scale` and `length_dist_scale`"""
+
+def dist_points(obj: Union[Hand, SuitHolding], scale: list[float] = shortage_nofit_dist_scale, exclude: Iterable[Denom] = []) -> float:
+	"""
+	Return the extra points for distribution for a hand or suit holding using the given scale.
+	Five scales are predefined:
+
+	* `shortage_nofit_dist_scale`: Standard evaluation of shortage points if no trump fit is agreed,
+	  void=3, singleton=2, doubleton=1
+
+	* `shortage_fit_dist_scale`: Standard evaluation of shortage points if trump fit is agreed,
+	  void=5, singleton=3, doubleton=1
+
+	* `length_dist_scale`: Standard evaluation of length points, one point for each extra card in a
+	  suit with more than four cards in it, i.e. 5 cards=1, 6 cards=2, etc...
+
+	:param obj: Hand or suit holding to evaluate
+	:param scale: A list of 14 numbers which assign points to each suit length in ascending order,
+		e.g. [3,2,1,0,...] is used for the standard shortage points where void=3, singleton=2 etc...
+	:param exclude: List of suits to be excluded from distribution calculations if a `Hand` object
+		is passed, in order to e.g. exclude the trump suit from the calculation
+	"""
+	if len(scale) < 14:
+		scale += [0] * (14 - len(scale))
+	if isinstance(obj, SuitHolding):
+		return scale[len(obj)]
+	return sum(dist_points(obj[suit], scale) if suit not in exclude else 0 for suit in Denom.suits())
+
+def total_points(
+	obj: Union[Hand, SuitHolding],
+	hcp_scale: list[float] = standard_hcp_scale,
+	dist_scale: list[float] = shortage_nofit_dist_scale,
+	trump: Optional[Denom] = None,
+	protect_honours: bool = False):
+	"""
+	Return the sum of high card points and distribution points in a hand.
+
+	:param obj: Hand or suit holding to evaluate
+	:param hcp_scale: The HCP scale to use, as for the `hcp` function
+	:param dist_scale: The distribution points scale, as for the `dist_scale` function
+	:param trump: If set then distribution points for the given suit are excluded from
+		the calculation
+	:param protect_honours: If `True`, then honours must be protected for their HCP
+		to be included, i.e. king singleton, queen doubleton etc do not contribute to
+		total points
+	"""
+	if isinstance(obj, SuitHolding):
+		points = dist_points(obj, dist_scale, [trump] if trump is not None else [])
+		if protect_honours:
+			obj = obj.copy()
+			ncards = len(obj)
+			if ncards < 4: obj.remove(Rank.RJ)
+			if ncards < 3: obj.remove(Rank.RQ)
+			if ncards < 2: obj.remove(Rank.RK)
+		return hcp(obj, hcp_scale) + points
+	else:
+		return sum(total_points(obj[suit], hcp_scale, dist_scale, trump, protect_honours) for suit in Denom.suits())
+
+def top_honours(hand: Union[Hand, SuitHolding], lowest_honour: Union[Rank, int] = Rank.RJ) -> int:
+	"""
+	Return the number of top honors in a suit
+
+	:param suit: The suit holding to evaluate
+	:param lowest_honour: The lowest rank to be treated as an honour, or an
+		integer for how many top cards are honours
+	"""
+	if not isinstance(lowest_honour, Rank):
+		lowest_honour = AlternateRank(15 - lowest_honour).to_standard()
+	if isinstance(hand, SuitHolding):
+		return sum(1 for rank in hand if rank >= lowest_honour)
+	else:
+		return sum(1 for card in hand if card.rank >= lowest_honour)
+
+def losers(hand: Union[Hand, SuitHolding]) -> int:
+	"""
+	Returns the number of losers in a hand. The number of losers in each
+	suit is calculated as: (a) 3 or more cards in a suit: 3 - 1 per AKQ
+	(b) Doubleton: AK=0, Ax/Kx=1, else 2 (c) Singleton: A=0, else 1 (d) Void: 0
+	"""
+	if isinstance(hand, SuitHolding):
+		a, k, q = Rank.RA in hand, Rank.RK in hand, Rank.RQ in hand
+		if len(hand) == 0: return 0
+		if len(hand) == 1: return 1 - a
+		if len(hand) == 2: return 2 - a - k
+		return 3 - a - k - q
+	else:
+		return sum(losers(hand[suit]) for suit in Denom.suits())
+
+def cccc(hand: Union[Hand, SuitHolding]) -> float:
+	"""
+	Uses the Kaplan four cs algorithm from the October 1982 issue of Bridge world
+	magazine. This implementation is based on the interpretation of the algorithm
+	described on http://www.rpbridge.net/8j19.htm
+	"""
+	if isinstance(hand, Hand):
+		return sum(cccc(hand[suit]) for suit in Denom.suits())
+	l = len(hand)
+	score = 0
+	# 1-5: Count point values A=4,K=3,Q=2,J=1,T=0.5
+	if Rank.RA in hand: score += 4
+	if Rank.RK in hand: score += 3
+	if Rank.RQ in hand: score += 2
+	if Rank.RJ in hand: score += 1
+	if Rank.RT in hand: score += 0.5
+	# 6-7: if between 2-6 cards, count points for supported T and 9
+	if l >= 2 and l <= 6:
+		if (Rank.RT in hand) and ((Rank.RJ in hand) or top_honours(hand, 4) >= 2):
+			score += 0.5
+		if (Rank.R9 in hand) and ((Rank.R8 in hand or Rank.RT in hand) or top_honours(hand, 5) == 2):
+			score += 0.5
+	# 8: if between 4-6 cards, count 9 without any touching cards and exactly three higher honours
+	if l >= 4 and l <= 6:
+		if (Rank.R9 in hand) and not (Rank.R8 in hand and Rank.RT in hand) and top_honours(hand, 4) == 3:
+			score += 0.5
+	# 9: 7+ cards missing queen or jack (or both)
+	if l >= 7 and (Rank.RQ not in hand or Rank.RJ not in hand):
+		score += 1
+	# 10: 8+ cards missing queen
+	if l >= 8 and Rank.RQ not in hand:
+		score += 1
+	# 11: 9+ cards missing queen and jack
+	if l >= 9 and (Rank.RQ not in hand and Rank.RJ not in hand):
+		score += 1
+	# 12: Multiply current total by suit length, divide by 10, then continue
+	score *= l / 10
+	# 13: Add 3 for an ace
+	if Rank.RA in hand:
+		score += 3
+	# 14-15: Add 2 for guarded king and 0.5 for king singleton
+	if Rank.RK in hand:
+		if l > 1: score += 2
+		else: score += 0.5
+	# 16-19: Add values for queen
+	if Rank.RQ in hand:
+		if l >= 3:
+			# 16-17: 3+ cards, +1 if has higher honour else +0.75
+			if Rank.RK in hand or Rank.RA in hand:
+				score += 1
+			else:
+				score += 0.75
+		elif l == 2:
+			# 18-19: doubleton, +0.5 if has higher honour else +0.25
+			if Rank.RK in hand or Rank.RA in hand:
+				score += 0.5
+			else:
+				score += 0.25
+	# 20-21: Jack with two higher honours=0.5, one higher honour=0.25
+	if Rank.RJ in hand:
+		hh = top_honours(hand, 3)
+		if hh == 2:
+			score += 0.5
+		elif hh == 1:
+			score += 0.25
+	# 22-23: Ten with two higher honours=0.25, T9 with one higher honour=0.25
+	if Rank.RT in hand:
+		hh = top_honours(hand, 4)
+		if hh == 2:
+			score += 0.25
+		if Rank.R9 in hand and hh == 1:
+			score += 0.25
+	# 24-26: void=3, singleton=2, doubleton=1
+	if l == 0:
+		score += 3
+	elif l == 1:
+		score += 2
+	elif l == 2:
+		score += 1
+	return score
+
+def quality(hand: SuitHolding) -> float:
+	"Uses the quality algorithm (from the October 1982 issue of Bridge World magazine)"
+	raise NotImplementedError
+
+def controls(hand: Union[Iterable, Card, Rank]) -> int:
+	"Return the number of controls in a sequence, using A=2 and K=1"
+	if isinstance(hand, Rank):
+		if hand == Rank.RA: return 2
+		elif hand == Rank.RK: return 1
+		else: return 0
+	elif isinstance(hand, Card):
+		return controls(hand.rank)
+	else:
+		return sum(controls(card) for card in hand)
+
+def rule_of_n(hand: Hand) -> float:
+	"Returns the hcp of the hand added to the length of the two longest suits"
+	s = shape(hand)
+	return hcp(hand) + s[0] + s[1]
+
+def exact_shape(hand: Hand) -> list[int]:
+	"Return the shape of a hand as a list starting from spades, e.g. (5, 2, 3, 3)"
+	return [len(hand[suit]) for suit in Denom.suits()]
+
+def shape(hand: Hand) -> list[int]:
+	"""
+	Return the shape of a hand as a list from longest to shortest, e.g. a 3424 would
+	return (4, 4, 3, 2)
+	"""
+	return sorted(exact_shape(hand), reverse=True)
+
+def major_shape(hand: Hand) -> list[int]:
+	"Return the shape of a hand's major holding from longest to shortest"
+	return sorted((len(hand[Denom.spades]), len(hand[Denom.hearts])), reverse=True)
+
+def minor_shape(hand: Hand) -> list[int]:
+	"""
+	Return the shape of a hand's minor holding from longest to shortest
+	"""
+	return sorted((len(hand[Denom.diamonds]), len(hand[Denom.clubs])), reverse=True)
+
+def is_balanced(hand: Hand) -> bool:
+	"""
+	Returns True if the hand shape is 4333, 4432 or 5332
+	"""
+	s = shape(hand)
+	return s in ([4,3,3,3],[4,4,3,2],[5,3,3,2])
+
+def is_semibalanced(hand: Hand) -> bool:
+	"""
+	Returns True if the hand shape is balanced or 5422
+	"""
+	s = shape(hand)
+	return is_balanced(hand) or s == [5, 4, 2, 2]
+
+def is_minor_semibalanced(hand: Hand) -> bool:
+	"""
+	Returns True if the hand shape is balanced or contains
+	doubletons in both minors
+	"""
+	return is_balanced(hand) or minor_shape(hand) == [2, 2]
+
+def is_single_suited(hand: Hand, min_length: int = 6, no_side_suit: bool = False) -> bool:
+	"""
+	Returns True if the hand is singled suited
+
+	:param min_length: The minimum number of cards to hold in the suit
+	:param no_side_suit: If True, the hand cannot contain another 4 card suit
+	"""
+	s = shape(hand)
+	if no_side_suit:
+		return s[0] >= min_length and s[1] < 4
+	else:
+		return s[0] >= min_length
+
+def is_two_suited(hand: Hand, strict: bool = False) -> bool:
+	"""
+	Returns True if the hand contains at least 10 cards in two suits.
+
+	:param strict: Hand must be at least 5-5
+	"""
+	s = shape(hand)
+	if strict:
+		return s[0] + s[1] >= 10 and s[1] >= 5
+	else:
+		return s[0] + s[1] >= 10
+
+def is_three_suited(hand: Hand, strict: bool = False) -> bool:
+	"""
+	Returns True if the hand has three suits with at least four cards in them.
+
+	:param strict: Only return true if the hand is 4441
+	"""
+	s = shape(hand)
+	if strict:
+		return s == [4, 4, 4, 1]
+	else:
+		return s[0] >= 4 and s[1] >= 4 and s[2] >= 4
```

### Comparing `endplay-0.4.8b0/src/endplay/experimental/playdetect.py` & `endplay-0.4.9b0/src/endplay/experimental/playdetect.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/interact/__main__.py` & `endplay-0.4.9b0/src/endplay/interact/__main__.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/interact/frontends/cmd.py` & `endplay-0.4.9b0/src/endplay/interact/frontends/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,37 +121,40 @@
 		
 	def do_redeal(self, arg):
 		"""
 		Redeal the hand to the given PBN string (or an empty string for a blank deal)
 		Example 1: redeal
 		Example 2: redeal N:95..A. 8.5.Q. .QT5.. Q..T4.
 		"""
+		self.deal.reset()
 		if arg:
 			try:
-				self.deal.reset(arg)
+				new_deal = Deal(arg)
+				for player, hand in new_deal:
+					self.deal[player] = hand
 			except RuntimeError:
 				print(f"Invalid PBN string: `{arg}`")
-		else:
-			self.deal = Deal()
 		self.needs_printing = True
 
 	def do_shuffle(self, arg):
 		"""
 		Generate a random deal satisfying the given constraints.
 		Example 1: shuffle
 		Example 2: shuffle hcp(north) > hcp(south)
 		"""
 		if arg:
 			try:
 				new_deal = generate_deal(arg)
 			except RuntimeError:
-				print("Could not generate deal satisfying this constraint")
+				raise RuntimeError("Could not generate deal satisfying this constraint")
 		else:
 			new_deal = generate_deal()
-		self.deal.reset(str(new_deal))
+		self.deal.reset()
+		for player, hand in new_deal:
+			self.deal[player] = hand
 		self.needs_printing = True
 
 	def do_first(self, arg):
 		"""
 		If no argument is provided, display the position of the player to play the first card to
 		the current trick. If a position is given, set that seat to be on lead
 		Example 1: first
```

### Comparing `endplay-0.4.8b0/src/endplay/interact/frontends/curses.py` & `endplay-0.4.9b0/src/endplay/interact/frontends/curses.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/interact/interactivedeal.py` & `endplay-0.4.9b0/src/endplay/interact/interactivedeal.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/parsers/dealer.py` & `endplay-0.4.9b0/src/endplay/parsers/dealer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿"""
+"""
 Parser for Dealer scripts
 """
 
 __all__ = [ "DealerParser", "ParseException" ]
 
 from typing import TextIO
 from endplay.types import Player, Vul, Hand, Contract, Denom, Deal
```

### Comparing `endplay-0.4.8b0/src/endplay/parsers/json.py` & `endplay-0.4.9b0/src/endplay/parsers/json.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-"Parser for endplay formatted JSON files"
-
-from __future__ import annotations
-
-__all__ = ["JSONEncoder", "JSONDecoder", "dump", "dumps", "load", "loads"]
-
-import json as _json
-from enum import IntEnum
-from collections.abc import Collection, Mapping
-from endplay.types import ContractBid, PenaltyBid, Denom, Penalty, \
-	Card, Rank, Contract, Player, Deal, Vul, Board, Hand, SuitHolding
-
-def _check_keys(keys: set, mandatory: set, optional: set = set()):
-	if not mandatory.issubset(keys):
-		return False
-	return (keys - mandatory).issubset(optional)
-
-def _object_hook(d: dict):
-	keys = set(d.keys())
-	if _check_keys(keys, 
-		set(["level", "denom"]), 
-		set(["alertable", "announcement"])):
-		return ContractBid(
-			d.get("level"), Denom.find(d.get("denom")), 
-			d.get("alertable", False), d.get("announcement"))
-	elif _check_keys(keys, 
-		set(["penalty"]), 
-		set(["alertable", "announcement"])):
-		return PenaltyBid(
-			Penalty.find(d.get("penalty")), 
-			d.get("alertable", False), d.get("announcement"))
-	elif _check_keys(keys, set(["suit", "rank"])):
-		return Card(
-			suit=Denom.find(d.get("suit")), 
-			rank=Rank.find(d.get("rank")))
-	elif _check_keys(keys, 
-		set(["level", "denom", "declarer"]), 
-		set(["penalty", "result"])):
-		return Contract(
-			level=d.get("level"),
-			denom=Denom.find(d.get("denom")),
-			declarer=Player.find(d.get("declarer")),
-			penalty=Penalty.find(d.get("penalty", "pass")),
-			result=d.get("result", 0))
-	elif _check_keys(keys,
-		set(["north", "south", "east", "west"]),
-		set(["first", "trump", "curtrick"])):
-		deal = Deal(
-			first=Player.find(d.get("first", "north")),
-			trump=Denom.find(d.get("trump", "nt")))
-		for hand in ["north", "south", "east", "west"]:
-			for card in d.get(hand, []):
-				deal[Player.find(hand)].add(card)
-		for card in d.get("curtrick", []):
-			deal.play(card)
-		return deal
-	elif _check_keys(keys,
-		set(["deal", "auction", "play", "board_num"]),
-		set(["vul", "dealer", "contract", "claimed", "info"])):
-		board = Board(
-			deal=d.get("deal"),
-			auction=d.get("auction"),
-			play=d.get("play"),
-			board_num=d.get("board_num"),)
-		if "vul" in d:
-			board.vul = Vul.find(d.get("vul"))
-		if "dealer" in d:
-			board.dealer = Player.find(d.get("dealer"))
-		if "contract" in d:
-			board.contract = d.get("contract")
-		if "claimed" in d:
-			board.claimed = d.get("claimed")
-		if "info" in d:
-			for key, val in d.get("info").items():
-				board.info[key] = val
-		return board
-	else:
-		return d 
-
-class JSONDecoder(_json.JSONDecoder):
-	"""
-	Class providing functionality for reading the JSON file format
-	"""
-	def __init__(self, 
-		*, object_hook=None, parse_float=None, parse_int=None,
-		parse_constant=None, strict=True, object_pairs_hook=None):
-		if object_hook is not None or object_pairs_hook is not None:
-			raise RuntimeError("object_hook and object_pairs_hook currently not supported")
-		super().__init__(
-			object_hook = _object_hook,
-			parse_float = parse_float,
-			parse_int = parse_int,
-			parse_constant = parse_constant,
-			strict = strict
-		)
-
-def _preprocess_intenum(o):
-    if isinstance(o, IntEnum):
-        return {'__class__': o.__class__.__name__,
-                '__value__': (o.value,)}
-    if isinstance(o, dict):
-        return {k: _preprocess_intenum(v) for k, v in o.iteritems()}
-    if isinstance(o, (list, tuple)):
-        return [_preprocess_intenum(v) for v in o]
-    return o
-
-class JSONEncoder(_json.JSONEncoder):
-	"""
-	Class providing functionality for writing to the JSON file format
-	"""
-	def iterencode(self, o, _one_shot=False):
-		return super().iterencode(_preprocess_intenum(o), _one_shot)
-
-	def default(self, o):
-		if isinstance(o, ContractBid):
-			res = {
-				"level": o.level,
-				"denom": o.denom.name,
-				"alertable": o.alertable,
-			}
-			if o.announcement:
-				res["announcement"] = o.announcement
-			return res
-		elif isinstance(o, PenaltyBid):
-			res = {
-				"penalty": "pass" if o.penalty is Penalty.passed else o.penalty.name[:-1],
-				"alertable": o.alertable
-			}
-			if o.announcement:
-				res["announcement"] = o.announcement
-			return res
-		elif isinstance(o, Board):
-			res = {
-				"deal": o.deal,
-				"auction": o.auction,
-				"play": o.play,
-				"board_num": o.board_num,
-				"info": dict(o.info)
-			}
-			if o.vul is not None:
-				res["vul"] = o.vul.name
-			if o.dealer is not None:
-				res["dealer"] = o.dealer.name
-			if o.contract is not None:
-				res["contract"] = o.contract
-			if o.claimed is not None:
-				res["claimed"] = o.claimed
-			return res
-		elif isinstance(o, Card):
-			return {
-				"suit": o.suit.name,
-				"rank": o.rank.name[1]
-			}
-		elif isinstance(o, Contract):
-			return {
-				"level": o.level,
-				"denom": o.denom.name,
-				"declarer": o.declarer.name,
-				"penalty": o.penalty.abbr,
-				"result": o.result
-			}
-		elif isinstance(o, Deal):
-			return {
-				"north": list(o.north),
-				"east": list(o.east),
-				"south": list(o.south),
-				"west": list(o.west),
-				"first": o.first.name,
-				"trump": o.trump.name,
-				"curtrick": list(o.curtrick)
-			}
-		elif isinstance(o, Hand):
-			return list(o)
-		elif isinstance(o, SuitHolding):
-			return [r.name for r in o] 
-		else:
-			return super().default(self, o)
-
-def dump(obj, fp, 
-	*, skipkeys=False, ensure_ascii=True, check_circular=True, 
-	allow_nan=True, indent=None, separators=None, default=None, 
-	sort_keys=False, **kw):
-	return _json.dump(obj, fp,
-		skipkeys=skipkeys,
-		ensure_ascii=ensure_ascii,
-		check_circular=check_circular,
-		allow_nan=allow_nan,
-		cls=JSONEncoder,
-		indent=indent,
-		separators=separators,
-		default=default,
-		sort_keys=sort_keys,
-		**kw)
-
-def dumps(obj, 
-	*, skipkeys=False, ensure_ascii=True, check_circular=True, 
-	allow_nan=True, indent=None, separators=None, default=None, 
-	sort_keys=False, **kw):
-	return _json.dumps(obj,
-		skipkeys=skipkeys,
-		ensure_ascii=ensure_ascii,
-		check_circular=check_circular,
-		allow_nan=allow_nan,
-		cls=JSONEncoder,
-		indent=indent,
-		separators=separators,
-		default=default,
-		sort_keys=sort_keys,
-		**kw)
-
-def load(fp, *, 
-	object_hook=None, parse_float=None, parse_int=None, 
-	parse_constant=None, object_pairs_hook=None, **kw):
-	return _json.load(fp,
-		cls=JSONDecoder,
-		object_hook=object_hook,
-		parse_float=parse_float,
-		parse_int=parse_int,
-		parse_constant=parse_constant,
-		object_pairs_hook=object_pairs_hook,
-		**kw
-	)
-
-def loads(s, *, 
-	object_hook=None, parse_float=None, parse_int=None, 
-	parse_constant=None, object_pairs_hook=None, **kw):
-	return _json.loads(s, 
-		cls=JSONDecoder,
-		object_hook=object_hook,
-		parse_float=parse_float,
-		parse_int=parse_int,
-		parse_constant=parse_constant,
-		object_pairs_hook=object_pairs_hook,
+"Parser for endplay formatted JSON files"
+
+from __future__ import annotations
+
+__all__ = ["JSONEncoder", "JSONDecoder", "dump", "dumps", "load", "loads"]
+
+import json as _json
+from enum import IntEnum
+from collections.abc import Collection, Mapping
+from endplay.types import ContractBid, PenaltyBid, Denom, Penalty, \
+	Card, Rank, Contract, Player, Deal, Vul, Board, Hand, SuitHolding
+
+def _check_keys(keys: set, mandatory: set, optional: set = set()):
+	if not mandatory.issubset(keys):
+		return False
+	return (keys - mandatory).issubset(optional)
+
+def _object_hook(d: dict):
+	keys = set(d.keys())
+	if _check_keys(keys, 
+		set(["level", "denom"]), 
+		set(["alertable", "announcement"])):
+		return ContractBid(
+			d.get("level"), Denom.find(d.get("denom")), 
+			d.get("alertable", False), d.get("announcement"))
+	elif _check_keys(keys, 
+		set(["penalty"]), 
+		set(["alertable", "announcement"])):
+		return PenaltyBid(
+			Penalty.find(d.get("penalty")), 
+			d.get("alertable", False), d.get("announcement"))
+	elif _check_keys(keys, set(["suit", "rank"])):
+		return Card(
+			suit=Denom.find(d.get("suit")), 
+			rank=Rank.find(d.get("rank")))
+	elif _check_keys(keys, 
+		set(["level", "denom", "declarer"]), 
+		set(["penalty", "result"])):
+		return Contract(
+			level=d.get("level"),
+			denom=Denom.find(d.get("denom")),
+			declarer=Player.find(d.get("declarer")),
+			penalty=Penalty.find(d.get("penalty", "pass")),
+			result=d.get("result", 0))
+	elif _check_keys(keys,
+		set(["north", "south", "east", "west"]),
+		set(["first", "trump", "curtrick"])):
+		deal = Deal(
+			first=Player.find(d.get("first", "north")),
+			trump=Denom.find(d.get("trump", "nt")))
+		for hand in ["north", "south", "east", "west"]:
+			for card in d.get(hand, []):
+				deal[Player.find(hand)].add(card)
+		for card in d.get("curtrick", []):
+			deal.play(card)
+		return deal
+	elif _check_keys(keys,
+		set(["deal", "auction", "play", "board_num"]),
+		set(["vul", "dealer", "contract", "claimed", "info"])):
+		board = Board(
+			deal=d.get("deal"),
+			auction=d.get("auction"),
+			play=d.get("play"),
+			board_num=d.get("board_num"),)
+		if "vul" in d:
+			board.vul = Vul.find(d.get("vul"))
+		if "dealer" in d:
+			board.dealer = Player.find(d.get("dealer"))
+		if "contract" in d:
+			board.contract = d.get("contract")
+		if "claimed" in d:
+			board.claimed = d.get("claimed")
+		if "info" in d:
+			for key, val in d.get("info").items():
+				board.info[key] = val
+		return board
+	else:
+		return d 
+
+class JSONDecoder(_json.JSONDecoder):
+	"""
+	Class providing functionality for reading the JSON file format
+	"""
+	def __init__(self, 
+		*, object_hook=None, parse_float=None, parse_int=None,
+		parse_constant=None, strict=True, object_pairs_hook=None):
+		if object_hook is not None or object_pairs_hook is not None:
+			raise RuntimeError("object_hook and object_pairs_hook currently not supported")
+		super().__init__(
+			object_hook = _object_hook,
+			parse_float = parse_float,
+			parse_int = parse_int,
+			parse_constant = parse_constant,
+			strict = strict
+		)
+
+def _preprocess_intenum(o):
+    if isinstance(o, IntEnum):
+        return {'__class__': o.__class__.__name__,
+                '__value__': (o.value,)}
+    if isinstance(o, dict):
+        return {k: _preprocess_intenum(v) for k, v in o.iteritems()}
+    if isinstance(o, (list, tuple)):
+        return [_preprocess_intenum(v) for v in o]
+    return o
+
+class JSONEncoder(_json.JSONEncoder):
+	"""
+	Class providing functionality for writing to the JSON file format
+	"""
+	def iterencode(self, o, _one_shot=False):
+		return super().iterencode(_preprocess_intenum(o), _one_shot)
+
+	def default(self, o):
+		if isinstance(o, ContractBid):
+			res = {
+				"level": o.level,
+				"denom": o.denom.name,
+				"alertable": o.alertable,
+			}
+			if o.announcement:
+				res["announcement"] = o.announcement
+			return res
+		elif isinstance(o, PenaltyBid):
+			res = {
+				"penalty": "pass" if o.penalty is Penalty.passed else o.penalty.name[:-1],
+				"alertable": o.alertable
+			}
+			if o.announcement:
+				res["announcement"] = o.announcement
+			return res
+		elif isinstance(o, Board):
+			res = {
+				"deal": o.deal,
+				"auction": o.auction,
+				"play": o.play,
+				"board_num": o.board_num,
+				"info": dict(o.info)
+			}
+			if o.vul is not None:
+				res["vul"] = o.vul.name
+			if o.dealer is not None:
+				res["dealer"] = o.dealer.name
+			if o.contract is not None:
+				res["contract"] = o.contract
+			if o.claimed is not None:
+				res["claimed"] = o.claimed
+			return res
+		elif isinstance(o, Card):
+			return {
+				"suit": o.suit.name,
+				"rank": o.rank.name[1]
+			}
+		elif isinstance(o, Contract):
+			return {
+				"level": o.level,
+				"denom": o.denom.name,
+				"declarer": o.declarer.name,
+				"penalty": o.penalty.abbr,
+				"result": o.result
+			}
+		elif isinstance(o, Deal):
+			return {
+				"north": list(o.north),
+				"east": list(o.east),
+				"south": list(o.south),
+				"west": list(o.west),
+				"first": o.first.name,
+				"trump": o.trump.name,
+				"curtrick": list(o.curtrick)
+			}
+		elif isinstance(o, Hand):
+			return list(o)
+		elif isinstance(o, SuitHolding):
+			return [r.name for r in o] 
+		else:
+			return super().default(self, o)
+
+def dump(obj, fp, 
+	*, skipkeys=False, ensure_ascii=True, check_circular=True, 
+	allow_nan=True, indent=None, separators=None, default=None, 
+	sort_keys=False, **kw):
+	return _json.dump(obj, fp,
+		skipkeys=skipkeys,
+		ensure_ascii=ensure_ascii,
+		check_circular=check_circular,
+		allow_nan=allow_nan,
+		cls=JSONEncoder,
+		indent=indent,
+		separators=separators,
+		default=default,
+		sort_keys=sort_keys,
+		**kw)
+
+def dumps(obj, 
+	*, skipkeys=False, ensure_ascii=True, check_circular=True, 
+	allow_nan=True, indent=None, separators=None, default=None, 
+	sort_keys=False, **kw):
+	return _json.dumps(obj,
+		skipkeys=skipkeys,
+		ensure_ascii=ensure_ascii,
+		check_circular=check_circular,
+		allow_nan=allow_nan,
+		cls=JSONEncoder,
+		indent=indent,
+		separators=separators,
+		default=default,
+		sort_keys=sort_keys,
+		**kw)
+
+def load(fp, *, 
+	object_hook=None, parse_float=None, parse_int=None, 
+	parse_constant=None, object_pairs_hook=None, **kw):
+	return _json.load(fp,
+		cls=JSONDecoder,
+		object_hook=object_hook,
+		parse_float=parse_float,
+		parse_int=parse_int,
+		parse_constant=parse_constant,
+		object_pairs_hook=object_pairs_hook,
+		**kw
+	)
+
+def loads(s, *, 
+	object_hook=None, parse_float=None, parse_int=None, 
+	parse_constant=None, object_pairs_hook=None, **kw):
+	return _json.loads(s, 
+		cls=JSONDecoder,
+		object_hook=object_hook,
+		parse_float=parse_float,
+		parse_int=parse_int,
+		parse_constant=parse_constant,
+		object_pairs_hook=object_pairs_hook,
 		**kw)
```

### Comparing `endplay-0.4.8b0/src/endplay/parsers/lin.py` & `endplay-0.4.9b0/src/endplay/parsers/lin.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/parsers/pbn.py` & `endplay-0.4.9b0/src/endplay/parsers/pbn.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/stats/__init__.py` & `endplay-0.4.9b0/src/endplay/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/__init__.py` & `endplay-0.4.9b0/src/endplay/types/__init__.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/bid.py` & `endplay-0.4.9b0/src/endplay/types/bid.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/board.py` & `endplay-0.4.9b0/src/endplay/types/board.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/card.py` & `endplay-0.4.9b0/src/endplay/types/card.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/contract.py` & `endplay-0.4.9b0/src/endplay/types/contract.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/deal.py` & `endplay-0.4.9b0/src/endplay/types/deal.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/denom.py` & `endplay-0.4.9b0/src/endplay/types/denom.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/hand.py` & `endplay-0.4.9b0/src/endplay/types/hand.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/penalty.py` & `endplay-0.4.9b0/src/endplay/types/penalty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿__all__ = ["Penalty"]
+__all__ = ["Penalty"]
 
 from enum import IntEnum
 
 class Penalty(IntEnum):
 	"Encodes a penalty"
 	passed = 1
 	doubled = 2
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `endplay-0.4.8b0/src/endplay/types/player.py` & `endplay-0.4.9b0/src/endplay/types/player.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/suitholding.py` & `endplay-0.4.9b0/src/endplay/types/suitholding.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/types/vul.py` & `endplay-0.4.9b0/src/endplay/types/vul.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/utils/escape.py` & `endplay-0.4.9b0/src/endplay/utils/escape.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/utils/io.py` & `endplay-0.4.9b0/src/endplay/utils/io.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay/utils/play.py` & `endplay-0.4.9b0/src/endplay/utils/play.py`

 * *Files identical despite different names*

### Comparing `endplay-0.4.8b0/src/endplay.egg-info/PKG-INFO` & `endplay-0.4.9b0/src/endplay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endplay
-Version: 0.4.8b0
+Version: 0.4.9b0
 Summary: A suite of tools for generation and analysis of bridge deals
 Home-page: https://github.com/dominicprice/endplay
 Author: Dominic Price
 Author-email: dominicprice@outlook.com
 Project-URL: Documentation, https://endplay.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/dominicprice/endplay/issues
 Keywords: bridge,cards,games,double dummy,dds,analysis,stats,deal,dealer
```

### Comparing `endplay-0.4.8b0/src/endplay.egg-info/SOURCES.txt` & `endplay-0.4.9b0/src/endplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

