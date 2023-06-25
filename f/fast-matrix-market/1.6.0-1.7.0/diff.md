# Comparing `tmp/fast-matrix-market-1.6.0.tar.gz` & `tmp/fast-matrix-market-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-matrix-market-1.6.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "fast-matrix-market-1.7.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `fast-matrix-market-1.6.0.tar` & `fast-matrix-market-1.7.0.tar`

### file list

```diff
@@ -1,102 +1,104 @@
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/CMakeLists.txt
--rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/LICENSE.txt
--rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/README.md
--rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/benchmark/bench_fmm.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/benchmark/requirements.txt
--rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/benchmark/run.sh
--rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/CMakeLists.txt
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/Blaze.cmake
--rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/Dragonbox.cmake
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/Eigen.cmake
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/GoogleBenchmark.cmake
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/GoogleTest.cmake
--rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/GraphBLAS.cmake
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/fast_float.cmake
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/from_chars_tests.cmake
--rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/cmake/to_chars_tests.cmake
--rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/README.md
--rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
--rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
--rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
--rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
--rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
--rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
--rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
--rw-r--r--   0        0        0   115829 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
--rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost
--rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/common.h
--rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
--rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
--rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c
--rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
--rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
--rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
--rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
--rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
--rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
--rw-r--r--   0        0        0    11093 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.c
--rw-r--r--   0        0        0    34192 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.h
--rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h
--rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h
--rw-r--r--   0        0        0     8362 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/s2d.c
--rw-r--r--   0        0        0     8591 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/s2f.c
--rw-r--r--   0        0        0     4008 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
--rw-r--r--   0        0        0    15527 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
--rw-r--r--   0        0        0     3193 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
--rw-r--r--   0        0        0     7193 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
--rw-r--r--   0        0        0    57595 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
--rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp
--rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
--rw-r--r--   0        0        0     4207 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
--rw-r--r--   0        0        0     3188 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp
--rw-r--r--   0        0        0     5251 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
--rw-r--r--   0        0        0    21182 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
--rw-r--r--   0        0        0    14746 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp
--rw-r--r--   0        0        0    10104 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/header.hpp
--rw-r--r--   0        0        0     9312 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
--rw-r--r--   0        0        0    18575 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp
--rw-r--r--   0        0        0     5539 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
--rw-r--r--   0        0        0    15554 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp
--rw-r--r--   0        0        0     5018 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/types.hpp
--rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp
--rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/pyproject.toml
--rw-r--r--   0        0        0    15990 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/src/fast_matrix_market/__init__.py
--rw-r--r--   0        0        0    23684 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/src/fast_matrix_market/core.cpp
--rw-r--r--   0        0        0    19485 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/src/fast_matrix_market/pystreambuf.h
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/eye3.mtx
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longcomplex_array.mtx
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longcomplex_coordinate.mtx
--rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longdouble_array.mtx
--rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/long_double/longdouble_coordinate.mtx
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_array_complex_general.mtx
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_array_integer_general.mtx
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_array_real_general.mtx
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_complex_general.mtx
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_complex_hermitian.mtx
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_integer_general.mtx
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_pattern_general.mtx
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_general.mtx
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_general.mtx.bz2
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_general.mtx.gz
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/matrix_coordinate_real_symmetric.mtx
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/misc/windows_newlines.mtx
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/scipy_crashes/vector_array_real_general.mtx
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
--rw-r--r--   0        0        0     1810 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_array.py
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_basic.py
--rw-r--r--   0        0        0     3235 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_coo.py
--rw-r--r--   0        0        0     3518 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_header.py
--rw-r--r--   0        0        0    13136 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/tests/test_scipy.py
--rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/testsuite_scipy/test_scipy_suite.py
--rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1460 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/README.md
+-rw-r--r--   0        0        0     8422 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/benchmark/bench_fmm.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/benchmark/requirements.txt
+-rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/benchmark/run.sh
+-rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/CMakeLists.txt
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/Blaze.cmake
+-rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/Dragonbox.cmake
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/Eigen.cmake
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/GoogleBenchmark.cmake
+-rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/GoogleTest.cmake
+-rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/GraphBLAS.cmake
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/fast_float.cmake
+-rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/from_chars_tests.cmake
+-rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/cmake/to_chars_tests.cmake
+-rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/README.md
+-rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
+-rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
+-rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
+-rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
+-rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
+-rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
+-rw-r--r--   0        0        0   115829 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
+-rw-r--r--   0        0        0      867 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost
+-rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/common.h
+-rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
+-rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
+-rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c
+-rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
+-rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
+-rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
+-rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
+-rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
+-rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
+-rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h
+-rw-r--r--   0        0        0     4017 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
+-rw-r--r--   0        0        0    15563 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
+-rw-r--r--   0        0        0     2967 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
+-rw-r--r--   0        0        0     7211 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
+-rw-r--r--   0        0        0    57614 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
+-rw-r--r--   0        0        0     4562 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp
+-rw-r--r--   0        0        0     4344 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
+-rw-r--r--   0        0        0     5854 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
+-rw-r--r--   0        0        0     3424 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp
+-rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
+-rw-r--r--   0        0        0    21988 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
+-rw-r--r--   0        0        0    14748 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp
+-rw-r--r--   0        0        0    10484 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/header.hpp
+-rw-r--r--   0        0        0     9566 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
+-rw-r--r--   0        0        0    22808 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp
+-rw-r--r--   0        0        0     7373 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
+-rw-r--r--   0        0        0    15554 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp
+-rw-r--r--   0        0        0     5142 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/types.hpp
+-rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp
+-rw-r--r--   0        0        0     2746 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0    17100 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/__init__.py
+-rw-r--r--   0        0        0     9584 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core.cpp
+-rw-r--r--   0        0        0     9435 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core.hpp
+-rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_read_array.cpp
+-rw-r--r--   0        0        0     2599 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_read_coo.cpp
+-rw-r--r--   0        0        0     1813 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_array.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_coo_32.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_coo_64.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_csc_32.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/_core_write_csc_64.cpp
+-rw-r--r--   0        0        0    20198 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/src/fast_matrix_market/pystreambuf.h
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/eye3.mtx
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longcomplex_array.mtx
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longcomplex_coordinate.mtx
+-rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longdouble_array.mtx
+-rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/long_double/longdouble_coordinate.mtx
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_array_complex_general.mtx
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_array_integer_general.mtx
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_array_real_general.mtx
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_complex_general.mtx
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_complex_hermitian.mtx
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_integer_general.mtx
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_pattern_general.mtx
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_general.mtx
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_general.mtx.bz2
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_general.mtx.gz
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/matrix_coordinate_real_symmetric.mtx
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/misc/windows_newlines.mtx
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/scipy_crashes/vector_array_real_general.mtx
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
+-rw-r--r--   0        0        0     2272 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_array.py
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_basic.py
+-rw-r--r--   0        0        0     3643 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_coo.py
+-rw-r--r--   0        0        0     3903 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_header.py
+-rw-r--r--   0        0        0    19343 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/tests/test_scipy.py
+-rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/testsuite_scipy/test_scipy_suite.py
+-rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.7.0/PKG-INFO
```

### Comparing `fast-matrix-market-1.6.0/LICENSE.txt` & `fast-matrix-market-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/README.md` & `fast-matrix-market-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/benchmark/bench_fmm.py` & `fast-matrix-market-1.7.0/benchmark/bench_fmm.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,24 +15,33 @@
 
 import fast_matrix_market as fmm
 
 
 def generate_large_coo_matrix(nnz):
     i = np.arange(nnz, dtype="int32")  # scipy uses intc indices (intc is usually int32)
     j = i
-    vals = np.arange(nnz, dtype="float64")
-    vals /= 100
+    vals = np.arange(nnz, dtype="float64") / 100
     return coo_matrix((vals, (i, j)), shape=(nnz, nnz))
 
 
+def generate_large_csc_matrix(nnz):
+    ncols = 1000
+    # nnz = int((size_bytes - (nrows + 1) * 4) / (4 + 8))
+    indptr = (np.arange(ncols + 1, dtype=np.float32) / ncols * nnz).astype(np.int32)
+    indptr[-1] = nnz
+    indices = np.arange(nnz, dtype=np.int32)
+    # vals = np.random.default_rng().uniform(low=0, high=1.0, size=nnz)
+    vals = np.arange(nnz, dtype="float64") / 100
+    return scipy.sparse.csc_matrix((vals, indices, indptr), shape=(nnz, ncols))
+
+
 def generate_large_array_matrix(nnz):
     n = int(math.sqrt(nnz))
     m = int(nnz / n)
-    mat = np.arange(m*n, dtype="float64")
-    mat /= 100
+    mat = np.arange(m*n, dtype="float64") / 100
     mat = np.reshape(mat, (m, n))
     return mat
 
 
 def matrix_to_bytes(mat):
     bio = BytesIO()
     fmm.write_scipy(bio, a=mat)
@@ -48,25 +57,34 @@
 large_coo_matrix = generate_large_coo_matrix(num_elements)
 large_coo_bytes = matrix_to_bytes(large_coo_matrix)
 large_coo_length = len(large_coo_bytes)   # About 265 MB for nnz=10M
 
 coo_read_path = Path(tempdir.name) / "readfile_coo.mtx"
 coo_read_path.write_bytes(large_coo_bytes)
 
+# Generate CSC matrix
+large_csc_matrix = generate_large_csc_matrix(num_elements)
+large_csc_bytes = matrix_to_bytes(large_csc_matrix)
+large_csc_length = len(large_csc_bytes)   # About 265 MB for nnz=10M
+
+csc_read_path = Path(tempdir.name) / "readfile_csc.mtx"
+csc_read_path.write_bytes(large_csc_bytes)
+
 # Generate array matrix
 large_array_matrix = generate_large_array_matrix(num_elements)
 
 large_array_bytes = matrix_to_bytes(large_array_matrix)
 large_array_length = len(large_array_bytes)  # About 50 MB for nnz=10M
 
 array_read_path = Path(tempdir.name) / "readfile_array.mtx"
 array_read_path.write_bytes(large_array_bytes)
 
 print(f"Array matrix has {large_array_matrix.size:,} elements and {large_array_length:,} bytes in MatrixMarket format.")
 print(f"Triplet matrix has {large_coo_matrix.size:,} elements and {large_coo_length:,} bytes in MatrixMarket format.")
+print(f"CSC matrix has {large_csc_matrix.size:,} elements and {large_csc_length:,} bytes in MatrixMarket format.")
 
 
 ##############################
 # Arrays
 
 @benchmark.register(name="op:read/matrix:Array/impl:FMM(Python)/lang:Python")
 @benchmark.option.use_real_time()
@@ -191,9 +209,44 @@
     while state:
         # Specifying a symmetry prevents scipy from searching for a symmetry.
         # This can greatly speed up mmwrite()
         scipy.io.mmwrite(write_path, large_coo_matrix, symmetry="general")
     state.bytes_processed = state.iterations * write_path.stat().st_size
 
 
+##############################
+# CSC
+
+@benchmark.register(name="op:write/matrix:CSC/impl:FMM(Python)/lang:Python")
+@benchmark.option.use_real_time()
+@benchmark.option.iterations(3)
+@benchmark.option.arg_name("p")
+@benchmark.option.arg(1)
+@benchmark.option.arg_name("p")
+@benchmark.option.arg(2)
+@benchmark.option.arg_name("p")
+@benchmark.option.arg(3)
+@benchmark.option.arg_name("p")
+@benchmark.option.arg(4)
+@benchmark.option.arg_name("p")
+@benchmark.option.arg(6)
+@benchmark.option.arg_name("p")
+@benchmark.option.arg(8)
+def csc_write_fmm(state):
+    while state:
+        parallelism = state.range(0)
+        fmm.write_scipy(write_path, large_csc_matrix, parallelism=parallelism)
+    state.bytes_processed = state.iterations * write_path.stat().st_size
+
+
+@benchmark.register(name="op:write/matrix:CSC/impl:SciPy/lang:Python")
+@benchmark.option.use_real_time()
+def csc_write_scipy(state):
+    while state:
+        # Specifying a symmetry prevents scipy from searching for a symmetry.
+        # This can greatly speed up mmwrite()
+        scipy.io.mmwrite(write_path, large_csc_matrix, symmetry="general")
+    state.bytes_processed = state.iterations * write_path.stat().st_size
+
+
 if __name__ == "__main__":
     benchmark.main()
