# Comparing `tmp/pyopencl-2023.1.tar.gz` & `tmp/pyopencl-2023.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencl-2023.1.tar", last modified: Tue May  9 13:32:55 2023, max compression
+gzip compressed data, was "pyopencl-2023.1.1.tar", last modified: Sun Jun 25 19:16:08 2023, max compression
```

## Comparing `pyopencl-2023.1.tar` & `pyopencl-2023.1.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.666548 pyopencl-2023.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-09 13:32:28.000000 pyopencl-2023.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-09 13:32:28.000000 pyopencl-2023.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-09 13:32:28.000000 pyopencl-2023.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 13:32:28.000000 pyopencl-2023.1/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-09 13:32:55.666548 pyopencl-2023.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-09 13:32:28.000000 pyopencl-2023.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-09 13:32:28.000000 pyopencl-2023.1/README_SETUP.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31984 2023-05-09 13:32:28.000000 pyopencl-2023.1/aksetup_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-05-09 13:32:28.000000 pyopencl-2023.1/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.642547 pyopencl-2023.1/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/cldis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.642547 pyopencl-2023.1/contrib/fortran-to-opencl/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/fortran-to-opencl/README
--rw-r--r--   0 runner    (1001) docker     (123)    43661 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/fortran-to-opencl/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/pyopencl.vim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.646547 pyopencl-2023.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/array.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/make_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_const.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_gl.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_memory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_platform.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_program.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_queue.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/subst.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/types.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.654548 pyopencl-2023.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/black-hole-accretion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo-struct-reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_array_svm.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_elementwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_elementwise_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_mandelbrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_meta_codepy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_meta_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/dump-performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/dump-properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/gl_interop_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/gl_particle_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/ipython-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/median-filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32112 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/n-body.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/narray.py
--rw-r--r--   0 runner    (1001) docker     (123)    66806 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/noisyImage.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35441 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/pi-monte-carlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl/
--rw-r--r--   0 runner    (1001) docker     (123)    80080 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/_cluda.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/_mymako.py
--rw-r--r--   0 runner    (1001) docker     (123)    51198 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)   111678 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/bitonic_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/bitonic_sort_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/capture_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl/characterize/
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/characterize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/characterize/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl/cl/
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-airy.cl
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j-complex.cl
--rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j.cl
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-y.cl
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-eval-tbl.cl
--rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-hankel-complex.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.662548 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/array.h
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/openclfeatures.h
--rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/philox.cl
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/threefry.cl
--rw-r--r--   0 runner    (1001) docker     (123)    38528 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-ranluxcl.cl
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/clmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    25553 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/clrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.662548 pyopencl-2023.1/pyopencl/compyte/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.662548 pyopencl-2023.1/pyopencl/compyte/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76836 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/gen_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    56332 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/gen_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/setup_opencl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    38637 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/elementwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/invoker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/ipython_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    25547 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    65279 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    45549 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 13:32:28.000000 pyopencl-2023.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-09 13:32:55.666548 pyopencl-2023.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-05-09 13:32:28.000000 pyopencl-2023.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.666548 pyopencl-2023.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/bitlog.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/bitlog.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/clinfo_ext.h
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/mempool.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/pyopencl_ext.h
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/tools.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   161960 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl_part_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl_part_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    38115 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_constants.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_mempool.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.666548 pyopencl-2023.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/add-vectors-32.spv
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/add-vectors-64.spv
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/empty-header.h
--rw-r--r--   0 runner    (1001) docker     (123)    35358 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    63301 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_arrays_in_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_clmath.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_clrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_enqueue_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    43703 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.618623 pyopencl-2023.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-25 19:16:08.618623 pyopencl-2023.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/README_SETUP.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31984 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/aksetup_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.594623 pyopencl-2023.1.1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/contrib/cldis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.594623 pyopencl-2023.1.1/contrib/fortran-to-opencl/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/contrib/fortran-to-opencl/README
+-rw-r--r--   0 runner    (1001) docker     (123)    43661 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/contrib/fortran-to-opencl/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/contrib/pyopencl.vim
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.598623 pyopencl-2023.1.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/array.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/make_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/runtime_const.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/runtime_gl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/runtime_memory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/runtime_platform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/runtime_program.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/runtime_queue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/subst.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/doc/types.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.602623 pyopencl-2023.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/black-hole-accretion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo-struct-reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo_array_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo_elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo_elementwise_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo_mandelbrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo_meta_codepy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/demo_meta_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/dump-performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/dump-properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/gl_interop_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/gl_particle_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/ipython-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/median-filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32112 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/n-body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/narray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66806 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/noisyImage.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35441 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/pi-monte-carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/examples/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.606623 pyopencl-2023.1.1/pyopencl/
+-rw-r--r--   0 runner    (1001) docker     (123)    80080 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/_cluda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/_mymako.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51198 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111639 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/bitonic_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/bitonic_sort_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/capture_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.610623 pyopencl-2023.1.1/pyopencl/characterize/
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/characterize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/characterize/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.610623 pyopencl-2023.1.1/pyopencl/cl/
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-airy.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-bessel-j-complex.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-bessel-j.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-bessel-y.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-eval-tbl.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-hankel-complex.cl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.610623 pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/openclfeatures.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/philox.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/threefry.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    38528 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cl/pyopencl-ranluxcl.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/clmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25553 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/cltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.610623 pyopencl-2023.1.1/pyopencl/compyte/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.614623 pyopencl-2023.1.1/pyopencl/compyte/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/ndarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76836 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/ndarray/gen_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56332 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/ndarray/gen_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/ndarray/setup_opencl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-06-25 19:16:07.000000 pyopencl-2023.1.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38637 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/ipython_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25547 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65279 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45549 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyopencl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.610623 pyopencl-2023.1.1/pyopencl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-25 19:16:08.000000 pyopencl-2023.1.1/pyopencl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-25 19:16:08.000000 pyopencl-2023.1.1/pyopencl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:16:08.000000 pyopencl-2023.1.1/pyopencl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:16:08.000000 pyopencl-2023.1.1/pyopencl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-25 19:16:08.000000 pyopencl-2023.1.1/pyopencl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 19:16:08.000000 pyopencl-2023.1.1/pyopencl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-25 19:16:08.618623 pyopencl-2023.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.614623 pyopencl-2023.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/bitlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/bitlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/clinfo_ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/mempool.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/pyopencl_ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/wrap_cl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   161960 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/wrap_cl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/wrap_cl_part_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/wrap_cl_part_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38115 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/wrap_constants.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/wrap_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/src/wrap_mempool.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:16:08.618623 pyopencl-2023.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/add-vectors-32.spv
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/add-vectors-64.spv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/empty-header.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35358 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63301 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/test_arrays_in_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/test_clmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/test_clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/test_enqueue_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43703 2023-06-25 19:15:43.000000 pyopencl-2023.1.1/test/test_wrapper.py
```

### Comparing `pyopencl-2023.1/CITATION.cff` & `pyopencl-2023.1.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/LICENSE` & `pyopencl-2023.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/MANIFEST.in` & `pyopencl-2023.1.1/MANIFEST.in`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 include src/*.h
 include src/*.hpp
 include src/*.cpp
 include test/*.py
 include test/*.h
 include test/*.spv
 include examples/*.py
+include experiments/*.py
 include examples/*.ipynb
 include examples/noisyImage.jpg
 
 include doc/*.rst
 include doc/Makefile
 include doc/*.py
 include doc/conf.py
```

