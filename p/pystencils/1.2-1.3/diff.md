# Comparing `tmp/pystencils-1.2.tar.gz` & `tmp/pystencils-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystencils-1.2.tar", last modified: Sun Apr  9 10:32:44 2023, max compression
+gzip compressed data, was "pystencils-1.3.tar", last modified: Sun Jun 25 13:47:28 2023, max compression
```

## Comparing `pystencils-1.2.tar` & `pystencils-1.3.tar`

### file list

```diff
@@ -1,271 +1,270 @@
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.542305 pystencils-1.2/
--rw-r--r--   0 holzer     (502) staff       (20)      151 2023-04-09 10:31:00.000000 pystencils-1.2/.flake8
--rw-r--r--   0 holzer     (502) staff       (20)       36 2023-04-09 10:31:00.000000 pystencils-1.2/.gitattributes
--rw-r--r--   0 holzer     (502) staff       (20)      462 2023-04-09 10:31:00.000000 pystencils-1.2/.gitignore
--rw-r--r--   0 holzer     (502) staff       (20)     8705 2023-04-09 10:31:00.000000 pystencils-1.2/.gitlab-ci.yml
--rw-r--r--   0 holzer     (502) staff       (20)       94 2023-04-09 10:31:00.000000 pystencils-1.2/.isort.cfg
--rw-r--r--   0 holzer     (502) staff       (20)      502 2023-04-09 10:31:00.000000 pystencils-1.2/AUTHORS.txt
--rw-r--r--   0 holzer     (502) staff       (20)      209 2023-04-09 10:31:00.000000 pystencils-1.2/CHANGELOG.md
--rw-r--r--   0 holzer     (502) staff       (20)     3797 2023-04-09 10:31:00.000000 pystencils-1.2/CONTRIBUTING.md
--rw-r--r--   0 holzer     (502) staff       (20)    34523 2023-04-09 10:31:00.000000 pystencils-1.2/COPYING.txt
--rw-r--r--   0 holzer     (502) staff       (20)      169 2023-04-09 10:31:00.000000 pystencils-1.2/MANIFEST.in
--rw-r--r--   0 holzer     (502) staff       (20)     4615 2023-04-09 10:32:44.542392 pystencils-1.2/PKG-INFO
--rw-r--r--   0 holzer     (502) staff       (20)     3451 2023-04-09 10:31:00.000000 pystencils-1.2/README.md
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.495893 pystencils-1.2/binder/
--rw-r--r--   0 holzer     (502) staff       (20)       32 2023-04-09 10:31:00.000000 pystencils-1.2/binder/apt.txt
--rw-r--r--   0 holzer     (502) staff       (20)     1404 2023-04-09 10:31:00.000000 pystencils-1.2/binder/environment.yml
--rwxr-xr-x   0 holzer     (502) staff       (20)       48 2023-04-09 10:31:00.000000 pystencils-1.2/binder/start
--rw-r--r--   0 holzer     (502) staff       (20)     5552 2023-04-09 10:31:00.000000 pystencils-1.2/conftest.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.496383 pystencils-1.2/doc/
--rw-r--r--   0 holzer     (502) staff       (20)     1985 2023-04-09 10:31:00.000000 pystencils-1.2/doc/conf.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.499168 pystencils-1.2/doc/img/
--rw-r--r--   0 holzer     (502) staff       (20)   241908 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/c_backend.svg
--rw-r--r--   0 holzer     (502) staff       (20)    80293 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/github_repo_card.png
--rw-r--r--   0 holzer     (502) staff       (20)    10116 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/logo.png
--rw-r--r--   0 holzer     (502) staff       (20)    14392 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/logo.svg
--rw-r--r--   0 holzer     (502) staff       (20)    15916 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/logo_large.svg
--rw-r--r--   0 holzer     (502) staff       (20)     5554 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/logo_no_text.png
--rw-r--r--   0 holzer     (502) staff       (20)    27415 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/pystencils_arch_block_diagram.svg
--rw-r--r--   0 holzer     (502) staff       (20)    21047 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/pystencils_stencil_four_points_with_arrows.svg
--rw-r--r--   0 holzer     (502) staff       (20)    33850 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/staggered_grid.svg
--rw-r--r--   0 holzer     (502) staff       (20)    27441 2023-04-09 10:31:00.000000 pystencils-1.2/doc/img/walberla_blocks.svg
--rw-r--r--   0 holzer     (502) staff       (20)      418 2023-04-09 10:31:00.000000 pystencils-1.2/doc/index.rst
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.505454 pystencils-1.2/doc/notebooks/
--rw-r--r--   0 holzer     (502) staff       (20)   196697 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/01_tutorial_getting_started.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)    82577 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/02_tutorial_basic_kernels.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)    85067 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/03_tutorial_datahandling.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)   433256 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/04_tutorial_advection_diffusion.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)  1773389 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/05_tutorial_phasefield_spinodal_decomposition.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)   787498 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/06_tutorial_phasefield_dentritic_growth.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)    25871 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/demo_assignment_collection.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)    48557 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/demo_benchmark.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)    51389 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/demo_derivatives.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)   846996 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/demo_plotting_and_animation.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)   248900 2023-04-09 10:31:00.000000 pystencils-1.2/doc/notebooks/demo_wave_equation.ipynb
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.508394 pystencils-1.2/doc/sphinx/
--rw-r--r--   0 holzer     (502) staff       (20)      244 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/api.rst
--rw-r--r--   0 holzer     (502) staff       (20)      303 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/ast.rst
--rw-r--r--   0 holzer     (502) staff       (20)       80 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/configuration.rst
--rw-r--r--   0 holzer     (502) staff       (20)      104 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/datahandling.rst
--rw-r--r--   0 holzer     (502) staff       (20)       86 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/enums.rst
--rw-r--r--   0 holzer     (502) staff       (20)       64 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/field.rst
--rw-r--r--   0 holzer     (502) staff       (20)      102 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/finite_differences.rst
--rw-r--r--   0 holzer     (502) staff       (20)      754 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/kernel_compile_and_call.rst
--rw-r--r--   0 holzer     (502) staff       (20)      117 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/plot.rst
--rw-r--r--   0 holzer     (502) staff       (20)        0 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/pystencils.bib
--rw-r--r--   0 holzer     (502) staff       (20)      880 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/simplifications.rst
--rw-r--r--   0 holzer     (502) staff       (20)       73 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/stencil.rst
--rw-r--r--   0 holzer     (502) staff       (20)      860 2023-04-09 10:31:00.000000 pystencils-1.2/doc/sphinx/tutorials.rst
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.542966 pystencils-1.2/pystencils/
--rw-r--r--   0 holzer     (502) staff       (20)     1660 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)      495 2023-04-09 10:32:44.543008 pystencils-1.2/pystencils/_version.py
--rw-r--r--   0 holzer     (502) staff       (20)     4808 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/alignedarray.py
--rw-r--r--   0 holzer     (502) staff       (20)     4043 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/assignment.py
--rw-r--r--   0 holzer     (502) staff       (20)    29015 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/astnodes.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.516720 pystencils-1.2/pystencils/backends/
--rw-r--r--   0 holzer     (502) staff       (20)      164 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     6556 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/arm_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)    40797 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/cbackend.py
--rw-r--r--   0 holzer     (502) staff       (20)     2824 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/cuda_backend.py
--rw-r--r--   0 holzer     (502) staff       (20)     3539 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/dot.py
--rw-r--r--   0 holzer     (502) staff       (20)     2479 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/json.py
--rw-r--r--   0 holzer     (502) staff       (20)     3931 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/ppc_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     3823 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/riscv_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     5152 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/simd_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     6137 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/backends/x86_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     1707 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/bit_masks.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.518925 pystencils-1.2/pystencils/boundaries/
--rw-r--r--   0 holzer     (502) staff       (20)      284 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/boundaries/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     4344 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/boundaries/boundaryconditions.py
--rw-r--r--   0 holzer     (502) staff       (20)    20920 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/boundaries/boundaryhandling.py
--rw-r--r--   0 holzer     (502) staff       (20)     8226 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/boundaries/createindexlist.py
--rw-r--r--   0 holzer     (502) staff       (20)  2023077 2023-04-09 10:32:44.000000 pystencils-1.2/pystencils/boundaries/createindexlistcython.c
--rw-r--r--   0 holzer     (502) staff       (20)     8006 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/boundaries/createindexlistcython.pyx
--rw-r--r--   0 holzer     (502) staff       (20)     2031 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/boundaries/inkernel.py
--rw-r--r--   0 holzer     (502) staff       (20)     2406 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/cache.py
--rw-r--r--   0 holzer     (502) staff       (20)     9015 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/config.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.520651 pystencils-1.2/pystencils/cpu/
--rw-r--r--   0 holzer     (502) staff       (20)      238 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/cpu/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    27504 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/cpu/cpujit.py
--rw-r--r--   0 holzer     (502) staff       (20)    10362 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/cpu/kernelcreation.py
--rw-r--r--   0 holzer     (502) staff       (20)     3758 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/cpu/msvc_detection.py
--rw-r--r--   0 holzer     (502) staff       (20)    20020 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/cpu/vectorization.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.521849 pystencils-1.2/pystencils/datahandling/
--rw-r--r--   0 holzer     (502) staff       (20)     3033 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/datahandling/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     5637 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/datahandling/blockiteration.py
--rw-r--r--   0 holzer     (502) staff       (20)    20854 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/datahandling/datahandling_interface.py
--rw-r--r--   0 holzer     (502) staff       (20)    17330 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/datahandling/parallel_datahandling.py
--rw-r--r--   0 holzer     (502) staff       (20)     1515 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/datahandling/pycuda.py
--rw-r--r--   0 holzer     (502) staff       (20)    18791 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/datahandling/serial_datahandling.py
--rw-r--r--   0 holzer     (502) staff       (20)     2136 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/datahandling/vtk.py
--rw-r--r--   0 holzer     (502) staff       (20)     3482 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/display_utils.py
--rw-r--r--   0 holzer     (502) staff       (20)      713 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/enums.py
--rw-r--r--   0 holzer     (502) staff       (20)     2624 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/fast_approximation.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.522830 pystencils-1.2/pystencils/fd/
--rw-r--r--   0 holzer     (502) staff       (20)      880 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/fd/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    14981 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/fd/derivation.py
--rw-r--r--   0 holzer     (502) staff       (20)    21404 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/fd/derivative.py
--rw-r--r--   0 holzer     (502) staff       (20)    15080 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/fd/finitedifferences.py
--rw-r--r--   0 holzer     (502) staff       (20)    11806 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/fd/finitevolumes.py
--rw-r--r--   0 holzer     (502) staff       (20)     7060 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/fd/spatial.py
--rw-r--r--   0 holzer     (502) staff       (20)    46691 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/field.py
--rw-r--r--   0 holzer     (502) staff       (20)     1538 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/functions.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.523591 pystencils-1.2/pystencils/gpucuda/
--rw-r--r--   0 holzer     (502) staff       (20)      376 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/gpucuda/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     7549 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/gpucuda/cudajit.py
--rw-r--r--   0 holzer     (502) staff       (20)    14940 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/gpucuda/indexing.py
--rw-r--r--   0 holzer     (502) staff       (20)     8773 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/gpucuda/kernelcreation.py
--rw-r--r--   0 holzer     (502) staff       (20)     2089 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/gpucuda/periodicity.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.525042 pystencils-1.2/pystencils/include/
--rw-r--r--   0 holzer     (502) staff       (20)      413 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/PyStencilsField.h
--rw-r--r--   0 holzer     (502) staff       (20)      231 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    28113 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/aesni_rand.h
--rw-r--r--   0 holzer     (502) staff       (20)     2055 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/arm_neon_helpers.h
--rw-r--r--   0 holzer     (502) staff       (20)    38818 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/cuda_complex.hpp
--rw-r--r--   0 holzer     (502) staff       (20)     3759 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/myintrin.h
--rw-r--r--   0 holzer     (502) staff       (20)      370 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/opencl_stdint.h
--rw-r--r--   0 holzer     (502) staff       (20)    57970 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/philox_rand.h
--rw-r--r--   0 holzer     (502) staff       (20)     1007 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/include/ppc_altivec_helpers.h
--rw-r--r--   0 holzer     (502) staff       (20)     6390 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/integer_functions.py
--rw-r--r--   0 holzer     (502) staff       (20)     2830 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/integer_set_analysis.py
--rw-r--r--   0 holzer     (502) staff       (20)     3989 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/jupyter.py
--rw-r--r--   0 holzer     (502) staff       (20)     5676 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/kernel_contrains_check.py
--rw-r--r--   0 holzer     (502) staff       (20)     5133 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/kernel_decorator.py
--rw-r--r--   0 holzer     (502) staff       (20)      545 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/kernel_wrapper.py
--rw-r--r--   0 holzer     (502) staff       (20)    19145 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/kernelcreation.py
--rw-r--r--   0 holzer     (502) staff       (20)     3190 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/node_collection.py
--rw-r--r--   0 holzer     (502) staff       (20)     2680 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/placeholder_function.py
--rw-r--r--   0 holzer     (502) staff       (20)    13234 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/plot.py
--rw-r--r--   0 holzer     (502) staff       (20)     4526 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/rng.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.525522 pystencils-1.2/pystencils/runhelper/
--rw-r--r--   0 holzer     (502) staff       (20)      150 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/runhelper/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     7898 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/runhelper/db.py
--rw-r--r--   0 holzer     (502) staff       (20)    17806 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/runhelper/parameterstudy.py
--rw-r--r--   0 holzer     (502) staff       (20)      286 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/session.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.526363 pystencils-1.2/pystencils/simp/
--rw-r--r--   0 holzer     (502) staff       (20)     1352 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/simp/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    21879 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/simp/assignment_collection.py
--rw-r--r--   0 holzer     (502) staff       (20)    10999 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/simp/simplifications.py
--rw-r--r--   0 holzer     (502) staff       (20)     6854 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/simp/simplificationstrategy.py
--rw-r--r--   0 holzer     (502) staff       (20)     3334 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/simp/subexpression_insertion.py
--rw-r--r--   0 holzer     (502) staff       (20)      804 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/simplificationfactory.py
--rw-r--r--   0 holzer     (502) staff       (20)     9760 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/slicing.py
--rw-r--r--   0 holzer     (502) staff       (20)      546 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/spatial_coordinates.py
--rw-r--r--   0 holzer     (502) staff       (20)    17146 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/stencil.py
--rw-r--r--   0 holzer     (502) staff       (20)    27160 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/sympyextensions.py
--rw-r--r--   0 holzer     (502) staff       (20)     4300 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/timeloop.py
--rw-r--r--   0 holzer     (502) staff       (20)    43948 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/transformations.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.527484 pystencils-1.2/pystencils/typing/
--rw-r--r--   0 holzer     (502) staff       (20)     1292 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/typing/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     4156 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/typing/cast_functions.py
--rw-r--r--   0 holzer     (502) staff       (20)    13559 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/typing/leaf_typing.py
--rw-r--r--   0 holzer     (502) staff       (20)      832 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/typing/transformations.py
--rw-r--r--   0 holzer     (502) staff       (20)     5816 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/typing/typed_sympy.py
--rw-r--r--   0 holzer     (502) staff       (20)     8885 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/typing/types.py
--rw-r--r--   0 holzer     (502) staff       (20)     9185 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/typing/utilities.py
--rw-r--r--   0 holzer     (502) staff       (20)     7760 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils/utils.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.515109 pystencils-1.2/pystencils.egg-info/
--rw-r--r--   0 holzer     (502) staff       (20)     4615 2023-04-09 10:32:44.000000 pystencils-1.2/pystencils.egg-info/PKG-INFO
--rw-r--r--   0 holzer     (502) staff       (20)     8522 2023-04-09 10:32:44.000000 pystencils-1.2/pystencils.egg-info/SOURCES.txt
--rw-r--r--   0 holzer     (502) staff       (20)        1 2023-04-09 10:32:44.000000 pystencils-1.2/pystencils.egg-info/dependency_links.txt
--rw-r--r--   0 holzer     (502) staff       (20)      314 2023-04-09 10:32:44.000000 pystencils-1.2/pystencils.egg-info/requires.txt
--rw-r--r--   0 holzer     (502) staff       (20)       11 2023-04-09 10:32:44.000000 pystencils-1.2/pystencils.egg-info/top_level.txt
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.540652 pystencils-1.2/pystencils_tests/
--rw-r--r--   0 holzer     (502) staff       (20)        0 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     3624 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_Min_Max.py
--rw-r--r--   0 holzer     (502) staff       (20)      617 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_abs.py
--rw-r--r--   0 holzer     (502) staff       (20)     1552 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_address_of.py
--rw-r--r--   0 holzer     (502) staff       (20)     2823 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_aligned_array.py
--rw-r--r--   0 holzer     (502) staff       (20)     6289 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_assignment_collection.py
--rw-r--r--   0 holzer     (502) staff       (20)     1133 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_assignment_collection_dict_conversion.py
--rw-r--r--   0 holzer     (502) staff       (20)      630 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_assignment_from_stencil.py
--rw-r--r--   0 holzer     (502) staff       (20)     2362 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_astnodes.py
--rw-r--r--   0 holzer     (502) staff       (20)     1213 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_bit_masks.py
--rw-r--r--   0 holzer     (502) staff       (20)     3186 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_blocking.py
--rw-r--r--   0 holzer     (502) staff       (20)      962 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_blocking_staggered.py
--rw-r--r--   0 holzer     (502) staff       (20)     9948 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_boundary.py
--rw-r--r--   0 holzer     (502) staff       (20)     5333 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_boundary_indexlist_creation.py
--rw-r--r--   0 holzer     (502) staff       (20)    12127 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_buffer.py
--rw-r--r--   0 holzer     (502) staff       (20)    14903 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_buffer_gpu.py
--rw-r--r--   0 holzer     (502) staff       (20)     2310 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_conditional_field_access.py
--rw-r--r--   0 holzer     (502) staff       (20)     4847 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_conditional_vec.py
--rw-r--r--   0 holzer     (502) staff       (20)     4433 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_config.py
--rw-r--r--   0 holzer     (502) staff       (20)     1285 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_create_kernel_config.py
--rw-r--r--   0 holzer     (502) staff       (20)     6721 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_cudagpu.py
--rw-r--r--   0 holzer     (502) staff       (20)     1611 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_custom_backends.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.541515 pystencils-1.2/pystencils_tests/test_data/
--rw-r--r--   0 holzer     (502) staff       (20)      410 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/datahandling_load_test.npz
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.541858 pystencils-1.2/pystencils_tests/test_data/datahandling_parallel_load_test/
--rw-r--r--   0 holzer     (502) staff       (20)      304 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/datahandling_parallel_load_test/dst.dat
--rw-r--r--   0 holzer     (502) staff       (20)      304 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/datahandling_parallel_load_test/src.dat
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-04-09 10:32:44.542171 pystencils-1.2/pystencils_tests/test_data/datahandling_parallel_save_test/
--rw-r--r--   0 holzer     (502) staff       (20)      304 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/datahandling_parallel_save_test/dst.dat
--rw-r--r--   0 holzer     (502) staff       (20)      304 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/datahandling_parallel_save_test/src.dat
--rw-r--r--   0 holzer     (502) staff       (20)      410 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/datahandling_save_test.npz
--rw-r--r--   0 holzer     (502) staff       (20)   473831 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/lenna.png
--rw-r--r--   0 holzer     (502) staff       (20)     7609 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_data/test_vessel2d_mask.png
--rw-r--r--   0 holzer     (502) staff       (20)    12296 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_datahandling.py
--rw-r--r--   0 holzer     (502) staff       (20)     6696 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_datahandling_parallel.py
--rw-r--r--   0 holzer     (502) staff       (20)     1786 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_derivative.py
--rw-r--r--   0 holzer     (502) staff       (20)    19953 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_dot_printer.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)      421 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_dot_printer.py
--rw-r--r--   0 holzer     (502) staff       (20)     1126 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_dtype_check.py
--rw-r--r--   0 holzer     (502) staff       (20)     1607 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_fast_approximation.py
--rw-r--r--   0 holzer     (502) staff       (20)    22011 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_fd_derivation.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)     5616 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_fd_derivation_via_rotation.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)      735 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_fd_derivative.py
--rw-r--r--   0 holzer     (502) staff       (20)     8348 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_field.py
--rw-r--r--   0 holzer     (502) staff       (20)      790 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_field_access_poly.py
--rw-r--r--   0 holzer     (502) staff       (20)     6443 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_field_equality.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)     3435 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_finite_differences.py
--rw-r--r--   0 holzer     (502) staff       (20)     1786 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_floor_ceil_int_optimization.py
--rw-r--r--   0 holzer     (502) staff       (20)    26645 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_fvm.py
--rw-r--r--   0 holzer     (502) staff       (20)     4056 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_global_definitions.py
--rw-r--r--   0 holzer     (502) staff       (20)      954 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_helpful_errors.py
--rw-r--r--   0 holzer     (502) staff       (20)     2183 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_indexed_kernels.py
--rw-r--r--   0 holzer     (502) staff       (20)     2778 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_jacobi_cbackend.py
--rw-r--r--   0 holzer     (502) staff       (20)      769 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_json_backend.py
--rw-r--r--   0 holzer     (502) staff       (20)    35405 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_jupyter_extensions.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)      585 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_logarithm.py
--rw-r--r--   0 holzer     (502) staff       (20)     5890 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_loop_cutting.py
--rw-r--r--   0 holzer     (502) staff       (20)     2454 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_match_subs_for_assignment_collection.py
--rw-r--r--   0 holzer     (502) staff       (20)     3837 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_math_functions.py
--rw-r--r--   0 holzer     (502) staff       (20)     1661 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_modulo.py
--rw-r--r--   0 holzer     (502) staff       (20)     1284 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_move_constant_before_loop.py
--rw-r--r--   0 holzer     (502) staff       (20)      487 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_nodecollection.py
--rw-r--r--   0 holzer     (502) staff       (20)     2680 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_parameterstudy.py
--rw-r--r--   0 holzer     (502) staff       (20)    37327 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_phasefield_dentritic_3D.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)      486 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_pickle_support.py
--rw-r--r--   0 holzer     (502) staff       (20)     1872 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_plot.py
--rw-r--r--   0 holzer     (502) staff       (20)      708 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_print_infinity.py
--rw-r--r--   0 holzer     (502) staff       (20)      513 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_print_unsupported_node.py
--rw-r--r--   0 holzer     (502) staff       (20)     2733 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_quicktests.py
--rw-r--r--   0 holzer     (502) staff       (20)    10200 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_random.py
--rw-r--r--   0 holzer     (502) staff       (20)     1885 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_sharedmethodcache.py
--rw-r--r--   0 holzer     (502) staff       (20)     2940 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_simplification_strategy.py
--rw-r--r--   0 holzer     (502) staff       (20)     6471 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_simplifications.py
--rw-r--r--   0 holzer     (502) staff       (20)     4674 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_size_and_layout_checks.py
--rw-r--r--   0 holzer     (502) staff       (20)     1060 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_sliced_iteration.py
--rw-r--r--   0 holzer     (502) staff       (20)     2449 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_slicing.py
--rw-r--r--   0 holzer     (502) staff       (20)    12457 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_small_block_benchmark.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)      839 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_source_code_comment.py
--rw-r--r--   0 holzer     (502) staff       (20)     3963 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_staggered_kernel.py
--rw-r--r--   0 holzer     (502) staff       (20)    14917 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_stencil_plot.ipynb
--rw-r--r--   0 holzer     (502) staff       (20)     1138 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_stencils.py
--rw-r--r--   0 holzer     (502) staff       (20)     1704 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_struct_types.py
--rw-r--r--   0 holzer     (502) staff       (20)     1540 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_subexpression_insertion.py
--rw-r--r--   0 holzer     (502) staff       (20)     2462 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_sum_prod.py
--rw-r--r--   0 holzer     (502) staff       (20)     7403 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_sympyextensions.py
--rw-r--r--   0 holzer     (502) staff       (20)     2561 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_timeloop.py
--rw-r--r--   0 holzer     (502) staff       (20)     3000 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_transformations.py
--rw-r--r--   0 holzer     (502) staff       (20)     1050 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_type_interference.py
--rw-r--r--   0 holzer     (502) staff       (20)     7652 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_types.py
--rw-r--r--   0 holzer     (502) staff       (20)     2389 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_utils.py
--rw-r--r--   0 holzer     (502) staff       (20)    10349 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_vectorization.py
--rw-r--r--   0 holzer     (502) staff       (20)    12821 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_vectorization_specific.py
--rw-r--r--   0 holzer     (502) staff       (20)      278 2023-04-09 10:31:00.000000 pystencils-1.2/pystencils_tests/test_version_string.py
--rw-r--r--   0 holzer     (502) staff       (20)     1854 2023-04-09 10:31:00.000000 pystencils-1.2/pytest.ini
--rw-r--r--   0 holzer     (502) staff       (20)      247 2023-04-09 10:31:00.000000 pystencils-1.2/release.sh
--rw-r--r--   0 holzer     (502) staff       (20)      217 2023-04-09 10:32:44.542712 pystencils-1.2/setup.cfg
--rw-r--r--   0 holzer     (502) staff       (20)     5200 2023-04-09 10:31:00.000000 pystencils-1.2/setup.py
--rw-r--r--   0 holzer     (502) staff       (20)    70144 2023-04-09 10:31:00.000000 pystencils-1.2/versioneer.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.654133 pystencils-1.3/
+-rw-r--r--   0 holzer     (502) staff       (20)      151 2023-06-25 13:46:03.000000 pystencils-1.3/.flake8
+-rw-r--r--   0 holzer     (502) staff       (20)       36 2023-06-25 13:46:03.000000 pystencils-1.3/.gitattributes
+-rw-r--r--   0 holzer     (502) staff       (20)      469 2023-06-25 13:46:03.000000 pystencils-1.3/.gitignore
+-rw-r--r--   0 holzer     (502) staff       (20)     8698 2023-06-25 13:46:03.000000 pystencils-1.3/.gitlab-ci.yml
+-rw-r--r--   0 holzer     (502) staff       (20)       94 2023-06-25 13:46:03.000000 pystencils-1.3/.isort.cfg
+-rw-r--r--   0 holzer     (502) staff       (20)      502 2023-06-25 13:46:03.000000 pystencils-1.3/AUTHORS.txt
+-rw-r--r--   0 holzer     (502) staff       (20)      209 2023-06-25 13:46:03.000000 pystencils-1.3/CHANGELOG.md
+-rw-r--r--   0 holzer     (502) staff       (20)     3797 2023-06-25 13:46:03.000000 pystencils-1.3/CONTRIBUTING.md
+-rw-r--r--   0 holzer     (502) staff       (20)    34523 2023-06-25 13:46:03.000000 pystencils-1.3/COPYING.txt
+-rw-r--r--   0 holzer     (502) staff       (20)      169 2023-06-25 13:46:03.000000 pystencils-1.3/MANIFEST.in
+-rw-r--r--   0 holzer     (502) staff       (20)     4626 2023-06-25 13:47:28.654221 pystencils-1.3/PKG-INFO
+-rw-r--r--   0 holzer     (502) staff       (20)     3462 2023-06-25 13:46:03.000000 pystencils-1.3/README.md
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.607819 pystencils-1.3/binder/
+-rw-r--r--   0 holzer     (502) staff       (20)       32 2023-06-25 13:46:03.000000 pystencils-1.3/binder/apt.txt
+-rw-r--r--   0 holzer     (502) staff       (20)     1416 2023-06-25 13:46:03.000000 pystencils-1.3/binder/environment.yml
+-rwxr-xr-x   0 holzer     (502) staff       (20)       48 2023-06-25 13:46:03.000000 pystencils-1.3/binder/start
+-rw-r--r--   0 holzer     (502) staff       (20)     5542 2023-06-25 13:46:03.000000 pystencils-1.3/conftest.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.608330 pystencils-1.3/doc/
+-rwxr-xr-x   0 holzer     (502) staff       (20)     1985 2023-06-25 13:46:03.000000 pystencils-1.3/doc/conf.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.611307 pystencils-1.3/doc/img/
+-rw-r--r--   0 holzer     (502) staff       (20)   241908 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/c_backend.svg
+-rw-r--r--   0 holzer     (502) staff       (20)    80293 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/github_repo_card.png
+-rw-r--r--   0 holzer     (502) staff       (20)    10116 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/logo.png
+-rw-r--r--   0 holzer     (502) staff       (20)    14392 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/logo.svg
+-rw-r--r--   0 holzer     (502) staff       (20)    15916 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/logo_large.svg
+-rw-r--r--   0 holzer     (502) staff       (20)     5554 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/logo_no_text.png
+-rw-r--r--   0 holzer     (502) staff       (20)    27415 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/pystencils_arch_block_diagram.svg
+-rw-r--r--   0 holzer     (502) staff       (20)    21047 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/pystencils_stencil_four_points_with_arrows.svg
+-rw-r--r--   0 holzer     (502) staff       (20)    33850 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/staggered_grid.svg
+-rw-r--r--   0 holzer     (502) staff       (20)    27441 2023-06-25 13:46:03.000000 pystencils-1.3/doc/img/walberla_blocks.svg
+-rw-r--r--   0 holzer     (502) staff       (20)      418 2023-06-25 13:46:03.000000 pystencils-1.3/doc/index.rst
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.617980 pystencils-1.3/doc/notebooks/
+-rw-r--r--   0 holzer     (502) staff       (20)   217876 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/01_tutorial_getting_started.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)    82577 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/02_tutorial_basic_kernels.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)   118499 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/03_tutorial_datahandling.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)   433256 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/04_tutorial_advection_diffusion.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)  1773389 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/05_tutorial_phasefield_spinodal_decomposition.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)   787498 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/06_tutorial_phasefield_dentritic_growth.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)    25871 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/demo_assignment_collection.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)    48557 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/demo_benchmark.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)    51389 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/demo_derivatives.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)   846996 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/demo_plotting_and_animation.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)    54083 2023-06-25 13:46:03.000000 pystencils-1.3/doc/notebooks/demo_wave_equation.ipynb
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.621930 pystencils-1.3/doc/sphinx/
+-rw-r--r--   0 holzer     (502) staff       (20)      244 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/api.rst
+-rw-r--r--   0 holzer     (502) staff       (20)      303 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/ast.rst
+-rw-r--r--   0 holzer     (502) staff       (20)       80 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/configuration.rst
+-rw-r--r--   0 holzer     (502) staff       (20)      104 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/datahandling.rst
+-rw-r--r--   0 holzer     (502) staff       (20)       86 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/enums.rst
+-rw-r--r--   0 holzer     (502) staff       (20)       64 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/field.rst
+-rw-r--r--   0 holzer     (502) staff       (20)      102 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/finite_differences.rst
+-rw-r--r--   0 holzer     (502) staff       (20)      742 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/kernel_compile_and_call.rst
+-rw-r--r--   0 holzer     (502) staff       (20)      117 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/plot.rst
+-rw-r--r--   0 holzer     (502) staff       (20)        0 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/pystencils.bib
+-rw-r--r--   0 holzer     (502) staff       (20)      880 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/simplifications.rst
+-rw-r--r--   0 holzer     (502) staff       (20)       73 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/stencil.rst
+-rw-r--r--   0 holzer     (502) staff       (20)      860 2023-06-25 13:46:03.000000 pystencils-1.3/doc/sphinx/tutorials.rst
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.654749 pystencils-1.3/pystencils/
+-rw-r--r--   0 holzer     (502) staff       (20)     2021 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)      495 2023-06-25 13:47:28.654786 pystencils-1.3/pystencils/_version.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4895 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/alignedarray.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4043 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/assignment.py
+-rw-r--r--   0 holzer     (502) staff       (20)    29015 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/astnodes.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.629748 pystencils-1.3/pystencils/backends/
+-rw-r--r--   0 holzer     (502) staff       (20)      164 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6411 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/arm_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)    40797 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/cbackend.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2824 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/cuda_backend.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3539 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/dot.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2479 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/json.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3931 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/ppc_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3823 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/riscv_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4742 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/simd_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6137 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/backends/x86_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1707 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/bit_masks.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.632387 pystencils-1.3/pystencils/boundaries/
+-rw-r--r--   0 holzer     (502) staff       (20)      284 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/boundaries/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4344 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/boundaries/boundaryconditions.py
+-rw-r--r--   0 holzer     (502) staff       (20)    21004 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/boundaries/boundaryhandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8226 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/boundaries/createindexlist.py
+-rw-r--r--   0 holzer     (502) staff       (20)  2023077 2023-06-25 13:47:28.000000 pystencils-1.3/pystencils/boundaries/createindexlistcython.c
+-rw-r--r--   0 holzer     (502) staff       (20)     8006 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/boundaries/createindexlistcython.pyx
+-rw-r--r--   0 holzer     (502) staff       (20)     2031 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/boundaries/inkernel.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2406 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/cache.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9011 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/config.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.633202 pystencils-1.3/pystencils/cpu/
+-rw-r--r--   0 holzer     (502) staff       (20)      238 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/cpu/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    27644 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/cpu/cpujit.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10362 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/cpu/kernelcreation.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3758 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/cpu/msvc_detection.py
+-rw-r--r--   0 holzer     (502) staff       (20)    20020 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/cpu/vectorization.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.634265 pystencils-1.3/pystencils/datahandling/
+-rw-r--r--   0 holzer     (502) staff       (20)     3033 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/datahandling/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5636 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/datahandling/blockiteration.py
+-rw-r--r--   0 holzer     (502) staff       (20)    20890 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/datahandling/datahandling_interface.py
+-rw-r--r--   0 holzer     (502) staff       (20)    17403 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/datahandling/parallel_datahandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19549 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/datahandling/serial_datahandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2136 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/datahandling/vtk.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3482 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/display_utils.py
+-rw-r--r--   0 holzer     (502) staff       (20)      713 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/enums.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2624 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/fast_approximation.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.635376 pystencils-1.3/pystencils/fd/
+-rw-r--r--   0 holzer     (502) staff       (20)      880 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/fd/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14981 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/fd/derivation.py
+-rw-r--r--   0 holzer     (502) staff       (20)    21404 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/fd/derivative.py
+-rw-r--r--   0 holzer     (502) staff       (20)    15080 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/fd/finitedifferences.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11806 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/fd/finitevolumes.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7060 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/fd/spatial.py
+-rw-r--r--   0 holzer     (502) staff       (20)    46691 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/field.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1538 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/functions.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.636290 pystencils-1.3/pystencils/gpu/
+-rw-r--r--   0 holzer     (502) staff       (20)      509 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/gpu/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7984 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/gpu/cudajit.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3568 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/gpu/gpu_array_handler.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14629 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/gpu/indexing.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8765 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/gpu/kernelcreation.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2092 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/gpu/periodicity.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.637555 pystencils-1.3/pystencils/include/
+-rw-r--r--   0 holzer     (502) staff       (20)      413 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/PyStencilsField.h
+-rw-r--r--   0 holzer     (502) staff       (20)      114 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    28113 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/aesni_rand.h
+-rw-r--r--   0 holzer     (502) staff       (20)     2208 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/arm_neon_helpers.h
+-rw-r--r--   0 holzer     (502) staff       (20)      140 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/gpu_defines.h
+-rw-r--r--   0 holzer     (502) staff       (20)     3807 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/myintrin.h
+-rw-r--r--   0 holzer     (502) staff       (20)    58160 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/philox_rand.h
+-rw-r--r--   0 holzer     (502) staff       (20)     1007 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/include/ppc_altivec_helpers.h
+-rw-r--r--   0 holzer     (502) staff       (20)     6390 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/integer_functions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2830 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/integer_set_analysis.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3989 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/jupyter.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5676 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/kernel_contrains_check.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5133 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/kernel_decorator.py
+-rw-r--r--   0 holzer     (502) staff       (20)      545 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/kernel_wrapper.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19137 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/kernelcreation.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3190 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/node_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2680 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/placeholder_function.py
+-rw-r--r--   0 holzer     (502) staff       (20)    13234 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/plot.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4526 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/rng.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.638052 pystencils-1.3/pystencils/runhelper/
+-rw-r--r--   0 holzer     (502) staff       (20)      150 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/runhelper/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7898 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/runhelper/db.py
+-rw-r--r--   0 holzer     (502) staff       (20)    17806 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/runhelper/parameterstudy.py
+-rw-r--r--   0 holzer     (502) staff       (20)      286 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/session.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.638878 pystencils-1.3/pystencils/simp/
+-rw-r--r--   0 holzer     (502) staff       (20)     1352 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/simp/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    21879 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/simp/assignment_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10999 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/simp/simplifications.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6854 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/simp/simplificationstrategy.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3334 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/simp/subexpression_insertion.py
+-rw-r--r--   0 holzer     (502) staff       (20)      804 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/simplificationfactory.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9760 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/slicing.py
+-rw-r--r--   0 holzer     (502) staff       (20)      546 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/spatial_coordinates.py
+-rw-r--r--   0 holzer     (502) staff       (20)    17147 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/stencil.py
+-rw-r--r--   0 holzer     (502) staff       (20)    27160 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/sympyextensions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4300 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/timeloop.py
+-rw-r--r--   0 holzer     (502) staff       (20)    43948 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/transformations.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.639901 pystencils-1.3/pystencils/typing/
+-rw-r--r--   0 holzer     (502) staff       (20)     1292 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/typing/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4156 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/typing/cast_functions.py
+-rw-r--r--   0 holzer     (502) staff       (20)    13559 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/typing/leaf_typing.py
+-rw-r--r--   0 holzer     (502) staff       (20)      832 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/typing/transformations.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5816 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/typing/typed_sympy.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8885 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/typing/types.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9044 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/typing/utilities.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7760 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils/utils.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.628140 pystencils-1.3/pystencils.egg-info/
+-rw-r--r--   0 holzer     (502) staff       (20)     4626 2023-06-25 13:47:28.000000 pystencils-1.3/pystencils.egg-info/PKG-INFO
+-rw-r--r--   0 holzer     (502) staff       (20)     8462 2023-06-25 13:47:28.000000 pystencils-1.3/pystencils.egg-info/SOURCES.txt
+-rw-r--r--   0 holzer     (502) staff       (20)        1 2023-06-25 13:47:28.000000 pystencils-1.3/pystencils.egg-info/dependency_links.txt
+-rw-r--r--   0 holzer     (502) staff       (20)      312 2023-06-25 13:47:28.000000 pystencils-1.3/pystencils.egg-info/requires.txt
+-rw-r--r--   0 holzer     (502) staff       (20)       11 2023-06-25 13:47:28.000000 pystencils-1.3/pystencils.egg-info/top_level.txt
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.652535 pystencils-1.3/pystencils_tests/
+-rw-r--r--   0 holzer     (502) staff       (20)        0 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3624 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_Min_Max.py
+-rw-r--r--   0 holzer     (502) staff       (20)      617 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_abs.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1552 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_address_of.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2823 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_aligned_array.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6289 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_assignment_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1133 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_assignment_collection_dict_conversion.py
+-rw-r--r--   0 holzer     (502) staff       (20)      630 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_assignment_from_stencil.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2362 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_astnodes.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1213 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_bit_masks.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3186 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_blocking.py
+-rw-r--r--   0 holzer     (502) staff       (20)      962 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_blocking_staggered.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9946 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_boundary.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5333 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_boundary_indexlist_creation.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12127 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_buffer.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14808 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_buffer_gpu.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2310 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_conditional_field_access.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4847 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_conditional_vec.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4433 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_config.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1285 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_create_kernel_config.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1600 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_custom_backends.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.653408 pystencils-1.3/pystencils_tests/test_data/
+-rw-r--r--   0 holzer     (502) staff       (20)      410 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/datahandling_load_test.npz
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.653718 pystencils-1.3/pystencils_tests/test_data/datahandling_parallel_load_test/
+-rw-r--r--   0 holzer     (502) staff       (20)      304 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/datahandling_parallel_load_test/dst.dat
+-rw-r--r--   0 holzer     (502) staff       (20)      304 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/datahandling_parallel_load_test/src.dat
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2023-06-25 13:47:28.654003 pystencils-1.3/pystencils_tests/test_data/datahandling_parallel_save_test/
+-rw-r--r--   0 holzer     (502) staff       (20)      304 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/datahandling_parallel_save_test/dst.dat
+-rw-r--r--   0 holzer     (502) staff       (20)      304 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/datahandling_parallel_save_test/src.dat
+-rw-r--r--   0 holzer     (502) staff       (20)      410 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/datahandling_save_test.npz
+-rw-r--r--   0 holzer     (502) staff       (20)   473831 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/lenna.png
+-rw-r--r--   0 holzer     (502) staff       (20)     7609 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_data/test_vessel2d_mask.png
+-rw-r--r--   0 holzer     (502) staff       (20)    13241 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_datahandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6691 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_datahandling_parallel.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1786 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_derivative.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19953 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_dot_printer.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)      421 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_dot_printer.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1126 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_dtype_check.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1603 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_fast_approximation.py
+-rw-r--r--   0 holzer     (502) staff       (20)    22011 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_fd_derivation.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)     5616 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_fd_derivation_via_rotation.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)      735 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_fd_derivative.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8348 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_field.py
+-rw-r--r--   0 holzer     (502) staff       (20)      790 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_field_access_poly.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6443 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_field_equality.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)     3435 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_finite_differences.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1786 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_floor_ceil_int_optimization.py
+-rw-r--r--   0 holzer     (502) staff       (20)    26645 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_fvm.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4056 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_global_definitions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6604 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_gpu.py
+-rw-r--r--   0 holzer     (502) staff       (20)      954 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_helpful_errors.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2018 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_indexed_kernels.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2778 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_jacobi_cbackend.py
+-rw-r--r--   0 holzer     (502) staff       (20)      769 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_json_backend.py
+-rw-r--r--   0 holzer     (502) staff       (20)    35405 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_jupyter_extensions.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)      585 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_logarithm.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5890 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_loop_cutting.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2454 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_match_subs_for_assignment_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3833 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_math_functions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1659 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_modulo.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1284 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_move_constant_before_loop.py
+-rw-r--r--   0 holzer     (502) staff       (20)      487 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_nodecollection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2680 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_parameterstudy.py
+-rw-r--r--   0 holzer     (502) staff       (20)    87788 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_phasefield_dentritic_3D.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)      486 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_pickle_support.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1872 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_plot.py
+-rw-r--r--   0 holzer     (502) staff       (20)      706 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_print_infinity.py
+-rw-r--r--   0 holzer     (502) staff       (20)      513 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_print_unsupported_node.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2733 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_quicktests.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10198 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_random.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1885 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_sharedmethodcache.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2940 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_simplification_strategy.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6467 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_simplifications.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4674 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_size_and_layout_checks.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1060 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_sliced_iteration.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2449 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_slicing.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12457 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_small_block_benchmark.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)      839 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_source_code_comment.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3963 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_staggered_kernel.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14917 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_stencil_plot.ipynb
+-rw-r--r--   0 holzer     (502) staff       (20)     1138 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_stencils.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1704 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_struct_types.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1540 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_subexpression_insertion.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2462 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_sum_prod.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7403 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_sympyextensions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2561 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_timeloop.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3000 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_transformations.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1050 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_type_interference.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7652 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_types.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2389 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_utils.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10349 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_vectorization.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12821 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_vectorization_specific.py
+-rw-r--r--   0 holzer     (502) staff       (20)      278 2023-06-25 13:46:03.000000 pystencils-1.3/pystencils_tests/test_version_string.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1854 2023-06-25 13:46:03.000000 pystencils-1.3/pytest.ini
+-rw-r--r--   0 holzer     (502) staff       (20)      247 2023-06-25 13:46:03.000000 pystencils-1.3/release.sh
+-rw-r--r--   0 holzer     (502) staff       (20)      217 2023-06-25 13:47:28.654529 pystencils-1.3/setup.cfg
+-rw-r--r--   0 holzer     (502) staff       (20)     5198 2023-06-25 13:46:03.000000 pystencils-1.3/setup.py
+-rw-r--r--   0 holzer     (502) staff       (20)    70144 2023-06-25 13:46:03.000000 pystencils-1.3/versioneer.py
```

### Comparing `pystencils-1.2/.gitlab-ci.yml` & `pystencils-1.3/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - pip install sympy --upgrade
     - env
     - pip list
     - export NUM_CORES=$(nproc --all)
     - mkdir -p ~/.config/matplotlib
     - echo "backend:template" > ~/.config/matplotlib/matplotlibrc
     - mkdir public