```

### Comparing `fast-matrix-market-1.6.0/benchmark/run.sh` & `fast-matrix-market-1.7.0/benchmark/run.sh`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/CMakeLists.txt` & `fast-matrix-market-1.7.0/fast_matrix_market/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/cmake/GraphBLAS.cmake` & `fast-matrix-market-1.7.0/fast_matrix_market/cmake/GraphBLAS.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/cmake/from_chars_tests.cmake` & `fast-matrix-market-1.7.0/fast_matrix_market/cmake/from_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/cmake/to_chars_tests.cmake` & `fast-matrix-market-1.7.0/fast_matrix_market/cmake/to_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/README.md` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Dependencies
 
 These optional dependencies speed up floating-point parsing and formatting.
-Standard library fallbacks are included but both sequential and parallel performance can suffer without them.
+Standard library fallbacks are included but both sequential and parallel performance suffer without them.
 
 ## [fast_float](https://github.com/fastfloat/fast_float)
 Floating-point parsing.
 
 Using the header-only single file release version. To upgrade just paste in a new version of `fast_float.h`.
 
 Optional, set `FMM_USE_FAST_FLOAT=OFF` to disable.
 
 ## [Dragonbox](https://github.com/jk-jeon/dragonbox)
-Floating-point rendering.
+Floating-point rendering for shortest representation only.
 
 Using a pruned copy of the dragonbox repo. The full release includes two large PDFs, subprojects, etc.
 Just clone the repo and delete anything not needed to build the library.
 
 Optional, set `FMM_USE_DRAGONBOX=OFF` to disable.
 
 ## [Ryu](https://github.com/ulfjack/ryu)
-Floating-point rendering with user-specified precision.
+Floating-point rendering supports both shortest representation and user-specified precision.
 
 Optional, set `FMM_USE_RYU=OFF` to disable.
 
-## [thread-pool](https://github.com/bshoshany/thread-pool)
+## [task-thread-pool](https://github.com/alugowski/task-thread-pool)
 A lightweight thread pool using C++11 threads. Bundled in `include/`.
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/common.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/common.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h` & `fast-matrix-market-1.7.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         header.object = matrix;
         if (header.field != pattern) {
             header.field = get_field_type((const VT *) nullptr);
         }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         line_formatter<arma::uword, VT> lf(header, options);
         auto formatter = csc_formatter(lf,
                                        m.col_ptrs, m.col_ptrs + m.n_cols,  // explicitly no +1
                                        m.row_indices, m.row_indices + m.n_nonzero,
                                        m.values, header.field == pattern ? m.values : m.values + m.n_nonzero,
                                        false);
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
         header.object = matrix;
         if (header.field != pattern) {
             header.field = get_field_type((const VT*)nullptr);
         }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         const bool is_row_major = blaze::IsRowMajorMatrix_v<SparseMatrix>;
 
         line_formatter<IT, VT> lf(header, options);
         auto formatter = Blaze_CompressedMatrix_formatter(lf, mat, is_row_major ? header.nrows : header.ncols);
         write_body(os, formatter, options);
     }
@@ -234,15 +234,15 @@
         header.ncols = mat.columns();
         header.nnz = mat.rows() * mat.columns();
 
         header.object = matrix;
         header.field = get_field_type((const VT *) nullptr);
         header.format = array;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         line_formatter<IT, VT> lf(header, options);
         auto formatter = dense_2d_call_formatter(lf, mat, header.nrows, header.ncols);
         write_body(os, formatter, options);
     }
 
 
@@ -349,15 +349,15 @@
 
         header.object = vector;
         if (header.field != pattern) {
             header.field = get_field_type((const VT*)nullptr);
         }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         // write the body
 
         vector_line_formatter<IT, VT> lf(header, options);
         auto formatter = triplet_formatter(lf,
                                            indices.begin(), indices.end(),
                                            indices.begin(), indices.end(),
@@ -380,14 +380,14 @@
         header.vector_length = vector_length;
         header.nnz = vector_length;
 
         header.object = vector;
         header.field = get_field_type((const VT *) nullptr);
         header.format = array;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         line_formatter<int64_t, VT> lf(header, options);
         auto formatter = array_formatter(lf, vec.data(), row_major, vector_length, 1);
         write_body(os, formatter, options);
     }
 }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,16 @@
         *cs = spalloc(header.nrows, header.ncols, get_storage_nnz(header, options),
                       header.field == pattern ? 0 : 1, // pattern field means do not allocate values
                       1);
         if (*cs == nullptr) {
             return;
         }
 
-        if (header.field == pattern) {
-            auto handler = triplet_pattern_parse_handler((*cs)->i, (*cs)->p);
-            read_matrix_market_body_no_pattern(instream, header, handler, options);
-        } else {
-            auto handler = triplet_parse_handler((*cs)->i, (*cs)->p, (*cs)->x);
-            read_matrix_market_body_no_pattern(instream, header, handler, options);
-        }
+        auto handler = triplet_parse_handler((*cs)->i, (*cs)->p, (*cs)->x);
+        read_matrix_market_body_no_adapters(instream, header, handler, options);
 
         // nz > 0 indicates a triplet matrix.
         (*cs)->nz = (*cs)->nzmax;
     }
 
     /**
      * Write a CXSparse cs_* structure to MatrixMarket.
@@ -55,15 +50,15 @@
         if (cs->x == nullptr) {
             header.field = pattern;
         } else {
             header.field = get_field_type(cs->x);
         }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         if (cs->nz == -1) {
             // compressed
             line_formatter<decltype(*cs->i), decltype(*cs->x)> lf(header, options);
             auto formatter = csc_formatter(lf,
                                            cs->p, cs->p + cs->n, // explicitly no +1
                                            cs->i, cs->i + cs->nzmax,
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
         header.object = matrix;
         if (header.field != pattern) {
             header.field = get_field_type((const typename SparseType::Scalar*)nullptr);
         }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         line_formatter<typename SparseType::Index, typename SparseType::Scalar> lf(header, options);
         auto formatter = sparse_Eigen_formatter(lf, mat);
         write_body(os, formatter, options);
     }
 
     /**
@@ -177,14 +177,14 @@
         header.ncols = mat.cols();
         header.nnz = mat.rows() * mat.cols();
 
         header.object = matrix;
         header.field = get_field_type((const typename DenseType::Scalar*)nullptr);
         header.format = array;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         line_formatter<typename DenseType::Index, typename DenseType::Scalar> lf(header, options);
         auto formatter = dense_2d_call_formatter(lf, mat, mat.rows(), mat.cols());
         write_body(os, formatter, options);
     }
 }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -554,15 +554,15 @@
         std::vector<GrB_Index> rows(storage_nnz);
         std::vector<GrB_Index> cols(storage_nnz);
 
 #if FMM_GXB_BUILD_SCALAR
         if (header.field == pattern) {
             // read the indices
             auto handler = triplet_pattern_parse_handler(rows.begin(), cols.begin());
-            read_matrix_market_body_no_pattern(instream, header, handler, options);
+            read_matrix_market_body_no_adapters(instream, header, handler, options);
 
             // create the scalar
             GrB_Scalar one;
             ok(GrB_Scalar_new(&one, GraphBLAS_typed<T>::type()));
             ok(GraphBLAS_typed<T>::set_element(one, pattern_default_value(static_cast<T*>(nullptr))));
 
             // Build iso matrix
@@ -1167,15 +1167,15 @@
         // GraphBLAS throws GrB_NOT_IMPLEMENTED.
 //        if (header.nnz == header.nrows * header.ncols) {
 //            // Full matrix. Only efficient way to write arrays is using a column iterator, which requires a GraphBLAS extension.
 //            header.format = array;
 //        }
 #endif
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         if (type == GrB_BOOL) {
             write_body_graphblas<bool>(os, header, mat, options);
         } else if (type == GrB_INT8) {
             write_body_graphblas<int8_t>(os, header, mat, options);
         } else if (type == GrB_INT16) {
             write_body_graphblas<int16_t>(os, header, mat, options);
@@ -1387,15 +1387,15 @@
 
         header.object = vector;
         if (header.field != pattern) {
             header.field = get_field(type);
         }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         if (type == GrB_BOOL) {
             write_body_graphblas<bool>(os, header, vec, options);
         } else if (type == GrB_INT8) {
             write_body_graphblas<int8_t>(os, header, vec, options);
         } else if (type == GrB_INT16) {
             write_body_graphblas<int16_t>(os, header, vec, options);
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         header.nnz = values.size();
 
         header.object = matrix;
         header.field = get_field_type((const VT*)nullptr);
         header.format = array;
         header.symmetry = general;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         line_formatter<int64_t, VT> lf(header, options);
         auto formatter = array_formatter(lf, values.begin(), order, header.nrows, header.ncols);
         write_body(os, formatter, options);
     }
 
 #if __cplusplus < 202002L
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -80,27 +80,31 @@
                                      matrix_market_header header,
                                      const IVEC& indices,
                                      const VVEC& values,
                                      const write_options& options = {}) {
         using IT = typename std::iterator_traits<decltype(indices.begin())>::value_type;
         using VT = typename std::iterator_traits<decltype(values.begin())>::value_type;
 
-        header.nnz = values.size();
+        header.nnz = indices.size();
 
         header.object = vector;
-        header.field = get_field_type((const VT*)nullptr);
+        if (header.nnz > 0 && (values.cbegin() == values.cend())) {
+            header.field = pattern;
+        } else if (header.field != pattern) {
+            header.field = get_field_type((const VT *) nullptr);
+        }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         vector_line_formatter<IT, VT> lf(header, options);
         auto formatter = triplet_formatter(lf,
-                                          indices.begin(), indices.end(),
-                                          indices.begin(), indices.end(),
-                                          values.begin(), values.end());
+                                          indices.cbegin(), indices.cend(),
+                                          indices.cbegin(), indices.cend(),
+                                          values.cbegin(), header.field == pattern ? values.cbegin() : values.cend());
         write_body(os, formatter, options);
     }
 
 #if __cplusplus < 202002L
     // clean up after ourselves
 #undef doublet_read_vector
 #undef doublet_write_vector
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -79,31 +79,68 @@
                                      const IVEC& rows,
                                      const IVEC& cols,
                                      const VVEC& values,
                                      const write_options& options = {}) {
         using IT = typename std::iterator_traits<decltype(rows.begin())>::value_type;
         using VT = typename std::iterator_traits<decltype(values.begin())>::value_type;
 
-        header.nnz = values.size();
+        header.nnz = rows.size();
 
         header.object = matrix;
-        if (header.field != pattern) {
+        if (header.nnz > 0 && (values.cbegin() == values.cend())) {
+            header.field = pattern;
+        } else if (header.field != pattern) {
             header.field = get_field_type((const VT *) nullptr);
         }
         header.format = coordinate;
 
-        write_header(os, header);
+        write_header(os, header, options);
 
         line_formatter<IT, VT> lf(header, options);
         auto formatter = triplet_formatter(lf,
                                            rows.cbegin(), rows.cend(),
                                            cols.cbegin(), cols.cend(),
                                            values.cbegin(), header.field == pattern ? values.cbegin() : values.cend());
         write_body(os, formatter, options);
     }
 
+    /**
+     * Write CSC/CSR to a Matrix Market file.
+     */
+    template <triplet_write_vector IVEC, triplet_write_vector VVEC>
+    void write_matrix_market_csc(std::ostream &os,
+                                 matrix_market_header header,
+                                 const IVEC& indptr,
+                                 const IVEC& indices,
+                                 const VVEC& values,
+                                 bool is_csr,
+                                 const write_options& options = {}) {
+        using IT = typename std::iterator_traits<decltype(indptr.begin())>::value_type;
+        using VT = typename std::iterator_traits<decltype(values.begin())>::value_type;
+
+        header.nnz = indices.size();
+
+        header.object = matrix;
+        if (header.nnz > 0 && (values.cbegin() == values.cend())) {
+            header.field = pattern;
+        } else if (header.field != pattern) {
+            header.field = get_field_type((const VT *) nullptr);
+        }
+        header.format = coordinate;
+
+        write_header(os, header, options);
+
+        line_formatter<IT, VT> lf(header, options);
+        auto formatter = csc_formatter(lf,
+                                       indptr.cbegin(), indptr.cend() - 1,
+                                       indices.cbegin(), indices.cend(),
+                                       values.cbegin(), header.field == pattern ? values.cbegin() : values.cend(),
+                                       is_csr);
+        write_body(os, formatter, options);
+    }
+
 #if __cplusplus < 202002L
     // clean up after ourselves
 #undef triplet_read_vector
 #undef triplet_write_vector
 #endif
 }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 #pragma once
 
 #include <istream>
 #include <string>
 
 namespace fast_matrix_market {
-    inline std::string get_next_chunk(std::istream &instream, const read_options &options) {
+    inline void get_next_chunk(std::string& chunk, std::istream &instream, const read_options &options) {
         constexpr size_t chunk_extra = 4096; // extra chunk bytes to leave room for rest of line
-
-        // allocate chunk
-        std::string chunk(options.chunk_size_bytes, ' ');
         size_t chunk_length = 0;
 
+        // ensure enough space
+        chunk.resize(options.chunk_size_bytes);
+
         // read chunk from the stream
         auto bytes_to_read = chunk.size() > chunk_extra ? (std::streamsize) (chunk.size() - chunk_extra) : 0;
         if (bytes_to_read > 0) {
             instream.read(chunk.data(), bytes_to_read);
             auto num_read = instream.gcount();
             chunk_length = num_read;
 
             // test for EOF
             if (num_read == 0 || instream.eof() || chunk[chunk_length - 1] == '\n') {
                 chunk.resize(chunk_length);
-                return chunk;
+                return;
             }
         }
 
         // Read rest of line and append to the chunk.
         std::string suffix;
         std::getline(instream, suffix);
         if (instream.good()) {
@@ -42,14 +42,20 @@
             chunk += suffix;
         } else {
             // the suffix fits in the chunk.
             std::copy(suffix.begin(), suffix.end(), chunk.begin() + (ptrdiff_t) chunk_length);
             chunk_length += suffix.size();
             chunk.resize(chunk_length);
         }
+    }
+
+    inline std::string get_next_chunk(std::istream &instream, const read_options &options) {
+        // allocate chunk
+        std::string chunk(options.chunk_size_bytes, ' ');
+        get_next_chunk(chunk, instream, options);
         return chunk;
     }
 
     template <typename ITER>
     bool is_all_spaces(ITER begin, ITER end) {
         return std::all_of(begin, end, [](char c) { return c == ' ' || c == '\t'; });
     }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #include "types.hpp"
 
 namespace fast_matrix_market {
 
     // Version macros.
     // Keep in sync with python/pyproject.toml
 #define FAST_MATRIX_MARKET_VERSION_MAJOR 1
-#define FAST_MATRIX_MARKET_VERSION_MINOR 6
+#define FAST_MATRIX_MARKET_VERSION_MINOR 7
 #define FAST_MATRIX_MARKET_VERSION_PATCH 0
 
     constexpr std::string_view kSpace = " ";
     constexpr std::string_view kNewline = "\n";
 
     template<class T> struct is_complex : std::false_type {};
     template<class T> struct is_complex<std::complex<T>> : std::true_type {};
@@ -82,14 +82,30 @@
      */
     class complex_incompatible : public invalid_argument {
     public:
         explicit complex_incompatible(std::string msg): invalid_argument(std::move(msg)) {}
     };
 
     /**
+     * A Matrix Market file requires a feature that has been disabled via compilation flags.
+     */
+    class support_not_selected : public invalid_argument {
+    public:
+        explicit support_not_selected(std::string msg): invalid_argument(std::move(msg)) {}
+    };
+
+    /**
+     * Matrix Market file is a `vector` type, but vector support is disabled in this build.
+     */
+    class no_vector_support : public support_not_selected {
+    public:
+        explicit no_vector_support(std::string msg): support_not_selected(std::move(msg)) {}
+    };
+
+    /**
      * A value type to use for pattern matrices. Pattern Matrix Market files do not write a value column, only the
      * coordinates. Setting this as the value type signals the parser to not attempt to read a column that isn't there.
      */
     struct pattern_placeholder_type {};
 
     /**
      * Negation of a pattern_placeholder_type needed to support symmetry generalization.
@@ -167,14 +183,32 @@
         // rtrim
         s.erase(std::find_if(s.rbegin(), s.rend(), [](unsigned char ch) {
             return !std::isspace(ch);
         }).base(), s.end());
 
         return s;
     }
+
+    /**
+     * Replace all instances of `from` with `to` in `str`.
+     */
+    inline std::string replace_all(const std::string& str, const std::string& from, const std::string& to) {
+        std::string ret(str);
+
+        if (from.empty())
+            return ret;
+
+        std::string::size_type start_pos = 0;
+        while ((start_pos = ret.find(from, start_pos)) != std::string::npos) {
+            ret.replace(start_pos, from.length(), to);
+            start_pos += to.length();
+        }
+
+        return ret;
+    }
 }
 
 #include "field_conv.hpp"
 #include "header.hpp"
 #include "parse_handlers.hpp"
 #include "formatters.hpp"
 #include "read_body.hpp"
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -408,93 +408,128 @@
         } else {
             std::ostringstream oss;
             oss << std::setprecision(precision) << value;
             return oss.str();
         }
     }
 