### Comparing `pyopencl-2023.1/PKG-INFO` & `pyopencl-2023.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2023.1
+Version: 2023.1.1
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopencl-2023.1/README.rst` & `pyopencl-2023.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/README_SETUP.txt` & `pyopencl-2023.1.1/README_SETUP.txt`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/aksetup_helper.py` & `pyopencl-2023.1.1/aksetup_helper.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/contrib/cldis.py` & `pyopencl-2023.1.1/contrib/cldis.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     device = ctx.devices[0]
     platform = device.platform
     if platform.name == "NVIDIA CUDA":
         supported_outputs = ["ptx", "sass"]
     elif platform.name == "Portable Computing Language":
         if device.name.startswith("NVIDIA"):
             supported_outputs = ["ptx", "sass"]
-        elif device.name.startswith("pthread-"):
+        elif device.name.startswith("pthread"):
             supported_outputs = ["asm"]
         else:
             raise NotImplementedError(f"Unknown pocl device '{device.name}'")
     else:
         raise NotImplementedError(f"Unknown opencl device '{device}'")
     if output is None:
         output = supported_outputs[0]
@@ -70,15 +70,15 @@
                     f"--gpu-name={gpu_name}", "--warn-on-spills"], cwd=tmp_dir)
                 res = subprocess.check_output(["cuobjdump", "-sass", "elf.o"],
                         cwd=tmp_dir).decode("utf-8")
 
         elif output == "asm" and platform.name == "Portable Computing Language":
             so = glob.glob(f"{tmp_dir}/**/*.so", recursive=True)[0]
             res = subprocess.check_output(["objdump", "-d", so]).decode("utf-8")
-        
+
         print(res)
 
 
 if __name__ == "__main__":
     with tempfile.TemporaryDirectory() as tmp_dir:
         os.environ["POCL_CACHE_DIR"] = os.path.join(tmp_dir, "pocl_cache")
         import pyopencl as cl
```