-    - py.test -v -n $NUM_CORES --cov-report html --cov-report term --cov=. -m "not longrun" --html test-report/index.html --junitxml=report.xml
+    - py.test -v -n $NUM_CORES --cov-report html --cov-report xml --cov-report term --cov=. -m "not longrun" --html test-report/index.html --junitxml=report.xml
     - python3 -m coverage xml
   tags:
     - docker
     - cuda11
     - AVX
   coverage: /Total coverage:\s\d+.\d+\%/
   artifacts:
@@ -152,45 +152,42 @@
     reports:
       junit: report.xml
 
 arm64v8:
   extends: .multiarch_template
   image: i10git.cs.fau.de:5005/pycodegen/pycodegen/arm64
   variables:
-    PYSTENCILS_SIMD: "neon"
+    QEMU_CPU: "cortex-a76"
   before_script:
     - *multiarch_before_script
     - sed -i s/march=native/march=armv8-a/g ~/.config/pystencils/config.json
 
 ppc64le:
   extends: .multiarch_template
   image: i10git.cs.fau.de:5005/pycodegen/pycodegen/ppc64le
-  variables:
-    PYSTENCILS_SIMD: "vsx"
   before_script:
     - *multiarch_before_script
     - sed -i s/mcpu=native/mcpu=power8/g ~/.config/pystencils/config.json
 
 arm64v9:
   # SVE support is still unreliable in GCC 11 (incorrect code for fixed-width vectors, internal compiler errors).
   extends: .multiarch_template
   image: i10git.cs.fau.de:5005/pycodegen/pycodegen/arm64
-  variables:
-    PYSTENCILS_SIMD: "sve256,sve512,sve"
   before_script:
     - *multiarch_before_script
     - sed -i s/march=native/march=armv8-a+sve/g ~/.config/pystencils/config.json
     - sed -i s/g\+\+/clang++/g ~/.config/pystencils/config.json
 
 riscv64:
   # RISC-V vector extension are currently not supported by GCC.
   # Also, the image is built without the libomp package which is not yet available on Ubuntu.
   extends: .multiarch_template
   image: i10git.cs.fau.de:5005/pycodegen/pycodegen/riscv64
   variables:
+    # explicitly set SIMD as detection does not appear to work on QEMU
     PYSTENCILS_SIMD: "rvv"
     QEMU_CPU: "rv64,v=true"
   before_script:
     - *multiarch_before_script
     - sed -i 's/march=native/march=rv64imfdv/g' ~/.config/pystencils/config.json
     - sed -i s/g\+\+/clang++/g ~/.config/pystencils/config.json
     - sed -i 's/fopenmp/fopenmp=libgomp -I\/usr\/include\/riscv64-linux-gnu/g' ~/.config/pystencils/config.json
```

### Comparing `pystencils-1.2/CONTRIBUTING.md` & `pystencils-1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/COPYING.txt` & `pystencils-1.3/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/PKG-INFO` & `pystencils-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystencils
-Version: 1.2
+Version: 1.3
 Summary: Speeding up stencil computations on CPUs and GPUs
 Home-page: https://i10git.cs.fau.de/pycodegen/pystencils/
 Author: Martin Bauer, Jan Hönig, Markus Holzer
 Author-email: cs10-codegen@fau.de
 License: AGPLv3
 Project-URL: Bug Tracker, https://i10git.cs.fau.de/pycodegen/pystencils/-/issues
 Project-URL: Documentation, https://pycodegen.pages.i10git.cs.fau.de/pystencils/
@@ -78,26 +78,26 @@
 ```bash
 pip install pystencils[interactive]
 ```
 
 Without `[interactive]` you get a minimal version with very little dependencies.
 
 All options:
-- `gpu`: use this if an NVIDIA GPU is available and CUDA is installed
+- `gpu`: use this if an NVIDIA or AMD GPU is available and CUDA or ROCm is installed
 - `alltrafos`: pulls in additional dependencies for loop simplification e.g. libisl
 - `bench_db`: functionality to store benchmark result in object databases
 - `interactive`: installs dependencies to work in Jupyter including image I/O, plotting etc.
 - `doc`: packages to build documentation
 
 Options can be combined e.g.
 ```bash
 pip install pystencils[interactive, gpu, doc]
 ```
 