-#ifdef FMM_USE_DRAGONBOX
+// Sometimes Dragonbox and Ryu may render '1' as '1E0'
+// This controls whether to truncate those suffixes.
+#ifndef FMM_DROP_ENDING_E0
+#define FMM_DROP_ENDING_E0 1
+#endif
 
-    #ifndef DRAGONBOX_DROP_E0
-    #define DRAGONBOX_DROP_E0 true
-    #endif
+// Same as above, but for context where precision is specified
+#ifndef FMM_DROP_ENDING_E0_PRECISION
+#define FMM_DROP_ENDING_E0_PRECISION 0
+#endif
+
+#ifdef FMM_USE_DRAGONBOX
 
     inline std::string value_to_string_dragonbox(const float& value) {
         std::string buffer(jkj::dragonbox::max_output_string_length<jkj::dragonbox::ieee754_binary32> + 1, ' ');
 
         char *end_ptr = jkj::dragonbox::to_chars(value, buffer.data());
         buffer.resize(end_ptr - buffer.data());
 
-        if (DRAGONBOX_DROP_E0 && ends_with(buffer, "E0")) {
+#if FMM_DROP_ENDING_E0
+        if (ends_with(buffer, "E0")) {
             buffer.resize(buffer.size() - 2);
         }
+#endif
         return buffer;
     }
 
     inline std::string value_to_string_dragonbox(const double& value) {
         std::string buffer(jkj::dragonbox::max_output_string_length<jkj::dragonbox::ieee754_binary64> + 1, ' ');
 
         char *end_ptr = jkj::dragonbox::to_chars(value, buffer.data());
         buffer.resize(end_ptr - buffer.data());
 
-        if (DRAGONBOX_DROP_E0 && ends_with(buffer, "E0")) {
+#if FMM_DROP_ENDING_E0
+        if (ends_with(buffer, "E0")) {
             buffer.resize(buffer.size() - 2);
         }
+#endif
         return buffer;
     }
 #endif
 
 #ifdef FMM_USE_RYU
     inline std::string value_to_string_ryu(const float& value, int precision) {
         std::string ret(16, ' ');
 
         if (precision < 0) {
             // shortest representation
             auto len = f2s_buffered_n(value, ret.data());
             ret.resize(len);
+
+#if FMM_DROP_ENDING_E0
+            if (ends_with(ret, "E0")) {
+                ret.resize(ret.size() - 2);
+            }
+#endif
         } else {
             // explicit precision
             if (precision > 0) {
                 // d2exp_buffered_n's precision means number of places after the decimal point, but
                 // we expect it to mean number of sigfigs.
                 --precision;
             }
             auto len = d2exp_buffered_n(static_cast<double>(value), precision, ret.data());
             ret.resize(len);
+
+#if FMM_DROP_ENDING_E0_PRECISION
+            if (ends_with(ret, "e+00")) {
+                ret.resize(ret.size() - 4);
+            }
+#endif
         }
 
         return ret;
     }
 
     inline std::string value_to_string_ryu(const double& value, int precision) {
         std::string ret(26, ' ');
 
         if (precision < 0) {
             // shortest representation
             auto len = d2s_buffered_n(value, ret.data());
             ret.resize(len);
+
+#if FMM_DROP_ENDING_E0
+            if (ends_with(ret, "E0")) {
+                ret.resize(ret.size() - 2);
+            }
+#endif
         } else {
             // explicit precision
             if (precision > 0) {
                 // d2exp_buffered_n's precision means number of places after the decimal point, but
                 // we expect it to mean number of sigfigs.
                 --precision;
             }
             auto len = d2exp_buffered_n(value, precision, ret.data());
             ret.resize(len);
+
+#if FMM_DROP_ENDING_E0_PRECISION
+            if (ends_with(ret, "e+00")) {
+                ret.resize(ret.size() - 4);
+            }
+#endif
         }
 
         return ret;
     }
 #endif
 
 #ifdef FMM_TO_CHARS_DOUBLE_SUPPORTED
     inline std::string value_to_string_to_chars(const float& value, int precision) {
         std::string ret(16, ' ');
-        std::to_chars_result result;
+        std::to_chars_result result{};
         if (precision < 0) {
             // shortest representation
             result = std::to_chars(ret.data(), ret.data() + ret.size(), value);
         } else {
             // explicit precision
             result = std::to_chars(ret.data(), ret.data() + ret.size(), value, std::chars_format::general, precision);
         }
@@ -504,15 +539,15 @@
         } else {
             return value_to_string_fallback(value, precision);
         }
     }
 
     inline std::string value_to_string_to_chars(const double& value, int precision) {
         std::string ret(25, ' ');
-        std::to_chars_result result;
+        std::to_chars_result result{};
         if (precision < 0) {
             // shortest representation
             result = std::to_chars(ret.data(), ret.data() + ret.size(), value);
         } else {
             // explicit precision
             result = std::to_chars(ret.data(), ret.data() + ret.size(), value, std::chars_format::general, precision);
         }
@@ -524,15 +559,15 @@
         }
     }
 #endif
 
 #ifdef FMM_TO_CHARS_LONG_DOUBLE_SUPPORTED
     inline std::string value_to_string_to_chars(const long double& value, int precision) {
         std::string ret(50, ' ');
-        std::to_chars_result result;
+        std::to_chars_result result{};
         if (precision < 0) {
             // shortest representation
             result = std::to_chars(ret.data(), ret.data() + ret.size(), value);
         } else {
             // explicit precision
             result = std::to_chars(ret.data(), ret.data() + ret.size(), value, std::chars_format::general, precision);
         }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             PTR_ITER ptr_begin, ptr_iter, ptr_end;
             IND_ITER ind_begin;
             VAL_ITER val_begin, val_end;
             bool transpose;
         };
 
         chunk next_chunk(const write_options& options) {
-            auto num_columns = (int64_t)(nnz_per_column * (double)options.chunk_size_values + 1);
+            auto num_columns = (int64_t)(((double)options.chunk_size_values / nnz_per_column) + 1);
 
             num_columns = std::min(num_columns, (int64_t)(ptr_end - ptr_iter));
             PTR_ITER ptr_chunk_end = ptr_iter + num_columns;
 
             chunk c(line_formatter,
                     ptr_begin, ptr_iter, ptr_chunk_end,
                     ind_begin,
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/header.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/header.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -109,23 +109,30 @@
      */
     inline bool read_comment(matrix_market_header& header, const std::string& line) {
         // empty lines are allowed anywhere in the file and are to be ignored
         if (is_line_all_spaces(line)) {
             return true;
         }
 
-        if (line[0] != '%') {
+        unsigned int pos = 0;
+
+        // skip leading whitespace
+        while ((pos+1) < line.size() && std::isblank(line[pos])) {
+            ++pos;
+        }
+
+        if (line[pos] != '%') {
             return false;
         }
 
+        // skip the '%'
+        ++pos;
+
         // Line is a comment. Save it to the header.
-        if (!header.comment.empty()) {
-            header.comment += "\n";
-        }
-        header.comment += line.substr(1);
+        header.comment += line.substr(pos) + "\n";
         return true;
     }
 
     /**
      * Parse an enum, but with error message fitting parsing of header.
      */
     template <typename ENUM>
@@ -185,14 +192,19 @@
             lines_read++;
 
             if (!instream) {
                 throw invalid_mm("Invalid MatrixMarket header: Premature EOF", lines_read);
             }
         } while (read_comment(header, line));
 
+        // trim off final comment newline
+        if (ends_with(header.comment, "\n")) {
+            header.comment.resize(header.comment.size() - 1);
+        }
+
         // parse the dimension line
         {
             std::istringstream iss(line);
             int expected_length = -1;
 
             const char* pos = line.c_str();
             const char* end = line.c_str() + line.size();
@@ -251,29 +263,29 @@
         }
 
         header.header_line_count = lines_read;
 
         return lines_read;
     }
 
-    inline bool write_header(std::ostream& os, const matrix_market_header& header) {
+    inline bool write_header(std::ostream& os, const matrix_market_header& header, const write_options options = {}) {
         // Write the banner
         os << kMatrixMarketBanner << kSpace;
         os << object_map.at(header.object) << kSpace;
         os << format_map.at(header.format) << kSpace;
         os << field_map.at(header.field) << kSpace;
         os << symmetry_map.at(header.symmetry) << kNewline;
 
         // Write the comment
-        {
-            std::istringstream iss(header.comment);
-            std::string line;
-            while (std::getline(iss, line)) {
-                os << "%" << line << kNewline;
-            }
+        if (!header.comment.empty()) {
+            std::string write_comment = replace_all(header.comment, "\n", "\n%");
+
+            os << "%" << write_comment << kNewline;
+        } else if (options.always_comment) {
+            os << "%" << kNewline;
         }
 
         // Write dimension line
         if (header.object == vector) {
             os << header.vector_length;
             if (header.format == coordinate) {
                 os << kSpace << header.nnz;
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,23 @@
             *values = value;
 
             ++rows;
             ++cols;
             ++values;
         }
 
+        void handle(const coordinate_type row, const coordinate_type col, [[maybe_unused]] const pattern_placeholder_type& pat) {
+            *rows = row;
+            *cols = col;
+
+            ++rows;
+            ++cols;
+            ++values;
+        }
+
         triplet_parse_handler<IT_ITER, VT_ITER> get_chunk_handler(int64_t offset_from_begin) {
             return triplet_parse_handler(begin_rows + offset_from_begin,
                                          begin_cols + offset_from_begin,
                                          begin_values + offset_from_begin);
         }
 
     protected:
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -12,66 +12,80 @@
 namespace fast_matrix_market {
 
     struct line_counts {
         int64_t file_line = 0;
         int64_t element_num = 0;
     };
 
+    enum compile_format {compile_array_only = 1, compile_coordinate_only = 2, compile_all = 3};
+
     /**
      * A handler wrapper for easily handling pattern matrices. This forwards a fixed value. For example, write 1.0 to
      * double matrices. Avoid using zero.
      */
     template<typename FWD_HANDLER>
     class pattern_parse_adapter {
     public:
         using coordinate_type = typename FWD_HANDLER::coordinate_type;
-        using value_type = pattern_placeholder_type;
+        using value_type = typename FWD_HANDLER::value_type;
         static constexpr int flags = FWD_HANDLER::flags;
 
         explicit pattern_parse_adapter(const FWD_HANDLER &handler, typename FWD_HANDLER::value_type fwd_value) : handler(
                 handler), fwd_value(fwd_value) {}
 
-        void handle(const coordinate_type row, const coordinate_type col, [[maybe_unused]] const value_type ignored) {
+        void handle(const coordinate_type row, const coordinate_type col, [[maybe_unused]] const pattern_placeholder_type ignored) {
             handler.handle(row, col, fwd_value);
         }
 
+        void handle(const coordinate_type row, const coordinate_type col, const value_type val) {
+            handler.handle(row, col, val);
+        }
+
         pattern_parse_adapter<FWD_HANDLER> get_chunk_handler(int64_t offset_from_start) {
             return pattern_parse_adapter<FWD_HANDLER>(handler.get_chunk_handler(offset_from_start), fwd_value);
         }
 
     protected:
         FWD_HANDLER handler;
         typename FWD_HANDLER::value_type fwd_value;
     };
 
+#ifndef FMM_SCIPY_PRUNE
     /**
      * A handler wrapper so that real/integer files can be read into std::complex matrices by setting all
      * imaginary parts to zero.
+     *
+     * @deprecated as this adaptation is now done in the inner loops, negating the need for this.
      */
     template<typename COMPLEX_HANDLER>
-    class complex_parse_adapter {
+    class [[maybe_unused]] complex_parse_adapter {
     public:
         using coordinate_type = typename COMPLEX_HANDLER::coordinate_type;
         using complex_type = typename COMPLEX_HANDLER::value_type;
         using value_type = typename complex_type::value_type;
         static constexpr int flags = COMPLEX_HANDLER::flags;
 
         explicit complex_parse_adapter(const COMPLEX_HANDLER &handler) : handler(handler) {}
 
+        void handle(const coordinate_type row, const coordinate_type col, const pattern_placeholder_type& pat) {
+            handler.handle(row, col, pat);
+        }
+
         void handle(const coordinate_type row, const coordinate_type col, const value_type real) {
             handler.handle(row, col, complex_type(real, 0));
         }
 
         complex_parse_adapter<COMPLEX_HANDLER> get_chunk_handler(int64_t offset_from_start) {
             return complex_parse_adapter(handler.get_chunk_handler(offset_from_start));
         }
 
     protected:
         COMPLEX_HANDLER handler;
     };
+#endif
 
     ///////////////////////////////////////////////////////////////////
     // Limit bool parallelism
     // vector<bool> is specialized to use a bitfield-like scheme. This means
     // that different elements can share the same bytes, making
     // writes to this container require locking.
     // Instead, disable parallelism for bools.
@@ -86,14 +100,100 @@
         return parallelism_selected;
     }
 
     ///////////////////////////////////////////////////////////////////
     // Chunks
     ///////////////////////////////////////////////////////////////////
 
+    template<typename HANDLER, typename IT, typename VT>
+    void generalize_symmetry_coordinate(HANDLER& handler,
+                                        const matrix_market_header &header,
+                                        const read_options &options,
+                                        const IT& row,
+                                        const IT& col,
+                                        const VT& value) {
+        if (col != row) {
+            switch (header.symmetry) {
+                case symmetric:
+                    handler.handle(col, row, value);
+                    break;
+                case skew_symmetric:
+                    if constexpr (!std::is_unsigned_v<typename HANDLER::value_type>) {
+                        handler.handle(col, row, negate(value));
+                    } else {
+                        throw invalid_argument("Cannot load skew-symmetric matrix into unsigned value type.");
+                    }
+                    break;
+                case hermitian:
+                    handler.handle(col, row, complex_conjugate(value));
+                    break;
+                case general: break;
+            }
+        } else {
+            if (!test_flag(HANDLER::flags, kAppending)) {
+                switch (options.generalize_coordinate_diagnonal_values) {
+                    case read_options::ExtraZeroElement:
+                        handler.handle(row, col, get_zero<typename HANDLER::value_type>());
+                        break;
+                    case read_options::DuplicateElement:
+                        handler.handle(row, col, value);
+                        break;
+                }
+            }
+        }
+    }
+
+    template<typename HANDLER, typename IT, typename VT>
+    void generalize_symmetry_array(HANDLER& handler,
+                                   const matrix_market_header &header,
+                                   const IT& row,
+                                   const IT& col,
+                                   const VT& value) {
+        switch (header.symmetry) {
+            case symmetric:
+                handler.handle(col, row, value);
+                break;
+            case skew_symmetric:
+                if constexpr (!std::is_unsigned_v<typename HANDLER::value_type>) {
+                    handler.handle(col, row, negate(value));
+                } else {
+                    throw invalid_argument("Cannot load skew-symmetric matrix into unsigned value type.");
+                }
+                break;
+            case hermitian:
+                handler.handle(col, row, complex_conjugate(value));
+                break;
+            case general:
+                break;
+        }
+    }
+
+    /**
+     * Read a value, adapting real matrix values to complex datastructures.
+     */
+    template <typename value_type>
+    void read_real_or_complex(value_type& value,
+                              const char*& pos,
+                              const char* end,
+                              const matrix_market_header &header,
+                              const read_options &options) {
+        if constexpr (is_complex<value_type>::value) {
+            if (header.field == complex) {
+                pos = read_value(pos, end, value, options);
+            } else {
+                typename value_type::value_type real;
+                pos = read_value(pos, end, real, options);
+                value.real(real);
+                value.imag(0);
+            }
+        } else {
+            pos = read_value(pos, end, value, options);
+        }
+    }
+
     template<typename HANDLER>
     line_counts read_chunk_matrix_coordinate(const std::string &chunk, const matrix_market_header &header,
                                              line_counts line, HANDLER &handler, const read_options &options) {
         const char *pos = chunk.c_str();
         const char *end = pos + chunk.size();
 
         while (pos != end) {
@@ -109,73 +209,59 @@
                 if (line.element_num >= header.nnz) {
                     throw invalid_mm("Too many lines in file (file too long)");
                 }
 
                 pos = read_int(pos, end, row);
                 pos = skip_spaces(pos);
                 pos = read_int(pos, end, col);
-                pos = skip_spaces(pos);
-                pos = read_value(pos, end, value, options);
+                if (header.field != pattern) {
+                    pos = skip_spaces(pos);
+                    read_real_or_complex(value, pos, end, header, options);
+                }
                 pos = bump_to_next_line(pos, end);
 
                 // validate
                 if (row <= 0 || static_cast<int64_t>(row) > header.nrows) {
                     throw invalid_mm("Row index out of bounds");
                 }
                 if (col <= 0 || static_cast<int64_t>(col) > header.ncols) {
                     throw invalid_mm("Column index out of bounds");
                 }
 
+                // Matrix Market is one-based
+                row = row - 1;
+                col = col - 1;
+
                 // Generalize symmetry
                 // This appears before the regular handler call for ExtraZeroElement handling.
                 if (header.symmetry != general && options.generalize_symmetry) {
-                    if (col != row) {
-                        switch (header.symmetry) {
-                            case symmetric:
-                                handler.handle(col - 1, row - 1, value);
-                                break;
-                            case skew_symmetric:
-                                if constexpr (!std::is_unsigned_v<typename HANDLER::value_type>) {
-                                    handler.handle(col - 1, row - 1, negate(value));
-                                } else {
-                                    throw invalid_argument("Cannot load skew-symmetric matrix into unsigned value type.");
-                                }
-                                break;
-                            case hermitian:
-                                handler.handle(col - 1, row - 1, complex_conjugate(value));
-                                break;
-                            case general: break;
-                        }
+                    if (header.field != pattern) {
+                        generalize_symmetry_coordinate(handler, header, options, row, col, value);
                     } else {
-                        if (!test_flag(HANDLER::flags, kAppending)) {
-                            switch (options.generalize_coordinate_diagnonal_values) {
-                                case read_options::ExtraZeroElement:
-                                    handler.handle(row - 1, col - 1, get_zero<typename HANDLER::value_type>());
-                                    break;
-                                case read_options::DuplicateElement:
-                                    handler.handle(row - 1, col - 1, value);
-                                    break;
-                            }
-                        }
+                        generalize_symmetry_coordinate(handler, header, options, row, col, pattern_placeholder_type());
                     }
                 }
 
-                // Matrix Market is one-based
-                handler.handle(row - 1, col - 1, value);
+                if (header.field != pattern) {
+                    handler.handle(row, col, value);
+                } else {
+                    handler.handle(row, col, pattern_placeholder_type());
+                }
 
                 ++line.file_line;
                 ++line.element_num;
             } catch (invalid_mm& inv) {
                 inv.prepend_line_number(line.file_line + 1);
                 throw;
             }
         }
         return line;
     }
 
+#ifndef FMM_NO_VECTOR
     template<typename HANDLER>
     line_counts read_chunk_vector_coordinate(const std::string &chunk, const matrix_market_header &header,
                                              line_counts line, HANDLER &handler, const read_options &options) {
         const char *pos = chunk.c_str();
         const char *end = pos + chunk.size();
 
         while (pos != end) {
@@ -188,35 +274,44 @@
                     // empty line
                     break;
                 }
                 if (line.element_num >= header.nnz) {
                     throw invalid_mm("Too many lines in file (file too long)");
                 }
                 pos = read_int(pos, end, row);
-                pos = skip_spaces(pos);
-                pos = read_value(pos, end, value, options);
+                if (header.field != pattern) {
+                    pos = skip_spaces(pos);
+                    read_real_or_complex(value, pos, end, header, options);
+                }
                 pos = bump_to_next_line(pos, end);
 
                 // validate
                 if (row <= 0 || static_cast<int64_t>(row) > header.vector_length) {
                     throw invalid_mm("Vector index out of bounds");
                 }
 
                 // Matrix Market is one-based
-                handler.handle(row - 1, 0, value);
+                row = row - 1;
+
+                if (header.field != pattern) {
+                    handler.handle(row, 0, value);
+                } else {
+                    handler.handle(row, 0, pattern_placeholder_type());
+                }
 
                 ++line.file_line;
                 ++line.element_num;
             } catch (invalid_mm& inv) {
                 inv.prepend_line_number(line.file_line + 1);
                 throw;
             }
         }
         return line;
     }
+#endif
 
     template<typename HANDLER>
     line_counts read_chunk_array(const std::string &chunk, const matrix_market_header &header, line_counts line,
                                  HANDLER &handler, const read_options &options,
                                  typename HANDLER::coordinate_type &row,
                                  typename HANDLER::coordinate_type &col) {
         const char *pos = chunk.c_str();
@@ -241,37 +336,21 @@
                     // empty line
                     break;
                 }
                 if (static_cast<int64_t>(col) >= header.ncols) {
                     throw invalid_mm("Too many values in array (file too long)");
                 }
 
-                pos = read_value(pos, end, value, options);
+                read_real_or_complex(value, pos, end, header, options);
                 pos = bump_to_next_line(pos, end);
 
                 handler.handle(row, col, value);
 
                 if (row != col && options.generalize_symmetry) {
-                    switch (header.symmetry) {
-                        case symmetric:
-                            handler.handle(col, row, value);
-                            break;
-                        case skew_symmetric:
-                            if constexpr (!std::is_unsigned_v<typename HANDLER::value_type>) {
-                                handler.handle(col, row, negate(value));
-                            } else {
-                                throw invalid_argument("Cannot load skew-symmetric matrix into unsigned value type.");
-                            }
-                            break;
-                        case hermitian:
-                            handler.handle(col, row, complex_conjugate(value));
-                            break;
-                        case general:
-                            break;
-                    }
+                    generalize_symmetry_array(handler, header, row, col, value);
                 }
 
                 // Matrix Market is column-major, advance down the column
                 ++row;
                 if (static_cast<int64_t>(row) == header.nrows) {
                     ++col;
                     if (header.symmetry == general) {
@@ -319,15 +398,19 @@
         while (instream.good()) {
             std::string chunk = get_next_chunk(instream, options);
 
             // parse the chunk
             if (header.object == matrix) {
                 lc = read_chunk_matrix_coordinate(chunk, header, lc, handler, options);
             } else {
+#ifdef FMM_NO_VECTOR
+                throw no_vector_support("Vector Matrix Market files not supported.");
+#else
                 lc = read_chunk_vector_coordinate(chunk, header, lc, handler, options);
+#endif
             }
         }
 
         return lc;
     }
 
     template <typename HANDLER>
@@ -349,24 +432,34 @@
 
         return lc;
     }
 
     /**
      * Read the body with no automatic adaptations.
      */
-    template <typename HANDLER>
+    template <typename HANDLER, compile_format FORMAT = compile_all>
     void read_matrix_market_body_no_adapters(std::istream& instream, const matrix_market_header& header,
                                              HANDLER& handler, const read_options& options = {}) {
+#ifdef FMM_NO_VECTOR
+        if (header.object == vector) {
+            throw no_vector_support("Vector Matrix Market files not supported.");
+        }
+#endif
+
         // Verify generalize symmetry is compatible with this file.
         if (header.symmetry != general && options.generalize_symmetry) {
             if (header.object != matrix) {
                 throw invalid_mm("Invalid Symmetry: vectors cannot have symmetry. Set generalize_symmetry=false to disregard this symmetry.");
             }
         }
 
+        if (header.format == array && header.field == pattern) {
+            throw invalid_mm("Array matrices may not be pattern.");
+        }
+
         line_counts lc;
         bool threads = options.parallel_ok && options.num_threads != 1 && test_flag(HANDLER::flags, kParallelOk);
 
         threads = limit_parallelism_for_value_type<typename HANDLER::value_type>(threads);
 
         if (header.symmetry != general && header.format == array) {
             // Parallel array loader does not handle symmetry
@@ -375,75 +468,90 @@
 
         if (header.format == coordinate && test_flag(HANDLER::flags, kDense)) {
             // Potential race condition if the file contains duplicates.
             threads = false;
         }
 
         if (threads) {
-            lc = read_body_threads(instream, header, handler, options);
+            lc = read_body_threads<HANDLER, FORMAT>(instream, header, handler, options);
         } else {
             if (header.format == coordinate) {
-                lc = read_coordinate_body_sequential(instream, header, handler, options);
+                if constexpr ((FORMAT & compile_coordinate_only) == compile_coordinate_only) {
+                    lc = read_coordinate_body_sequential(instream, header, handler, options);
+                } else {
+                    throw support_not_selected("Matrix is coordinate but reading coordinate files not enabled for this method.");
+                }
             } else {
-                lc = read_array_body_sequential(instream, header, handler, options);
+                if constexpr ((FORMAT & compile_array_only) == compile_array_only) {
+                    lc = read_array_body_sequential(instream, header, handler, options);
+                } else {
+                    throw support_not_selected("Matrix is array but reading array files not enabled for this method.");
+                }
             }
         }
 
         // verify the file is not truncated
         if (lc.element_num < header.nnz) {
             if (!(header.symmetry != general && header.format == array)) {
                 throw invalid_mm(std::string("Truncated file. Expected another ") +
                                  std::to_string(header.nnz - lc.element_num) + " lines.");
             }
         }
     }
 
+#ifndef FMM_SCIPY_PRUNE
     /**
      * Read the body by adapting real files to complex HANDLER.
+     *
+     * @deprecated Use read_matrix_market_body_no_adapters() directly. It now handles the adaptation that this method does.
      */
     template <typename HANDLER, typename std::enable_if<is_complex<typename HANDLER::value_type>::value, int>::type = 0>
-    void read_matrix_market_body_no_pattern(std::istream& instream, const matrix_market_header& header,
+    [[deprecated]] [[maybe_unused]] void read_matrix_market_body_no_pattern(std::istream& instream, const matrix_market_header& header,
                                             HANDLER& handler, const read_options& options = {}) {
         if (header.field == complex) {
             read_matrix_market_body_no_adapters(instream, header, handler, options);
         } else {
             // the handler is expecting std::complex values, but the file is only integer/real
             // provide adapter
             auto fwd_handler = complex_parse_adapter<HANDLER>(handler);
             read_matrix_market_body_no_adapters(instream, header, fwd_handler, options);
         }
     }
 
     /**
      * Read the body by adapting real files to complex HANDLER.
+     *
+     * @deprecated Use read_matrix_market_body_no_adapters() directly. It now handles the adaptation that this method does.
      */
     template <typename HANDLER, typename std::enable_if<!is_complex<typename HANDLER::value_type>::value, int>::type = 0>
-    void read_matrix_market_body_no_pattern(std::istream& instream, const matrix_market_header& header,
+    [[deprecated]] [[maybe_unused]] void read_matrix_market_body_no_pattern(std::istream& instream, const matrix_market_header& header,
                                             HANDLER& handler, const read_options& options = {}) {
         if (header.field != complex) {
             read_matrix_market_body_no_adapters(instream, header, handler, options);
         } else {
             // the file is complex but the values are not
             throw complex_incompatible("Matrix Market file has complex fields but passed data structure cannot handle complex values.");
         }
     }
+#endif
 
     /**
      * Main body reader entry point.
      *
      * This will handle the following adaptations automatically:
      *  - If the file is a pattern file, the pattern_value will be substituted for each element
      *  - If the HANDLER expects std::complex values but the file is not complex then imag=0 is provided for each value.
      */
-    template <typename HANDLER>
+    template <typename HANDLER, compile_format FORMAT = compile_all>
     void read_matrix_market_body(std::istream& instream, const matrix_market_header& header,
                                  HANDLER& handler,
                                  typename HANDLER::value_type pattern_value,
                                  const read_options& options = {}) {
-        if (header.field == pattern) {
-            auto fwd_handler = pattern_parse_adapter<HANDLER>(handler, pattern_value);
-            read_matrix_market_body_no_pattern(instream, header, fwd_handler, options);
-        } else {
-            read_matrix_market_body_no_pattern(instream, header, handler, options);
+        if (header.field == complex && !is_complex<typename HANDLER::value_type>::value) {
+            // the file is complex but the values are not
+            throw complex_incompatible("Matrix Market file has complex fields but passed data structure cannot handle complex values.");
         }
+
+        auto fwd_handler = pattern_parse_adapter<HANDLER>(handler, pattern_value);
+        read_matrix_market_body_no_adapters<decltype(fwd_handler), FORMAT>(instream, header, fwd_handler, options);
     }
 }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -4,125 +4,157 @@
 
 #pragma once
 
 #include <future>
 #include <queue>
 
 #include "fast_matrix_market.hpp"
-#include "thirdparty//task_thread_pool.hpp"
+#include "thirdparty/task_thread_pool.hpp"
 
 namespace fast_matrix_market {
 
-    struct line_count_result {
+    struct line_count_result_s {
         std::string chunk;
         line_counts counts;
+
+        explicit line_count_result_s(std::string && c): chunk(c) {}
     };
 
+    using line_count_result = std::shared_ptr<line_count_result_s>;
+
     inline line_count_result count_chunk_lines(line_count_result lcr) {
-        auto [lines, empties] = count_lines(lcr.chunk);
+        auto [lines, empties] = count_lines(lcr->chunk);
 
-        lcr.counts.file_line = lines;
-        lcr.counts.element_num = lines - empties;
+        lcr->counts.file_line = lines;
+        lcr->counts.element_num = lines - empties;
         return lcr;
     }
 
-    template <typename HANDLER>
+    template <typename HANDLER, compile_format FORMAT = compile_all>
     line_counts read_body_threads(std::istream& instream, const matrix_market_header& header,
                                   HANDLER& handler, const read_options& options = {}) {
         /*
          * Pipeline:
          * 1. Read chunk
          * 2. Calculate chunk's line count
          * 3. Parse chunk.
          *
          * The line count is needed for
          * 1. for array files the line number determines the row/column indices of the value
          * 2. for coordinate files the line number determines the chunk's offset into the result arrays
          * 3. for error messages
          *
-         * We do the I/O reading only in the main thread. Everything else is done by tasks in a thread pool.
+         * Only the main threads performs I/O reads. Everything else is done by tasks in a thread pool.
          *
          * The line count is fast, but we still spawn line count tasks. The futures for these tasks are saved in a
-         * queue so they can be retrieved in order. This way we can easily keep track of the line number of each chunk.
+         * queue to be retrieved in order. This enables easy tracking of the line numbers of each chunk.
          *
-         * Once a line count is complete we spawn a task to parse this chunk. We also then read another chunk from
-         * the input stream.
+         * Once a chunk's line count is complete we spawn a task to parse it. We also then read another chunk from
+         * the input stream and start its line count.
          *
          * The line count step is significantly faster than the parse step. As a form of backpressure we don't read
          * additional chunks if there are too many inflight chunks.
          */
         line_counts lc{header.header_line_count, 0};
 
         std::queue<std::future<line_count_result>> line_count_futures;
-        std::queue<std::future<void>> parse_futures;
+        std::queue<std::future<line_count_result>> parse_futures;
         task_thread_pool::task_thread_pool pool(options.num_threads);
 
+        // Reuse the line_count_result objects. Each chunk would otherwise allocate a new 1MB std::string.
+        // The lifetime of these strings is relatively short, but some allocators do not immediately reuse the memory.
+        // This object pool can reduce overall RSS memory usage in many cases.
+        std::queue<line_count_result> lcr_reuse_pool;
+
         int generalizing_symmetry_factor = (header.symmetry != general && options.generalize_symmetry) ? 2 : 1;
 
         // Number of concurrent chunks available to work on.
         // Too few may starve workers (such as due to uneven chunk splits)
         // Too many increases costs, such as storing chunk results in memory before they're written.
-        const unsigned inflight_count = 5 * pool.get_num_threads();
+        const unsigned inflight_count = pool.get_num_threads() + 1;
 
         // Start reading chunks and counting lines.
         for (unsigned seed_i = 0; seed_i < inflight_count && instream.good(); ++seed_i) {
-            line_count_result lcr;
-            lcr.chunk = get_next_chunk(instream, options);
-
+            line_count_result lcr = std::make_shared<line_count_result_s>(get_next_chunk(instream, options));
             line_count_futures.push(pool.submit(count_chunk_lines, lcr));
         }
 
         // Read chunks in order, as they become available.
         while (!line_count_futures.empty()) {
 
             // Wait on any parse results. This serves as backpressure.
             while (!parse_futures.empty() && (is_ready(parse_futures.front()) || parse_futures.size() > inflight_count)) {
                 // This will throw any parse errors.
-                parse_futures.front().get();
+                auto lcr_to_reuse = parse_futures.front().get();
                 parse_futures.pop();
+
+                // save the lcr struct to reuse the memory
+                lcr_reuse_pool.push(lcr_to_reuse);
             }
 
             // We are ready to start another parse task.
             line_count_result lcr = line_count_futures.front().get();
             line_count_futures.pop();
 
             // Next chunk has finished line count. Start another to replace it.
             if (instream.good()) {
-                line_count_result new_lcr;
-                new_lcr.chunk = get_next_chunk(instream, options);
+                line_count_result lcr_reuse;
+                // attempt to reuse the chunk string object from a previous chunk
+                if (lcr_reuse_pool.empty()) {
+                    lcr_reuse = std::make_shared<line_count_result_s>("");
+                } else {
+                    lcr_reuse = lcr_reuse_pool.front();
+                    lcr_reuse_pool.pop();
+                }
 
-                line_count_futures.push(pool.submit(count_chunk_lines, new_lcr));
+                get_next_chunk(lcr_reuse->chunk, instream, options);
+                line_count_futures.push(pool.submit(count_chunk_lines, lcr_reuse));
             }
 
             // Parse it.
             if (lc.element_num > header.nnz) {
                 throw invalid_mm("File too long", lc.file_line + 1);
             }
             auto chunk_handler = handler.get_chunk_handler(lc.element_num * generalizing_symmetry_factor);
             if (header.format == array) {
-                // compute the starting row/column for this array chunk
-                typename HANDLER::coordinate_type row = lc.element_num % header.nrows;
-                typename HANDLER::coordinate_type col = lc.element_num / header.nrows;
-
-                parse_futures.push(pool.submit([=]() mutable {
-                    read_chunk_array(lcr.chunk, header, lc, chunk_handler, options, row, col);
-                }));
+                if constexpr ((FORMAT & compile_array_only) == compile_array_only) {
+                    // compute the starting row/column for this array chunk
+                    typename HANDLER::coordinate_type row = lc.element_num % header.nrows;
+                    typename HANDLER::coordinate_type col = lc.element_num / header.nrows;
+
+                    parse_futures.push(pool.submit([=]() mutable {
+                        read_chunk_array(lcr->chunk, header, lc, chunk_handler, options, row, col);
+                        return lcr;
+                    }));
+                } else {
+                    throw support_not_selected("Matrix is array but reading array files not enabled for this method.");
+                }
             } else if (header.object == matrix) {
-                parse_futures.push(pool.submit([=]() mutable {
-                    read_chunk_matrix_coordinate(lcr.chunk, header, lc, chunk_handler, options);
-                }));
+                if constexpr ((FORMAT & compile_coordinate_only) == compile_coordinate_only) {
+                    parse_futures.push(pool.submit([=]() mutable {
+                        read_chunk_matrix_coordinate(lcr->chunk, header, lc, chunk_handler, options);
+                        return lcr;
+                    }));
+                } else {
+                    throw support_not_selected("Matrix is coordinate but reading coordinate files not enabled for this method.");
+                }
             } else {
+#ifdef FMM_NO_VECTOR
+                throw no_vector_support("Vector Matrix Market files not supported.");
+#else
                 parse_futures.push(pool.submit([=]() mutable {
-                    read_chunk_vector_coordinate(lcr.chunk, header, lc, chunk_handler, options);
+                    read_chunk_vector_coordinate(lcr->chunk, header, lc, chunk_handler, options);
+                    return lcr;
                 }));
+#endif
             }
 
             // Advance counts for next chunk
-            lc.file_line += lcr.counts.file_line;
-            lc.element_num += lcr.counts.element_num;
+            lc.file_line += lcr->counts.file_line;
+            lc.element_num += lcr->counts.element_num;
         }
 
         // Wait on any parse results. This will throw any parse errors.
         while (!parse_futures.empty()) {
             parse_futures.front().get();
             parse_futures.pop();
         }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/thirdparty/task_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/types.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/types.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,15 @@
          *
          *  This value is ignored if the parse handler has the kAppending flag set. In that case only a single
          *  diagonal element is emitted.
          */
         enum {ExtraZeroElement, DuplicateElement} generalize_coordinate_diagnonal_values = ExtraZeroElement;
 
         /**
-         * Whether or not parallel implementation is allowed.
+         * Whether parallel implementation is allowed.
          */
         bool parallel_ok = true;
 
         /**
          * Number of threads to use. 0 means std::thread::hardware_concurrency().
          */
         int num_threads = 0;
@@ -120,23 +120,28 @@
         out_of_range_behavior float_out_of_range_behavior = BestMatch;
     };
 
     struct write_options {
         int64_t chunk_size_values = 2 << 12;
 
         /**
-         * Whether or not parallel implementation is allowed.
+         * Whether parallel implementation is allowed.
          */
         bool parallel_ok = true;
 
         /**
          * Number of threads to use. 0 means std::thread::hardware_concurrency().
          */
         int num_threads = 0;
 
         /**
          * Floating-point formatting precision.
          * Placeholder. Currently not used due to the various supported float rendering backends.
          */
         int precision = -1;
+
+        /**
+         * Whether to always write a comment line even if comment is empty.
+         */
+        bool always_comment = false;
     };
 }
```

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp` & `fast-matrix-market-1.7.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // SPDX-License-Identifier: BSD-2-Clause
 
 #pragma once
 
 #include <queue>
 
 #include "fast_matrix_market.hpp"
-#include "thirdparty//task_thread_pool.hpp"
+#include "thirdparty/task_thread_pool.hpp"
 
 namespace fast_matrix_market {
     /**
      * Write Matrix Market body.
      *
      * Chunk based so that it can be made parallel. Each chunk is written by a FORMATTER class.
      * @tparam FORMATTER implementation class that writes chunks.
@@ -35,29 +35,31 @@
          */
         std::queue<std::future<std::string>> futures;
         task_thread_pool::task_thread_pool pool(options.num_threads);
 
         // Number of concurrent chunks available to work on.
         // Too few may starve workers (such as due to uneven chunk splits)
         // Too many increases costs, such as storing chunk results in memory before they're written.
-        const int inflight_count = 5 * (int)pool.get_num_threads();
+        const int inflight_count = 2 * (int)pool.get_num_threads();
 
         // Start computing tasks.
         for (int batch_i = 0; batch_i < inflight_count && formatter.has_next(); ++batch_i) {
-            futures.push(pool.submit(formatter.next_chunk(options)));
+            // Could push the chunk directly, but MSVC.
+            futures.push(pool.submit([](auto chunk){ return chunk(); }, formatter.next_chunk(options)));
+//            futures.push(pool.submit(formatter.next_chunk(options)));
         }
 
         // Write chunks in order as they become available.
         while (!futures.empty()) {
             std::string chunk = futures.front().get();
             futures.pop();
 
             // Next chunk is ready. Start another to replace it.
             if (formatter.has_next()) {
-                futures.push(pool.submit(formatter.next_chunk(options)));
+                futures.push(pool.submit([](auto chunk){ return chunk(); }, formatter.next_chunk(options)));
             }
 
             // Write this one out.
             os.write(chunk.c_str(), (std::streamsize) chunk.size());
         }
     }
 }
```

### Comparing `fast-matrix-market-1.6.0/pyproject.toml` & `fast-matrix-market-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "fast_matrix_market"
-version = "1.6.0"
+version = "1.7.0"
 description="Fast and full-featured Matrix Market file I/O"
 readme = "README.md"
 authors = [
     { name = "Adam Lugowski"},
 ]
 requires-python = ">=3.7"
```

### Comparing `fast-matrix-market-1.6.0/src/fast_matrix_market/__init__.py` & `fast-matrix-market-1.7.0/src/fast_matrix_market/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,40 +5,48 @@
 Read and write Matrix Market files.
 
 Supports sparse coo/triplet matrices, sparse scipy matrices, and numpy array dense matrices.
 """
 import io
 import os
 
-from . import _core
-from ._core import __version__, header
+from . import _core  # type: ignore
+
+__version__ = _core.__version__
+header = _core.header
+
+__all__ = [
+    "read_header", "write_header",
+    "read_array", "write_array", "read_coo", "write_coo", "read_array_or_coo",
+    "mminfo", "mmread", "mmwrite", "read_scipy", "write_scipy"]
 
 PARALLELISM = 0
 """
-Number of threads to use. 0 means number of CPUs in the system.
+Default value for the parallelism argument to mmread() and mmwrite().
+0 means number of CPUs in the system.
 """
 
 ALWAYS_FIND_SYMMETRY = False
 """
-If True then equivalent to always passing find_symmetry=True to mmwrite().
-This matches scipy.io.mmwrite()'s behavior, as well as its performance cost.
+Whether mmwrite() with symmetry='AUTO' will always search for symmetry inside the matrix.
+This is scipy.io._mmio.mmwrite()'s default behavior, but has a significant performance cost on large matrices.
 """
 
 _field_to_dtype = {
     "integer": "int64",
     "unsigned-integer": "uint64",
     "real": "float64",
     "complex": "complex",
     "pattern": "float64",
 
     "long-integer": "int64",
     "long-unsigned-integer": "uint64",
     "long-real": "longdouble",
     "long-complex": "longcomplex",
-    "long-pattern": "float64",
+    "long-pattern": "longdouble",
 }
 
 
 class _TextToBytesWrapper(io.BufferedReader):
     """
     Convert a TextIOBase string stream to a byte stream.
     """
@@ -62,27 +70,40 @@
 
     def read1(self, size=-1):
         return self._encoding_call('read1', size)
 
     def peek(self, size=-1):
         return self._encoding_call('peek', size)
 
+    def seek(self, offset, whence=0):
+        # Random seeks are not allowed because of non-trivial conversion between byte and character offsets,
+        # with the possibility of a byte offset landing within a character.
+        if offset == 0 and whence == 0 or \
+           offset == 0 and whence == 2:
+            # seek to start or end is ok
+            super(_TextToBytesWrapper, self).seek(offset, whence)
+        else:
+            # Drop any other seek
+            # In this application this may happen when pystreambuf seeks during sync(), which can happen when closing
+            # a partially-read stream. Ex. when mminfo() only reads the header then exits.
+            pass
+
 
 def _read_body_array(cursor, long_type):
     import numpy as np
     vals = np.zeros(cursor.header.shape, dtype=_field_to_dtype.get(("long-" if long_type else "")+cursor.header.field))
     _core.read_body_array(cursor, vals)
     return vals
 
 
 def _read_body_coo(cursor, long_type, generalize_symmetry=True):
     import numpy as np
 
-    index_dtype = "int32"  # SciPy uses this size
-    if cursor.header.nrows > 2**31 or cursor.header.ncols > 2**31:
+    index_dtype = "int32"
+    if cursor.header.nrows >= 2**31 or cursor.header.ncols >= 2**31:
         # Dimensions are too large to fit in int32
         index_dtype = "int64"
 
     i = np.zeros(cursor.header.nnz, dtype=index_dtype)
     j = np.zeros(cursor.header.nnz, dtype=index_dtype)
     data = np.zeros(cursor.header.nnz, dtype=_field_to_dtype.get(("long-" if long_type else "")+cursor.header.field))
 
@@ -120,15 +141,15 @@
     except TypeError:
         is_path = False
 
     if is_path:
         path = str(source)
         if path.endswith('.gz'):
             import gzip
-            source = gzip.open(path, 'r')
+            source = gzip.GzipFile(path, 'r')
         elif path.endswith('.bz2'):
             import bz2
             source = bz2.BZ2File(path, 'rb')
         else:
             return _core.open_read_file(path, parallelism)
 
     # Stream object.
@@ -161,14 +182,16 @@
         # It's a file path
         return _core.open_write_file(str(target), h, parallelism, precision)
     except TypeError:
         pass
 
     if hasattr(target, "write"):
         # Stream object.
+        if isinstance(target, io.TextIOBase):
+            raise TypeError("target stream must be open in binary mode")
         return _core.open_write_stream(target, h, parallelism, precision)
     else:
         raise TypeError("Unknown source object")
 
 
 def _apply_field(data, field, no_pattern=False):
     """
@@ -184,15 +207,14 @@
         return data
     if field == "pattern":
         if no_pattern:
             return data
         else:
             return np.zeros(0)
 
-    import numpy as np
     dtype = _field_to_dtype.get(field, None)
     if dtype is None:
         raise ValueError("Invalid field.")
 
     return np.asarray(data, dtype=dtype)
 
 
@@ -249,16 +271,15 @@
 
 def read_array(source, parallelism=None, long_type=False):
     """
     Read MatrixMarket file into dense NumPy Array, regardless if the file is sparse or dense.
 
     :param source: path to MatrixMarket file or open file-like object
     :param parallelism: number of threads to use. 0 means auto.
-    :param long_type: Use long floating point datatypes (if available in your NumPy).
-    This means longdouble and longcomplex instead of float64 and complex64.
+    :param long_type: Whether to use 'longdouble' and 'longcomplex' extended-precision floating-point number types.
     :return: numpy array
     """
     return _read_body_array(_get_read_cursor(source, parallelism), long_type=long_type)
 
 
 def write_array(target, a, comment=None, parallelism=None):
     """
@@ -268,25 +289,24 @@
     :param a: convertible to a Numpy array.
     :param comment: comment to include in the MatrixMarket header
     :param parallelism: number of threads to use, None means auto.
     """
     import numpy as np
     a = np.asarray(a)
     cursor = _get_write_cursor(target, comment=comment, parallelism=parallelism)
-    _core.write_array(cursor, a)
+    _core.write_body_array(cursor, a)
 
 
 def read_coo(source, parallelism=None, long_type=False, generalize_symmetry=True):
     """
     Read MatrixMarket file to a (data, (i, j)) triplet, regardless if the file is sparse or dense.
 
     :param source: path to MatrixMarket file or open file-like object
     :param parallelism: number of threads to use. 0 means auto.
-    :param long_type: Use long floating point datatypes (if available in your NumPy).
-    This means longdouble and longcomplex instead of float64 and complex64.
+    :param long_type: Whether to use 'longdouble' and 'longcomplex' extended-precision floating-point number types.
     :param generalize_symmetry: if the MatrixMarket file specifies a symmetry, emit the symmetric entries too.
     :return: (data, (row_indices, column_indices)) (same as scipy.io.mmread)
     """
     (data, (rows, cols)), shape = _read_body_coo(_get_read_cursor(source, parallelism),
                                                  long_type=long_type, generalize_symmetry=generalize_symmetry)
     return (data, (rows, cols)), shape
 
@@ -304,27 +324,26 @@
     if len(shape) != 2:
         raise ValueError("shape needs to be: (# of rows, # of columns)")
 
     # unpack a
     data, (row, col) = a
 
     cursor = _get_write_cursor(target, comment=comment, parallelism=parallelism)
-    _core.write_coo(cursor, shape, row, col, data)
+    _core.write_body_coo(cursor, shape, row, col, data)
 
 
 def read_array_or_coo(source, parallelism=None, long_type=False, generalize_symmetry=True):
     """
     Read MatrixMarket file. If the file is dense, return a 2D numpy array. Else return a coordinate matrix.
 
     This is the same as read_array() if the file is dense, and read_coo() if the file is sparse.
 
     :param source: path to MatrixMarket file or open file-like object
     :param parallelism: number of threads to use. 0 means auto.
-    :param long_type: Use long floating point datatypes (if available in your NumPy).
-    This means longdouble and longcomplex instead of float64 and complex64.
+    :param long_type: Whether to use 'longdouble' and 'longcomplex' extended-precision floating-point number types.
     :param generalize_symmetry: if the MatrixMarket file specifies a symmetry, emit the symmetric entries too.
     Always True for dense files.
     :return: a tuple of (matrix, shape), where matrix is an ndarray if the MatrixMarket file is dense,
     a triplet tuple if the MatrixMarket file is sparse.
     """
     cursor = _get_read_cursor(source, parallelism)
 
@@ -341,68 +360,73 @@
     """
     Read MatrixMarket file. If the file is dense, return a 2D numpy array. Else return a SciPy sparse matrix.
 
     Interchangeable with scipy.io.mmread() but faster and supports longdouble.
 
     :param source: path to MatrixMarket file or open file-like object
     :param parallelism: number of threads to use. 0 means auto.
-    :param long_type: Use long floating point datatypes (if available in your NumPy).
-    This means longdouble and longcomplex instead of float64 and complex64.
+    :param long_type: Whether to use 'longdouble' and 'longcomplex' extended-precision floating-point number types.
     :return: an ndarray if the MatrixMarket file is dense, a scipy.sparse.coo_matrix if the MatrixMarket file is sparse.
     """
     cursor = _get_read_cursor(source, parallelism)
 
     if cursor.header.format == "array":
         return _read_body_array(cursor, long_type=long_type)
     else:
         from scipy.sparse import coo_matrix
         triplet, shape = _read_body_coo(cursor, long_type=long_type, generalize_symmetry=True)
         return coo_matrix(triplet, shape=shape)
 
 
-def mmwrite(target, a, comment=None, field=None, precision=None, symmetry=None,
+def mmwrite(target, a, comment=None, field=None, precision=None, symmetry="AUTO",
                 parallelism=None, find_symmetry=False):
     """
     Write a matrix to a MatrixMarket file or file-like object.
 
     Interchangeable with scipy.io.mmwrite() but faster.
 
     :param target: path to MatrixMarket file or open file-like object
     :param a: a 2D ndarray (or an array convertible to one) or a scipy.sparse matrix
     :param comment: comment to include in the MatrixMarket header
-    :param field: convert matrix values to this MatrixMarket field
-    :param precision: floating-point precision to use. If None then use shortest representation.
-    :param symmetry: if not None then the matrix is written as having this MatrixMarket symmetry. "pattern" means write
+    :param field: convert matrix values to this MatrixMarket field. "pattern" means write
     only the nonzero structure and no values.
+    :param precision: floating-point precision to use. If None then use shortest representation.
+    :param symmetry: if not None then the matrix is written as having this MatrixMarket symmetry.
     :param parallelism: number of threads to use. 0 means auto.
     :param find_symmetry: autodetect what symmetry the matrix contains and set the `symmetry` field accordingly. This
     can be slow. scipy.io.mmwrite always does this if symmetry is not set, but it is very slow on large matrices.
     """
     import numpy as np
     import scipy.sparse
 
-    if isinstance(a, list) or isinstance(a, tuple) or hasattr(a, '__array__'):
+    if isinstance(a, list) or isinstance(a, tuple) or hasattr(a, "__array__"):
         a = np.asarray(a)
 
-    if ALWAYS_FIND_SYMMETRY or find_symmetry:
+    if symmetry == "AUTO":
+        if ALWAYS_FIND_SYMMETRY or (hasattr(a, "shape") and max(a.shape) < 100):
+            symmetry = None
+        else:
+            symmetry = "general"
+
+    if symmetry is None or find_symmetry:
         # Attempt to use scipy's method for finding matrix symmetry
         import scipy.io
         try:
             # noinspection PyProtectedMember
             symmetry = scipy.io._mmio.MMFile()._get_symmetry(a)
         except AttributeError:
             symmetry = "general"
 
     symmetry = _validate_symmetry(symmetry)
     cursor = _get_write_cursor(target, comment=comment, parallelism=parallelism, precision=precision, symmetry=symmetry)
 
     if isinstance(a, np.ndarray):
         # Write dense numpy arrays
         a = _apply_field(a, field, no_pattern=True)
-        _core.write_array(cursor, a)
+        _core.write_body_array(cursor, a)
         return
 
     if scipy.sparse.isspmatrix(a):
         # Write sparse scipy matrices
         if symmetry is not None and symmetry != "general":
             # A symmetric matrix only specifies the elements below the diagonal.
             # Ensure that the matrix satisfies this requirement.
@@ -421,17 +445,17 @@
             a = a.tocoo()
 
         data = _apply_field(a.data, field)
 
         if is_compressed:
             # CSC and CSR can be written directly
             is_csr = isinstance(a, scipy.sparse.csr_matrix)
-            _core.write_csc(cursor, a.shape, a.indptr, a.indices, data, is_csr)
+            _core.write_body_csc(cursor, a.shape, a.indptr, a.indices, data, is_csr)
         else:
-            _core.write_coo(cursor, a.shape, a.row, a.col, data)
+            _core.write_body_coo(cursor, a.shape, a.row, a.col, data)
         return
 
     raise ValueError("unknown matrix type: %s" % type(a))
 
 
 def mminfo(source):
     """
```

### Comparing `fast-matrix-market-1.6.0/src/fast_matrix_market/pystreambuf.h` & `fast-matrix-market-1.7.0/src/fast_matrix_market/pystreambuf.h`

 * *Files 4% similar despite different names*

```diff
@@ -260,16 +260,25 @@
     virtual int_type overflow(int_type c=traits_type::eof()) {
       if (py_write.is_none()) {
         throw std::invalid_argument(
           "That Python file object has no 'write' attribute");
       }
       farthest_pptr = (std::max)(farthest_pptr, pptr());
       off_type n_written = (off_type)(farthest_pptr - pbase());
-      py::bytes chunk(pbase(), n_written);
-      py_write(chunk);
+
+      // Write all outstanding bytes. Write in chunks to support 32-bit systems.
+      // The py::bytes constructor insists that sizeof(second argument) <= sizeof(ssize_t)
+      // This is an issue on 32-bit systems where off_type may be long long but ssize_t is an int.
+      for (off_type offset = 0; offset < n_written; ) {
+        off_type chunk_len = std::min((n_written - offset), (off_type)(1 << 25));
+        py::bytes chunk(pbase() + offset, (int)chunk_len);
+        py_write(chunk);
+        offset += chunk_len;
+      }
+
       if (!traits_type::eq_int_type(c, traits_type::eof())) {
         char cs = traits_type::to_char_type(c);
         py_write(py::bytes(&cs, 1));
         n_written++;
       }
       if (n_written) {
         pos_of_write_buffer_end_in_py_file += n_written;
@@ -526,14 +535,17 @@
     }
   }
 };
 
 };
 
 namespace pybind11 { namespace detail {
+    // Wrapping the stream objects with std::shared_ptr so that the streams can be used between API calls.
+    // This enables one API call to open the stream and a follow-up call to read/write to it, with the stream
+    // reference kept in C++.
     template <> struct type_caster<std::shared_ptr<pystream::istream>> {
     public:
         bool load(handle src, bool) {
             if (getattr(src, "read", py::none()).is_none()){
               return false;
             }
```

### Comparing `fast-matrix-market-1.6.0/tests/test_array.py` & `fast-matrix-market-1.7.0/tests/test_array.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
 # SPDX-License-Identifier: BSD-2-Clause
 
 from io import BytesIO, StringIO
 from pathlib import Path
+
 import numpy as np
 import unittest
 import scipy
-import sys
 
 import fast_matrix_market as fmm
 
 matrices = Path("matrices")
-IS_PYPY = "PyPy" in sys.version
+
+try:
+    import bz2
+    HAVE_BZ2 = True
+except ImportError:
+    HAVE_BZ2 = False
 
 
 class TestArray(unittest.TestCase):
     def assertMatrixEqual(self, lhs, rhs, types=True):
         """
         Assert dense numpy matrices are equal.
         """
         self.assertEqual(lhs.shape, rhs.shape)
         self.assertEqual(type(lhs), type(rhs))
         if types:
+            if np.dtype('intp') == np.dtype('int32'):
+                # 32-bit system. scipy.io._mmio will load integer arrays as int32
+                if lhs.dtype == np.dtype('int32'):
+                    lhs = lhs.astype('int64')
+                if rhs.dtype == np.dtype('int32'):
+                    rhs = rhs.astype('int64')
             self.assertEqual(lhs.dtype, rhs.dtype)
         np.testing.assert_almost_equal(lhs, rhs)
 
     def test_read(self):
         for mtx in sorted(list(matrices.glob("*.mtx*"))):
+            if str(mtx).endswith(".bz2") and not HAVE_BZ2:
+                continue
             mtx_header = fmm.read_header(mtx)
             if mtx_header.format != "array":
                 continue
 
             with self.subTest(msg=mtx.stem):
                 m = scipy.io.mmread(mtx)
                 m_fmm = fmm.read_array(mtx)
                 self.assertMatrixEqual(m, m_fmm)
 
-    @unittest.skipIf(IS_PYPY, "Writing into BytesIO has no effect on PyPy")
     def test_write(self):
         for mtx in sorted(list(matrices.glob("*.mtx*"))):
+            if str(mtx).endswith(".bz2") and not HAVE_BZ2:
+                continue
             mtx_header = fmm.read_header(mtx)
             if mtx_header.format != "array":
                 continue
 
             with self.subTest(msg=mtx.stem):
                 m_fmm = fmm.read_array(mtx)
```

### Comparing `fast-matrix-market-1.6.0/tests/test_coo.py` & `fast-matrix-market-1.7.0/tests/test_coo.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,74 +3,85 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from io import BytesIO, StringIO
 from pathlib import Path
 import numpy as np
 import unittest
 import scipy
-import sys
 
 import fast_matrix_market as fmm
 
 matrices = Path("matrices")
-IS_PYPY = "PyPy" in sys.version
+
+try:
+    import bz2
+    HAVE_BZ2 = True
+except ImportError:
+    HAVE_BZ2 = False
 
 
 class TestTriplet(unittest.TestCase):
     def assertMatrixEqual(self, lhs, rhs, types=True):
         """
         Assert sparse triplet matrices are equal.
         """
         # Avoid failing on different ordering by using a CSC with sorted indices
         lhs_csc = lhs.tocsc().sorted_indices()
         rhs_csc = rhs.tocsc().sorted_indices()
 
         if types:
+            if np.dtype('intp') == np.dtype('int32'):
+                # 32-bit system. scipy.io._mmio will load integer arrays as int32
+                if lhs_csc.data.dtype == np.dtype('int32'):
+                    lhs_csc.data = lhs_csc.data.astype('int64')
+                if rhs_csc.data.dtype == np.dtype('int32'):
+                    rhs_csc.data = rhs_csc.data.astype('int64')
             self.assertEqual(lhs_csc.indptr.dtype, rhs_csc.indptr.dtype)
             self.assertEqual(lhs_csc.indices.dtype, rhs_csc.indices.dtype)
             self.assertEqual(lhs_csc.data.dtype, rhs_csc.data.dtype)
         np.testing.assert_almost_equal(lhs_csc.indptr, rhs_csc.indptr, err_msg="indptr")
         np.testing.assert_almost_equal(lhs_csc.indices, rhs_csc.indices, err_msg="indices")
         np.testing.assert_almost_equal(lhs_csc.data, rhs_csc.data, err_msg="data")
 
     def test_read(self):
         for mtx in sorted(list(matrices.glob("*.mtx*"))):
+            if str(mtx).endswith(".bz2") and not HAVE_BZ2:
+                continue
             mtx_header = fmm.read_header(mtx)
             if mtx_header.format != "coordinate":
                 continue
 
             with self.subTest(msg=mtx.stem):
                 m = scipy.io.mmread(mtx)
                 triplet, shape = fmm.read_coo(mtx)
                 fmm_scipy = scipy.sparse.coo_matrix(triplet, shape=shape)
                 self.assertMatrixEqual(m, fmm_scipy)
 
-    @unittest.skipIf(IS_PYPY, "Writing into BytesIO has no effect on PyPy")
     def test_write(self):
         for mtx in sorted(list(matrices.glob("*.mtx*"))):
+            if str(mtx).endswith(".bz2") and not HAVE_BZ2:
+                continue
             mtx_header = fmm.read_header(mtx)
             if mtx_header.format != "coordinate":
                 continue
 
             with self.subTest(msg=mtx.stem):
                 triplet, shape = fmm.read_coo(mtx)
-                print(triplet)
 
                 bio = BytesIO()
                 fmm.write_coo(bio, triplet, shape=shape)
                 fmms = bio.getvalue().decode()
 
                 triplet2, shape2 = fmm.read_coo(StringIO(fmms))
 
                 self.assertEqual(shape, shape2)
                 fmm_scipy = scipy.sparse.coo_matrix(triplet, shape=shape)
                 fmm_scipy2 = scipy.sparse.coo_matrix(triplet2, shape=shape2)
                 self.assertMatrixEqual(fmm_scipy, fmm_scipy2)
 
-    @unittest.skipIf(IS_PYPY, "Writing into BytesIO has no effect on PyPy")
     def test_list(self):
         i = [0, 1, 2]
         j = [0, 1, 2]
         data = [1, 1, 1]
 
         bio = BytesIO()
         fmm.write_coo(bio, (data, (i, j)), shape=(3, 3))
```

### Comparing `fast-matrix-market-1.6.0/tests/test_header.py` & `fast-matrix-market-1.7.0/tests/test_header.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # Copyright (C) 2022-2023 Adam Lugowski. All rights reserved.
 # Use of this source code is governed by the BSD 2-clause license found in the LICENSE.txt file.
 # SPDX-License-Identifier: BSD-2-Clause
 
 from io import BytesIO, StringIO
 import unittest
 from pathlib import Path
-import sys
 
 import fast_matrix_market as fmm
 
 matrices = Path("matrices")
 cpp_matrices = matrices / ".." / ".." / ".." / "tests" / "matrices"
-IS_PYPY = "PyPy" in sys.version
 
 
 class TestHeader(unittest.TestCase):
     def test_object(self):
         for value in ["matrix", "vector", "Matrix", "Vector"]:
             h = fmm.header(object=value)
             self.assertEqual(h.object, value.lower(), value)
@@ -51,25 +49,37 @@
             self.assertEqual(h.symmetry, value.lower(), value)
             h.symmetry = value
             self.assertEqual(h.symmetry, value.lower(), value)
 
         with self.assertRaises(ValueError):
             fmm.header(symmetry="foo")
 
+    def test_comment(self):
+        for comment in ["", "one-line", "\n", "multi\nline", "\npadded\n"]:
+            h = fmm.header(shape=(1, 1), nnz=1, comment=comment,
+                           object="matrix", format="array", field="integer", symmetry="general")
+
+            # Write to a buffer
+            bio = BytesIO()
+            fmm.write_header(bio, h)
+            s = bio.getvalue().decode()
+
+            h2 = fmm.read_header(StringIO(s))
+            self.assertEqual(h.comment, h2.comment)
+
     def test_read_file(self):
         path = matrices / "eye3.mtx"
         if not path.exists():
             self.skipTest("eye3.mtx is missing. Only happens when testing with cibuildwheel for some reason.")
 
         h = fmm.read_header(path)
         expected = fmm.header(shape=(3, 3), nnz=3, comment="3-by-3 identity matrix",
                               object="matrix", format="coordinate", field="real", symmetry="general")
         self.assertEqual(h.to_dict(), expected.to_dict())
 
-    @unittest.skipIf(IS_PYPY, "Writing into BytesIO has no effect on PyPy")
     def test_read_write(self):
         h = fmm.header(shape=(3, 3), nnz=3, comment="3-by-3 identity matrix",
                        object="matrix", format="coordinate", field="real", symmetry="general")
 
         # Write to a buffer
         bio = BytesIO()
         fmm.write_header(bio, h)
```

### Comparing `fast-matrix-market-1.6.0/testsuite_scipy/test_scipy_suite.py` & `fast-matrix-market-1.7.0/testsuite_scipy/test_scipy_suite.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.6.0/PKG-INFO` & `fast-matrix-market-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-matrix-market
-Version: 1.6.0
+Version: 1.7.0
 Summary: Fast and full-featured Matrix Market file I/O
 Home-page: https://github.com/alugowski/fast_matrix_market
 Author: Adam Lugowski
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