### Comparing `pyopencl-2023.1/contrib/fortran-to-opencl/README` & `pyopencl-2023.1.1/contrib/fortran-to-opencl/README`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/contrib/fortran-to-opencl/translate.py` & `pyopencl-2023.1.1/contrib/fortran-to-opencl/translate.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/contrib/pyopencl.vim` & `pyopencl-2023.1.1/contrib/pyopencl.vim`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/Makefile` & `pyopencl-2023.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/algorithm.rst` & `pyopencl-2023.1.1/doc/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/array.rst` & `pyopencl-2023.1.1/doc/array.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/conf.py` & `pyopencl-2023.1.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/howto.rst` & `pyopencl-2023.1.1/doc/howto.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/index.rst` & `pyopencl-2023.1.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/make_constants.py` & `pyopencl-2023.1.1/doc/make_constants.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/misc.rst` & `pyopencl-2023.1.1/doc/misc.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/runtime.rst` & `pyopencl-2023.1.1/doc/runtime.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/runtime_const.rst` & `pyopencl-2023.1.1/doc/runtime_const.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/runtime_gl.rst` & `pyopencl-2023.1.1/doc/runtime_gl.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/runtime_memory.rst` & `pyopencl-2023.1.1/doc/runtime_memory.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/runtime_platform.rst` & `pyopencl-2023.1.1/doc/runtime_platform.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/runtime_program.rst` & `pyopencl-2023.1.1/doc/runtime_program.rst`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,28 @@
         produces a new kernel object, so that this **won't** work::
 
             prg.sum.set_args(a_g, b_g, res_g)
             ev = cl.enqueue_nd_range_kernel(queue, prg.sum, a_np.shape, None)
 
         Instead, either use the (recommended, stateless) calling interface::
 
-            prg.sum(queue, prg.sum, a_np.shape, None)
-
-        or keep the kernel in a temporary variable::
-
             sum_knl = prg.sum
+            sum_knl(queue, a_np.shape, None, a_g, b_g, res_g)    
+            
+        or the long, stateful way around, if you prefer::
+
             sum_knl.set_args(a_g, b_g, res_g)
             ev = cl.enqueue_nd_range_kernel(queue, sum_knl, a_np.shape, None)
 
+        The following will also work, however note that a number of caches that
+        are important for efficient kernel enqueue are attached to the :class:`Kernel`
+        object, and these caches will be ineffective in this usage pattern::
+
+            prg.sum(queue, a_np.shape, None, a_g, b_g, res_g)
+
         Note that the :class:`Program` has to be built (see :meth:`build`) in
         order for this to work simply by attribute lookup.
 
         .. note::
 
             The :class:`program_info` attributes live
             in the same name space and take precedence over