-pystencils is also fully compatible with Windows machines. If working with visual studio and pycuda makes sure to run example files first to ensure that pycuda can find the compiler's executable.
+pystencils is also fully compatible with Windows machines. If working with visual studio and cupy makes sure to run example files first to ensure that cupy can find the compiler's executable.
 
 Documentation
 -------------
 
 Read the docs [here](https://pycodegen.pages.i10git.cs.fau.de/pystencils) and
 check out the Jupyter notebooks in `doc/notebooks`. The **Changelog** of pystencils can be found [here](https://i10git.cs.fau.de/pycodegen/pystencils/-/blob/master/CHANGELOG.md).
```

### Comparing `pystencils-1.2/README.md` & `pystencils-1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,26 +48,26 @@
 ```bash
 pip install pystencils[interactive]
 ```
 
 Without `[interactive]` you get a minimal version with very little dependencies.
 
 All options:
-- `gpu`: use this if an NVIDIA GPU is available and CUDA is installed
+- `gpu`: use this if an NVIDIA or AMD GPU is available and CUDA or ROCm is installed
 - `alltrafos`: pulls in additional dependencies for loop simplification e.g. libisl
 - `bench_db`: functionality to store benchmark result in object databases
 - `interactive`: installs dependencies to work in Jupyter including image I/O, plotting etc.
 - `doc`: packages to build documentation
 
 Options can be combined e.g.
 ```bash
 pip install pystencils[interactive, gpu, doc]
 ```
 
-pystencils is also fully compatible with Windows machines. If working with visual studio and pycuda makes sure to run example files first to ensure that pycuda can find the compiler's executable.
+pystencils is also fully compatible with Windows machines. If working with visual studio and cupy makes sure to run example files first to ensure that cupy can find the compiler's executable.
 
 Documentation
 -------------
 
 Read the docs [here](https://pycodegen.pages.i10git.cs.fau.de/pystencils) and
 check out the Jupyter notebooks in `doc/notebooks`. The **Changelog** of pystencils can be found [here](https://i10git.cs.fau.de/pycodegen/pystencils/-/blob/master/CHANGELOG.md).
```

### Comparing `pystencils-1.2/binder/environment.yml` & `pystencils-1.3/binder/environment.yml`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Environment with all dependencies to use pystencils
 #
 #
 # Download conda at https://conda.io/miniconda.html and create this environment by running:
 #     conda env create -f conda_environment_user.yml
 #     . activate pystencils
 #
-# If you have CUDA installed and want to use your GPU, uncomment the last line to install pycuda
+# If you have CUDA or ROCm installed and want to use your GPU, uncomment the last line to install cupy
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 name: pystencils
 dependencies:
   # Basic dependencies:
   - python >= 3.8
@@ -28,8 +28,8 @@
   - pip:
       - islpy # used to optimize staggered kernels
       - py-cpuinfo # get cpu info like cache sizes, supported vector instruction sets, ...
       - graphviz  # can show abstract syntax trees as formatted graphs
       - ipy_table  # HTML tables for jupyter notebooks
       - pyevtk # VTK output for serial simulations
       - blitzdb # file-based No-SQL database to store simulation results
-      #- pycuda # add this if you have CUDA installed
+      #- cupy # add this if you have CUDA or ROCm installed
```

### Comparing `pystencils-1.2/conftest.py` & `pystencils-1.3/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 collect_ignore = [os.path.join(SCRIPT_FOLDER, "doc", "conf.py"),
                   os.path.join(SCRIPT_FOLDER, "pystencils", "opencl", "opencl.autoinit")]
 add_path_to_ignore('pystencils_tests/benchmark')
 add_path_to_ignore('_local_tmp')
 
 
 try:
-    import pycuda
+    import cupy
 except ImportError:
-    collect_ignore += [os.path.join(SCRIPT_FOLDER, "pystencils_tests/test_cudagpu.py")]
-    add_path_to_ignore('pystencils/gpucuda')
+    collect_ignore += [os.path.join(SCRIPT_FOLDER, "pystencils_tests/test_gpu.py")]
+    add_path_to_ignore('pystencils/gpu')
 
 try:
     import waLBerla
 except ImportError:
     collect_ignore += [os.path.join(SCRIPT_FOLDER, "pystencils_tests/test_aligned_array.py"),
                        os.path.join(SCRIPT_FOLDER, "pystencils_tests/test_datahandling_parallel.py"),
                        os.path.join(SCRIPT_FOLDER, "doc/notebooks/03_tutorial_datahandling.ipynb"),
```

### Comparing `pystencils-1.2/doc/conf.py` & `pystencils-1.3/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 copyright = f'{datetime.datetime.now().year}, Martin Bauer, Markus Holzer, Frederik Hennig'
 author = 'Martin Bauer, Markus Holzer, Frederik Hennig'
 # The short X.Y version (including .devXXXX, rcX, b1 suffixes if present)
 version = re.sub(r'(\d+\.\d+)\.\d+(.*)', r'\1\2', pystencils.__version__)
 version = re.sub(r'(\.dev\d+).*?$', r'\1', version)
 # The full version, including alpha/beta/rc tags.
 release = pystencils.__version__
-language = None
+language = 'en'
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', '**.ipynb_checkpoints']
 default_role = 'any'
 pygments_style = 'sphinx'
 todo_include_todos = False
 
 # Options for HTML output
```

### Comparing `pystencils-1.2/doc/img/c_backend.svg` & `pystencils-1.3/doc/img/c_backend.svg`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/github_repo_card.png` & `pystencils-1.3/doc/img/github_repo_card.png`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/logo.png` & `pystencils-1.3/doc/img/logo.png`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/logo.svg` & `pystencils-1.3/doc/img/logo.svg`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/logo_large.svg` & `pystencils-1.3/doc/img/logo_large.svg`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/logo_no_text.png` & `pystencils-1.3/doc/img/logo_no_text.png`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/pystencils_arch_block_diagram.svg` & `pystencils-1.3/doc/img/pystencils_arch_block_diagram.svg`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/pystencils_stencil_four_points_with_arrows.svg` & `pystencils-1.3/doc/img/pystencils_stencil_four_points_with_arrows.svg`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/staggered_grid.svg` & `pystencils-1.3/doc/img/staggered_grid.svg`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/img/walberla_blocks.svg` & `pystencils-1.3/doc/img/walberla_blocks.svg`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/notebooks/01_tutorial_getting_started.ipynb` & `pystencils-1.3/doc/notebooks/01_tutorial_getting_started.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977292500591454%*

 * *Differences: {"'cells'": "{5: {'outputs': {0: {'text': ['4.78 ms ± 9.53 µs per loop (mean ± std. dev. of 7 "*

 * *            "runs, 100 loops each)\\n']}}}, 8: {'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAARUAAAEnCAYAAACHXNdEAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAAP7UlEQVR4nO3df3DUdX7H8dd3f2Q32SwJbORnBWTEg0tPfulMvZYTM5I7q9AZB0fr1VhuLNibttC5mwpl7Iw9O/UPtPbu8Begp5m7Gx2tZ9Ub6zltbcc5ZSgWjh6KEUEQgfyAbIjZze5+v/0jBo […]*

```diff
@@ -66,15 +66,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "4.92 ms \u00b1 124 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 100 loops each)\n"
+                        "4.78 ms \u00b1 9.53 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 100 loops each)\n"
                     ]
                 }
             ],
             "source": [
                 "%%timeit \n",
                 "numpy_kernel()"
             ]
@@ -116,15 +116,15 @@
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 300x300 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -175,15 +175,15 @@
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "1.01 ms \u00b1 24.6 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 1,000 loops each)\n"
+                        "987 \u00b5s \u00b1 5.12 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 1,000 loops each)\n"
                     ]
                 }
             ],
             "source": [
                 "%%timeit\n",
                 "pystencils_kernel()"
             ]
@@ -256,15 +256,15 @@
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle x^{2} \\left(x + y + 5\\right) + x^{2}$"
                         ],
                         "text/plain": [
                             " 2                2\n",
                             "x \u22c5(x + y + 5) + x "
                         ]
@@ -289,15 +289,15 @@
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAI0AAAAXCAYAAAA2o8yAAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAABJ0AAASdAHeZh94AAAFBklEQVR4nO2aa4hVVRTHf44WTRmFREhkDyrsg5qVpkmKPSYrCUUrSLImNDKUNDNzylr9yVJTa7AwJCKtvpQivSYzNEJMC6V8ZGVYDRRYJo6iaC+dPqx983rmzuPM3feRzB+Gzex99tr/tc66e6299unU2NhIBzqQBl3ymSxpInA/cEHo2g7MMrO6PHkVFJJqgFFAT+BP4HOgxsy+LimxMkFr9qnIU/4vwAzgSqAf8AnwjqQ+ecotNIYCi4BBwHXAP8BqSd1KSaqMMJQW7NMpdniStBf3ysVRBRcQkroC+4GRZvZ+qfmUG5L2ySs8JQR3Bu4AugLrY8ktEk7Hd929pSbSVkgaDEzBd4NuOPdtQK2ZfRh5uePsk7fTSOoNbABOAQ7g3rgtX7lFRi2wGY/dZQ9JM4GngT3AB8Au4Czgcjy0xHaaWrLsE2On2QH0Bc4ERgOvSxqaNqmUVA28BlxrZp9G4NXWdecBQ4DBZnakSGtW005dJd2OO8xqYJSZHUiMnxSJZkZeE/t0STzwMVAFjDazFVn9nXAl7wHmmtmMzJiZ/QXsDP9uktQf3zbHxyTfGtrDXdIC4C785e1MiETSw8B8YJqZLcgx3hPYCnxhZkMiq9QEkiqAucAhYEzSYQDM7O8c81LbJozntE/y9PQIcBSYFXKUDOYHwa8kBedABR6qio1U3CUt5JhBvmlG5rrQDmxm/EWgMzApH+IpMAi4EA8/DZKGS3pU0mRJV7cwL/V7bck+x+00ZrZF0htB0FhgiaTHgKnA28CEhOA5QB3wM54sjcFj6vDW9Y+LNNwlLcINMhLYK6l7GDpoZgezxH4JHAYGJNcLYaIKWGhmW+NrlBP9Q/tb4NY7wWktcJuZ/Z7d34732qJ9ctVpZgJ/AE9JmgQ8A6wCxprZ0cSz3YE38bxmTVDqZjNb2SYTxEdbuT+AO/kaPInM/E3LFha2+o1AD0nnZPolnQY8D+wGniyYNk1xdmgnAJXADbgevXA9hwDLmpmb5r22aJ+cdRpJs/GiHfjxucrMDqVWsRlIqgfOTzFlqZlVt1F2VO6SngVqyMoHJM0FpgP3mtmSVubXE0lXSc9xLNRcYWZbssYqge+Bc4FBZrYhx/wotmnu9JS9vY2L6TABtfhpKxt9gRHAUqA+MbY5hezY3D8L7QBghaRLgYfwMsPSNsyvJZ6uDaH9MdthAMzssKRVwDjgqsAviSi2aeI0ku7EE6Rf8fAzGd+uosHManOsW40bckl7j9wF4r4eaORYMvwSnvxONLNWy+mRdd0R2n3NjGecqjLHmtFsc1xOI+kW3Pu3A32A74Dx4ddV1igUdzNrAL4F+kkaA1wPLDazr/Kk3B6sxe+BLpF0co7xXqGtz+6MbZv/nEbSNcBy/BLyxpCBP4HvRnPaI7xYKAL3dcCpwGK8CjszgszUMLM9wFvAGSQScElVwDD8juijrP7otqkIgi/Dy9H78eRoVyC5HNgEjAh3HWWHInHP5DVd8cvYUt5RTcWLqY9LWitpvqRlwErgCHCfme2DwtmmQtLF+NGrERhmZj8knqkJ7by0wguNInL/KbQbgVfzlJUXzGw3npS/APQAHsQ/X6jDS/3LoLC2if5pxIkISe/hBcuBZrax1HxKjXw/wjrhEZLfW4GXOxzGEe17mhMJks7Dr0QuAu7GTx3TS0qqjNDhNLlxEzAbr4e8C0wpQIHzf4uOnKYDqfEvcwBygSAVIEgAAAAASUVORK5CYII=\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAI0AAAAXCAYAAAA2o8yAAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAABJ0AAASdAHeZh94AAAFB0lEQVR4nO2ae4hVVRTGfzMaVho9oDAoCyqUKBky85HKpExWEloplGBNaEYpWOKj6fXx0cPMNC0rJohG6q+yoTQrRSOitLDS1Cihx1SC0UsFsadOf+xz5c6ZM3Pn3nvuvZPMB8Nm9j577W+ts+7aa699qlpbW+lBD/JB72Im254F3A6cG3V9ATwsaV2RvEoK2w3A9cBA4C/gI6BB0q6KEusmyGWf6iLl7wEWApcAlwLvAq/bHlyk3FKjFngWGAmMBf4FNto+rZKkuhFq6cQ+VWlvT7Z/J3hlY6qCSwjb/YADwCRJayvNp7shbp+itqeY4F7AFKAfsDktuWXCSYSou6/SRLoK2+OA2cAI4FTgN2AnsELSWykv18Y+RTuN7YuBLcDxwEHgOkk7i5VbZqwAthP06Paw/Tgwn5AerAF+BU4HhhC2lrSdpo190og0u4Ea4GRgMrDKdm2+SaXteuBF4ApJ76XAq6vrLgNGAaMkHS7TmvUUqKvt2wgOswqYKenv2PhxKdHMyGtnn96xBzYAdcBkSa9l9VcRlLwFWCzpnsxYRPrr6N9PbQ8F7gamp0k+FwrhbvtJ4EbCy/s2QeZcYCkwT9LShPGBwA7gY0ljUlapHWz3AR4BfiDBYQAk/ZMwL2/bROOJ9omfnuYDR4CHohwlgyciwc/HBSegGuiT45lSIC/utlcANwFjJX3VgcwPo3Z4B+NPA70IuUU5UEfYhpqBI7Yn2F5oe47tEZ3My/u9dmafNpFG0ue2X4oETQOabN8LzAVeAe6ICX4MWAf8SEiWphL21Am59U8X+XC3/Uz0zCRgn+3+0dBBSQezxH4G/AEMi69newrhJT4laUf6GiViaNT+CWwDLopxep8QTX7J7i/gvXZqn6Q6zQMRKdmeTQiH64Fpko7Enu0PvEzIazZFSl0t6e0umSB9dJX7nQQn3wTszfqbly0sCvVbgbNtn5npt90XWAb8DDxYMm3a44yonQ+0AqMJegwGNgBjgFc7mJvPe+3UPol1GtuLgEy42gzUSTqUt4odwHYLcE4eU1ZJqu+i7FS5234UaABukNQc9S0GFgC3SmrKMb+FlHS13QjMJFRpB0lqyRo7kfDjPQsYKandSTAt23R0esoOb9PTdJgIy4FTYn01wETCqaAlNrY9D9lpc8/kNcOAZtuDCIn+FgLXXFhOerruj9pt2Q4DIOmQ7fWEA8hlJJcPUrFNO6exPZWQIP1E2H7mENvzioWk5Qnr1hMM2VTokbtE3DcTtoJMMrySkPzOkpSznJ6yrrujdn8H45ni5AkJa6ZmmzY5je1rgCZgF2Gf3A3MiI6W3Rql4i5pH/AlMCQy/DigUdK24hgXhE0EB77QdlI+mkmMv8vuTNs2Rxe2PQpYTagyjo8y8PsJ0WhxIcLLhTJw/wDoCzQSqq/3pSAzb0j6HlgLDCBEiqOwfSUwnhCF3snqT9021ZHgGuBNwqVUnaS9EcnVwCfARNujC1mg1CgT90xe049wGVvJO6pZhBLHMtsbbS+xvZpwdXAYmCHpAJTONtW2zyd4ZivBE7+JPdMQtUvyFV5qlJF7JtxvBV4oUlZRkLSHcMe0EriAEHFqCRHo8kzFt5S2Sf3TiGMRttcQCpbDJW2tNJ9Ko9iPsI55RMnvtcBzPQ4TkNr3NMcSbA8gXImcB9xM+Ix1QUVJdSP0OE0yrgIWEU4ibwB3laDA+b9FT07Tg7zxH/RCc51argrkAAAAAElFTkSuQmCC",
                         "text/latex": [
                             "$\\displaystyle x^{3} + x^{2} y + 6 x^{2}$"
                         ],
                         "text/plain": [
                             " 3    2        2\n",
                             "x  + x \u22c5y + 6\u22c5x "
                         ]
@@ -314,15 +314,15 @@
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAHsAAAAXCAYAAAAr8TBeAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAABJ0AAASdAHeZh94AAAFN0lEQVR4nO2ae7CWUxTGf+cUI9VEbg2K3GKmwRCV0aF0ZDSm3P7QiBDDiJJQLj09htRUOhNqQqP4R1SDErlMVIrJJZEwUUMjYrq45ZLyx95fHe95v3Pqu51M55n5Zn2z19rver693r322nt/Zdu3b6cBewca59PZ9jDgEqAd8CfwLjBM0qcF4NaAAqM8z/7nAhOBs4BuwFbgDdst83xuA4qAskKmcdvNgM1Ab0mzU/RPAxcAbSX9VjDHDagB26cD7wP9JU2BPNN4CpoTssWGFOcdgCuBIQ2Bzh22uwCDCNm0JWGsPwGqJM3N2En6wPYLwAO2p0v6Nd80nkQVsIywdicxEvgZmFRgn3sNbN8LLAAqgFeBccBs4EDCkprEQ0Ar4FYoYBq3PYYwc7tIWpXQnQB8Djwp6YaCOKybTz/gKaCrpLdK4bM25MvH9uXAc8AbwCWSfkno95H0d0q/lcD+wDGNE4rXgErgUkmzqrWXRaJXA6MlDU30G0cIdNdkoCOuBcqA6Vl+SE5+iwHbtwNjCcvNuBR9O2A58J6kimLziT7LgdHA70CfZKAB0gId8SwwAuieTON3ANsIeb5RtfaxhAF/IiXQE9gZ6M+yOOwO/EN6es/JbxGxKMpOWfSPAI2AAaWhA4T1uS0wF9hou6ftu2wPtN25jr7vRFn5n2BL+hh4BjgJ6Atg+25gMCGF3Fjd3vZEoB9wBbDBdqv4aVbNpilwKrAyW2G2u36LjA+BLUDHpCKm0krgMUnLS8jpjCh/IPCbA4wi1EiLbb9t+5AsfZdGWZFWoN0L/AGMsD0AeBCYB/SVtC1hexOhAn8TWFftM6SazRGEmbCujh+0O36LhpgOlwKtbR+eaY8v7cPAemB4qfhEHBrljUATQqZsDrQnjFEF8HxaR0mbCePapsbWS9Ja21XAUELKWkwoCP5KsS3bBaIHRbmxNqPd8ZuE7TXAUVnU820n26ZJ6lfLI98hDGAnIFNDDAeOBK6JA1hKPpmlrQy4LGZCgBW2Lwa+BM6x3VnSkpT+G4DDsu2zf6z2/TpJv9dCpC5siXK/XbDN1W8VcECi7VSgFzANWJPQLavjeZl1riMwy/aJwG3Akvi8UvPJTJSvqwUaAElbbM8DrgPOjByTaAJsqRFs21cQCqPvCXu0gYR0nSvWR3lQbUb5+JVUlfK8foTBnZrDVmcxsJ2dRdqjhNl1s6Q696pF4PNFlJuy6DMvQ5MUv+WEF291eUJxIeHNWwGcTNgb949vdq5YR5ix7bIZFMlvzpC0EVgJdLDdBzgPmCzpo/rgQzhI2Qocb3vfFH37KNek6NoR0v+yHcG2fTYwA1gLnC/pR+A+wpHqqFxZxpmwADjY9nFJfbH8FgCLCIcRk4GfCAVkvUDST4QzihYkikPblUAPwp3EqyndM9lpfnnscAqhnN8MVEpaF53MIBym94pnsrliZpQ9EkSL7TcfZNbtZoRr2xrn/SXGYGAVcI/tBbbH2n4eeIVwhnG9pE0p/c6P+hfL42ybR1ijekj6KmE8LMoxeRCdSdgjXpVpKJHffLA6yqXAlHrisAOS1hMKxvFAa8J5dzfgZcIRdY2tl+0WQG9gjqRvC3rFWRviHx1GAqfV49q3y7D9EtAT6CRpaV32eyJs3wJMACokLSz0rVdtGA98A9xfQp85IRZlFwGT/seBbkLIjjMlLYTC32dnhaQ/bPcFutpuuqfdadtuA/QBjiUsNyuAO+uVVH44GngcmJppKFka39Nh+wZC5b0JeB0YJOm7eiVVYDQEey/CvxiiNb+5640IAAAAAElFTkSuQmCC\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAHsAAAAXCAYAAAAr8TBeAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAABJ0AAASdAHeZh94AAAFMklEQVR4nO2afazWYxjHP+eUkTIviQxhXsLMmqQOlV6czmiUxkZblF42imhFefv6Mi9Jb0irZTrzT6hGpVWysAo7KJVVf1DUHCtURoV0/HH/nvb4nd9zTj1vJ+t8t2fX89zXfd/X9buv33293PdTUlNTQyOODTTNZbDtcUA/oC3wJ/AZME7Shjzo1og8ozTH8d2A14BrgR7AAWC57dNynLcRBUBJPt247RbAHqCvpIUJ/ErgRuACSX/kTXAjasF2e+ALYKikWZCjG0/ASQRvsStBeAdgADC60dDZw3ZPYARQBpwK/AKsB6ZKWpzqJ+lL2+8Cz9ieI+n3XN14HFOBtcCnCbxngd+A6XmWeczA9ovAcuBqYAEwEXgfaEUIqXE8D7QGHoA8unHbk4A7gM6SvovxLgE2AbMkDcuLwPr1GQi8AXSX9FExZNaFXPWxPRSYCVQCwyT9FeMfJ+nvhHEbgROBC5rGGMuAcuA2SfPS2ksiRe8GxksaGxs3mWDo7nFDR7gHKAHeyvAgWcktBGyPIuyY0ZImJvDbAuuAzyV1LbQ+kczjCZ7xBxIMDZBk6AhzgKeA8rgbHwMcJPj5JmntLxEWfGaCoacCdwI9JG3KIPAG4B9CaZaEI5ZbQKyKaKcM/FeAJoS4WSyUE1z1fOCg7d62H7E90nZZPWNTz/NfY0v6GngTuIyQTGH7UWAU8DZwb3p/29OAQUB/YJft1tGnRVqf5kA7YGOmxOxI5RYYXwH7gI5xhu3bCQs/TdK6IurUIaL7gTXAIuAFYAqw2vbHtltlGFsV0a5JCdoT0aSyPYLgPpYCAyQdjPW9j5CBfwhUp31Gp/U5m7ATqut5oCORWzBE7rAKONf2Wan26KWdBOwAniyWPhHOiOgYoAboQlj3K4FlQFfgnaSBkvYQ1rVNrdJL0jbbU4CxBJe1GuiXIU6UHIaiLSNaqxzLVm4ctrcC52Vgr7Adb6uUNLCOKVcRFrCM4DohGPgcYFC0gMXUJ7UpDwC3SNoa/V5v+1ZgM3C97TJJSZXQr8CZmersnWnfB0vaW4ci9WFfRE84jL7Zyp0CnBJrawf0IWSvW2O8tfXMl4pzHYH5ti8FHiKUlJUNoM/uiK5JMzQAkvbaXgoMBq4huextBuyrZWzb/QmJ0U+EGm0kucXMHRFtWVenXORKmpIw30DC4s7OotRZTXCXqSTtVUIoGi6p3lq1APpsjujuDPyU12yWILeU8OJtKY0xbgJmAxsI8WAzMCQqN7JFNWHHZpyjQHKzhqRdwEagffQS9gRmSFrTEPoQcqIa4PLIeHFcEdEtCby2hLJ37aGBtjsDc4HtQIWkncDjhCPV8dlqGe2ET4DTbV8U5xdKbh6wEmgOzAB+Bh5rKEUkfQ8sBNoQPN4h2O4FVBB2/ZKE4SnvtKI0GtCOkM7vAcolVUdC5hIO0/vY7pKDvqmDkoqYooWWmwtScbsF4dq2zgSzCBgObAMm2V5ue4LtucBiwhnGkAyJY6+I/15ptNuWENxEhaRvY53HRXRCDorOI8Tuu1INRZKbC1IusQp4vYF0OARJ24H2hPzhYsIO70bY8delnzymYPtkoC+wSNK2vF5x1oXojw7PAVc1YOw7bNheAPQGOkmqqq//0Qjb9wMvA10krcz3rVddmEw42326iDKzQpSU3QxM/x8buhnBO86TtBLyf5+dEZL22x4AdLfd/Gi707bdhnDseyEh3HwDPNygSuWG8wm3ZLNTDUVz40c7bA8jZN67gQ+AByX92KBK5RmNxj6G8C8PHDfc7bZAEwAAAABJRU5ErkJggg==",
                         "text/latex": [
                             "$\\displaystyle x^{2} \\left(x + y + 6\\right)$"
                         ],
                         "text/plain": [
                             " 2            \n",
                             "x \u22c5(x + y + 6)"
                         ]
@@ -339,15 +339,15 @@
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle x^{2} \\left(x + \\cos{\\left(x \\right)} + 5\\right) + x^{2}$"
                         ],
                         "text/plain": [
                             " 2                     2\n",
                             "x \u22c5(x + cos(x) + 5) + x "
                         ]
@@ -371,15 +371,15 @@
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle x^{2} \\left(x + y + 5\\right) + x^{2} = 1$"
                         ],
                         "text/plain": [
                             " 2                2    \n",
                             "x \u22c5(x + y + 5) + x  = 1"
                         ]
@@ -397,15 +397,15 @@
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAHsAAAAfCAYAAADHorIzAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAABJ0AAASdAHeZh94AAAEpUlEQVR4nO2ba4hVVRiGnzEtukFYSf0QLSxIDK2syPKSNRn2Q7vYXRIssIgUSTCbentLUdFohn72ozErKEWpxrwgXSwmLEkthBK1qSRLB0cJLFKbfqx14ng4c9wzc86eo7Mf2Kx91trrm5f97bXXt9a3p6a9vZ2M3kHf/B+2zwfG5lVtlnQgXUkZALbHAHOA64BLgSmSVibodzkwNPdbUlPuvE/BtYOAFWVRm9FdzgW2A093sf8A4KP8ir5FLjqe/zRk9AyS1gJrAWx3pt8eYI/twYVthSM74zSm2MjuVdgeDcwCRgH9gYPA90C9pI97UFrZ6dXOtl0HvAK0Ak3APuAi4BpgHJA5+3TA9hSCozcC90j6s6C9XxftTgPeBG6V9Fk3ZZaV1JxtewNQC9wraVVefQ3h5jwGLJY0NwUtfYDFwBHg4UJHA0g6WmkdaZPmyJ4DfAvMt/2BpOOxfinB0W+k4ejIKOAyYCXQZvsuYBjwN/C1pK9S0tEhts8DhuRVDbY9Ajgo6Zeu2EwtGpe0HVgOXAVMBbA9D5gNvA/MSEsLcH0s/yA8gE3AIqAeaLb9ue2LU9RTjJHA1ngALInnL3fVYNpzdh3wAPBSfHIXAOuBqZL+TVHHgFjOAH4Cbgc2EzaVXgUmEDaXxqWo6QTifF9TTpuJnG27hXAjkvKOpEcLKyXttV0PzAVeB5oJwdE/aWmInBHLGuC++NYB2GH7bmAnMNb2TaVe6SfR9GmRzZBlkqYlEV8Jko7s3YT5LCm/lWjL32ufLulID2hoi+WePEcDIOkv2+uB6cANQKn5ux64oKBuBDAJWAa0FLRtK2Gr4iRytqTbyvHHbD9ECMh+By4BZgJPpqkh8mMsD3XQnnsYzi5lRFJ9YV1cek0CGnvz0msi4WnfAYwHNgGP226Q9ENaOiKbgGPAFbbPLDKNDItlS1qCbHc71yyp5ByfirNt30JY5uwF7pB0wPYLhCBoETA5DR05JLXafg94BHiREDjmtNYSArTDwLoUNZ00GLM9kLCiGQAcBZy/Z3EyKr70sj2csLQ5DNRK2gcQc7NbgElxfzptZgO7gOdtb7K91PYKQqbpOPCEpEM9oKsUx4CZkoYSNqgabJ+TtHNFnW17CGFp1Q5MkLS74JLnYrmkkjqKIWk/cCPwGjAQeIYwvawBRkuqury+pH25gDLqbyPs5Seioq9xSbsIgVhH7Rsp81qyM0g6SBjhs8tosxFoLJe9jrA9EugH/Jq0T5bPPgWxfSHwFmHpmjiwy5x9imH7LGA1sFBSc2f69toUZzUS065vA1dK+jnWNQATCcmbVsIU8Ymk5Z21n43s6mIl4SuZOgDbzwIPAnfGr3xvJuQWJtveFo+rkxrPRnYVIak9ZgLX2N4NzAPG51Yxkr6kGwM0G9lVhqQNwDfAfOB+SVvKZTtzdpVhezwwnOCb/eW0nTm7ioi7jauAp4APCfn+slFszu5ne1Y8X52LCjMqi+1BhK9Zl0haZnsrsM32aElfdMLOtcAYwmfRJ1A4sncSXiHr4tHaVfEZybHdn3C/myQtAJD0HSE6X9hJcy3R1ruET8D+pyb7L87ew39WYqU0g6OV0QAAAABJRU5ErkJggg==\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAHsAAAAfCAYAAADHorIzAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAABJ0AAASdAHeZh94AAAElUlEQVR4nO2bbYhUVRjHfyuFSH4owaggLbBAERS0YH2prWU1erMXI4oWLTWIiiJcMDH+/C1Js2Kl+tKHWhO/pJKkmUovirFCZrupSBJLppKKvegX20qdPpyzMQw768x65+7o3B8M595z7nnuwzzzPOc855ypy+VyZNQGl+Xf2L4W2ADsBnLAakk7BkKxWsf2bcB8YAJwHfCkpLYS+tUDs+LtROBhSb9AgbGBwVH4FEndCemd0T+GAvuAj+KnJCTtBHYC2M4BQ3raCo2dUSVI2gRsArDdloTMQUkIybg4yDwbsN0IPAfUA1cBvwN7gRXRwy4Jat7Ytt8AWoAjwKfAb8BwwtylgRhKLwVq2ti25xEMvRJ4WtI/Be2X90PmbOBD4A5J2xJQMzFSM7btrUATMFPSurz6OsKXMwtYJmlBSvoMBpYAh+jF0ACS/k1Dl7RI07NbgO+BV22vl3Q21r9JMPT7aRk60kQI163AOdv3AGOBbuDbmMIMGLaHAqPi7SBghO3xwB+SDvVHZmqzcUk/AKuA0UAzgO2FwEvAx8AzaekSuSWW3UAHsBFYSjB+u+3ttoenrFM+E6NeHYRc2fF6cX8Fpj1mvwI8Cij+cpcAW4BmSedS1uXqWLYA+4GpQCdwIyHaTAPWECZpqRPH+7okZZZkbNsHgZFlyF0t6YnCSkmHbbcCC4B3gHbgod7Gy0rpkEdPVDsD3C/pYLzfa/tB4ABwu+36YiH9PDp9bbuwbqWk2SXoXhFK9ewuQrgrlV/7aDuRdz1H0ukB0AHgZCw78gwNgKTTtrcAc4BbicuPvdAKXFlQNx6YQZjhHyxo6zyPThWlJGNLakziZbYfJ4TIY8A1wAuUOFYnpUMeB2J5skj7n7EcUqQdSa2FdTH1mgG0lZN6xXXsC0JSn2E/zdTrbqCNsLjfCOwA5tpulXSgr74V4kvCzt4Y24N6mTOMjeXPaShzPkMlQSqzcdtTgLWEVarpkk4Aiwg/tmVp6FBI3PbbAIwgRJj/sT0NmE7w+s2pK1cE29fb3mZ7v+09th8pp3/FjR1zw43AKaBJ0lEASWuB74AZtqdWWo8iPAscBt62/YXt5bbXEpZIzwJzJZ0aIN164wzwoqQxhGyh1fYVpXauqLFtjyJ4Ro7g0V0Fj7wcy+WV1KMYko4Q1sDfBW4ieHgDweMn56/0VQOSjkrqjNfHCOv4w0rtX5d/LMn2DYQxakh2eKG6sT2BkMqN7eOZHDBa0o9Q4xshFyu2hxFOr8wrp19m7CrC9kxgNXBzz7kx2yuAe4FJko7HDZz1wFJJ7eXIz06qVBfrCIcmFgHYng88BtwVDV1HSF+/krSqXOGZZ1cRknJxc+gz213AQqBR0k/xkcmEvYU9th+Idc2S9pYiPzN2lSFpq+1dwGvAfZJ25bV9wwVE4yyMVxm27wTGEXa8jicpOzN2FWF7HPAJ8DxhEvZ6kvIzY1cJtkcCnwNvSfoAENBkuyGpdxSO2X8T/vrzXkzIV0nantTLMnon5s2bgQ2SFgNI2md7DcG768uQNQl4Kt7uBv7qaavL/thXO2RhvIb4DyfqqX/syaykAAAAAElFTkSuQmCC",
                         "text/latex": [
                             "$\\displaystyle \\left[ - x - 6 + \\frac{1}{x^{2}}\\right]$"
                         ],
                         "text/plain": [
                             "\u23a1         1 \u23a4\n",
                             "\u23a2-x - 6 + \u2500\u2500\u23a5\n",
                             "\u23a2          2\u23a5\n",
@@ -431,15 +431,15 @@
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle x^{2} \\left(x + y + 5\\right) + x^{2}$"
                         ],
                         "text/plain": [
                             " 2                2\n",
                             "x \u22c5(x + y + 5) + x "
                         ]
@@ -455,19 +455,175 @@
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "graphviz is not installed. Visualizing the AST is not available\n"
-                    ]
+                    "data": {
+                        "image/svg+xml": [
+                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
+                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
+                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
+                            "<!-- Generated by graphviz version 2.43.0 (0)\n",
+                            " -->\n",
+                            "<!-- Title: %3 Pages: 1 -->\n",
+                            "<svg width=\"425pt\" height=\"260pt\"\n",
+                            " viewBox=\"0.00 0.00 425.00 260.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
+                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 256)\">\n",
+                            "<title>%3</title>\n",
+                            "<polygon fill=\"white\" stroke=\"transparent\" points=\"-4,4 -4,-256 421,-256 421,4 -4,4\"/>\n",
+                            "<!-- Add(Pow(Symbol(&#39;x&#39;), Integer(2)), Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))))_() -->\n",
+                            "<g id=\"node1\" class=\"node\">\n",
+                            "<title>Add(Pow(Symbol(&#39;x&#39;), Integer(2)), Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))))_()</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"136\" cy=\"-234\" rx=\"28.7\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"136\" y=\"-230.3\" font-family=\"Times,serif\" font-size=\"14.00\">Add</text>\n",
+                            "</g>\n",
+                            "<!-- Pow(Symbol(&#39;x&#39;), Integer(2))_(0,) -->\n",
+                            "<g id=\"node2\" class=\"node\">\n",
+                            "<title>Pow(Symbol(&#39;x&#39;), Integer(2))_(0,)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"98\" cy=\"-162\" rx=\"29.8\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"98\" y=\"-158.3\" font-family=\"Times,serif\" font-size=\"14.00\">Pow</text>\n",
+                            "</g>\n",
+                            "<!-- Add(Pow(Symbol(&#39;x&#39;), Integer(2)), Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))))_()&#45;&gt;Pow(Symbol(&#39;x&#39;), Integer(2))_(0,) -->\n",
+                            "<g id=\"edge1\" class=\"edge\">\n",
+                            "<title>Add(Pow(Symbol(&#39;x&#39;), Integer(2)), Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))))_()&#45;&gt;Pow(Symbol(&#39;x&#39;), Integer(2))_(0,)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M127.19,-216.76C122.65,-208.4 117.01,-198.02 111.9,-188.61\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"114.88,-186.75 107.03,-179.63 108.72,-190.09 114.88,-186.75\"/>\n",
+                            "</g>\n",
+                            "<!-- Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,) -->\n",
+                            "<g id=\"node5\" class=\"node\">\n",
+                            "<title>Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"174\" cy=\"-162\" rx=\"28.7\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"174\" y=\"-158.3\" font-family=\"Times,serif\" font-size=\"14.00\">Mul</text>\n",
+                            "</g>\n",
+                            "<!-- Add(Pow(Symbol(&#39;x&#39;), Integer(2)), Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))))_()&#45;&gt;Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,) -->\n",
+                            "<g id=\"edge2\" class=\"edge\">\n",
+                            "<title>Add(Pow(Symbol(&#39;x&#39;), Integer(2)), Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))))_()&#45;&gt;Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M144.81,-216.76C149.42,-208.28 155.16,-197.71 160.32,-188.2\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"163.54,-189.61 165.23,-179.15 157.39,-186.27 163.54,-189.61\"/>\n",
+                            "</g>\n",
+                            "<!-- Symbol(&#39;x&#39;)_(0, 0) -->\n",
+                            "<g id=\"node3\" class=\"node\">\n",
+                            "<title>Symbol(&#39;x&#39;)_(0, 0)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"27\" cy=\"-90\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"27\" y=\"-86.3\" font-family=\"Times,serif\" font-size=\"14.00\">x</text>\n",
+                            "</g>\n",
+                            "<!-- Pow(Symbol(&#39;x&#39;), Integer(2))_(0,)&#45;&gt;Symbol(&#39;x&#39;)_(0, 0) -->\n",
+                            "<g id=\"edge3\" class=\"edge\">\n",
+                            "<title>Pow(Symbol(&#39;x&#39;), Integer(2))_(0,)&#45;&gt;Symbol(&#39;x&#39;)_(0, 0)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M82.94,-146.15C73.02,-136.37 59.87,-123.4 48.81,-112.5\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"51.13,-109.87 41.55,-105.35 46.21,-114.86 51.13,-109.87\"/>\n",
+                            "</g>\n",
+                            "<!-- Integer(2)_(0, 1) -->\n",
+                            "<g id=\"node4\" class=\"node\">\n",
+                            "<title>Integer(2)_(0, 1)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"99\" cy=\"-90\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"99\" y=\"-86.3\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n",
+                            "</g>\n",
+                            "<!-- Pow(Symbol(&#39;x&#39;), Integer(2))_(0,)&#45;&gt;Integer(2)_(0, 1) -->\n",
+                            "<g id=\"edge4\" class=\"edge\">\n",
+                            "<title>Pow(Symbol(&#39;x&#39;), Integer(2))_(0,)&#45;&gt;Integer(2)_(0, 1)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M98.25,-143.7C98.36,-135.98 98.49,-126.71 98.61,-118.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"102.11,-118.15 98.76,-108.1 95.11,-118.05 102.11,-118.15\"/>\n",
+                            "</g>\n",
+                            "<!-- Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0) -->\n",
+                            "<g id=\"node6\" class=\"node\">\n",
+                            "<title>Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"174\" cy=\"-90\" rx=\"29.8\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"174\" y=\"-86.3\" font-family=\"Times,serif\" font-size=\"14.00\">Pow</text>\n",
+                            "</g>\n",
+                            "<!-- Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,)&#45;&gt;Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0) -->\n",
+                            "<g id=\"edge5\" class=\"edge\">\n",
+                            "<title>Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,)&#45;&gt;Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M174,-143.7C174,-135.98 174,-126.71 174,-118.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"177.5,-118.1 174,-108.1 170.5,-118.1 177.5,-118.1\"/>\n",
+                            "</g>\n",
+                            "<!-- Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1) -->\n",
+                            "<g id=\"node9\" class=\"node\">\n",
+                            "<title>Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"284\" cy=\"-90\" rx=\"28.7\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"284\" y=\"-86.3\" font-family=\"Times,serif\" font-size=\"14.00\">Add</text>\n",
+                            "</g>\n",
+                            "<!-- Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,)&#45;&gt;Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1) -->\n",
+                            "<g id=\"edge6\" class=\"edge\">\n",
+                            "<title>Mul(Pow(Symbol(&#39;x&#39;), Integer(2)), Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;)))_(1,)&#45;&gt;Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M193.41,-148.65C210.74,-137.62 236.33,-121.33 255.9,-108.88\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"257.85,-111.79 264.41,-103.47 254.1,-105.88 257.85,-111.79\"/>\n",
+                            "</g>\n",
+                            "<!-- Symbol(&#39;x&#39;)_(1, 0, 0) -->\n",
+                            "<g id=\"node7\" class=\"node\">\n",
+                            "<title>Symbol(&#39;x&#39;)_(1, 0, 0)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"102\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"102\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">x</text>\n",
+                            "</g>\n",
+                            "<!-- Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0)&#45;&gt;Symbol(&#39;x&#39;)_(1, 0, 0) -->\n",
+                            "<g id=\"edge7\" class=\"edge\">\n",
+                            "<title>Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0)&#45;&gt;Symbol(&#39;x&#39;)_(1, 0, 0)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M158.73,-74.15C148.67,-64.37 135.33,-51.4 124.11,-40.5\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"126.36,-37.81 116.75,-33.35 121.49,-42.83 126.36,-37.81\"/>\n",
+                            "</g>\n",
+                            "<!-- Integer(2)_(1, 0, 1) -->\n",
+                            "<g id=\"node8\" class=\"node\">\n",
+                            "<title>Integer(2)_(1, 0, 1)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"174\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"174\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n",
+                            "</g>\n",
+                            "<!-- Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0)&#45;&gt;Integer(2)_(1, 0, 1) -->\n",
+                            "<g id=\"edge8\" class=\"edge\">\n",
+                            "<title>Pow(Symbol(&#39;x&#39;), Integer(2))_(1, 0)&#45;&gt;Integer(2)_(1, 0, 1)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M174,-71.7C174,-63.98 174,-54.71 174,-46.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"177.5,-46.1 174,-36.1 170.5,-46.1 177.5,-46.1\"/>\n",
+                            "</g>\n",
+                            "<!-- Integer(5)_(1, 1, 0) -->\n",
+                            "<g id=\"node10\" class=\"node\">\n",
+                            "<title>Integer(5)_(1, 1, 0)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"246\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"246\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">5</text>\n",
+                            "</g>\n",
+                            "<!-- Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)&#45;&gt;Integer(5)_(1, 1, 0) -->\n",
+                            "<g id=\"edge9\" class=\"edge\">\n",
+                            "<title>Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)&#45;&gt;Integer(5)_(1, 1, 0)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M275.19,-72.76C270.58,-64.28 264.84,-53.71 259.68,-44.2\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"262.61,-42.27 254.77,-35.15 256.46,-45.61 262.61,-42.27\"/>\n",
+                            "</g>\n",
+                            "<!-- Symbol(&#39;x&#39;)_(1, 1, 1) -->\n",
+                            "<g id=\"node11\" class=\"node\">\n",
+                            "<title>Symbol(&#39;x&#39;)_(1, 1, 1)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"318\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"318\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">x</text>\n",
+                            "</g>\n",
+                            "<!-- Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)&#45;&gt;Symbol(&#39;x&#39;)_(1, 1, 1) -->\n",
+                            "<g id=\"edge10\" class=\"edge\">\n",
+                            "<title>Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)&#45;&gt;Symbol(&#39;x&#39;)_(1, 1, 1)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M292.06,-72.41C296.08,-64.13 301.04,-53.92 305.54,-44.66\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"308.78,-45.99 310,-35.47 302.48,-42.94 308.78,-45.99\"/>\n",
+                            "</g>\n",
+                            "<!-- Symbol(&#39;y&#39;)_(1, 1, 2) -->\n",
+                            "<g id=\"node12\" class=\"node\">\n",
+                            "<title>Symbol(&#39;y&#39;)_(1, 1, 2)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"390\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"390\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">y</text>\n",
+                            "</g>\n",
+                            "<!-- Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)&#45;&gt;Symbol(&#39;y&#39;)_(1, 1, 2) -->\n",
+                            "<g id=\"edge11\" class=\"edge\">\n",
+                            "<title>Add(Integer(5), Symbol(&#39;x&#39;), Symbol(&#39;y&#39;))_(1, 1)&#45;&gt;Symbol(&#39;y&#39;)_(1, 1, 2)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M302.95,-76.49C319.71,-65.42 344.35,-49.15 363.14,-36.74\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"365.15,-39.6 371.57,-31.17 361.29,-33.76 365.15,-39.6\"/>\n",
+                            "</g>\n",
+                            "</g>\n",
+                            "</svg>\n"
+                        ],
+                        "text/plain": [
+                            "<graphviz.sources.Source at 0x7f41d153f050>"
+                        ]
+                    },
+                    "execution_count": 19,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ps.to_dot(expr, graph_style={'size': \"9.5,12.5\"} )"
             ]
         },
         {
@@ -501,15 +657,15 @@
         {
             "cell_type": "code",
             "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left( x^{2}, \\  x^{2} \\left(x + y + 5\\right)\\right)$"
                         ],
                         "text/plain": [
                             "\u239b 2   2            \u239e\n",
                             "\u239dx , x \u22c5(x + y + 5)\u23a0"
                         ]
@@ -558,15 +714,15 @@
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAC0AAAAaCAYAAAAjZdWPAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAABJ0AAASdAHeZh94AAADAklEQVR4nM3YXYgWZRQH8N+bFW1fYEikRGwQUUHfdiPlReRFGhFEFNGFEBGJhQRChXA4UkEIQlQWWlBUF4HdeNG6EiRUYoFtHxSCShSxIS1BeFGItl3MvMvD7OzurO6+9L955vk/5zz858x5zpyZ3uTkpC7IzNXYjNuxHA9FxO5OzguMc+ZhexG+w8ZF0tIZ57aRmXkpXsT9WIHz8FxEbKnXByawDa2i8SHuwyf4AKewZ1Ci5sI00Zl5nUrwaESsG7ykudGW03fX48eDFDIfTEU6Mx9EWQ12ZubO+vr6iDg8UGWzoEyP35HYgKV4qeYncWTAumZFr6zTmbkEJ3A0Im4qDTPzYlxTT8dUNftT/BkRvw5GboXmQbwBQ/imxXYlPivm2+rxPaxfcGWzoCn6tnqcJjoi9qO32IK6oFk9+qLHBi1kPmiL9CS+bRpm5lIcxqqIOLb40sjM3TgQEdtLvix5PdyMIxFxomWPF7C3L3ghGqjM3FDvsRw/YlNEfF6YbMX+zHwnIv7qk2V6XItLtKRGZl6IJ/B2QZ9VA5WZD+NVvIxb8SVGMvOqvk1EfI+f8VjpW6bHjIcQ6/Avvig2HMFILeBMdD+LdyNiVz1/JjPvxVN4vrDbg0fxRp8oIz2b6DtxKCK6Nd9zIDPPV6XVvsbSPqxqcF/hjswc6hNTkY6Izar8asMwxs9WbIFlWILjDf447mlw46rWeAWO0f0j4AL8c+YaZ0TzyfVauL/rcSrSXUVPqPqRhcIETuOKBn+56dG/rB7/6BNdRY+pXvELgog4iUNY01hagwMN7kaMR8TUzcz05dLEKF7JzGURMcG0BgqGM/MW3Ruo7Xg/M79WlbsnVXn7VsNuNfaWRKdIR8QPqlP8SEGvVD2Bfl3fVl9v7Rtk5vrMnMzM4ZY9P8ImbFG9ge/C2oj4pfAfwgPYVfp2jTRVr/1aZr4ZEac7NlBX4yf81rYYETuwYxb/x3EwIg6WZOdfCBExitdxZVcfrMXGiDg1D58SJ/F0k+x1/Vnzf8J/lSTmjUVQzcoAAAAASUVORK5CYII=\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAC0AAAAaCAYAAAAjZdWPAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAABJ0AAASdAHeZh94AAAC/ElEQVR4nM3YT6hVVRQG8N/Vil5YYAaShBVEhET/aSDZIBLCIogGFTQoalCGJJIDJVgsqahBgYNEtOBBNYhq4uCVjooo7IG9oL9UBkVZkgXhoCjlNjjn3jbnHd87z/fepQ8O+55vr7Xvxzprr73O6fX7fV2QmTfjCVyPVXgwIsY7OS8wlszBdhk+w+P4c3HkdMMZbWRmnoencKcqqmdiW0Rsr+fHRyWwDa2i8RruwARexQnsG5Wo2TBNdGZeoRK8PyJuH72k2dGW07fU41ujFDIXDCOdmXfjzWJuT2buqX+viYgvR6psBpTp8TMSG7EcT9d8H1+PWNeM6JV1OjOX4ji+jYirSsPMXIbL6tsP8axqc/4eET+MRm6FZk6vwRg+brG9AVP1NaZ6KlPYsZgC29CsHtfV4zTREfEueostqAuakR6Inhq1kLmgLdJ9fNI0zMzl+AprI+Lw4ksjM9/AwYh4vuTLktfD1fgmIo63rLEdEwPBC9FAZeZGbMWF+BybI+L9wmQH3svMlyLijwFZpsflOFdLamTmOXgYLxf0vBqozLwHO/EMrlVVpLczc/XAJiI+xXe4v/Qt0+OUmxAbVGnzQbHghKo3Od0GagvGI2Jvfb8pM2/Do9hW2O3DfXhxQJSRnkn0OhyKiG7N9yzIzLNUaXWgMXUAaxvcJG7MzLEBMYx0RGxV5VcbLsaReav9DxdgKY42+KO4tcEdUbXGq3CY7i8BY/jr9DXOC4P9Mox0V9HHVP3IQuEYTmJlg1+JXxrc+fX464DoKnpKdcQvCCLibxzC+sbUelUVKXElfoqIYSqd6s2lif14LjNXRMRvTGuglmB1Zl6jewP1Al7JzElVVXpElbe7G3br6v8folOk63o5iXsLetYGKjMfyMx+Zl7Ssubr2IwnVSfwTdgQEd8X/mfjLuwtfbtGWi1qZ2bujoiTHRuoS/EFfmybjIhd2DWD/0P4KCIOlmTnTwgR8Y6qwF/U1Ud1KD0WESfm4FPiH2xqkr2uH2v+T/gXmdDo73n+u0IAAAAASUVORK5CYII=",
                         "text/latex": [
                             "$\\displaystyle {f}_{(1,0)}^{1}$"
                         ],
                         "text/plain": [
                             "f_E__1"
                         ]
                     },
@@ -628,24 +784,21 @@
         {
             "cell_type": "code",
             "execution_count": 26,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAzUAAAAaCAYAAACO/nKSAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAABJ0AAASdAHeZh94AAAN6UlEQVR4nO2dfdBVRR3HP/gSmKCCjhqViEOaqKOCiWPoPCiiYzWSOamZDWpqQibjaEWZv35oviXKMwbpWAlhzpillZOZA6HjO8ZLavlOYPmWCqKMCopPf+w5cNh7zr33vJ977n5mmAv7cs6e/X532b27Z2+/vr4+mqGq/UVkXdNEJaOq04Djgb2AdcAjwDQRebLUgjlyw2neXTi9Ha1wHnHExXnGUQTOZ61R1Y+JyPoWaVrW4xYtLnAmMCJ9cXOnB5gNHAocAXwIzFfVIWUWypErPTjNu4kenN6O5vTgPOKIRw/OM4786cH5rBX7q+rRLdL00KIe+0Wt1KjqOGCCiEwLiTsfmAGcIiK3JCp+jqjqQGANMFFE7iy7PJ1O1fUGp3nWVF1zp3e5VN0f4DxSRaruG+eZzqfqHgPnsyhUdQYwR0SeaDN9Qz2GrtSo6rbAFcD0iGsd5H3+PVaJi2MQ5tlWl12QmlB1vcFpnjVV19zpXS5V9wc4j1SRqvvGeabzqbrHwPksiunALFVtuossQEM9RmX8LrBQRN6LiP8+sDfwXJs3LppeYBnwcMnlqAtV1xuc5llTdc2d3uVSdX+A80gVqbpvnGc6n6p7DJzPQhGRNcBTwKltZmmox4btZ6o6CHgRGCMiz2ZS0gJR1WuAk4CxIrK87PI48sdp3l04vdOhqpOAm4BxInJvuaXJB+cRR1ycZxxF4HzWHFU9GPgdMKLZwQFR9bhVSNoTgFVRExrvXZu/AVeLyIVW2AzgFuBi4HBgSy/8HBF5VVVHAhcB44H+wP3AZBF5MeQ+A4CpwDeAPYDXgBuAK4G3gBUisp+V51rvIceVaRZVPRKYD1wiIhcHwsdgTmsAGC4iKwJxNwNfA/YWkWcKLG5TwvS2wjPRPIneXr7SNa+T3uDaeB7UySNV9oeXryM9YlMnz0C1fVMXzyShTj5z45XsKdofIrLIewXmi8DtEWWKrMew7WcnAEua3HOU97kkJGxP4AFgA/BLzIrPROBXqvolYBEwEJgLPAt8Afh1SIG3BRYClwPvYpaYFmKMOMe7xhIrTy9wMnCEiDzdpPxF4O/vG2SFfy/w942nNajqUOCrwJ1V6iA8wvQOhqfWPIneXr6qaF4nvcG18Tyok0cq6Q8vXyd7xKZOnoGK+qZmnklCnXzmxivZU4Y/lmLmIg20qsetrMRbAGMxs80omnVMBwOHiMjj3vWmY0wzATgQOEpEHvbiPgY8DxyuqgNE5P3A9W4ADsGY5FIR6fPyzMPMGDe7v6rOwuzBmwisVtVdvai1IrK2ybPkRYMJVHVP4DjgD5hyDg6knwJsDfy0mOLFolUnkYXmsfT24qqkeZ30BtfG86BOHqmcP7y4TveITZ08AxX0TQ09k4Q6+cyNV7KnDH8sAU6xA9upR3ulZg9gO2BFk5uNAtZiZrHBMIBJvlkAROQd71pbAhf6ZvHi1gPPAP2AbQOFPsR7mD+KyCW+Ybw8CzAG9B/aZzKmwhcArwT+XNDkOfIkbGZ7AfAOcJX37yGwcRnzLOBREXmgsBK2T5jefjik1Dyh3lAtzeukN7g2ngd18kgV/QGd7xGbOnkGqumbunkmCXXymRuvZE8Z/lgJDFXVHa3wlvVov1Mz3PtcE3YXb9ltT+ChwOzUD1suIneHZBsGrAJujYh7R0TeDIRN8T5/ElYG4E3g05gTDwAQkX4RactiDfARnglUdRfM3ste4D9eGn+57lRgJ+CctDdV1RWYOm2X34jI15tcr0FvKzwLzWPrDZXTvBS9vXutIGfNXRvPhCr2CQtV1Q6bKyKTmlyvkv6AWnjExvUrrl8pglr4zI1XcqMMf/hzkOGYOgXaq0d7UuMvIb0dkX5/zOrOkpCw+XZiVd3du+btIvKBFTcQGIHZ3xhkAuYhos4Y/wTwnDfDriQi0qeqa9g0sz0PM9vvxcxuYVNdnwe8QOCFKFWdBhwP7AWsw7yMNU1Enmxx6xeA91ukCfJyi/gwvYPhWWje9XoDqOrhmG8bRgNDgdNEZE4bty9Cc9fGU5JBn5DUHzOBHaywAzBbB+bSuCq/rMX1nD8KwvUrzjdFUGLfBNn6zI1XcqCk8aw/B9khbnntSU1/7/PdiPT+Et7SkLDFIelHN4k7EFMxwf2tA4CdgWXBmXYg/rPArsC9Vvhg4GngUBF5IaLsmaOqtwGPiMiMkOjVwCCvYZwD3CIiL3v5NgBDVHUCsA/wbRH5KJC3B5gNPIapo+nAfFUdKSKrosojIkdm8FhBwvQOhqfSPKneXlzhmueoN5iXC5/EvJTY8AJsFAVp3rVtPC45eiSpP2aGlHESZlIzR+If6VxJf3hxHeERG9evuH6lCKrWN0HmPnPjlRRUbDzrz0EGxH0Oe1Lj/9jmwIj0zV70C5u5jm4Sd2DItTZ4fwY3JgfMj4LaeQB+ANwVNEvKbw/8a0wGLsTMvv8JTBWR+wNJpgP3qeovxPxoUJDV3nOcBWzP5i9NvY1ZrpuKmfXfFMwoIkdb5TgVsxz3eeDOOM+QklYv3aXVPKneYGmeVu828+eiN4CI3AXc5ZWl7XLnQMe08bh0skecPzZSWJ+QBa5f2UhVfVN6v5IFrm8COmi8EpcuHM/6c5D3IuIjsQ8K8GdN20WkH4VZKvyXFbYeM1O3aTYLbjCgt/z3DDBMzdnYG1HVKcBpdh5V/TjwTczxfEH8bw/OI0HFqOqJmOW1yzDmfgj4i6ruFijvE8ByIGyPp2+CqRgzB+tsDTAGOAaYLSJRK2M+gzBarW6RLmvC9PbDU2ueRG8vLkzzVHq3k79Avcukk9p4XJxH0lM5f3hxefQJWeA8Y6icbyrUr2SB81lnjVfi0m3jWX8O8maTNKHYKzXLvc/t7YSq2h8YiVl6+9AKe1zCf/lzNLDSepnPZxRGnKes8MuBecCfVfVW4FXMMdOfwSzf7cXmpjkW6AMeDF4kg28Pzsdsz7jR+/e5qnoMZultWiDdnzBnZs+y8vsmGIx5eSrIW5h97e8DP2ujLL2Yve4Pt0iXGWF6W+FZaR5XbwjRPK3eMfIXoXcpdFobj4vzSDoq7A/IoU/Igm73DFTaN5XoV7Kg233WaeOVuHTheNafgyxvkiYUe6VmJWa1ZkRI2n0xZ08vCQlrmOWq6jBgx4i4/sDeGKNtCMaJyM3Ad4CXMJV7MqYCPsem/YzBGd5hwOKwPY5JUXM++WjgHivqHuBQK2wRcLCqbmOF+2V8TETus+L8pb15IvK/FmW5BtNovmLXVc6E6R0Mz0TzBHpDDprHIFe9S6Zr2njO1NUjVfUHdJ5HbOrqGaiubzrdM0moq8/ceCWCDh3PjgCeF5GoQ8si2WylRswpB/exadktGLcY85JP07BA3MomceswRgtFRK4DrguGefvwhmBmykGG0frklbjshDm3/DUr/DVgvBX2MuZZhmJOfQBARM4Gzg67uIj0tFMIVb0WOAkYJyKxZ6xpiNI2D81j6g35aN4uueldNl3WxvOk0h7x9mLPSZCvqv6AzvOITaU9k4YK+6bTPZOEWvrMjVea0onj2VHAwnaua2NvPwP4LXB1koulRVW3BHa0Z3uqOh74OeZM7OutbNvQKFaR+Psb7ZltKlS1FzgRY4Cns7x2VUioN5SreS56dwtZtnFVvRT4YYtbjpP4J3ylxXkkIVXtEwrwmvNMCurQrxR0X+ezhGTZN3Xb/11xxrOqugXmGO4fJ7lX2KTmDuBKVR3tzXKLZCTwmKr+FTNL3BqzV28s8DpwnIistfK8QfRpFEl5A3PKxS5W+C6YPZRB/B8dej2rm6vqLMy+xYnAalXd1YtaG/L8nUwSvSEfzdslc70BdNOZ+GC2he6mqgcAq0TkxciMnUeWbXwmcHOL+5VRd3n0Cc4f5fYJM8nXa65fSUcd+pUi7uv6puRk2TfNpDiPddp49gjgFbJaqRGRdar6I+B0wk+EyJP1mJehxgBHY37F9N/AVcA1IhL2TdxSYFKWhRCR9aq6GDgKuC0QdRTweyv5vsBLEWVLymTvc4EVriScvVaUJHpDDprHIA+9AQ5i80as3p+5lPeseZBZGxeRNzAddtXIwyPOHyX2CQV4zfUr6ej4fqWg+7q+KTmZ9U1FeqwDx7OnA5dK429utUW/vr7Gd5e85Z8FmJd5In/ssQqo6n6YF7V2lsAJFta3Bw8BV2BOdmjr2wPvCLx5GEEeBL4FnAHs4+3F9NPNATaIyBlZPI+jNWGaZ6B3W/md3sUT1cYTXMd5pKbk0SdkVC7nmYpSlX4lC5zPqksWPuuW8ayqfhLzA67jJeHBCvbpZwB4M6SzgYuSF68YxJytvQjzAlKQgzAz5KWY/YHq/X26n0BVJ6lqn6ruHnLdWzFncl+EMeRY4FjLAAOALwM32vkd+RGheSq928zv9C6BJm08Lk01buGPlvm9aziPlEBOfUIWOM9UlKL6FXA+62Yy8lm3jGcvA85MOqGB8HdqABCRZ1X1DlU9QESWJb1BQSjQq6rXi3dMnPeCVejJFgGGY36o6b9hkSIyG5jdJP8ZwKMi8kjsEjvSspnmafVuM7/Tuzwa2nhc2tC4VX/QKj84j5RJpn1CFjjPVJ4i+hVwPut2UvmsG8azqnoYcFMbJ6M1JXSlxkdE7gf+keYGRSAid2N+LOhTMbMeC0yRwI81xeQD4NyEeR0pSKi507tDSdHG45DWH+A8Uhol9QlZ4DxTEgX1K+B81tV0yP9fZfvjgSxOewt9p8bhcDgcDofD4XA4OoX/A1EFgqlLrdzJAAAAAElFTkSuQmCC",
                         "text/latex": [
                             "$\\displaystyle \\left({img}_{(1,0)}^{2} w_{2} - {img}_{(1,1)}^{2} w_{1} - {img}_{(-1,1)}^{2} w_{1} + {img}_{(1,-1)}^{2} w_{1} - {img}_{(-1,-1)}^{2} w_{1} - {img}_{(-1,0)}^{2} w_{2}\\right)^{2}$"
                         ],
                         "text/plain": [
-                            "                                                                              \n",
-                            "(img_E__2\u22c5w\u2082 - img_NE__2\u22c5w\u2081 - img_NW__2\u22c5w\u2081 + img_SE__2\u22c5w\u2081 - img_SW__2\u22c5w\u2081 - img\n",
-                            "\n",
-                            "         2\n",
-                            "_W__2\u22c5w\u2082) "
+                            "                                                                                       2\n",
+                            "(img_E__2\u22c5w\u2082 - img_NE__2\u22c5w\u2081 - img_NW__2\u22c5w\u2081 + img_SE__2\u22c5w\u2081 - img_SW__2\u22c5w\u2081 - img_W__2\u22c5w\u2082) "
                         ]
                     },
                     "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -667,24 +820,21 @@
         {
             "cell_type": "code",
             "execution_count": 27,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left({img}_{(1,0)}^{2} w_{2} - 0.5 {img}_{(1,1)}^{2} - 0.5 {img}_{(-1,1)}^{2} + 0.5 {img}_{(1,-1)}^{2} - 0.5 {img}_{(-1,-1)}^{2} - {img}_{(-1,0)}^{2} w_{2}\\right)^{2}$"
                         ],
                         "text/plain": [
-                            "                                                                              \n",
-                            "(img_E__2\u22c5w\u2082 - 0.5\u22c5img_NE__2 - 0.5\u22c5img_NW__2 + 0.5\u22c5img_SE__2 - 0.5\u22c5img_SW__2 -\n",
-                            "\n",
-                            "             2\n",
-                            " img_W__2\u22c5w\u2082) "
+                            "                                                                                           2\n",
+                            "(img_E__2\u22c5w\u2082 - 0.5\u22c5img_NE__2 - 0.5\u22c5img_NW__2 + 0.5\u22c5img_SE__2 - 0.5\u22c5img_SW__2 - img_W__2\u22c5w\u2082) "
                         ]
                     },
                     "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -703,24 +853,21 @@
         {
             "cell_type": "code",
             "execution_count": 28,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle {dst}_{(0,0)} \\leftarrow \\left({img}_{(1,0)}^{2} w_{2} - 0.5 {img}_{(1,1)}^{2} - 0.5 {img}_{(-1,1)}^{2} + 0.5 {img}_{(1,-1)}^{2} - 0.5 {img}_{(-1,-1)}^{2} - {img}_{(-1,0)}^{2} w_{2}\\right)^{2}$"
                         ],
                         "text/plain": [
-                            "                                                                              \n",
-                            "dst_C := (img_E__2\u22c5w\u2082 - 0.5\u22c5img_NE__2 - 0.5\u22c5img_NW__2 + 0.5\u22c5img_SE__2 - 0.5\u22c5im\n",
-                            "\n",
-                            "                      2\n",
-                            "g_SW__2 - img_W__2\u22c5w\u2082) "
+                            "                                                                                                    2\n",
+                            "dst_C := (img_E__2\u22c5w\u2082 - 0.5\u22c5img_NE__2 - 0.5\u22c5img_NW__2 + 0.5\u22c5img_SE__2 - 0.5\u22c5img_SW__2 - img_W__2\u22c5w\u2082) "
                         ]
                     },
                     "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -759,15 +906,15 @@
         {
             "cell_type": "code",
             "execution_count": 30,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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t9sNp9MpexEEQRAEQQhMW9DwPI+nnnoKGzZswPLlywEA3d3dMBgMsFqtsrwFBQXo7u4W80jFjHBeOKfGrl27YLFYxFdpael0m00QBEEQxCxEN92CO3bswPnz53H48OFYtkeVp59+Gjt37hSPHQ4HysrKyFJDEARBECmEMG7PINolLNMSNE8++STef/99HDx4ECUlJWK6zWaDx+OB3W6XWWl6enpgs9nEPMePH5fVJ8yCEvIoMRqNMBqN4rHQIWSpIQiCIIjUY2BgABaLJaZ1RiVoGGP43ve+h7fffhv79+9HZWWl7HxNTQ30ej327duHbdu2AQAuX76MtrY21NXVAQDq6urwd3/3d+jt7UV+fj4AYO/evTCbzVi2bFlE7SgqKsLFixexbNkytLe3U2DwDHA6nSgtLaV+jAHUl7GB+jF2UF/GBurH2CF4WITY21gSlaDZsWMHXnvtNfzud79DVlaWGPNisVhgMplgsVjwxBNPYOfOncjOzobZbMb3vvc91NXVYf369QCAe+65B8uWLcPXv/51/MM//AO6u7vxV3/1V9ixY4fMCjMZGo0GxcXFAACz2UxfsBhA/Rg7qC9jA/Vj7KC+jA3Uj7FDo4n9ur5RCZrnn38eAHDnnXfK0l966SV84xvfAAD80z/9EzQaDbZt2wa3243NmzfjX/7lX8S8Wq0W77//Pr773e+irq4OGRkZePzxx/GTn/xkZndCEARBEMScJWqX01SkpaXhueeew3PPPRc2T3l5OT744INoLk0QBEEQBBGWlN3LyWg04plnnonYTUWoQ/0YO6gvYwP1Y+ygvowN1I+xI559OaOVggmCIAiCIG4GUtZCQxAEQRAEIUCChiAIgiCIlIcEDUEQBEEQKQ8JGoIgCIIgUp6UFDTPPfccKioqkJaWhtra2pCtFOY6Bw8exAMPPICioiJwHId33nlHdp4xhh//+McoLCyEyWRCfX09rly5IsszODiI7du3w2w2w2q14oknnoDL5UrgXSSfXbt24dZbb0VWVhby8/Px0EMP4fLly7I84+Pj2LFjB3JycpCZmYlt27aJW3kItLW14b777kN6ejry8/PxZ3/2Z/D5fIm8laTz/PPPY+XKleLCZHV1ddi9e7d4nvpxevz93/89OI7DU089JaZRX0bG3/zN34DjONmrqqpKPE/9GDkdHR342te+hpycHJhM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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -790,15 +937,15 @@
         {
             "cell_type": "code",
             "execution_count": 31,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -821,19 +968,163 @@
         },
         {
             "cell_type": "code",
             "execution_count": 32,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "graphviz is not installed. Visualizing the AST is not available\n"
-                    ]
+                    "data": {
+                        "image/svg+xml": [
+                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
+                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
+                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
+                            "<!-- Generated by graphviz version 2.43.0 (0)\n",
+                            " -->\n",
+                            "<!-- Title: %3 Pages: 1 -->\n",
+                            "<svg width=\"684pt\" height=\"391pt\"\n",
+                            " viewBox=\"0.00 0.00 684.00 390.75\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
+                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1.22 1.22) rotate(0) translate(4 472)\">\n",
+                            "<title>%3</title>\n",
+                            "<polygon fill=\"white\" stroke=\"transparent\" points=\"-4,4 -4,-472 829.23,-472 829.23,4 -4,4\"/>\n",
+                            "<!-- 139920670537616 -->\n",
+                            "<g id=\"node1\" class=\"node\">\n",
+                            "<title>139920670537616</title>\n",
+                            "<ellipse fill=\"#a056db\" stroke=\"black\" cx=\"263.84\" cy=\"-450\" rx=\"134.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"263.84\" y=\"-446.3\" font-family=\"Times,serif\" font-size=\"14.00\">Func: kernel (dst,img,w_2)</text>\n",
+                            "</g>\n",
+                            "<!-- 139920670664720 -->\n",
+                            "<g id=\"node11\" class=\"node\">\n",
+                            "<title>139920670664720</title>\n",
+                            "<ellipse fill=\"#dbc256\" stroke=\"black\" cx=\"263.84\" cy=\"-378\" rx=\"36.29\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"263.84\" y=\"-374.3\" font-family=\"Times,serif\" font-size=\"14.00\">Block</text>\n",
+                            "</g>\n",
+                            "<!-- 139920670537616&#45;&gt;139920670664720 -->\n",
+                            "<g id=\"edge10\" class=\"edge\">\n",
+                            "<title>139920670537616&#45;&gt;139920670664720</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M263.84,-431.7C263.84,-423.98 263.84,-414.71 263.84,-406.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"267.34,-406.1 263.84,-396.1 260.34,-406.1 267.34,-406.1\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920666169168 -->\n",
+                            "<g id=\"node2\" class=\"node\">\n",
+                            "<title>139920666169168</title>\n",
+                            "<ellipse fill=\"#56db7f\" stroke=\"black\" cx=\"175.84\" cy=\"-306\" rx=\"73.39\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"175.84\" y=\"-302.3\" font-family=\"Times,serif\" font-size=\"14.00\">_data_img_22</text>\n",
+                            "</g>\n",
+                            "<!-- 139920670656400 -->\n",
+                            "<g id=\"node3\" class=\"node\">\n",
+                            "<title>139920670656400</title>\n",
+                            "<ellipse fill=\"#3498db\" stroke=\"black\" cx=\"352.84\" cy=\"-306\" rx=\"85.59\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"352.84\" y=\"-302.3\" font-family=\"Times,serif\" font-size=\"14.00\">Loop over dim 0</text>\n",
+                            "</g>\n",
+                            "<!-- 139920657663504 -->\n",
+                            "<g id=\"node10\" class=\"node\">\n",
+                            "<title>139920657663504</title>\n",
+                            "<ellipse fill=\"#dbc256\" stroke=\"black\" cx=\"352.84\" cy=\"-234\" rx=\"36.29\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"352.84\" y=\"-230.3\" font-family=\"Times,serif\" font-size=\"14.00\">Block</text>\n",
+                            "</g>\n",
+                            "<!-- 139920670656400&#45;&gt;139920657663504 -->\n",
+                            "<g id=\"edge7\" class=\"edge\">\n",
+                            "<title>139920670656400&#45;&gt;139920657663504</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M352.84,-287.7C352.84,-279.98 352.84,-270.71 352.84,-262.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"356.34,-262.1 352.84,-252.1 349.34,-262.1 356.34,-262.1\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920670665808 -->\n",
+                            "<g id=\"node4\" class=\"node\">\n",
+                            "<title>139920670665808</title>\n",
+                            "<ellipse fill=\"#56db7f\" stroke=\"black\" cx=\"70.84\" cy=\"-162\" rx=\"70.69\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"70.84\" y=\"-158.3\" font-family=\"Times,serif\" font-size=\"14.00\">_data_dst_00</text>\n",
+                            "</g>\n",
+                            "<!-- 139920670698640 -->\n",
+                            "<g id=\"node5\" class=\"node\">\n",
+                            "<title>139920670698640</title>\n",
+                            "<ellipse fill=\"#56db7f\" stroke=\"black\" cx=\"249.84\" cy=\"-162\" rx=\"89.88\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"249.84\" y=\"-158.3\" font-family=\"Times,serif\" font-size=\"14.00\">_data_img_22_01</text>\n",
+                            "</g>\n",
+                            "<!-- 139920661915920 -->\n",
+                            "<g id=\"node6\" class=\"node\">\n",
+                            "<title>139920661915920</title>\n",
+                            "<ellipse fill=\"#56db7f\" stroke=\"black\" cx=\"455.84\" cy=\"-162\" rx=\"98.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"455.84\" y=\"-158.3\" font-family=\"Times,serif\" font-size=\"14.00\">_data_img_22_0m1</text>\n",
+                            "</g>\n",
+                            "<!-- 139920657676048 -->\n",
+                            "<g id=\"node7\" class=\"node\">\n",
+                            "<title>139920657676048</title>\n",
+                            "<ellipse fill=\"#3498db\" stroke=\"black\" cx=\"658.84\" cy=\"-162\" rx=\"85.59\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"658.84\" y=\"-158.3\" font-family=\"Times,serif\" font-size=\"14.00\">Loop over dim 1</text>\n",
+                            "</g>\n",
+                            "<!-- 139920657567760 -->\n",
+                            "<g id=\"node9\" class=\"node\">\n",
+                            "<title>139920657567760</title>\n",
+                            "<ellipse fill=\"#dbc256\" stroke=\"black\" cx=\"658.84\" cy=\"-90\" rx=\"36.29\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"658.84\" y=\"-86.3\" font-family=\"Times,serif\" font-size=\"14.00\">Block</text>\n",
+                            "</g>\n",
+                            "<!-- 139920657676048&#45;&gt;139920657567760 -->\n",
+                            "<g id=\"edge2\" class=\"edge\">\n",
+                            "<title>139920657676048&#45;&gt;139920657567760</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M658.84,-143.7C658.84,-135.98 658.84,-126.71 658.84,-118.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"662.34,-118.1 658.84,-108.1 655.34,-118.1 662.34,-118.1\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920662243472 -->\n",
+                            "<g id=\"node8\" class=\"node\">\n",
+                            "<title>139920662243472</title>\n",
+                            "<ellipse fill=\"#56db7f\" stroke=\"black\" cx=\"658.84\" cy=\"-18\" rx=\"166.27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"658.84\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">_data_dst_00[_stride_dst_1*ctr_1]</text>\n",
+                            "</g>\n",
+                            "<!-- 139920657567760&#45;&gt;139920662243472 -->\n",
+                            "<g id=\"edge1\" class=\"edge\">\n",
+                            "<title>139920657567760&#45;&gt;139920662243472</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M658.84,-71.7C658.84,-63.98 658.84,-54.71 658.84,-46.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"662.34,-46.1 658.84,-36.1 655.34,-46.1 662.34,-46.1\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920657663504&#45;&gt;139920670665808 -->\n",
+                            "<g id=\"edge3\" class=\"edge\">\n",
+                            "<title>139920657663504&#45;&gt;139920670665808</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M321.04,-225.11C274.68,-213.6 187.72,-192.01 129.54,-177.57\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"130.29,-174.15 119.74,-175.14 128.61,-180.94 130.29,-174.15\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920657663504&#45;&gt;139920670698640 -->\n",
+                            "<g id=\"edge4\" class=\"edge\">\n",
+                            "<title>139920657663504&#45;&gt;139920670698640</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M332,-218.83C317.82,-209.19 298.75,-196.24 282.56,-185.23\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"284.15,-182.08 273.91,-179.35 280.21,-187.87 284.15,-182.08\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920657663504&#45;&gt;139920661915920 -->\n",
+                            "<g id=\"edge5\" class=\"edge\">\n",
+                            "<title>139920657663504&#45;&gt;139920661915920</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M373.69,-218.83C387.77,-209.26 406.67,-196.42 422.79,-185.46\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"425.11,-188.12 431.41,-179.61 421.17,-182.33 425.11,-188.12\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920657663504&#45;&gt;139920657676048 -->\n",
+                            "<g id=\"edge6\" class=\"edge\">\n",
+                            "<title>139920657663504&#45;&gt;139920657676048</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M385.3,-225.58C434.58,-214.3 529.28,-192.64 593.27,-178\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"594.3,-181.35 603.27,-175.71 592.74,-174.53 594.3,-181.35\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920670664720&#45;&gt;139920666169168 -->\n",
+                            "<g id=\"edge8\" class=\"edge\">\n",
+                            "<title>139920670664720&#45;&gt;139920666169168</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M245.18,-362.15C233.32,-352.72 217.72,-340.31 204.33,-329.66\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"206.33,-326.78 196.32,-323.29 201.97,-332.25 206.33,-326.78\"/>\n",
+                            "</g>\n",
+                            "<!-- 139920670664720&#45;&gt;139920670656400 -->\n",
+                            "<g id=\"edge9\" class=\"edge\">\n",
+                            "<title>139920670664720&#45;&gt;139920670656400</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M282.72,-362.15C294.63,-352.78 310.27,-340.49 323.75,-329.88\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"326.12,-332.47 331.82,-323.54 321.79,-326.97 326.12,-332.47\"/>\n",
+                            "</g>\n",
+                            "</g>\n",
+                            "</svg>\n"
+                        ],
+                        "text/plain": [
+                            "<graphviz.sources.Source at 0x7f4230138790>"
+                        ]
+                    },
+                    "execution_count": 32,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ps.to_dot(ast, graph_style={'size': \"9.5,12.5\"})"
             ]
         },
         {
@@ -932,28 +1223,28 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_2</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2</span><span class=\"o\">*</span><span class=\"n\">_stride_img_2</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_00</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_01</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_0m1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"n\">_data_dst_00</span><span class=\"p\">[</span><span class=\"n\">_stride_dst_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">])</span><span class=\"o\">*</span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]);</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"p\">}</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"p\">}</span><span class=\"w\"></span>\n",
-                            "<span class=\"p\">}</span><span class=\"w\"></span>\n",
+                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_2</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"p\">)</span>\n",
+                            "<span class=\"p\">{</span>\n",
+                            "<span class=\"w\">   </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2</span><span class=\"o\">*</span><span class=\"n\">_stride_img_2</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">   </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span>\n",
+                            "<span class=\"w\">   </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_00</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_01</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_0m1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span>\n",
+                            "<span class=\"w\">      </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">         </span><span class=\"n\">_data_dst_00</span><span class=\"p\">[</span><span class=\"n\">_stride_dst_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">])</span><span class=\"o\">*</span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]);</span>\n",
+                            "<span class=\"w\">      </span><span class=\"p\">}</span>\n",
+                            "<span class=\"w\">   </span><span class=\"p\">}</span>\n",
+                            "<span class=\"p\">}</span>\n",
                             "</pre></div>\n"
                         ],
                         "text/plain": [
                             "FUNC_PREFIX void kernel(double * RESTRICT  _data_dst, double * RESTRICT const _data_img, int64_t const _size_dst_0, int64_t const _size_dst_1, int64_t const _stride_dst_0, int64_t const _stride_dst_1, int64_t const _stride_img_0, int64_t const _stride_img_1, int64_t const _stride_img_2, double w_2)\n",
                             "{\n",
                             "   double * RESTRICT _data_img_22 = _data_img + 2*_stride_img_2;\n",
                             "   for (int64_t ctr_0 = 1; ctr_0 < _size_dst_0 - 1; ctr_0 += 1)\n",
@@ -1073,32 +1364,32 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_2</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"p\">{</span><span class=\"w\"></span>\n",
+                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_stride_img_2</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"p\">)</span>\n",
+                            "<span class=\"p\">{</span>\n",
                             "<span class=\"w\">   </span><span class=\"cp\">#pragma omp parallel num_threads(2)</span>\n",
-                            "<span class=\"w\">   </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2</span><span class=\"o\">*</span><span class=\"n\">_stride_img_2</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
+                            "<span class=\"w\">   </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_img</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2</span><span class=\"o\">*</span><span class=\"n\">_stride_img_2</span><span class=\"p\">;</span>\n",
                             "<span class=\"w\">      </span><span class=\"cp\">#pragma omp for schedule(static)</span>\n",
-                            "<span class=\"w\">      </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_00</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_01</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_0m1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">            </span><span class=\"n\">_data_dst_00</span><span class=\"p\">[</span><span class=\"n\">_stride_dst_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">])</span><span class=\"o\">*</span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]);</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"p\">}</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"p\">}</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"p\">}</span><span class=\"w\"></span>\n",
-                            "<span class=\"p\">}</span><span class=\"w\"></span>\n",
+                            "<span class=\"w\">      </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span>\n",
+                            "<span class=\"w\">      </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">         </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_00</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_dst_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">         </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_01</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">         </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_img_22_0m1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_img_22</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">         </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"n\">_size_dst_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span>\n",
+                            "<span class=\"w\">         </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">            </span><span class=\"n\">_data_dst_00</span><span class=\"p\">[</span><span class=\"n\">_stride_dst_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">])</span><span class=\"o\">*</span><span class=\"p\">(</span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">w_2</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_0m1</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">0.5</span><span class=\"o\">*</span><span class=\"n\">_data_img_22_01</span><span class=\"p\">[</span><span class=\"n\">_stride_img_1</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"n\">_stride_img_1</span><span class=\"p\">]);</span>\n",
+                            "<span class=\"w\">         </span><span class=\"p\">}</span>\n",
+                            "<span class=\"w\">      </span><span class=\"p\">}</span>\n",
+                            "<span class=\"w\">   </span><span class=\"p\">}</span>\n",
+                            "<span class=\"p\">}</span>\n",
                             "</pre></div>\n"
                         ],
                         "text/plain": [
                             "FUNC_PREFIX void kernel(double * RESTRICT  _data_dst, double * RESTRICT const _data_img, int64_t const _size_dst_0, int64_t const _size_dst_1, int64_t const _stride_dst_0, int64_t const _stride_dst_1, int64_t const _stride_img_0, int64_t const _stride_img_1, int64_t const _stride_img_2, double w_2)\n",
                             "{\n",
                             "   #pragma omp parallel num_threads(2)\n",
                             "   {\n",
@@ -1227,28 +1518,28 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">202</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_00</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">601</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_21_01</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I_21</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_21_0m1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I_21</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">600</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">         </span><span class=\"n\">_data_dst_00</span><span class=\"p\">[</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_01</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_0m1</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_0m1</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_0m1</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_01</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_I_21_01</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">];</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"p\">}</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"p\">}</span><span class=\"w\"></span>\n",
-                            "<span class=\"p\">}</span><span class=\"w\"></span>\n",
+                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">)</span>\n",
+                            "<span class=\"p\">{</span>\n",
+                            "<span class=\"w\">   </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">   </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">202</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span>\n",
+                            "<span class=\"w\">   </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_00</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">601</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_21_01</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I_21</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_21_0m1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I_21</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"k\">for</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">600</span><span class=\"p\">;</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+=</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">)</span>\n",
+                            "<span class=\"w\">      </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">         </span><span class=\"n\">_data_dst_00</span><span class=\"p\">[</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_01</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_0m1</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_0m1</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_0m1</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_21_01</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_I_21_01</span><span class=\"p\">[</span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"p\">];</span>\n",
+                            "<span class=\"w\">      </span><span class=\"p\">}</span>\n",
+                            "<span class=\"w\">   </span><span class=\"p\">}</span>\n",
+                            "<span class=\"p\">}</span>\n",
                             "</pre></div>\n"
                         ],
                         "text/plain": [
                             "FUNC_PREFIX void kernel(double * RESTRICT const _data_I, double * RESTRICT  _data_dst)\n",
                             "{\n",
                             "   double * RESTRICT _data_I_21 = _data_I + 1;\n",
                             "   for (int64_t ctr_0 = 1; ctr_0 < 202; ctr_0 += 1)\n",
@@ -1288,15 +1579,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Running on GPU\n",
                 "\n",
-                "If you have a CUDA enabled graphics card and [pycuda](https://mathema.tician.de/software/pycuda/) installed, *pystencils* can run your kernel on the GPU as well. You can find more details about this in the GPU tutorial."
+                "If you have a GPU and [cupy](https://cupy.dev/) installed, *pystencils* can run your kernel on the GPU as well. You can find more details about this in the GPU tutorial."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 36,
             "metadata": {},
             "outputs": [
@@ -1384,27 +1675,27 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"nf\">__launch_bounds__</span><span class=\"p\">(</span><span class=\"mi\">256</span><span class=\"p\">)</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"k\">if</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">202</span><span class=\"w\"> </span><span class=\"o\">&amp;&amp;</span><span class=\"w\"> </span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">600</span><span class=\"p\">)</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">   </span><span class=\"p\">{</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_10</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_11_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">5</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_1m1_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">3</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_10_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span><span class=\"w\"></span>\n",
-                            "<span class=\"w\">      </span><span class=\"n\">_data_dst_10</span><span class=\"p\">[</span><span class=\"mi\">601</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_11_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_11_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_1m1_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_10_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_10_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_I_1m1_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">];</span><span class=\"w\"></span>\n",
+                            "<div class=\"highlight\"><pre><span></span><span class=\"n\">FUNC_PREFIX</span><span class=\"w\"> </span><span class=\"nf\">__launch_bounds__</span><span class=\"p\">(</span><span class=\"mi\">256</span><span class=\"p\">)</span><span class=\"w\"> </span><span class=\"kt\">void</span><span class=\"w\"> </span><span class=\"n\">kernel</span><span class=\"p\">(</span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"p\">,</span><span class=\"w\"> </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst</span><span class=\"p\">)</span>\n",
+                            "<span class=\"p\">{</span>\n",
+                            "<span class=\"w\">   </span><span class=\"k\">if</span><span class=\"w\"> </span><span class=\"p\">(</span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">202</span><span class=\"w\"> </span><span class=\"o\">&amp;&amp;</span><span class=\"w\"> </span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"w\"> </span><span class=\"o\">&lt;</span><span class=\"w\"> </span><span class=\"mi\">600</span><span class=\"p\">)</span>\n",
+                            "<span class=\"w\">   </span><span class=\"p\">{</span>\n",
+                            "<span class=\"w\">      </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">x</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"k\">const</span><span class=\"w\"> </span><span class=\"kt\">int64_t</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">blockDim</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"o\">*</span><span class=\"n\">blockIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">threadIdx</span><span class=\"p\">.</span><span class=\"n\">y</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\">  </span><span class=\"n\">_data_dst_10</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_dst</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">ctr_1</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_11_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">5</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_1m1_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">3</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"kt\">double</span><span class=\"w\"> </span><span class=\"o\">*</span><span class=\"w\"> </span><span class=\"n\">RESTRICT</span><span class=\"w\"> </span><span class=\"n\">_data_I_10_21</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"n\">_data_I</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">4</span><span class=\"o\">*</span><span class=\"n\">ctr_1</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">1</span><span class=\"p\">;</span>\n",
+                            "<span class=\"w\">      </span><span class=\"n\">_data_dst_10</span><span class=\"p\">[</span><span class=\"mi\">601</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">=</span><span class=\"w\"> </span><span class=\"mf\">-1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_11_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_11_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">1.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_1m1_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_10_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">-</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mf\">2.0</span><span class=\"o\">*</span><span class=\"n\">_data_I_10_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">]</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"n\">_data_I_1m1_21</span><span class=\"p\">[</span><span class=\"mi\">2404</span><span class=\"o\">*</span><span class=\"n\">ctr_0</span><span class=\"w\"> </span><span class=\"o\">+</span><span class=\"w\"> </span><span class=\"mi\">2404</span><span class=\"p\">];</span>\n",
                             "<span class=\"w\">   </span><span class=\"p\">}</span><span class=\"w\"> </span>\n",
-                            "<span class=\"p\">}</span><span class=\"w\"></span>\n",
+                            "<span class=\"p\">}</span>\n",
                             "</pre></div>\n"
                         ],
                         "text/plain": [
                             "FUNC_PREFIX __launch_bounds__(256) void kernel(double * RESTRICT const _data_I, double * RESTRICT  _data_dst)\n",
                             "{\n",
                             "   if (blockDim.x*blockIdx.x + threadIdx.x + 1 < 202 && blockDim.y*blockIdx.y + threadIdx.y + 1 < 600)\n",
                             "   {\n",
@@ -1421,24 +1712,24 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "try:\n",
-                "    import pycuda\n",
-                "    from pystencils.gpucuda import BlockIndexing\n",
+                "    import cupy\n",
+                "    from pystencils.gpu import BlockIndexing\n",
                 "\n",
                 "    gpu_ast = create_kernel(update_rule, target=ps.Target.GPU,\n",
                 "                            gpu_indexing=BlockIndexing,\n",
                 "                            gpu_indexing_params={'blockSize': (64, 1, 1)})\n",
                 "\n",
                 "    ps.show_code(gpu_ast)\n",
                 "except ImportError:\n",
-                "    print(\"Please install pycuda for GPU support\")"
+                "    print(\"Please install cupy for GPU support\")"
             ]
         }
     ],
     "metadata": {
         "anaconda-cloud": {},
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
@@ -1451,13 +1742,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.11.0rc1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pystencils-1.2/doc/notebooks/02_tutorial_basic_kernels.ipynb` & `pystencils-1.3/doc/notebooks/02_tutorial_basic_kernels.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/notebooks/04_tutorial_advection_diffusion.ipynb` & `pystencils-1.3/doc/notebooks/04_tutorial_advection_diffusion.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/notebooks/05_tutorial_phasefield_spinodal_decomposition.ipynb` & `pystencils-1.3/doc/notebooks/05_tutorial_phasefield_spinodal_decomposition.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/notebooks/06_tutorial_phasefield_dentritic_growth.ipynb` & `pystencils-1.3/doc/notebooks/06_tutorial_phasefield_dentritic_growth.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.9.5'}}"}*

```diff
@@ -598,13 +598,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.9"
+            "version": "3.9.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `pystencils-1.2/doc/notebooks/demo_assignment_collection.ipynb` & `pystencils-1.3/doc/notebooks/demo_assignment_collection.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/notebooks/demo_benchmark.ipynb` & `pystencils-1.3/doc/notebooks/demo_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/notebooks/demo_derivatives.ipynb` & `pystencils-1.3/doc/notebooks/demo_derivatives.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/notebooks/demo_plotting_and_animation.ipynb` & `pystencils-1.3/doc/notebooks/demo_plotting_and_animation.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/sphinx/kernel_compile_and_call.rst` & `pystencils-1.3/doc/sphinx/kernel_compile_and_call.rst`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 .. autofunction:: pystencils.show_code
 
 
 GPU Indexing
 -------------
 
-.. autoclass:: pystencils.gpucuda.AbstractIndexing
+.. autoclass:: pystencils.gpu.AbstractIndexing
    :members:
 
-.. autoclass:: pystencils.gpucuda.BlockIndexing
+.. autoclass:: pystencils.gpu.BlockIndexing
    :members:
 
-.. autoclass:: pystencils.gpucuda.LineIndexing
+.. autoclass:: pystencils.gpu.LineIndexing
    :members:
```

### Comparing `pystencils-1.2/doc/sphinx/simplifications.rst` & `pystencils-1.3/doc/sphinx/simplifications.rst`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/doc/sphinx/tutorials.rst` & `pystencils-1.3/doc/sphinx/tutorials.rst`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/__init__.py` & `pystencils-1.3/pystencils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Module to generate stencil kernels in C or CUDA using sympy expressions and call them as Python functions"""
 from .enums import Backend, Target
 from . import fd
 from . import stencil as stencil
 from .assignment import Assignment, assignment_from_stencil
-from pystencils.typing.typed_sympy import TypedSymbol
-from .datahandling import create_data_handling
+from .typing.typed_sympy import TypedSymbol
 from .display_utils import get_code_obj, get_code_str, show_code, to_dot
 from .field import Field, FieldType, fields
 from .config import CreateKernelConfig
 from .cache import clear_cache
 from .kernel_decorator import kernel, kernel_config
 from .kernelcreation import create_kernel, create_staggered_kernel
 from .simp import AssignmentCollection
 from .slicing import make_slice
 from .spatial_coordinates import x_, x_staggered, x_staggered_vector, x_vector, y_, y_staggered, z_, z_staggered
 from .sympyextensions import SymbolCreator
+from .datahandling import create_data_handling
 
 __all__ = ['Field', 'FieldType', 'fields',
            'TypedSymbol',
            'make_slice',
            'CreateKernelConfig',
            'create_kernel', 'create_staggered_kernel',
            'Target', 'Backend',
@@ -36,7 +36,16 @@
            'fd',
            'stencil']
 
 from ._version import get_versions
 
 __version__ = get_versions()['version']
 del get_versions
+
+# setting the default GPU to the one with maximal memory. GPU_DEVICE is safe to overwrite for different needs
+try:
+    import cupy
+    if cupy.cuda.runtime.getDeviceCount() > 0:
+        GPU_DEVICE = sorted(range(cupy.cuda.runtime.getDeviceCount()),
+                            key=lambda i: cupy.cuda.Device(i).mem_info[1], reverse=True)[0]
+except ImportError:
+    pass
```

### Comparing `pystencils-1.2/pystencils/alignedarray.py` & `pystencils-1.3/pystencils/alignedarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
                                                                get_vector_instruction_set)
 
         instruction_sets = get_supported_instruction_sets()
         if instruction_sets is None:
             byte_alignment = 64
         elif byte_alignment == 'cacheline':
             cacheline_sizes = [get_cacheline_size(is_name) for is_name in instruction_sets]
-            if all([s is None for s in cacheline_sizes]):
+            if all([s is None for s in cacheline_sizes]) or \
+                    max([s for s in cacheline_sizes if s is not None]) > 0x100000:
                 widths = [get_vector_instruction_set(dtype, is_name)['width'] * np.dtype(dtype).itemsize
                           for is_name in instruction_sets
                           if type(get_vector_instruction_set(dtype, is_name)['width']) is int]
                 byte_alignment = 64 if all([s is None for s in widths]) else max(widths)
             else:
                 byte_alignment = max([s for s in cacheline_sizes if s is not None])
         elif not any([type(get_vector_instruction_set(dtype, is_name)['width']) is int
```

### Comparing `pystencils-1.2/pystencils/assignment.py` & `pystencils-1.3/pystencils/assignment.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/astnodes.py` & `pystencils-1.3/pystencils/astnodes.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/backends/arm_instruction_sets.py` & `pystencils-1.3/pystencils/backends/arm_instruction_sets.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,13 +147,11 @@
 
         result['&'] = f'vandq_u{bits[data_type]}' + '({0}, {1})'
         result['|'] = f'vorrq_u{bits[data_type]}' + '({0}, {1})'
         result['blendv'] = f'vbslq_f{bits[data_type]}' + '({2}, {1}, {0})'
         result['any'] = f'vaddlvq_u8(vreinterpretq_u8_u{bits[data_type]}({{0}})) > 0'
         result['all'] = f'vaddlvq_u8(vreinterpretq_u8_u{bits[data_type]}({{0}})) == 16*0xff'
 
-    if instruction_set == 'sve' or bitwidth & (bitwidth - 1) == 0:
-        # only power-of-2 vector sizes will evenly divide a cacheline
-        result['cachelineSize'] = 'cachelineSize()'
-        result['cachelineZero'] = 'cachelineZero((void*) {0})'
+    result['cachelineSize'] = 'cachelineSize()'
+    result['cachelineZero'] = 'cachelineZero((void*) {0})'
 
     return result
```

### Comparing `pystencils-1.2/pystencils/backends/cbackend.py` & `pystencils-1.3/pystencils/backends/cbackend.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/backends/cuda_backend.py` & `pystencils-1.3/pystencils/backends/cuda_backend.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/backends/dot.py` & `pystencils-1.3/pystencils/backends/dot.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/backends/json.py` & `pystencils-1.3/pystencils/backends/json.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/backends/ppc_instruction_sets.py` & `pystencils-1.3/pystencils/backends/ppc_instruction_sets.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/backends/riscv_instruction_sets.py` & `pystencils-1.3/pystencils/backends/riscv_instruction_sets.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/backends/simd_instruction_sets.py` & `pystencils-1.3/pystencils/backends/simd_instruction_sets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import math
 import os
 import platform
 from ctypes import CDLL
 from warnings import warn
 
 import numpy as np
 
 from pystencils.backends.x86_instruction_sets import get_vector_instruction_set_x86
 from pystencils.backends.arm_instruction_sets import get_vector_instruction_set_arm
 from pystencils.backends.ppc_instruction_sets import get_vector_instruction_set_ppc
 from pystencils.backends.riscv_instruction_sets import get_vector_instruction_set_riscv
+from pystencils.cache import memorycache
 from pystencils.typing import numpy_name_to_c
 
 
 def get_vector_instruction_set(data_type='double', instruction_set='avx'):
     if data_type == 'float':
         warn(f"Ambiguous input for data_type: {data_type}. For single precision please use float32. "
              f"For more information please take numpy.dtype as a reference. This input will not be supported in future "
@@ -28,98 +28,82 @@
         return get_vector_instruction_set_ppc(type_name, instruction_set)
     elif instruction_set in ['rvv']:
         return get_vector_instruction_set_riscv(type_name, instruction_set)
     else:
         return get_vector_instruction_set_x86(type_name, instruction_set)
 
 
-_cache = None
-_cachelinesize = None
-
-
+@memorycache
 def get_supported_instruction_sets():
     """List of supported instruction sets on current hardware, or None if query failed."""
-    global _cache
-    if _cache is not None:
-        return _cache.copy()
     if 'PYSTENCILS_SIMD' in os.environ:
         return os.environ['PYSTENCILS_SIMD'].split(',')
-    if (platform.system() == 'Darwin' or platform.system() == 'Linux') and platform.machine() == 'arm64':
-        # not supported by cpuinfo
+    if platform.system() == 'Darwin' and platform.machine() == 'arm64':
+        return ['neon']
+    elif platform.system() == 'Windows' and platform.machine() == 'ARM64':
         return ['neon']
-    elif platform.system() == 'Linux' and platform.machine().startswith('riscv'):  # not supported by cpuinfo
+    elif platform.system() == 'Linux' and platform.machine() == 'aarch64':
+        result = ['neon']  # Neon is mandatory on 64-bit ARM
+        libc = CDLL('libc.so.6')
+        hwcap = libc.getauxval(16)  # AT_HWCAP
+        if hwcap & (1 << 22):  # HWCAP_SVE
+            length = 8 * libc.prctl(51, 0, 0, 0, 0)  # PR_SVE_GET_VL
+            if length < 0:
+                raise OSError("SVE length query failed")
+            while length >= 128:
+                result.append(f"sve{length}")
+                length //= 2
+            result.append("sve")
+        return result
+    elif platform.system() == 'Linux' and platform.machine().startswith('riscv'):
         libc = CDLL('libc.so.6')
         hwcap = libc.getauxval(16)  # AT_HWCAP
         hwcap_isa_v = 1 << (ord('V') - ord('A'))  # COMPAT_HWCAP_ISA_V
         return ['rvv'] if hwcap & hwcap_isa_v else []
-    elif platform.machine().startswith('ppc64'):  # no flags reported by cpuinfo
-        import subprocess
-        import tempfile
-        from pystencils.cpu.cpujit import get_compiler_config
-        f = tempfile.NamedTemporaryFile(suffix='.cpp')
-        command = [get_compiler_config()['command'], '-mcpu=native', '-dM', '-E', f.name]
-        macros = subprocess.check_output(command, input='', text=True)
-        if '#define __VSX__' in macros and '#define __ALTIVEC__' in macros:
-            _cache = ['vsx']
-        else:
-            _cache = []
-        return _cache.copy()
-    try:
-        from cpuinfo import get_cpu_info
-    except ImportError:
-        return None
-
-    result = []
-    required_sse_flags = {'sse', 'sse2', 'ssse3', 'sse4_1', 'sse4_2'}
-    required_avx_flags = {'avx', 'avx2'}
-    required_avx512_flags = {'avx512f'}
-    required_neon_flags = {'neon'}
-    required_sve_flags = {'sve'}
-    flags = set(get_cpu_info()['flags'])
-    if flags.issuperset(required_sse_flags):
-        result.append("sse")
-    if flags.issuperset(required_avx_flags):
-        result.append("avx")
-    if flags.issuperset(required_avx512_flags):
-        result.append("avx512")
-    if flags.issuperset(required_neon_flags):
-        result.append("neon")
-    if flags.issuperset(required_sve_flags):
-        if platform.system() == 'Linux':
-            libc = CDLL('libc.so.6')
-            native_length = 8 * libc.prctl(51, 0, 0, 0, 0)  # PR_SVE_GET_VL
-            if native_length < 0:
-                raise OSError("SVE length query failed")
-            pwr2_length = int(2**math.floor(math.log2(native_length)))
-            if pwr2_length % 256 == 0:
-                result.append(f"sve{pwr2_length//2}")
-            if native_length != pwr2_length:
-                result.append(f"sve{pwr2_length}")
-            result.append(f"sve{native_length}")
-        result.append("sve")
-    return result
+    elif platform.system() == 'Linux' and platform.machine().startswith('ppc64'):
+        libc = CDLL('libc.so.6')
+        hwcap = libc.getauxval(16)  # AT_HWCAP
+        return ['vsx'] if hwcap & 0x00000080 else []  # PPC_FEATURE_HAS_VSX
+    elif platform.machine() in ['x86_64', 'x86', 'AMD64', 'i386']:
+        try:
+            from cpuinfo import get_cpu_info
+        except ImportError:
+            return None
+
+        result = []
+        required_sse_flags = {'sse', 'sse2', 'ssse3', 'sse4_1', 'sse4_2'}
+        required_avx_flags = {'avx', 'avx2'}
+        required_avx512_flags = {'avx512f'}
+        flags = set(get_cpu_info()['flags'])
+        if flags.issuperset(required_sse_flags):
+            result.append("sse")
+        if flags.issuperset(required_avx_flags):
+            result.append("avx")
+        if flags.issuperset(required_avx512_flags):
+            result.append("avx512")
+        return result
+    else:
+        raise NotImplementedError('Instruction set detection for %s on %s is not implemented' %
+                                  (platform.system(), platform.machine()))
 
 
+@memorycache
 def get_cacheline_size(instruction_set):
     """Get the size (in bytes) of a cache block that can be zeroed without memory access.
        Usually, this is identical to the cache line size."""
-    global _cachelinesize
     
     instruction_sets = get_vector_instruction_set('double', instruction_set)
     if 'cachelineSize' not in instruction_sets:
         return None
-    if _cachelinesize is not None:
-        return _cachelinesize
     
     import pystencils as ps
     from pystencils.astnodes import SympyAssignment
     import numpy as np
     from pystencils.cpu.vectorization import CachelineSize
     
     arr = np.zeros((1, 1), dtype=np.float32)
     f = ps.Field.create_from_numpy_array('f', arr, index_dimensions=0)
     ass = [CachelineSize(), SympyAssignment(f.center, CachelineSize.symbol)]
     ast = ps.create_kernel(ass, cpu_vectorize_info={'instruction_set': instruction_set})
     kernel = ast.compile()
     kernel(**{f.name: arr, CachelineSize.symbol.name: 0})
-    _cachelinesize = int(arr[0, 0])
-    return _cachelinesize
+    return int(arr[0, 0])
```

### Comparing `pystencils-1.2/pystencils/backends/x86_instruction_sets.py` & `pystencils-1.3/pystencils/backends/x86_instruction_sets.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/bit_masks.py` & `pystencils-1.3/pystencils/bit_masks.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/boundaries/boundaryconditions.py` & `pystencils-1.3/pystencils/boundaries/boundaryconditions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/boundaries/boundaryhandling.py` & `pystencils-1.3/pystencils/boundaries/boundaryhandling.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pystencils import create_kernel, CreateKernelConfig, Target
 from pystencils.astnodes import SympyAssignment
 from pystencils.backends.cbackend import CustomCodeNode
 from pystencils.boundaries.createindexlist import (
     create_boundary_index_array, numpy_data_type_for_boundary_object)
 from pystencils.typing import TypedSymbol, create_type
-from pystencils.datahandling.pycuda import PyCudaArrayHandler
+from pystencils.gpu.gpu_array_handler import GPUArrayHandler
 from pystencils.field import Field
 from pystencils.typing.typed_sympy import FieldPointerSymbol
 
 try:
     # noinspection PyPep8Naming
     import waLBerla as wlb
     if wlb.cpp_available:
@@ -96,15 +96,15 @@
         self._boundary_object_to_boundary_info = {}
         self.stencil = stencil
         self._dirty = True
         fi = flag_interface
         self.flag_interface = fi if fi is not None else FlagInterface(data_handling, name + "Flags")
 
         if ParallelDataHandling and isinstance(self.data_handling, ParallelDataHandling):
-            array_handler = PyCudaArrayHandler()
+            array_handler = GPUArrayHandler()
         else:
             array_handler = self.data_handling.array_handler
 
         def to_cpu(gpu_version, cpu_version):
             gpu_version = gpu_version.boundary_object_to_index_list
             cpu_version = cpu_version.boundary_object_to_index_list
             for obj, cpu_arr in cpu_version.items():
@@ -112,15 +112,16 @@
 
         def to_gpu(gpu_version, cpu_version):
             gpu_version = gpu_version.boundary_object_to_index_list
             cpu_version = cpu_version.boundary_object_to_index_list
 
             for obj, cpu_arr in cpu_version.items():
                 if obj not in gpu_version or gpu_version[obj].shape != cpu_arr.shape:
-                    gpu_version[obj] = array_handler.to_gpu(cpu_arr)
+                    gpu_version[obj] = array_handler.empty(cpu_arr.shape, cpu_arr.dtype)
+                    array_handler.upload(gpu_version[obj], cpu_arr)
                 else:
                     array_handler.upload(gpu_version[obj], cpu_arr)
 
         class_ = self.IndexFieldBlockData
         class_.to_cpu = to_cpu
         class_.to_gpu = to_gpu
         gpu = self._target in data_handling._GPU_LIKE_TARGETS
```

### Comparing `pystencils-1.2/pystencils/boundaries/createindexlist.py` & `pystencils-1.3/pystencils/boundaries/createindexlist.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/boundaries/createindexlistcython.c` & `pystencils-1.3/pystencils/boundaries/createindexlistcython.c`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/boundaries/createindexlistcython.pyx` & `pystencils-1.3/pystencils/boundaries/createindexlistcython.pyx`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/boundaries/inkernel.py` & `pystencils-1.3/pystencils/boundaries/inkernel.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/cache.py` & `pystencils-1.3/pystencils/cache.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/config.py` & `pystencils-1.3/pystencils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     """
     omp_single_loop: bool = True
     """
     If OpenMP is active: whether multiple outer loops are permitted
     """
     gpu_indexing: str = 'block'
     """
-    Either 'block' or 'line' , or custom indexing class, see `pystencils.gpucuda.AbstractIndexing`
+    Either 'block' or 'line' , or custom indexing class, see `pystencils.gpu.AbstractIndexing`
     """
     gpu_indexing_params: MappingProxyType = field(default_factory=lambda: MappingProxyType({}))
     """
     Dict with indexing parameters (constructor parameters of indexing class)
     e.g. for 'block' one can specify '{'block_size': (20, 20, 10) }'.
     """
     # TODO Markus rework this docstring
```

### Comparing `pystencils-1.2/pystencils/cpu/cpujit.py` & `pystencils-1.3/pystencils/cpu/cpujit.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,27 +142,28 @@
     if platform.system().lower() == 'linux':
         default_compiler_config = OrderedDict([
             ('os', 'linux'),
             ('command', 'g++'),
             ('flags', '-Ofast -DNDEBUG -fPIC -march=native -fopenmp -std=c++11'),
             ('restrict_qualifier', '__restrict__')
         ])
-        if platform.machine() == 'arm64':
-            default_compiler_config['flags'] = default_compiler_config['flags'].replace('-march=native', '')
-        elif platform.machine().startswith('ppc64'):
+        if platform.machine().startswith('ppc64') or platform.machine() == 'arm64':
             default_compiler_config['flags'] = default_compiler_config['flags'].replace('-march=native',
                                                                                         '-mcpu=native')
     elif platform.system().lower() == 'windows':
         default_compiler_config = OrderedDict([
             ('os', 'windows'),
             ('msvc_version', 'latest'),
             ('arch', 'x64'),
             ('flags', '/Ox /fp:fast /OpenMP /arch:avx'),
             ('restrict_qualifier', '__restrict')
         ])
+        if platform.machine() == 'ARM64':
+            default_compiler_config['arch'] = 'ARM64'
+            default_compiler_config['flags'] = default_compiler_config['flags'].replace(' /arch:avx', '')
     elif platform.system().lower() == 'darwin':
         default_compiler_config = OrderedDict([
             ('os', 'darwin'),
             ('command', 'clang++'),
             ('flags', '-Ofast -DNDEBUG -fPIC -march=native -Xclang -fopenmp -std=c++11'),
             ('restrict_qualifier', '__restrict__')
         ])
@@ -170,16 +171,16 @@
             default_compiler_config['flags'] = default_compiler_config['flags'].replace('-march=native ', '')
         for libomp in ['/opt/local/lib/libomp/libomp.dylib', '/usr/local/lib/libomp.dylib',
                        '/opt/homebrew/lib/libomp.dylib']:
             if os.path.exists(libomp):
                 default_compiler_config['flags'] += ' ' + libomp
                 break
     else:
-        raise ValueError("The detection of the platform with platform.system() did not work. "
-                         "Pystencils is only supported for linux, windows, and darwin platforms.")
+        raise NotImplementedError('Generation of default compiler flags for %s is not implemented' %
+                                  (platform.system(),))
 
     default_cache_config = OrderedDict([
         ('object_cache', os.path.join(user_cache_dir('pystencils'), 'objectcache')),
         ('clear_cache_on_start', False),
     ])
 
     default_config = OrderedDict([('compiler', default_compiler_config),
@@ -389,15 +390,16 @@
                     if 'cachelineZero' in ast_node.instruction_set:
                         has_openmp, has_nontemporal = False, False
                         for loop in ast_node.atoms(LoopOverCoordinate):
                             has_openmp = has_openmp or any(['#pragma omp' in p for p in loop.prefix_lines])
                             has_nontemporal = has_nontemporal or any([a.args[0].field == field and a.args[3] for a in
                                                                       loop.atoms(VectorMemoryAccess)])
                         if has_openmp and has_nontemporal:
-                            byte_width = ast_node.instruction_set['cachelineSize']
+                            cl_size = ast_node.instruction_set['cachelineSize']
+                            byte_width = f"({cl_size}) < SIZE_MAX ? ({cl_size}) : ({byte_width})"
                     offset = max(max(ast_node.ghost_layers)) * item_size
                     offset_cond = f"(((uintptr_t) buffer_{field.name}.buf) + {offset}) % ({byte_width}) == 0"
 
                     message = str(offset) + ". This is probably due to a different number of ghost_layers chosen for " \
                                             "the arrays and the kernel creation. If the number of ghost layers for " \
                                             "the kernel creation is not specified it will choose a suitable value " \
                                             "automatically. This value might not " \
```

### Comparing `pystencils-1.2/pystencils/cpu/kernelcreation.py` & `pystencils-1.3/pystencils/cpu/kernelcreation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/cpu/msvc_detection.py` & `pystencils-1.3/pystencils/cpu/msvc_detection.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/cpu/vectorization.py` & `pystencils-1.3/pystencils/cpu/vectorization.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/datahandling/__init__.py` & `pystencils-1.3/pystencils/datahandling/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/datahandling/blockiteration.py` & `pystencils-1.3/pystencils/datahandling/blockiteration.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     def __getitem__(self, data_name):
         result = self._block[self._name_prefix + data_name]
         type_name = type(result).__name__
         if 'GhostLayerField' in type_name:
             result = wlb.field.toArray(result, with_ghost_layers=self._gls)
             result = self._normalize_array_shape(result)
         elif 'GpuField' in type_name:
-            result = wlb.cuda.toGpuArray(result, with_ghost_layers=self._gls)
+            result = wlb.gpu.toGpuArray(result, with_ghost_layers=self._gls)
             result = self._normalize_array_shape(result)
         return result
 
     def _normalize_array_shape(self, arr):
         if arr.shape[-1] == 1 and len(arr.shape) == 4:
             arr = arr[..., 0]
         return arr[self._localSlice]
```

### Comparing `pystencils-1.2/pystencils/datahandling/datahandling_interface.py` & `pystencils-1.3/pystencils/datahandling/datahandling_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,14 +327,15 @@
             if value_idx is not None:
                 if isinstance(value_idx, int):
                     value_idx = (value_idx,)
                 assert len(value_idx) == len(self.values_per_cell(array_name))
                 b[array_name][(Ellipsis, *value_idx)].fill(val)
             else:
                 b[array_name].fill(val)
+            self.to_gpu(array_name)
 
     def min(self, array_name, slice_obj=None, ghost_layers=False, inner_ghost_layers=False, reduce=True):
         """Returns the minimum value inside the domain or slice of the domain.
 
         For meaning of arguments see documentation of :func:`DataHandling.fill`.
 
         Returns:
```

### Comparing `pystencils-1.2/pystencils/datahandling/parallel_datahandling.py` & `pystencils-1.3/pystencils/datahandling/parallel_datahandling.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 
         if cpu:
             wlb.field.addToStorage(self.blocks, name, dtype, fSize=values_per_cell, layout=layout_map[layout],
                                    ghostLayers=ghost_layers, alignment=alignment)
         if gpu:
             if alignment != 0:
                 raise ValueError("Alignment for walberla GPU fields not yet supported")
-            wlb.cuda.addGpuFieldToStorage(self.blocks, self.GPU_DATA_PREFIX + name, dtype, fSize=values_per_cell,
-                                          usePitchedMem=False, ghostLayers=ghost_layers, layout=layout_map[layout])
+            wlb.gpu.addGpuFieldToStorage(self.blocks, self.GPU_DATA_PREFIX + name, dtype, fSize=values_per_cell,
+                                         usePitchedMem=False, ghostLayers=ghost_layers, layout=layout_map[layout])
 
         if cpu and gpu:
             self._cpu_gpu_pairs.append((name, self.GPU_DATA_PREFIX + name))
 
         block_bb = self.blocks.getBlockCellBB(self.blocks[0])
         shape = tuple(s + 2 * ghost_layers for s in block_bb.size[:self.dim])
         index_dimensions = 1 if values_per_cell > 1 else 0
@@ -251,15 +251,15 @@
     def run_kernel(self, kernel_function, **kwargs):
         for arg_dict in self.get_kernel_kwargs(kernel_function, **kwargs):
             kernel_function(**arg_dict)
 
     def get_kernel_kwargs(self, kernel_function, **kwargs):
         if kernel_function.ast.backend == Backend.CUDA:
             name_map = self._field_name_to_gpu_data_name
-            to_array = wlb.cuda.toGpuArray
+            to_array = wlb.gpu.toGpuArray
         else:
             name_map = self._field_name_to_cpu_data_name
             to_array = wlb.field.toArray
         data_used_in_kernel = [(name_map[p.symbol.field_name], self.fields[p.symbol.field_name])
                                for p in kernel_function.parameters if
                                isinstance(p.symbol, FieldPointerSymbol) and p.symbol.field_name not in kwargs]
 
@@ -276,36 +276,38 @@
 
     def to_cpu(self, name):
         if name in self._custom_data_transfer_functions:
             transfer_func = self._custom_data_transfer_functions[name][1]
             for block in self.blocks:
                 transfer_func(block[self.GPU_DATA_PREFIX + name], block[name])
         else:
-            wlb.cuda.copyFieldToCpu(self.blocks, self.GPU_DATA_PREFIX + name, name)
+            if self.is_on_gpu(name):
+                wlb.gpu.copyFieldToCpu(self.blocks, self.GPU_DATA_PREFIX + name, name)
 
     def to_gpu(self, name):
         if name in self._custom_data_transfer_functions:
             transfer_func = self._custom_data_transfer_functions[name][0]
             for block in self.blocks:
                 transfer_func(block[self.GPU_DATA_PREFIX + name], block[name])
         else:
-            wlb.cuda.copyFieldToGpu(self.blocks, self.GPU_DATA_PREFIX + name, name)
+            if self.is_on_gpu(name):
+                wlb.gpu.copyFieldToGpu(self.blocks, self.GPU_DATA_PREFIX + name, name)
 
     def is_on_gpu(self, name):
         return (name, self.GPU_DATA_PREFIX + name) in self._cpu_gpu_pairs
 
     def all_to_cpu(self):
         for cpu_name, gpu_name in self._cpu_gpu_pairs:
-            wlb.cuda.copyFieldToCpu(self.blocks, gpu_name, cpu_name)
+            wlb.gpu.copyFieldToCpu(self.blocks, gpu_name, cpu_name)
         for name in self._custom_data_transfer_functions.keys():
             self.to_cpu(name)
 
     def all_to_gpu(self):
         for cpu_name, gpu_name in self._cpu_gpu_pairs:
-            wlb.cuda.copyFieldToGpu(self.blocks, gpu_name, cpu_name)
+            wlb.gpu.copyFieldToGpu(self.blocks, gpu_name, cpu_name)
         for name in self._custom_data_transfer_functions.keys():
             self.to_gpu(name)
 
     def synchronization_function_cpu(self, names, stencil=None, buffered=True, stencil_restricted=False, **_):
         return self.synchronization_function(names, stencil, Target.CPU, buffered, stencil_restricted)
 
     def synchronization_function_gpu(self, names, stencil=None, buffered=True, stencil_restricted=False, **_):
@@ -324,15 +326,15 @@
         create_scheme = wlb.createUniformBufferedScheme if buffered else wlb.createUniformDirectScheme
         if target == Target.CPU:
             create_packing = wlb.field.createPackInfo if buffered else wlb.field.createMPIDatatypeInfo
             if buffered and stencil_restricted:
                 create_packing = wlb.field.createStencilRestrictedPackInfo
         else:
             assert target == Target.GPU
-            create_packing = wlb.cuda.createPackInfo if buffered else wlb.cuda.createMPIDatatypeInfo
+            create_packing = wlb.gpu.createPackInfo if buffered else wlb.gpu.createMPIDatatypeInfo
             names = [self.GPU_DATA_PREFIX + name for name in names]
 
         sync_function = create_scheme(self.blocks, stencil)
         for name in names:
             sync_function.addDataToCommunicate(create_packing(self.blocks, name))
 
         return sync_function
```

### Comparing `pystencils-1.2/pystencils/datahandling/serial_datahandling.py` & `pystencils-1.3/pystencils/datahandling/serial_datahandling.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import time
 from typing import Sequence, Union
 
 import numpy as np
 
 from pystencils.datahandling.blockiteration import SerialBlock
 from pystencils.datahandling.datahandling_interface import DataHandling
-from pystencils.datahandling.pycuda import PyCudaArrayHandler, PyCudaNotAvailableHandler
 from pystencils.enums import Target
-from pystencils.field import (
-    Field, FieldType, create_numpy_array_with_layout, layout_string_to_tuple,
-    spatial_layout_string_to_tuple)
+from pystencils.field import (Field, FieldType, create_numpy_array_with_layout,
+                              layout_string_to_tuple, spatial_layout_string_to_tuple)
+from pystencils.gpu.gpu_array_handler import GPUArrayHandler, GPUNotAvailableHandler
 from pystencils.slicing import normalize_slice, remove_ghost_layers
 from pystencils.utils import DotDict
 
 
 class SerialDataHandling(DataHandling):
 
     def __init__(self,
@@ -44,17 +43,17 @@
         self.gpu_arrays = DotDict()
         self.custom_data_cpu = DotDict()
         self.custom_data_gpu = DotDict()
         self._custom_data_transfer_functions = {}
 
         if not array_handler:
             try:
-                self.array_handler = PyCudaArrayHandler()
+                self.array_handler = GPUArrayHandler()
             except Exception:
-                self.array_handler = PyCudaNotAvailableHandler()
+                self.array_handler = GPUNotAvailableHandler()
         else:
             self.array_handler = array_handler
 
         if periodicity is None or periodicity is False:
             periodicity = [False] * self.dim
         if periodicity is True:
             periodicity = [True] * self.dim
@@ -122,18 +121,22 @@
         kwargs['shape'] = kwargs['shape'] + values_per_cell
 
         if index_dimensions > 0:
             layout_tuple = layout_string_to_tuple(layout, self.dim + index_dimensions)
         else:
             layout_tuple = spatial_layout_string_to_tuple(layout, self.dim)
 
-        # cpu_arr is always created - since there is no create_pycuda_array_with_layout()
+        # cpu_arr is always created - since there is no create_gpu_array_with_layout()
         byte_offset = ghost_layers * np.dtype(dtype).itemsize
-        cpu_arr = create_numpy_array_with_layout(layout=layout_tuple, alignment=alignment,
-                                                 byte_offset=byte_offset, **kwargs)
+
+        if gpu:
+            cpu_arr = self.array_handler.pinned_numpy_array(shape=kwargs['shape'], layout=layout_tuple, dtype=dtype)
+        else:
+            cpu_arr = create_numpy_array_with_layout(layout=layout_tuple, alignment=alignment,
+                                                     byte_offset=byte_offset, **kwargs)
 
         if alignment and gpu:
             raise NotImplementedError("Alignment for GPU fields not supported")
 
         if cpu:
             if name in self.cpu_arrays:
                 raise ValueError("CPU Field with this name already exists")
@@ -247,22 +250,24 @@
         return [result]
 
     def to_cpu(self, name):
         if name in self._custom_data_transfer_functions:
             transfer_func = self._custom_data_transfer_functions[name][1]
             transfer_func(self.custom_data_gpu[name], self.custom_data_cpu[name])
         else:
-            self.array_handler.download(self.gpu_arrays[name], self.cpu_arrays[name])
+            if name in self.cpu_arrays.keys() & self.gpu_arrays.keys():
+                self.array_handler.download(self.gpu_arrays[name], self.cpu_arrays[name])
 
     def to_gpu(self, name):
         if name in self._custom_data_transfer_functions:
             transfer_func = self._custom_data_transfer_functions[name][0]
             transfer_func(self.custom_data_gpu[name], self.custom_data_cpu[name])
         else:
-            self.array_handler.upload(self.gpu_arrays[name], self.cpu_arrays[name])
+            if name in self.cpu_arrays.keys() & self.gpu_arrays.keys():
+                self.array_handler.upload(self.gpu_arrays[name], self.cpu_arrays[name])
 
     def is_on_gpu(self, name):
         return name in self.gpu_arrays
 
     def synchronization_function_cpu(self, names, stencil_name=None, **_):
         return self.synchronization_function(names, stencil_name, target=Target.CPU)
 
@@ -309,15 +314,15 @@
                 if target == Target.CPU:
                     if functor is None:
                         from pystencils.slicing import get_periodic_boundary_functor
                         functor = get_periodic_boundary_functor
                     result.append(functor(filtered_stencil, ghost_layers=gls))
                 else:
                     if functor is None:
-                        from pystencils.gpucuda.periodicity import get_periodic_boundary_functor as functor
+                        from pystencils.gpu.periodicity import get_periodic_boundary_functor as functor
                         target = Target.GPU
                     result.append(functor(filtered_stencil, self._domainSize,
                                           index_dimensions=self.fields[name].index_dimensions,
                                           index_dim_shape=values_per_cell,
                                           dtype=self.fields[name].dtype.numpy_dtype,
                                           ghost_layers=gls,
                                           target=target))
@@ -415,23 +420,32 @@
     def is_root(self):
         return True
 
     @property
     def world_rank(self):
         return 0
 
-    def save_all(self, file):
-        np.savez_compressed(file, **self.cpu_arrays)
+    def save_all(self, filename, compressed=True, synchronise_data=True):
+        if synchronise_data:
+            for name in (self.cpu_arrays.keys() & self.gpu_arrays.keys()):
+                self.to_cpu(name)
+        if compressed:
+            np.savez_compressed(filename, **self.cpu_arrays)
+        else:
+            np.savez(filename, **self.cpu_arrays)
 
-    def load_all(self, file):
-        if '.npz' not in file:
-            file += '.npz'
-        file_contents = np.load(file)
+    def load_all(self, filename, synchronise_data=True):
+        if '.npz' not in filename:
+            filename += '.npz'
+        file_contents = np.load(filename)
         for arr_name, arr_contents in self.cpu_arrays.items():
             if arr_name not in file_contents:
                 print(f"Skipping read data {arr_name} because there is no data with this name in data handling")
                 continue
             if file_contents[arr_name].shape != arr_contents.shape:
                 print(f"Skipping read data {arr_name} because shapes don't match. "
                       f"Read array shape {file_contents[arr_name].shape}, existing array shape {arr_contents.shape}")
                 continue
             np.copyto(arr_contents, file_contents[arr_name])
+            if synchronise_data:
+                if arr_name in self.gpu_arrays.keys():
+                    self.to_gpu(arr_name)
```

### Comparing `pystencils-1.2/pystencils/datahandling/vtk.py` & `pystencils-1.3/pystencils/datahandling/vtk.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/display_utils.py` & `pystencils-1.3/pystencils/display_utils.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/enums.py` & `pystencils-1.3/pystencils/enums.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/fast_approximation.py` & `pystencils-1.3/pystencils/fast_approximation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/fd/__init__.py` & `pystencils-1.3/pystencils/fd/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/fd/derivation.py` & `pystencils-1.3/pystencils/fd/derivation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/fd/derivative.py` & `pystencils-1.3/pystencils/fd/derivative.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/fd/finitedifferences.py` & `pystencils-1.3/pystencils/fd/finitedifferences.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/fd/finitevolumes.py` & `pystencils-1.3/pystencils/fd/finitevolumes.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/fd/spatial.py` & `pystencils-1.3/pystencils/fd/spatial.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/field.py` & `pystencils-1.3/pystencils/field.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/functions.py` & `pystencils-1.3/pystencils/functions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/gpucuda/cudajit.py` & `pystencils-1.3/pystencils/gpu/cudajit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 
+import pystencils
 from pystencils.backends.cbackend import get_headers
 from pystencils.backends.cuda_backend import generate_cuda
 from pystencils.typing import StructType
 from pystencils.field import FieldType
-from pystencils.include import get_pycuda_include_path, get_pystencils_include_path
+from pystencils.include import get_pystencils_include_path
 from pystencils.kernel_wrapper import KernelWrapper
 from pystencils.typing.typed_sympy import FieldPointerSymbol
 
 USE_FAST_MATH = True
 
 
 def get_cubic_interpolation_include_paths():
@@ -17,73 +18,82 @@
     return [join(dirname(__file__), "CubicInterpolationCUDA", "code"),
             join(dirname(__file__), "CubicInterpolationCUDA", "code", "internal")]
 
 
 def make_python_function(kernel_function_node, argument_dict=None, custom_backend=None):
     """
     Creates a kernel function from an abstract syntax tree which
-    was created e.g. by :func:`pystencils.gpucuda.create_cuda_kernel`
-    or :func:`pystencils.gpucuda.created_indexed_cuda_kernel`
+    was created e.g. by :func:`pystencils.gpu.create_cuda_kernel`
+    or :func:`pystencils.gpu.created_indexed_cuda_kernel`
 
     Args:
         kernel_function_node: the abstract syntax tree
         argument_dict: parameters passed here are already fixed. Remaining parameters have to be passed to the
                        returned kernel functor.
+        custom_backend: use own custom printer for code generation
 
     Returns:
         compiled kernel as Python function
     """
-    import pycuda.autoinit  # NOQA
-    from pycuda.compiler import SourceModule
+    import cupy as cp
 
     if argument_dict is None:
         argument_dict = {}
 
-    header_list = ['<cstdint>'] + list(get_headers(kernel_function_node))
+    if cp.cuda.runtime.is_hip:
+        header_list = ['"gpu_defines.h"'] + list(get_headers(kernel_function_node))
+    else:
+        header_list = ['"gpu_defines.h"', '<cstdint>'] + list(get_headers(kernel_function_node))
     includes = "\n".join([f"#include {include_file}" for include_file in header_list])
 
     code = includes + "\n"
     code += "#define FUNC_PREFIX __global__\n"
     code += "#define RESTRICT __restrict__\n\n"
     code += str(generate_cuda(kernel_function_node, custom_backend=custom_backend))
+    code = 'extern "C" {\n%s\n}\n' % code
 
-    nvcc_options = ["-w", "-std=c++11", "-Wno-deprecated-gpu-targets"]
+    options = ["-w", "-std=c++11"]
     if USE_FAST_MATH:
-        nvcc_options.append("-use_fast_math")
+        options.append("-use_fast_math")
+    options.append("-I" + get_pystencils_include_path())
 
-    mod = SourceModule(code, options=nvcc_options, include_dirs=[
-                       get_pystencils_include_path(), get_pycuda_include_path()])
+    mod = cp.RawModule(code=code, options=tuple(options), backend="nvrtc", jitify=True)
     func = mod.get_function(kernel_function_node.function_name)
 
     parameters = kernel_function_node.get_parameters()
 
     cache = {}
     cache_values = []
 
     def wrapper(**kwargs):
         key = hash(tuple((k, v.ctypes.data, v.strides, v.shape) if isinstance(v, np.ndarray) else (k, id(v))
                          for k, v in kwargs.items()))
         try:
             args, block_and_thread_numbers = cache[key]
-            func(*args, **block_and_thread_numbers)
+            with cp.cuda.Device(pystencils.GPU_DEVICE):
+                func(block_and_thread_numbers['grid'], block_and_thread_numbers['block'], args)
         except KeyError:
             full_arguments = argument_dict.copy()
             full_arguments.update(kwargs)
             shape = _check_arguments(parameters, full_arguments)
 
             indexing = kernel_function_node.indexing
             block_and_thread_numbers = indexing.call_parameters(shape)
             block_and_thread_numbers['block'] = tuple(int(i) for i in block_and_thread_numbers['block'])
             block_and_thread_numbers['grid'] = tuple(int(i) for i in block_and_thread_numbers['grid'])
 
-            args = _build_numpy_argument_list(parameters, full_arguments)
+            args = tuple(_build_numpy_argument_list(parameters, full_arguments))
             cache[key] = (args, block_and_thread_numbers)
             cache_values.append(kwargs)  # keep objects alive such that ids remain unique
-            func(*args, **block_and_thread_numbers)
-        # import pycuda.driver as cuda
+            with cp.cuda.Device(pystencils.GPU_DEVICE):
+                func(block_and_thread_numbers['grid'], block_and_thread_numbers['block'], args)
+            # useful for debugging:
+            # with cp.cuda.Device(pystencils.GPU_DEVICE):
+            #     cp.cuda.runtime.deviceSynchronize()
+
         # cuda.Context.synchronize() # useful for debugging, to get errors right after kernel was called
     ast = kernel_function_node
     parameters = kernel_function_node.get_parameters()
     wrapper = KernelWrapper(wrapper, parameters, ast)
     wrapper.num_regs = func.num_regs
     return wrapper
 
@@ -94,16 +104,16 @@
 
     for param in parameters:
         if param.is_field_pointer:
             array = argument_dict[param.field_name]
             actual_type = array.dtype
             expected_type = param.fields[0].dtype.numpy_dtype
             if expected_type != actual_type:
-                raise ValueError("Data type mismatch for field '%s'. Expected '%s' got '%s'." %
-                                 (param.field_name, expected_type, actual_type))
+                raise ValueError(f"Data type mismatch for field {param.field_name}. "
+                                 f"Expected {expected_type} got {actual_type}.")
             result.append(array)
         elif param.is_field_stride:
             cast_to_dtype = param.symbol.dtype.numpy_dtype.type
             array = argument_dict[param.field_name]
             stride = cast_to_dtype(array.strides[param.symbol.coordinate] // array.dtype.itemsize)
             result.append(stride)
         elif param.is_field_shape:
@@ -130,38 +140,38 @@
     for param in parameter_specification:
         if isinstance(param.symbol, FieldPointerSymbol):
             symbolic_field = param.fields[0]
 
             try:
                 field_arr = argument_dict[symbolic_field.name]
             except KeyError:
-                raise KeyError("Missing field parameter for kernel call " + str(symbolic_field))
+                raise KeyError(f"Missing field parameter for kernel call {str(symbolic_field)}")
 
             if symbolic_field.has_fixed_shape:
                 symbolic_field_shape = tuple(int(i) for i in symbolic_field.shape)
                 if isinstance(symbolic_field.dtype, StructType):
                     symbolic_field_shape = symbolic_field_shape[:-1]
                 if symbolic_field_shape != field_arr.shape:
-                    raise ValueError("Passed array '%s' has shape %s which does not match expected shape %s" %
-                                     (symbolic_field.name, str(field_arr.shape), str(symbolic_field.shape)))
+                    raise ValueError(f"Passed array {symbolic_field.name} has shape {str(field_arr.shape)} "
+                                     f"which does not match expected shape {str(symbolic_field.shape)}")
             if symbolic_field.has_fixed_shape:
                 symbolic_field_strides = tuple(int(i) * field_arr.dtype.itemsize for i in symbolic_field.strides)
                 if isinstance(symbolic_field.dtype, StructType):
                     symbolic_field_strides = symbolic_field_strides[:-1]
                 if symbolic_field_strides != field_arr.strides:
-                    raise ValueError("Passed array '%s' has strides %s which does not match expected strides %s" %
-                                     (symbolic_field.name, str(field_arr.strides), str(symbolic_field_strides)))
+                    raise ValueError(f"Passed array {symbolic_field.name} has strides {str(field_arr.strides)} "
+                                     f"which does not match expected strides {str(symbolic_field_strides)}")
 
             if FieldType.is_indexed(symbolic_field):
                 index_arr_shapes.add(field_arr.shape[:symbolic_field.spatial_dimensions])
             elif FieldType.is_generic(symbolic_field):
                 array_shapes.add(field_arr.shape[:symbolic_field.spatial_dimensions])
 
     if len(array_shapes) > 1:
-        raise ValueError("All passed arrays have to have the same size " + str(array_shapes))
+        raise ValueError(f"All passed arrays have to have the same size {str(array_shapes)}")
     if len(index_arr_shapes) > 1:
-        raise ValueError("All passed index arrays have to have the same size " + str(array_shapes))
+        raise ValueError(f"All passed index arrays have to have the same size {str(array_shapes)}")
 
     if len(index_arr_shapes) > 0:
         return list(index_arr_shapes)[0]
     else:
         return list(array_shapes)[0]
```

### Comparing `pystencils-1.2/pystencils/gpucuda/indexing.py` & `pystencils-1.3/pystencils/gpu/indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 from functools import partial
 
 import sympy as sp
 from sympy.core.cache import cacheit
 
+import pystencils
 from pystencils.astnodes import Block, Conditional
 from pystencils.typing import TypedSymbol, create_type
 from pystencils.integer_functions import div_ceil, div_floor
 from pystencils.slicing import normalize_slice
 from pystencils.sympyextensions import is_integer_sequence, prod
 
 
@@ -29,28 +30,28 @@
 BLOCK_DIM = [ThreadIndexingSymbol("blockDim." + coord, create_type("int32")) for coord in ('x', 'y', 'z')]
 GRID_DIM = [ThreadIndexingSymbol("gridDim." + coord, create_type("int32")) for coord in ('x', 'y', 'z')]
 
 
 class AbstractIndexing(abc.ABC):
     """
     Abstract base class for all Indexing classes. An Indexing class defines how a multidimensional
-    field is mapped to CUDA's block and grid system. It calculates indices based on CUDA's thread and block indices
+    field is mapped to GPU's block and grid system. It calculates indices based on GPU's thread and block indices
     and computes the number of blocks and threads a kernel is started with. The Indexing class is created with
     a pystencils field, a slice to iterate over, and further optional parameters that must have default values.
     """
 
     @property
     @abc.abstractmethod
     def coordinates(self):
-        """Returns a sequence of coordinate expressions for (x,y,z) depending on symbolic CUDA block and thread indices.
+        """Returns a sequence of coordinate expressions for (x,y,z) depending on symbolic GPU block and thread indices.
         These symbolic indices can be obtained with the method `index_variables` """
 
     @property
     def index_variables(self):
-        """Sympy symbols for CUDA's block and thread indices, and block and grid dimensions. """
+        """Sympy symbols for GPU's block and thread indices, and block and grid dimensions. """
         return BLOCK_IDX + THREAD_IDX + BLOCK_DIM + GRID_DIM
 
     @abc.abstractmethod
     def call_parameters(self, arr_shape):
         """Determine grid and block size for kernel call.
 
         Args:
@@ -84,43 +85,40 @@
         """Set of symbols required in call_parameters code"""
 
 
 # -------------------------------------------- Implementations ---------------------------------------------------------
 
 
 class BlockIndexing(AbstractIndexing):
-    """Generic indexing scheme that maps sub-blocks of an array to CUDA blocks.
+    """Generic indexing scheme that maps sub-blocks of an array to GPU blocks.
 
     Args:
         field: pystencils field (common to all Indexing classes)
         iteration_slice: slice that defines rectangular subarea which is iterated over
         permute_block_size_dependent_on_layout: if True the block_size is permuted such that the fastest coordinate
                                                 gets the largest amount of threads
-        compile_time_block_size: compile in concrete block size, otherwise the cuda variable 'blockDim' is used
+        compile_time_block_size: compile in concrete block size, otherwise the gpu variable 'blockDim' is used
     """
 
     def __init__(self, field, iteration_slice,
                  block_size=(16, 16, 1), permute_block_size_dependent_on_layout=True, compile_time_block_size=False,
                  maximum_block_size=(1024, 1024, 64)):
         if field.spatial_dimensions > 3:
             raise NotImplementedError("This indexing scheme supports at most 3 spatial dimensions")
 
         if permute_block_size_dependent_on_layout:
             block_size = self.permute_block_size_according_to_layout(block_size, field.layout)
 
         self._block_size = block_size
         if maximum_block_size == 'auto':
             # Get device limits
-            import pycuda.driver as cuda
-            # noinspection PyUnresolvedReferences
-            import pycuda.autoinit  # NOQA
-            da = cuda.device_attribute
-            device = cuda.Context.get_device()
-            maximum_block_size = tuple(device.get_attribute(a)
-                                       for a in (da.MAX_BLOCK_DIM_X, da.MAX_BLOCK_DIM_Y, da.MAX_BLOCK_DIM_Z))
+            import cupy as cp
+            device = cp.cuda.Device(pystencils.GPU_DEVICE)
+            da = device.attributes
+            maximum_block_size = tuple(da[f"MaxBlockDim{c}"] for c in ["X", "Y", "Z"])
 
         self._maximum_block_size = maximum_block_size
         self._iterationSlice = normalize_slice(iteration_slice, field.spatial_shape)
         self._dim = field.spatial_dimensions
         self._symbolic_shape = [e if isinstance(e, sp.Basic) else None for e in field.spatial_shape]
         self._compile_time_block_size = compile_time_block_size
 
@@ -180,25 +178,22 @@
     def iteration_space(self, arr_shape):
         return _iteration_space(self._iterationSlice, arr_shape)
 
     @staticmethod
     def limit_block_size_by_register_restriction(block_size, required_registers_per_thread, device=None):
         """Shrinks the block_size if there are too many registers used per multiprocessor.
         This is not done automatically, since the required_registers_per_thread are not known before compilation.
-        They can be obtained by ``func.num_regs`` from a pycuda function.
+        They can be obtained by ``func.num_regs`` from a cupy function.
         :returns smaller block_size if too many registers are used.
         """
-        import pycuda.driver as cuda
-        # noinspection PyUnresolvedReferences
-        import pycuda.autoinit  # NOQA
-
-        da = cuda.device_attribute
-        if device is None:
-            device = cuda.Context.get_device()
-        available_registers_per_mp = device.get_attribute(da.MAX_REGISTERS_PER_MULTIPROCESSOR)
+        import cupy as cp
+        device = cp.cuda.Device(pystencils.GPU_DEVICE)
+        da = device.attributes
+
+        available_registers_per_mp = da.get("MaxRegistersPerMultiprocessor")
 
         block = block_size
 
         while True:
             num_threads = 1
             for t in block:
                 num_threads *= t
@@ -233,18 +228,18 @@
 
     def symbolic_parameters(self):
         return set(b for b in self._block_size if isinstance(b, sp.Symbol))
 
 
 class LineIndexing(AbstractIndexing):
     """
-    Indexing scheme that assigns the innermost 'line' i.e. the elements which are adjacent in memory to a 1D CUDA block.
+    Indexing scheme that assigns the innermost 'line' i.e. the elements which are adjacent in memory to a 1D GPU block.
     The fastest coordinate is indexed with thread_idx.x, the remaining coordinates are mapped to block_idx.{x,y,z}
     This indexing scheme supports up to 4 spatial dimensions, where the innermost dimensions is not larger than the
-    maximum amount of threads allowed in a CUDA block (which depends on device).
+    maximum amount of threads allowed in a GPU block (which depends on device).
     """
 
     def __init__(self, field, iteration_slice):
         available_indices = [THREAD_IDX[0]] + BLOCK_IDX
         if field.spatial_dimensions > 4:
             raise NotImplementedError("This indexing scheme supports at most 4 spatial dimensions")
```

### Comparing `pystencils-1.2/pystencils/gpucuda/kernelcreation.py` & `pystencils-1.3/pystencils/gpu/kernelcreation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from pystencils.astnodes import Block, KernelFunction, LoopOverCoordinate, SympyAssignment
 from pystencils.config import CreateKernelConfig
 from pystencils.typing import StructType, TypedSymbol
 from pystencils.typing.transformations import add_types
 from pystencils.field import Field, FieldType
 from pystencils.enums import Target, Backend
-from pystencils.gpucuda.cudajit import make_python_function
+from pystencils.gpu.cudajit import make_python_function
 from pystencils.node_collection import NodeCollection
-from pystencils.gpucuda.indexing import indexing_creator_from_params
+from pystencils.gpu.indexing import indexing_creator_from_params
 from pystencils.simp.assignment_collection import AssignmentCollection
 from pystencils.transformations import (
     get_base_buffer_index, get_common_field, parse_base_pointer_info,
     resolve_buffer_accesses, resolve_field_accesses, unify_shape_symbols)
 
 
 def create_cuda_kernel(assignments: Union[AssignmentCollection, NodeCollection],
```

### Comparing `pystencils-1.2/pystencils/gpucuda/periodicity.py` & `pystencils-1.3/pystencils/gpu/periodicity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from itertools import product
 
 from pystencils import CreateKernelConfig, create_kernel
-import pystencils.gpucuda
+from pystencils.gpu import make_python_function
 from pystencils import Assignment, Field
 from pystencils.enums import Target
 from pystencils.slicing import get_periodic_boundary_src_dst_slices, normalize_slice
 
 
 def create_copy_kernel(domain_size, from_slice, to_slice, index_dimensions=0, index_dim_shape=1, dtype=np.float64):
     """Copies a rectangular part of an array to another non-overlapping part"""
@@ -36,14 +36,14 @@
                                   thickness=None, dtype=np.float64, target=Target.GPU):
     assert target in {Target.GPU}
     src_dst_slice_tuples = get_periodic_boundary_src_dst_slices(stencil, ghost_layers, thickness)
     kernels = []
 
     for src_slice, dst_slice in src_dst_slice_tuples:
         ast = create_copy_kernel(domain_size, src_slice, dst_slice, index_dimensions, index_dim_shape, dtype)
-        kernels.append(pystencils.gpucuda.make_python_function(ast))
+        kernels.append(make_python_function(ast))
 
     def functor(pdfs, **_):
         for kernel in kernels:
             kernel(pdfs=pdfs)
 
     return functor
```

### Comparing `pystencils-1.2/pystencils/include/aesni_rand.h` & `pystencils-1.3/pystencils/include/aesni_rand.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/include/arm_neon_helpers.h` & `pystencils-1.3/pystencils/include/arm_neon_helpers.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+#if defined(_MSC_VER)
+#define __ARM_NEON
+#endif
+
 #ifdef __ARM_NEON
 #include <arm_neon.h>
 #endif
 
 #if defined(__ARM_FEATURE_SVE) && defined(__ARM_FEATURE_SVE_BITS) && __ARM_FEATURE_SVE_BITS > 0
 #include <arm_sve.h>
 
@@ -28,18 +32,21 @@
 {
     alignas(16) int data[4] = {a, b, c, d};
     return vld1q_s32(data);
 }
 #endif
 
 inline void cachelineZero(void * p) {
+#if !defined(_MSC_VER) || defined(__clang__)
 	__asm__ volatile("dc zva, %0"::"r"(p):"memory");
+#endif
 }
 
 inline size_t _cachelineSize() {
+#if !defined(_MSC_VER) || defined(__clang__)
 	// check that dc zva is permitted
 	uint64_t dczid;
 	__asm__ volatile ("mrs %0, dczid_el0" : "=r"(dczid));
 	if ((dczid & (1 << 4)) != 0) {
 		return SIZE_MAX;
 	}
 
@@ -68,14 +75,15 @@
 
 	// find the last byte that was zeroed
 	for (size_t size = 1; size < max_size; ++size) {
 		if (data[offset + size] != 0) {
 			return size;
 		}
 	}
+#endif
 	
 	// too much was zeroed
 	return SIZE_MAX;
 }
 
 inline size_t cachelineSize() {
 	static size_t size = _cachelineSize();
```

### Comparing `pystencils-1.2/pystencils/include/myintrin.h` & `pystencils-1.3/pystencils/include/myintrin.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #pragma once
 
-#if defined(__SSE2__) || defined(_MSC_VER)
+#if defined(__SSE2__) || (defined(_MSC_VER) && !defined(_M_ARM64))
 QUALIFIERS __m128 _my_cvtepu32_ps(const __m128i v)
 {
 #ifdef __AVX512VL__
     return _mm_cvtepu32_ps(v);
 #else
     __m128i v2 = _mm_srli_epi32(v, 1);
     __m128i v1 = _mm_and_si128(v, _mm_set1_epi32(1));
@@ -24,15 +24,15 @@
     R0  = _mm_unpacklo_epi64(T0, T1);
     R1  = _mm_unpackhi_epi64(T0, T1);
     R2  = _mm_unpacklo_epi64(T2, T3);
     R3  = _mm_unpackhi_epi64(T2, T3);
 }
 #endif
 
-#if defined(__SSE4_1__) || defined(_MSC_VER)
+#if defined(__SSE4_1__) || (defined(_MSC_VER) && !defined(_M_ARM64))
 #if !defined(__AVX512VL__) && defined(__GNUC__) && __GNUC__ >= 5 && !defined(__clang__)
 __attribute__((optimize("no-associative-math")))
 #endif
 QUALIFIERS __m128d _my_cvtepu64_pd(const __m128i x)
 {
 #ifdef __AVX512VL__
     return _mm_cvtepu64_pd(x);
```

### Comparing `pystencils-1.2/pystencils/include/philox_rand.h` & `pystencils-1.3/pystencils/include/philox_rand.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 #ifndef __OPENCL_VERSION__
-#if defined(__SSE2__) || defined(_MSC_VER)
+#if defined(__SSE2__) || (defined(_MSC_VER) && !defined(_M_ARM64))
 #include <emmintrin.h> // SSE2
 #endif
 #ifdef __AVX2__
 #include <immintrin.h> // AVX*
-#elif defined(__SSE4_1__) || defined(_MSC_VER)
+#elif defined(__SSE4_1__) || (defined(_MSC_VER) && !defined(_M_ARM64))
 #include <smmintrin.h>  // SSE4
 #ifdef __FMA__
 #include <immintrin.h> // FMA
 #endif
 #endif
 
+#if defined(_MSC_VER) && defined(_M_ARM64)
+#define __ARM_NEON
+#endif
+
 #ifdef __ARM_NEON
 #include <arm_neon.h>
 #endif
 #ifdef __ARM_FEATURE_SVE
 #include <arm_sve.h>
 #endif
 
@@ -179,15 +183,15 @@
     rnd2 = ctr[1] * TWOPOW32_INV_FLOAT + (TWOPOW32_INV_FLOAT/2.0f);
     rnd3 = ctr[2] * TWOPOW32_INV_FLOAT + (TWOPOW32_INV_FLOAT/2.0f);
     rnd4 = ctr[3] * TWOPOW32_INV_FLOAT + (TWOPOW32_INV_FLOAT/2.0f);
 #endif
 }
 
 #if !defined(__CUDA_ARCH__) && !defined(__OPENCL_VERSION__)
-#if defined(__SSE4_1__) || defined(_MSC_VER)
+#if defined(__SSE4_1__) || (defined(_MSC_VER) && !defined(_M_ARM64))
 QUALIFIERS void _philox4x32round(__m128i* ctr, __m128i* key)
 {
     __m128i lohi0a = _mm_mul_epu32(ctr[0], _mm_set1_epi32(PHILOX_M4x32_0));
     __m128i lohi0b = _mm_mul_epu32(_mm_srli_epi64(ctr[0], 32), _mm_set1_epi32(PHILOX_M4x32_0));
     __m128i lohi1a = _mm_mul_epu32(ctr[2], _mm_set1_epi32(PHILOX_M4x32_1));
     __m128i lohi1b = _mm_mul_epu32(_mm_srli_epi64(ctr[2], 32), _mm_set1_epi32(PHILOX_M4x32_1));
 
@@ -661,20 +665,22 @@
     uint32x4_t ctr0v = vdupq_n_u32(ctr0);
     uint32x4_t ctr2v = vdupq_n_u32(ctr2);
     uint32x4_t ctr3v = vdupq_n_u32(ctr3);
 
     philox_float4(ctr0v, ctr1, ctr2v, ctr3v, key0, key1, rnd1, rnd2, rnd3, rnd4);
 }
 
+#ifndef _MSC_VER
 QUALIFIERS void philox_float4(uint32 ctr0, int32x4_t ctr1, uint32 ctr2, uint32 ctr3,
                               uint32 key0, uint32 key1,
                               float32x4_t & rnd1, float32x4_t & rnd2, float32x4_t & rnd3, float32x4_t & rnd4)
 {
     philox_float4(ctr0, vreinterpretq_u32_s32(ctr1), ctr2, ctr3, key0, key1, rnd1, rnd2, rnd3, rnd4);
 }
+#endif
 
 QUALIFIERS void philox_double2(uint32 ctr0, uint32x4_t ctr1, uint32 ctr2, uint32 ctr3,
                                uint32 key0, uint32 key1,
                                float64x2_t & rnd1lo, float64x2_t & rnd1hi, float64x2_t & rnd2lo, float64x2_t & rnd2hi)
 {
     uint32x4_t ctr0v = vdupq_n_u32(ctr0);
     uint32x4_t ctr2v = vdupq_n_u32(ctr2);
@@ -691,21 +697,23 @@
     uint32x4_t ctr2v = vdupq_n_u32(ctr2);
     uint32x4_t ctr3v = vdupq_n_u32(ctr3);
 
     float64x2_t ignore;
     philox_double2(ctr0v, ctr1, ctr2v, ctr3v, key0, key1, rnd1, ignore, rnd2, ignore);
 }
 
+#ifndef _MSC_VER
 QUALIFIERS void philox_double2(uint32 ctr0, int32x4_t ctr1, uint32 ctr2, uint32 ctr3,
                                uint32 key0, uint32 key1,
                                float64x2_t & rnd1, float64x2_t & rnd2)
 {
     philox_double2(ctr0, vreinterpretq_u32_s32(ctr1), ctr2, ctr3, key0, key1, rnd1, rnd2);
 }
 #endif
+#endif
 
 
 #if defined(__ARM_FEATURE_SVE)
 QUALIFIERS void _philox4x32round(svuint32x4_t & ctr, svuint32x2_t & key)
 {
     svuint32_t lo0 = svmul_u32_x(svptrue_b32(), svget4_u32(ctr, 0), svdup_u32(PHILOX_M4x32_0));
     svuint32_t hi0 = svmulh_u32_x(svptrue_b32(), svget4_u32(ctr, 0), svdup_u32(PHILOX_M4x32_0));
```

### Comparing `pystencils-1.2/pystencils/include/ppc_altivec_helpers.h` & `pystencils-1.3/pystencils/include/ppc_altivec_helpers.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/integer_functions.py` & `pystencils-1.3/pystencils/integer_functions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/integer_set_analysis.py` & `pystencils-1.3/pystencils/integer_set_analysis.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/jupyter.py` & `pystencils-1.3/pystencils/jupyter.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/kernel_contrains_check.py` & `pystencils-1.3/pystencils/kernel_contrains_check.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/kernel_decorator.py` & `pystencils-1.3/pystencils/kernel_decorator.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/kernel_wrapper.py` & `pystencils-1.3/pystencils/kernel_wrapper.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/kernelcreation.py` & `pystencils-1.3/pystencils/kernelcreation.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                         # cache line boundary, it's okay. But we cannot determine that here.
                         # We don't need to disallow OpenMP collapsing because it is never applied to the inner loop.
                         raise ValueError("Blocking cannot be combined with cacheline-zeroing")
                 else:
                     raise ValueError("Invalid value for cpu_vectorize_info")
     elif config.target == Target.GPU:
         if config.backend == Backend.CUDA:
-            from pystencils.gpucuda import create_cuda_kernel
+            from pystencils.gpu import create_cuda_kernel
             ast = create_cuda_kernel(assignments, config=config)
 
     if not ast:
         raise NotImplementedError(
             f'{config.target} together with {config.backend} is not supported by `create_domain_kernel`')
 
     if config.use_auto_for_assignments:
@@ -237,15 +237,15 @@
     if config.target == Target.CPU and config.backend == Backend.C:
         from pystencils.cpu import add_openmp, create_indexed_kernel
         ast = create_indexed_kernel(assignments, config=config)
         if config.cpu_openmp:
             add_openmp(ast, num_threads=config.cpu_openmp)
     elif config.target == Target.GPU:
         if config.backend == Backend.CUDA:
-            from pystencils.gpucuda import created_indexed_cuda_kernel
+            from pystencils.gpu import created_indexed_cuda_kernel
             ast = created_indexed_cuda_kernel(assignments, config=config)
 
     if not ast:
         raise NotImplementedError(f'Indexed kernels are not yet supported for {config.target} with {config.backend}')
     return ast
```

### Comparing `pystencils-1.2/pystencils/node_collection.py` & `pystencils-1.3/pystencils/node_collection.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/placeholder_function.py` & `pystencils-1.3/pystencils/placeholder_function.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/plot.py` & `pystencils-1.3/pystencils/plot.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/rng.py` & `pystencils-1.3/pystencils/rng.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/runhelper/db.py` & `pystencils-1.3/pystencils/runhelper/db.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/runhelper/parameterstudy.py` & `pystencils-1.3/pystencils/runhelper/parameterstudy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/simp/__init__.py` & `pystencils-1.3/pystencils/simp/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/simp/assignment_collection.py` & `pystencils-1.3/pystencils/simp/assignment_collection.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/simp/simplifications.py` & `pystencils-1.3/pystencils/simp/simplifications.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/simp/simplificationstrategy.py` & `pystencils-1.3/pystencils/simp/simplificationstrategy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/simp/subexpression_insertion.py` & `pystencils-1.3/pystencils/simp/subexpression_insertion.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/simplificationfactory.py` & `pystencils-1.3/pystencils/simplificationfactory.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/slicing.py` & `pystencils-1.3/pystencils/slicing.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/spatial_coordinates.py` & `pystencils-1.3/pystencils/spatial_coordinates.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/stencil.py` & `pystencils-1.3/pystencils/stencil.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
 
     if data is None:
         data = list(range(len(stencil)))
 
     for direction, annotation in zip(stencil, data):
         assert len(direction) == 2, "Works only for 2D stencils"
         direction = tuple(int(i) for i in direction)
-        if not(direction[0] == 0 and direction[1] == 0):
+        if not (direction[0] == 0 and direction[1] == 0):
             axes.arrow(0, 0, direction[0], direction[1], head_width=0.08, head_length=head_length, color='k')
 
         if isinstance(annotation, sp.Basic):
             annotation = "$" + sp.latex(annotation) + "$"
         else:
             annotation = str(annotation)
```

### Comparing `pystencils-1.2/pystencils/sympyextensions.py` & `pystencils-1.3/pystencils/sympyextensions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/timeloop.py` & `pystencils-1.3/pystencils/timeloop.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/transformations.py` & `pystencils-1.3/pystencils/transformations.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/typing/__init__.py` & `pystencils-1.3/pystencils/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/typing/cast_functions.py` & `pystencils-1.3/pystencils/typing/cast_functions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/typing/leaf_typing.py` & `pystencils-1.3/pystencils/typing/leaf_typing.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/typing/transformations.py` & `pystencils-1.3/pystencils/typing/transformations.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/typing/typed_sympy.py` & `pystencils-1.3/pystencils/typing/typed_sympy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/typing/types.py` & `pystencils-1.3/pystencils/typing/types.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils/typing/utilities.py` & `pystencils-1.3/pystencils/typing/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -183,40 +183,35 @@
                 return create_type(default_float_type)
 
     raise NotImplementedError("Could not determine type for", expr, type(expr))
 
 
 # Fix for sympy versions from 1.9
 sympy_version = sp.__version__.split('.')
-if int(sympy_version[0]) * 100 + int(sympy_version[1]) >= 109:
+sympy_version_int = int(sympy_version[0]) * 100 + int(sympy_version[1])
+if sympy_version_int >= 109:
     # __setstate__ would bypass the contructor, so we remove it
-    sp.Number.__getstate__ = sp.Basic.__getstate__
-    del sp.Basic.__getstate__
-
-    class FunctorWithStoredKwargs:
-        def __init__(self, func, **kwargs):
-            self.func = func
-            self.kwargs = kwargs
-
-        def __call__(self, *args):
-            return self.func(*args, **self.kwargs)
+    if sympy_version_int >= 111:
+        del sp.Basic.__setstate__
+        del sp.Symbol.__setstate__
+    else:
+        sp.Number.__getstate__ = sp.Basic.__getstate__
+        del sp.Basic.__getstate__
 
     # __reduce_ex__ would strip kwargs, so we override it
     def basic_reduce_ex(self, protocol):
         if hasattr(self, '__getnewargs_ex__'):
             args, kwargs = self.__getnewargs_ex__()
         else:
             args, kwargs = self.__getnewargs__(), {}
         if hasattr(self, '__getstate__'):
             state = self.__getstate__()
         else:
             state = None
-        return FunctorWithStoredKwargs(type(self), **kwargs), args, state
-
-    sp.Number.__reduce_ex__ = sp.Basic.__reduce_ex__
+        return partial(type(self), **kwargs), args, state
     sp.Basic.__reduce_ex__ = basic_reduce_ex
 
 
 def get_next_parent_of_type(node, parent_type):
     """Returns the next parent node of given type or None, if root is reached.
 
     Traverses the AST nodes parents until a parent of given type was found.
```

### Comparing `pystencils-1.2/pystencils/utils.py` & `pystencils-1.3/pystencils/utils.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils.egg-info/PKG-INFO` & `pystencils-1.3/pystencils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystencils
-Version: 1.2
+Version: 1.3
 Summary: Speeding up stencil computations on CPUs and GPUs
 Home-page: https://i10git.cs.fau.de/pycodegen/pystencils/
 Author: Martin Bauer, Jan Hönig, Markus Holzer
 Author-email: cs10-codegen@fau.de
 License: AGPLv3
 Project-URL: Bug Tracker, https://i10git.cs.fau.de/pycodegen/pystencils/-/issues
 Project-URL: Documentation, https://pycodegen.pages.i10git.cs.fau.de/pystencils/
@@ -78,26 +78,26 @@
 ```bash
 pip install pystencils[interactive]
 ```
 
 Without `[interactive]` you get a minimal version with very little dependencies.
 
 All options:
-- `gpu`: use this if an NVIDIA GPU is available and CUDA is installed
+- `gpu`: use this if an NVIDIA or AMD GPU is available and CUDA or ROCm is installed
 - `alltrafos`: pulls in additional dependencies for loop simplification e.g. libisl
 - `bench_db`: functionality to store benchmark result in object databases
 - `interactive`: installs dependencies to work in Jupyter including image I/O, plotting etc.
 - `doc`: packages to build documentation
 
 Options can be combined e.g.
 ```bash
 pip install pystencils[interactive, gpu, doc]
 ```
 
-pystencils is also fully compatible with Windows machines. If working with visual studio and pycuda makes sure to run example files first to ensure that pycuda can find the compiler's executable.
+pystencils is also fully compatible with Windows machines. If working with visual studio and cupy makes sure to run example files first to ensure that cupy can find the compiler's executable.
 
 Documentation
 -------------
 
 Read the docs [here](https://pycodegen.pages.i10git.cs.fau.de/pystencils) and
 check out the Jupyter notebooks in `doc/notebooks`. The **Changelog** of pystencils can be found [here](https://i10git.cs.fau.de/pycodegen/pystencils/-/blob/master/CHANGELOG.md).
```

### Comparing `pystencils-1.2/pystencils.egg-info/SOURCES.txt` & `pystencils-1.3/pystencils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -114,35 +114,34 @@
 pystencils/cpu/kernelcreation.py
 pystencils/cpu/msvc_detection.py
 pystencils/cpu/vectorization.py
 pystencils/datahandling/__init__.py
 pystencils/datahandling/blockiteration.py
 pystencils/datahandling/datahandling_interface.py
 pystencils/datahandling/parallel_datahandling.py
-pystencils/datahandling/pycuda.py
 pystencils/datahandling/serial_datahandling.py
 pystencils/datahandling/vtk.py
 pystencils/fd/__init__.py
 pystencils/fd/derivation.py
 pystencils/fd/derivative.py
 pystencils/fd/finitedifferences.py
 pystencils/fd/finitevolumes.py
 pystencils/fd/spatial.py
-pystencils/gpucuda/__init__.py
-pystencils/gpucuda/cudajit.py
-pystencils/gpucuda/indexing.py
-pystencils/gpucuda/kernelcreation.py
-pystencils/gpucuda/periodicity.py
+pystencils/gpu/__init__.py
+pystencils/gpu/cudajit.py
+pystencils/gpu/gpu_array_handler.py
+pystencils/gpu/indexing.py
+pystencils/gpu/kernelcreation.py
+pystencils/gpu/periodicity.py
 pystencils/include/PyStencilsField.h
 pystencils/include/__init__.py
 pystencils/include/aesni_rand.h
 pystencils/include/arm_neon_helpers.h
-pystencils/include/cuda_complex.hpp
+pystencils/include/gpu_defines.h
 pystencils/include/myintrin.h
-pystencils/include/opencl_stdint.h
 pystencils/include/philox_rand.h
 pystencils/include/ppc_altivec_helpers.h
 pystencils/runhelper/__init__.py
 pystencils/runhelper/db.py
 pystencils/runhelper/parameterstudy.py
 pystencils/simp/__init__.py
 pystencils/simp/assignment_collection.py
@@ -172,15 +171,14 @@
 pystencils_tests/test_boundary_indexlist_creation.py
 pystencils_tests/test_buffer.py
 pystencils_tests/test_buffer_gpu.py
 pystencils_tests/test_conditional_field_access.py
 pystencils_tests/test_conditional_vec.py
 pystencils_tests/test_config.py
 pystencils_tests/test_create_kernel_config.py
-pystencils_tests/test_cudagpu.py
 pystencils_tests/test_custom_backends.py
 pystencils_tests/test_datahandling.py
 pystencils_tests/test_datahandling_parallel.py
 pystencils_tests/test_derivative.py
 pystencils_tests/test_dot_printer.ipynb
 pystencils_tests/test_dot_printer.py
 pystencils_tests/test_dtype_check.py
@@ -191,14 +189,15 @@
 pystencils_tests/test_field.py
 pystencils_tests/test_field_access_poly.py
 pystencils_tests/test_field_equality.ipynb
 pystencils_tests/test_finite_differences.py
 pystencils_tests/test_floor_ceil_int_optimization.py
 pystencils_tests/test_fvm.py
 pystencils_tests/test_global_definitions.py
+pystencils_tests/test_gpu.py
 pystencils_tests/test_helpful_errors.py
 pystencils_tests/test_indexed_kernels.py
 pystencils_tests/test_jacobi_cbackend.py
 pystencils_tests/test_json_backend.py
 pystencils_tests/test_jupyter_extensions.ipynb
 pystencils_tests/test_logarithm.py
 pystencils_tests/test_loop_cutting.py
```

### Comparing `pystencils-1.2/pystencils_tests/test_Min_Max.py` & `pystencils-1.3/pystencils_tests/test_Min_Max.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_abs.py` & `pystencils-1.3/pystencils_tests/test_abs.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_address_of.py` & `pystencils-1.3/pystencils_tests/test_address_of.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_aligned_array.py` & `pystencils-1.3/pystencils_tests/test_aligned_array.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_assignment_collection.py` & `pystencils-1.3/pystencils_tests/test_assignment_collection.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_assignment_collection_dict_conversion.py` & `pystencils-1.3/pystencils_tests/test_assignment_collection_dict_conversion.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_assignment_from_stencil.py` & `pystencils-1.3/pystencils_tests/test_assignment_from_stencil.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_astnodes.py` & `pystencils-1.3/pystencils_tests/test_astnodes.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_bit_masks.py` & `pystencils-1.3/pystencils_tests/test_bit_masks.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_blocking.py` & `pystencils-1.3/pystencils_tests/test_blocking.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_blocking_staggered.py` & `pystencils-1.3/pystencils_tests/test_blocking_staggered.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_boundary.py` & `pystencils-1.3/pystencils_tests/test_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         boundaries = list(boundary_handling._boundary_object_to_boundary_info.keys()) + ['domain']
         boundary_handling.geometry_to_vtk(file_name=os.path.join(tmp_dir, 'test_output3'),
                                           boundaries=boundaries[0], ghost_layers=False)
 
 
 def test_boundary_gpu():
-    pytest.importorskip('pycuda')
+    pytest.importorskip('cupy')
     dh = SerialDataHandling(domain_size=(7, 7), default_target=Target.GPU)
     src = dh.add_array('src')
     dh.fill("src", 0.0, ghost_layers=True)
     dh.fill("src", 1.0, ghost_layers=False)
     src_cpu = dh.add_array('src_cpu', gpu=False)
     dh.fill("src_cpu", 0.0, ghost_layers=True)
     dh.fill("src_cpu", 1.0, ghost_layers=False)
```

### Comparing `pystencils-1.2/pystencils_tests/test_boundary_indexlist_creation.py` & `pystencils-1.3/pystencils_tests/test_boundary_indexlist_creation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_buffer.py` & `pystencils-1.3/pystencils_tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_buffer_gpu.py` & `pystencils-1.3/pystencils_tests/test_buffer_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,43 +10,42 @@
 from pystencils.field import create_numpy_array_with_layout, layout_string_to_tuple
 from pystencils.slicing import (
     add_ghost_layers, get_ghost_region_slice, get_slice_before_ghost_layer)
 from pystencils.stencil import direction_string_to_offset
 
 try:
     # noinspection PyUnresolvedReferences
-    import pycuda.autoinit
-    import pycuda.gpuarray as gpuarray
+    import cupy as cp
 except ImportError:
     pass
 
 
 FIELD_SIZES = [(4, 3), (9, 3, 7)]
 
 
 def _generate_fields(dt=np.uint8, stencil_directions=1, layout='numpy'):
-    pytest.importorskip('pycuda')
+    pytest.importorskip('cupy')
     field_sizes = FIELD_SIZES
     if stencil_directions > 1:
         field_sizes = [s + (stencil_directions,) for s in field_sizes]
 
     fields = []
     for size in field_sizes:
         field_layout = layout_string_to_tuple(layout, len(size))
         src_arr = create_numpy_array_with_layout(size, field_layout).astype(dt)
 
         array_data = np.reshape(np.arange(1, int(np.prod(size)+1)), size)
         # Use flat iterator to input data into the array
         src_arr.flat = add_ghost_layers(array_data,
                                         index_dimensions=1 if stencil_directions > 1 else 0).astype(dt).flat
 
-        gpu_src_arr = gpuarray.to_gpu(src_arr)
-        gpu_dst_arr = gpuarray.empty_like(gpu_src_arr)
+        gpu_src_arr = cp.asarray(src_arr)
+        gpu_dst_arr = cp.zeros_like(gpu_src_arr)
         size = int(np.prod(src_arr.shape))
-        gpu_buffer_arr = gpuarray.zeros(size, dtype=dt)
+        gpu_buffer_arr = cp.zeros(size, dtype=dt)
 
         fields.append((src_arr, gpu_src_arr, gpu_dst_arr, gpu_buffer_arr))
     return fields
 
 
 def test_full_scalar_field():
     """Tests fully (un)packing a scalar field (from)to a GPU buffer."""
@@ -159,15 +158,15 @@
 
         dst_arr = gpu_dst_arr.get()
 
         np.testing.assert_equal(src_arr, dst_arr)
 
 
 def test_subset_cell_values():
-    """Tests (un)packing a subset of cell values of the a field (from)to a buffer."""
+    """Tests (un)packing a subset of cell values of a field (from)to a buffer."""
     num_cell_values = 7
     # Cell indices of the field to be (un)packed (from)to the buffer
     cell_indices = [1, 3, 5, 6]
     fields = _generate_fields(stencil_directions=num_cell_values)
     for (src_arr, gpu_src_arr, gpu_dst_arr, gpu_buffer_arr) in fields:
         src_field = Field.create_from_numpy_array("src_field", gpu_src_arr, index_dimensions=1)
         dst_field = Field.create_from_numpy_array("dst_field", gpu_src_arr, index_dimensions=1)
@@ -296,15 +295,15 @@
         dim = src_field.spatial_dimensions
 
         #   Pack only the leftmost slice, only every second cell
         pack_slice = (slice(None, None, 2),) * (dim - 1) + (0,)
 
         #   Fill the entire array with data
         src_arr[(slice(None, None, 1),) * dim] = np.arange(num_cell_values)
-        gpu_src_arr[(slice(None, None, 1),) * dim] = src_arr
+        gpu_src_arr.set(src_arr)
         gpu_dst_arr.fill(0)
 
         config = CreateKernelConfig(target=Target.GPU, iteration_slice=pack_slice,
                                     data_type={'src_field': gpu_src_arr.dtype, 'buffer': gpu_buffer_arr.dtype})
 
         pack_code = create_kernel(pack_eqs, config=config)
         pack_kernel = pack_code.compile()
```

### Comparing `pystencils-1.2/pystencils_tests/test_conditional_field_access.py` & `pystencils-1.3/pystencils_tests/test_conditional_field_access.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_conditional_vec.py` & `pystencils-1.3/pystencils_tests/test_conditional_vec.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_config.py` & `pystencils-1.3/pystencils_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_create_kernel_config.py` & `pystencils-1.3/pystencils_tests/test_create_kernel_config.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_cudagpu.py` & `pystencils-1.3/pystencils_tests/test_gpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
-import pycuda.autoinit
-import pycuda.gpuarray as gpuarray
+import cupy as cp
 import sympy as sp
 from scipy.ndimage import convolve
 
 from pystencils import Assignment, Field, fields, CreateKernelConfig, create_kernel, Target
-from pystencils.gpucuda import BlockIndexing
+from pystencils.gpu import BlockIndexing
 from pystencils.simp import sympy_cse_on_assignment_list
 from pystencils.slicing import add_ghost_layers, make_slice, remove_ghost_layers
 
 
 def test_averaging_kernel():
     size = (40, 55)
     src_arr = np.random.rand(*size)
@@ -21,18 +20,18 @@
     update_rule = Assignment(dst_field[0, 0],
                              (src_field[0, 1] + src_field[0, -1] + src_field[1, 0] + src_field[-1, 0]) / 4)
 
     config = CreateKernelConfig(target=Target.GPU)
     ast = create_kernel(sympy_cse_on_assignment_list([update_rule]), config=config)
     kernel = ast.compile()
 
-    gpu_src_arr = gpuarray.to_gpu(src_arr)
-    gpu_dst_arr = gpuarray.to_gpu(dst_arr)
+    gpu_src_arr = cp.asarray(src_arr)
+    gpu_dst_arr = cp.asarray(dst_arr)
     kernel(src=gpu_src_arr, dst=gpu_dst_arr)
-    gpu_dst_arr.get(dst_arr)
+    dst_arr = gpu_dst_arr.get()
 
     stencil = np.array([[0, 1, 0], [1, 0, 1], [0, 1, 0]]) / 4.0
     reference = convolve(remove_ghost_layers(src_arr), stencil, mode='constant', cval=0.0)
     reference = add_ghost_layers(reference)
     np.testing.assert_almost_equal(reference, dst_arr)
 
 
@@ -48,18 +47,18 @@
     kernel = ast.compile()
 
     size = (3, 3)
     src_arr = np.random.rand(*size)
     src_arr = add_ghost_layers(src_arr)
     dst_arr = np.zeros_like(src_arr)
 
-    gpu_src_arr = gpuarray.to_gpu(src_arr)
-    gpu_dst_arr = gpuarray.to_gpu(dst_arr)
+    gpu_src_arr = cp.asarray(src_arr)
+    gpu_dst_arr = cp.asarray(dst_arr)
     kernel(src=gpu_src_arr, dst=gpu_dst_arr)
-    gpu_dst_arr.get(dst_arr)
+    dst_arr = gpu_dst_arr.get()
 
     stencil = np.array([[0, 1, 0], [1, 0, 1], [0, 1, 0]]) / 4.0
     reference = convolve(remove_ghost_layers(src_arr), stencil, mode='constant', cval=0.0)
     reference = add_ghost_layers(reference)
     np.testing.assert_almost_equal(reference, dst_arr)
 
 
@@ -77,18 +76,18 @@
     update_rule = Assignment(dst_field[0, 0],
                              sum([src_field[offset[0], offset[1]](i) for i in range(src_size[-1])]))
 
     config = CreateKernelConfig(target=Target.GPU)
     ast = create_kernel([update_rule], config=config)
     kernel = ast.compile()
 
-    gpu_src_arr = gpuarray.to_gpu(src_arr)
-    gpu_dst_arr = gpuarray.to_gpu(dst_arr)
+    gpu_src_arr = cp.asarray(src_arr)
+    gpu_dst_arr = cp.asarray(dst_arr)
     kernel(src=gpu_src_arr, dst=gpu_dst_arr)
-    gpu_dst_arr.get(dst_arr)
+    dst_arr = gpu_dst_arr.get()
 
     reference = np.zeros_like(dst_arr)
     gl = np.max(np.abs(np.array(offset, dtype=int)))
     for x in range(gl, src_size[0]-gl):
         for y in range(gl, src_size[1]-gl):
             reference[x, y] = sum([src_arr[x+offset[0], y+offset[1], i] for i in range(src_size[2])])
 
@@ -105,57 +104,56 @@
     update_rule = Assignment(dst_field[0, 0], src_field[0, 0])
     ghost_layers = [(1, 2), (2, 1)]
 
     config = CreateKernelConfig(target=Target.GPU, ghost_layers=ghost_layers, gpu_indexing="line")
     ast = create_kernel(sympy_cse_on_assignment_list([update_rule]), config=config)
     kernel = ast.compile()
 
-    gpu_src_arr = gpuarray.to_gpu(src_arr)
-    gpu_dst_arr = gpuarray.to_gpu(dst_arr)
+    gpu_src_arr = cp.asarray(src_arr)
+    gpu_dst_arr = cp.asarray(dst_arr)
     kernel(src=gpu_src_arr, dst=gpu_dst_arr)
-    gpu_dst_arr.get(dst_arr)
+    dst_arr = gpu_dst_arr.get()
 
     reference = np.zeros_like(src_arr)
     reference[ghost_layers[0][0]:-ghost_layers[0][1], ghost_layers[1][0]:-ghost_layers[1][1]] = 1
     np.testing.assert_equal(reference, dst_arr)
 
 
 def test_setting_value():
     arr_cpu = np.arange(25, dtype=np.float64).reshape(5, 5)
-    arr_gpu = gpuarray.to_gpu(arr_cpu)
+    arr_gpu = cp.asarray(arr_cpu)
 
     iteration_slice = make_slice[:, :]
     f = Field.create_generic("f", 2)
     update_rule = [Assignment(f(0), sp.Symbol("value"))]
 
     config = CreateKernelConfig(target=Target.GPU, gpu_indexing="line", iteration_slice=iteration_slice)
     ast = create_kernel(sympy_cse_on_assignment_list(update_rule), config=config)
     kernel = ast.compile()
 
     kernel(f=arr_gpu, value=np.float64(42.0))
     np.testing.assert_equal(arr_gpu.get(), np.ones((5, 5)) * 42.0)
 
 
 def test_periodicity():
-    from pystencils.gpucuda.periodicity import get_periodic_boundary_functor as periodic_gpu
+    from pystencils.gpu.periodicity import get_periodic_boundary_functor as periodic_gpu
     from pystencils.slicing import get_periodic_boundary_functor as periodic_cpu
 
     arr_cpu = np.arange(50, dtype=np.float64).reshape(5, 5, 2)
-    arr_gpu = gpuarray.to_gpu(arr_cpu)
+    arr_gpu = cp.asarray(arr_cpu)
 
     periodicity_stencil = [(1, 0), (-1, 0), (1, 1)]
     periodic_gpu_kernel = periodic_gpu(periodicity_stencil, (5, 5), 1, 2)
     periodic_cpu_kernel = periodic_cpu(periodicity_stencil)
 
     cpu_result = np.copy(arr_cpu)
     periodic_cpu_kernel(cpu_result)
 
-    gpu_result = np.copy(arr_cpu)
     periodic_gpu_kernel(pdfs=arr_gpu)
-    arr_gpu.get(gpu_result)
+    gpu_result = arr_gpu.get()
     np.testing.assert_equal(cpu_result, gpu_result)
 
 
 def test_block_indexing():
     f = fields("f: [3D]")
     bi = BlockIndexing(f, make_slice[:, :, :], block_size=(16, 8, 2), permute_block_size_dependent_on_layout=False)
     assert bi.call_parameters((3, 2, 32))['block'] == (3, 2, 32)
```

### Comparing `pystencils-1.2/pystencils_tests/test_custom_backends.py` & `pystencils-1.3/pystencils_tests/test_custom_backends.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     ast = pystencils.create_kernel(normal_assignments, target=Target.CPU)
     pystencils.show_code(ast, ScreamingBackend())
     with pytest.raises(CalledProcessError):
         pystencils.cpu.cpujit.make_python_function(ast, custom_backend=ScreamingBackend())
 
 
 def test_custom_backends_gpu():
-    pytest.importorskip('pycuda')
-    import pycuda.driver
-    import pystencils.gpucuda.cudajit
+    pytest.importorskip('cupy')
+    import cupy
+    import pystencils.gpu.cudajit
 
     z, x, y = pystencils.fields("z, y, x: [2d]")
 
     normal_assignments = pystencils.AssignmentCollection([pystencils.Assignment(
         z[0, 0], x[0, 0] * x[0, 0] * y[0, 0])], [])
 
     ast = pystencils.create_kernel(normal_assignments, target=Target.GPU)
     pystencils.show_code(ast, ScreamingGpuBackend())
-    with pytest.raises(pycuda.driver.CompileError):
-        pystencils.gpucuda.cudajit.make_python_function(ast, custom_backend=ScreamingGpuBackend())
+    with pytest.raises(cupy.cuda.compiler.JitifyException):
+        pystencils.gpu.cudajit.make_python_function(ast, custom_backend=ScreamingGpuBackend())
```

### Comparing `pystencils-1.2/pystencils_tests/test_data/lenna.png` & `pystencils-1.3/pystencils_tests/test_data/lenna.png`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_data/test_vessel2d_mask.png` & `pystencils-1.3/pystencils_tests/test_data/test_vessel2d_mask.png`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_datahandling.py` & `pystencils-1.3/pystencils_tests/test_datahandling.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tempfile import TemporaryDirectory
 from pathlib import Path
 
 import numpy as np
 
 import pystencils as ps
 from pystencils import create_data_handling, create_kernel
-from pystencils.datahandling.pycuda import PyCudaArrayHandler
+from pystencils.gpu.gpu_array_handler import GPUArrayHandler
 from pystencils.enums import Target
 
 try:
     import pytest
 except ImportError:
     import unittest.mock
     pytest = unittest.mock.MagicMock()
@@ -81,19 +81,15 @@
                     assert len(domain_size) == 2
                     assert full_arr[x, y] == x + y
 
 
 def synchronization(dh, test_gpu=False):
     field_name = 'comm_field_test'
     if test_gpu:
-        try:
-            from pycuda import driver
-            import pycuda.autoinit
-        except ImportError:
-            return
+        pytest.importorskip("cupy")
         field_name += 'Gpu'
 
     dh.add_array(field_name, ghost_layers=1, dtype=np.int8, cpu=True, gpu=test_gpu)
 
     # initialize everything with 1
     for b in dh.iterate(ghost_layers=1):
         b[field_name].fill(1)
@@ -211,26 +207,26 @@
     for domain_shape in [(4, 5), (3, 4, 5)]:
         dh = create_data_handling(domain_size=domain_shape, periodicity=True)
         assert all(dh.periodicity)
         kernel_execution_jacobi(dh, Target.CPU)
         reduction(dh)
 
         try:
-            import pycuda
+            import cupy
             dh = create_data_handling(domain_size=domain_shape, periodicity=True)
             kernel_execution_jacobi(dh, Target.GPU)
         except ImportError:
             pass
 
 
 @pytest.mark.parametrize('target', (Target.CPU, Target.GPU))
 def test_kernel_param(target):
     for domain_shape in [(4, 5), (3, 4, 5)]:
         if target == Target.GPU:
-            pytest.importorskip('pycuda')
+            pytest.importorskip('cupy')
 
         dh = create_data_handling(domain_size=domain_shape, periodicity=True, default_target=target)
         kernel_execution_jacobi(dh, target)
         reduction(dh)
 
 
 def test_vtk_output():
@@ -251,51 +247,63 @@
 
     assert x_ == x
     assert y_ == y
     assert x == dh.fields['x']
     assert y == dh.fields['y']
 
 
+@pytest.mark.parametrize('shape', [(17, 12), (7, 11, 18)])
+@pytest.mark.parametrize('layout', ['zyxf', 'fzyx'])
+def test_add_arrays_with_layout(shape, layout):
+    pytest.importorskip('cupy')
+
+    dh = create_data_handling(domain_size=shape, default_layout=layout, default_target=ps.Target.GPU)
+    f1 = dh.add_array("f1", values_per_cell=19)
+    dh.fill(f1.name, 1.0)
+
+    assert dh.cpu_arrays[f1.name].shape == dh.gpu_arrays[f1.name].shape
+    assert dh.cpu_arrays[f1.name].strides == dh.gpu_arrays[f1.name].strides
+    assert dh.cpu_arrays[f1.name].dtype == dh.gpu_arrays[f1.name].dtype
+
+
 def test_get_kwarg():
     domain_shape = (10, 10)
     field_description = 'src, dst'
 
     dh = create_data_handling(domain_size=domain_shape, default_ghost_layers=1)
     src, dst = dh.add_arrays(field_description)
     dh.fill("src", 1.0, ghost_layers=True)
     dh.fill("dst", 0.0, ghost_layers=True)
 
     with pytest.raises(ValueError):
-        dh.add_array('src')
+        dh.add_array('src', values_per_cell=1)
 
     ur = ps.Assignment(src.center, dst.center)
     kernel = ps.create_kernel(ur).compile()
 
     kw = dh.get_kernel_kwargs(kernel)
     assert np.all(kw[0]['src'] == dh.cpu_arrays['src'])
     assert np.all(kw[0]['dst'] == dh.cpu_arrays['dst'])
 
 
 def test_add_custom_data():
-    pytest.importorskip('pycuda')
-
-    import pycuda.gpuarray as gpuarray
-    import pycuda.autoinit  # noqa
+    pytest.importorskip('cupy')
+    import cupy as cp
 
     def cpu_data_create_func():
         return np.ones((2, 2), dtype=np.float64)
 
     def gpu_data_create_func():
-        return gpuarray.zeros((2, 2), dtype=np.float64)
+        return cp.zeros((2, 2), dtype=np.float64)
 
     def cpu_to_gpu_transfer_func(gpuarr, cpuarray):
         gpuarr.set(cpuarray)
 
     def gpu_to_cpu_transfer_func(gpuarr, cpuarray):
-        gpuarr.get(cpuarray)
+        cpuarray[:] = gpuarr.get()
 
     dh = create_data_handling(domain_size=(10, 10))
     dh.add_custom_data('custom_data',
                        cpu_data_create_func,
                        gpu_data_create_func,
                        cpu_to_gpu_transfer_func,
                        gpu_to_cpu_transfer_func)
@@ -355,27 +363,42 @@
     assert np.all(dh.cpu_arrays['src']) == 0
     assert np.all(dh.cpu_arrays['dst']) == 0
     assert np.all(dh.cpu_arrays['dst2']) == 0
 
 
 def test_array_handler():
     size = (2, 2)
-    pytest.importorskip('pycuda')
-    array_handler = PyCudaArrayHandler()
+    pytest.importorskip('cupy')
+    array_handler = GPUArrayHandler()
 
     zero_array = array_handler.zeros(size)
     cpu_array = np.empty(size)
     array_handler.download(zero_array, cpu_array)
     assert np.all(cpu_array) == 0
 
     ones_array = array_handler.ones(size)
     cpu_array = np.empty(size)
     array_handler.download(ones_array, cpu_array)
     assert np.all(cpu_array) == 1
 
     empty = array_handler.empty(size)
     assert empty.strides == (16, 8)
-    empty = array_handler.empty(shape=size, layout=(1, 0))
+    empty = array_handler.empty(shape=size, order="F")
     assert empty.strides == (8, 16)
 
     random_array = array_handler.randn(size)
 
+    cpu_array = np.empty((20, 40), dtype=np.float64)
+    gpu_array = array_handler.to_gpu(cpu_array)
+
+    assert cpu_array.base is None
+    assert gpu_array.base is None
+    assert gpu_array.strides == cpu_array.strides
+
+    cpu_array2 = np.empty((20, 40), dtype=np.float64)
+    cpu_array2 = cpu_array2.swapaxes(0, 1)
+    gpu_array2 = array_handler.to_gpu(cpu_array2)
+
+    assert cpu_array2.base is not None
+    assert gpu_array2.base is not None
+    assert gpu_array2.strides == cpu_array2.strides
+
```

### Comparing `pystencils-1.2/pystencils_tests/test_datahandling_parallel.py` & `pystencils-1.3/pystencils_tests/test_datahandling_parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     num_blocks = (3, 2, 1)
     cells = tuple(a * b for a, b in zip(block_size, num_blocks))
     blocks = wlb.createUniformBlockGrid(blocks=num_blocks, cellsPerBlock=block_size, oneBlockPerProcess=False,
                                         periodic=(1, 1, 1))
     dh = ParallelDataHandling(blocks, default_ghost_layers=2)
     access_and_gather(dh, cells)
     synchronization(dh, test_gpu=False)
-    if hasattr(wlb, 'cuda'):
+    if hasattr(wlb, 'gpu'):
         synchronization(dh, test_gpu=True)
 
 
 def test_gpu():
-    pytest.importorskip('waLBerla.cuda')
+    pytest.importorskip('waLBerla.gpu')
 
     block_size = (4, 7, 1)
     num_blocks = (3, 2, 1)
     blocks = wlb.createUniformBlockGrid(blocks=num_blocks, cellsPerBlock=block_size, oneBlockPerProcess=False)
     dh = ParallelDataHandling(blocks, default_ghost_layers=2)
     dh.add_array('v', values_per_cell=3, dtype=np.int64, ghost_layers=2, gpu=True)
 
@@ -55,15 +55,15 @@
     for b in dh.iterate():
         np.testing.assert_equal(b['v'], 42)
 
 
 @pytest.mark.parametrize('target', (pystencils.Target.CPU, pystencils.Target.GPU))
 def test_kernel(target):
     if target == pystencils.Target.GPU:
-        pytest.importorskip('waLBerla.cuda')
+        pytest.importorskip('waLBerla.gpu')
 
     # 3D
     blocks = wlb.createUniformBlockGrid(blocks=(3, 2, 4), cellsPerBlock=(3, 2, 5), oneBlockPerProcess=False)
     dh = ParallelDataHandling(blocks, default_target=target)
     kernel_execution_jacobi(dh, target)
     reduction(dh)
 
@@ -104,15 +104,15 @@
     for b in dh.iterate():
         s += np.sum(b['v'])
 
     assert s == 40*40*40 - 20*20*20
 
 
 def test_getter_setter():
-    pytest.importorskip('waLBerla.cuda')
+    pytest.importorskip('waLBerla.gpu')
 
     block_size = (2, 2, 2)
     num_blocks = (2, 2, 2)
     blocks = wlb.createUniformBlockGrid(blocks=num_blocks, cellsPerBlock=block_size, oneBlockPerProcess=False)
     dh = ParallelDataHandling(blocks, default_ghost_layers=2, default_target=pystencils.Target.GPU)
     dh.add_array('v', values_per_cell=1, dtype=np.int64, ghost_layers=2, gpu=True)
 
@@ -127,15 +127,15 @@
 
     dh.to_gpu('v')
     assert dh.is_on_gpu('v') is True
     dh.all_to_cpu()
 
 
 def test_parallel_datahandling_boundary_conditions():
-    pytest.importorskip('waLBerla.cuda')
+    pytest.importorskip('waLBerla.gpu')
 
     dh = create_data_handling(domain_size=(7, 7), periodicity=True, parallel=True,
                               default_target=pystencils.Target.GPU)
 
     src = dh.add_array('src', values_per_cell=1)
     dh.fill(src.name, 0.0, ghost_layers=True)
     dh.fill(src.name, 1.0, ghost_layers=False)
```

### Comparing `pystencils-1.2/pystencils_tests/test_derivative.py` & `pystencils-1.3/pystencils_tests/test_derivative.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_dot_printer.ipynb` & `pystencils-1.3/pystencils_tests/test_dot_printer.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_dtype_check.py` & `pystencils-1.3/pystencils_tests/test_dtype_check.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_fast_approximation.py` & `pystencils-1.3/pystencils_tests/test_fast_approximation.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pystencils as ps
 from pystencils.fast_approximation import (
     fast_division, fast_inv_sqrt, fast_sqrt, insert_fast_divisions, insert_fast_sqrts)
 
 
 def test_fast_sqrt():
-    pytest.importorskip('pycuda')
+    pytest.importorskip('cupy')
     f, g = ps.fields("f, g: double[2D]")
     expr = sp.sqrt(f[0, 0] + f[1, 0])
 
     assert len(insert_fast_sqrts(expr).atoms(fast_sqrt)) == 1
     assert len(insert_fast_sqrts([expr])[0].atoms(fast_sqrt)) == 1
     ast_gpu = ps.create_kernel(ps.Assignment(g[0, 0], insert_fast_sqrts(expr)), target=ps.Target.GPU)
     ast_gpu.compile()
@@ -26,15 +26,15 @@
     ast_gpu = ps.create_kernel(insert_fast_sqrts(ac), target=ps.Target.GPU)
     ast_gpu.compile()
     code_str = ps.get_code_str(ast_gpu)
     assert '__frsqrt_rn' in code_str
 
 
 def test_fast_divisions():
-    pytest.importorskip('pycuda')
+    pytest.importorskip('cupy')
     f, g = ps.fields("f, g: double[2D]")
     expr = f[0, 0] / f[1, 0]
     assert len(insert_fast_divisions(expr).atoms(fast_division)) == 1
 
     expr = 1 / f[0, 0] * 2 / f[0, 1]
     assert len(insert_fast_divisions(expr).atoms(fast_division)) == 1
```

### Comparing `pystencils-1.2/pystencils_tests/test_fd_derivation.ipynb` & `pystencils-1.3/pystencils_tests/test_fd_derivation.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_fd_derivation_via_rotation.ipynb` & `pystencils-1.3/pystencils_tests/test_fd_derivation_via_rotation.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_fd_derivative.py` & `pystencils-1.3/pystencils_tests/test_fd_derivative.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_field.py` & `pystencils-1.3/pystencils_tests/test_field.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_field_access_poly.py` & `pystencils-1.3/pystencils_tests/test_field_access_poly.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_field_equality.ipynb` & `pystencils-1.3/pystencils_tests/test_field_equality.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_finite_differences.py` & `pystencils-1.3/pystencils_tests/test_finite_differences.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_floor_ceil_int_optimization.py` & `pystencils-1.3/pystencils_tests/test_floor_ceil_int_optimization.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_fvm.py` & `pystencils-1.3/pystencils_tests/test_fvm.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_global_definitions.py` & `pystencils-1.3/pystencils_tests/test_global_definitions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_helpful_errors.py` & `pystencils-1.3/pystencils_tests/test_helpful_errors.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_indexed_kernels.py` & `pystencils-1.3/pystencils_tests/test_indexed_kernels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import numpy as np
+import pytest
+
 import pystencils as ps
 from pystencils import Assignment, Field, CreateKernelConfig, create_kernel, Target
 
 
 def test_indexed_kernel():
     arr = np.zeros((3, 4))
     dtype = np.dtype([('x', int), ('y', int), ('value', arr.dtype)])
@@ -20,39 +22,33 @@
     kernel = ast.compile()
     kernel(f=arr, index=index_arr)
     code = ps.get_code_str(kernel)
     for i in range(index_arr.shape[0]):
         np.testing.assert_allclose(arr[index_arr[i]['x'], index_arr[i]['y']], index_arr[i]['value'], atol=1e-13)
 
 
-def test_indexed_cuda_kernel():
-    try:
-        import pycuda
-    except ImportError:
-        pycuda = None
-
-    if pycuda:
-        import pycuda.gpuarray as gpuarray
-
-        arr = np.zeros((3, 4))
-        dtype = np.dtype([('x', int), ('y', int), ('value', arr.dtype)])
-        index_arr = np.zeros((3,), dtype=dtype)
-        index_arr[0] = (0, 2, 3.0)
-        index_arr[1] = (1, 3, 42.0)
-        index_arr[2] = (2, 1, 5.0)
-
-        indexed_field = Field.create_from_numpy_array('index', index_arr)
-        normal_field = Field.create_from_numpy_array('f', arr)
-        update_rule = Assignment(normal_field[0, 0], indexed_field('value'))
-
-        config = CreateKernelConfig(target=Target.GPU, index_fields=[indexed_field])
-        ast = create_kernel([update_rule], config=config)
-        kernel = ast.compile()
-
-        gpu_arr = gpuarray.to_gpu(arr)
-        gpu_index_arr = gpuarray.to_gpu(index_arr)
-        kernel(f=gpu_arr, index=gpu_index_arr)
-        gpu_arr.get(arr)
-        for i in range(index_arr.shape[0]):
-            np.testing.assert_allclose(arr[index_arr[i]['x'], index_arr[i]['y']], index_arr[i]['value'], atol=1e-13)
-    else:
-        print("Did not run test on GPU since no pycuda is available")
+def test_indexed_gpu_kernel():
+    pytest.importorskip("cupy")
+    import cupy as cp
+
+    arr = np.zeros((3, 4))
+    dtype = np.dtype([('x', int), ('y', int), ('value', arr.dtype)])
+    index_arr = np.zeros((3,), dtype=dtype)
+    index_arr[0] = (0, 2, 3.0)
+    index_arr[1] = (1, 3, 42.0)
+    index_arr[2] = (2, 1, 5.0)
+
+    indexed_field = Field.create_from_numpy_array('index', index_arr)
+    normal_field = Field.create_from_numpy_array('f', arr)
+    update_rule = Assignment(normal_field[0, 0], indexed_field('value'))
+
+    config = CreateKernelConfig(target=Target.GPU, index_fields=[indexed_field])
+    ast = create_kernel([update_rule], config=config)
+    kernel = ast.compile()
+
+    gpu_arr = cp.asarray(arr)
+    gpu_index_arr = cp.ndarray(index_arr.shape, dtype=index_arr.dtype)
+    gpu_index_arr.set(index_arr)
+    kernel(f=gpu_arr, index=gpu_index_arr)
+    arr = gpu_arr.get()
+    for i in range(index_arr.shape[0]):
+        np.testing.assert_allclose(arr[index_arr[i]['x'], index_arr[i]['y']], index_arr[i]['value'], atol=1e-13)
```

### Comparing `pystencils-1.2/pystencils_tests/test_jacobi_cbackend.py` & `pystencils-1.3/pystencils_tests/test_jacobi_cbackend.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_json_backend.py` & `pystencils-1.3/pystencils_tests/test_json_backend.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_jupyter_extensions.ipynb` & `pystencils-1.3/pystencils_tests/test_jupyter_extensions.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_logarithm.py` & `pystencils-1.3/pystencils_tests/test_logarithm.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_loop_cutting.py` & `pystencils-1.3/pystencils_tests/test_loop_cutting.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_match_subs_for_assignment_collection.py` & `pystencils-1.3/pystencils_tests/test_match_subs_for_assignment_collection.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_math_functions.py` & `pystencils-1.3/pystencils_tests/test_math_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 @pytest.mark.parametrize('dtype', ["float64", "float32"])
 @pytest.mark.parametrize('func', [sp.Pow, sp.atan2])
 @pytest.mark.parametrize('target', [ps.Target.CPU, ps.Target.GPU])
 def test_two_arguments(dtype, func, target):
     if target == ps.Target.GPU:
-        pytest.importorskip("pycuda")
+        pytest.importorskip("cupy")
     dh = ps.create_data_handling(domain_size=(10, 10), periodicity=True, default_target=target)
 
     x = dh.add_array('x', values_per_cell=1, dtype=dtype)
     dh.fill("x", 0.0, ghost_layers=True)
     y = dh.add_array('y', values_per_cell=1, dtype=dtype)
     dh.fill("y", 1.0, ghost_layers=True)
     z = dh.add_array('z', values_per_cell=1, dtype=dtype)
@@ -39,15 +39,15 @@
 
 
 @pytest.mark.parametrize('dtype', ["float64", "float32"])
 @pytest.mark.parametrize('func', [sp.sin, sp.cos, sp.sinh, sp.cosh, sp.atan])
 @pytest.mark.parametrize('target', [ps.Target.CPU, ps.Target.GPU])
 def test_single_arguments(dtype, func, target):
     if target == ps.Target.GPU:
-        pytest.importorskip("pycuda")
+        pytest.importorskip("cupy")
     dh = ps.create_data_handling(domain_size=(10, 10), periodicity=True, default_target=target)
 
     x = dh.add_array('x', values_per_cell=1, dtype=dtype)
     dh.fill("x", 0.0, ghost_layers=True)
     y = dh.add_array('y', values_per_cell=1, dtype=dtype)
     dh.fill("y", 1.0, ghost_layers=True)
```

### Comparing `pystencils-1.2/pystencils_tests/test_modulo.py` & `pystencils-1.3/pystencils_tests/test_modulo.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pystencils.astnodes import LoopOverCoordinate, Conditional, Block, SympyAssignment
 
 
 @pytest.mark.parametrize('target', [ps.Target.CPU, ps.Target.GPU])
 @pytest.mark.parametrize('iteration_slice', [False, True])
 def test_mod(target, iteration_slice):
     if target == ps.Target.GPU:
-        pytest.importorskip("pycuda")
+        pytest.importorskip("cupy")
     dh = ps.create_data_handling(domain_size=(5, 5), periodicity=True, default_target=ps.Target.CPU)
 
     loop_ctrs = [LoopOverCoordinate.get_loop_counter_symbol(i) for i in range(dh.dim)]
     cond = [sp.Eq(sp.Mod(loop_ctrs[i], 2), 1) for i in range(dh.dim)]
 
     field = dh.add_array("a", values_per_cell=1)
```

### Comparing `pystencils-1.2/pystencils_tests/test_move_constant_before_loop.py` & `pystencils-1.3/pystencils_tests/test_move_constant_before_loop.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_parameterstudy.py` & `pystencils-1.3/pystencils_tests/test_parameterstudy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_plot.py` & `pystencils-1.3/pystencils_tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_print_infinity.py` & `pystencils-1.3/pystencils_tests/test_print_infinity.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     if negative:
         assignment = pystencils.Assignment(x.center, -oo)
     else:
         assignment = pystencils.Assignment(x.center, oo)
     ast = pystencils.create_kernel(assignment, data_type=type, target=target)
 
     if target == pystencils.Target.GPU:
-        pytest.importorskip('pycuda')
+        pytest.importorskip('cupy')
 
     ast.compile()
 
     print(ast.compile().code)
```

### Comparing `pystencils-1.2/pystencils_tests/test_print_unsupported_node.py` & `pystencils-1.3/pystencils_tests/test_print_unsupported_node.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_quicktests.py` & `pystencils-1.3/pystencils_tests/test_quicktests.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_random.py` & `pystencils-1.3/pystencils_tests/test_random.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 @pytest.mark.parametrize('target, rng', ((Target.CPU, 'philox'), (Target.CPU, 'aesni'), (Target.GPU, 'philox')))
 @pytest.mark.parametrize('precision', ('float', 'double'))
 @pytest.mark.parametrize('dtype', ('float', 'double'))
 def test_rng(target, rng, precision, dtype, t=124, offsets=(0, 0), keys=(0, 0), offset_values=None):
     if target == Target.GPU:
-        pytest.importorskip('pycuda')
+        pytest.importorskip('cupy')
     if instruction_sets and {'neon', 'sve', 'vsx', 'rvv'}.intersection(instruction_sets) and rng == 'aesni':
         pytest.xfail('AES not yet implemented for this architecture')
     if rng == 'aesni' and len(keys) == 2:
         keys *= 2
     if offset_values is None:
         offset_values = offsets
```

### Comparing `pystencils-1.2/pystencils_tests/test_sharedmethodcache.py` & `pystencils-1.3/pystencils_tests/test_sharedmethodcache.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_simplification_strategy.py` & `pystencils-1.3/pystencils_tests/test_simplification_strategy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_simplifications.py` & `pystencils-1.3/pystencils_tests/test_simplifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 
 @pytest.mark.parametrize('target', (ps.Target.CPU, ps.Target.GPU))
 @pytest.mark.parametrize('dtype', ('float32', 'float64'))
 @pytest.mark.skipif((vs.major, vs.minor, vs.micro) == (3, 8, 2), reason="does not work on python 3.8.2 for some reason")
 def test_sympy_optimizations(target, dtype):
     if target == ps.Target.GPU:
-        pytest.importorskip("pycuda")
+        pytest.importorskip("cupy")
     src, dst = ps.fields(f'src, dst:  {dtype}[2d]')
 
     assignments = ps.AssignmentCollection({
         src[0, 0]: 1.0 * (sp.exp(dst[0, 0]) - 1)
     })
 
     config = pystencils.config.CreateKernelConfig(target=target, default_number_float=dtype)
@@ -168,15 +168,15 @@
 
 
 @pytest.mark.parametrize('target', (ps.Target.CPU, ps.Target.GPU))
 @pytest.mark.parametrize('simplification', (True, False))
 @pytest.mark.skipif((vs.major, vs.minor, vs.micro) == (3, 8, 2), reason="does not work on python 3.8.2 for some reason")
 def test_evaluate_constant_terms(target, simplification):
     if target == ps.Target.GPU:
-        pytest.importorskip("pycuda")
+        pytest.importorskip("cupy")
     src, dst = ps.fields('src, dst:  float32[2d]')
 
     # cos of a number will always be simplified
     assignments = ps.AssignmentCollection({
         src[0, 0]: -sp.cos(1) + dst[0, 0]
     })
```

### Comparing `pystencils-1.2/pystencils_tests/test_size_and_layout_checks.py` & `pystencils-1.3/pystencils_tests/test_size_and_layout_checks.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_sliced_iteration.py` & `pystencils-1.3/pystencils_tests/test_sliced_iteration.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_slicing.py` & `pystencils-1.3/pystencils_tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_small_block_benchmark.ipynb` & `pystencils-1.3/pystencils_tests/test_small_block_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_source_code_comment.py` & `pystencils-1.3/pystencils_tests/test_source_code_comment.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_staggered_kernel.py` & `pystencils-1.3/pystencils_tests/test_staggered_kernel.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_stencil_plot.ipynb` & `pystencils-1.3/pystencils_tests/test_stencil_plot.ipynb`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_stencils.py` & `pystencils-1.3/pystencils_tests/test_stencils.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_struct_types.py` & `pystencils-1.3/pystencils_tests/test_struct_types.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_subexpression_insertion.py` & `pystencils-1.3/pystencils_tests/test_subexpression_insertion.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_sum_prod.py` & `pystencils-1.3/pystencils_tests/test_sum_prod.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_sympyextensions.py` & `pystencils-1.3/pystencils_tests/test_sympyextensions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_timeloop.py` & `pystencils-1.3/pystencils_tests/test_timeloop.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_transformations.py` & `pystencils-1.3/pystencils_tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_type_interference.py` & `pystencils-1.3/pystencils_tests/test_type_interference.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_types.py` & `pystencils-1.3/pystencils_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_utils.py` & `pystencils-1.3/pystencils_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_vectorization.py` & `pystencils-1.3/pystencils_tests/test_vectorization.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pystencils_tests/test_vectorization_specific.py` & `pystencils-1.3/pystencils_tests/test_vectorization_specific.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/pytest.ini` & `pystencils-1.3/pytest.ini`

 * *Files identical despite different names*

### Comparing `pystencils-1.2/setup.py` & `pystencils-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                  ],
                  project_urls={
                      "Bug Tracker": "https://i10git.cs.fau.de/pycodegen/pystencils/-/issues",
                      "Documentation": "https://pycodegen.pages.i10git.cs.fau.de/pystencils/",
                      "Source Code": "https://i10git.cs.fau.de/pycodegen/pystencils",
                  },
                  extras_require={
-                     'gpu': ['pycuda'],
+                     'gpu': ['cupy'],
                      'alltrafos': ['islpy', 'py-cpuinfo'],
                      'bench_db': ['blitzdb', 'pymongo', 'pandas'],
                      'interactive': ['matplotlib', 'ipy_table', 'imageio', 'jupyter', 'pyevtk', 'rich', 'graphviz'],
                      'doc': ['sphinx', 'sphinx_rtd_theme', 'nbsphinx',
                              'sphinxcontrib-bibtex', 'sphinx_autodoc_typehints', 'pandoc'],
                      'use_cython': ['Cython']
                  },
```

### Comparing `pystencils-1.2/versioneer.py` & `pystencils-1.3/versioneer.py`

 * *Files identical despite different names*