```

### Comparing `pyopencl-2023.1/doc/runtime_queue.rst` & `pyopencl-2023.1.1/doc/runtime_queue.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/subst.rst` & `pyopencl-2023.1.1/doc/subst.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/doc/types.rst` & `pyopencl-2023.1.1/doc/types.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/black-hole-accretion.py` & `pyopencl-2023.1.1/examples/black-hole-accretion.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo-struct-reduce.py` & `pyopencl-2023.1.1/examples/demo-struct-reduce.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo.py` & `pyopencl-2023.1.1/examples/demo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo_array.py` & `pyopencl-2023.1.1/examples/demo_array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo_array_svm.py` & `pyopencl-2023.1.1/examples/demo_array_svm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo_elementwise.py` & `pyopencl-2023.1.1/examples/demo_elementwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo_elementwise_complex.py` & `pyopencl-2023.1.1/examples/demo_elementwise_complex.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo_mandelbrot.py` & `pyopencl-2023.1.1/examples/demo_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo_meta_codepy.py` & `pyopencl-2023.1.1/examples/demo_meta_codepy.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/demo_meta_template.py` & `pyopencl-2023.1.1/examples/demo_meta_template.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/dump-performance.py` & `pyopencl-2023.1.1/examples/dump-performance.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/dump-properties.py` & `pyopencl-2023.1.1/examples/dump-properties.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/gl_interop_demo.py` & `pyopencl-2023.1.1/examples/gl_interop_demo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/gl_particle_animation.py` & `pyopencl-2023.1.1/examples/gl_particle_animation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/ipython-demo.ipynb` & `pyopencl-2023.1.1/examples/ipython-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/median-filter.py` & `pyopencl-2023.1.1/examples/median-filter.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/n-body.py` & `pyopencl-2023.1.1/examples/n-body.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/narray.py` & `pyopencl-2023.1.1/examples/narray.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/noisyImage.jpg` & `pyopencl-2023.1.1/examples/noisyImage.jpg`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/pi-monte-carlo.py` & `pyopencl-2023.1.1/examples/pi-monte-carlo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/svm.py` & `pyopencl-2023.1.1/examples/svm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/examples/transpose.py` & `pyopencl-2023.1.1/examples/transpose.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/__init__.py` & `pyopencl-2023.1.1/pyopencl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/_cluda.py` & `pyopencl-2023.1.1/pyopencl/_cluda.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/_mymako.py` & `pyopencl-2023.1.1/pyopencl/_mymako.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/algorithm.py` & `pyopencl-2023.1.1/pyopencl/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/array.py` & `pyopencl-2023.1.1/pyopencl/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,26 +128,26 @@
             obj1 = np.zeros(1, dtype=o1_dtype)
         if o2_is_array:
             obj2 = np.zeros(1, dtype=o2_dtype)
 
         result = (obj1 + obj2).dtype
     else:
         array_types = []
-        scalar_types = []
+        scalars = []
 
         if o1_is_array:
             array_types.append(o1_dtype)
         else:
-            scalar_types.append(o1_dtype)
+            scalars.append(obj1)
         if o2_is_array:
             array_types.append(o2_dtype)
         else:
-            scalar_types.append(o2_dtype)
+            scalars.append(obj2)
 
-        result = np.find_common_type(array_types, scalar_types)
+        result = np.result_type(*array_types, *scalars)
 
     if not allow_double:
         if result == np.float64:
             result = np.dtype(np.float32)
             warn(_DOUBLE_DOWNCAST_WARNING, DoubleDowncastWarning, stacklevel=3)
         elif result == np.complex128:
             result = np.dtype(np.complex64)
@@ -2799,15 +2799,15 @@
 
             # pylint: disable=unsupported-assignment-operation
             shape[axis] += ary.shape[axis]
 
     # }}}
 
     shape = tuple(shape)
-    dtype = np.find_common_type([ary.dtype for ary in arrays], [])
+    dtype = np.result_type(*[ary.dtype for ary in arrays])
 
     if __debug__:
         if builtins.any(type(ary) != type(arrays[0])  # noqa: E721
                         for ary in arrays[1:]):
             warn("Elements of 'arrays' not of the same type, returning "
                  "an instance of the type of arrays[0]",
                  stacklevel=2)
```

### Comparing `pyopencl-2023.1/pyopencl/bitonic_sort.py` & `pyopencl-2023.1.1/pyopencl/bitonic_sort.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/bitonic_sort_templates.py` & `pyopencl-2023.1.1/pyopencl/bitonic_sort_templates.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cache.py` & `pyopencl-2023.1.1/pyopencl/cache.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/capture_call.py` & `pyopencl-2023.1.1/pyopencl/capture_call.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/characterize/__init__.py` & `pyopencl-2023.1.1/pyopencl/characterize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/characterize/performance.py` & `pyopencl-2023.1.1/pyopencl/characterize/performance.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-airy.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-airy.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j-complex.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-bessel-j-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-bessel-j.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-y.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-bessel-y.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-complex.h` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-complex.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-eval-tbl.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-eval-tbl.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-hankel-complex.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-hankel-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/array.h` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/array.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/openclfeatures.h` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/openclfeatures.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/philox.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/philox.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/threefry.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-random123/threefry.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cl/pyopencl-ranluxcl.cl` & `pyopencl-2023.1.1/pyopencl/cl/pyopencl-ranluxcl.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/clmath.py` & `pyopencl-2023.1.1/pyopencl/clmath.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/clrandom.py` & `pyopencl-2023.1.1/pyopencl/clrandom.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/cltypes.py` & `pyopencl-2023.1.1/pyopencl/cltypes.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/compyte/array.py` & `pyopencl-2023.1.1/pyopencl/compyte/array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/compyte/dtypes.py` & `pyopencl-2023.1.1/pyopencl/compyte/dtypes.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/compyte/ndarray/gen_elemwise.py` & `pyopencl-2023.1.1/pyopencl/compyte/ndarray/gen_elemwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/compyte/ndarray/gen_reduction.py` & `pyopencl-2023.1.1/pyopencl/compyte/ndarray/gen_reduction.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/compyte/ndarray/setup_opencl.py` & `pyopencl-2023.1.1/pyopencl/compyte/ndarray/setup_opencl.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py` & `pyopencl-2023.1.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py` & `pyopencl-2023.1.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/elementwise.py` & `pyopencl-2023.1.1/pyopencl/elementwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/invoker.py` & `pyopencl-2023.1.1/pyopencl/invoker.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/ipython_ext.py` & `pyopencl-2023.1.1/pyopencl/ipython_ext.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/reduction.py` & `pyopencl-2023.1.1/pyopencl/reduction.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/scan.py` & `pyopencl-2023.1.1/pyopencl/scan.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl/tools.py` & `pyopencl-2023.1.1/pyopencl/tools.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyopencl.egg-info/PKG-INFO` & `pyopencl-2023.1.1/pyopencl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2023.1
+Version: 2023.1.1
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopencl-2023.1/pyopencl.egg-info/SOURCES.txt` & `pyopencl-2023.1.1/pyopencl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/pyproject.toml` & `pyopencl-2023.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/setup.cfg` & `pyopencl-2023.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/setup.py` & `pyopencl-2023.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/bitlog.cpp` & `pyopencl-2023.1.1/src/bitlog.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/bitlog.hpp` & `pyopencl-2023.1.1/src/bitlog.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/clinfo_ext.h` & `pyopencl-2023.1.1/src/clinfo_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/mempool.hpp` & `pyopencl-2023.1.1/src/mempool.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/pyopencl_ext.h` & `pyopencl-2023.1.1/src/pyopencl_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/tools.hpp` & `pyopencl-2023.1.1/src/tools.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/wrap_cl.cpp` & `pyopencl-2023.1.1/src/wrap_cl.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/wrap_cl.hpp` & `pyopencl-2023.1.1/src/wrap_cl.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/wrap_cl_part_1.cpp` & `pyopencl-2023.1.1/src/wrap_cl_part_1.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/wrap_cl_part_2.cpp` & `pyopencl-2023.1.1/src/wrap_cl_part_2.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/wrap_constants.cpp` & `pyopencl-2023.1.1/src/wrap_constants.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/wrap_helpers.hpp` & `pyopencl-2023.1.1/src/wrap_helpers.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/src/wrap_mempool.cpp` & `pyopencl-2023.1.1/src/wrap_mempool.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/add-vectors-32.spv` & `pyopencl-2023.1.1/test/add-vectors-32.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/add-vectors-64.spv` & `pyopencl-2023.1.1/test/add-vectors-64.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/test_algorithm.py` & `pyopencl-2023.1.1/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/test_array.py` & `pyopencl-2023.1.1/test/test_array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/test_arrays_in_structs.py` & `pyopencl-2023.1.1/test/test_arrays_in_structs.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/test_clmath.py` & `pyopencl-2023.1.1/test/test_clmath.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/test_clrandom.py` & `pyopencl-2023.1.1/test/test_clrandom.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2023.1/test/test_enqueue_copy.py` & `pyopencl-2023.1.1/test/test_enqueue_copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,16 +73,16 @@
     buf_out_shp = 300, 400  # shape of 2nd device buffer
 
     # Create host array of random values.
     rng = np.random.default_rng(seed=42)
     h_ary_in = rng.integers(0, 256, ary_in_shp, dtype=np.uint8)
 
     # Create device buffers
-    d_in_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.product(buf_in_shp))
-    d_out_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.product(buf_out_shp))
+    d_in_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.prod(buf_in_shp))
+    d_out_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.prod(buf_out_shp))
 
     # Copy sub-array (rectangular buffer) from host to device
     cl.enqueue_copy(
         queue,
         d_in_buf,
         h_ary_in,
         buffer_origin=buf_in_origin[::-1],
@@ -162,16 +162,16 @@
     buf_out_shp = 300, 400, 40  # shape of 2nd device buffer
 
     # Create host array of random values.
     rng = np.random.default_rng(seed=42)
     h_ary_in = rng.integers(0, 256, ary_in_shp, dtype=np.uint8)
 
     # Create device buffers
-    d_in_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.product(buf_in_shp))
-    d_out_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.product(buf_out_shp))
+    d_in_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.prod(buf_in_shp))
+    d_out_buf = cl.Buffer(ctx, cl.mem_flags.READ_ONLY, size=np.prod(buf_out_shp))
 
     # Copy sub-array (rectangular buffer) from host to device
     cl.enqueue_copy(
         queue,
         d_in_buf,
         h_ary_in,
         buffer_origin=buf_in_origin[::-1],
```

### Comparing `pyopencl-2023.1/test/test_wrapper.py` & `pyopencl-2023.1.1/test/test_wrapper.py`

 * *Files identical despite different names*

