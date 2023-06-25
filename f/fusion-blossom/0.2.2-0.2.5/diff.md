# Comparing `tmp/fusion_blossom-0.2.2.tar.gz` & `tmp/fusion_blossom-0.2.5.tar.gz`

## Comparing `fusion_blossom-0.2.2.tar` & `fusion_blossom-0.2.5.tar`

### file list

```diff
@@ -1,60 +1,71 @@
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 fusion_blossom-0.2.2/Cargo.toml
--rw-r--r--   0      501       20      766 2022-11-10 15:52:17.000000 fusion_blossom-0.2.2/.gitignore
--rw-r--r--   0      501       20      587 2022-10-15 12:28:31.000000 fusion_blossom-0.2.2/CHANGELOG.md
--rw-r--r--   0      501       20    20716 2022-11-10 18:02:45.000000 fusion_blossom-0.2.2/Cargo.lock
--rw-r--r--   0      501       20     1063 2022-04-15 02:53:09.000000 fusion_blossom-0.2.2/LICENSE
--rw-r--r--   0      501       20    14957 2022-10-26 01:57:07.000000 fusion_blossom-0.2.2/README.md
--rw-r--r--   0      501       20      731 2022-04-19 19:09:23.000000 fusion_blossom-0.2.2/blossomV/blossomV.cpp
--rw-rw-r--   0      501       20     2047 2022-10-19 02:18:42.000000 fusion_blossom-0.2.2/build.rs
--rwxr-xr-x   0      501       20      172 2022-10-08 02:57:09.000000 fusion_blossom-0.2.2/install_environment.sh
--rw-rw-r--   0      501       20     1040 2022-04-19 03:09:55.000000 fusion_blossom-0.2.2/katex-header.html
--rw-r--r--   0      501       20     2390 2022-10-20 17:42:31.000000 fusion_blossom-0.2.2/pyproject.toml
--rw-r--r--   0      501       20       32 2022-10-08 00:38:32.000000 fusion_blossom-0.2.2/rust-toolchain.toml
--rw-r--r--   0      501       20       49 2022-11-10 15:53:27.000000 fusion_blossom-0.2.2/scripts/.gitignore
--rw-r--r--   0      501       20     5126 2022-10-25 17:22:43.000000 fusion_blossom-0.2.2/scripts/NOTES.md
--rw-r--r--   0      501       20     1936 2022-11-10 14:42:44.000000 fusion_blossom-0.2.2/scripts/demo.py
--rw-r--r--   0      501       20     1461 2022-11-10 16:27:34.000000 fusion_blossom-0.2.2/scripts/demo_local_render.py
--rw-r--r--   0      501       20      801 2022-11-09 19:00:37.000000 fusion_blossom-0.2.2/scripts/generate_icon.py
--rw-rw-r--   0      501       20     2828 2022-10-24 19:11:46.000000 fusion_blossom-0.2.2/src/blossom_v.rs
--rw-r--r--   0      501       20   170898 2022-10-09 15:39:13.000000 fusion_blossom-0.2.2/src/bottle.py
--rw-r--r--   0      501       20     9631 2022-10-11 01:18:55.000000 fusion_blossom-0.2.2/src/complete_graph.rs
--rw-r--r--   0      501       20    65537 2022-10-25 16:51:23.000000 fusion_blossom-0.2.2/src/dual_module.rs
--rw-r--r--   0      501       20    77798 2022-10-28 03:00:14.000000 fusion_blossom-0.2.2/src/dual_module_parallel.rs
--rw-r--r--   0      501       20   127689 2022-10-28 02:58:56.000000 fusion_blossom-0.2.2/src/dual_module_serial.rs
--rw-r--r--   0      501       20    42175 2022-11-08 01:33:14.000000 fusion_blossom-0.2.2/src/example_codes.rs
--rw-r--r--   0      501       20    27010 2022-10-28 03:00:14.000000 fusion_blossom-0.2.2/src/example_partition.rs
--rw-r--r--   0      501       20     5557 2022-11-10 15:55:24.000000 fusion_blossom-0.2.2/src/helper.py
--rw-r--r--   0      501       20    10317 2022-11-10 15:30:23.000000 fusion_blossom-0.2.2/src/lib.rs
--rw-r--r--   0      501       20    37194 2022-11-10 15:49:16.000000 fusion_blossom-0.2.2/src/main.rs
--rw-r--r--   0      501       20    23409 2022-11-08 03:19:50.000000 fusion_blossom-0.2.2/src/mwpm_solver.rs
--rw-r--r--   0      501       20    26967 2022-10-15 12:29:43.000000 fusion_blossom-0.2.2/src/pointers.rs
--rw-r--r--   0      501       20    22932 2022-10-25 16:59:22.000000 fusion_blossom-0.2.2/src/primal_module.rs
--rw-r--r--   0      501       20    39257 2022-10-28 03:18:54.000000 fusion_blossom-0.2.2/src/primal_module_parallel.rs
--rw-r--r--   0      501       20   111512 2022-10-25 16:59:22.000000 fusion_blossom-0.2.2/src/primal_module_serial.rs
--rw-r--r--   0      501       20     6622 2022-04-20 18:18:00.000000 fusion_blossom-0.2.2/src/union_find.rs
--rw-r--r--   0      501       20    34985 2022-10-28 03:18:54.000000 fusion_blossom-0.2.2/src/util.rs
--rw-r--r--   0      501       20    35549 2022-11-10 18:29:01.000000 fusion_blossom-0.2.2/src/visualize.rs
--rwxr-xr-x   0      501       20      615 2022-10-19 18:26:47.000000 fusion_blossom-0.2.2/test.sh
--rwxr-xr-x   0      501       20      634 2022-10-19 18:26:49.000000 fusion_blossom-0.2.2/test_build.sh
--rw-r--r--   0      501       20      517 2022-10-28 03:18:23.000000 fusion_blossom-0.2.2/visualize/cmd.js
--rw-r--r--   0      501       20       97 2022-04-20 18:38:15.000000 fusion_blossom-0.2.2/visualize/data/NOTE.md
--rw-r--r--   0      501       20     1115 2022-07-22 14:56:08.000000 fusion_blossom-0.2.2/visualize/data/filter_data.py
--rw-r--r--   0      501       20    40694 2022-11-10 18:14:34.000000 fusion_blossom-0.2.2/visualize/gui3d.js
--rw-r--r--   0      501       20      447 2022-11-09 18:56:43.000000 fusion_blossom-0.2.2/visualize/icon.svg
--rw-r--r--   0      501       20   222696 2022-04-28 01:17:21.000000 fusion_blossom-0.2.2/visualize/img/basic_CSS_3D_bottom_image.png
--rw-r--r--   0      501       20   585200 2022-10-07 19:20:39.000000 fusion_blossom-0.2.2/visualize/img/parallel_circuit_level.png
--rw-r--r--   0      501       20   481044 2022-10-07 19:19:34.000000 fusion_blossom-0.2.2/visualize/img/parallel_phenomenological.png
--rw-r--r--   0      501       20    70570 2022-10-07 19:18:06.000000 fusion_blossom-0.2.2/visualize/img/parallel_simple.png
--rw-r--r--   0      501       20    83192 2022-10-07 19:15:51.000000 fusion_blossom-0.2.2/visualize/img/serial_example.png
--rw-r--r--   0      501       20    90978 2022-10-07 18:59:02.000000 fusion_blossom-0.2.2/visualize/img/serial_random.png
--rw-r--r--   0      501       20    63904 2022-10-07 19:14:29.000000 fusion_blossom-0.2.2/visualize/img/serial_simple.png
--rw-r--r--   0      501       20    14997 2022-11-09 21:10:49.000000 fusion_blossom-0.2.2/visualize/index.html
--rw-r--r--   0      501       20    16448 2022-11-10 18:33:44.000000 fusion_blossom-0.2.2/visualize/index.js
--rw-r--r--   0      501       20     3884 2022-11-10 18:14:29.000000 fusion_blossom-0.2.2/visualize/mocker.js
--rw-r--r--   0      501       20   237147 2022-11-10 14:41:50.000000 fusion_blossom-0.2.2/visualize/package-lock.json
--rw-r--r--   0      501       20      472 2022-11-10 18:11:59.000000 fusion_blossom-0.2.2/visualize/package.json
--rw-r--r--   0      501       20    39569 2022-10-25 17:03:33.000000 fusion_blossom-0.2.2/visualize/partition-profile.html
--rw-r--r--   0      501       20     9266 2022-11-10 18:16:35.000000 fusion_blossom-0.2.2/visualize/patches.js
--rw-r--r--   0      501       20     8259 2022-11-09 21:09:24.000000 fusion_blossom-0.2.2/visualize/primal.js
--rwxr-xr-x   0      501       20     2446 2022-10-09 02:47:30.000000 fusion_blossom-0.2.2/visualize/server.py
--rw-r--r--   0        0        0    16418 1970-01-01 00:00:00.000000 fusion_blossom-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 fusion_blossom-0.2.5/Cargo.toml
+-rw-r--r--   0      501       20      766 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/.gitignore
+-rw-r--r--   0      501       20      587 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/CHANGELOG.md
+-rw-r--r--   0      501       20      294 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/CITATION.cff
+-rw-r--r--   0      501       20    52074 2023-06-24 19:12:20.000000 fusion_blossom-0.2.5/Cargo.lock
+-rw-r--r--   0      501       20     1063 2022-04-15 02:53:09.000000 fusion_blossom-0.2.5/LICENSE
+-rw-r--r--   0      501       20    12493 2023-06-02 18:21:20.000000 fusion_blossom-0.2.5/README.md
+-rw-r--r--   0      501       20      731 2022-04-19 19:09:23.000000 fusion_blossom-0.2.5/blossomV/blossomV.cpp
+-rw-r--r--   0      501       20     2183 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/build.rs
+-rwxr-xr-x   0      501       20      172 2022-10-08 02:57:09.000000 fusion_blossom-0.2.5/install_environment.sh
+-rw-rw-r--   0      501       20     1040 2022-04-19 03:09:55.000000 fusion_blossom-0.2.5/katex-header.html
+-rw-r--r--   0      501       20     2390 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/pyproject.toml
+-rw-r--r--   0      501       20       32 2023-05-29 20:07:24.000000 fusion_blossom-0.2.5/rust-toolchain.toml
+-rw-r--r--   0      501       20       48 2023-06-25 03:00:38.000000 fusion_blossom-0.2.5/rustfmt.toml
+-rw-r--r--   0      501       20       49 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/.gitignore
+-rw-r--r--   0      501       20     5126 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/NOTES.md
+-rw-r--r--   0      501       20     1695 2023-06-02 18:21:20.000000 fusion_blossom-0.2.5/scripts/count_Rust_LOC.py
+-rw-r--r--   0      501       20     1930 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/demo.py
+-rw-r--r--   0      501       20     1461 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/demo_local_render.py
+-rw-r--r--   0      501       20     1293 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/demo_visualizer.py
+-rw-r--r--   0      501       20      801 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/generate_icon.py
+-rw-r--r--   0      501       20    26333 2023-06-25 03:14:00.000000 fusion_blossom-0.2.5/src/bin/aps2023.rs
+-rw-r--r--   0      501       20    31586 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/bin/fusion-paper.rs
+-rw-r--r--   0      501       20     3928 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/bin/partition-strategy.rs
+-rw-r--r--   0      501       20     2834 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/blossom_v.rs
+-rw-r--r--   0      501       20   170898 2022-10-09 15:39:13.000000 fusion_blossom-0.2.5/src/bottle.py
+-rw-r--r--   0      501       20    47658 2023-06-25 03:04:12.000000 fusion_blossom-0.2.5/src/cli.rs
+-rw-r--r--   0      501       20    15491 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/complete_graph.rs
+-rw-r--r--   0      501       20    69826 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/dual_module.rs
+-rw-r--r--   0      501       20    87247 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/dual_module_parallel.rs
+-rw-r--r--   0      501       20   142629 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/dual_module_serial.rs
+-rw-r--r--   0      501       20    55382 2023-06-25 03:16:42.000000 fusion_blossom-0.2.5/src/example_codes.rs
+-rw-r--r--   0      501       20    38310 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/example_partition.rs
+-rw-r--r--   0      501       20     5557 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/src/helper.py
+-rw-r--r--   0      501       20    10844 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/lib.rs
+-rw-r--r--   0      501       20       91 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/main.rs
+-rw-r--r--   0      501       20    33564 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/mwpm_solver.rs
+-rw-r--r--   0      501       20    27238 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/pointers.rs
+-rw-r--r--   0      501       20    25243 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/primal_module.rs
+-rw-r--r--   0      501       20    49538 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/primal_module_parallel.rs
+-rw-r--r--   0      501       20   129499 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/primal_module_serial.rs
+-rw-r--r--   0      501       20    37642 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/util.rs
+-rw-r--r--   0      501       20    41597 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/visualize.rs
+-rwxr-xr-x   0      501       20      615 2023-06-25 01:30:13.000000 fusion_blossom-0.2.5/test.sh
+-rwxr-xr-x   0      501       20      860 2023-06-25 01:42:55.000000 fusion_blossom-0.2.5/test_build.sh
+-rwxr-xr-x   0      501       20      742 2023-06-25 02:49:16.000000 fusion_blossom-0.2.5/test_check.sh
+-rwxr-xr-x   0      501       20       81 2023-06-24 17:38:10.000000 fusion_blossom-0.2.5/test_python.sh
+-rw-r--r--   0      501       20      825 2023-06-24 17:52:59.000000 fusion_blossom-0.2.5/tests/python/test_demo.py
+-rw-r--r--   0      501       20     1528 2023-06-24 18:21:06.000000 fusion_blossom-0.2.5/tests/python/test_dynamic_weights.py
+-rw-r--r--   0      501       20      517 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/cmd.js
+-rw-r--r--   0      501       20       97 2022-04-20 18:38:15.000000 fusion_blossom-0.2.5/visualize/data/NOTE.md
+-rw-r--r--   0      501       20     1115 2022-07-22 14:56:08.000000 fusion_blossom-0.2.5/visualize/data/filter_data.py
+-rw-r--r--   0      501       20    41031 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/gui3d.js
+-rw-r--r--   0      501       20      447 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/icon.svg
+-rw-r--r--   0      501       20   222696 2022-04-28 01:17:21.000000 fusion_blossom-0.2.5/visualize/img/basic_CSS_3D_bottom_image.png
+-rw-r--r--   0      501       20   585200 2022-10-07 19:20:39.000000 fusion_blossom-0.2.5/visualize/img/parallel_circuit_level.png
+-rw-r--r--   0      501       20   481044 2022-10-07 19:19:34.000000 fusion_blossom-0.2.5/visualize/img/parallel_phenomenological.png
+-rw-r--r--   0      501       20    70570 2022-10-07 19:18:06.000000 fusion_blossom-0.2.5/visualize/img/parallel_simple.png
+-rw-r--r--   0      501       20    83192 2022-10-07 19:15:51.000000 fusion_blossom-0.2.5/visualize/img/serial_example.png
+-rw-r--r--   0      501       20    90978 2022-10-07 18:59:02.000000 fusion_blossom-0.2.5/visualize/img/serial_random.png
+-rw-r--r--   0      501       20    63904 2022-10-07 19:14:29.000000 fusion_blossom-0.2.5/visualize/img/serial_simple.png
+-rw-r--r--   0      501       20    14997 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/index.html
+-rw-r--r--   0      501       20    16448 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/index.js
+-rw-r--r--   0      501       20     3884 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/mocker.js
+-rw-r--r--   0      501       20   237147 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/package-lock.json
+-rw-r--r--   0      501       20      472 2022-11-10 18:11:59.000000 fusion_blossom-0.2.5/visualize/package.json
+-rw-r--r--   0      501       20    39914 2023-06-02 18:21:20.000000 fusion_blossom-0.2.5/visualize/partition-profile.html
+-rw-r--r--   0      501       20     9266 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/patches.js
+-rw-r--r--   0      501       20     8259 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/primal.js
+-rwxr-xr-x   0      501       20     2446 2022-12-11 15:29:34.000000 fusion_blossom-0.2.5/visualize/server.py
+-rw-r--r--   0        0        0    13954 1970-01-01 00:00:00.000000 fusion_blossom-0.2.5/PKG-INFO
```

### Comparing `fusion_blossom-0.2.2/Cargo.toml` & `fusion_blossom-0.2.5/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "fusion-blossom"
-version = "0.2.2"
+version = "0.2.5"
 authors = ["Yue Wu <wuyue16pku@gmail.com>"]
 edition = "2021"
 license = "MIT"
 description = "A fast minimum-weight perfect matching solver for quantum error correction"
 readme = "README.md"
 homepage = "https://fusionblossom.com"
 repository = "https://github.com/yuewuo/fusion-blossom"
@@ -12,14 +12,15 @@
 categories = ["science"]
 exclude = [
     "tutorial/*",
     "benchmark/*",
     "visualize/data/persist/*",
     ".github/*",
 ]
+default-run = "fusion_blossom"
 
 # see https://doc.rust-lang.org/1.39.0/cargo/reference/manifest.html#the-documentation-field-optional
 [badges]
 maintenance = { status = "actively-developed" }
 
 [lib]
 name = "fusion_blossom"
@@ -46,33 +47,39 @@
 i32_weight = []  # use i32 instead of i64 as weight type, to be the same as blossom V library
 u32_index = []  # use u32 instead of usize as index type, to save memory by at most half
 ordered_conflicts = []  # sort conflict events, by default do not sort for better performance
 disable_visualizer = []  # disable all visualizer behavior
 unsafe_pointer = []  # use raw pointers to access data without lock when appropriate; fusion blossom requires very little synchronization
 dangerous_pointer = ["unsafe_pointer"]  # use raw pointers instead of Arc and Weak, require "unsafe_pointer" feature
 python_binding = ["pyo3"]  # bind to Python
+qecp_integrate = ["qecp"]
 
 [dependencies]
 rand_xoshiro = "0.6.0"
 libc = "0.2.124"
 cfg-if = "1.0.0"
 priority-queue = "1.2.1"
 parking_lot = { version = "0.12.1", features = ["hardware-lock-elision"] }
 serde = { version = "1.0.117", features = ["derive", "rc"] }
 serde_json = "1.0.59"
 chrono = "0.4.19"
 derivative = "2.2.0"
 urlencoding = "2.1.0"
-clap = { version = "3.2.22", features = ["cargo", "derive"] }
+clap = { version = "4.2.4", features = ["cargo", "derive"] }
 pbr = "1.0.4"
-rayon = "1.5.3"
+rayon = "1.7.0"
 weak-table = "0.3.2"
 rand = "0.8.5"
-core_affinity = "0.5.10"
-pyo3 = { version =  "0.17.2", features = ["extension-module", "multiple-pymethods", "abi3-py37"], optional = true }
+core_affinity = "0.8.0"
+pyo3 = { version =  "0.18.3", features = ["extension-module", "multiple-pymethods", "abi3-py37"], optional = true }
+lazy_static = "1.4.0"
+petgraph = "0.6.3"
+qecp = { version = "0.2.2", features = ["fusion-blossom"], optional = true }
 
 [build-dependencies]
 cc = "1.0.66"
 
+[dev-dependencies]
+
 [package.metadata.docs.rs]
 rustdoc-args = [ "--html-in-header", "katex-header.html" ]
 # to run locally: `RUSTDOCFLAGS="--html-in-header katex-header.html" cargo doc --no-deps`
```

### Comparing `fusion_blossom-0.2.2/.gitignore` & `fusion_blossom-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/CHANGELOG.md` & `fusion_blossom-0.2.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/LICENSE` & `fusion_blossom-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/README.md` & `fusion_blossom-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,146 @@
+Metadata-Version: 2.1
+Name: fusion_blossom
+Version: 0.2.5
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Internet
+License-File: LICENSE
+Summary: A fast minimum-weight perfect matching solver for quantum error correction
+Keywords: QEC,quantum-computing,error-correction,visualization
+Home-Page: https://fusionblossom.com
+Author: Yue Wu <wuyue16pku@gmail.com>
+Author-email: Yue Wu <wuyue16pku@gmail.com>
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/yuewuo/fusion-blossom
+
 ![Build Status](https://jenkins.fusionblossom.com/buildStatus/icon?job=FusionBlossomBuild&subject=build&style=flat-square)
 ![Test Status](https://jenkins.fusionblossom.com/buildStatus/icon?job=FusionBlossomCI&subject=test&style=flat-square)
 <!-- ![Build Python Binding](https://github.com/yuewuo/fusion-blossom/actions/workflows/wheels.yml/badge.svg) -->
 
 # Fusion Blossom
 A fast Minimum-Weight Perfect Matching (MWPM) solver for Quantum Error Correction (QEC)
 
 Please see [our tutorial for a quick explanation and some Python demos](https://tutorial.fusionblossom.com).
 
+Our paper is out on arXiv! [https://arxiv.org/abs/2305.08307](https://arxiv.org/abs/2305.08307)
+
 ## Key Features
 
 - **Correctness**: This is an exact MWPM solver, verified against the [Blossom V library](https://pub.ist.ac.at/~vnk/software.html) with millions of randomized test cases .
-- **Linear Complexity**: The decoding time is roughly $O(N)$ given small physical error rate, proportional to the number of defect vertices $N$.
+- **Linear Complexity**: The average decoding time is roughly $O(N)$ given small physical error rate, proportional to the number of defect vertices $N$.
 - **Parallelism**: A single MWPM decoding problem can be partitioned and solved in parallel, then *fused* together to find an **exact** global MWPM solution.
-- **Simple Interface**: The graph problem is abstracted and easy-to-use for QEC applications.
+- **Simple Interface**: The graph problem is abstracted and easy-to-use for QEC applications. Especially, it supports decoding erasure errors (by setting some edge weights to 0 on the fly).
 
 ## Benchmark Highlights
 
-- In phenomenological noise model with **$p$ = 0.005**, code distance **$d$ = 21**, planar code with $d(d-1)$ = 420 $Z$ stabilizers, 100000 measurement rounds
-  - single-thread: **2.4us per defect vertex** or 29us per measurement round
-  - 64-threads: 58ns per defect vertex or **0.7us per measurement round**
+- In circuit-level noise model with **$p$ = 0.001**, code distance **$d$ = 21**, rotated CSS code, 100000 measurement rounds
+  - single-thread: **3.9us per defect vertex** or 13us per measurement round
+  - 64-threads: 95ns per defect vertex or **0.3us per measurement round**
+  - in streaming mode, the latency is **0.7ms regardless of rounds of measurement**
 
 ## Background and Key Ideas
 
 MWPM decoders are widely known for its high accuracy [[1]](#fowler2012topological) and several optimizations that further improves its accuracy [[2]](#criger2018multi). However, there weren't many publications that improve the speed of the MWPM decoder over the past 10 years. Fowler implemented an $O(N)$ asymptotic complexity MWPM decoder in [[3]](#fowler2012towards) and proposed an $O(1)$ complexity parallel MWPM decoder in [[4]](#fowler2013minimum), but none of these are publicly available to our best knowledge. Higgott implemented a fast but approximate MWPM decoder (namely "local matching") with roughly $O(N)$ complexity in [[5]](#higgott2022pymatching). With recent experiments of successful QEC on real hardware, it's time for a fast and accurate MWPM decoder to become available to the community.
 
 Our idea comes from our study on the Union-Find (UF) decoder [[6]](#delfosse2021almost). UF decoder is a fast decoder with $O(N)$ worst-case time complexity, at the cost of being less accurate compared to the MWPM decoder. Inspired by the Fowler's diagram [[3]](#fowler2012towards), we found a relationship between the UF decoder [[7]](#wu2022interpretation). This [nice animation](https://us.wuyue98.cn/aps2022/#/3/1) (press space to trigger animation) could help people see the analogy between UF and MWPM decoders. With this interpretation, we're able to combind the strength of UF and MWPM decoders together.
 
 - From the UF decoder, we learnt to use a sparse decoding graph representation for fast speed
 - From the MWPM decoder, we learnt to find an exact minimum-weight perfect matching for high accuracy
 
-We shall note that Oscar Higgott and Craig Gidney independently reach the same approach of using sparse decoding graph to solve MWPM more efficiently in PyMatching V2 [[8]](#pymatchingv2). It's impressive to see that they have much better single-thread performance than fusion-blossom (about 5x-20x speedup). They use more optimizations like priority queue and single-tree strategy that appears in existing literature of blossom algorithms  (possibly some other novel techniques, looking forward to their paper!). Also, they use C++ language rather than Rust programming language. Rust enforces memory safety which adds some runtime overhead (like vector boundary check and unnecessary locks in parallel programming). We use `unsafe` Rust to improve the speed by 1.5x-3x but these features are not yet enabled in the Python library and only available when using the native Rust library. In fact, PyMatching V2's optimizations and fusion-blossom's parallel computation (fusion operation) are compatible with each other. With their impressive work, we're looking forward to another 5x-20x speed of the parallel MWPM decoder if combined together. For now, user should use PyMatching for better CPU efficiency in large-scale simulations, and use fusion-blossom library as an educational tool with [visualization tool](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json) and [entry-level tutorials](https://tutorial.fusionblossom.com).
+We shall note that Oscar Higgott and Craig Gidney independently reach the same approach of using sparse decoding graph to solve MWPM more efficiently in PyMatching V2 [[8]](#pymatchingv2). It's impressive to see that they have much better single-thread performance than fusion-blossom (about 5x-20x speedup). They use more optimizations like priority queue that appears in existing literature of blossom algorithms (check their paper at [[9]](#higgott2023sparse)). Also, they use C++ language rather than Rust programming language. Rust enforces memory safety which adds some runtime overhead (like vector boundary check and unnecessary locks in parallel programming). We use `unsafe` Rust to improve the speed by 1.5x-3x but these features are not yet enabled in the Python library and only available when using the native Rust library. In fact, PyMatching V2's optimizations and fusion-blossom's parallel computation (fusion operation) are compatible with each other. With their impressive work, we're looking forward to another 5x-20x speed of the parallel MWPM decoder if combined together. For now, user should use PyMatching for better CPU efficiency in large-scale simulations, and use fusion-blossom library as an educational tool with [visualization tool](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json) and [entry-level tutorials](https://tutorial.fusionblossom.com).
 
 ## Demo
 
 We highly suggest you watch through several demos here to get a sense of how the algorithm works. All our demos are captured from real algorithm execution. In fact, we're showing you the visualized debugger tool we wrote for fusion blossom. The demo is a 3D website and you can control the view point as you like.
 
-For more details of why it finds an exact MWPM, please read our paper [coming soon 💪].
-
 Click the demo image below to view the corresponding demo
 
 #### Serial Execution
 
-[<img src="https://visualize.fusionblossom.com/img/serial_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_1.json)
-[<img src="https://visualize.fusionblossom.com/img/serial_example.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json)
-[<img src="https://visualize.fusionblossom.com/img/serial_random.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_11.json)
+[<img src="./visualize/img/serial_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_1.json)
+[<img src="./visualize/img/serial_example.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json)
+[<img src="./visualize/img/serial_random.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_11.json)
 
 #### Parallel Execution (Shown in Serial For Better Visual)
 
-[<img src="https://visualize.fusionblossom.com/img/parallel_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_parallel_basic_3.json)
-[<img src="https://visualize.fusionblossom.com/img/parallel_phenomenological.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_1.json)
-[<img src="https://visualize.fusionblossom.com/img/parallel_circuit_level.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_2.json)
+[<img src="./visualize/img/parallel_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_parallel_basic_3.json)
+[<img src="./visualize/img/parallel_phenomenological.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_1.json)
+[<img src="./visualize/img/parallel_circuit_level.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_2.json)
 
 ## Usage
 
-Our code is written in [Rust](https://www.rust-lang.org/) programming language for speed and memory safety, but it's hardly a easy language to learn. To make the decoder more accessible, we bind the library to Python and user can simply install the library using `pip3 install fusion-blossom`.
+Our code is written in [Rust](https://www.rust-lang.org/) programming language for speed and memory safety, but it's hardly an easy language to learn. To make the decoder more accessible, we bind the library to Python and user can simply install the library using `pip3 install fusion-blossom`.
 
 We have several Python demos at [the tutorial website](https://tutorial.fusionblossom.com/demo/example-qec-codes.html) . Also there is a simple example for decoder, and you can run it by cloning the project and run `python3 scripts/demo.py`.
 
-For parallel solver, it needs user to provide a partition strategy. Please wait for our paper for a thorough description of how partition works.
-
-## Evaluation
-
-We use Intel(R) Xeon(R) Platinum 8375C CPU for evaluation, with 64 physical cores and 128 threads. Note that Apple m1max CPU has roughly 2x single-core decoding speed, but it has limited number of cores so we do not use data from m1max. The benchmark scripts can be found in `benchmark` folder, running in Rust native binary (not the Python package, which has fewer optimization features enabled). By default, we test phenomenological noise model with **$p$ = 0.005**, code distance **$d$ = 21**, planar code with $d(d-1)$ = 420 $Z$ stabilizers, 100000 measurement rounds.
-
-First of all, the number of partitions will effect the speed. Intuitively, the more partitions there are, the more overhead because fusing two partitions consumes more computation than solving them as a whole. But in practice, memory access is not always at the same speed. If cache cannot hold the data, then solving big partition may consume even more time than solving small ones. We test on a single-thread decoder, and try different partition numbers. At partition number = 2000, we get roughly the minimum decoding time of 2.4us per defect vertex. This corresponds to each partition hosting 50 measurement rounds (decoding blocks of 49 * 21 * 20).
-
-![](https://visualize.fusionblossom.com/data/benchmark/paper_parallel_fusion_blossom/partition_num_single_thread_2_tree/decoding_time_per_defect.svg)
-
-Given the optimal partition number of a single thread, we keep the partition number the same and try increasing the number of threads. Note that the partition number may not be optimal for large number of threads, but even in this case, we reach 41x speed up given 64 physical cores. The decoding time is pushed to 58ns per sydnrome or 0.7us per measurement round. This can catch up with the 1us measurement round of a superconducting circuit. Interestingly, we found that hyperthreading won't help much in this case, perhaps because this decoder is memory-bounded, meaning memory throughput is the bottleneck. Although the number of defect vertices is only a small portion, they are randomly distributed so every time a new syndrome is given, the memory is almost always cold and incur large cache miss panelty.
-
-![](https://visualize.fusionblossom.com/data/benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/decoding_time_per_defect.svg)
-
-In order to understand the bottleneck of  parallel execution, we wrote a visualization tool to display the execution windows of base partitions and fusion operations on multiple threads. Blue blocks is the base partition and green blocks is the fusion operation. Fusion operation only scales with the size of the fusion boundary and the depth of active partitions, irrelevant to the base partition's size. We'll study different partition and fusion strategies in our paper. Below shows the parallel execution on 64 threads. Blue blocks are base partitions, each is a 49 * 21 * 20 decoding graph block. Green blocks are fusion blocks, each is a 1 * 21 * 20 decoding graph block sandwiched by two neighbor base partitions. You can click the image which jumps to this interactive visualization tool.
-
-[<img src="https://visualize.fusionblossom.com/data/benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/64.svg"/>](https://visualize.fusionblossom.com/partition-profile.html?filename=benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/tmp/64.profile)
+For parallel solver, it needs user to provide a partition strategy. Please check our paper for a thorough description of how partition works.
 
 ## Interface
 
 #### Sparse Decoding Graph and Integer Weights
 
 The weights in QEC decoding graph are computed by taking the log of error probability, e.g. $w_e = \log\{(1-p)/p\}$ or roughly $w_e = -\log{p}$, we can safely use integers to save weights by e.g. multiplying the weights by 1e6 and truncate to nearest integer. In this way, the truncation error $\Delta w_e = 1$ of integer weights corresponds to relative error $\Delta p /{p}=10^{-6}$ which is small enough. Suppose physical error rate $p$ is in the range of a positive `f64` variable (2.2e-308 to 1), the maximum weight is 7e7,which is well below the maximum value of a `u32` variable (4.3e9). Since weights only sum up in our algorithm (no multiplication), `u32` is large enough and accurate enough. By default we use `usize` which is platform dependent (usually 64 bits), but you can 
 
 We use integer also for ease of migrating to FPGA implementation. In order to fit more vertices into a single FPGA, it's necessary to reduce the resource usage for each vertex. Integers are much cheaper than floating-point numbers, and also it allows flexible trade-off between resource usage and accuracy, e.g. if all weights are equal, we can simply use a 2 bit integer.
 
 Note that other libraries of MWPM solver like [Blossom V](https://doi.org/10.1007/s12532-009-0002-8) also default to integer weights as well. Although one can change the macro to use floating-point weights, it's not recommended because "the code may even get stuck due to rounding errors".
 
-## Installation
-
-Here is an example installation on Ubuntu20.04.
-
-```sh
-# install rust compiler and package manager
-curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
-# install build dependencies
-sudo apt install build-essential
-```
-
 ## Tests
 
-In order to test the correctness of our MWPM solver, we need a ground-truth MWPM solver. [Blossom V](https://doi.org/10.1007/s12532-009-0002-8) is widely-used in existing MWPM decoders, but according to the license we cannot embed it in this library. To run the test cases with ground truth comparison or enable the functions like `blossom_v_mwpm`, you need to download this library [at this website](https://pub.ist.ac.at/~vnk/software.html) to a folder named `blossomV` at the root directory of this git repo.
+In order to test the correctness of our MWPM solver, we need a ground-truth MWPM solver. [Blossom V](https://doi.org/10.1007/s12532-009-0002-8) is widely-used in existing MWPM decoders, but according to the license we cannot embed it in this library.To run the test cases with ground truth comparison or enable the functions like `blossom_v_mwpm`, you need to download this library [at this website](https://pub.ist.ac.at/~vnk/software.html) to a folder named `blossomV` at the root directory of this git repo.
 
 ```shell
 wget -c https://pub.ist.ac.at/~vnk/software/blossom5-v2.05.src.tar.gz -O - | tar -xz
 cp -r blossom5-v2.05.src/* blossomV/
 rm -r blossom5-v2.05.src
 ```
 
-# Visualize
+# Visualization
+
+## Visualize the solving procedure of a single decoding problem
 
 To start a server, run the following
 ```sh
 cd visualize
-npm install  # to download packages
-# you can choose to render locally or to view it in a browser interactively
-# interactive: open url using a browser (Chrome recommended)
-node index.js <url> <width> <height>  # local render
+python3 server.py  # server
 
-# for example you can run the following command to get url
+# to view it in a browser interactively, you can run the following command to get url
 cd ..
 cargo test visualize_paper_weighted_union_find_decoder -- --nocapture
+
+# alternatively, you can choose to render locally
+npm install  # to download packages
+node index.js <url> <width> <height>  # local render
 ```
 
+## Visualize parallel execution of multiple decoding problems
+
+In order to understand the bottleneck of  parallel execution, we wrote a visualization tool to display the execution windows of base partitions and fusion operations on multiple threads. Fusion operation only scales with the size of the fusion boundary and the depth of active partitions, irrelevant to the base partition's size. We study different partition and fusion strategies in our paper. Below shows the parallel execution on 64 threads. Blue blocks are base partitions, each consists of 49 rounds of measurement. Green blocks are fusion operations, a single round of measurement sandwiched by two neighbor base partitions. You can click the image which jumps to this interactive visualization tool.
+
+[<img src="./benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/64.svg"/>](https://visualize.fusionblossom.com/partition-profile.html?filename=benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/tmp/64.profile)
+
 # TODOs
 
 - [ ] support erasures in parallel solver
 
 # Acknowledgements
 
 This project is funded by [NSF MRI: Development of PARAGON: Control Instrument for Post NISQ Quantum Computing](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2216030)
@@ -143,7 +159,10 @@
 
 <a id="delfosse2021almost">[6]</a> Delfosse, Nicolas, and Naomi H. Nickerson. "Almost-linear time decoding algorithm for topological codes." Quantum 5 (2021): 595.
 
 <a id="wu2022interpretation">[7]</a> Wu, Yue. APS 2022 March Meeting Talk "Interpretation of Union-Find Decoder on Weighted Graphs and Application to XZZX Surface Code". Slides: [https://us.wuyue98.cn/aps2022](https://us.wuyue98.cn/aps2022), Video: [https://youtu.be/BbhqUHKPdQk](https://youtu.be/BbhqUHKPdQk)
 
 <a id="pymatchingv2">[8]</a> Higgott, Oscar. PyMatching v2 https://github.com/oscarhiggott/PyMatching
 
+<a id="higgott2023sparse">[9]</a> Higgott, Oscar, and Craig Gidney. "Sparse Blossom: correcting a million errors per core second with minimum-weight matching." arXiv preprint arXiv:2303.15933 (2023).
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fusion_blossom-0.2.2/blossomV/blossomV.cpp` & `fusion_blossom-0.2.5/blossomV/blossomV.cpp`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/build.rs` & `fusion_blossom-0.2.5/build.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 extern crate cc;
 use std::env;
 use std::path::Path;
 
 fn main() {
+    if cfg!(feature = "unsafe_pointer") {
+        println!("cargo:allow=dropping_references");
+    }
 
     // even if the blossom V library exists, sometimes we don't want to compile it
     let mut try_include_blossom_v = true;
     if cfg!(feature = "remove_blossom_v") {
         try_include_blossom_v = false;
     }
 
     if try_include_blossom_v && Path::new("./blossomV/PerfectMatching.h").exists() {
-
         println!("cargo:rustc-cfg=feature=\"blossom_v\"");
 
         let target_os = env::var("CARGO_CFG_TARGET_OS");
 
         let mut build = cc::Build::new();
 
-        build.cpp(true)
+        build
+            .cpp(true)
             .file("./blossomV/blossomV.cpp")
             .file("./blossomV/PMinterface.cpp")
             .file("./blossomV/PMduals.cpp")
             .file("./blossomV/PMexpand.cpp")
             .file("./blossomV/PMinit.cpp")
             .file("./blossomV/PMmain.cpp")
             .file("./blossomV/PMrepair.cpp")
             .file("./blossomV/PMshrink.cpp")
             .file("./blossomV/misc.cpp")
             .file("./blossomV/MinCost/MinCost.cpp");
-    
-        if target_os != Ok("macos".to_string()) {  // exclude from macOS
+
+        if target_os != Ok("macos".to_string()) {
+            // exclude from macOS
             build.cpp_link_stdlib("stdc++"); // use libstdc++
-            build.flag("-Wno-unused-but-set-variable");  // this option is not available in clang
+            build.flag("-Wno-unused-but-set-variable"); // this option is not available in clang
         }
 
         // ignore warnings from blossom library
-        build.flag("-Wno-unused-parameter")
+        build
+            .flag("-Wno-unused-parameter")
             .flag("-Wno-unused-variable")
             .flag("-Wno-reorder-ctor")
             .flag("-Wno-reorder")
             .compile("blossomV");
 
         println!("cargo:rerun-if-changed=./blossomV/blossomV.cpp");
         println!("cargo:rerun-if-changed=./blossomV/PerfectMatching.h");
-    
+
         println!("cargo:rustc-link-lib=static=blossomV");
 
-        if target_os != Ok("macos".to_string()) {  // exclude from macOS
+        if target_os != Ok("macos".to_string()) {
+            // exclude from macOS
             // println!("cargo:rustc-link-lib=static=stdc++");  // have to add this to compile c++ (new, delete operators)
-            println!("cargo:rustc-link-lib=dylib=stdc++");  // NOTE: this MUST be put after "cargo:rustc-link-lib=static=blossomV"
+            println!("cargo:rustc-link-lib=dylib=stdc++"); // NOTE: this MUST be put after "cargo:rustc-link-lib=static=blossomV"
         }
-
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/katex-header.html` & `fusion_blossom-0.2.5/katex-header.html`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/pyproject.toml` & `fusion_blossom-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/scripts/NOTES.md` & `fusion_blossom-0.2.5/scripts/NOTES.md`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/scripts/demo.py` & `fusion_blossom-0.2.5/scripts/demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import fusion_blossom as fb
 
 # create an example code
 code = fb.CodeCapacityPlanarCode(d=11, p=0.05, max_half_weight=500)
 initializer = code.get_initializer()  # the decoding graph structure (you can easily construct your own)
 positions = code.get_positions()  # the positions of vertices in the 3D visualizer, optional
 
-# randomly generate a syndrome according to the error model
+# randomly generate a syndrome according to the noise model
 syndrome = code.generate_random_errors(seed=1000)
 with fb.PyMut(syndrome, "defect_vertices") as defect_vertices:
     defect_vertices.append(0)  # you can modify the defect vertices
 print(syndrome)
 
 # visualizer (optional for debugging)
 visualizer = None
@@ -22,17 +22,17 @@
     visualize_filename = fb.static_visualize_data_filename()
     visualizer = fb.Visualizer(filepath=visualize_filename, positions=positions)
 
 solver = fb.SolverSerial(initializer)
 solver.solve(syndrome, visualizer)  # enable visualizer for debugging
 perfect_matching = solver.perfect_matching()
 print(f"\n\nMinimum Weight Perfect Matching (MWPM):")
-print(f"    - peer_matchings: {perfect_matching.peer_matchings}")  # Vec<(SyndromeIndex, SyndromeIndex)>
+print(f"    - peer_matchings: {perfect_matching.peer_matchings}")  # Vec<(DefectIndex, DefectIndex)>
 print(f"          = vertices: {[(defect_vertices[a], defect_vertices[b]) for a, b in perfect_matching.peer_matchings]}")
-print(f"    - virtual_matchings: {perfect_matching.virtual_matchings}")  # Vec<(SyndromeIndex, VertexIndex)>
+print(f"    - virtual_matchings: {perfect_matching.virtual_matchings}")  # Vec<(DefectIndex, VertexIndex)>
 print(f"             = vertices: {[(defect_vertices[a], b) for a, b in perfect_matching.virtual_matchings]}")
 subgraph = solver.subgraph(visualizer)
 print(f"Minimum Weight Parity Subgraph (MWPS): {subgraph}\n\n")  # Vec<EdgeIndex>
 solver.clear()  # clear is O(1) complexity, recommended for repetitive simulation
 
 # view in browser
 if visualizer is not None:
```

### Comparing `fusion_blossom-0.2.2/scripts/demo_local_render.py` & `fusion_blossom-0.2.5/scripts/demo_local_render.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/scripts/generate_icon.py` & `fusion_blossom-0.2.5/scripts/generate_icon.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from svgwrite import cm
 
 
 def main():
     dir = os.path.dirname(__file__)
     draw(os.path.join(dir, f"F.svg"), "F", "#7743DB", "#FFFFFF")
     draw(os.path.join(dir, f"Q.svg"), "Q", "#7D8F69", "#FFFFFF")
-    draw(os.path.join(dir, f"M.svg"), "M", "#9F73AB", "#FFFFFF")
+    draw(os.path.join(dir, f"M.svg"), "M", "#F49D1A", "#FFFFFF")
 
 def draw(filepath, letter, background_color, text_color):
     width = 1000
     dwg = svgwrite.Drawing(filename=filepath, size=(width, width), debug=True)
     font_size = 800
     dwg.add(dwg.rect(insert=(0,0), size=(width, width), rx=f"{width/6}", fill=background_color))
     dwg.add(dwg.text(f"{letter}", x=[width/2], y=[width/2+font_size/2-100], fill=text_color, stroke=text_color
```

### Comparing `fusion_blossom-0.2.2/src/blossom_v.rs` & `fusion_blossom-0.2.5/src/blossom_v.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 use super::cfg_if;
 
-
 cfg_if::cfg_if! {
     if #[cfg(feature="blossom_v")] {
 
         use super::libc;
         use libc::{c_int};
         use std::collections::BTreeSet;
 
@@ -60,14 +59,15 @@
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
-    fn blossom_v_test_1() {  // cargo test blossom_v_test_1 -- --nocapture
+    fn blossom_v_test_1() {
+        // cargo test blossom_v_test_1 -- --nocapture
         let node_num = 4;
         let edges: Vec<(usize, usize, u32)> = vec![(0, 1, 100), (2, 3, 110), (0, 2, 500), (1, 3, 300)];
         let output = safe_minimum_weight_perfect_matching(node_num, &edges);
         assert_eq!(output, vec![1, 0, 3, 2]);
     }
 }
```

### Comparing `fusion_blossom-0.2.2/src/bottle.py` & `fusion_blossom-0.2.5/src/bottle.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/src/complete_graph.rs` & `fusion_blossom-0.2.5/src/complete_graph.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+use super::dual_module::EdgeWeightModifier;
 use super::util::*;
 use crate::priority_queue::PriorityQueue;
+use crate::rayon::prelude::*;
 use std::collections::BTreeMap;
-use super::dual_module::EdgeWeightModifier;
-
 
 /// build complete graph out of skeleton graph using Dijkstra's algorithm
 #[derive(Debug, Clone)]
 pub struct CompleteGraph {
     /// number of vertices
     pub vertex_num: VertexNum,
     /// the vertices to run Dijkstra's algorithm
@@ -24,47 +24,57 @@
     /// all skeleton graph edges connected to this vertex
     pub edges: BTreeMap<VertexIndex, Weight>,
     /// timestamp for Dijkstra's algorithm
     timestamp: FastClearTimestamp,
 }
 
 impl CompleteGraph {
-
     /// create complete graph given skeleton graph
+    #[allow(clippy::unnecessary_cast)]
     pub fn new(vertex_num: VertexNum, weighted_edges: &[(VertexIndex, VertexIndex, Weight)]) -> Self {
-        let mut vertices: Vec<CompleteGraphVertex> = (0..vertex_num).map(|_| CompleteGraphVertex { edges: BTreeMap::new(), timestamp: 0, }).collect();
+        let mut vertices: Vec<CompleteGraphVertex> = (0..vertex_num)
+            .map(|_| CompleteGraphVertex {
+                edges: BTreeMap::new(),
+                timestamp: 0,
+            })
+            .collect();
         for &(i, j, weight) in weighted_edges.iter() {
             vertices[i as usize].edges.insert(j, weight);
             vertices[j as usize].edges.insert(i, weight);
         }
         Self {
             vertex_num,
             vertices,
             active_timestamp: 0,
             edge_modifier: EdgeWeightModifier::new(),
             weighted_edges: weighted_edges.to_owned(),
         }
     }
 
     /// reset any temporary changes like erasure edges
+    #[allow(clippy::unnecessary_cast)]
     pub fn reset(&mut self) {
         // recover erasure edges
         while self.edge_modifier.has_modified_edges() {
             let (edge_index, original_weight) = self.edge_modifier.pop_modified_edge();
             let (vertex_idx_1, vertex_idx_2, _) = &self.weighted_edges[edge_index as usize];
             let vertex_1 = &mut self.vertices[*vertex_idx_1 as usize];
-            assert_eq!(vertex_1.edges.insert(*vertex_idx_2, original_weight), Some(0), "previous weight should be 0");
+            vertex_1.edges.insert(*vertex_idx_2, original_weight);
             let vertex_2 = &mut self.vertices[*vertex_idx_2 as usize];
-            assert_eq!(vertex_2.edges.insert(*vertex_idx_1, original_weight), Some(0), "previous weight should be 0");
+            vertex_2.edges.insert(*vertex_idx_1, original_weight);
             self.weighted_edges[edge_index as usize] = (*vertex_idx_1, *vertex_idx_2, original_weight);
         }
     }
 
+    #[allow(clippy::unnecessary_cast)]
     fn load_edge_modifier(&mut self, edge_modifier: &[(EdgeIndex, Weight)]) {
-        assert!(!self.edge_modifier.has_modified_edges(), "the current erasure modifier is not clean, probably forget to clean the state?");
+        assert!(
+            !self.edge_modifier.has_modified_edges(),
+            "the current erasure modifier is not clean, probably forget to clean the state?"
+        );
         for (edge_index, target_weight) in edge_modifier.iter() {
             let (vertex_idx_1, vertex_idx_2, original_weight) = &self.weighted_edges[*edge_index as usize];
             let vertex_1 = &mut self.vertices[*vertex_idx_1 as usize];
             vertex_1.edges.insert(*vertex_idx_2, *target_weight);
             let vertex_2 = &mut self.vertices[*vertex_idx_2 as usize];
             vertex_2.edges.insert(*vertex_idx_1, *target_weight);
             self.edge_modifier.push_modified_edge(*edge_index, *original_weight);
@@ -74,68 +84,94 @@
 
     /// temporarily set some edges to 0 weight, and when it resets, those edges will be reverted back to the original weight
     pub fn load_erasures(&mut self, erasures: &[EdgeIndex]) {
         let edge_modifier: Vec<_> = erasures.iter().map(|edge_index| (*edge_index, 0)).collect();
         self.load_edge_modifier(&edge_modifier);
     }
 
+    pub fn load_dynamic_weights(&mut self, dynamic_weights: &[(EdgeIndex, Weight)]) {
+        let edge_modifier = dynamic_weights.to_vec();
+        self.load_edge_modifier(&edge_modifier);
+    }
+
     /// invalidate Dijkstra's algorithm state from previous call
+    #[allow(clippy::unnecessary_cast)]
     pub fn invalidate_previous_dijkstra(&mut self) -> usize {
-        if self.active_timestamp == FastClearTimestamp::MAX {  // rarely happens
+        if self.active_timestamp == FastClearTimestamp::MAX {
+            // rarely happens
             self.active_timestamp = 0;
             for i in 0..self.vertex_num {
-                self.vertices[i as usize].timestamp = 0;  // refresh all timestamps to avoid conflicts
+                self.vertices[i as usize].timestamp = 0; // refresh all timestamps to avoid conflicts
             }
         }
-        self.active_timestamp += 1;  // implicitly invalidate all vertices
+        self.active_timestamp += 1; // implicitly invalidate all vertices
         self.active_timestamp
     }
 
     /// get all complete graph edges from the specific vertex, but will terminate if `terminate` vertex is found
-    pub fn all_edges_with_terminate(&mut self, vertex: VertexIndex, terminate: VertexIndex) -> BTreeMap<VertexIndex, (VertexIndex, Weight)> {
+    #[allow(clippy::unnecessary_cast)]
+    pub fn all_edges_with_terminate(
+        &mut self,
+        vertex: VertexIndex,
+        terminate: VertexIndex,
+    ) -> BTreeMap<VertexIndex, (VertexIndex, Weight)> {
         let active_timestamp = self.invalidate_previous_dijkstra();
         let mut pq = PriorityQueue::<EdgeIndex, PriorityElement>::new();
         pq.push(vertex, PriorityElement::new(0, vertex));
-        let mut computed_edges = BTreeMap::<VertexIndex, (VertexIndex, Weight)>::new();  // { peer: (previous, weight) }
-        loop {  // until no more elements
+        let mut computed_edges = BTreeMap::<VertexIndex, (VertexIndex, Weight)>::new(); // { peer: (previous, weight) }
+        loop {
+            // until no more elements
             if pq.is_empty() {
-                break
+                break;
             }
             let (target, PriorityElement { weight, previous }) = pq.pop().unwrap();
             // eprintln!("target: {}, weight: {}, next: {}", target, weight, next);
             debug_assert!({
-                !computed_edges.contains_key(&target)  // this entry shouldn't have been set
+                !computed_edges.contains_key(&target) // this entry shouldn't have been set
             });
             // update entry
-            self.vertices[target as usize].timestamp = active_timestamp;  // mark as visited
+            self.vertices[target as usize].timestamp = active_timestamp; // mark as visited
             if target != vertex {
                 computed_edges.insert(target, (previous, weight));
                 if target == terminate {
-                    break  // early terminate
+                    break; // early terminate
                 }
             }
             // add its neighbors to priority queue
             for (&neighbor, &neighbor_weight) in self.vertices[target as usize].edges.iter() {
                 let edge_weight = weight + neighbor_weight;
-                if let Some(PriorityElement { weight: existing_weight, previous: existing_previous }) = pq.get_priority(&neighbor) {
+                if let Some(PriorityElement {
+                    weight: existing_weight,
+                    previous: existing_previous,
+                }) = pq.get_priority(&neighbor)
+                {
                     // update the priority if weight is smaller or weight is equal but distance is smaller
                     // this is necessary if the graph has weight-0 edges, which could lead to cycles in the graph and cause deadlock
                     let mut update = &edge_weight < existing_weight;
                     if &edge_weight == existing_weight {
-                        let distance = if neighbor > previous { neighbor - previous } else { previous - neighbor };
-                        let existing_distance = if &neighbor > existing_previous { neighbor - existing_previous } else { existing_previous - neighbor };
+                        let distance = if neighbor > previous {
+                            neighbor - previous
+                        } else {
+                            previous - neighbor
+                        };
+                        let existing_distance = if &neighbor > existing_previous {
+                            neighbor - existing_previous
+                        } else {
+                            existing_previous - neighbor
+                        };
                         // prevent loop by enforcing strong non-descending
                         if distance < existing_distance || (distance == existing_distance && &previous < existing_previous) {
                             update = true;
                         }
                     }
                     if update {
                         pq.change_priority(&neighbor, PriorityElement::new(edge_weight, target));
                     }
-                } else {  // insert new entry only if neighbor has not been visited
+                } else {
+                    // insert new entry only if neighbor has not been visited
                     if self.vertices[neighbor as usize].timestamp != active_timestamp {
                         pq.push(neighbor, PriorityElement::new(edge_weight, target));
                     }
                 }
             }
         }
         // println!("[debug] computed_edges: {:?}", computed_edges);
@@ -152,29 +188,140 @@
         assert_ne!(a, b, "cannot get path between the same vertex");
         let edges = self.all_edges_with_terminate(a, b);
         // println!("edges: {:?}", edges);
         let mut vertex = b;
         let mut path = Vec::new();
         loop {
             if vertex == a {
-                break
+                break;
             }
             let &(previous, weight) = &edges[&vertex];
             path.push((vertex, weight));
             if path.len() > 1 {
                 let previous_index = path.len() - 2;
                 path[previous_index].1 -= weight;
             }
             vertex = previous;
         }
         path.reverse();
         (path, edges[&b].1)
     }
 }
 
+#[derive(Clone)]
+pub struct PrebuiltCompleteGraph {
+    /// number of vertices
+    pub vertex_num: VertexNum,
+    /// all edge weights, if set to Weight::MAX then this edge does not exist
+    pub edges: Vec<BTreeMap<VertexIndex, Weight>>,
+    /// the virtual boundary weight
+    pub virtual_boundary_weight: Vec<Option<(VertexIndex, Weight)>>,
+}
+
+impl PrebuiltCompleteGraph {
+    #[allow(clippy::unnecessary_cast)]
+    pub fn new_threaded(initializer: &SolverInitializer, thread_pool_size: usize) -> Self {
+        let mut thread_pool_builder = rayon::ThreadPoolBuilder::new();
+        if thread_pool_size != 0 {
+            thread_pool_builder = thread_pool_builder.num_threads(thread_pool_size);
+        }
+        let thread_pool = thread_pool_builder.build().expect("creating thread pool failed");
+        let vertex_num = initializer.vertex_num as usize;
+        // first collect virtual vertices and real vertices
+        let mut is_virtual = vec![false; vertex_num];
+        for &virtual_vertex in initializer.virtual_vertices.iter() {
+            is_virtual[virtual_vertex as usize] = true;
+        }
+        type Result = (BTreeMap<VertexIndex, Weight>, Option<(VertexIndex, Weight)>);
+        let mut results: Vec<Result> = vec![];
+        thread_pool.scope(|_| {
+            (0..vertex_num)
+                .into_par_iter()
+                .map(|vertex_index| {
+                    let mut complete_graph = CompleteGraph::new(initializer.vertex_num, &initializer.weighted_edges);
+                    let mut edges = BTreeMap::new();
+                    let mut virtual_boundary_weight = None;
+                    if !is_virtual[vertex_index] {
+                        // only build graph for non-virtual vertices
+                        let complete_graph_edges = complete_graph.all_edges(vertex_index as VertexIndex);
+                        let mut boundary: Option<(VertexIndex, Weight)> = None;
+                        for (&peer, &(_, weight)) in complete_graph_edges.iter() {
+                            if !is_virtual[peer as usize] {
+                                edges.insert(peer, weight);
+                            }
+                            if is_virtual[peer as usize] && (boundary.is_none() || weight < boundary.as_ref().unwrap().1) {
+                                boundary = Some((peer, weight));
+                            }
+                        }
+                        virtual_boundary_weight = boundary;
+                    }
+                    (edges, virtual_boundary_weight)
+                })
+                .collect_into_vec(&mut results);
+        });
+        // optimization: remove edges in the middle
+        type UnzipResult = (Vec<BTreeMap<VertexIndex, Weight>>, Vec<Option<(VertexIndex, Weight)>>);
+        let (mut edges, virtual_boundary_weight): UnzipResult = results.into_iter().unzip();
+        let mut to_be_removed_vec: Vec<Vec<VertexIndex>> = vec![];
+        thread_pool.scope(|_| {
+            (0..vertex_num)
+                .into_par_iter()
+                .map(|vertex_index| {
+                    let mut to_be_removed = vec![];
+                    if !is_virtual[vertex_index] {
+                        for (&peer, &weight) in edges[vertex_index].iter() {
+                            let boundary_weight = if let Some((_, weight)) = virtual_boundary_weight[vertex_index as usize] {
+                                weight
+                            } else {
+                                Weight::MAX
+                            };
+                            let boundary_weight_peer = if let Some((_, weight)) = virtual_boundary_weight[peer as usize] {
+                                weight
+                            } else {
+                                Weight::MAX
+                            };
+                            if boundary_weight != Weight::MAX
+                                && boundary_weight_peer != Weight::MAX
+                                && weight > boundary_weight + boundary_weight_peer
+                            {
+                                to_be_removed.push(peer);
+                            }
+                        }
+                    }
+                    to_be_removed
+                })
+                .collect_into_vec(&mut to_be_removed_vec);
+        });
+        for vertex_index in 0..vertex_num {
+            for peer in to_be_removed_vec[vertex_index].iter() {
+                edges[vertex_index].remove(peer);
+            }
+        }
+        Self {
+            vertex_num: initializer.vertex_num,
+            edges,
+            virtual_boundary_weight,
+        }
+    }
+
+    pub fn new(initializer: &SolverInitializer) -> Self {
+        Self::new_threaded(initializer, 1)
+    }
+
+    #[allow(clippy::unnecessary_cast)]
+    pub fn get_edge_weight(&self, vertex_1: VertexIndex, vertex_2: VertexIndex) -> Option<Weight> {
+        self.edges[vertex_1 as usize].get(&vertex_2).cloned()
+    }
+
+    #[allow(clippy::unnecessary_cast)]
+    pub fn get_boundary_weight(&self, vertex_index: VertexIndex) -> Option<(VertexIndex, Weight)> {
+        self.virtual_boundary_weight[vertex_index as usize]
+    }
+}
+
 #[derive(Eq, Debug)]
 pub struct PriorityElement {
     pub weight: Weight,
     pub previous: VertexIndex,
 }
 
 impl std::cmp::PartialEq for PriorityElement {
@@ -183,26 +330,23 @@
         self.weight == other.weight
     }
 }
 
 impl std::cmp::PartialOrd for PriorityElement {
     #[inline]
     fn partial_cmp(&self, other: &PriorityElement) -> Option<std::cmp::Ordering> {
-        other.weight.partial_cmp(&self.weight)  // reverse `self` and `other` to prioritize smaller weight
+        other.weight.partial_cmp(&self.weight) // reverse `self` and `other` to prioritize smaller weight
     }
 }
 
 impl std::cmp::Ord for PriorityElement {
     #[inline]
     fn cmp(&self, other: &PriorityElement) -> std::cmp::Ordering {
-        other.weight.cmp(&self.weight)  // reverse `self` and `other` to prioritize smaller weight
+        other.weight.cmp(&self.weight) // reverse `self` and `other` to prioritize smaller weight
     }
 }
 
 impl PriorityElement {
     pub fn new(weight: Weight, previous: VertexIndex) -> Self {
-        Self {
-            weight,
-            previous,
-        }
+        Self { weight, previous }
     }
 }
```

### Comparing `fusion_blossom-0.2.2/src/dual_module.rs` & `fusion_blossom-0.2.5/src/dual_module.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 //! Dual Module
-//! 
+//!
 //! Generics for dual modules, defining the necessary interfaces for a dual module
 //!
 
+#![cfg_attr(feature = "unsafe_pointer", allow(dropping_references))]
+use super::pointers::*;
 use super::util::*;
-#[cfg(not(feature="dangerous_pointer"))]
-use std::sync::Arc;
+use super::visualize::*;
 use crate::derivative::Derivative;
 use core::cmp::Ordering;
 use std::collections::{BTreeMap, HashSet};
-use super::visualize::*;
-use super::pointers::*;
-
+#[cfg(not(feature = "dangerous_pointer"))]
+use std::sync::Arc;
 
 /// A dual node is either a blossom or a vertex
 #[derive(Derivative, Clone)]
 #[derivative(Debug)]
 pub enum DualNodeClass {
     Blossom {
         nodes_circle: Vec<DualNodeWeak>,
@@ -23,75 +23,77 @@
     },
     DefectVertex {
         defect_index: VertexIndex,
     },
 }
 
 impl DualNodeClass {
-    pub fn is_blossom(&self) -> bool { matches!(self, Self::Blossom{ .. }) }
+    pub fn is_blossom(&self) -> bool {
+        matches!(self, Self::Blossom { .. })
+    }
 }
 
 /// Three possible states: Grow (+1), Stay (+0), Shrink (-1)
 #[derive(Derivative, PartialEq, Eq, Clone, Copy)]
 #[derivative(Debug)]
 pub enum DualNodeGrowState {
     Grow,
     Stay,
     Shrink,
 }
 
 impl DualNodeGrowState {
-
     pub fn is_against(&self, other: &Self) -> bool {
-        matches!((self, other), (Self::Grow, Self::Grow | Self::Stay) | (Self::Stay, Self::Grow))
+        matches!(
+            (self, other),
+            (Self::Grow, Self::Grow | Self::Stay) | (Self::Stay, Self::Grow)
+        )
     }
-
 }
 
 /// synchronize request on vertices, when a vertex is mirrored
 #[derive(Derivative)]
 #[derivative(Debug)]
 pub struct SyncRequest {
     /// the unit that owns this vertex
     pub mirror_unit_weak: PartitionUnitWeak,
     /// the vertex index to be synchronized
     pub vertex_index: VertexIndex,
     /// propagated dual node index and the dual variable of the propagated dual node;
-    /// this field is necessary to differentiate between normal shrink and the one that needs to report VertexShrinkStop event, when the syndrome is on the interface
-    pub propagated_dual_node: Option<(DualNodeWeak, Weight)>,
+    /// this field is necessary to differentiate between normal shrink and the one that needs to report VertexShrinkStop event, when the syndrome is on the interface;
+    /// it also includes the representative vertex of the dual node, so that parents can keep track of whether it should be elevated
+    pub propagated_dual_node: Option<(DualNodeWeak, Weight, VertexIndex)>,
     /// propagated grandson node: must be a syndrome node
-    pub propagated_grandson_dual_node: Option<(DualNodeWeak, Weight)>,
+    pub propagated_grandson_dual_node: Option<(DualNodeWeak, Weight, VertexIndex)>,
 }
 
 impl SyncRequest {
-
     /// update all the interface nodes to be up-to-date, only necessary when there are fusion
     pub fn update(&self) {
-        if let Some((weak, _)) = &self.propagated_dual_node {
+        if let Some((weak, ..)) = &self.propagated_dual_node {
             weak.upgrade_force().update();
         }
-        if let Some((weak, _)) = &self.propagated_grandson_dual_node {
+        if let Some((weak, ..)) = &self.propagated_grandson_dual_node {
             weak.upgrade_force().update();
         }
     }
-
 }
 
 /// gives the maximum absolute length to grow, if not possible, give the reason;
 /// note that strong reference is stored in `MaxUpdateLength` so dropping these temporary messages are necessary to avoid memory leakage;
 /// the strong reference is required when multiple `BlossomNeedExpand` event is reported in different partitions and sorting them requires a reference
 #[derive(Derivative, PartialEq, Eq, Clone)]
 #[derivative(Debug)]
 pub enum MaxUpdateLength {
     /// non-zero maximum update length, has_empty_boundary_node (useful in fusion)
     NonZeroGrow((Weight, bool)),
     /// conflicting growth
-    Conflicting((DualNodePtr, DualNodePtr), (DualNodePtr, DualNodePtr)),  // (node_1, touching_1), (node_2, touching_2)
+    Conflicting((DualNodePtr, DualNodePtr), (DualNodePtr, DualNodePtr)), // (node_1, touching_1), (node_2, touching_2)
     /// conflicting growth because of touching virtual node
-    TouchingVirtual((DualNodePtr, DualNodePtr), (VertexIndex, bool)),  // (node, touching), (virtual_vertex, is_mirror)
+    TouchingVirtual((DualNodePtr, DualNodePtr), (VertexIndex, bool)), // (node, touching), (virtual_vertex, is_mirror)
     /// blossom hitting 0 dual variable while shrinking
     BlossomNeedExpand(DualNodePtr),
     /// node hitting 0 dual variable while shrinking: note that this should have the lowest priority, normally it won't show up in a normal primal module;
     /// in case that the dual module is partitioned and nobody can report this conflicting event, one needs to embed the potential conflicts using the second
     /// argument so that dual module can gather two `VertexShrinkStop` events to form a single `Conflicting` event
     VertexShrinkStop((DualNodePtr, Option<(DualNodePtr, DualNodePtr)>)),
 }
@@ -117,15 +119,14 @@
 impl Default for GroupMaxUpdateLength {
     fn default() -> Self {
         Self::new()
     }
 }
 
 impl GroupMaxUpdateLength {
-
     pub fn new() -> Self {
         Self::NonZeroGrow((Weight::MAX, false))
     }
 
     /// update all the interface nodes to be up-to-date, only necessary in existence of fusion
     #[inline(never)]
     pub fn update(&self) {
@@ -135,27 +136,33 @@
             }
             for (_, max_update_length) in pending_stops.iter() {
                 max_update_length.update();
             }
         }
     }
 
-    pub fn add_pending_stop(list: &mut ConflictList, pending_stops: &mut BTreeMap<VertexIndex, MaxUpdateLength>, max_update_length: MaxUpdateLength) {
+    pub fn add_pending_stop(
+        list: &mut ConflictList,
+        pending_stops: &mut BTreeMap<VertexIndex, MaxUpdateLength>,
+        max_update_length: MaxUpdateLength,
+    ) {
         if let Some(dual_node_ptr) = max_update_length.get_vertex_shrink_stop() {
             let vertex_index = dual_node_ptr.get_representative_vertex();
             if let Some(existing_length) = pending_stops.get(&vertex_index) {
-                if let MaxUpdateLength::VertexShrinkStop((_, Some(weak_pair))) = &max_update_length {  // otherwise don't update
+                if let MaxUpdateLength::VertexShrinkStop((_, Some(weak_pair))) = &max_update_length {
+                    // otherwise don't update
                     if let MaxUpdateLength::VertexShrinkStop((_, Some(existing_weak_pair))) = existing_length {
                         if weak_pair.0 != existing_weak_pair.0 {
                             // two such conflicts form a Conflicting event
                             list.push(MaxUpdateLength::Conflicting(weak_pair.clone(), existing_weak_pair.clone()));
                             pending_stops.remove(&vertex_index);
                         }
                     } else {
-                        pending_stops.insert(vertex_index, max_update_length.clone());  // update the entry
+                        pending_stops.insert(vertex_index, max_update_length.clone());
+                        // update the entry
                     }
                 }
             } else {
                 pending_stops.insert(vertex_index, max_update_length);
             }
         } else {
             list.push(max_update_length);
@@ -163,117 +170,122 @@
     }
 
     pub fn add(&mut self, max_update_length: MaxUpdateLength) {
         match self {
             Self::NonZeroGrow((current_length, current_has_empty_boundary_node)) => {
                 if let MaxUpdateLength::NonZeroGrow((length, has_empty_boundary_node)) = max_update_length {
                     *current_length = std::cmp::min(*current_length, length);
-                    *current_has_empty_boundary_node |= has_empty_boundary_node;  // or
+                    *current_has_empty_boundary_node |= has_empty_boundary_node;
+                // or
                 } else {
                     let mut list = ConflictList::new();
                     let mut pending_stops = BTreeMap::new();
                     if let Some(dual_node_ptr) = max_update_length.get_vertex_shrink_stop() {
                         let vertex_index = dual_node_ptr.get_representative_vertex();
                         pending_stops.insert(vertex_index, max_update_length);
                     } else {
                         list.push(max_update_length);
                     }
                     *self = Self::Conflicts((list, pending_stops));
                 }
-            },
+            }
             Self::Conflicts((list, pending_stops)) => {
                 // only add conflicts, not NonZeroGrow
                 if !matches!(max_update_length, MaxUpdateLength::NonZeroGrow(_)) {
                     Self::add_pending_stop(list, pending_stops, max_update_length);
                 }
-            },
+            }
         }
     }
 
     pub fn extend(&mut self, other: Self) {
         if other.is_empty() {
-            return  // do nothing
+            return; // do nothing
         }
         match self {
-            Self::NonZeroGrow(current_length) => {
-                match other {
-                    Self::NonZeroGrow(length) => {
-                        *current_length = std::cmp::min(*current_length, length);
-                    },
-                    Self::Conflicts((mut other_list, mut other_pending_stops)) => {
-                        let mut list = ConflictList::new();
-                        let mut pending_stops = BTreeMap::new();
-                        std::mem::swap(&mut list, &mut other_list);
-                        std::mem::swap(&mut pending_stops, &mut other_pending_stops);
-                        *self = Self::Conflicts((list, pending_stops));
-                    },
+            Self::NonZeroGrow(current_length) => match other {
+                Self::NonZeroGrow(length) => {
+                    *current_length = std::cmp::min(*current_length, length);
+                }
+                Self::Conflicts((mut other_list, mut other_pending_stops)) => {
+                    let mut list = ConflictList::new();
+                    let mut pending_stops = BTreeMap::new();
+                    std::mem::swap(&mut list, &mut other_list);
+                    std::mem::swap(&mut pending_stops, &mut other_pending_stops);
+                    *self = Self::Conflicts((list, pending_stops));
                 }
             },
             Self::Conflicts((list, pending_stops)) => {
                 if let Self::Conflicts((other_list, other_pending_stops)) = other {
                     list.extend(other_list.into_iter());
                     for (_, max_update_length) in other_pending_stops.into_iter() {
                         Self::add_pending_stop(list, pending_stops, max_update_length);
                     }
-                }  // only add conflicts, not NonZeroGrow
-            },
+                } // only add conflicts, not NonZeroGrow
+            }
         }
     }
 
     pub fn is_empty(&self) -> bool {
-        matches!(self, Self::NonZeroGrow((Weight::MAX, _)))  // if `has_empty_boundary_node`, then it's not considered empty
+        matches!(self, Self::NonZeroGrow((Weight::MAX, _))) // if `has_empty_boundary_node`, then it's not considered empty
     }
 
     pub fn is_active(&self) -> bool {
-        !matches!(self, Self::NonZeroGrow((Weight::MAX, false)))  // if `has_empty_boundary_node`, then it's still considered active
+        !matches!(self, Self::NonZeroGrow((Weight::MAX, false))) // if `has_empty_boundary_node`, then it's still considered active
     }
 
     pub fn get_none_zero_growth(&self) -> Option<Weight> {
         match self {
             Self::NonZeroGrow((length, _has_empty_boundary_node)) => {
-                debug_assert!(*length != Weight::MAX, "please call GroupMaxUpdateLength::is_empty to check if this group is empty");
+                debug_assert!(
+                    *length != Weight::MAX,
+                    "please call GroupMaxUpdateLength::is_empty to check if this group is empty"
+                );
                 Some(*length)
-            },
-            _ => { None }
+            }
+            _ => None,
         }
     }
 
     pub fn pop(&mut self) -> Option<MaxUpdateLength> {
         match self {
             Self::NonZeroGrow(_) => {
                 panic!("please call GroupMaxUpdateLength::get_none_zero_growth to check if this group is none_zero_growth");
-            },
+            }
             Self::Conflicts((list, pending_stops)) => {
                 list.pop().or(if let Some(key) = pending_stops.keys().next().cloned() {
                     pending_stops.remove(&key)
                 } else {
                     None
                 })
             }
         }
     }
 
     pub fn peek(&self) -> Option<&MaxUpdateLength> {
         match self {
             Self::NonZeroGrow(_) => {
                 panic!("please call GroupMaxUpdateLength::get_none_zero_growth to check if this group is none_zero_growth");
-            },
+            }
             Self::Conflicts((list, pending_stops)) => {
                 cfg_if::cfg_if! {
                     if #[cfg(feature="ordered_conflicts")] {
                         let peek_element = list.peek();
                     } else {
                         let peek_element = list.last();
                     }
                 }
-                peek_element.or(if pending_stops.is_empty() { None } else { pending_stops.values().next() })
+                peek_element.or(if pending_stops.is_empty() {
+                    None
+                } else {
+                    pending_stops.values().next()
+                })
             }
         }
     }
-
 }
 
 /// A dual node corresponds to either a vertex or a blossom (on which the dual variables are defined)
 #[derive(Derivative, Clone)]
 #[derivative(Debug)]
 pub struct DualNode {
     /// the index of this dual node, helps to locate internal details of this dual node
@@ -281,31 +293,31 @@
     /// the class of this dual node
     pub class: DualNodeClass,
     /// whether it grows, stays or shrinks
     pub grow_state: DualNodeGrowState,
     /// parent blossom: when parent exists, grow_state should be [`DualNodeGrowState::Stay`]
     pub parent_blossom: Option<DualNodeWeak>,
     /// information used to compute dual variable of this node: (last dual variable, last global progress)
-    dual_variable_cache: (Weight, Weight),
+    pub dual_variable_cache: (Weight, Weight),
     /// belonging of the dual module interface; a dual node is never standalone
     pub belonging: DualModuleInterfaceWeak,
 }
 
 impl DualNode {
-
     /// get the current dual variable of a node
     pub fn get_dual_variable(&self, interface: &DualModuleInterface) -> Weight {
         let (last_dual_variable, last_global_progress) = self.dual_variable_cache;
         match self.grow_state {
             DualNodeGrowState::Grow => last_dual_variable + (interface.dual_variable_global_progress - last_global_progress),
             DualNodeGrowState::Stay => last_dual_variable,
-            DualNodeGrowState::Shrink => last_dual_variable - (interface.dual_variable_global_progress - last_global_progress),
+            DualNodeGrowState::Shrink => {
+                last_dual_variable - (interface.dual_variable_global_progress - last_global_progress)
+            }
         }
     }
-
 }
 
 // should not use dangerous pointer because expanding a blossom will leave a weak pointer invalid
 pub type DualNodePtr = ArcManualSafeLock<DualNode>;
 pub type DualNodeWeak = WeakManualSafeLock<DualNode>;
 
 impl Ord for DualNodePtr {
@@ -337,39 +349,38 @@
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         Some(self.cmp(other))
     }
 }
 
 impl std::fmt::Debug for DualNodePtr {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
-        self.update();  // to make sure index is up-to-date
-        let dual_node = self.read_recursive();  // reading index is consistent
+        self.update(); // to make sure index is up-to-date
+        let dual_node = self.read_recursive(); // reading index is consistent
         write!(f, "{}", dual_node.index)
     }
 }
 
 impl std::fmt::Debug for DualNodeWeak {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         self.upgrade_force().fmt(f)
     }
 }
 
 impl DualNodePtr {
-
     /// when fused, dual node may be outdated; refresh here
     pub fn update(&self) -> &Self {
         let mut current_belonging = self.read_recursive().belonging.upgrade_force();
         let mut bias = 0;
         let mut node = self.write();
         while current_belonging.read_recursive().parent.is_some() {
             let belonging_interface = current_belonging.read_recursive();
             bias += belonging_interface.index_bias;
             let new_current_belonging = belonging_interface.parent.clone().unwrap().upgrade_force();
-            let dual_variable = node.get_dual_variable(&belonging_interface);  // aggregate the dual variable
-            node.dual_variable_cache = (dual_variable, 0);  // this will be the state when joining the new interface
+            let dual_variable = node.get_dual_variable(&belonging_interface); // aggregate the dual variable
+            node.dual_variable_cache = (dual_variable, 0); // this will be the state when joining the new interface
             drop(belonging_interface);
             current_belonging = new_current_belonging;
         }
         node.belonging = current_belonging.downgrade();
         node.index += bias;
         self
     }
@@ -378,15 +389,18 @@
         self.update();
         self.read_recursive().index
     }
 
     /// helper function to set grow state with sanity check
     fn set_grow_state(&self, grow_state: DualNodeGrowState) {
         let mut dual_node = self.write();
-        debug_assert!(dual_node.parent_blossom.is_none(), "setting node grow state inside a blossom forbidden");
+        debug_assert!(
+            dual_node.parent_blossom.is_none(),
+            "setting node grow state inside a blossom forbidden"
+        );
         dual_node.grow_state = grow_state;
     }
 
     /// get parent blossom recursively
     pub fn get_ancestor_blossom(&self) -> DualNodePtr {
         let dual_node = self.read_recursive();
         match &dual_node.parent_blossom {
@@ -394,38 +408,45 @@
             None => self.clone(),
         }
     }
 
     /// get the parent blossom before the most parent one, useful when expanding a blossom
     pub fn get_secondary_ancestor_blossom(&self) -> DualNodePtr {
         let mut secondary_ancestor = self.clone();
-        let mut ancestor = self.read_recursive().parent_blossom.as_ref().expect("secondary ancestor does not exist").upgrade_force();
+        let mut ancestor = self
+            .read_recursive()
+            .parent_blossom
+            .as_ref()
+            .expect("secondary ancestor does not exist")
+            .upgrade_force();
         loop {
             let dual_node = ancestor.read_recursive();
             let new_ancestor = match &dual_node.parent_blossom {
                 Some(weak) => weak.upgrade_force(),
-                None => { return secondary_ancestor; },
+                None => {
+                    return secondary_ancestor;
+                }
             };
             drop(dual_node);
             secondary_ancestor = ancestor.clone();
             ancestor = new_ancestor;
         }
     }
 
     fn __get_all_vertices(&self, pending_vec: &mut Vec<VertexIndex>) {
         let dual_node = self.read_recursive();
         match &dual_node.class {
             DualNodeClass::Blossom { nodes_circle, .. } => {
                 for node_ptr in nodes_circle.iter() {
                     node_ptr.upgrade_force().__get_all_vertices(pending_vec);
                 }
-            },
+            }
             DualNodeClass::DefectVertex { defect_index } => {
                 pending_vec.push(*defect_index);
-            },
+            }
         };
     }
 
     /// find all vertices that belongs to the dual node, i.e. any vertices inside a blossom
     pub fn get_all_vertices(&self) -> Vec<VertexIndex> {
         let mut pending_vec = vec![];
         self.__get_all_vertices(&mut pending_vec);
@@ -436,15 +457,14 @@
     pub fn get_representative_vertex(&self) -> VertexIndex {
         let dual_node = self.read_recursive();
         match &dual_node.class {
             DualNodeClass::Blossom { nodes_circle, .. } => nodes_circle[0].upgrade_force().get_representative_vertex(),
             DualNodeClass::DefectVertex { defect_index } => *defect_index,
         }
     }
-
 }
 
 /// a sharable array of dual nodes, supporting dynamic partitioning;
 /// note that a node can be destructed and we do not reuse its index, leaving a blank space
 #[derive(Derivative)]
 #[derivative(Debug)]
 pub struct DualModuleInterface {
@@ -489,56 +509,66 @@
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         self.upgrade_force().fmt(f)
     }
 }
 
 /// common trait that must be implemented for each implementation of dual module
 pub trait DualModuleImpl {
-
     /// create a new dual module with empty syndrome
     fn new_empty(initializer: &SolverInitializer) -> Self;
 
     /// clear all growth and existing dual nodes, prepared for the next decoding
     fn clear(&mut self);
 
     /// add corresponding dual node
     fn add_dual_node(&mut self, dual_node_ptr: &DualNodePtr);
 
     #[inline(always)]
     /// helper function to specifically add a syndrome node
     fn add_defect_node(&mut self, dual_node_ptr: &DualNodePtr) {
-        debug_assert!({
-            let node = dual_node_ptr.read_recursive();
-            matches!(node.class, DualNodeClass::DefectVertex{ .. })
-        }, "node class mismatch");
+        debug_assert!(
+            {
+                let node = dual_node_ptr.read_recursive();
+                matches!(node.class, DualNodeClass::DefectVertex { .. })
+            },
+            "node class mismatch"
+        );
         self.add_dual_node(dual_node_ptr)
     }
 
     #[inline(always)]
     /// helper function to specifically add a blossom node
     fn add_blossom(&mut self, dual_node_ptr: &DualNodePtr) {
-        debug_assert!({
-            let node = dual_node_ptr.read_recursive();
-            matches!(node.class, DualNodeClass::Blossom{ .. })
-        }, "node class mismatch");
+        debug_assert!(
+            {
+                let node = dual_node_ptr.read_recursive();
+                matches!(node.class, DualNodeClass::Blossom { .. })
+            },
+            "node class mismatch"
+        );
         self.add_dual_node(dual_node_ptr)
     }
 
     /// remove a blossom, note that this dual node ptr is already expanded from the root: normally you only need to remove this blossom;
     /// when force flag is set, remove blossom even if its dual variable is not 0: this action cannot be undone
     fn remove_blossom(&mut self, dual_node_ptr: DualNodePtr);
 
     /// update grow state
     fn set_grow_state(&mut self, dual_node_ptr: &DualNodePtr, grow_state: DualNodeGrowState);
 
     /// An optional function that helps to break down the implementation of [`DualModuleImpl::compute_maximum_update_length`]
     /// check the maximum length to grow (shrink) specific dual node, if length is 0, give the reason of why it cannot further grow (shrink).
     /// if `is_grow` is false, return `length` <= 0, in any case |`length`| is maximized so that at least one edge becomes fully grown or fully not-grown.
     /// if `simultaneous_update` is true, also check for the peer node according to [`DualNode::grow_state`].
-    fn compute_maximum_update_length_dual_node(&mut self, _dual_node_ptr: &DualNodePtr, _is_grow: bool, _simultaneous_update: bool) -> MaxUpdateLength {
+    fn compute_maximum_update_length_dual_node(
+        &mut self,
+        _dual_node_ptr: &DualNodePtr,
+        _is_grow: bool,
+        _simultaneous_update: bool,
+    ) -> MaxUpdateLength {
         panic!("the dual module implementation doesn't support this function, please use another dual module")
     }
 
     /// check the maximum length to grow (shrink) for all nodes, return a list of conflicting reason and a single number indicating the maximum length to grow:
     /// this number will be 0 if any conflicting reason presents
     fn compute_maximum_update_length(&mut self) -> GroupMaxUpdateLength;
 
@@ -550,37 +580,49 @@
     /// grow a specific length globally, length must be positive.
     /// note that reversing the process is possible, but not recommended: to do that, reverse the state of each dual node, Grow->Shrink, Shrink->Grow
     fn grow(&mut self, length: Weight);
 
     /// optional support for edge modifier. for example, erasure errors temporarily set some edges to 0 weight.
     /// When it clears, those edges must be reverted back to the original weight
     fn load_edge_modifier(&mut self, _edge_modifier: &[(EdgeIndex, Weight)]) {
-        unimplemented!("load_edge_modifier is an optional interface, and the current dual module implementation doesn't support it");
+        unimplemented!(
+            "load_edge_modifier is an optional interface, and the current dual module implementation doesn't support it"
+        );
     }
 
     /// an erasure error means this edge is totally uncertain: p=0.5, so new weight = ln((1-p)/p) = 0
     fn load_erasures(&mut self, erasures: &[EdgeIndex]) {
         let edge_modifier: Vec<_> = erasures.iter().map(|edge_index| (*edge_index, 0)).collect();
         self.load_edge_modifier(&edge_modifier);
     }
 
+    fn load_dynamic_weights(&mut self, dynamic_weights: &[(EdgeIndex, Weight)]) {
+        let edge_modifier = dynamic_weights.to_vec();
+        self.load_edge_modifier(&edge_modifier);
+    }
+
     /// prepare a list of nodes as shrinking state; useful in creating a blossom
     fn prepare_nodes_shrink(&mut self, _nodes_circle: &[DualNodePtr]) -> &mut Vec<SyncRequest> {
         panic!("the dual module implementation doesn't support this function, please use another dual module")
     }
 
     /// performance profiler report
-    fn generate_profiler_report(&self) -> serde_json::Value { json!({}) }
+    fn generate_profiler_report(&self) -> serde_json::Value {
+        json!({})
+    }
 
     /*
      * the following apis are only required when this dual module can be used as a partitioned one
      */
 
     /// create a partitioned dual module (hosting only a subgraph and subset of dual nodes) to be used in the parallel dual module
-    fn new_partitioned(_partitioned_initializer: &PartitionedSolverInitializer) -> Self where Self: std::marker::Sized {
+    fn new_partitioned(_partitioned_initializer: &PartitionedSolverInitializer) -> Self
+    where
+        Self: std::marker::Sized,
+    {
         panic!("the dual module implementation doesn't support this function, please use another dual module")
     }
 
     /// prepare the growing or shrinking state of all nodes and return a list of sync requests in case of mirrored vertices are changed
     fn prepare_all(&mut self) -> &mut Vec<SyncRequest> {
         panic!("the dual module implementation doesn't support this function, please use another dual module")
     }
@@ -595,39 +637,36 @@
         panic!("the dual module implementation doesn't support this function, please use another dual module")
     }
 
     /// judge whether the current module hosts any of these dual node
     fn contains_dual_nodes_any(&self, dual_node_ptrs: &[DualNodePtr]) -> bool {
         for dual_node_ptr in dual_node_ptrs.iter() {
             if self.contains_dual_node(dual_node_ptr) {
-                return true
+                return true;
             }
         }
         false
     }
 
     /// judge whether the current module hosts a vertex
     fn contains_vertex(&self, _vertex_index: VertexIndex) -> bool {
         panic!("the dual module implementation doesn't support this function, please use another dual module")
     }
 
     /// bias the global dual node indices
     fn bias_dual_node_index(&mut self, _bias: NodeIndex) {
         panic!("the dual module implementation doesn't support this function, please use another dual module")
     }
-
 }
 
 /// this dual module is a parallel version that hosts many partitioned ones
 pub trait DualModuleParallelImpl {
-
     type UnitType: DualModuleImpl + Send + Sync;
 
     fn get_unit(&self, unit_index: usize) -> ArcManualSafeLock<Self::UnitType>;
-
 }
 
 impl FusionVisualizer for DualModuleInterfacePtr {
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         // do the sanity check first before taking snapshot
         let flattened_nodes = self.sanity_check().unwrap();
         let interface = self.read_recursive();
@@ -673,68 +712,73 @@
             },
             "dual_nodes": dual_nodes,
         })
     }
 }
 
 impl DualModuleInterface {
-
     /// return the count of all nodes including those of the children interfaces
     pub fn nodes_count(&self) -> NodeNum {
         let mut count = self.nodes_length as NodeNum;
         if let Some(((_, left_count), (_, right_count))) = &self.children {
             count += left_count + right_count;
         }
         count
     }
 
     /// get node ptr by index; if calling from the ancestor interface, node_index is absolute, otherwise it's relative
+    #[allow(clippy::unnecessary_cast)]
     pub fn get_node(&self, relative_node_index: NodeIndex) -> Option<DualNodePtr> {
         debug_assert!(relative_node_index < self.nodes_count(), "cannot find node in this interface");
         let mut bias = 0;
         if let Some(((left_weak, left_count), (right_weak, right_count))) = &self.children {
             if relative_node_index < *left_count {
                 // this node belongs to the left
                 return left_weak.upgrade_force().read_recursive().get_node(relative_node_index);
             } else if relative_node_index < *left_count + *right_count {
                 // this node belongs to the right
-                return right_weak.upgrade_force().read_recursive().get_node(relative_node_index - *left_count);
+                return right_weak
+                    .upgrade_force()
+                    .read_recursive()
+                    .get_node(relative_node_index - *left_count);
             }
             bias = left_count + right_count;
         }
         self.nodes[(relative_node_index - bias) as usize].clone()
     }
 
     /// set the corresponding node index to None
+    #[allow(clippy::unnecessary_cast)]
     pub fn remove_node(&mut self, relative_node_index: NodeIndex) {
         debug_assert!(relative_node_index < self.nodes_count(), "cannot find node in this interface");
         let mut bias = 0;
         if let Some(((left_weak, left_count), (right_weak, right_count))) = &self.children {
             if relative_node_index < *left_count {
                 // this node belongs to the left
                 left_weak.upgrade_force().write().remove_node(relative_node_index);
-                return
+                return;
             } else if relative_node_index < *left_count + *right_count {
                 // this node belongs to the right
-                right_weak.upgrade_force().write().remove_node(relative_node_index - *left_count);
-                return
+                right_weak
+                    .upgrade_force()
+                    .write()
+                    .remove_node(relative_node_index - *left_count);
+                return;
             }
             bias = left_count + right_count;
         }
         self.nodes[(relative_node_index - bias) as usize] = None;
     }
-
 }
 
 impl DualModuleInterfacePtr {
-
     /// create an empty interface
     pub fn new_empty() -> Self {
         Self::new_value(DualModuleInterface {
-            unit_index: 0,  // if necessary, manually change it
+            unit_index: 0, // if necessary, manually change it
             nodes: Vec::new(),
             nodes_length: 0,
             is_fusion: false,
             sum_grow_speed: 0,
             sum_dual_variables: 0,
             debug_print_actions: false,
             dual_variable_global_progress: 0,
@@ -752,16 +796,23 @@
     }
 
     pub fn load(&self, syndrome_pattern: &SyndromePattern, dual_module_impl: &mut impl DualModuleImpl) {
         for vertex_idx in syndrome_pattern.defect_vertices.iter() {
             self.create_defect_node(*vertex_idx, dual_module_impl);
         }
         if !syndrome_pattern.erasures.is_empty() {
+            assert!(
+                syndrome_pattern.dynamic_weights.is_empty(),
+                "erasures and dynamic_weights cannot be provided at the same time"
+            );
             dual_module_impl.load_erasures(&syndrome_pattern.erasures);
         }
+        if !syndrome_pattern.dynamic_weights.is_empty() {
+            dual_module_impl.load_dynamic_weights(&syndrome_pattern.dynamic_weights);
+        }
     }
 
     /// a constant clear function, without dropping anything;
     /// this is for consideration of reducing the garbage collection time in the parallel solver,
     /// by distributing the clear cost into each thread but not the single main thread.
     pub fn clear(&self) {
         let mut interface = self.write();
@@ -787,25 +838,31 @@
         for node_index in 0..interface.nodes_length {
             let dual_node_ptr = &interface.nodes[node_index];
             if let Some(dual_node_ptr) = dual_node_ptr {
                 dual_node_ptr.update();
             }
             flattened_nodes.push(dual_node_ptr.clone());
         }
-        debug_assert_eq!(flattened_nodes.len() as NodeNum - flattened_nodes_length, interface.nodes_count());
+        debug_assert_eq!(
+            flattened_nodes.len() as NodeNum - flattened_nodes_length,
+            interface.nodes_count()
+        );
     }
 
     pub fn create_defect_node(&self, vertex_idx: VertexIndex, dual_module_impl: &mut impl DualModuleImpl) -> DualNodePtr {
         let belonging = self.downgrade();
         let mut interface = self.write();
         interface.sum_grow_speed += 1;
         let local_node_index = interface.nodes_length;
         let node_index = interface.nodes_count();
         // try to reuse existing pointer to avoid list allocation
-        let node_ptr = if !interface.is_fusion && local_node_index < interface.nodes.len() && interface.nodes[local_node_index].is_some() {
+        let node_ptr = if !interface.is_fusion
+            && local_node_index < interface.nodes.len()
+            && interface.nodes[local_node_index].is_some()
+        {
             let node_ptr = interface.nodes[local_node_index].take().unwrap();
             let mut node = node_ptr.write();
             node.index = node_index;
             node.class = DualNodeClass::DefectVertex {
                 defect_index: vertex_idx,
             };
             node.grow_state = DualNodeGrowState::Grow;
@@ -827,45 +884,55 @@
             })
         };
         interface.nodes_length += 1;
         if interface.nodes.len() < interface.nodes_length {
             interface.nodes.push(None);
         }
         let cloned_node_ptr = node_ptr.clone();
-        interface.nodes[local_node_index] = Some(node_ptr);  // feature `dangerous_pointer`: must push the owner
+        interface.nodes[local_node_index] = Some(node_ptr); // feature `dangerous_pointer`: must push the owner
         drop(interface);
         dual_module_impl.add_defect_node(&cloned_node_ptr);
         cloned_node_ptr
     }
 
     /// check whether a pointer belongs to this node, it will acquire a reader lock on `dual_node_ptr`
     pub fn check_ptr_belonging(&self, dual_node_ptr: &DualNodePtr) -> bool {
         let interface = self.read_recursive();
         let dual_node = dual_node_ptr.read_recursive();
-        if dual_node.index >= interface.nodes_count() { return false }
+        if dual_node.index >= interface.nodes_count() {
+            return false;
+        }
         if let Some(ptr) = interface.get_node(dual_node.index).as_ref() {
             ptr == dual_node_ptr
         } else {
             false
         }
     }
 
     /// create a dual node corresponding to a blossom, automatically set the grow state of internal nodes;
     /// the nodes circle MUST starts with a growing node and ends with a shrinking node
-    pub fn create_blossom(&self, nodes_circle: Vec<DualNodePtr>, mut touching_children: Vec<(DualNodeWeak, DualNodeWeak)>
-            , dual_module_impl: &mut impl DualModuleImpl) -> DualNodePtr {
+    pub fn create_blossom(
+        &self,
+        nodes_circle: Vec<DualNodePtr>,
+        mut touching_children: Vec<(DualNodeWeak, DualNodeWeak)>,
+        dual_module_impl: &mut impl DualModuleImpl,
+    ) -> DualNodePtr {
         let belonging = self.downgrade();
         let mut interface = self.write();
-        if touching_children.is_empty() {  // automatically fill the children, only works when nodes_circle consists of all syndrome nodes
+        if touching_children.is_empty() {
+            // automatically fill the children, only works when nodes_circle consists of all syndrome nodes
             touching_children = nodes_circle.iter().map(|ptr| (ptr.downgrade(), ptr.downgrade())).collect();
         }
         debug_assert_eq!(touching_children.len(), nodes_circle.len(), "circle length mismatch");
         let local_node_index = interface.nodes_length;
         let node_index = interface.nodes_count();
-        let blossom_node_ptr = if !interface.is_fusion && local_node_index < interface.nodes.len() && interface.nodes[local_node_index].is_some() {
+        let blossom_node_ptr = if !interface.is_fusion
+            && local_node_index < interface.nodes.len()
+            && interface.nodes[local_node_index].is_some()
+        {
             let node_ptr = interface.nodes[local_node_index].take().unwrap();
             let mut node = node_ptr.write();
             node.index = node_index;
             node.class = DualNodeClass::Blossom {
                 nodes_circle: vec![],
                 touching_children: vec![],
             };
@@ -886,43 +953,57 @@
                 parent_blossom: None,
                 dual_variable_cache: (0, interface.dual_variable_global_progress),
                 belonging,
             })
         };
         drop(interface);
         for (i, node_ptr) in nodes_circle.iter().enumerate() {
-            debug_assert!(self.check_ptr_belonging(node_ptr), "this ptr doesn't belong to this interface");
+            debug_assert!(
+                self.check_ptr_belonging(node_ptr),
+                "this ptr doesn't belong to this interface"
+            );
             let node = node_ptr.read_recursive();
-            debug_assert!(node.parent_blossom.is_none(), "cannot create blossom on a node that already belongs to a blossom");
-            debug_assert!(&node.grow_state == (if i % 2 == 0 { &DualNodeGrowState::Grow } else { &DualNodeGrowState::Shrink })
-                , "the nodes circle MUST starts with a growing node and ends with a shrinking node");
+            debug_assert!(
+                node.parent_blossom.is_none(),
+                "cannot create blossom on a node that already belongs to a blossom"
+            );
+            debug_assert!(
+                &node.grow_state
+                    == (if i % 2 == 0 {
+                        &DualNodeGrowState::Grow
+                    } else {
+                        &DualNodeGrowState::Shrink
+                    }),
+                "the nodes circle MUST starts with a growing node and ends with a shrinking node"
+            );
             drop(node);
             // set state must happen before setting parent
             self.set_grow_state(node_ptr, DualNodeGrowState::Stay, dual_module_impl);
             // then update parent
             let mut node = node_ptr.write();
             node.parent_blossom = Some(blossom_node_ptr.downgrade());
         }
         let mut interface = self.write();
         if interface.debug_print_actions {
             eprintln!("[create blossom] {:?} -> {}", nodes_circle, node_index);
         }
         let cloned_blossom_node_ptr = blossom_node_ptr.clone();
-        {  // fill in the nodes because they're in a valid state (all linked to this blossom)
+        {
+            // fill in the nodes because they're in a valid state (all linked to this blossom)
             let mut node = blossom_node_ptr.write();
             node.class = DualNodeClass::Blossom {
                 nodes_circle: nodes_circle.iter().map(|ptr| ptr.downgrade()).collect(),
                 touching_children,
             };
             interface.nodes_length += 1;
             if interface.nodes.len() < interface.nodes_length {
                 interface.nodes.push(None);
             }
             drop(node);
-            interface.nodes[local_node_index] = Some(blossom_node_ptr);  // feature `dangerous_pointer`: must push the owner
+            interface.nodes[local_node_index] = Some(blossom_node_ptr); // feature `dangerous_pointer`: must push the owner
         }
         interface.sum_grow_speed += 1;
         drop(interface);
         dual_module_impl.prepare_nodes_shrink(&nodes_circle);
         dual_module_impl.add_blossom(&cloned_blossom_node_ptr);
         cloned_blossom_node_ptr
     }
@@ -932,90 +1013,127 @@
     /// bottleneck as long as physical error rate is well below the threshold. All internal nodes will have a [`DualNodeGrowState::Grow`] state afterwards.
     pub fn expand_blossom(&self, blossom_node_ptr: DualNodePtr, dual_module_impl: &mut impl DualModuleImpl) {
         let interface = self.read_recursive();
         if interface.debug_print_actions {
             let node = blossom_node_ptr.read_recursive();
             if let DualNodeClass::Blossom { nodes_circle, .. } = &node.class {
                 eprintln!("[expand blossom] {:?} -> {:?}", blossom_node_ptr, nodes_circle);
-            } else { unreachable!() }
+            } else {
+                unreachable!()
+            }
         }
         let is_fusion = interface.is_fusion;
         drop(interface);
-        if is_fusion {  // must update all the nodes before calling `remove_blossom` of the implementation
+        if is_fusion {
+            // must update all the nodes before calling `remove_blossom` of the implementation
             let node = blossom_node_ptr.read_recursive();
             if let DualNodeClass::Blossom { nodes_circle, .. } = &node.class {
                 for node_weak in nodes_circle.iter() {
                     node_weak.upgrade_force().update();
                 }
             }
         }
         dual_module_impl.remove_blossom(blossom_node_ptr.clone());
         let mut interface = self.write();
         let node = blossom_node_ptr.read_recursive();
         match &node.grow_state {
-            DualNodeGrowState::Grow => { interface.sum_grow_speed += -1; },
-            DualNodeGrowState::Shrink => { interface.sum_grow_speed += 1; },
-            DualNodeGrowState::Stay => { },
+            DualNodeGrowState::Grow => {
+                interface.sum_grow_speed += -1;
+            }
+            DualNodeGrowState::Shrink => {
+                interface.sum_grow_speed += 1;
+            }
+            DualNodeGrowState::Stay => {}
         }
         let node_idx = node.index;
-        debug_assert!(interface.get_node(node_idx).is_some(), "the blossom should not be expanded before");
-        debug_assert!(interface.get_node(node_idx).as_ref().unwrap() == &blossom_node_ptr, "the blossom doesn't belong to this DualModuleInterface");
+        debug_assert!(
+            interface.get_node(node_idx).is_some(),
+            "the blossom should not be expanded before"
+        );
+        debug_assert!(
+            interface.get_node(node_idx).as_ref().unwrap() == &blossom_node_ptr,
+            "the blossom doesn't belong to this DualModuleInterface"
+        );
         drop(interface);
         match &node.class {
             DualNodeClass::Blossom { nodes_circle, .. } => {
                 for node_weak in nodes_circle.iter() {
                     let node_ptr = node_weak.upgrade_force();
                     let mut node = node_ptr.write();
-                    debug_assert!(node.parent_blossom.is_some() && node.parent_blossom.as_ref().unwrap() == &blossom_node_ptr.downgrade()
-                        , "internal error: parent blossom must be this blossom");
-                    debug_assert!(node.grow_state == DualNodeGrowState::Stay, "internal error: children node must be DualNodeGrowState::Stay");
+                    debug_assert!(
+                        node.parent_blossom.is_some()
+                            && node.parent_blossom.as_ref().unwrap() == &blossom_node_ptr.downgrade(),
+                        "internal error: parent blossom must be this blossom"
+                    );
+                    debug_assert!(
+                        node.grow_state == DualNodeGrowState::Stay,
+                        "internal error: children node must be DualNodeGrowState::Stay"
+                    );
                     node.parent_blossom = None;
                     drop(node);
-                    {  // safest way: to avoid sub-optimal result being found, set all nodes to growing state
+                    {
+                        // safest way: to avoid sub-optimal result being found, set all nodes to growing state
                         // WARNING: expanding a blossom like this way MAY CAUSE DEADLOCK!
                         // think about this extreme case: after a blossom is expanded, they may gradually form a new blossom and needs expanding again!
                         self.set_grow_state(&node_ptr, DualNodeGrowState::Grow, dual_module_impl);
                         // the solution is to provide two entry points, the two children of this blossom that directly connect to the two + node in the alternating tree
                         // only in that way it's guaranteed to make some progress without re-constructing this blossom
                         // It's the primal module's responsibility to avoid this happening, using the dual module's API: [``]
                     }
                 }
-            },
-            _ => { unreachable!() }
+            }
+            _ => {
+                unreachable!()
+            }
         }
         let mut interface = self.write();
-        interface.remove_node(node_idx);  // remove this blossom from root, feature `dangerous_pointer` requires running this at the end
+        interface.remove_node(node_idx); // remove this blossom from root, feature `dangerous_pointer` requires running this at the end
     }
 
     /// a helper function to update grow state
-    pub fn set_grow_state(&self, dual_node_ptr: &DualNodePtr, grow_state: DualNodeGrowState, dual_module_impl: &mut impl DualModuleImpl) {
+    pub fn set_grow_state(
+        &self,
+        dual_node_ptr: &DualNodePtr,
+        grow_state: DualNodeGrowState,
+        dual_module_impl: &mut impl DualModuleImpl,
+    ) {
         if self.read_recursive().is_fusion {
-            dual_node_ptr.update();  // these dual node may not be update-to-date in fusion
+            dual_node_ptr.update(); // these dual node may not be update-to-date in fusion
         }
         let mut interface = self.write();
         if interface.debug_print_actions {
             eprintln!("[set grow state] {:?} {:?}", dual_node_ptr, grow_state);
         }
-        {  // update sum_grow_speed and dual variable cache
+        {
+            // update sum_grow_speed and dual variable cache
             let mut node = dual_node_ptr.write();
             match &node.grow_state {
-                DualNodeGrowState::Grow => { interface.sum_grow_speed -= 1; },
-                DualNodeGrowState::Shrink => { interface.sum_grow_speed += 1; },
-                DualNodeGrowState::Stay => { },
+                DualNodeGrowState::Grow => {
+                    interface.sum_grow_speed -= 1;
+                }
+                DualNodeGrowState::Shrink => {
+                    interface.sum_grow_speed += 1;
+                }
+                DualNodeGrowState::Stay => {}
             }
             match grow_state {
-                DualNodeGrowState::Grow => { interface.sum_grow_speed += 1; },
-                DualNodeGrowState::Shrink => { interface.sum_grow_speed -= 1; },
-                DualNodeGrowState::Stay => { },
+                DualNodeGrowState::Grow => {
+                    interface.sum_grow_speed += 1;
+                }
+                DualNodeGrowState::Shrink => {
+                    interface.sum_grow_speed -= 1;
+                }
+                DualNodeGrowState::Stay => {}
             }
             let current_dual_variable = node.get_dual_variable(&interface);
-            node.dual_variable_cache = (current_dual_variable, interface.dual_variable_global_progress);  // update the cache
+            node.dual_variable_cache = (current_dual_variable, interface.dual_variable_global_progress);
+            // update the cache
         }
         drop(interface);
-        dual_module_impl.set_grow_state(dual_node_ptr, grow_state);  // call this before dual node actually sets; to give history information
+        dual_module_impl.set_grow_state(dual_node_ptr, grow_state); // call this before dual node actually sets; to give history information
         dual_node_ptr.set_grow_state(grow_state);
     }
 
     /// grow the dual module and update [`DualModuleInterface::sum_`]
     pub fn grow(&self, length: Weight, dual_module_impl: &mut impl DualModuleImpl) {
         dual_module_impl.grow(length);
         let mut interface = self.write();
@@ -1023,36 +1141,42 @@
         interface.dual_variable_global_progress += length;
     }
 
     /// grow a specific length globally but iteratively: will try to keep growing that much
     pub fn grow_iterative(&self, mut length: Weight, dual_module_impl: &mut impl DualModuleImpl) {
         while length > 0 {
             let max_update_length = dual_module_impl.compute_maximum_update_length();
-            let safe_growth = max_update_length.get_none_zero_growth().unwrap_or_else(|| panic!("iterative grow failed because of conflicts {max_update_length:?}"));
+            let safe_growth = max_update_length
+                .get_none_zero_growth()
+                .unwrap_or_else(|| panic!("iterative grow failed because of conflicts {max_update_length:?}"));
             let growth = std::cmp::min(length, safe_growth);
             self.grow(growth, dual_module_impl);
             length -= growth;
         }
     }
 
     /// fuse two interfaces by copying the nodes in `other` into myself
+    #[allow(clippy::unnecessary_cast)]
     pub fn slow_fuse(&self, left: &Self, right: &Self) {
         let mut interface = self.write();
-        interface.is_fusion = true;  // for safety
+        interface.is_fusion = true; // for safety
         for other in [left, right] {
             let mut other_interface = other.write();
             other_interface.is_fusion = true;
             let bias = interface.nodes_length as NodeNum;
             for other_node_index in 0..other_interface.nodes_length as NodeNum {
                 let node_ptr = &other_interface.nodes[other_node_index as usize];
                 if let Some(node_ptr) = node_ptr {
                     let mut node = node_ptr.write();
                     debug_assert_eq!(node.index, other_node_index);
                     node.index += bias;
-                    node.dual_variable_cache = (node.get_dual_variable(&other_interface), interface.dual_variable_global_progress)
+                    node.dual_variable_cache = (
+                        node.get_dual_variable(&other_interface),
+                        interface.dual_variable_global_progress,
+                    )
                 }
                 interface.nodes_length += 1;
                 if interface.nodes.len() < interface.nodes_length {
                     interface.nodes.push(None);
                 }
                 interface.nodes[(bias + other_node_index) as usize] = node_ptr.clone();
             }
@@ -1063,174 +1187,247 @@
 
     /// fuse two interfaces by (virtually) copying the nodes in `other` into myself, with O(1) time complexity
     pub fn fuse(&self, left: &Self, right: &Self) {
         let parent_weak = self.downgrade();
         let left_weak = left.downgrade();
         let right_weak = right.downgrade();
         let mut interface = self.write();
-        interface.is_fusion = true;  // for safety
+        interface.is_fusion = true; // for safety
         debug_assert_eq!(interface.nodes_length, 0, "fast fuse doesn't support non-empty fuse");
         debug_assert!(interface.children.is_none(), "cannot fuse twice");
         let mut left_interface = left.write();
         let mut right_interface = right.write();
         left_interface.is_fusion = true;
         right_interface.is_fusion = true;
         debug_assert!(left_interface.parent.is_none(), "cannot fuse an interface twice");
         debug_assert!(right_interface.parent.is_none(), "cannot fuse an interface twice");
         left_interface.parent = Some(parent_weak.clone());
         right_interface.parent = Some(parent_weak);
         left_interface.index_bias = 0;
         right_interface.index_bias = left_interface.nodes_count();
         interface.children = Some((
             (left_weak, left_interface.nodes_count()),
-            (right_weak, right_interface.nodes_count())
+            (right_weak, right_interface.nodes_count()),
         ));
         for other_interface in [left_interface, right_interface] {
             interface.sum_dual_variables += other_interface.sum_dual_variables;
             interface.sum_grow_speed += other_interface.sum_grow_speed;
         }
     }
 
     /// do a sanity check of if all the nodes are in consistent state
     #[inline(never)]
+    #[allow(clippy::unnecessary_cast)]
     pub fn sanity_check(&self) -> Result<Vec<Option<DualNodePtr>>, String> {
         let mut flattened_nodes = vec![];
         self.flatten_nodes(&mut flattened_nodes);
         let interface = self.read_recursive();
         if false {
             eprintln!("[warning] sanity check disabled for dual_module.rs");
             return Ok(flattened_nodes);
         }
         let mut visited_syndrome = HashSet::with_capacity((interface.nodes_count() * 2) as usize);
         let mut sum_individual_dual_variable = 0;
         for (index, dual_node_ptr) in flattened_nodes.iter().enumerate() {
             if let Some(dual_node_ptr) = dual_node_ptr {
                 let dual_node = dual_node_ptr.read_recursive();
                 sum_individual_dual_variable += dual_node.get_dual_variable(&interface);
-                if dual_node.index != index as NodeIndex { return Err(format!("dual node index wrong: expected {}, actual {}", index, dual_node.index)) }
+                if dual_node.index != index as NodeIndex {
+                    return Err(format!(
+                        "dual node index wrong: expected {}, actual {}",
+                        index, dual_node.index
+                    ));
+                }
                 match &dual_node.class {
-                    DualNodeClass::Blossom { nodes_circle, touching_children } => {
+                    DualNodeClass::Blossom {
+                        nodes_circle,
+                        touching_children,
+                    } => {
                         for (idx, circle_node_weak) in nodes_circle.iter().enumerate() {
                             let circle_node_ptr = circle_node_weak.upgrade_force();
                             if &circle_node_ptr == dual_node_ptr {
-                                return Err("a blossom should not contain itself".to_string())
+                                return Err("a blossom should not contain itself".to_string());
                             }
                             let circle_node = circle_node_ptr.read_recursive();
                             if circle_node.parent_blossom.as_ref() != Some(&dual_node_ptr.downgrade()) {
-                                return Err(format!("blossom {} contains {} but child's parent pointer = {:?} is not pointing back"
-                                    , dual_node.index, circle_node.index, circle_node.parent_blossom))
+                                return Err(format!(
+                                    "blossom {} contains {} but child's parent pointer = {:?} is not pointing back",
+                                    dual_node.index, circle_node.index, circle_node.parent_blossom
+                                ));
+                            }
+                            if circle_node.grow_state != DualNodeGrowState::Stay {
+                                return Err(format!("child node {} is not at Stay state", circle_node.index));
                             }
-                            if circle_node.grow_state != DualNodeGrowState::Stay { return Err(format!("child node {} is not at Stay state", circle_node.index)) }
                             // check if circle node is still tracked, i.e. inside self.nodes
-                            if circle_node.index >= interface.nodes_count() || interface.get_node(circle_node.index).is_none() {
-                                return Err(format!("child's index {} is not in the interface", circle_node.index))
+                            if circle_node.index >= interface.nodes_count()
+                                || interface.get_node(circle_node.index).is_none()
+                            {
+                                return Err(format!("child's index {} is not in the interface", circle_node.index));
                             }
                             let tracked_circle_node_ptr = interface.get_node(circle_node.index).unwrap();
                             if tracked_circle_node_ptr != circle_node_ptr {
-                                return Err(format!("the tracked ptr of child {} is not what's being pointed", circle_node.index))
+                                return Err(format!(
+                                    "the tracked ptr of child {} is not what's being pointed",
+                                    circle_node.index
+                                ));
                             }
                             // check children belongings
                             let (child_weak_1, child_weak_2) = &touching_children[idx];
-                            if matches!(circle_node.class, DualNodeClass::DefectVertex{..}) {
-                                if child_weak_1 != circle_node_weak { return Err(format!("touching child can only be syndrome node {}", circle_node.index)) }
-                                if child_weak_2 != circle_node_weak { return Err(format!("touching child can only be syndrome node {}", circle_node.index)) }
+                            if matches!(circle_node.class, DualNodeClass::DefectVertex { .. }) {
+                                if child_weak_1 != circle_node_weak {
+                                    return Err(format!("touching child can only be syndrome node {}", circle_node.index));
+                                }
+                                if child_weak_2 != circle_node_weak {
+                                    return Err(format!("touching child can only be syndrome node {}", circle_node.index));
+                                }
                             } else {
                                 let child_ptr_1 = child_weak_1.upgrade_force();
                                 let child_ptr_2 = child_weak_2.upgrade_force();
                                 let child_1_ancestor = child_ptr_1.get_ancestor_blossom();
                                 let child_2_ancestor = child_ptr_2.get_ancestor_blossom();
                                 let circle_ancestor = circle_node_ptr.get_ancestor_blossom();
-                                if child_1_ancestor != circle_ancestor { return Err(format!("{:?} is not descendent of {}", child_ptr_1, circle_node.index)) }
-                                if child_2_ancestor != circle_ancestor { return Err(format!("{:?} is not descendent of {}", child_ptr_2, circle_node.index)) }
+                                if child_1_ancestor != circle_ancestor {
+                                    return Err(format!("{:?} is not descendent of {}", child_ptr_1, circle_node.index));
+                                }
+                                if child_2_ancestor != circle_ancestor {
+                                    return Err(format!("{:?} is not descendent of {}", child_ptr_2, circle_node.index));
+                                }
                             }
                         }
-                    },
+                    }
                     DualNodeClass::DefectVertex { defect_index } => {
-                        if visited_syndrome.contains(defect_index) { return Err(format!("duplicate defect index: {}", defect_index)) }
+                        if visited_syndrome.contains(defect_index) {
+                            return Err(format!("duplicate defect index: {}", defect_index));
+                        }
                         visited_syndrome.insert(*defect_index);
-                    },
+                    }
                 }
                 if let Some(parent_blossom_weak) = &dual_node.parent_blossom {
-                    if dual_node.grow_state != DualNodeGrowState::Stay { return Err(format!("child node {} is not at Stay state", dual_node.index)) }
+                    if dual_node.grow_state != DualNodeGrowState::Stay {
+                        return Err(format!("child node {} is not at Stay state", dual_node.index));
+                    }
                     let parent_blossom_ptr = parent_blossom_weak.upgrade_force();
                     let parent_blossom = parent_blossom_ptr.read_recursive();
                     // check if child is actually inside this blossom
                     match &parent_blossom.class {
                         DualNodeClass::Blossom { nodes_circle, .. } => {
                             let mut found_match_count = 0;
                             for node_weak in nodes_circle.iter() {
                                 let node_ptr = node_weak.upgrade_force();
                                 if &node_ptr == dual_node_ptr {
                                     found_match_count += 1;
                                 }
                             }
                             if found_match_count != 1 {
-                                return Err(format!("{} is the parent of {} but the child only presents {} times", parent_blossom.index, dual_node.index, found_match_count))
+                                return Err(format!(
+                                    "{} is the parent of {} but the child only presents {} times",
+                                    parent_blossom.index, dual_node.index, found_match_count
+                                ));
                             }
-                        }, _ => { return Err(format!("{}, as the parent of {}, is not a blossom", parent_blossom.index, dual_node.index)) }
+                        }
+                        _ => {
+                            return Err(format!(
+                                "{}, as the parent of {}, is not a blossom",
+                                parent_blossom.index, dual_node.index
+                            ))
+                        }
                     }
                     // check if blossom is still tracked, i.e. inside interface.nodes
-                    if parent_blossom.index >= interface.nodes_count() || interface.get_node(parent_blossom.index).is_none() {
-                        return Err(format!("parent blossom's index {} is not in the interface", parent_blossom.index))
+                    if parent_blossom.index >= interface.nodes_count() || interface.get_node(parent_blossom.index).is_none()
+                    {
+                        return Err(format!(
+                            "parent blossom's index {} is not in the interface",
+                            parent_blossom.index
+                        ));
                     }
                     let tracked_parent_blossom_ptr = interface.get_node(parent_blossom.index).unwrap();
                     if tracked_parent_blossom_ptr != parent_blossom_ptr {
-                        return Err(format!("the tracked ptr of parent blossom {} is not what's being pointed", parent_blossom.index))
+                        return Err(format!(
+                            "the tracked ptr of parent blossom {} is not what's being pointed",
+                            parent_blossom.index
+                        ));
                     }
                 }
             }
         }
         if sum_individual_dual_variable != interface.sum_dual_variables {
-            return Err(format!("internal error: the sum of dual variables is {} but individual sum is {}", interface.sum_dual_variables, sum_individual_dual_variable))
+            return Err(format!(
+                "internal error: the sum of dual variables is {} but individual sum is {}",
+                interface.sum_dual_variables, sum_individual_dual_variable
+            ));
         }
         Ok(flattened_nodes)
     }
 
     pub fn sum_dual_variables(&self) -> Weight {
         self.read_recursive().sum_dual_variables
     }
-
 }
 
 impl Ord for MaxUpdateLength {
     fn cmp(&self, other: &Self) -> Ordering {
-        debug_assert!(!matches!(self, MaxUpdateLength::NonZeroGrow(_)), "priority ordering is not valid for NonZeroGrow");
-        debug_assert!(!matches!(other, MaxUpdateLength::NonZeroGrow(_)), "priority ordering is not valid for NonZeroGrow");
+        debug_assert!(
+            !matches!(self, MaxUpdateLength::NonZeroGrow(_)),
+            "priority ordering is not valid for NonZeroGrow"
+        );
+        debug_assert!(
+            !matches!(other, MaxUpdateLength::NonZeroGrow(_)),
+            "priority ordering is not valid for NonZeroGrow"
+        );
         if self == other {
-            return Ordering::Equal
+            return Ordering::Equal;
         }
         // VertexShrinkStop has the lowest priority: it should be put at the end of any ordered list
         // this is because solving VertexShrinkStop conflict is not possible, but when this happens, the primal module
         // should have put this node as a "-" node in the alternating tree, so there must be a parent and a child that
         // are "+" nodes, conflicting with each other at exactly this VertexShrinkStop node. In this case, as long as
         // one solves those "+" nodes conflicting, e.g. forming a blossom, this node's VertexShrinkStop conflict is automatically solved
-        match (matches!(self, MaxUpdateLength::VertexShrinkStop( .. )), matches!(other, MaxUpdateLength::VertexShrinkStop( .. ))) {
-            (true, false) => { return Ordering::Less },  // less priority
-            (false, true) => { return Ordering::Greater },  // greater priority
-            (true, true) => { return self.get_vertex_shrink_stop().unwrap().cmp(&other.get_vertex_shrink_stop().unwrap()) },  // don't care, just compare pointer
-            _ => { }
+        match (
+            matches!(self, MaxUpdateLength::VertexShrinkStop(..)),
+            matches!(other, MaxUpdateLength::VertexShrinkStop(..)),
+        ) {
+            (true, false) => return Ordering::Less,    // less priority
+            (false, true) => return Ordering::Greater, // greater priority
+            (true, true) => {
+                return self
+                    .get_vertex_shrink_stop()
+                    .unwrap()
+                    .cmp(&other.get_vertex_shrink_stop().unwrap())
+            } // don't care, just compare pointer
+            _ => {}
         }
         // then, blossom expanding has the low priority, because it's infrequent and expensive
-        match (matches!(self, MaxUpdateLength::BlossomNeedExpand( .. )), matches!(other, MaxUpdateLength::BlossomNeedExpand( .. ))) {
-            (true, false) => { return Ordering::Less },  // less priority
-            (false, true) => { return Ordering::Greater },  // greater priority
-            (true, true) => { return self.get_blossom_need_expand().unwrap().cmp(&other.get_blossom_need_expand().unwrap()) },  // don't care, just compare pointer
-            _ => { }
+        match (
+            matches!(self, MaxUpdateLength::BlossomNeedExpand(..)),
+            matches!(other, MaxUpdateLength::BlossomNeedExpand(..)),
+        ) {
+            (true, false) => return Ordering::Less,    // less priority
+            (false, true) => return Ordering::Greater, // greater priority
+            (true, true) => {
+                return self
+                    .get_blossom_need_expand()
+                    .unwrap()
+                    .cmp(&other.get_blossom_need_expand().unwrap())
+            } // don't care, just compare pointer
+            _ => {}
         }
         // We'll prefer match nodes internally instead of to boundary, because there might be less path connecting to boundary
         // this is only an attempt to optimize the MWPM decoder, but anyway it won't be an optimal decoder
-        match (matches!(self, MaxUpdateLength::TouchingVirtual( .. )), matches!(other, MaxUpdateLength::TouchingVirtual( .. ))) {
-            (true, false) => { return Ordering::Less },  // less priority
-            (false, true) => { return Ordering::Greater },  // greater priority
+        match (
+            matches!(self, MaxUpdateLength::TouchingVirtual(..)),
+            matches!(other, MaxUpdateLength::TouchingVirtual(..)),
+        ) {
+            (true, false) => return Ordering::Less,    // less priority
+            (false, true) => return Ordering::Greater, // greater priority
             (true, true) => {
                 let (a, c) = self.get_touching_virtual().unwrap();
                 let (b, d) = other.get_touching_virtual().unwrap();
-                return a.cmp(&b).reverse().then(c.cmp(&d).reverse())
-            },  // don't care, just compare pointer
-            _ => { }
+                return a.cmp(&b).reverse().then(c.cmp(&d).reverse());
+            } // don't care, just compare pointer
+            _ => {}
         }
         // last, both of them MUST be MaxUpdateLength::Conflicting
         let (a, c) = self.get_conflicting().unwrap();
         let (b, d) = other.get_conflicting().unwrap();
         a.cmp(&b).reverse().then(c.cmp(&d).reverse())
     }
 }
@@ -1238,102 +1435,104 @@
 impl PartialOrd for MaxUpdateLength {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         Some(self.cmp(other))
     }
 }
 
 impl MaxUpdateLength {
-
     /// update all the interface nodes to be up-to-date
     pub fn update(&self) {
         match self {
-            Self::NonZeroGrow(_) => { },
+            Self::NonZeroGrow(_) => {}
             Self::Conflicting((a, b), (c, d)) => {
-                for x in [a, b, c, d] { x.update(); }
-            },
+                for x in [a, b, c, d] {
+                    x.update();
+                }
+            }
             Self::TouchingVirtual((a, b), _) => {
-                for x in [a, b] { x.update(); }
-            },
+                for x in [a, b] {
+                    x.update();
+                }
+            }
             Self::BlossomNeedExpand(x) => {
                 x.update();
-            },
+            }
             Self::VertexShrinkStop((a, option)) => {
                 a.update();
                 if let Some((b, c)) = option {
                     b.update();
                     c.update();
                 }
-            },
+            }
         }
     }
 
     /// useful function to assert expected case
     #[allow(dead_code)]
     pub fn is_conflicting(&self, a: &DualNodePtr, b: &DualNodePtr) -> bool {
         if let MaxUpdateLength::Conflicting((n1, _), (n2, _)) = self {
             if n1 == a && n2 == b {
-                return true
+                return true;
             }
             if n1 == b && n2 == a {
-                return true
+                return true;
             }
         }
         false
     }
 
     /// helper function that get values out of the enum
     #[allow(dead_code)]
     #[inline(always)]
     pub fn get_none_zero_growth(&self) -> Option<Weight> {
         match self {
-            Self::NonZeroGrow((length, _has_empty_boundary_node)) => { Some(*length) },
-            _ => { None },
+            Self::NonZeroGrow((length, _has_empty_boundary_node)) => Some(*length),
+            _ => None,
         }
     }
 
     /// helper function that get values out of the enum
     #[allow(dead_code)]
     #[inline(always)]
     pub fn get_conflicting(&self) -> Option<(DualNodePtr, DualNodePtr)> {
         match self {
-            Self::Conflicting((a, _), (b, _)) => { Some((a.clone(), b.clone())) },
-            _ => { None },
+            Self::Conflicting((a, _), (b, _)) => Some((a.clone(), b.clone())),
+            _ => None,
         }
     }
 
     /// helper function that get values out of the enum
     #[allow(dead_code)]
     #[inline(always)]
     pub fn get_touching_virtual(&self) -> Option<(DualNodePtr, VertexIndex)> {
         match self {
-            Self::TouchingVirtual((a, _), (b, _)) => { Some((a.clone(), *b)) },
-            _ => { None },
+            Self::TouchingVirtual((a, _), (b, _)) => Some((a.clone(), *b)),
+            _ => None,
         }
     }
 
     /// helper function that get values out of the enum
     #[allow(dead_code)]
     #[inline(always)]
     pub fn get_blossom_need_expand(&self) -> Option<DualNodePtr> {
         match self {
-            Self::BlossomNeedExpand(a) => { Some(a.clone()) },
-            _ => { None },
+            Self::BlossomNeedExpand(a) => Some(a.clone()),
+            _ => None,
         }
     }
 
     /// helper function that get values out of the enum
     #[allow(dead_code)]
     #[inline(always)]
     pub fn get_vertex_shrink_stop(&self) -> Option<DualNodePtr> {
         match self {
-            Self::VertexShrinkStop((a, _)) => { Some(a.clone()) },
-            _ => { None },
+            Self::VertexShrinkStop((a, _)) => Some(a.clone()),
+            _ => None,
         }
     }
-
 }
 
 /// temporarily remember the weights that has been changed, so that it can revert back
 #[derive(Debug, Clone)]
 pub struct EdgeWeightModifier {
     /// edge with changed weighted caused by the erasure or X/Z correlation
     pub modified: Vec<(EdgeIndex, Weight)>,
@@ -1342,40 +1541,36 @@
 impl Default for EdgeWeightModifier {
     fn default() -> Self {
         Self::new()
     }
 }
 
 impl EdgeWeightModifier {
-
     pub fn new() -> Self {
-        Self {
-            modified: vec![],
-        }
+        Self { modified: vec![] }
     }
 
     /// record the modified edge
     pub fn push_modified_edge(&mut self, erasure_edge: EdgeIndex, original_weight: Weight) {
         self.modified.push((erasure_edge, original_weight));
     }
 
     /// if some edges are not recovered
     pub fn has_modified_edges(&self) -> bool {
         !self.modified.is_empty()
     }
 
     /// retrieve the last modified edge, panic if no more modified edges
     pub fn pop_modified_edge(&mut self) -> (EdgeIndex, Weight) {
-        self.modified.pop().expect("no more modified edges, please check `has_modified_edges` before calling this method")
+        self.modified
+            .pop()
+            .expect("no more modified edges, please check `has_modified_edges` before calling this method")
     }
-
 }
 
 impl std::ops::Deref for EdgeWeightModifier {
-
     type Target = Vec<(EdgeIndex, Weight)>;
 
     fn deref(&self) -> &Self::Target {
         &self.modified
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/src/dual_module_parallel.rs` & `fusion_blossom-0.2.5/src/dual_module_parallel.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 //! Serial Dual Parallel
-//! 
+//!
 //! A parallel implementation of the dual module, leveraging the serial version
-//! 
+//!
 //! While it assumes single machine (using async runtime of Rust), the design targets distributed version
-//! that can spawn on different machines efficiently. The distributed version can be build based on this 
+//! that can spawn on different machines efficiently. The distributed version can be build based on this
 //! parallel version.
-//! 
+//!
 //! Notes:
-//! 
+//!
 //! According to https://tokio.rs/tokio/tutorial, tokio is not good for parallel computation. It suggests
-//! using https://docs.rs/rayon/latest/rayon/. 
+//! using https://docs.rs/rayon/latest/rayon/.
 //!
 
-use super::util::*;
-use std::sync::{Arc, Weak};
+#![cfg_attr(feature = "unsafe_pointer", allow(dropping_references))]
+use super::complete_graph::CompleteGraph;
 use super::dual_module::*;
 use super::dual_module_serial::*;
-use crate::serde_json;
-use serde::{Serialize, Deserialize};
+use super::pointers::*;
+use super::util::*;
 use super::visualize::*;
 use crate::rayon::prelude::*;
-use std::collections::{BTreeSet, HashSet};
-use super::complete_graph::CompleteGraph;
+use crate::serde_json;
 use crate::weak_table::PtrWeakHashSet;
-use super::pointers::*;
-
+use serde::{Deserialize, Serialize};
+use std::collections::{BTreeSet, HashSet};
+use std::sync::{Arc, Weak};
 
 pub struct DualModuleParallel<SerialModule: DualModuleImpl + Send + Sync> {
     /// the basic wrapped serial modules at the beginning, afterwards the fused units are appended after them
     pub units: Vec<ArcManualSafeLock<DualModuleParallelUnit<SerialModule>>>,
     /// local configuration
     pub config: DualModuleParallelConfig,
     /// partition information generated by the config
@@ -42,34 +42,42 @@
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[serde(deny_unknown_fields)]
 pub struct DualModuleParallelConfig {
     /// enable async execution of dual operations; only used when calling top-level operations, not used in individual units
     #[serde(default = "dual_module_parallel_default_configs::thread_pool_size")]
     pub thread_pool_size: usize,
     /// strategy of edges placement: if edges are placed in the fusion unit, it's good for software implementation because there are no duplicate
-    /// edges and no unnecessary vertices in the descendant units. On the other hand, it's not very favorable if implemented on hardware: the 
+    /// edges and no unnecessary vertices in the descendant units. On the other hand, it's not very favorable if implemented on hardware: the
     /// fusion unit usually contains a very small amount of vertices and edges for the interfacing between two blocks, but maintaining this small graph
     /// may consume additional hardware resources and increase the decoding latency. I want the algorithm to finally work on the hardware efficiently
     /// so I need to verify that it does work by holding all the fusion unit's owned vertices and edges in the descendants, although usually duplicated.
     #[serde(default = "dual_module_parallel_default_configs::edges_in_fusion_unit")]
     pub edges_in_fusion_unit: bool,
     /// enable parallel execution of a fused dual module
     #[serde(default = "dual_module_parallel_default_configs::enable_parallel_execution")]
     pub enable_parallel_execution: bool,
 }
 
 impl Default for DualModuleParallelConfig {
-    fn default() -> Self { serde_json::from_value(json!({})).unwrap() }
+    fn default() -> Self {
+        serde_json::from_value(json!({})).unwrap()
+    }
 }
 
 pub mod dual_module_parallel_default_configs {
-    pub fn thread_pool_size() -> usize { 0 }  // by default to the number of CPU cores
-    // pub fn thread_pool_size() -> usize { 1 }  // debug: use a single core
-    pub fn edges_in_fusion_unit() -> bool { true }  // by default use the software-friendly approach because of removing duplicate edges
-    pub fn enable_parallel_execution() -> bool { false }  // by default disabled: parallel execution may cause too much context switch, yet not much speed benefit
+    pub fn thread_pool_size() -> usize {
+        0
+    } // by default to the number of CPU cores
+      // pub fn thread_pool_size() -> usize { 1 }  // debug: use a single core
+    pub fn edges_in_fusion_unit() -> bool {
+        true
+    } // by default use the software-friendly approach because of removing duplicate edges
+    pub fn enable_parallel_execution() -> bool {
+        false
+    } // by default disabled: parallel execution may cause too much context switch, yet not much speed benefit
 }
 
 pub struct DualModuleParallelUnit<SerialModule: DualModuleImpl + Send + Sync> {
     /// the index
     pub unit_index: usize,
     /// partition information generated by the config
     pub partition_info: Arc<PartitionInfo>,
@@ -82,15 +90,18 @@
     /// the vertices owned by this unit, note that owning_range is a subset of whole_range
     pub owning_range: VertexRange,
     /// the vertices that are mirrored outside of whole_range, in order to propagate a vertex's sync event to every unit that mirrors it
     pub extra_descendant_mirrored_vertices: HashSet<VertexIndex>,
     /// the owned serial dual module
     pub serial_module: SerialModule,
     /// left and right children dual modules
-    pub children: Option<(DualModuleParallelUnitWeak<SerialModule>, DualModuleParallelUnitWeak<SerialModule>)>,
+    pub children: Option<(
+        DualModuleParallelUnitWeak<SerialModule>,
+        DualModuleParallelUnitWeak<SerialModule>,
+    )>,
     /// parent dual module
     pub parent: Option<DualModuleParallelUnitWeak<SerialModule>>,
     /// elevated dual nodes: whose descendent not on the representative path of a dual node
     pub elevated_dual_nodes: PtrWeakHashSet<DualNodeWeak>,
     /// an empty sync requests queue just to implement the trait
     pub empty_sync_request: Vec<SyncRequest>,
     /// run things in thread pool
@@ -111,169 +122,245 @@
 
 impl<SerialModule: DualModuleImpl + Send + Sync> std::fmt::Debug for DualModuleParallelUnitWeak<SerialModule> {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         self.upgrade_force().fmt(f)
     }
 }
 
-
 impl<SerialModule: DualModuleImpl + Send + Sync> DualModuleParallel<SerialModule> {
-
     /// recommended way to create a new instance, given a customized configuration
-    pub fn new_config(initializer: &SolverInitializer, partition_info: &PartitionInfo, config: DualModuleParallelConfig) -> Self {
+    #[allow(clippy::unnecessary_cast)]
+    pub fn new_config(
+        initializer: &SolverInitializer,
+        partition_info: &PartitionInfo,
+        config: DualModuleParallelConfig,
+    ) -> Self {
         let partition_info = Arc::new(partition_info.clone());
         let mut thread_pool_builder = rayon::ThreadPoolBuilder::new();
         if config.thread_pool_size != 0 {
             thread_pool_builder = thread_pool_builder.num_threads(config.thread_pool_size);
         }
         let thread_pool = thread_pool_builder.build().expect("creating thread pool failed");
         let mut units = vec![];
         let unit_count = partition_info.units.len();
-        let complete_graph = CompleteGraph::new(initializer.vertex_num, &initializer.weighted_edges);  // build the graph to construct the NN data structure
-        let mut contained_vertices_vec: Vec<BTreeSet<VertexIndex>> = vec![];  // all vertices maintained by each unit
+        let complete_graph = CompleteGraph::new(initializer.vertex_num, &initializer.weighted_edges); // build the graph to construct the NN data structure
+        let mut contained_vertices_vec: Vec<BTreeSet<VertexIndex>> = vec![]; // all vertices maintained by each unit
         let mut is_vertex_virtual: Vec<_> = (0..initializer.vertex_num).map(|_| false).collect();
         for virtual_vertex in initializer.virtual_vertices.iter() {
             is_vertex_virtual[*virtual_vertex as usize] = true;
         }
-        let partition_units: Vec<PartitionUnitPtr> = (0..unit_count).map(|unit_index| PartitionUnitPtr::new_value(PartitionUnit {
-            unit_index,
-            enabled: unit_index < partition_info.config.partitions.len(),
-        })).collect();
-        let mut partitioned_initializers: Vec<PartitionedSolverInitializer> = (0..unit_count).map(|unit_index| {
-            let mut interfaces = vec![];
-            let mut current_index = unit_index;
-            let owning_range = &partition_info.units[unit_index].owning_range;
-            let mut contained_vertices = BTreeSet::new();
-            for vertex_index in owning_range.iter() {
-                contained_vertices.insert(vertex_index);
-            }
-            while let Some(parent_index) = &partition_info.units[current_index].parent {
-                let mut mirror_vertices = vec![];
-                if config.edges_in_fusion_unit {
-                    for vertex_index in partition_info.units[*parent_index].owning_range.iter() {
-                        let mut is_incident = false;
-                        for (peer_index, _) in complete_graph.vertices[vertex_index as usize].edges.iter() {
-                            if owning_range.contains(*peer_index) {
-                                is_incident = true;
-                                break
+        let partition_units: Vec<PartitionUnitPtr> = (0..unit_count)
+            .map(|unit_index| {
+                PartitionUnitPtr::new_value(PartitionUnit {
+                    unit_index,
+                    enabled: unit_index < partition_info.config.partitions.len(),
+                })
+            })
+            .collect();
+        let mut partitioned_initializers: Vec<PartitionedSolverInitializer> = (0..unit_count)
+            .map(|unit_index| {
+                let mut interfaces = vec![];
+                let mut current_index = unit_index;
+                let owning_range = &partition_info.units[unit_index].owning_range;
+                let mut contained_vertices = BTreeSet::new();
+                for vertex_index in owning_range.iter() {
+                    contained_vertices.insert(vertex_index);
+                }
+                while let Some(parent_index) = &partition_info.units[current_index].parent {
+                    let mut mirror_vertices = vec![];
+                    if config.edges_in_fusion_unit {
+                        for vertex_index in partition_info.units[*parent_index].owning_range.iter() {
+                            let mut is_incident = false;
+                            for (peer_index, _) in complete_graph.vertices[vertex_index as usize].edges.iter() {
+                                if owning_range.contains(*peer_index) {
+                                    is_incident = true;
+                                    break;
+                                }
+                            }
+                            if is_incident {
+                                mirror_vertices.push((vertex_index, is_vertex_virtual[vertex_index as usize]));
+                                contained_vertices.insert(vertex_index);
                             }
                         }
-                        if is_incident {
-                            mirror_vertices.push((vertex_index, is_vertex_virtual[vertex_index as usize]));
-                            contained_vertices.insert(vertex_index);
-                        }
-                    }
-                } else {
-                    // first check if there EXISTS any vertex that's adjacent of it's contains vertex
-                    let mut has_incident = false;
-                    for vertex_index in partition_info.units[*parent_index].owning_range.iter() {
-                        for (peer_index, _) in complete_graph.vertices[vertex_index as usize].edges.iter() {
-                            if contained_vertices.contains(peer_index) {  // important diff: as long as it has an edge with contained vertex, add it
-                                has_incident = true;
-                                break
+                    } else {
+                        // first check if there EXISTS any vertex that's adjacent of it's contains vertex
+                        let mut has_incident = false;
+                        for vertex_index in partition_info.units[*parent_index].owning_range.iter() {
+                            for (peer_index, _) in complete_graph.vertices[vertex_index as usize].edges.iter() {
+                                if contained_vertices.contains(peer_index) {
+                                    // important diff: as long as it has an edge with contained vertex, add it
+                                    has_incident = true;
+                                    break;
+                                }
+                            }
+                            if has_incident {
+                                break;
                             }
                         }
                         if has_incident {
-                            break
+                            // add all vertices as mirrored
+                            for vertex_index in partition_info.units[*parent_index].owning_range.iter() {
+                                mirror_vertices.push((vertex_index, is_vertex_virtual[vertex_index as usize]));
+                                contained_vertices.insert(vertex_index);
+                            }
                         }
                     }
-                    if has_incident {
-                        // add all vertices as mirrored
-                        for vertex_index in partition_info.units[*parent_index].owning_range.iter() {
-                            mirror_vertices.push((vertex_index, is_vertex_virtual[vertex_index as usize]));
-                            contained_vertices.insert(vertex_index);
-                        }
+                    if !mirror_vertices.is_empty() {
+                        // only add non-empty mirrored parents is enough
+                        interfaces.push((partition_units[*parent_index].downgrade(), mirror_vertices));
                     }
+                    current_index = *parent_index;
                 }
-                if !mirror_vertices.is_empty() {  // only add non-empty mirrored parents is enough
-                    interfaces.push((partition_units[*parent_index].downgrade(), mirror_vertices));
-                }
-                current_index = *parent_index;
-            }
-            contained_vertices_vec.push(contained_vertices);
-            PartitionedSolverInitializer {
-                unit_index,
-                vertex_num: initializer.vertex_num,
-                edge_num: initializer.weighted_edges.len(),
-                owning_range: *owning_range,
-                owning_interface: if unit_index < partition_info.config.partitions.len() { None } else { Some(partition_units[unit_index].downgrade()) },
-                weighted_edges: vec![],  // to be filled later
-                interfaces,
-                virtual_vertices: owning_range.iter().filter(|vertex_index| is_vertex_virtual[*vertex_index as usize]).collect(),
-            }  // note that all fields can be modified later
-        }).collect();
+                contained_vertices_vec.push(contained_vertices);
+                PartitionedSolverInitializer {
+                    unit_index,
+                    vertex_num: initializer.vertex_num,
+                    edge_num: initializer.weighted_edges.len(),
+                    owning_range: *owning_range,
+                    owning_interface: if unit_index < partition_info.config.partitions.len() {
+                        None
+                    } else {
+                        Some(partition_units[unit_index].downgrade())
+                    },
+                    weighted_edges: vec![], // to be filled later
+                    interfaces,
+                    virtual_vertices: owning_range
+                        .iter()
+                        .filter(|vertex_index| is_vertex_virtual[*vertex_index as usize])
+                        .collect(),
+                } // note that all fields can be modified later
+            })
+            .collect();
         // assign each edge to its unique partition
         for (edge_index, &(i, j, weight)) in initializer.weighted_edges.iter().enumerate() {
             assert_ne!(i, j, "invalid edge from and to the same vertex {}", i);
-            assert!(i < initializer.vertex_num, "edge ({}, {}) connected to an invalid vertex {}", i, j, i);
-            assert!(j < initializer.vertex_num, "edge ({}, {}) connected to an invalid vertex {}", i, j, j);
+            assert!(
+                i < initializer.vertex_num,
+                "edge ({}, {}) connected to an invalid vertex {}",
+                i,
+                j,
+                i
+            );
+            assert!(
+                j < initializer.vertex_num,
+                "edge ({}, {}) connected to an invalid vertex {}",
+                i,
+                j,
+                j
+            );
             let i_unit_index = partition_info.vertex_to_owning_unit[i as usize];
             let j_unit_index = partition_info.vertex_to_owning_unit[j as usize];
             // either left is ancestor of right or right is ancestor of left, otherwise the edge is invalid (because crossing two independent partitions)
             let is_i_ancestor = partition_info.units[i_unit_index].descendants.contains(&j_unit_index);
             let is_j_ancestor = partition_info.units[j_unit_index].descendants.contains(&i_unit_index);
-            assert!(is_i_ancestor || is_j_ancestor || i_unit_index == j_unit_index, "violating edge ({}, {}) crossing two independent partitions {} and {}"
-                , i, j, i_unit_index, j_unit_index);
+            assert!(
+                is_i_ancestor || is_j_ancestor || i_unit_index == j_unit_index,
+                "violating edge ({}, {}) crossing two independent partitions {} and {}",
+                i,
+                j,
+                i_unit_index,
+                j_unit_index
+            );
             let ancestor_unit_index = if is_i_ancestor { i_unit_index } else { j_unit_index };
             let descendant_unit_index = if is_i_ancestor { j_unit_index } else { i_unit_index };
             if config.edges_in_fusion_unit {
                 // the edge should be added to the descendant, and it's guaranteed that the descendant unit contains (although not necessarily owned) the vertex
-                partitioned_initializers[descendant_unit_index].weighted_edges.push((i, j, weight, edge_index as EdgeIndex));
+                partitioned_initializers[descendant_unit_index]
+                    .weighted_edges
+                    .push((i, j, weight, edge_index as EdgeIndex));
             } else {
                 // add edge to every unit from the descendant (including) and the ancestor (excluding) who mirrored the vertex
                 if ancestor_unit_index < partition_info.config.partitions.len() {
                     // leaf unit holds every unit
-                    partitioned_initializers[descendant_unit_index].weighted_edges.push((i, j, weight, edge_index as EdgeIndex));
+                    partitioned_initializers[descendant_unit_index].weighted_edges.push((
+                        i,
+                        j,
+                        weight,
+                        edge_index as EdgeIndex,
+                    ));
                 } else {
                     // iterate every leaf unit of the `descendant_unit_index` to see if adding the edge or not
                     struct DfsInfo<'a> {
                         partition_config: &'a PartitionConfig,
                         partition_info: &'a PartitionInfo,
                         i: VertexIndex,
                         j: VertexIndex,
                         weight: Weight,
                         contained_vertices_vec: &'a Vec<BTreeSet<VertexIndex>>,
                         edge_index: EdgeIndex,
                     }
                     let dfs_info = DfsInfo {
-                        partition_config: &partition_info.config, partition_info: &partition_info
-                        , i, j, weight, contained_vertices_vec: &contained_vertices_vec, edge_index: edge_index as EdgeIndex,
+                        partition_config: &partition_info.config,
+                        partition_info: &partition_info,
+                        i,
+                        j,
+                        weight,
+                        contained_vertices_vec: &contained_vertices_vec,
+                        edge_index: edge_index as EdgeIndex,
                     };
-                    fn dfs_add(unit_index: usize, dfs_info: &DfsInfo, partitioned_initializers: &mut Vec<PartitionedSolverInitializer>) {
+                    fn dfs_add(
+                        unit_index: usize,
+                        dfs_info: &DfsInfo,
+                        partitioned_initializers: &mut Vec<PartitionedSolverInitializer>,
+                    ) {
                         if unit_index >= dfs_info.partition_config.partitions.len() {
-                            let (left_index, right_index) = &dfs_info.partition_info.units[unit_index].children.expect("fusion unit must have children");
+                            let (left_index, right_index) = &dfs_info.partition_info.units[unit_index]
+                                .children
+                                .expect("fusion unit must have children");
                             dfs_add(*left_index, dfs_info, partitioned_initializers);
                             dfs_add(*right_index, dfs_info, partitioned_initializers);
                         } else {
                             let contain_i = dfs_info.contained_vertices_vec[unit_index].contains(&dfs_info.i);
                             let contain_j = dfs_info.contained_vertices_vec[unit_index].contains(&dfs_info.j);
-                            assert!(!(contain_i ^ contain_j), "{} and {} must either be both contained or not contained by {}", dfs_info.i, dfs_info.j, unit_index);
+                            assert!(
+                                !(contain_i ^ contain_j),
+                                "{} and {} must either be both contained or not contained by {}",
+                                dfs_info.i,
+                                dfs_info.j,
+                                unit_index
+                            );
                             if contain_i {
-                                partitioned_initializers[unit_index].weighted_edges.push((dfs_info.i, dfs_info.j, dfs_info.weight, dfs_info.edge_index));
+                                partitioned_initializers[unit_index].weighted_edges.push((
+                                    dfs_info.i,
+                                    dfs_info.j,
+                                    dfs_info.weight,
+                                    dfs_info.edge_index,
+                                ));
                             }
                         }
                     }
                     dfs_add(descendant_unit_index, &dfs_info, &mut partitioned_initializers);
                 }
             }
         }
         // println!("partitioned_initializers: {:?}", partitioned_initializers);
         thread_pool.scope(|_| {
-            (0..unit_count).into_par_iter().map(|unit_index| {
-                // println!("unit_index: {unit_index}");
-                let dual_module = SerialModule::new_partitioned(&partitioned_initializers[unit_index]);
-                DualModuleParallelUnitPtr::new_wrapper(dual_module, unit_index, Arc::clone(&partition_info), partition_units[unit_index].clone()
-                    , config.enable_parallel_execution)
-            }).collect_into_vec(&mut units);
+            (0..unit_count)
+                .into_par_iter()
+                .map(|unit_index| {
+                    // println!("unit_index: {unit_index}");
+                    let dual_module = SerialModule::new_partitioned(&partitioned_initializers[unit_index]);
+                    DualModuleParallelUnitPtr::new_wrapper(
+                        dual_module,
+                        unit_index,
+                        Arc::clone(&partition_info),
+                        partition_units[unit_index].clone(),
+                        config.enable_parallel_execution,
+                    )
+                })
+                .collect_into_vec(&mut units);
         });
         // fill in the children and parent references
         for unit_index in 0..unit_count {
             let mut unit = units[unit_index].write();
             if let Some((left_children_index, right_children_index)) = &partition_info.units[unit_index].children {
-                unit.children = Some((units[*left_children_index].downgrade(), units[*right_children_index].downgrade()))
+                unit.children = Some((
+                    units[*left_children_index].downgrade(),
+                    units[*right_children_index].downgrade(),
+                ))
             }
             if let Some(parent_index) = &partition_info.units[unit_index].parent {
                 unit.parent = Some(units[*parent_index].downgrade());
             }
         }
         // fill in the extra_descendant_mirrored_vertices
         for unit_index in 0..unit_count {
@@ -286,15 +373,20 @@
                         unit.extra_descendant_mirrored_vertices.insert(*vertex_index);
                     }
                 }
             }
             if let Some((left_children_weak, right_children_weak)) = unit.children.clone() {
                 for child_weak in [left_children_weak, right_children_weak] {
                     // note: although iterating over HashSet is not performance optimal, this only happens at initialization and thus it's fine
-                    for vertex_index in child_weak.upgrade_force().read_recursive().extra_descendant_mirrored_vertices.iter() {
+                    for vertex_index in child_weak
+                        .upgrade_force()
+                        .read_recursive()
+                        .extra_descendant_mirrored_vertices
+                        .iter()
+                    {
                         if !whole_range.contains(*vertex_index) {
                             unit.extra_descendant_mirrored_vertices.insert(*vertex_index);
                         }
                     }
                 }
             }
             // println!("{} extra_descendant_mirrored_vertices: {:?}", unit.unit_index, unit.extra_descendant_mirrored_vertices);
@@ -310,72 +402,82 @@
 
     /// find the active ancestor to handle this dual node (should be unique, i.e. any time only one ancestor is active)
     #[inline(never)]
     pub fn find_active_ancestor(&self, dual_node_ptr: &DualNodePtr) -> DualModuleParallelUnitPtr<SerialModule> {
         self.find_active_ancestor_option(dual_node_ptr).unwrap()
     }
 
-    pub fn find_active_ancestor_option(&self, dual_node_ptr: &DualNodePtr) -> Option<DualModuleParallelUnitPtr<SerialModule>> {
+    #[allow(clippy::unnecessary_cast)]
+    pub fn find_active_ancestor_option(
+        &self,
+        dual_node_ptr: &DualNodePtr,
+    ) -> Option<DualModuleParallelUnitPtr<SerialModule>> {
         // find the first active ancestor unit that should handle this dual node
         let representative_vertex = dual_node_ptr.get_representative_vertex();
         let owning_unit_index = self.partition_info.vertex_to_owning_unit[representative_vertex as usize];
         let mut owning_unit_ptr = self.units[owning_unit_index].clone();
         loop {
             let owning_unit = owning_unit_ptr.read_recursive();
             if owning_unit.is_active {
-                break  // find an active unit
+                break; // find an active unit
             }
             if let Some(parent_weak) = &owning_unit.parent {
                 let parent_owning_unit_ptr = parent_weak.upgrade_force();
                 drop(owning_unit);
                 owning_unit_ptr = parent_owning_unit_ptr;
             } else {
-                return None
+                return None;
             }
         }
         Some(owning_unit_ptr)
     }
 
     /// statically fuse them all, may be called at any state (meaning each unit may not necessarily be solved locally)
     pub fn static_fuse_all(&mut self) {
         for unit_ptr in self.units.iter() {
             lock_write!(unit, unit_ptr);
             if let Some((left_child_weak, right_child_weak)) = &unit.children {
-                {  // ignore already fused children and work on others
+                {
+                    // ignore already fused children and work on others
                     let left_child_ptr = left_child_weak.upgrade_force();
                     let right_child_ptr = right_child_weak.upgrade_force();
                     let left_child = left_child_ptr.read_recursive();
                     let right_child = right_child_ptr.read_recursive();
                     if !left_child.is_active && !right_child.is_active {
-                        continue  // already fused, it's ok to just ignore
+                        continue; // already fused, it's ok to just ignore
                     }
-                    debug_assert!(left_child.is_active && right_child.is_active, "children must be active at the same time if fusing all together");
+                    debug_assert!(
+                        left_child.is_active && right_child.is_active,
+                        "children must be active at the same time if fusing all together"
+                    );
                 }
                 unit.static_fuse();
             }
         }
     }
-
 }
 
 impl<SerialModule: DualModuleImpl + Send + Sync> DualModuleImpl for DualModuleParallel<SerialModule> {
-
     /// initialize the dual module, which is supposed to be reused for multiple decoding tasks with the same structure
     fn new_empty(initializer: &SolverInitializer) -> Self {
-        Self::new_config(initializer, &PartitionConfig::new(initializer.vertex_num).info(), DualModuleParallelConfig::default())
+        Self::new_config(
+            initializer,
+            &PartitionConfig::new(initializer.vertex_num).info(),
+            DualModuleParallelConfig::default(),
+        )
     }
 
     /// clear all growth and existing dual nodes
     #[inline(never)]
     fn clear(&mut self) {
         self.thread_pool.scope(|_| {
             self.units.par_iter().enumerate().for_each(|(unit_idx, unit_ptr)| {
                 lock_write!(unit, unit_ptr);
                 unit.clear();
-                unit.is_active = unit_idx < self.partition_info.config.partitions.len();  // only partitioned serial modules are active at the beginning
+                unit.is_active = unit_idx < self.partition_info.config.partitions.len(); // only partitioned serial modules are active at the beginning
                 unit.partition_unit.write().enabled = false;
                 unit.elevated_dual_nodes.clear();
             });
         })
     }
 
     // although not the intended way to use it, we do support these common APIs for compatibility with normal primal modules
@@ -400,29 +502,40 @@
         let unit_ptr = self.find_active_ancestor(dual_node_ptr);
         self.thread_pool.scope(|_| {
             lock_write!(unit, unit_ptr);
             unit.set_grow_state(dual_node_ptr, grow_state);
         })
     }
 
-    fn compute_maximum_update_length_dual_node(&mut self, dual_node_ptr: &DualNodePtr, is_grow: bool, simultaneous_update: bool) -> MaxUpdateLength {
+    fn compute_maximum_update_length_dual_node(
+        &mut self,
+        dual_node_ptr: &DualNodePtr,
+        is_grow: bool,
+        simultaneous_update: bool,
+    ) -> MaxUpdateLength {
         let unit_ptr = self.find_active_ancestor(dual_node_ptr);
         self.thread_pool.scope(|_| {
             lock_write!(unit, unit_ptr);
             unit.compute_maximum_update_length_dual_node(dual_node_ptr, is_grow, simultaneous_update)
         })
     }
 
     fn compute_maximum_update_length(&mut self) -> GroupMaxUpdateLength {
         self.thread_pool.scope(|_| {
-            let results: Vec<_> = self.units.par_iter().filter_map(|unit_ptr| {
-                lock_write!(unit, unit_ptr);
-                if !unit.is_active { return None }
-                Some(unit.compute_maximum_update_length())
-            }).collect();
+            let results: Vec<_> = self
+                .units
+                .par_iter()
+                .filter_map(|unit_ptr| {
+                    lock_write!(unit, unit_ptr);
+                    if !unit.is_active {
+                        return None;
+                    }
+                    Some(unit.compute_maximum_update_length())
+                })
+                .collect();
             let mut group_max_update_length = GroupMaxUpdateLength::new();
             for local_group_max_update_length in results.into_iter() {
                 group_max_update_length.extend(local_group_max_update_length);
             }
             group_max_update_length
         })
     }
@@ -435,121 +548,142 @@
         })
     }
 
     fn grow(&mut self, length: Weight) {
         self.thread_pool.scope(|_| {
             self.units.par_iter().for_each(|unit_ptr| {
                 lock_write!(unit, unit_ptr);
-                if !unit.is_active { return }
+                if !unit.is_active {
+                    return;
+                }
                 unit.grow(length);
             });
         })
     }
 
     fn load_edge_modifier(&mut self, edge_modifier: &[(EdgeIndex, Weight)]) {
         self.thread_pool.scope(|_| {
             self.units.par_iter().for_each(|unit_ptr| {
                 lock_write!(unit, unit_ptr);
-                if !unit.is_active { return }
+                if !unit.is_active {
+                    return;
+                }
                 unit.load_edge_modifier(edge_modifier);
             });
         })
     }
 
     fn prepare_nodes_shrink(&mut self, nodes_circle: &[DualNodePtr]) -> &mut Vec<SyncRequest> {
         let unit_ptr = self.find_active_ancestor(&nodes_circle[0]);
         self.thread_pool.scope(|_| {
             lock_write!(unit, unit_ptr);
             unit.prepare_nodes_shrink(nodes_circle);
         });
         &mut self.empty_sync_request
     }
-
 }
 
 impl<SerialModule: DualModuleImpl + Send + Sync> DualModuleParallelImpl for DualModuleParallel<SerialModule> {
-
     type UnitType = DualModuleParallelUnit<SerialModule>;
 
     fn get_unit(&self, unit_index: usize) -> ArcManualSafeLock<Self::UnitType> {
         self.units[unit_index].clone()
     }
-
 }
 
-
 /*
 Implementing visualization functions
 */
 
 impl<SerialModule: DualModuleImpl + FusionVisualizer + Send + Sync> FusionVisualizer for DualModuleParallel<SerialModule> {
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         // do the sanity check first before taking snapshot
         // self.sanity_check().unwrap();
         let mut value = json!({});
         for unit_ptr in self.units.iter() {
             let unit = unit_ptr.read_recursive();
-            if !unit.is_active { continue }  // do not visualize inactive units
+            if !unit.is_active {
+                continue;
+            } // do not visualize inactive units
             let value_2 = unit.snapshot(abbrev);
             snapshot_combine_values(&mut value, value_2, abbrev);
         }
         value
     }
 }
 
-impl<SerialModule: DualModuleImpl + FusionVisualizer + Send + Sync> FusionVisualizer for DualModuleParallelUnit<SerialModule> {
+impl<SerialModule: DualModuleImpl + FusionVisualizer + Send + Sync> FusionVisualizer
+    for DualModuleParallelUnit<SerialModule>
+{
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         let mut value = self.serial_module.snapshot(abbrev);
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
-            snapshot_combine_values(&mut value, left_child_weak.upgrade_force().read_recursive().snapshot(abbrev), abbrev);
-            snapshot_combine_values(&mut value, right_child_weak.upgrade_force().read_recursive().snapshot(abbrev), abbrev);
+            snapshot_combine_values(
+                &mut value,
+                left_child_weak.upgrade_force().read_recursive().snapshot(abbrev),
+                abbrev,
+            );
+            snapshot_combine_values(
+                &mut value,
+                right_child_weak.upgrade_force().read_recursive().snapshot(abbrev),
+                abbrev,
+            );
         }
         value
     }
 }
 
 impl<SerialModule: DualModuleImpl + Send + Sync> DualModuleParallelUnit<SerialModule> {
-
     /// statically fuse the children of this unit
     pub fn static_fuse(&mut self) {
         debug_assert!(!self.is_active, "cannot fuse the child an already active unit");
-        let (left_child_ptr, right_child_ptr) = (self.children.as_ref().unwrap().0.upgrade_force(), self.children.as_ref().unwrap().1.upgrade_force());
+        let (left_child_ptr, right_child_ptr) = (
+            self.children.as_ref().unwrap().0.upgrade_force(),
+            self.children.as_ref().unwrap().1.upgrade_force(),
+        );
         let mut left_child = left_child_ptr.write();
         let mut right_child = right_child_ptr.write();
         debug_assert!(left_child.is_active && right_child.is_active, "cannot fuse inactive pairs");
         // update active state
         self.is_active = true;
         left_child.is_active = false;
         right_child.is_active = false;
         // set partition unit as enabled
         let mut partition_unit = self.partition_unit.write();
         partition_unit.enabled = true;
     }
 
     /// fuse the children of this unit and also fuse the interfaces of them
-    pub fn fuse(&mut self, parent_interface: &DualModuleInterfacePtr, children_interfaces: (&DualModuleInterfacePtr, &DualModuleInterfacePtr)) {
+    pub fn fuse(
+        &mut self,
+        parent_interface: &DualModuleInterfacePtr,
+        children_interfaces: (&DualModuleInterfacePtr, &DualModuleInterfacePtr),
+    ) {
         self.static_fuse();
         let (left_interface, right_interface) = children_interfaces;
         let right_child_ptr = self.children.as_ref().unwrap().1.upgrade_force();
         lock_write!(right_child, right_child_ptr);
         // change the index of dual nodes in the right children
         let bias = left_interface.read_recursive().nodes_count();
         right_child.iterative_bias_dual_node_index(bias);
         parent_interface.fuse(left_interface, right_interface);
     }
 
     pub fn iterative_bias_dual_node_index(&mut self, bias: NodeIndex) {
         // depth-first search
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_bias_dual_node_index(bias);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_bias_dual_node_index(bias);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak.upgrade_force().write().iterative_bias_dual_node_index(bias);
+                    },
+                    || {
+                        right_child_weak.upgrade_force().write().iterative_bias_dual_node_index(bias);
+                    },
+                );
             } else {
                 left_child_weak.upgrade_force().write().iterative_bias_dual_node_index(bias);
                 right_child_weak.upgrade_force().write().iterative_bias_dual_node_index(bias);
             }
         }
         // my serial module
         self.serial_module.bias_dual_node_index(bias);
@@ -568,137 +702,223 @@
             self.execute_sync_event(sync_request);
         }
     }
 
     /// iteratively prepare all growing and shrinking and append the sync requests
     fn iterative_prepare_all(&mut self, sync_requests: &mut Vec<SyncRequest>) {
         if !self.has_active_node {
-            return  // early return to avoid going through all units
+            return; // early return to avoid going through all units
         }
         // depth-first search
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
                 let mut sync_requests_2 = vec![];
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_prepare_all(sync_requests);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_prepare_all(&mut sync_requests_2);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak.upgrade_force().write().iterative_prepare_all(sync_requests);
+                    },
+                    || {
+                        right_child_weak
+                            .upgrade_force()
+                            .write()
+                            .iterative_prepare_all(&mut sync_requests_2);
+                    },
+                );
                 sync_requests.append(&mut sync_requests_2);
             } else {
                 left_child_weak.upgrade_force().write().iterative_prepare_all(sync_requests);
                 right_child_weak.upgrade_force().write().iterative_prepare_all(sync_requests);
             }
         }
         // my serial module
         let local_sync_requests = self.serial_module.prepare_all();
         sync_requests.append(local_sync_requests);
     }
 
     /// iteratively set grow state
-    fn iterative_set_grow_state(&mut self, dual_node_ptr: &DualNodePtr, grow_state: DualNodeGrowState, representative_vertex: VertexIndex) {
+    fn iterative_set_grow_state(
+        &mut self,
+        dual_node_ptr: &DualNodePtr,
+        grow_state: DualNodeGrowState,
+        representative_vertex: VertexIndex,
+    ) {
         if !self.whole_range.contains(representative_vertex) && !self.elevated_dual_nodes.contains(dual_node_ptr) {
-            return  // no descendant related to this dual node
+            return; // no descendant related to this dual node
         }
         if grow_state != DualNodeGrowState::Stay {
             self.has_active_node = true;
         }
         // depth-first search
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
-            left_child_weak.upgrade_force().write().iterative_set_grow_state(dual_node_ptr, grow_state, representative_vertex);
-            right_child_weak.upgrade_force().write().iterative_set_grow_state(dual_node_ptr, grow_state, representative_vertex);
+            left_child_weak.upgrade_force().write().iterative_set_grow_state(
+                dual_node_ptr,
+                grow_state,
+                representative_vertex,
+            );
+            right_child_weak.upgrade_force().write().iterative_set_grow_state(
+                dual_node_ptr,
+                grow_state,
+                representative_vertex,
+            );
         }
         if self.owning_range.contains(representative_vertex) || self.serial_module.contains_dual_node(dual_node_ptr) {
             self.serial_module.set_grow_state(dual_node_ptr, grow_state);
         }
     }
 
     /// check if elevated_dual_nodes contains any dual node in the list
     pub fn elevated_dual_nodes_contains_any(&self, nodes: &[DualNodePtr]) -> bool {
         for node_ptr in nodes.iter() {
             if self.elevated_dual_nodes.contains(node_ptr) {
-                return true
+                return true;
             }
         }
         false
     }
 
     /// prepare the initial shrink of a blossom
-    fn iterative_prepare_nodes_shrink(&mut self, nodes_circle: &[DualNodePtr], nodes_circle_vertices: &[VertexIndex]
-            , sync_requests: &mut Vec<SyncRequest>) {
+    fn iterative_prepare_nodes_shrink(
+        &mut self,
+        nodes_circle: &[DualNodePtr],
+        nodes_circle_vertices: &[VertexIndex],
+        sync_requests: &mut Vec<SyncRequest>,
+    ) {
         if !self.whole_range.contains_any(nodes_circle_vertices) && !self.elevated_dual_nodes_contains_any(nodes_circle) {
-            return  // no descendant related to this dual node
+            return; // no descendant related to this dual node
         }
         self.has_active_node = true;
         // depth-first search
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
                 let mut sync_requests_2 = vec![];
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(nodes_circle, nodes_circle_vertices, sync_requests);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(nodes_circle, nodes_circle_vertices, &mut sync_requests_2);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(
+                            nodes_circle,
+                            nodes_circle_vertices,
+                            sync_requests,
+                        );
+                    },
+                    || {
+                        right_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(
+                            nodes_circle,
+                            nodes_circle_vertices,
+                            &mut sync_requests_2,
+                        );
+                    },
+                );
                 sync_requests.append(&mut sync_requests_2);
             } else {
-                left_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(nodes_circle, nodes_circle_vertices, sync_requests);
-                right_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(nodes_circle, nodes_circle_vertices, sync_requests);
+                left_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(
+                    nodes_circle,
+                    nodes_circle_vertices,
+                    sync_requests,
+                );
+                right_child_weak.upgrade_force().write().iterative_prepare_nodes_shrink(
+                    nodes_circle,
+                    nodes_circle_vertices,
+                    sync_requests,
+                );
             }
         }
         let local_sync_requests = self.serial_module.prepare_nodes_shrink(nodes_circle);
         sync_requests.append(local_sync_requests);
     }
 
-    fn iterative_add_blossom(&mut self, blossom_ptr: &DualNodePtr, nodes_circle: &[DualNodePtr], representative_vertex: VertexIndex
-            , nodes_circle_vertices: &[VertexIndex]) {
+    fn iterative_add_blossom(
+        &mut self,
+        blossom_ptr: &DualNodePtr,
+        nodes_circle: &[DualNodePtr],
+        representative_vertex: VertexIndex,
+        nodes_circle_vertices: &[VertexIndex],
+    ) {
         if !self.whole_range.contains_any(nodes_circle_vertices) && !self.elevated_dual_nodes_contains_any(nodes_circle) {
-            return  // no descendant related to this dual node
+            return; // no descendant related to this dual node
         }
         self.has_active_node = true;
         // depth-first search
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_add_blossom(blossom_ptr, nodes_circle, representative_vertex, nodes_circle_vertices);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_add_blossom(blossom_ptr, nodes_circle, representative_vertex, nodes_circle_vertices);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak.upgrade_force().write().iterative_add_blossom(
+                            blossom_ptr,
+                            nodes_circle,
+                            representative_vertex,
+                            nodes_circle_vertices,
+                        );
+                    },
+                    || {
+                        right_child_weak.upgrade_force().write().iterative_add_blossom(
+                            blossom_ptr,
+                            nodes_circle,
+                            representative_vertex,
+                            nodes_circle_vertices,
+                        );
+                    },
+                );
             } else {
-                left_child_weak.upgrade_force().write().iterative_add_blossom(blossom_ptr, nodes_circle, representative_vertex, nodes_circle_vertices);
-                right_child_weak.upgrade_force().write().iterative_add_blossom(blossom_ptr, nodes_circle, representative_vertex, nodes_circle_vertices);
+                left_child_weak.upgrade_force().write().iterative_add_blossom(
+                    blossom_ptr,
+                    nodes_circle,
+                    representative_vertex,
+                    nodes_circle_vertices,
+                );
+                right_child_weak.upgrade_force().write().iterative_add_blossom(
+                    blossom_ptr,
+                    nodes_circle,
+                    representative_vertex,
+                    nodes_circle_vertices,
+                );
             }
         }
-        if self.owning_range.contains_any(nodes_circle_vertices) || self.serial_module.contains_dual_nodes_any(nodes_circle) {
+        if self.owning_range.contains_any(nodes_circle_vertices) || self.serial_module.contains_dual_nodes_any(nodes_circle)
+        {
             self.serial_module.add_blossom(blossom_ptr);
         }
         // if I'm not on the representative path of this dual node, I need to register the propagated_dual_node
         // note that I don't need to register propagated_grandson_dual_node because it's never gonna grow inside the blossom
         if !self.whole_range.contains(representative_vertex) {
             self.elevated_dual_nodes.insert(blossom_ptr.clone());
         }
     }
 
     fn iterative_add_defect_node(&mut self, dual_node_ptr: &DualNodePtr, vertex_index: VertexIndex) {
         // if the vertex is not hold by any descendant, simply return
         if !self.is_vertex_in_descendant(vertex_index) {
-            return
+            return;
         }
         self.has_active_node = true;
         // println!("sync_prepare_growth_update_sync_event: vertex {}, unit index {}", sync_event.vertex_index, self.unit_index);
         // depth-first search
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_add_defect_node(dual_node_ptr, vertex_index);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_add_defect_node(dual_node_ptr, vertex_index);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak
+                            .upgrade_force()
+                            .write()
+                            .iterative_add_defect_node(dual_node_ptr, vertex_index);
+                    },
+                    || {
+                        right_child_weak
+                            .upgrade_force()
+                            .write()
+                            .iterative_add_defect_node(dual_node_ptr, vertex_index);
+                    },
+                );
             } else {
-                left_child_weak.upgrade_force().write().iterative_add_defect_node(dual_node_ptr, vertex_index);
-                right_child_weak.upgrade_force().write().iterative_add_defect_node(dual_node_ptr, vertex_index);
+                left_child_weak
+                    .upgrade_force()
+                    .write()
+                    .iterative_add_defect_node(dual_node_ptr, vertex_index);
+                right_child_weak
+                    .upgrade_force()
+                    .write()
+                    .iterative_add_defect_node(dual_node_ptr, vertex_index);
             }
         }
         // update on my serial module
         if self.serial_module.contains_vertex(vertex_index) {
             self.serial_module.add_defect_node(dual_node_ptr);
         }
         // if I'm not on the representative path of this dual node, I need to register the propagated_dual_node
@@ -707,136 +927,191 @@
             self.elevated_dual_nodes.insert(dual_node_ptr.clone());
         }
     }
 
     fn iterative_compute_maximum_update_length(&mut self, group_max_update_length: &mut GroupMaxUpdateLength) -> bool {
         // early terminate if no active dual nodes anywhere in the descendant
         if !self.has_active_node {
-            return false
+            return false;
         }
         let serial_module_group_max_update_length = self.serial_module.compute_maximum_update_length();
         if !serial_module_group_max_update_length.is_active() {
             self.has_active_node = false;
         }
         group_max_update_length.extend(serial_module_group_max_update_length);
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             let (left_child_has_active_node, right_child_has_active_node) = if self.enable_parallel_execution {
                 let mut group_max_update_length_2 = GroupMaxUpdateLength::new();
-                let (left_child_has_active_node, right_child_has_active_node) = rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_compute_maximum_update_length(group_max_update_length)
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_compute_maximum_update_length(&mut group_max_update_length_2)
-                });
+                let (left_child_has_active_node, right_child_has_active_node) = rayon::join(
+                    || {
+                        left_child_weak
+                            .upgrade_force()
+                            .write()
+                            .iterative_compute_maximum_update_length(group_max_update_length)
+                    },
+                    || {
+                        right_child_weak
+                            .upgrade_force()
+                            .write()
+                            .iterative_compute_maximum_update_length(&mut group_max_update_length_2)
+                    },
+                );
                 group_max_update_length.extend(group_max_update_length_2);
                 (left_child_has_active_node, right_child_has_active_node)
             } else {
-                (left_child_weak.upgrade_force().write().iterative_compute_maximum_update_length(group_max_update_length),
-                    right_child_weak.upgrade_force().write().iterative_compute_maximum_update_length(group_max_update_length))
+                (
+                    left_child_weak
+                        .upgrade_force()
+                        .write()
+                        .iterative_compute_maximum_update_length(group_max_update_length),
+                    right_child_weak
+                        .upgrade_force()
+                        .write()
+                        .iterative_compute_maximum_update_length(group_max_update_length),
+                )
             };
             if left_child_has_active_node || right_child_has_active_node {
                 self.has_active_node = true
             }
         }
         self.has_active_node
     }
 
     fn iterative_grow_dual_node(&mut self, dual_node_ptr: &DualNodePtr, length: Weight, representative_vertex: VertexIndex) {
         if !self.whole_range.contains(representative_vertex) && !self.elevated_dual_nodes.contains(dual_node_ptr) {
-            return  // no descendant related to this dual node
+            return; // no descendant related to this dual node
         }
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_grow_dual_node(dual_node_ptr, length, representative_vertex);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_grow_dual_node(dual_node_ptr, length, representative_vertex);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak.upgrade_force().write().iterative_grow_dual_node(
+                            dual_node_ptr,
+                            length,
+                            representative_vertex,
+                        );
+                    },
+                    || {
+                        right_child_weak.upgrade_force().write().iterative_grow_dual_node(
+                            dual_node_ptr,
+                            length,
+                            representative_vertex,
+                        );
+                    },
+                );
             } else {
-                left_child_weak.upgrade_force().write().iterative_grow_dual_node(dual_node_ptr, length, representative_vertex);
-                right_child_weak.upgrade_force().write().iterative_grow_dual_node(dual_node_ptr, length, representative_vertex);
+                left_child_weak.upgrade_force().write().iterative_grow_dual_node(
+                    dual_node_ptr,
+                    length,
+                    representative_vertex,
+                );
+                right_child_weak.upgrade_force().write().iterative_grow_dual_node(
+                    dual_node_ptr,
+                    length,
+                    representative_vertex,
+                );
             }
         }
         if self.owning_range.contains(representative_vertex) || self.serial_module.contains_dual_node(dual_node_ptr) {
             self.serial_module.grow_dual_node(dual_node_ptr, length);
         }
     }
 
     fn iterative_grow(&mut self, length: Weight) {
         // early terminate if no active dual nodes anywhere in the descendant
         if !self.has_active_node {
-            return
+            return;
         }
         self.serial_module.grow(length);
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_grow(length);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_grow(length);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak.upgrade_force().write().iterative_grow(length);
+                    },
+                    || {
+                        right_child_weak.upgrade_force().write().iterative_grow(length);
+                    },
+                );
             } else {
                 left_child_weak.upgrade_force().write().iterative_grow(length);
                 right_child_weak.upgrade_force().write().iterative_grow(length);
             }
         }
     }
 
     fn iterative_remove_blossom(&mut self, dual_node_ptr: &DualNodePtr, representative_vertex: VertexIndex) {
         if !self.whole_range.contains(representative_vertex) && !self.elevated_dual_nodes.contains(dual_node_ptr) {
-            return  // no descendant related to this dual node
+            return; // no descendant related to this dual node
         }
         self.has_active_node = true;
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             if self.enable_parallel_execution {
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().write().iterative_remove_blossom(dual_node_ptr, representative_vertex);
-                }, || {
-                    right_child_weak.upgrade_force().write().iterative_remove_blossom(dual_node_ptr, representative_vertex);
-                });
+                rayon::join(
+                    || {
+                        left_child_weak
+                            .upgrade_force()
+                            .write()
+                            .iterative_remove_blossom(dual_node_ptr, representative_vertex);
+                    },
+                    || {
+                        right_child_weak
+                            .upgrade_force()
+                            .write()
+                            .iterative_remove_blossom(dual_node_ptr, representative_vertex);
+                    },
+                );
             } else {
-                left_child_weak.upgrade_force().write().iterative_remove_blossom(dual_node_ptr, representative_vertex);
-                right_child_weak.upgrade_force().write().iterative_remove_blossom(dual_node_ptr, representative_vertex);
+                left_child_weak
+                    .upgrade_force()
+                    .write()
+                    .iterative_remove_blossom(dual_node_ptr, representative_vertex);
+                right_child_weak
+                    .upgrade_force()
+                    .write()
+                    .iterative_remove_blossom(dual_node_ptr, representative_vertex);
             }
         }
         if self.owning_range.contains(representative_vertex) || self.serial_module.contains_dual_node(dual_node_ptr) {
             self.serial_module.remove_blossom(dual_node_ptr.clone());
         }
     }
-
 }
 
 impl<SerialModule: DualModuleImpl + Send + Sync> DualModuleParallelUnitPtr<SerialModule> {
-
     /// create a simple wrapper over a serial dual module
-    pub fn new_wrapper(serial_module: SerialModule, unit_index: usize, partition_info: Arc<PartitionInfo>, partition_unit: PartitionUnitPtr
-            , enable_parallel_execution: bool) -> Self {
+    pub fn new_wrapper(
+        serial_module: SerialModule,
+        unit_index: usize,
+        partition_info: Arc<PartitionInfo>,
+        partition_unit: PartitionUnitPtr,
+        enable_parallel_execution: bool,
+    ) -> Self {
         let partition_unit_info = &partition_info.units[unit_index];
         Self::new_value(DualModuleParallelUnit {
             unit_index,
             partition_info: partition_info.clone(),
             partition_unit,
-            is_active: partition_unit_info.children.is_none(),  // only activate the leaves in the dependency tree
+            is_active: partition_unit_info.children.is_none(), // only activate the leaves in the dependency tree
             whole_range: partition_unit_info.whole_range,
             owning_range: partition_unit_info.owning_range,
-            extra_descendant_mirrored_vertices: HashSet::new(),  // to be filled later
+            extra_descendant_mirrored_vertices: HashSet::new(), // to be filled later
             serial_module,
-            children: None,  // to be filled later
-            parent: None,  // to be filled later
+            children: None, // to be filled later
+            parent: None,   // to be filled later
             elevated_dual_nodes: PtrWeakHashSet::new(),
             empty_sync_request: vec![],
             enable_parallel_execution,
-            has_active_node: true,  // by default to true, because children may have active nodes
+            has_active_node: true, // by default to true, because children may have active nodes
         })
     }
-
 }
 
 /// We cannot implement async function because a RwLockWriteGuard implements !Send
 impl<SerialModule: DualModuleImpl + Send + Sync> DualModuleImpl for DualModuleParallelUnit<SerialModule> {
-
     /// clear all growth and existing dual nodes
     fn new_empty(_initializer: &SolverInitializer) -> Self {
         panic!("creating parallel unit directly from initializer is forbidden, use `DualModuleParallel::new` instead");
     }
 
     /// clear all growth and existing dual nodes
     fn clear(&mut self) {
@@ -847,88 +1122,129 @@
     /// add a new dual node from dual module root
     fn add_dual_node(&mut self, dual_node_ptr: &DualNodePtr) {
         self.has_active_node = true;
         let representative_vertex = dual_node_ptr.get_representative_vertex();
         match &dual_node_ptr.read_recursive().class {
             // fast path: if dual node is a single vertex, then only add to the owning node; single vertex dual node can only add when dual variable = 0
             DualNodeClass::DefectVertex { defect_index } => {
-                if self.owning_range.contains(representative_vertex) {  // fast path: the most common one
+                if self.owning_range.contains(representative_vertex) {
+                    // fast path: the most common one
                     self.iterative_add_defect_node(dual_node_ptr, *defect_index);
                 } else {
                     // find the one that owns it and add the dual node, and then add the serial_module
                     if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
-                        let mut child_ptr = if representative_vertex < self.owning_range.start() { left_child_weak.upgrade_force() } else { right_child_weak.upgrade_force() };
+                        let mut child_ptr = if representative_vertex < self.owning_range.start() {
+                            left_child_weak.upgrade_force()
+                        } else {
+                            right_child_weak.upgrade_force()
+                        };
                         let mut is_owning_dual_node = false;
                         while !is_owning_dual_node {
                             let mut child = child_ptr.write();
                             child.has_active_node = true;
-                            debug_assert!(child.whole_range.contains(representative_vertex), "selected child must contains the vertex");
+                            debug_assert!(
+                                child.whole_range.contains(representative_vertex),
+                                "selected child must contains the vertex"
+                            );
                             is_owning_dual_node = child.owning_range.contains(representative_vertex);
-                            if !is_owning_dual_node {  // search for the grandsons
-                                let grandson_ptr = if let Some((left_child_weak, right_child_weak)) = child.children.as_ref() {
-                                    if representative_vertex < child.owning_range.start() { left_child_weak.upgrade_force() } else { right_child_weak.upgrade_force() }
-                                } else { unreachable!() };
+                            if !is_owning_dual_node {
+                                // search for the grandsons
+                                let grandson_ptr = if let Some((left_child_weak, right_child_weak)) = child.children.as_ref()
+                                {
+                                    if representative_vertex < child.owning_range.start() {
+                                        left_child_weak.upgrade_force()
+                                    } else {
+                                        right_child_weak.upgrade_force()
+                                    }
+                                } else {
+                                    unreachable!()
+                                };
                                 drop(child);
                                 child_ptr = grandson_ptr;
                             }
                         }
                         lock_write!(child, child_ptr);
                         child.iterative_add_defect_node(dual_node_ptr, *defect_index);
-                    } else { unreachable!() }
+                    } else {
+                        unreachable!()
+                    }
                 }
                 // if it's children mirrors this vertex as well, then it's necessary to add this dual node to those children as well
-            },
+            }
             // this is a blossom, meaning it's children dual nodes may reside on any path
             DualNodeClass::Blossom { nodes_circle, .. } => {
                 // first set all children dual nodes as shrinking, to be safe
                 let nodes_circle_ptrs: Vec<_> = nodes_circle.iter().map(|weak| weak.upgrade_force()).collect();
-                let nodes_circle_vertices: Vec<_> = nodes_circle.iter().map(|weak| weak.upgrade_force().get_representative_vertex()).collect();
+                let nodes_circle_vertices: Vec<_> = nodes_circle
+                    .iter()
+                    .map(|weak| weak.upgrade_force().get_representative_vertex())
+                    .collect();
                 self.prepare_nodes_shrink(&nodes_circle_ptrs);
-                self.iterative_add_blossom(dual_node_ptr, &nodes_circle_ptrs, representative_vertex, &nodes_circle_vertices);
-            },
+                self.iterative_add_blossom(
+                    dual_node_ptr,
+                    &nodes_circle_ptrs,
+                    representative_vertex,
+                    &nodes_circle_vertices,
+                );
+            }
         }
     }
 
     fn remove_blossom(&mut self, dual_node_ptr: DualNodePtr) {
         let representative_vertex = dual_node_ptr.get_representative_vertex();
         self.iterative_remove_blossom(&dual_node_ptr, representative_vertex);
     }
 
     fn set_grow_state(&mut self, dual_node_ptr: &DualNodePtr, grow_state: DualNodeGrowState) {
         // println!("unit {} set_grow_state {:?} {:?}", self.unit_index, dual_node_ptr, grow_state);
         // find the path towards the owning unit of this dual node, and also try paths towards the elevated
         let representative_vertex = dual_node_ptr.get_representative_vertex();
-        debug_assert!(self.whole_range.contains(representative_vertex), "cannot set growth state of dual node outside of the scope");
+        debug_assert!(
+            self.whole_range.contains(representative_vertex),
+            "cannot set growth state of dual node outside of the scope"
+        );
         self.iterative_set_grow_state(dual_node_ptr, grow_state, representative_vertex);
     }
 
-    fn compute_maximum_update_length_dual_node(&mut self, dual_node_ptr: &DualNodePtr, is_grow: bool, simultaneous_update: bool) -> MaxUpdateLength {
+    fn compute_maximum_update_length_dual_node(
+        &mut self,
+        dual_node_ptr: &DualNodePtr,
+        is_grow: bool,
+        simultaneous_update: bool,
+    ) -> MaxUpdateLength {
         // TODO: execute on all nodes that handles this dual node
-        let max_update_length = self.serial_module.compute_maximum_update_length_dual_node(dual_node_ptr, is_grow, simultaneous_update);
-        if !(self.children.is_none() && self.is_active) {  // for those base partitions without being fused, we don't need to update
-            max_update_length.update();  // only necessary after involved in fusion
+        let max_update_length =
+            self.serial_module
+                .compute_maximum_update_length_dual_node(dual_node_ptr, is_grow, simultaneous_update);
+        if !(self.children.is_none() && self.is_active) {
+            // for those base partitions without being fused, we don't need to update
+            max_update_length.update(); // only necessary after involved in fusion
         }
         max_update_length
     }
 
     fn compute_maximum_update_length(&mut self) -> GroupMaxUpdateLength {
         // first prepare all dual node for growth and shrink accordingly and synchronize them
         self.prepare_all();
         // them do the functions independently
         let mut group_max_update_length = GroupMaxUpdateLength::new();
         self.iterative_compute_maximum_update_length(&mut group_max_update_length);
-        if !(self.children.is_none() && self.is_active) {  // for those base partitions without being fused, we don't need to update
-            group_max_update_length.update();  // only necessary after involved in fusion
+        if !(self.children.is_none() && self.is_active) {
+            // for those base partitions without being fused, we don't need to update
+            group_max_update_length.update(); // only necessary after involved in fusion
         }
         group_max_update_length
     }
 
     fn grow_dual_node(&mut self, dual_node_ptr: &DualNodePtr, length: Weight) {
         let representative_vertex = dual_node_ptr.get_representative_vertex();
-        debug_assert!(self.whole_range.contains(representative_vertex), "cannot grow dual node outside of the scope");
+        debug_assert!(
+            self.whole_range.contains(representative_vertex),
+            "cannot grow dual node outside of the scope"
+        );
         self.iterative_grow_dual_node(dual_node_ptr, length, representative_vertex);
     }
 
     fn grow(&mut self, length: Weight) {
         self.iterative_grow(length);
     }
 
@@ -940,15 +1256,15 @@
 
     fn prepare_nodes_shrink(&mut self, nodes_circle: &[DualNodePtr]) -> &mut Vec<SyncRequest> {
         let nodes_circle_vertices: Vec<_> = nodes_circle.iter().map(|ptr| ptr.get_representative_vertex()).collect();
         let mut sync_requests = vec![];
         loop {
             self.iterative_prepare_nodes_shrink(nodes_circle, &nodes_circle_vertices, &mut sync_requests);
             if sync_requests.is_empty() {
-                break
+                break;
             }
             // println!("sync_requests: {sync_requests:?}");
             self.execute_sync_events(&sync_requests);
             sync_requests.clear();
         }
         &mut self.empty_sync_request
     }
@@ -957,28 +1273,28 @@
         if self.children.is_none() {
             // don't do anything, not even prepare the growth because it will be done in the serial module
         } else {
             let mut sync_requests = vec![];
             loop {
                 self.iterative_prepare_all(&mut sync_requests);
                 if sync_requests.is_empty() {
-                    break
+                    break;
                 }
                 // println!("sync_requests: {sync_requests:?}");
                 self.execute_sync_events(&sync_requests);
                 sync_requests.clear();
             }
         }
         &mut self.empty_sync_request
     }
 
     fn execute_sync_event(&mut self, sync_event: &SyncRequest) {
         // if the vertex is not hold by any descendant, simply return
         if !self.is_vertex_in_descendant(sync_event.vertex_index) {
-            return
+            return;
         }
         self.has_active_node = true;
         // println!("sync_prepare_growth_update_sync_event: vertex {}, unit index {}", sync_event.vertex_index, self.unit_index);
         // depth-first search
         if let Some((left_child_weak, right_child_weak)) = self.children.as_ref() {
             left_child_weak.upgrade_force().write().execute_sync_event(sync_event);
             right_child_weak.upgrade_force().write().execute_sync_event(sync_event);
@@ -986,21 +1302,27 @@
         // update on my serial module
         if self.serial_module.contains_vertex(sync_event.vertex_index) {
             // println!("update: vertex {}, unit index {}", sync_event.vertex_index, self.unit_index);
             self.serial_module.execute_sync_event(sync_event);
         }
         // if I'm not on the representative path of this dual node, I need to register the propagated_dual_node
         // note that I don't need to register propagated_grandson_dual_node because it's never gonna grow inside the blossom
-        if !self.whole_range.contains(sync_event.vertex_index) {
-            if let Some((propagated_dual_node_weak, _)) = sync_event.propagated_dual_node.as_ref() {
+        if let Some((propagated_dual_node_weak, _, representative_vertex)) = sync_event.propagated_dual_node.as_ref() {
+            if !self.whole_range.contains(*representative_vertex) {
+                self.elevated_dual_nodes.insert(propagated_dual_node_weak.upgrade_force());
+            }
+        }
+        if let Some((propagated_dual_node_weak, _, representative_vertex)) =
+            sync_event.propagated_grandson_dual_node.as_ref()
+        {
+            if !self.whole_range.contains(*representative_vertex) {
                 self.elevated_dual_nodes.insert(propagated_dual_node_weak.upgrade_force());
             }
         }
     }
-
 }
 
 /// interface consists of several vertices; each vertex exists as a virtual vertex in several different serial dual modules.
 /// each virtual vertex exists in at most one interface
 pub struct InterfaceData {
     /// the serial dual modules that processes these virtual vertices,
     pub possession_modules: Vec<DualModuleSerialWeak>,
@@ -1012,394 +1334,527 @@
 pub struct Interface {
     /// unique interface id for ease of zero-cost switching
     pub interface_id: usize,
     /// link to interface data
     pub data: Weak<InterfaceData>,
 }
 
-
 #[cfg(test)]
 pub mod tests {
-    use super::*;
     use super::super::example_codes::*;
     use super::super::primal_module::*;
     use super::super::primal_module_serial::*;
+    use super::*;
 
-    pub fn dual_module_parallel_basic_standard_syndrome_optional_viz<F>(mut code: impl ExampleCode, visualize_filename: Option<String>
-            , mut defect_vertices: Vec<VertexIndex>, final_dual: Weight, partition_func: F, reordered_vertices: Option<Vec<VertexIndex>>)
-            -> (DualModuleInterfacePtr, PrimalModuleSerialPtr, DualModuleParallel<DualModuleSerial>) where F: Fn(&SolverInitializer, &mut PartitionConfig) {
+    pub fn dual_module_parallel_basic_standard_syndrome_optional_viz<F>(
+        mut code: impl ExampleCode,
+        visualize_filename: Option<String>,
+        mut defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+        partition_func: F,
+        reordered_vertices: Option<Vec<VertexIndex>>,
+    ) -> (
+        DualModuleInterfacePtr,
+        PrimalModuleSerialPtr,
+        DualModuleParallel<DualModuleSerial>,
+    )
+    where
+        F: Fn(&SolverInitializer, &mut PartitionConfig),
+    {
         println!("{defect_vertices:?}");
         if let Some(reordered_vertices) = &reordered_vertices {
             code.reorder_vertices(reordered_vertices);
             defect_vertices = translated_defect_to_reordered(reordered_vertices, &defect_vertices);
         }
         let mut visualizer = match visualize_filename.as_ref() {
             Some(visualize_filename) => {
-                let visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+                let visualizer = Visualizer::new(
+                    Some(visualize_data_folder() + visualize_filename.as_str()),
+                    code.get_positions(),
+                    true,
+                )
+                .unwrap();
                 print_visualize_link(visualize_filename.clone());
                 Some(visualizer)
-            }, None => None
+            }
+            None => None,
         };
         let initializer = code.get_initializer();
         let mut partition_config = PartitionConfig::new(initializer.vertex_num);
         partition_func(&initializer, &mut partition_config);
         println!("partition_config: {partition_config:?}");
         let partition_info = partition_config.info();
         // create dual module
-        let mut dual_module = DualModuleParallel::new_config(&initializer, &partition_info, DualModuleParallelConfig::default());
+        let mut dual_module =
+            DualModuleParallel::new_config(&initializer, &partition_info, DualModuleParallelConfig::default());
         dual_module.static_fuse_all();
         // create primal module
         let mut primal_module = PrimalModuleSerialPtr::new_empty(&initializer);
-        primal_module.write().debug_resolve_only_one = true;  // to enable debug mode
-        // try to work on a simple syndrome
+        primal_module.write().debug_resolve_only_one = true; // to enable debug mode
+                                                             // try to work on a simple syndrome
         code.set_defect_vertices(&defect_vertices);
         let interface_ptr = DualModuleInterfacePtr::new_empty();
         primal_module.solve_visualizer(&interface_ptr, &code.get_syndrome(), &mut dual_module, visualizer.as_mut());
         let perfect_matching = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         let mut subgraph_builder = SubGraphBuilder::new(&initializer);
         subgraph_builder.load_perfect_matching(&perfect_matching);
         let subgraph = subgraph_builder.get_subgraph();
         if let Some(visualizer) = visualizer.as_mut() {
-            visualizer.snapshot_combined("perfect matching and subgraph".to_string(), vec![&interface_ptr, &dual_module
-                , &perfect_matching, &VisualizeSubgraph::new(&subgraph)]).unwrap();
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), subgraph_builder.total_weight(), "unmatched sum dual variables");
-        assert_eq!(interface_ptr.sum_dual_variables(), final_dual * 2, "unexpected final dual variable sum");
+            visualizer
+                .snapshot_combined(
+                    "perfect matching and subgraph".to_string(),
+                    vec![
+                        &interface_ptr,
+                        &dual_module,
+                        &perfect_matching,
+                        &VisualizeSubgraph::new(&subgraph),
+                    ],
+                )
+                .unwrap();
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            subgraph_builder.total_weight(),
+            "unmatched sum dual variables"
+        );
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            final_dual * 2,
+            "unexpected final dual variable sum"
+        );
         (interface_ptr, primal_module, dual_module)
     }
 
-    pub fn dual_module_parallel_standard_syndrome<F>(code: impl ExampleCode, visualize_filename: String, defect_vertices: Vec<VertexIndex>
-            , final_dual: Weight, partition_func: F, reordered_vertices: Option<Vec<VertexIndex>>)
-            -> (DualModuleInterfacePtr, PrimalModuleSerialPtr, DualModuleParallel<DualModuleSerial>) where F: Fn(&SolverInitializer, &mut PartitionConfig) {
-        dual_module_parallel_basic_standard_syndrome_optional_viz(code, Some(visualize_filename), defect_vertices, final_dual, partition_func, reordered_vertices)
+    pub fn dual_module_parallel_standard_syndrome<F>(
+        code: impl ExampleCode,
+        visualize_filename: String,
+        defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+        partition_func: F,
+        reordered_vertices: Option<Vec<VertexIndex>>,
+    ) -> (
+        DualModuleInterfacePtr,
+        PrimalModuleSerialPtr,
+        DualModuleParallel<DualModuleSerial>,
+    )
+    where
+        F: Fn(&SolverInitializer, &mut PartitionConfig),
+    {
+        dual_module_parallel_basic_standard_syndrome_optional_viz(
+            code,
+            Some(visualize_filename),
+            defect_vertices,
+            final_dual,
+            partition_func,
+            reordered_vertices,
+        )
     }
 
     /// test a simple case
     #[test]
-    fn dual_module_parallel_basic_1() {  // cargo test dual_module_parallel_basic_1 -- --nocapture
+    fn dual_module_parallel_basic_1() {
+        // cargo test dual_module_parallel_basic_1 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_basic_1.json");
         let defect_vertices = vec![39, 52, 63, 90, 100];
         let half_weight = 500;
-        dual_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |initializer, _config| {
-            println!("initializer: {initializer:?}");
-        }, None);
+        dual_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |initializer, _config| {
+                println!("initializer: {initializer:?}");
+            },
+            None,
+        );
     }
 
     /// split into 2, with no syndrome vertex on the interface
     #[test]
-    fn dual_module_parallel_basic_2() {  // cargo test dual_module_parallel_basic_2 -- --nocapture
+    fn dual_module_parallel_basic_2() {
+        // cargo test dual_module_parallel_basic_2 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_basic_2.json");
         let defect_vertices = vec![39, 52, 63, 90, 100];
         let half_weight = 500;
-        dual_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 72),    // unit 0
-                VertexRange::new(84, 132),  // unit 1
-            ];
-            config.fusions = vec![
-                (0, 1),  // unit 2, by fusing 0 and 1
-            ];
-        }, None);
+        dual_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 72),   // unit 0
+                    VertexRange::new(84, 132), // unit 1
+                ];
+                config.fusions = vec![
+                    (0, 1), // unit 2, by fusing 0 and 1
+                ];
+            },
+            None,
+        );
     }
 
     /// split into 2, with a syndrome vertex on the interface
     #[test]
-    fn dual_module_parallel_basic_3() {  // cargo test dual_module_parallel_basic_3 -- --nocapture
+    fn dual_module_parallel_basic_3() {
+        // cargo test dual_module_parallel_basic_3 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_basic_3.json");
         let defect_vertices = vec![39, 52, 63, 90, 100];
         let half_weight = 500;
-        dual_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 60),    // unit 0
-                VertexRange::new(72, 132),  // unit 1
-            ];
-            config.fusions = vec![
-                (0, 1),  // unit 2, by fusing 0 and 1
-            ];
-        }, None);
+        dual_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 60),   // unit 0
+                    VertexRange::new(72, 132), // unit 1
+                ];
+                config.fusions = vec![
+                    (0, 1), // unit 2, by fusing 0 and 1
+                ];
+            },
+            None,
+        );
     }
 
     /// split into 4, with no syndrome vertex on the interface
     #[test]
-    fn dual_module_parallel_basic_4() {  // cargo test dual_module_parallel_basic_4 -- --nocapture
+    fn dual_module_parallel_basic_4() {
+        // cargo test dual_module_parallel_basic_4 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_basic_4.json");
         // reorder vertices to enable the partition;
-        let defect_vertices = vec![39, 52, 63, 90, 100];  // indices are before the reorder
+        let defect_vertices = vec![39, 52, 63, 90, 100]; // indices are before the reorder
         let half_weight = 500;
-        dual_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 36),
-                VertexRange::new(42, 72),
-                VertexRange::new(84, 108),
-                VertexRange::new(112, 132),
-            ];
-            config.fusions = vec![
-                (0, 1),
-                (2, 3),
-                (4, 5),
-            ];
-        }, Some((|| {
-            let mut reordered_vertices = vec![];
-            let split_horizontal = 6;
-            let split_vertical = 5;
-            for i in 0..split_horizontal {  // left-top block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
+        dual_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 36),
+                    VertexRange::new(42, 72),
+                    VertexRange::new(84, 108),
+                    VertexRange::new(112, 132),
+                ];
+                config.fusions = vec![(0, 1), (2, 3), (4, 5)];
+            },
+            Some((|| {
+                let mut reordered_vertices = vec![];
+                let split_horizontal = 6;
+                let split_vertical = 5;
+                for i in 0..split_horizontal {
+                    // left-top block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
                 }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in 0..split_horizontal {  // interface between the left-top block and the right-top block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in 0..split_horizontal {  // right-top block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
+                for i in 0..split_horizontal {
+                    // interface between the left-top block and the right-top block
+                    reordered_vertices.push(i * 12 + split_vertical);
                 }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            {  // the big interface between top and bottom
-                for j in 0..12 {
-                    reordered_vertices.push(split_horizontal * 12 + j);
+                for i in 0..split_horizontal {
+                    // right-top block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
                 }
-            }
-            for i in (split_horizontal+1)..11 {  // left-bottom block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
+                {
+                    // the big interface between top and bottom
+                    for j in 0..12 {
+                        reordered_vertices.push(split_horizontal * 12 + j);
+                    }
                 }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in (split_horizontal+1)..11 {  // interface between the left-bottom block and the right-bottom block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in (split_horizontal+1)..11 {  // right-bottom block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
+                for i in (split_horizontal + 1)..11 {
+                    // left-bottom block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
                 }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            reordered_vertices
-        })()));
+                for i in (split_horizontal + 1)..11 {
+                    // interface between the left-bottom block and the right-bottom block
+                    reordered_vertices.push(i * 12 + split_vertical);
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // right-bottom block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
+                }
+                reordered_vertices
+            })()),
+        );
     }
 
     /// split into 4, with 2 defect vertices on parent interfaces
     #[test]
-    fn dual_module_parallel_basic_5() {  // cargo test dual_module_parallel_basic_5 -- --nocapture
+    fn dual_module_parallel_basic_5() {
+        // cargo test dual_module_parallel_basic_5 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_basic_5.json");
         // reorder vertices to enable the partition;
-        let defect_vertices = vec![39, 52, 63, 90, 100];  // indices are before the reorder
+        let defect_vertices = vec![39, 52, 63, 90, 100]; // indices are before the reorder
         let half_weight = 500;
-        dual_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 25),
-                VertexRange::new(30, 60),
-                VertexRange::new(72, 97),
-                VertexRange::new(102, 132),
-            ];
-            config.fusions = vec![
-                (0, 1),
-                (2, 3),
-                (4, 5),
-            ];
-        }, Some((|| {
-            let mut reordered_vertices = vec![];
-            let split_horizontal = 5;
-            let split_vertical = 4;
-            for i in 0..split_horizontal {  // left-top block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
+        dual_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 25),
+                    VertexRange::new(30, 60),
+                    VertexRange::new(72, 97),
+                    VertexRange::new(102, 132),
+                ];
+                config.fusions = vec![(0, 1), (2, 3), (4, 5)];
+            },
+            Some((|| {
+                let mut reordered_vertices = vec![];
+                let split_horizontal = 5;
+                let split_vertical = 4;
+                for i in 0..split_horizontal {
+                    // left-top block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
                 }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in 0..split_horizontal {  // interface between the left-top block and the right-top block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in 0..split_horizontal {  // right-top block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
+                for i in 0..split_horizontal {
+                    // interface between the left-top block and the right-top block
+                    reordered_vertices.push(i * 12 + split_vertical);
                 }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            {  // the big interface between top and bottom
-                for j in 0..12 {
-                    reordered_vertices.push(split_horizontal * 12 + j);
+                for i in 0..split_horizontal {
+                    // right-top block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
                 }
-            }
-            for i in (split_horizontal+1)..11 {  // left-bottom block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
+                {
+                    // the big interface between top and bottom
+                    for j in 0..12 {
+                        reordered_vertices.push(split_horizontal * 12 + j);
+                    }
                 }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in (split_horizontal+1)..11 {  // interface between the left-bottom block and the right-bottom block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in (split_horizontal+1)..11 {  // right-bottom block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
+                for i in (split_horizontal + 1)..11 {
+                    // left-bottom block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
                 }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            reordered_vertices
-        })()));
+                for i in (split_horizontal + 1)..11 {
+                    // interface between the left-bottom block and the right-bottom block
+                    reordered_vertices.push(i * 12 + split_vertical);
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // right-bottom block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
+                }
+                reordered_vertices
+            })()),
+        );
     }
 
-    fn dual_module_parallel_debug_repetition_code_common(d: VertexNum, visualize_filename: String, defect_vertices: Vec<VertexIndex>, final_dual: Weight) {
+    fn dual_module_parallel_debug_repetition_code_common(
+        d: VertexNum,
+        visualize_filename: String,
+        defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+    ) {
         let half_weight = 500;
         let split_vertical = (d + 1) / 2;
-        dual_module_parallel_standard_syndrome(CodeCapacityRepetitionCode::new(d, 0.1, half_weight), visualize_filename, defect_vertices, final_dual * half_weight, |initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, split_vertical + 1),
-                VertexRange::new(split_vertical + 2, initializer.vertex_num),
-            ];
-            config.fusions = vec![
-                (0, 1),
-            ];
-        }, Some((|| {
-            let mut reordered_vertices = vec![];
-            for j in 0..split_vertical {
-                reordered_vertices.push(j);
-            }
-            reordered_vertices.push(d);
-            for j in split_vertical..d {
-                reordered_vertices.push(j);
-            }
-            reordered_vertices
-        })()));
+        dual_module_parallel_standard_syndrome(
+            CodeCapacityRepetitionCode::new(d, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            final_dual * half_weight,
+            |initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, split_vertical + 1),
+                    VertexRange::new(split_vertical + 2, initializer.vertex_num),
+                ];
+                config.fusions = vec![(0, 1)];
+            },
+            Some((|| {
+                let mut reordered_vertices = vec![];
+                for j in 0..split_vertical {
+                    reordered_vertices.push(j);
+                }
+                reordered_vertices.push(d);
+                for j in split_vertical..d {
+                    reordered_vertices.push(j);
+                }
+                reordered_vertices
+            })()),
+        );
     }
 
     /// debug blossom not growing properly
     #[test]
-    fn dual_module_parallel_debug_1() {  // cargo test dual_module_parallel_debug_1 -- --nocapture
+    fn dual_module_parallel_debug_1() {
+        // cargo test dual_module_parallel_debug_1 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_1.json");
-        let defect_vertices = vec![2, 3, 4, 5, 6, 7, 8];  // indices are before the reorder
+        let defect_vertices = vec![2, 3, 4, 5, 6, 7, 8]; // indices are before the reorder
         dual_module_parallel_debug_repetition_code_common(11, visualize_filename, defect_vertices, 5);
     }
 
     /// debug 'internal error: entered unreachable code: VertexShrinkStop conflict cannot be solved by primal module
     /// the reason of this bug is that a shrinking node on the interface is sandwiched by two growing nodes resides on different children units
     /// for the serial implementation, this event can be easily handled by doing special configs
     /// but for the fused units, how to do it?
     /// This is the benefit of using software to develop first; if directly working on the hardware implementation, one would have to add more interface
     /// to support it, which could be super time-consuming
     #[test]
-    fn dual_module_parallel_debug_2() {  // cargo test dual_module_parallel_debug_2 -- --nocapture
+    fn dual_module_parallel_debug_2() {
+        // cargo test dual_module_parallel_debug_2 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_2.json");
-        let defect_vertices = vec![5, 6, 7];  // indices are before the reorder
+        let defect_vertices = vec![5, 6, 7]; // indices are before the reorder
         dual_module_parallel_debug_repetition_code_common(11, visualize_filename, defect_vertices, 4);
     }
 
-    /// the reason for this bug is that I forgot to set dual_variable correctly, leading to false VertexShrinkStop event at the 
+    /// the reason for this bug is that I forgot to set dual_variable correctly, leading to false VertexShrinkStop event at the
     #[test]
-    fn dual_module_parallel_debug_3() {  // cargo test dual_module_parallel_debug_3 -- --nocapture
+    fn dual_module_parallel_debug_3() {
+        // cargo test dual_module_parallel_debug_3 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_3.json");
-        let defect_vertices = vec![3, 5, 7];  // indices are before the reorder
+        let defect_vertices = vec![3, 5, 7]; // indices are before the reorder
         dual_module_parallel_debug_repetition_code_common(11, visualize_filename, defect_vertices, 5);
     }
 
     /// incorrect final result
     /// the reason is I didn't search through all the representative vertices of all children nodes, causing the parent blossom not propagating correctly
     #[test]
-    fn dual_module_parallel_debug_4() {  // cargo test dual_module_parallel_debug_4 -- --nocapture
+    fn dual_module_parallel_debug_4() {
+        // cargo test dual_module_parallel_debug_4 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_4.json");
-        let defect_vertices = vec![2, 3, 5, 6, 7];  // indices are before the reorder
+        let defect_vertices = vec![2, 3, 5, 6, 7]; // indices are before the reorder
         dual_module_parallel_debug_repetition_code_common(11, visualize_filename, defect_vertices, 5);
     }
 
     /// unwrap fail on dual node to internal dual node
     /// the reason is I forgot to implement the remove_blossom API...
     #[test]
-    fn dual_module_parallel_debug_5() {  // cargo test dual_module_parallel_debug_5 -- --nocapture
+    fn dual_module_parallel_debug_5() {
+        // cargo test dual_module_parallel_debug_5 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_5.json");
-        let defect_vertices = vec![0, 4, 7, 8, 9, 11];  // indices are before the reorder
+        let defect_vertices = vec![0, 4, 7, 8, 9, 11]; // indices are before the reorder
         dual_module_parallel_debug_repetition_code_common(15, visualize_filename, defect_vertices, 7);
     }
 
-    fn dual_module_parallel_debug_planar_code_common(d: VertexNum, visualize_filename: String, defect_vertices: Vec<VertexIndex>, final_dual: Weight) {
+    fn dual_module_parallel_debug_planar_code_common(
+        d: VertexNum,
+        visualize_filename: String,
+        defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+    ) {
         let half_weight = 500;
         let split_horizontal = (d + 1) / 2;
         let row_count = d + 1;
-        dual_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(d, 0.1, half_weight), visualize_filename, defect_vertices, final_dual * half_weight, |initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, split_horizontal * row_count),
-                VertexRange::new((split_horizontal + 1) * row_count, initializer.vertex_num),
-            ];
-            config.fusions = vec![
-                (0, 1),
-            ];
-        }, None);
+        dual_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(d, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            final_dual * half_weight,
+            |initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, split_horizontal * row_count),
+                    VertexRange::new((split_horizontal + 1) * row_count, initializer.vertex_num),
+                ];
+                config.fusions = vec![(0, 1)];
+            },
+            None,
+        );
     }
 
     /// panic 'one cannot conflict with itself, double check to avoid deadlock'
     /// reason: when merging two `VertexShrinkStop` events into a single `Conflicting` event, I forget to check whether the two pointers are the same;
     /// if so, I should simply ignore it
     #[test]
-    fn dual_module_parallel_debug_6() {  // cargo test dual_module_parallel_debug_6 -- --nocapture
+    fn dual_module_parallel_debug_6() {
+        // cargo test dual_module_parallel_debug_6 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_6.json");
-        let defect_vertices = vec![10, 11, 13, 32, 36, 37, 40, 44];  // indices are before the reorder
+        let defect_vertices = vec![10, 11, 13, 32, 36, 37, 40, 44]; // indices are before the reorder
         dual_module_parallel_debug_planar_code_common(7, visualize_filename, defect_vertices, 5);
     }
 
     /// panic 'one cannot conflict with itself, double check to avoid deadlock'
     /// reason: when comparing the pointers of two `VertexShrinkStop` events, only compare their conflicting dual node, not the touching dual node
     #[test]
-    fn dual_module_parallel_debug_7() {  // cargo test dual_module_parallel_debug_7 -- --nocapture
+    fn dual_module_parallel_debug_7() {
+        // cargo test dual_module_parallel_debug_7 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_7.json");
-        let defect_vertices = vec![3, 12, 21, 24, 27, 28, 33, 35, 36, 43, 50, 51];  // indices are before the reorder
+        let defect_vertices = vec![3, 12, 21, 24, 27, 28, 33, 35, 36, 43, 50, 51]; // indices are before the reorder
         dual_module_parallel_debug_planar_code_common(7, visualize_filename, defect_vertices, 10);
     }
 
     /// panic `Option::unwrap()` on a `None` value', src/dual_module.rs:242:1
     #[test]
-    fn dual_module_parallel_debug_8() {  // cargo test dual_module_parallel_debug_8 -- --nocapture
+    fn dual_module_parallel_debug_8() {
+        // cargo test dual_module_parallel_debug_8 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_8.json");
-        let defect_vertices = vec![1, 2, 3, 4, 9, 10, 13, 16, 17, 19, 24, 29, 33, 36, 37, 44, 48, 49, 51, 52];  // indices are before the reorder
+        let defect_vertices = vec![1, 2, 3, 4, 9, 10, 13, 16, 17, 19, 24, 29, 33, 36, 37, 44, 48, 49, 51, 52]; // indices are before the reorder
         dual_module_parallel_debug_planar_code_common(7, visualize_filename, defect_vertices, 13);
     }
 
     /// panicked at 'dual node of edge should be some', src/dual_module_serial.rs:379:13
     /// reason: blossom's boundary has duplicate edges, solved by adding dedup functionality to edges
     #[test]
-    fn dual_module_parallel_debug_9() {  // cargo test dual_module_parallel_debug_9 -- --nocapture
+    fn dual_module_parallel_debug_9() {
+        // cargo test dual_module_parallel_debug_9 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_9.json");
-        let defect_vertices = vec![60, 61, 72, 74, 84, 85, 109];  // indices are before the reorder
+        let defect_vertices = vec![60, 61, 72, 74, 84, 85, 109]; // indices are before the reorder
         dual_module_parallel_debug_planar_code_common(11, visualize_filename, defect_vertices, 6);
     }
 
     /// infinite loop at group_max_update_length: Conflicts(([Conflicting((12, 4), (15, 5))], {}))
     /// reason: I falsely use representative_vertex of the blossom instead of the representative vertices in the nodes circle in sync_prepare_blossom_initial_shrink
     #[test]
-    fn dual_module_parallel_debug_10() {  // cargo test dual_module_parallel_debug_10 -- --nocapture
+    fn dual_module_parallel_debug_10() {
+        // cargo test dual_module_parallel_debug_10 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_10.json");
-        let defect_vertices = vec![145, 146, 165, 166, 183, 185, 203, 204, 205, 225, 264];  // indices are before the reorder
+        let defect_vertices = vec![145, 146, 165, 166, 183, 185, 203, 204, 205, 225, 264]; // indices are before the reorder
         dual_module_parallel_debug_planar_code_common(19, visualize_filename, defect_vertices, 11);
     }
 
     /// panicked at 'dual node of edge should be none', src/dual_module_serial.rs:400:25
     /// reason: duplicate edge in the boundary... again...
     /// this time it's because when judging whether an edge is already in the boundary, I mistakenly put the clearing edge logic into
     /// the if condition as well... when the edge is duplicate in the boundary already, my code will not clear the edge properly
     #[test]
-    fn dual_module_parallel_debug_11() {  // cargo test dual_module_parallel_debug_11 -- --nocapture
+    fn dual_module_parallel_debug_11() {
+        // cargo test dual_module_parallel_debug_11 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_11.json");
-        let defect_vertices = vec![192, 193, 194, 212, 214, 232, 233];  // indices are before the reorder
+        let defect_vertices = vec![192, 193, 194, 212, 214, 232, 233]; // indices are before the reorder
         dual_module_parallel_debug_planar_code_common(19, visualize_filename, defect_vertices, 7);
     }
 
     /// panicked at 'no sync requests should arise here; make sure to deal with all sync requests before growing', src/dual_module_serial.rs:582:13
     /// just loop the synchronization process until no sync requests emerge
     #[test]
-    fn dual_module_parallel_debug_12() {  // cargo test dual_module_parallel_debug_12 -- --nocapture
+    fn dual_module_parallel_debug_12() {
+        // cargo test dual_module_parallel_debug_12 -- --nocapture
         let visualize_filename = format!("dual_module_parallel_debug_12.json");
-        let defect_vertices = vec![197, 216, 235, 275, 296, 316];  // indices are before the reorder
+        let defect_vertices = vec![197, 216, 235, 275, 296, 316]; // indices are before the reorder
         dual_module_parallel_debug_planar_code_common(19, visualize_filename, defect_vertices, 5);
     }
 
     /// test rayon global thread pool
     #[test]
-    fn dual_module_parallel_rayon_test_1() {  // cargo test dual_module_parallel_rayon_test_1 -- --nocapture
+    fn dual_module_parallel_rayon_test_1() {
+        // cargo test dual_module_parallel_rayon_test_1 -- --nocapture
         rayon::scope(|_| {
             println!("A");
             rayon::scope(|s| {
                 s.spawn(|_| println!("B"));
                 s.spawn(|_| println!("C"));
                 s.spawn(|_| println!("D"));
                 s.spawn(|_| println!("E"));
@@ -1411,15 +1866,16 @@
                 s.spawn(|_| println!("J"));
             });
             println!("K");
         });
     }
 
     #[test]
-    fn dual_module_parallel_rayon_test_2() {  // cargo test dual_module_parallel_rayon_test_2 -- --nocapture
+    fn dual_module_parallel_rayon_test_2() {
+        // cargo test dual_module_parallel_rayon_test_2 -- --nocapture
         let mut results = vec![];
         rayon::scope(|_| {
             results.push("A");
             let (mut ret_b, mut ret_c, mut ret_d, mut ret_e) = (None, None, None, None);
             rayon::scope(|s| {
                 s.spawn(|_| ret_b = Some("B"));
                 s.spawn(|_| ret_c = Some("C"));
@@ -1442,15 +1898,16 @@
             results.push(ret_j.unwrap());
             results.push("K");
         });
         println!("results: {results:?}");
     }
 
     #[test]
-    fn dual_module_parallel_rayon_test_3() {  // cargo test dual_module_parallel_rayon_test_3 -- --nocapture
+    fn dual_module_parallel_rayon_test_3() {
+        // cargo test dual_module_parallel_rayon_test_3 -- --nocapture
         let mut results = vec![];
         rayon::scope(|_| {
             results.push("A");
             results.par_extend(["B", "C", "D", "E"].into_par_iter().map(|id| {
                 // some complex calculation
                 id
             }));
@@ -1459,9 +1916,8 @@
                 // some complex calculation
                 id
             }));
             results.push("K");
         });
         println!("results: {results:?}");
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/src/dual_module_serial.rs` & `fusion_blossom-0.2.5/src/dual_module_serial.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 //! Serial Dual Module
-//! 
+//!
 //! A serial implementation of the dual module. This is the very basic fusion blossom algorithm that aims at debugging and as a ground truth
 //! where traditional matching is too time consuming because of their |E| = O(|V|^2) scaling.
-//! 
+//!
 //! This implementation supports fast clear: optimized for a small number of syndrome and small cluster coverage, the ``clear growth'' operator
 //! can be executed in O(1) time, at the cost of dynamic check and dynamic reset. This also increases cache coherency, because a global clear
 //! operation is unfriendly to cache.
 //!
 
-use super::util::*;
-use crate::derivative::Derivative;
+#![cfg_attr(feature = "unsafe_pointer", allow(dropping_references))]
 use super::dual_module::*;
+use super::pointers::*;
+use super::util::*;
 use super::visualize::*;
-use std::collections::HashMap;
+use crate::derivative::Derivative;
 use crate::weak_table::PtrWeakKeyHashMap;
-use super::pointers::*;
-
+use std::collections::HashMap;
 
 pub struct DualModuleSerial {
     /// all vertices including virtual ones
     pub vertices: Vec<VertexPtr>,
     /// nodes internal information
     pub nodes: Vec<Option<DualNodeInternalPtr>>,
     /// current nodes length, to enable constant-time clear operation
@@ -114,15 +114,15 @@
     /// if a vertex is virtual, then it can be matched any times
     pub is_virtual: bool,
     /// if a vertex is defect, then [`Vertex::propagated_dual_node`] always corresponds to that root
     pub is_defect: bool,
     /// if it's a mirrored vertex (present on multiple units), then this is the parallel unit that exclusively owns it
     pub mirror_unit: Option<PartitionUnitWeak>,
     /// all neighbor edges, in surface code this should be constant number of edges
-    #[derivative(Debug="ignore")]
+    #[derivative(Debug = "ignore")]
     pub edges: Vec<EdgeWeak>,
     /// propagated dual node
     pub propagated_dual_node: Option<DualNodeInternalWeak>,
     /// propagated grandson node: must be a syndrome node
     pub propagated_grandson_dual_node: Option<DualNodeInternalWeak>,
     /// for fast clear
     pub timestamp: FastClearTimestamp,
@@ -142,27 +142,26 @@
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         let vertex_ptr = self.upgrade_force();
         let vertex = vertex_ptr.read_recursive_force();
         write!(f, "{}", vertex.vertex_index)
     }
 }
 
-
 #[derive(Derivative)]
 #[derivative(Debug)]
 pub struct Edge {
     /// global edge index, not necessary the index in [`DualModuleSerial::edges`]
     pub edge_index: EdgeIndex,
     /// total weight of this edge
     pub weight: Weight,
     /// left vertex (always with smaller index for consistency)
-    #[derivative(Debug="ignore")]
+    #[derivative(Debug = "ignore")]
     pub left: VertexWeak,
     /// right vertex (always with larger index for consistency)
-    #[derivative(Debug="ignore")]
+    #[derivative(Debug = "ignore")]
     pub right: VertexWeak,
     /// growth from the left point
     pub left_growth: Weight,
     /// growth from the right point
     pub right_growth: Weight,
     /// left active tree node (if applicable)
     pub left_dual_node: Option<DualNodeInternalWeak>,
@@ -193,42 +192,63 @@
         let edge_ptr = self.upgrade_force();
         let edge = edge_ptr.read_recursive_force();
         write!(f, "{}", edge.edge_index)
     }
 }
 
 impl DualModuleImpl for DualModuleSerial {
-
     /// initialize the dual module, which is supposed to be reused for multiple decoding tasks with the same structure
+    #[allow(clippy::unnecessary_cast)]
     fn new_empty(initializer: &SolverInitializer) -> Self {
         let active_timestamp = 0;
         // create vertices
-        let vertices: Vec<VertexPtr> = (0..initializer.vertex_num).map(|vertex_index| VertexPtr::new_value(Vertex {
-            vertex_index,
-            is_virtual: false,
-            is_defect: false,
-            mirror_unit: None,
-            edges: Vec::new(),
-            propagated_dual_node: None,
-            propagated_grandson_dual_node: None,
-            timestamp: active_timestamp,
-        })).collect();
+        let vertices: Vec<VertexPtr> = (0..initializer.vertex_num)
+            .map(|vertex_index| {
+                VertexPtr::new_value(Vertex {
+                    vertex_index,
+                    is_virtual: false,
+                    is_defect: false,
+                    mirror_unit: None,
+                    edges: Vec::new(),
+                    propagated_dual_node: None,
+                    propagated_grandson_dual_node: None,
+                    timestamp: active_timestamp,
+                })
+            })
+            .collect();
         // set virtual vertices
         for &virtual_vertex in initializer.virtual_vertices.iter() {
             let mut vertex = vertices[virtual_vertex as usize].write(active_timestamp);
             vertex.is_virtual = true;
         }
         // set edges
         let mut edges = Vec::<EdgePtr>::new();
         for &(i, j, weight) in initializer.weighted_edges.iter() {
             assert_ne!(i, j, "invalid edge from and to the same vertex {}", i);
-            assert!(weight % 2 == 0, "edge ({}, {}) has odd weight value; weight should be even", i, j);
+            assert!(
+                weight % 2 == 0,
+                "edge ({}, {}) has odd weight value; weight should be even",
+                i,
+                j
+            );
             assert!(weight >= 0, "edge ({}, {}) is negative-weighted", i, j);
-            assert!(i < initializer.vertex_num, "edge ({}, {}) connected to an invalid vertex {}", i, j, i);
-            assert!(j < initializer.vertex_num, "edge ({}, {}) connected to an invalid vertex {}", i, j, j);
+            assert!(
+                i < initializer.vertex_num,
+                "edge ({}, {}) connected to an invalid vertex {}",
+                i,
+                j,
+                i
+            );
+            assert!(
+                j < initializer.vertex_num,
+                "edge ({}, {}) connected to an invalid vertex {}",
+                i,
+                j,
+                j
+            );
             let left = VertexIndex::min(i, j);
             let right = VertexIndex::max(i, j);
             let edge_ptr = EdgePtr::new_value(Edge {
                 edge_index: edges.len() as EdgeIndex,
                 weight,
                 left: vertices[left as usize].downgrade(),
                 right: vertices[right as usize].downgrade(),
@@ -239,23 +259,24 @@
                 right_dual_node: None,
                 right_grandson_dual_node: None,
                 timestamp: 0,
                 dedup_timestamp: (0, 0),
             });
             for (a, b) in [(i, j), (j, i)] {
                 lock_write!(vertex, vertices[a as usize], active_timestamp);
-                debug_assert!({  // O(N^2) sanity check, debug mode only (actually this bug is not critical, only the shorter edge will take effect)
+                debug_assert!({
+                    // O(N^2) sanity check, debug mode only (actually this bug is not critical, only the shorter edge will take effect)
                     let mut no_duplicate = true;
                     for edge_weak in vertex.edges.iter() {
                         let edge_ptr = edge_weak.upgrade_force();
                         let edge = edge_ptr.read_recursive(active_timestamp);
                         if edge.left == vertices[b as usize].downgrade() || edge.right == vertices[b as usize].downgrade() {
                             no_duplicate = false;
                             eprintln!("duplicated edge between {} and {} with weight w1 = {} and w2 = {}, consider merge them into a single edge", i, j, weight, edge.weight);
-                            break
+                            break;
                         }
                     }
                     no_duplicate
                 });
                 vertex.edges.push(edge_ptr.downgrade());
             }
             edges.push(edge_ptr);
@@ -265,44 +286,46 @@
             nodes: vec![],
             nodes_length: 0,
             edges,
             active_timestamp: 0,
             vertex_num: initializer.vertex_num,
             edge_num: initializer.weighted_edges.len(),
             owning_range: VertexRange::new(0, initializer.vertex_num),
-            unit_module_info: None,  // disabled
+            unit_module_info: None, // disabled
             active_list: vec![],
             current_cycle: 0,
             edge_modifier: EdgeWeightModifier::new(),
             edge_dedup_timestamp: 0,
             sync_requests: vec![],
             updated_boundary: vec![],
             propagating_vertices: vec![],
         }
     }
 
     /// clear all growth and existing dual nodes
+    #[allow(clippy::unnecessary_cast)]
     fn clear(&mut self) {
         // recover erasure edges first
         while self.edge_modifier.has_modified_edges() {
             let (edge_index, original_weight) = self.edge_modifier.pop_modified_edge();
             let edge_ptr = &self.edges[edge_index as usize];
             let mut edge = edge_ptr.write(self.active_timestamp);
             edge.weight = original_weight;
         }
         self.clear_graph();
-        self.nodes_length = 0;  // without actually dropping all the nodes, to enable constant time clear
+        self.nodes_length = 0; // without actually dropping all the nodes, to enable constant time clear
         if let Some(unit_module_info) = self.unit_module_info.as_mut() {
             unit_module_info.owning_dual_range = VertexRange::new(0, 0);
             unit_module_info.dual_node_pointers = PtrWeakKeyHashMap::<DualNodeWeak, usize>::new();
         }
         self.active_list.clear();
     }
 
     /// add a new dual node from dual module root
+    #[allow(clippy::unnecessary_cast)]
     fn add_dual_node(&mut self, dual_node_ptr: &DualNodePtr) {
         self.register_dual_node_ptr(dual_node_ptr);
         let active_timestamp = self.active_timestamp;
         let node = dual_node_ptr.read_recursive();
         let node_index = self.nodes_length as NodeIndex;
         let node_internal_ptr = if node_index < self.nodes.len() as NodeIndex && self.nodes[node_index as usize].is_some() {
             let node_ptr = self.nodes[node_index as usize].take().unwrap();
@@ -328,177 +351,255 @@
         {
             let boundary = &mut node_internal_ptr.write().boundary;
             match &node.class {
                 DualNodeClass::Blossom { nodes_circle, .. } => {
                     // copy all the boundary edges and modify edge belongings
                     for dual_node_weak in nodes_circle.iter() {
                         let dual_node_ptr = dual_node_weak.upgrade_force();
-                        if self.unit_module_info.is_none() {  // it's required to do it in the outer loop and synchronize everybody, so no need to do it here
-                            self.prepare_dual_node_growth(&dual_node_ptr, false);  // prepare all nodes in shrinking mode for consistency
+                        if self.unit_module_info.is_none() {
+                            // it's required to do it in the outer loop and synchronize everybody, so no need to do it here
+                            self.prepare_dual_node_growth(&dual_node_ptr, false);
+                            // prepare all nodes in shrinking mode for consistency
                         }
                         if let Some(dual_node_internal_ptr) = self.get_dual_node_internal_ptr_optional(&dual_node_ptr) {
                             let dual_node_internal = dual_node_internal_ptr.read_recursive();
                             for (is_left, edge_weak) in dual_node_internal.boundary.iter() {
                                 let edge_ptr = edge_weak.upgrade_force();
                                 boundary.push((*is_left, edge_weak.clone()));
                                 let mut edge = edge_ptr.write(active_timestamp);
-                                debug_assert!(if *is_left { edge.left_dual_node.is_some() } else { edge.right_dual_node.is_some() }, "dual node of edge should be some");
-                                debug_assert!(if *is_left { edge.left_dual_node == Some(dual_node_internal_ptr.downgrade())
-                                    } else { edge.right_dual_node == Some(dual_node_internal_ptr.downgrade()) }, "edge belonging");
+                                debug_assert!(
+                                    if *is_left {
+                                        edge.left_dual_node.is_some()
+                                    } else {
+                                        edge.right_dual_node.is_some()
+                                    },
+                                    "dual node of edge should be some"
+                                );
+                                debug_assert!(
+                                    if *is_left {
+                                        edge.left_dual_node == Some(dual_node_internal_ptr.downgrade())
+                                    } else {
+                                        edge.right_dual_node == Some(dual_node_internal_ptr.downgrade())
+                                    },
+                                    "edge belonging"
+                                );
                                 if *is_left {
                                     edge.left_dual_node = Some(node_internal_ptr.downgrade());
                                 } else {
                                     edge.right_dual_node = Some(node_internal_ptr.downgrade());
                                 }
                             }
                         } else {
-                            debug_assert!(self.unit_module_info.is_some(), "only partitioned could ignore some of its children");
+                            debug_assert!(
+                                self.unit_module_info.is_some(),
+                                "only partitioned could ignore some of its children"
+                            );
                         }
                     }
-                },
+                }
                 DualNodeClass::DefectVertex { defect_index } => {
-                    let vertex_index = self.get_vertex_index(*defect_index).expect("syndrome not belonging to this dual module");
+                    let vertex_index = self
+                        .get_vertex_index(*defect_index)
+                        .expect("syndrome not belonging to this dual module");
                     let vertex_ptr = &self.vertices[vertex_index];
                     vertex_ptr.dynamic_clear(active_timestamp);
                     let mut vertex = vertex_ptr.write(active_timestamp);
                     vertex.propagated_dual_node = Some(node_internal_ptr.downgrade());
                     vertex.propagated_grandson_dual_node = Some(node_internal_ptr.downgrade());
                     vertex.is_defect = true;
                     for edge_weak in vertex.edges.iter() {
                         let edge_ptr = edge_weak.upgrade_force();
                         edge_ptr.dynamic_clear(active_timestamp);
                         let mut edge = edge_ptr.write(active_timestamp);
                         let is_left = vertex_ptr.downgrade() == edge.left;
-                        debug_assert!(if is_left { edge.left_dual_node.is_none() } else { edge.right_dual_node.is_none() }, "dual node of edge should be none");
+                        debug_assert!(
+                            if is_left {
+                                edge.left_dual_node.is_none()
+                            } else {
+                                edge.right_dual_node.is_none()
+                            },
+                            "dual node of edge should be none"
+                        );
                         if is_left {
                             edge.left_dual_node = Some(node_internal_ptr.downgrade());
                             edge.left_grandson_dual_node = Some(node_internal_ptr.downgrade());
                         } else {
                             edge.right_dual_node = Some(node_internal_ptr.downgrade());
                             edge.right_grandson_dual_node = Some(node_internal_ptr.downgrade());
                         }
                         boundary.push((is_left, edge_weak.clone()));
                     }
-                },
+                }
             }
         }
         self.active_list.push(node_internal_ptr.downgrade());
         self.nodes_length += 1;
         if self.nodes.len() < self.nodes_length {
             self.nodes.push(None);
         }
         self.nodes[node_index as usize] = Some(node_internal_ptr);
     }
 
+    #[allow(clippy::unnecessary_cast)]
     fn remove_blossom(&mut self, dual_node_ptr: DualNodePtr) {
         let active_timestamp = self.active_timestamp;
-        self.prepare_dual_node_growth(&dual_node_ptr, false);  // prepare the blossom into shrinking
+        self.prepare_dual_node_growth(&dual_node_ptr, false); // prepare the blossom into shrinking
         let node = dual_node_ptr.read_recursive();
         let dual_node_internal_ptr = self.get_dual_node_internal_ptr(&dual_node_ptr);
         let dual_node_internal = dual_node_internal_ptr.read_recursive();
-        debug_assert_eq!(dual_node_internal.dual_variable, 0, "only blossom with dual variable = 0 can be safely removed");
-        debug_assert!(dual_node_internal.overgrown_stack.is_empty(), "removing a blossom with non-empty overgrown stack forbidden");
+        debug_assert_eq!(
+            dual_node_internal.dual_variable, 0,
+            "only blossom with dual variable = 0 can be safely removed"
+        );
+        debug_assert!(
+            dual_node_internal.overgrown_stack.is_empty(),
+            "removing a blossom with non-empty overgrown stack forbidden"
+        );
         let node_idx = dual_node_internal.index;
-        debug_assert!(self.nodes[node_idx as usize].is_some(), "blossom may have already been removed, do not call twice");
-        debug_assert!(self.nodes[node_idx as usize].as_ref().unwrap() == &dual_node_internal_ptr, "the blossom doesn't belong to this DualModuleInterface");
+        debug_assert!(
+            self.nodes[node_idx as usize].is_some(),
+            "blossom may have already been removed, do not call twice"
+        );
+        debug_assert!(
+            self.nodes[node_idx as usize].as_ref().unwrap() == &dual_node_internal_ptr,
+            "the blossom doesn't belong to this DualModuleInterface"
+        );
         // recover edge belongings
         for (is_left, edge_weak) in dual_node_internal.boundary.iter() {
             let edge_ptr = edge_weak.upgrade_force();
             let mut edge = edge_ptr.write(active_timestamp);
-            debug_assert!(if *is_left { edge.left_dual_node.is_some() } else { edge.right_dual_node.is_some() }, "dual node of edge should be some");
+            debug_assert!(
+                if *is_left {
+                    edge.left_dual_node.is_some()
+                } else {
+                    edge.right_dual_node.is_some()
+                },
+                "dual node of edge should be some"
+            );
             if *is_left {
                 edge.left_dual_node = None;
             } else {
                 edge.right_dual_node = None;
             }
         }
-        if let DualNodeClass::Blossom{ nodes_circle, .. } = &node.class {
+        if let DualNodeClass::Blossom { nodes_circle, .. } = &node.class {
             for circle_dual_node_weak in nodes_circle.iter() {
                 let circle_dual_node_ptr = circle_dual_node_weak.upgrade_force();
-                if let Some(circle_dual_node_internal_ptr) = self.get_dual_node_internal_ptr_optional(&circle_dual_node_ptr) {
+                if let Some(circle_dual_node_internal_ptr) = self.get_dual_node_internal_ptr_optional(&circle_dual_node_ptr)
+                {
                     let circle_dual_node_internal = circle_dual_node_internal_ptr.read_recursive();
                     for (is_left, edge_weak) in circle_dual_node_internal.boundary.iter() {
                         let edge_ptr = edge_weak.upgrade_force();
                         let mut edge = edge_ptr.write(active_timestamp);
-                        debug_assert!(if *is_left { edge.left_dual_node.is_none() } else { edge.right_dual_node.is_none() }, "dual node of edge should be none");
+                        debug_assert!(
+                            if *is_left {
+                                edge.left_dual_node.is_none()
+                            } else {
+                                edge.right_dual_node.is_none()
+                            },
+                            "dual node of edge should be none"
+                        );
                         if *is_left {
                             edge.left_dual_node = Some(circle_dual_node_internal_ptr.downgrade());
                         } else {
                             edge.right_dual_node = Some(circle_dual_node_internal_ptr.downgrade());
                         }
                     }
                 } else {
                     debug_assert!(self.unit_module_info.is_some(), "only happens if partitioned");
                 }
             }
         } else {
             unreachable!()
         }
-        self.nodes[node_idx as usize] = None;  // simply remove this blossom node
+        self.nodes[node_idx as usize] = None; // simply remove this blossom node
     }
 
     fn set_grow_state(&mut self, dual_node_ptr: &DualNodePtr, grow_state: DualNodeGrowState) {
         let dual_node = dual_node_ptr.read_recursive();
         if dual_node.grow_state == DualNodeGrowState::Stay && grow_state != DualNodeGrowState::Stay {
             let dual_node_internal_ptr = self.get_dual_node_internal_ptr(dual_node_ptr);
             self.active_list.push(dual_node_internal_ptr.downgrade())
         }
     }
 
     #[allow(clippy::collapsible_else_if)]
-    fn compute_maximum_update_length_dual_node(&mut self, dual_node_ptr: &DualNodePtr, is_grow: bool, simultaneous_update: bool) -> MaxUpdateLength {
+    fn compute_maximum_update_length_dual_node(
+        &mut self,
+        dual_node_ptr: &DualNodePtr,
+        is_grow: bool,
+        simultaneous_update: bool,
+    ) -> MaxUpdateLength {
         let active_timestamp = self.active_timestamp;
         if !simultaneous_update {
             // when `simultaneous_update` is set, it's assumed that all nodes are prepared to grow or shrink
             // this is because if we dynamically prepare them, it would be inefficient
             self.prepare_dual_node_growth(dual_node_ptr, is_grow);
         }
         let mut max_length_abs = Weight::MAX;
         let dual_node_internal_ptr = self.get_dual_node_internal_ptr(dual_node_ptr);
         let dual_node_internal = dual_node_internal_ptr.read_recursive();
         if !is_grow {
             if dual_node_internal.dual_variable == 0 {
                 let dual_node = dual_node_ptr.read_recursive();
                 match dual_node.class {
-                    DualNodeClass::Blossom { .. } => { return MaxUpdateLength::BlossomNeedExpand(dual_node_ptr.clone()) }
+                    DualNodeClass::Blossom { .. } => return MaxUpdateLength::BlossomNeedExpand(dual_node_ptr.clone()),
                     DualNodeClass::DefectVertex { defect_index } => {
                         // try to report Conflicting event or give a VertexShrinkStop with potential conflicting node
-                        if let Some(vertex_index) = self.get_vertex_index(defect_index) {  // since propagated node is never removed, this event could happen with no vertex
+                        if let Some(vertex_index) = self.get_vertex_index(defect_index) {
+                            // since propagated node is never removed, this event could happen with no vertex
                             let vertex_ptr = &self.vertices[vertex_index];
                             let vertex = vertex_ptr.read_recursive(active_timestamp);
                             let mut potential_conflict: Option<(DualNodePtr, DualNodePtr)> = None;
                             for edge_weak in vertex.edges.iter() {
                                 let edge_ptr = edge_weak.upgrade_force();
                                 let edge = edge_ptr.read_recursive(active_timestamp);
                                 let is_left = vertex_ptr.downgrade() == edge.left;
                                 let remaining_length = edge.weight - edge.left_growth - edge.right_growth;
                                 if remaining_length == 0 {
-                                    let peer_dual_node = if is_left { &edge.right_dual_node } else { &edge.left_dual_node };
+                                    let peer_dual_node = if is_left {
+                                        &edge.right_dual_node
+                                    } else {
+                                        &edge.left_dual_node
+                                    };
                                     if let Some(peer_dual_node_ptr) = peer_dual_node {
-                                        let peer_grandson_dual_node = if is_left { &edge.right_grandson_dual_node } else { &edge.left_grandson_dual_node };
-                                        let peer_dual_node_ptr = peer_dual_node_ptr.upgrade_force().read_recursive().origin.upgrade_force();
-                                        let peer_grandson_dual_node_ptr = peer_grandson_dual_node.as_ref().unwrap().upgrade_force().read_recursive().origin.upgrade_force();
+                                        let peer_grandson_dual_node = if is_left {
+                                            &edge.right_grandson_dual_node
+                                        } else {
+                                            &edge.left_grandson_dual_node
+                                        };
+                                        let peer_dual_node_ptr =
+                                            peer_dual_node_ptr.upgrade_force().read_recursive().origin.upgrade_force();
+                                        let peer_grandson_dual_node_ptr = peer_grandson_dual_node
+                                            .as_ref()
+                                            .unwrap()
+                                            .upgrade_force()
+                                            .read_recursive()
+                                            .origin
+                                            .upgrade_force();
                                         if peer_dual_node_ptr.read_recursive().grow_state == DualNodeGrowState::Grow {
-                                            if let Some((other_dual_node_ptr, other_grandson_dual_node)) = &potential_conflict {
+                                            if let Some((other_dual_node_ptr, other_grandson_dual_node)) =
+                                                &potential_conflict
+                                            {
                                                 if &peer_dual_node_ptr != other_dual_node_ptr {
                                                     return MaxUpdateLength::Conflicting(
                                                         (other_dual_node_ptr.clone(), other_grandson_dual_node.clone()),
-                                                        (peer_dual_node_ptr, peer_grandson_dual_node_ptr)
-                                                    )
+                                                        (peer_dual_node_ptr, peer_grandson_dual_node_ptr),
+                                                    );
                                                 }
                                             } else {
                                                 potential_conflict = Some((peer_dual_node_ptr, peer_grandson_dual_node_ptr));
                                             }
                                         }
                                     }
                                 }
                             }
-                            return MaxUpdateLength::VertexShrinkStop((dual_node_ptr.clone(), potential_conflict))
+                            return MaxUpdateLength::VertexShrinkStop((dual_node_ptr.clone(), potential_conflict));
                         } else {
-                            return MaxUpdateLength::VertexShrinkStop((dual_node_ptr.clone(), None))
+                            return MaxUpdateLength::VertexShrinkStop((dual_node_ptr.clone(), None));
                         }
                     }
                 }
             }
             if !dual_node_internal.overgrown_stack.is_empty() {
                 let last_index = dual_node_internal.overgrown_stack.len() - 1;
                 let (_, overgrown) = &dual_node_internal.overgrown_stack[last_index];
@@ -516,75 +617,113 @@
                     edge.right_dual_node.as_ref().map(|ptr| ptr.upgrade_force())
                 } else {
                     edge.left_dual_node.as_ref().map(|ptr| ptr.upgrade_force())
                 };
                 match peer_dual_node_internal_ptr {
                     Some(peer_dual_node_internal_ptr) => {
                         if peer_dual_node_internal_ptr == dual_node_internal_ptr {
-                            continue
+                            continue;
                         } else {
                             let peer_dual_node_internal = peer_dual_node_internal_ptr.read_recursive();
                             let peer_dual_node_ptr = peer_dual_node_internal.origin.upgrade_force();
                             let peer_dual_node = peer_dual_node_ptr.read_recursive();
                             let remaining_length = edge.weight - edge.left_growth - edge.right_growth;
                             let local_max_length_abs = match peer_dual_node.grow_state {
                                 DualNodeGrowState::Grow => {
                                     debug_assert!(remaining_length % 2 == 0, "there is odd gap between two growing nodes, please make sure all weights are even numbers");
                                     remaining_length / 2
-                                },
+                                }
                                 DualNodeGrowState::Shrink => {
                                     // Yue 2022.9.5: remove Conflicting event detection here, move it to the 0-dual syndrome node
-                                    continue
-                                },
-                                DualNodeGrowState::Stay => { remaining_length }
+                                    continue;
+                                }
+                                DualNodeGrowState::Stay => remaining_length,
                             };
                             if local_max_length_abs == 0 {
                                 let peer_grandson_ptr = if is_left {
-                                    edge.right_grandson_dual_node.as_ref().map(|ptr| ptr.upgrade_force()).unwrap().read_recursive().origin.upgrade_force()
+                                    edge.right_grandson_dual_node
+                                        .as_ref()
+                                        .map(|ptr| ptr.upgrade_force())
+                                        .unwrap()
+                                        .read_recursive()
+                                        .origin
+                                        .upgrade_force()
                                 } else {
-                                    edge.left_grandson_dual_node.as_ref().map(|ptr| ptr.upgrade_force()).unwrap().read_recursive().origin.upgrade_force()
+                                    edge.left_grandson_dual_node
+                                        .as_ref()
+                                        .map(|ptr| ptr.upgrade_force())
+                                        .unwrap()
+                                        .read_recursive()
+                                        .origin
+                                        .upgrade_force()
                                 };
                                 let grandson_ptr = if is_left {
-                                    edge.left_grandson_dual_node.as_ref().map(|ptr| ptr.upgrade_force()).unwrap().read_recursive().origin.upgrade_force()
+                                    edge.left_grandson_dual_node
+                                        .as_ref()
+                                        .map(|ptr| ptr.upgrade_force())
+                                        .unwrap()
+                                        .read_recursive()
+                                        .origin
+                                        .upgrade_force()
                                 } else {
-                                    edge.right_grandson_dual_node.as_ref().map(|ptr| ptr.upgrade_force()).unwrap().read_recursive().origin.upgrade_force()
+                                    edge.right_grandson_dual_node
+                                        .as_ref()
+                                        .map(|ptr| ptr.upgrade_force())
+                                        .unwrap()
+                                        .read_recursive()
+                                        .origin
+                                        .upgrade_force()
                                 };
                                 return MaxUpdateLength::Conflicting(
-                                    (peer_dual_node_ptr.clone(), peer_grandson_ptr), 
-                                    (dual_node_ptr.clone(), grandson_ptr)
+                                    (peer_dual_node_ptr.clone(), peer_grandson_ptr),
+                                    (dual_node_ptr.clone(), grandson_ptr),
                                 );
                             }
                             max_length_abs = std::cmp::min(max_length_abs, local_max_length_abs);
                         }
-                    },
+                    }
                     None => {
                         let local_max_length_abs = edge.weight - edge.left_growth - edge.right_growth;
                         if local_max_length_abs == 0 {
                             // check if peer is virtual node
                             let peer_vertex_ptr = if is_left {
                                 edge.right.upgrade_force()
                             } else {
                                 edge.left.upgrade_force()
                             };
                             let peer_vertex = peer_vertex_ptr.read_recursive(active_timestamp);
                             if peer_vertex.is_virtual || peer_vertex.is_mirror_blocked() {
                                 let grandson_ptr = if is_left {
-                                    edge.left_grandson_dual_node.as_ref().map(|ptr| ptr.upgrade_force()).unwrap().read_recursive().origin.upgrade_force()
+                                    edge.left_grandson_dual_node
+                                        .as_ref()
+                                        .map(|ptr| ptr.upgrade_force())
+                                        .unwrap()
+                                        .read_recursive()
+                                        .origin
+                                        .upgrade_force()
                                 } else {
-                                    edge.right_grandson_dual_node.as_ref().map(|ptr| ptr.upgrade_force()).unwrap().read_recursive().origin.upgrade_force()
+                                    edge.right_grandson_dual_node
+                                        .as_ref()
+                                        .map(|ptr| ptr.upgrade_force())
+                                        .unwrap()
+                                        .read_recursive()
+                                        .origin
+                                        .upgrade_force()
                                 };
-                                return MaxUpdateLength::TouchingVirtual((dual_node_ptr.clone(), grandson_ptr)
-                                    , (peer_vertex.vertex_index, peer_vertex.is_mirror_blocked()));
+                                return MaxUpdateLength::TouchingVirtual(
+                                    (dual_node_ptr.clone(), grandson_ptr),
+                                    (peer_vertex.vertex_index, peer_vertex.is_mirror_blocked()),
+                                );
                             } else {
                                 println!("edge: {edge_ptr:?}, peer_vertex_ptr: {peer_vertex_ptr:?}");
                                 unreachable!("this edge should've been removed from boundary because it's already fully grown, and it's peer vertex is not virtual")
                             }
                         }
                         max_length_abs = std::cmp::min(max_length_abs, local_max_length_abs);
-                    },
+                    }
                 }
             } else {
                 if is_left {
                     if edge.left_growth == 0 {
                         unreachable!()
                     }
                     max_length_abs = std::cmp::min(max_length_abs, edge.left_growth);
@@ -599,61 +738,70 @@
         MaxUpdateLength::NonZeroGrow((max_length_abs, dual_node_internal.boundary.is_empty()))
     }
 
     fn compute_maximum_update_length(&mut self) -> GroupMaxUpdateLength {
         // first prepare all nodes for individual grow or shrink; Stay nodes will be prepared to shrink in order to minimize effect on others
         self.prepare_all();
         // after preparing all the growth, there should be no sync requests
-        debug_assert!(self.sync_requests.is_empty(), "no sync requests should arise here; make sure to deal with all sync requests before growing");
+        debug_assert!(
+            self.sync_requests.is_empty(),
+            "no sync requests should arise here; make sure to deal with all sync requests before growing"
+        );
         let mut group_max_update_length = GroupMaxUpdateLength::new();
         for i in 0..self.active_list.len() {
             let dual_node_ptr = {
                 let internal_dual_node_ptr = self.active_list[i].upgrade_force();
                 let dual_node_internal = internal_dual_node_ptr.read_recursive();
                 dual_node_internal.origin.upgrade_force()
             };
             let dual_node = dual_node_ptr.read_recursive();
             let is_grow = match dual_node.grow_state {
                 DualNodeGrowState::Grow => true,
                 DualNodeGrowState::Shrink => false,
-                DualNodeGrowState::Stay => { continue }
+                DualNodeGrowState::Stay => continue,
             };
-            drop(dual_node);  // unlock, otherwise it causes deadlock when updating the dual node
+            drop(dual_node); // unlock, otherwise it causes deadlock when updating the dual node
             let max_update_length = self.compute_maximum_update_length_dual_node(&dual_node_ptr, is_grow, true);
             group_max_update_length.add(max_update_length);
         }
         group_max_update_length
     }
 
     fn grow_dual_node(&mut self, dual_node_ptr: &DualNodePtr, length: Weight) {
         let active_timestamp = self.active_timestamp;
         if length == 0 {
             eprintln!("[warning] calling `grow_dual_node` with zero length, nothing to do");
-            return
+            return;
         }
         self.prepare_dual_node_growth(dual_node_ptr, length > 0);
         let dual_node_internal_ptr = self.get_dual_node_internal_ptr(dual_node_ptr);
         {
             // update node dual variable and do sanity check
             let mut dual_node_internal = dual_node_internal_ptr.write();
             dual_node_internal.dual_variable += length;
-            debug_assert!(dual_node_internal.dual_variable >= 0, "shrinking to negative dual variable is forbidden");
+            debug_assert!(
+                dual_node_internal.dual_variable >= 0,
+                "shrinking to negative dual variable is forbidden"
+            );
             // update over-grown vertices
             if !dual_node_internal.overgrown_stack.is_empty() {
                 let last_index = dual_node_internal.overgrown_stack.len() - 1;
                 let (_, overgrown) = &mut dual_node_internal.overgrown_stack[last_index];
-                if length < 0 { debug_assert!( *overgrown >= -length, "overgrown vertex cannot shrink so much"); }
+                if length < 0 {
+                    debug_assert!(*overgrown >= -length, "overgrown vertex cannot shrink so much");
+                }
                 *overgrown += length;
             }
         }
         let dual_node_internal = dual_node_internal_ptr.read_recursive();
         for (is_left, edge_weak) in dual_node_internal.boundary.iter() {
             let edge_ptr = edge_weak.upgrade_force();
             let is_left = *is_left;
-            let (growth, weight) = {  // minimize writer lock acquisition
+            let (growth, weight) = {
+                // minimize writer lock acquisition
                 let mut edge = edge_ptr.write(active_timestamp);
                 if is_left {
                     edge.left_growth += length;
                     debug_assert!(edge.left_growth >= 0, "negative growth forbidden");
                 } else {
                     edge.right_growth += length;
                     debug_assert!(edge.right_growth >= 0, "negative growth forbidden");
@@ -664,25 +812,37 @@
             if growth > weight {
                 // first check for if both side belongs to the same dual node, if so, it's ok
                 let dual_node_internal_ptr_2: &Option<DualNodeInternalWeak> = if is_left {
                     &edge.right_dual_node
                 } else {
                     &edge.left_dual_node
                 };
-                if dual_node_internal_ptr_2.is_none() || dual_node_internal_ptr_2.as_ref().unwrap() != &dual_node_internal_ptr.downgrade() {
+                if dual_node_internal_ptr_2.is_none()
+                    || dual_node_internal_ptr_2.as_ref().unwrap() != &dual_node_internal_ptr.downgrade()
+                {
                     let left_ptr = edge.left.upgrade_force();
                     let right_ptr = edge.right.upgrade_force();
-                    panic!("over-grown edge ({},{}): {}/{}", left_ptr.read_recursive(active_timestamp).vertex_index
-                        , right_ptr.read_recursive(active_timestamp).vertex_index, growth, weight);
+                    panic!(
+                        "over-grown edge ({},{}): {}/{}",
+                        left_ptr.read_recursive(active_timestamp).vertex_index,
+                        right_ptr.read_recursive(active_timestamp).vertex_index,
+                        growth,
+                        weight
+                    );
                 }
             } else if growth < 0 {
                 let left_ptr = edge.left.upgrade_force();
                 let right_ptr = edge.right.upgrade_force();
-                panic!("under-grown edge ({},{}): {}/{}", left_ptr.read_recursive(active_timestamp).vertex_index
-                    , right_ptr.read_recursive(active_timestamp).vertex_index, growth, weight);
+                panic!(
+                    "under-grown edge ({},{}): {}/{}",
+                    left_ptr.read_recursive(active_timestamp).vertex_index,
+                    right_ptr.read_recursive(active_timestamp).vertex_index,
+                    growth,
+                    weight
+                );
             }
         }
     }
 
     fn grow(&mut self, length: Weight) {
         debug_assert!(length > 0, "only positive growth is supported");
         self.renew_active_list();
@@ -708,124 +868,161 @@
             let dual_node = dual_node_ptr.read_recursive();
             if matches!(dual_node.grow_state, DualNodeGrowState::Grow) {
                 self.grow_dual_node(&dual_node_ptr, length);
             }
         }
     }
 
+    #[allow(clippy::unnecessary_cast)]
     fn load_edge_modifier(&mut self, edge_modifier: &[(EdgeIndex, Weight)]) {
-        debug_assert!(!self.edge_modifier.has_modified_edges(), "the current erasure modifier is not clean, probably forget to clean the state?");
+        debug_assert!(
+            !self.edge_modifier.has_modified_edges(),
+            "the current erasure modifier is not clean, probably forget to clean the state?"
+        );
         let active_timestamp = self.active_timestamp;
         for (edge_index, target_weight) in edge_modifier.iter() {
             let edge_ptr = &self.edges[*edge_index as usize];
-            edge_ptr.dynamic_clear(active_timestamp);  // may visit stale edges
+            edge_ptr.dynamic_clear(active_timestamp); // may visit stale edges
             let mut edge = edge_ptr.write(active_timestamp);
             let original_weight = edge.weight;
             edge.weight = *target_weight;
             self.edge_modifier.push_modified_edge(*edge_index, original_weight);
         }
     }
 
     fn prepare_all(&mut self) -> &mut Vec<SyncRequest> {
-        debug_assert!(self.sync_requests.is_empty(), "make sure to remove all sync requests before prepare to avoid out-dated requests");
+        debug_assert!(
+            self.sync_requests.is_empty(),
+            "make sure to remove all sync requests before prepare to avoid out-dated requests"
+        );
         self.renew_active_list();
         for i in 0..self.active_list.len() {
             let dual_node_ptr = {
                 if let Some(internal_dual_node_ptr) = self.active_list[i].upgrade() {
                     let dual_node_internal = internal_dual_node_ptr.read_recursive();
                     dual_node_internal.origin.upgrade_force()
                 } else {
-                    continue  // a blossom could be in the active list even after it's been removed
+                    continue; // a blossom could be in the active list even after it's been removed
                 }
             };
             let dual_node = dual_node_ptr.read_recursive();
             match dual_node.grow_state {
-                DualNodeGrowState::Grow => { },
-                DualNodeGrowState::Shrink => { self.prepare_dual_node_growth(&dual_node_ptr, false); },
-                DualNodeGrowState::Stay => { },  // do not touch, Stay nodes might have become a part of a blossom, so it's not safe to change the boundary
+                DualNodeGrowState::Grow => {}
+                DualNodeGrowState::Shrink => {
+                    self.prepare_dual_node_growth(&dual_node_ptr, false);
+                }
+                DualNodeGrowState::Stay => {} // do not touch, Stay nodes might have become a part of a blossom, so it's not safe to change the boundary
             };
         }
         for i in 0..self.active_list.len() {
             let dual_node_ptr = {
                 if let Some(internal_dual_node_ptr) = self.active_list[i].upgrade() {
                     let dual_node_internal = internal_dual_node_ptr.read_recursive();
                     dual_node_internal.origin.upgrade_force()
                 } else {
-                    continue  // a blossom could be in the active list even after it's been removed
+                    continue; // a blossom could be in the active list even after it's been removed
                 }
             };
             let dual_node = dual_node_ptr.read_recursive();
             match dual_node.grow_state {
-                DualNodeGrowState::Grow => { self.prepare_dual_node_growth(&dual_node_ptr, true); },
-                DualNodeGrowState::Shrink => { },
-                DualNodeGrowState::Stay => { },  // do not touch, Stay nodes might have become a part of a blossom, so it's not safe to change the boundary
+                DualNodeGrowState::Grow => {
+                    self.prepare_dual_node_growth(&dual_node_ptr, true);
+                }
+                DualNodeGrowState::Shrink => {}
+                DualNodeGrowState::Stay => {} // do not touch, Stay nodes might have become a part of a blossom, so it's not safe to change the boundary
             };
         }
         &mut self.sync_requests
     }
 
     fn prepare_nodes_shrink(&mut self, nodes_circle: &[DualNodePtr]) -> &mut Vec<SyncRequest> {
-        debug_assert!(self.sync_requests.is_empty(), "make sure to remove all sync requests before prepare to avoid out-dated requests");
+        debug_assert!(
+            self.sync_requests.is_empty(),
+            "make sure to remove all sync requests before prepare to avoid out-dated requests"
+        );
         for dual_node_ptr in nodes_circle.iter() {
             if self.contains_dual_node(dual_node_ptr) {
-                self.prepare_dual_node_growth(dual_node_ptr, false);  // prepare to shrink
+                self.prepare_dual_node_growth(dual_node_ptr, false); // prepare to shrink
             }
         }
         &mut self.sync_requests
     }
 
     fn contains_dual_node(&self, dual_node_ptr: &DualNodePtr) -> bool {
         self.get_dual_node_index(dual_node_ptr).is_some()
     }
 
+    #[allow(clippy::unnecessary_cast)]
     fn new_partitioned(partitioned_initializer: &PartitionedSolverInitializer) -> Self {
         let active_timestamp = 0;
         // create vertices
-        let mut vertices: Vec<VertexPtr> = partitioned_initializer.owning_range.iter().map(|vertex_index| VertexPtr::new_value(Vertex {
-            vertex_index,
-            is_virtual: false,
-            is_defect: false,
-            mirror_unit: partitioned_initializer.owning_interface.clone(),
-            edges: Vec::new(),
-            propagated_dual_node: None,
-            propagated_grandson_dual_node: None,
-            timestamp: active_timestamp,
-        })).collect();
+        let mut vertices: Vec<VertexPtr> = partitioned_initializer
+            .owning_range
+            .iter()
+            .map(|vertex_index| {
+                VertexPtr::new_value(Vertex {
+                    vertex_index,
+                    is_virtual: false,
+                    is_defect: false,
+                    mirror_unit: partitioned_initializer.owning_interface.clone(),
+                    edges: Vec::new(),
+                    propagated_dual_node: None,
+                    propagated_grandson_dual_node: None,
+                    timestamp: active_timestamp,
+                })
+            })
+            .collect();
         // set virtual vertices
         for &virtual_vertex in partitioned_initializer.virtual_vertices.iter() {
-            let mut vertex = vertices[(virtual_vertex - partitioned_initializer.owning_range.start()) as usize].write(active_timestamp);
+            let mut vertex =
+                vertices[(virtual_vertex - partitioned_initializer.owning_range.start()) as usize].write(active_timestamp);
             vertex.is_virtual = true;
         }
         // add interface vertices
-        let mut mirrored_vertices = HashMap::<VertexIndex, VertexIndex>::new();  // all mirrored vertices mapping to their local indices
+        let mut mirrored_vertices = HashMap::<VertexIndex, VertexIndex>::new(); // all mirrored vertices mapping to their local indices
         for (mirror_unit, interface_vertices) in partitioned_initializer.interfaces.iter() {
             for (vertex_index, is_virtual) in interface_vertices.iter() {
                 mirrored_vertices.insert(*vertex_index, vertices.len() as VertexIndex);
                 vertices.push(VertexPtr::new_value(Vertex {
                     vertex_index: *vertex_index,
-                    is_virtual: *is_virtual,  // interface vertices are always virtual at the beginning
+                    is_virtual: *is_virtual, // interface vertices are always virtual at the beginning
                     is_defect: false,
                     mirror_unit: Some(mirror_unit.clone()),
                     edges: Vec::new(),
                     propagated_dual_node: None,
                     propagated_grandson_dual_node: None,
                     timestamp: active_timestamp,
                 }))
             }
         }
         // set edges
         let mut edges = Vec::<EdgePtr>::new();
         for &(i, j, weight, edge_index) in partitioned_initializer.weighted_edges.iter() {
             assert_ne!(i, j, "invalid edge from and to the same vertex {}", i);
-            assert!(weight % 2 == 0, "edge ({}, {}) has odd weight value; weight should be even", i, j);
+            assert!(
+                weight % 2 == 0,
+                "edge ({}, {}) has odd weight value; weight should be even",
+                i,
+                j
+            );
             assert!(weight >= 0, "edge ({}, {}) is negative-weighted", i, j);
-            debug_assert!(partitioned_initializer.owning_range.contains(i) || mirrored_vertices.contains_key(&i)
-                , "edge ({}, {}) connected to an invalid vertex {}", i, j, i);
-            debug_assert!(partitioned_initializer.owning_range.contains(j) || mirrored_vertices.contains_key(&j)
-                , "edge ({}, {}) connected to an invalid vertex {}", i, j, j);
+            debug_assert!(
+                partitioned_initializer.owning_range.contains(i) || mirrored_vertices.contains_key(&i),
+                "edge ({}, {}) connected to an invalid vertex {}",
+                i,
+                j,
+                i
+            );
+            debug_assert!(
+                partitioned_initializer.owning_range.contains(j) || mirrored_vertices.contains_key(&j),
+                "edge ({}, {}) connected to an invalid vertex {}",
+                i,
+                j,
+                j
+            );
             let left = VertexIndex::min(i, j);
             let right = VertexIndex::max(i, j);
             let left_index = if partitioned_initializer.owning_range.contains(left) {
                 left - partitioned_initializer.owning_range.start()
             } else {
                 mirrored_vertices[&left]
             };
@@ -846,23 +1043,24 @@
                 right_dual_node: None,
                 right_grandson_dual_node: None,
                 timestamp: 0,
                 dedup_timestamp: (0, 0),
             });
             for (a, b) in [(left_index, right_index), (right_index, left_index)] {
                 lock_write!(vertex, vertices[a as usize], active_timestamp);
-                debug_assert!({  // O(N^2) sanity check, debug mode only (actually this bug is not critical, only the shorter edge will take effect)
+                debug_assert!({
+                    // O(N^2) sanity check, debug mode only (actually this bug is not critical, only the shorter edge will take effect)
                     let mut no_duplicate = true;
                     for edge_weak in vertex.edges.iter() {
                         let edge_ptr = edge_weak.upgrade_force();
                         let edge = edge_ptr.read_recursive(active_timestamp);
                         if edge.left == vertices[b as usize].downgrade() || edge.right == vertices[b as usize].downgrade() {
                             no_duplicate = false;
                             eprintln!("duplicated edge between {} and {} with weight w1 = {} and w2 = {}, consider merge them into a single edge", i, j, weight, edge.weight);
-                            break
+                            break;
                         }
                     }
                     no_duplicate
                 });
                 vertex.edges.push(edge_ptr.downgrade());
             }
             edges.push(edge_ptr);
@@ -899,31 +1097,41 @@
     fn bias_dual_node_index(&mut self, bias: NodeIndex) {
         self.unit_module_info.as_mut().unwrap().owning_dual_range.bias_by(bias);
     }
 
     fn execute_sync_event(&mut self, sync_event: &SyncRequest) {
         let active_timestamp = self.active_timestamp;
         debug_assert!(self.contains_vertex(sync_event.vertex_index));
-        let propagated_dual_node_internal_ptr = sync_event.propagated_dual_node.as_ref().map(|(dual_node_weak, dual_variable)| {
-            self.get_otherwise_add_dual_node(&dual_node_weak.upgrade_force(), *dual_variable)
-        });
-        let propagated_grandson_dual_node_internal_ptr = sync_event.propagated_grandson_dual_node.as_ref().map(|(dual_node_weak, dual_variable)| {
-            self.get_otherwise_add_dual_node(&dual_node_weak.upgrade_force(), *dual_variable)
-        });
-        let local_vertex_index = self.get_vertex_index(sync_event.vertex_index).expect("cannot synchronize at a non-existing vertex");
+        let propagated_dual_node_internal_ptr =
+            sync_event
+                .propagated_dual_node
+                .as_ref()
+                .map(|(dual_node_weak, dual_variable, _representative_vertex)| {
+                    self.get_otherwise_add_dual_node(&dual_node_weak.upgrade_force(), *dual_variable)
+                });
+        let propagated_grandson_dual_node_internal_ptr = sync_event.propagated_grandson_dual_node.as_ref().map(
+            |(dual_node_weak, dual_variable, _representative_vertex)| {
+                self.get_otherwise_add_dual_node(&dual_node_weak.upgrade_force(), *dual_variable)
+            },
+        );
+        let local_vertex_index = self
+            .get_vertex_index(sync_event.vertex_index)
+            .expect("cannot synchronize at a non-existing vertex");
         let vertex_ptr = &self.vertices[local_vertex_index];
         vertex_ptr.dynamic_clear(active_timestamp);
         let mut vertex = vertex_ptr.write(active_timestamp);
         if vertex.propagated_dual_node == propagated_dual_node_internal_ptr.as_ref().map(|x| x.downgrade()) {
             // actually this may happen: if the same vertex is propagated from two different units with the same distance
             // to the closest grandson, it may happen that sync event will conflict on the grandson...
             // this conflict doesn't matter anyway: any grandson is good, as long as they're consistent
             // assert_eq!(vertex.propagated_grandson_dual_node, propagated_grandson_dual_node_internal_ptr.as_ref().map(|x| x.downgrade()));
-            vertex.propagated_grandson_dual_node = propagated_grandson_dual_node_internal_ptr.as_ref().map(|x| x.downgrade());
-        } else {  // conflict with existing value, action needed
+            vertex.propagated_grandson_dual_node =
+                propagated_grandson_dual_node_internal_ptr.as_ref().map(|x| x.downgrade());
+        } else {
+            // conflict with existing value, action needed
             // first vacate the vertex, recovering dual node boundaries accordingly
             if let Some(dual_node_internal_weak) = vertex.propagated_dual_node.as_ref() {
                 debug_assert!(!vertex.is_defect, "cannot vacate a syndrome vertex: it shouldn't happen that a syndrome vertex is updated in any partitioned unit");
                 let mut updated_boundary = Vec::<(bool, EdgeWeak)>::new();
                 let dual_node_internal_ptr = dual_node_internal_weak.upgrade_force();
                 lock_write!(dual_node_internal, dual_node_internal_ptr);
                 vertex.propagated_dual_node = None;
@@ -935,16 +1143,27 @@
                     let mut edge = edge_ptr.write(active_timestamp);
                     let this_vertex_ptr = if is_left {
                         edge.left.upgrade_force()
                     } else {
                         edge.right.upgrade_force()
                     };
                     if &this_vertex_ptr == vertex_ptr {
-                        debug_assert!(if is_left { edge.left_growth == 0 } else { edge.right_growth == 0 }, "vacating a non-boundary vertex is forbidden");
-                        let dual_node = if is_left { &edge.left_dual_node } else { &edge.right_dual_node };
+                        debug_assert!(
+                            if is_left {
+                                edge.left_growth == 0
+                            } else {
+                                edge.right_growth == 0
+                            },
+                            "vacating a non-boundary vertex is forbidden"
+                        );
+                        let dual_node = if is_left {
+                            &edge.left_dual_node
+                        } else {
+                            &edge.right_dual_node
+                        };
                         if let Some(dual_node_weak) = dual_node.as_ref() {
                             // sanity check: if exists, must be the same
                             debug_assert!(dual_node_weak.upgrade_force() == dual_node_internal_ptr);
                             // reset the dual node to be unoccupied
                             if is_left {
                                 edge.left_dual_node = None;
                                 edge.left_grandson_dual_node = None;
@@ -959,15 +1178,19 @@
                 }
                 // iterate over the edges around the vertex to add edges to the boundary
                 for edge_weak in vertex.edges.iter() {
                     let edge_ptr = edge_weak.upgrade_force();
                     edge_ptr.dynamic_clear(active_timestamp);
                     let mut edge = edge_ptr.write(active_timestamp);
                     let is_left = vertex_ptr.downgrade() == edge.left;
-                    let dual_node = if is_left { &edge.left_dual_node } else { &edge.right_dual_node };
+                    let dual_node = if is_left {
+                        &edge.left_dual_node
+                    } else {
+                        &edge.right_dual_node
+                    };
                     if let Some(dual_node_weak) = dual_node.as_ref() {
                         // sanity check: if exists, must be the same
                         debug_assert!(dual_node_weak.upgrade_force() == dual_node_internal_ptr);
                         // need to add to the boundary
                         if is_left {
                             edge.left_dual_node = None;
                             edge.left_grandson_dual_node = None;
@@ -990,86 +1213,91 @@
                 lock_write!(dual_node_internal, dual_node_internal_ptr);
                 for edge_weak in vertex.edges.iter() {
                     let edge_ptr = edge_weak.upgrade_force();
                     edge_ptr.dynamic_clear(active_timestamp);
                     let mut edge = edge_ptr.write(active_timestamp);
                     let is_left = vertex_ptr.downgrade() == edge.left;
                     if is_left {
-                        debug_assert_eq!(edge.left_dual_node, None, "edges incident to the vertex must have been vacated");
+                        debug_assert_eq!(
+                            edge.left_dual_node, None,
+                            "edges incident to the vertex must have been vacated"
+                        );
                         edge.left_dual_node = Some(dual_node_internal_ptr.downgrade());
                         edge.left_grandson_dual_node = Some(grandson_dual_node_internal_ptr.downgrade());
                     } else {
-                        debug_assert_eq!(edge.right_dual_node, None, "edges incident to the vertex must have been vacated");
+                        debug_assert_eq!(
+                            edge.right_dual_node, None,
+                            "edges incident to the vertex must have been vacated"
+                        );
                         edge.right_dual_node = Some(dual_node_internal_ptr.downgrade());
                         edge.right_grandson_dual_node = Some(grandson_dual_node_internal_ptr.downgrade());
                     }
                     dual_node_internal.boundary.push((is_left, edge_weak.clone()));
                 }
                 self.active_list.push(dual_node_internal_ptr.downgrade());
             }
-            
         }
     }
-
 }
 
 /*
 Implementing fast clear operations
 */
 
 impl FastClear for Edge {
-
     fn hard_clear(&mut self) {
         self.left_growth = 0;
         self.right_growth = 0;
         self.left_dual_node = None;
         self.left_grandson_dual_node = None;
         self.right_dual_node = None;
         self.right_grandson_dual_node = None;
     }
 
     #[inline(always)]
-    fn get_timestamp(&self) -> FastClearTimestamp { self.timestamp }
+    fn get_timestamp(&self) -> FastClearTimestamp {
+        self.timestamp
+    }
     #[inline(always)]
-    fn set_timestamp(&mut self, timestamp: FastClearTimestamp) { self.timestamp = timestamp; }
-
+    fn set_timestamp(&mut self, timestamp: FastClearTimestamp) {
+        self.timestamp = timestamp;
+    }
 }
 
 impl FastClear for Vertex {
-
     fn hard_clear(&mut self) {
         self.is_defect = false;
         self.propagated_dual_node = None;
         self.propagated_grandson_dual_node = None;
     }
 
     #[inline(always)]
-    fn get_timestamp(&self) -> FastClearTimestamp { self.timestamp }
+    fn get_timestamp(&self) -> FastClearTimestamp {
+        self.timestamp
+    }
     #[inline(always)]
-    fn set_timestamp(&mut self, timestamp: FastClearTimestamp) { self.timestamp = timestamp; }
-
+    fn set_timestamp(&mut self, timestamp: FastClearTimestamp) {
+        self.timestamp = timestamp;
+    }
 }
 
 impl Vertex {
-
     /// if this vertex is a mirrored vertex and it's disabled, it can be temporarily matched just like a virtual vertex
     pub fn is_mirror_blocked(&self) -> bool {
         if let Some(ref mirror_unit_ptr) = self.mirror_unit {
             let mirror_unit_ptr = mirror_unit_ptr.upgrade_force();
             let mirror_unit = mirror_unit_ptr.read_recursive();
             !mirror_unit.enabled
         } else {
             false
         }
     }
-
 }
 
 impl DualModuleSerial {
-
     /// hard clear all growth (manual call not recommended due to performance drawback)
     pub fn hard_clear_graph(&mut self) {
         for edge in self.edges.iter() {
             let mut edge = edge.write_force();
             edge.hard_clear();
             edge.timestamp = 0;
         }
@@ -1079,46 +1307,47 @@
             vertex.timestamp = 0;
         }
         self.active_timestamp = 0;
     }
 
     /// soft clear all growth
     pub fn clear_graph(&mut self) {
-        if self.active_timestamp == FastClearTimestamp::MAX {  // rarely happens
+        if self.active_timestamp == FastClearTimestamp::MAX {
+            // rarely happens
             self.hard_clear_graph();
         }
-        self.active_timestamp += 1;  // implicitly clear all edges growth
+        self.active_timestamp += 1; // implicitly clear all edges growth
     }
 
     /// necessary for boundary deduplicate when the unit is partitioned
     fn hard_clear_edge_dedup(&mut self) {
         for edge in self.edges.iter() {
             let mut edge = edge.write_force();
-            edge.dedup_timestamp = (0 ,0);
+            edge.dedup_timestamp = (0, 0);
         }
         self.edge_dedup_timestamp = 0;
     }
 
     fn clear_edge_dedup(&mut self) {
-        if self.edge_dedup_timestamp == FastClearTimestamp::MAX {  // rarely happens
+        if self.edge_dedup_timestamp == FastClearTimestamp::MAX {
+            // rarely happens
             self.hard_clear_edge_dedup();
         }
-        self.edge_dedup_timestamp += 1;  // implicitly clear all edges growth
+        self.edge_dedup_timestamp += 1; // implicitly clear all edges growth
     }
 
     /// increment the global cycle so that each node in the active list can be accessed exactly once
+    #[allow(clippy::unnecessary_cast)]
     fn renew_active_list(&mut self) {
         if self.current_cycle == usize::MAX {
             for i in 0..self.nodes_length {
                 let internal_dual_node_ptr = {
                     match self.nodes[i].as_ref() {
-                        Some(internal_dual_node_ptr) => {
-                            internal_dual_node_ptr.clone()
-                        },
-                        _ => { continue }
+                        Some(internal_dual_node_ptr) => internal_dual_node_ptr.clone(),
+                        _ => continue,
                     }
                 };
                 let mut internal_dual_node = internal_dual_node_ptr.write();
                 internal_dual_node.last_visit_cycle = 0;
             }
             self.current_cycle = 0;
         }
@@ -1126,179 +1355,266 @@
         // renew the active_list
         let mut updated_active_list = Vec::with_capacity(self.active_list.len());
         for i in 0..self.active_list.len() {
             let (dual_node_ptr, internal_dual_node_ptr) = {
                 match self.active_list[i].upgrade() {
                     Some(internal_dual_node_ptr) => {
                         let mut dual_node_internal = internal_dual_node_ptr.write();
-                        if self.nodes[dual_node_internal.index as usize].is_none() { continue }  // removed
-                        if dual_node_internal.last_visit_cycle == self.current_cycle { continue }  // visited
-                        dual_node_internal.last_visit_cycle = self.current_cycle;  // mark as visited
+                        if self.nodes[dual_node_internal.index as usize].is_none() {
+                            continue;
+                        } // removed
+                        if dual_node_internal.last_visit_cycle == self.current_cycle {
+                            continue;
+                        } // visited
+                        dual_node_internal.last_visit_cycle = self.current_cycle; // mark as visited
                         (dual_node_internal.origin.upgrade_force(), internal_dual_node_ptr.clone())
-                    },
-                    _ => { continue }
+                    }
+                    _ => continue,
                 }
             };
             let dual_node = dual_node_ptr.read_recursive();
             match dual_node.grow_state {
                 DualNodeGrowState::Grow | DualNodeGrowState::Shrink => {
                     updated_active_list.push(internal_dual_node_ptr.downgrade());
-                }, DualNodeGrowState::Stay => {
-
-                },  // no longer in the active list
+                }
+                DualNodeGrowState::Stay => {} // no longer in the active list
             };
         }
         self.active_list = updated_active_list;
     }
 
-    fn sanity_check_grandson(&self, propagated_dual_node_weak: &DualNodeInternalWeak, propagated_grandson_dual_node_weak: &DualNodeInternalWeak) -> Result<(), String> {
+    fn sanity_check_grandson(
+        &self,
+        propagated_dual_node_weak: &DualNodeInternalWeak,
+        propagated_grandson_dual_node_weak: &DualNodeInternalWeak,
+    ) -> Result<(), String> {
         let propagated_dual_node_ptr = propagated_dual_node_weak.upgrade_force();
         let propagated_grandson_dual_node_ptr = propagated_grandson_dual_node_weak.upgrade_force();
         let propagated_dual_node = propagated_dual_node_ptr.read_recursive();
         let propagated_grandson_dual_node = propagated_grandson_dual_node_ptr.read_recursive();
         let propagated_node_ptr = propagated_dual_node.origin.upgrade_force();
         let propagated_node = propagated_node_ptr.read_recursive();
         let propagated_grandson_ptr = propagated_grandson_dual_node.origin.upgrade_force();
         let propagated_grandson = propagated_grandson_ptr.read_recursive();
-        if matches!(propagated_grandson.class, DualNodeClass::DefectVertex{..}) {
-            if matches!(propagated_node.class, DualNodeClass::DefectVertex{..}) {
+        if matches!(propagated_grandson.class, DualNodeClass::DefectVertex { .. }) {
+            if matches!(propagated_node.class, DualNodeClass::DefectVertex { .. }) {
                 if propagated_dual_node_ptr != propagated_grandson_dual_node_ptr {
-                    return Err(format!("syndrome node {:?} must have grandson equal to itself {:?}", propagated_dual_node_ptr, propagated_grandson_dual_node_ptr))
+                    return Err(format!(
+                        "syndrome node {:?} must have grandson equal to itself {:?}",
+                        propagated_dual_node_ptr, propagated_grandson_dual_node_ptr
+                    ));
                 }
             } else {
                 // test if grandson is a real grandson
                 drop(propagated_grandson);
                 let mut descendant_ptr = propagated_grandson_ptr;
                 loop {
                     let descendant = descendant_ptr.read_recursive();
                     if let Some(descendant_parent_ptr) = descendant.parent_blossom.as_ref() {
                         let descendant_parent_ptr = descendant_parent_ptr.upgrade_force();
                         if descendant_parent_ptr == propagated_node_ptr {
-                            return Ok(())
+                            return Ok(());
                         }
                         drop(descendant);
                         descendant_ptr = descendant_parent_ptr;
                     } else {
                         return Err("grandson check failed".to_string());
                     }
                 }
             }
         } else {
-            return Err("grandson must be a vertex".to_string())
+            return Err("grandson must be a vertex".to_string());
         }
         Ok(())
     }
 
     /// do a sanity check of if all the nodes are in consistent state
+    #[allow(clippy::unnecessary_cast)]
     pub fn sanity_check(&self) -> Result<(), String> {
         let active_timestamp = self.active_timestamp;
         for vertex_ptr in self.vertices.iter() {
             vertex_ptr.dynamic_clear(active_timestamp);
             let vertex = vertex_ptr.read_recursive(active_timestamp);
             if let Some(propagated_grandson_dual_node) = vertex.propagated_grandson_dual_node.as_ref() {
                 if let Some(propagated_dual_node) = vertex.propagated_dual_node.as_ref() {
                     self.sanity_check_grandson(propagated_dual_node, propagated_grandson_dual_node)?;
                 } else {
-                    return Err(format!("vertex {} has propagated grandson dual node {:?} but missing propagated dual node"
-                        , vertex.vertex_index, vertex.propagated_grandson_dual_node))
+                    return Err(format!(
+                        "vertex {} has propagated grandson dual node {:?} but missing propagated dual node",
+                        vertex.vertex_index, vertex.propagated_grandson_dual_node
+                    ));
                 }
             }
             if vertex.propagated_dual_node.is_some() && vertex.propagated_grandson_dual_node.is_none() {
-                return Err(format!("vertex {} has propagated dual node {:?} but missing grandson", vertex.vertex_index, vertex.propagated_dual_node))
+                return Err(format!(
+                    "vertex {} has propagated dual node {:?} but missing grandson",
+                    vertex.vertex_index, vertex.propagated_dual_node
+                ));
             }
         }
         // sanity check that boundary doesn't include duplicate edges
         let mut duplicate_edges = HashMap::<(bool, EdgeIndex), NodeIndex>::new();
         for node_index in 0..self.nodes_length as NodeIndex {
             let node_ptr = &self.nodes[node_index as usize];
             if let Some(node_ptr) = node_ptr {
                 let dual_node_internal = node_ptr.read_recursive();
-                if dual_node_internal.origin.upgrade_force().read_recursive().parent_blossom.is_some() {
-                    continue  // skip this node, since it's inactive
+                if dual_node_internal
+                    .origin
+                    .upgrade_force()
+                    .read_recursive()
+                    .parent_blossom
+                    .is_some()
+                {
+                    continue; // skip this node, since it's inactive
                 }
                 for (is_left, edge_weak) in dual_node_internal.boundary.iter() {
                     let edge_ptr = edge_weak.upgrade_force();
                     let edge = edge_ptr.read_recursive(active_timestamp);
                     if duplicate_edges.contains_key(&(*is_left, edge.edge_index)) {
-                        return Err(format!("boundary edge {:?} appears twice in node {} and {}", (*is_left, edge.edge_index), duplicate_edges.get(&(*is_left, edge.edge_index)).unwrap(), node_index));
+                        return Err(format!(
+                            "boundary edge {:?} appears twice in node {} and {}",
+                            (*is_left, edge.edge_index),
+                            duplicate_edges.get(&(*is_left, edge.edge_index)).unwrap(),
+                            node_index
+                        ));
                     }
                     duplicate_edges.insert((*is_left, edge.edge_index), node_index);
                 }
             }
         }
         Ok(())
     }
-
 }
 
 /*
 Implementing visualization functions
 */
 
 impl FusionVisualizer for DualModuleSerial {
+    #[allow(clippy::unnecessary_cast)]
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         // do the sanity check first before taking snapshot
         self.sanity_check().unwrap();
         let active_timestamp = self.active_timestamp;
-        let mut vertices: Vec::<serde_json::Value> = (0..self.vertex_num).map(|_| serde_json::Value::Null).collect();
+        let mut vertices: Vec<serde_json::Value> = (0..self.vertex_num).map(|_| serde_json::Value::Null).collect();
         for vertex_ptr in self.vertices.iter() {
             vertex_ptr.dynamic_clear(active_timestamp);
             let vertex = vertex_ptr.read_recursive(active_timestamp);
             vertices[vertex.vertex_index as usize] = json!({
                 if abbrev { "v" } else { "is_virtual" }: i32::from(vertex.is_virtual),
             });
-            if self.owning_range.contains(vertex.vertex_index) {  // otherwise I don't know whether it's syndrome or not
-                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert((if abbrev { "s" } else { "is_defect" })
-                    .to_string(), json!(i32::from(vertex.is_defect)));
-            }
-            if let Some(value) = vertex.propagated_dual_node.as_ref().map(|weak| weak.upgrade_force().read_recursive().origin.upgrade_force().read_recursive().index) {
-                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert((if abbrev { "p" } else { "propagated_dual_node" })
-                    .to_string(), json!(value));
-            }
-            if let Some(value) = vertex.propagated_grandson_dual_node.as_ref().map(|weak| weak.upgrade_force().read_recursive().origin.upgrade_force().read_recursive().index) {
-                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert((if abbrev { "pg" } else { "propagated_grandson_dual_node" })
-                    .to_string(), json!(value));
+            if self.owning_range.contains(vertex.vertex_index) {
+                // otherwise I don't know whether it's syndrome or not
+                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert(
+                    (if abbrev { "s" } else { "is_defect" }).to_string(),
+                    json!(i32::from(vertex.is_defect)),
+                );
+            }
+            if let Some(value) = vertex.propagated_dual_node.as_ref().map(|weak| {
+                weak.upgrade_force()
+                    .read_recursive()
+                    .origin
+                    .upgrade_force()
+                    .read_recursive()
+                    .index
+            }) {
+                vertices[vertex.vertex_index as usize]
+                    .as_object_mut()
+                    .unwrap()
+                    .insert((if abbrev { "p" } else { "propagated_dual_node" }).to_string(), json!(value));
+            }
+            if let Some(value) = vertex.propagated_grandson_dual_node.as_ref().map(|weak| {
+                weak.upgrade_force()
+                    .read_recursive()
+                    .origin
+                    .upgrade_force()
+                    .read_recursive()
+                    .index
+            }) {
+                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert(
+                    (if abbrev { "pg" } else { "propagated_grandson_dual_node" }).to_string(),
+                    json!(value),
+                );
             }
             if let Some(mirror_unit_ptr) = vertex.mirror_unit.as_ref() {
                 let mirror_unit_ptr = mirror_unit_ptr.upgrade_force();
                 let mirror_unit = mirror_unit_ptr.read_recursive();
-                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert((if abbrev { "mi" } else { "mirror_unit_index" }).to_string()
-                    , json!(mirror_unit.unit_index));
-                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert((if abbrev { "me" } else { "mirror_enabled" }).to_string()
-                    , json!(i32::from(mirror_unit.enabled)));
+                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert(
+                    (if abbrev { "mi" } else { "mirror_unit_index" }).to_string(),
+                    json!(mirror_unit.unit_index),
+                );
+                vertices[vertex.vertex_index as usize].as_object_mut().unwrap().insert(
+                    (if abbrev { "me" } else { "mirror_enabled" }).to_string(),
+                    json!(i32::from(mirror_unit.enabled)),
+                );
             }
         }
-        let mut edges: Vec::<serde_json::Value> = (0..self.edge_num).map(|_| serde_json::Value::Null).collect();
+        let mut edges: Vec<serde_json::Value> = (0..self.edge_num).map(|_| serde_json::Value::Null).collect();
         for edge_ptr in self.edges.iter() {
             edge_ptr.dynamic_clear(active_timestamp);
             let edge = edge_ptr.read_recursive(active_timestamp);
             edges[edge.edge_index as usize] = json!({
                 if abbrev { "w" } else { "weight" }: edge.weight,
                 if abbrev { "l" } else { "left" }: edge.left.upgrade_force().read_recursive(active_timestamp).vertex_index,
                 if abbrev { "r" } else { "right" }: edge.right.upgrade_force().read_recursive(active_timestamp).vertex_index,
                 if abbrev { "lg" } else { "left_growth" }: edge.left_growth,
                 if abbrev { "rg" } else { "right_growth" }: edge.right_growth,
             });
-            if let Some(value) = edge.left_dual_node.as_ref().map(|weak| weak.upgrade_force().read_recursive().origin.upgrade_force().read_recursive().index) {
-                edges[edge.edge_index as usize].as_object_mut().unwrap().insert((if abbrev { "ld" } else { "left_dual_node" })
-                    .to_string(), json!(value));
-            }
-            if let Some(value) = edge.left_grandson_dual_node.as_ref().map(|weak| weak.upgrade_force().read_recursive().origin.upgrade_force().read_recursive().index) {
-                edges[edge.edge_index as usize].as_object_mut().unwrap().insert((if abbrev { "lgd" } else { "left_grandson_dual_node" })
-                    .to_string(), json!(value));
-            }
-            if let Some(value) = edge.right_dual_node.as_ref().map(|weak| weak.upgrade_force().read_recursive().origin.upgrade_force().read_recursive().index) {
-                edges[edge.edge_index as usize].as_object_mut().unwrap().insert((if abbrev { "rd" } else { "right_dual_node" })
-                    .to_string(), json!(value));
-            }
-            if let Some(value) = edge.right_grandson_dual_node.as_ref().map(|weak| weak.upgrade_force().read_recursive().origin.upgrade_force().read_recursive().index) {
-                edges[edge.edge_index as usize].as_object_mut().unwrap().insert((if abbrev { "rgd" } else { "right_grandson_dual_node" })
-                    .to_string(), json!(value));
+            if let Some(value) = edge.left_dual_node.as_ref().map(|weak| {
+                weak.upgrade_force()
+                    .read_recursive()
+                    .origin
+                    .upgrade_force()
+                    .read_recursive()
+                    .index
+            }) {
+                edges[edge.edge_index as usize]
+                    .as_object_mut()
+                    .unwrap()
+                    .insert((if abbrev { "ld" } else { "left_dual_node" }).to_string(), json!(value));
+            }
+            if let Some(value) = edge.left_grandson_dual_node.as_ref().map(|weak| {
+                weak.upgrade_force()
+                    .read_recursive()
+                    .origin
+                    .upgrade_force()
+                    .read_recursive()
+                    .index
+            }) {
+                edges[edge.edge_index as usize].as_object_mut().unwrap().insert(
+                    (if abbrev { "lgd" } else { "left_grandson_dual_node" }).to_string(),
+                    json!(value),
+                );
+            }
+            if let Some(value) = edge.right_dual_node.as_ref().map(|weak| {
+                weak.upgrade_force()
+                    .read_recursive()
+                    .origin
+                    .upgrade_force()
+                    .read_recursive()
+                    .index
+            }) {
+                edges[edge.edge_index as usize]
+                    .as_object_mut()
+                    .unwrap()
+                    .insert((if abbrev { "rd" } else { "right_dual_node" }).to_string(), json!(value));
+            }
+            if let Some(value) = edge.right_grandson_dual_node.as_ref().map(|weak| {
+                weak.upgrade_force()
+                    .read_recursive()
+                    .origin
+                    .upgrade_force()
+                    .read_recursive()
+                    .index
+            }) {
+                edges[edge.edge_index as usize].as_object_mut().unwrap().insert(
+                    (if abbrev { "rgd" } else { "right_grandson_dual_node" }).to_string(),
+                    json!(value),
+                );
             }
-            
         }
         let mut value = json!({
             "vertices": vertices,
             "edges": edges,
         });
         // TODO: since each serial module only processes a part of the dual nodes, it's not feasible to list them in a reasonable vector now...
         // update the visualizer to be able to join multiple dual nodes
@@ -1313,137 +1629,165 @@
                             (*is_left, edge_weak.upgrade_force().read_recursive(active_timestamp).edge_index)).collect::<Vec<(bool, EdgeIndex)>>(),
                         if abbrev { "d" } else { "dual_variable" }: node.dual_variable,
                     }));
                 } else {
                     dual_nodes.push(json!(null));
                 }
             }
-            value.as_object_mut().unwrap().insert("dual_nodes".to_string(), json!(dual_nodes));
+            value
+                .as_object_mut()
+                .unwrap()
+                .insert("dual_nodes".to_string(), json!(dual_nodes));
         }
         value
     }
 }
 
 /*
 Implement internal helper functions that maintains the state of dual clusters
 */
 
 impl DualModuleSerial {
-
     /// register a new dual node ptr, but not creating the internal dual node
     fn register_dual_node_ptr(&mut self, dual_node_ptr: &DualNodePtr) {
         // println!("unit {:?}, register_dual_node_ptr: {:?}", self.unit_module_info, dual_node_ptr);
         let node = dual_node_ptr.read_recursive();
         if let Some(unit_module_info) = self.unit_module_info.as_mut() {
-            if unit_module_info.owning_dual_range.is_empty() {  // set the range instead of inserting into the lookup table, to minimize table lookup
+            if unit_module_info.owning_dual_range.is_empty() {
+                // set the range instead of inserting into the lookup table, to minimize table lookup
                 unit_module_info.owning_dual_range = VertexRange::new(node.index, node.index);
             }
-            if unit_module_info.owning_dual_range.end() == node.index && self.nodes_length == unit_module_info.owning_dual_range.len() {
+            if unit_module_info.owning_dual_range.end() == node.index
+                && self.nodes_length == unit_module_info.owning_dual_range.len()
+            {
                 // it's able to append into the owning range, minimizing table lookup and thus better performance
                 unit_module_info.owning_dual_range.append_by(1);
             } else {
                 // will be inserted at this place
-                unit_module_info.dual_node_pointers.insert(dual_node_ptr.clone(), self.nodes_length);
+                unit_module_info
+                    .dual_node_pointers
+                    .insert(dual_node_ptr.clone(), self.nodes_length);
             }
         } else {
-            debug_assert!(self.nodes_length as NodeIndex == node.index, "dual node must be created in a sequential manner: no missing or duplicating");
+            debug_assert!(
+                self.nodes_length as NodeIndex == node.index,
+                "dual node must be created in a sequential manner: no missing or duplicating"
+            );
         }
         // println!("unit {:?}, register_dual_node_ptr: {:?}", self.unit_module_info, dual_node_ptr);
     }
 
     /// get the local index of a dual node, thus has usize type
+    #[allow(clippy::unnecessary_cast)]
     pub fn get_dual_node_index(&self, dual_node_ptr: &DualNodePtr) -> Option<usize> {
         let dual_node = dual_node_ptr.read_recursive();
         if let Some(unit_module_info) = self.unit_module_info.as_ref() {
             if unit_module_info.owning_dual_range.contains(dual_node.index) {
-                debug_assert!(dual_node.belonging.upgrade_force().read_recursive().parent.is_none(), "dual node is not updated");
+                debug_assert!(
+                    dual_node.belonging.upgrade_force().read_recursive().parent.is_none(),
+                    "dual node is not updated"
+                );
                 Some((dual_node.index - unit_module_info.owning_dual_range.start()) as usize)
             } else {
                 // println!("from unit {:?}, dual_node: {}", self.unit_module_info, dual_node.index);
                 unit_module_info.dual_node_pointers.get(dual_node_ptr).copied()
             }
         } else {
             Some(dual_node.index as usize)
         }
     }
 
     /// get the local index of a vertex, thus has usize type
+    #[allow(clippy::unnecessary_cast)]
     pub fn get_vertex_index(&self, vertex_index: VertexIndex) -> Option<usize> {
         if self.owning_range.contains(vertex_index) {
-            return Some((vertex_index - self.owning_range.start()) as usize)
+            return Some((vertex_index - self.owning_range.start()) as usize);
         }
         if let Some(unit_module_info) = self.unit_module_info.as_ref() {
             if let Some(index) = unit_module_info.mirrored_vertices.get(&vertex_index) {
-                return Some(*index as usize)
+                return Some(*index as usize);
             }
         }
         None
     }
 
     pub fn get_dual_node_internal_ptr(&self, dual_node_ptr: &DualNodePtr) -> DualNodeInternalPtr {
         self.get_dual_node_internal_ptr_optional(dual_node_ptr).unwrap()
     }
 
     /// dual node ptr may not hold in this module
     pub fn get_dual_node_internal_ptr_optional(&self, dual_node_ptr: &DualNodePtr) -> Option<DualNodeInternalPtr> {
         self.get_dual_node_index(dual_node_ptr).map(|dual_node_index| {
             let dual_node_internal_ptr = self.nodes[dual_node_index].as_ref().expect("internal dual node must exists");
-            debug_assert!(dual_node_ptr == &dual_node_internal_ptr.read_recursive().origin.upgrade_force(), "dual node and dual internal node must corresponds to each other");
+            debug_assert!(
+                dual_node_ptr == &dual_node_internal_ptr.read_recursive().origin.upgrade_force(),
+                "dual node and dual internal node must corresponds to each other"
+            );
             dual_node_internal_ptr.clone()
         })
     }
 
     /// possibly add dual node only when sync_event is provided
-    pub fn get_otherwise_add_dual_node(&mut self, dual_node_ptr: &DualNodePtr, dual_variable: Weight) -> DualNodeInternalPtr {
+    #[allow(clippy::unnecessary_cast)]
+    pub fn get_otherwise_add_dual_node(
+        &mut self,
+        dual_node_ptr: &DualNodePtr,
+        dual_variable: Weight,
+    ) -> DualNodeInternalPtr {
         let dual_node_index = self.get_dual_node_index(dual_node_ptr).unwrap_or_else(|| {
             // add a new internal dual node corresponding to the dual_node_ptr
             self.register_dual_node_ptr(dual_node_ptr);
             let node_index = self.nodes_length as NodeIndex;
-            let node_internal_ptr = if node_index < self.nodes.len() as NodeIndex && self.nodes[node_index as usize].is_some() {
-                let node_ptr = self.nodes[node_index as usize].as_ref().unwrap().clone();
-                let mut node = node_ptr.write();
-                node.origin = dual_node_ptr.downgrade();
-                node.index = node_index;
-                node.dual_variable = dual_variable;
-                node.boundary.clear();
-                node.overgrown_stack.clear();
-                node.last_visit_cycle = 0;
-                drop(node);
-                node_ptr
-            } else {
-                DualNodeInternalPtr::new_value(DualNodeInternal {
-                    origin: dual_node_ptr.downgrade(),
-                    index: node_index,
-                    dual_variable,
-                    boundary: Vec::new(),
-                    overgrown_stack: Vec::new(),
-                    last_visit_cycle: 0,
-                })
-            };
+            let node_internal_ptr =
+                if node_index < self.nodes.len() as NodeIndex && self.nodes[node_index as usize].is_some() {
+                    let node_ptr = self.nodes[node_index as usize].as_ref().unwrap().clone();
+                    let mut node = node_ptr.write();
+                    node.origin = dual_node_ptr.downgrade();
+                    node.index = node_index;
+                    node.dual_variable = dual_variable;
+                    node.boundary.clear();
+                    node.overgrown_stack.clear();
+                    node.last_visit_cycle = 0;
+                    drop(node);
+                    node_ptr
+                } else {
+                    DualNodeInternalPtr::new_value(DualNodeInternal {
+                        origin: dual_node_ptr.downgrade(),
+                        index: node_index,
+                        dual_variable,
+                        boundary: Vec::new(),
+                        overgrown_stack: Vec::new(),
+                        last_visit_cycle: 0,
+                    })
+                };
             self.active_list.push(node_internal_ptr.downgrade());
             self.nodes_length += 1;
             if self.nodes.len() < self.nodes_length {
                 self.nodes.push(None);
             }
             self.nodes[node_index as usize] = Some(node_internal_ptr);
             node_index as usize
         });
         let dual_node_internal_ptr = self.nodes[dual_node_index].as_ref().expect("internal dual node must exists");
-        debug_assert!(dual_node_ptr == &dual_node_internal_ptr.read_recursive().origin.upgrade_force(), "dual node and dual internal node must corresponds to each other");
+        debug_assert!(
+            dual_node_ptr == &dual_node_internal_ptr.read_recursive().origin.upgrade_force(),
+            "dual node and dual internal node must corresponds to each other"
+        );
         dual_node_internal_ptr.clone()
     }
 
     /// this is equivalent to [`DualModuleSerial::prepare_dual_node_growth`] when there are no 0 weight edges, but when it encounters zero-weight edges, it will report `true`
     pub fn prepare_dual_node_growth_single(&mut self, dual_node_ptr: &DualNodePtr, is_grow: bool) -> bool {
         let active_timestamp = self.active_timestamp;
         self.updated_boundary.clear();
         self.propagating_vertices.clear();
         let dual_node_internal_ptr = self.get_dual_node_internal_ptr(dual_node_ptr);
         let mut newly_propagated_edge_has_zero_weight = false;
-        if is_grow {  // gracefully update the boundary to ease growing
+        if is_grow {
+            // gracefully update the boundary to ease growing
             let dual_node_internal = dual_node_internal_ptr.read_recursive();
             for (is_left, edge_weak) in dual_node_internal.boundary.iter() {
                 let edge_ptr = edge_weak.upgrade_force();
                 let is_left = *is_left;
                 let edge = edge_ptr.read_recursive(active_timestamp);
                 let peer_dual_node: &Option<DualNodeInternalWeak> = if is_left {
                     &edge.right_dual_node
@@ -1456,59 +1800,82 @@
                         edge.right.upgrade_force()
                     } else {
                         edge.left.upgrade_force()
                     };
                     // to avoid already occupied node being propagated
                     peer_vertex_ptr.dynamic_clear(active_timestamp);
                     let peer_vertex = peer_vertex_ptr.read_recursive(active_timestamp);
-                    if peer_vertex.is_virtual || peer_vertex.is_mirror_blocked() {  // virtual node is never propagated, so keep this edge in the boundary
+                    if peer_vertex.is_virtual || peer_vertex.is_mirror_blocked() {
+                        // virtual node is never propagated, so keep this edge in the boundary
                         self.updated_boundary.push((is_left, edge_weak.clone()));
                     } else {
-                        debug_assert!(peer_vertex.propagated_dual_node.is_none(), "growing into another propagated vertex forbidden");
-                        debug_assert!(peer_vertex.propagated_grandson_dual_node.is_none(), "growing into another propagated vertex forbidden");
-                        self.propagating_vertices.push((peer_vertex_ptr.downgrade(), if is_left { edge.left_grandson_dual_node.clone() } else { edge.right_grandson_dual_node.clone() }));
+                        debug_assert!(
+                            peer_vertex.propagated_dual_node.is_none(),
+                            "growing into another propagated vertex forbidden"
+                        );
+                        debug_assert!(
+                            peer_vertex.propagated_grandson_dual_node.is_none(),
+                            "growing into another propagated vertex forbidden"
+                        );
+                        self.propagating_vertices.push((
+                            peer_vertex_ptr.downgrade(),
+                            if is_left {
+                                edge.left_grandson_dual_node.clone()
+                            } else {
+                                edge.right_grandson_dual_node.clone()
+                            },
+                        ));
                         // this edge is dropped, so we need to set both end of this edge to this dual node
-                        drop(edge);  // unlock read
+                        drop(edge); // unlock read
                         let mut edge = edge_ptr.write(active_timestamp);
                         if is_left {
                             edge.right_dual_node = Some(dual_node_internal_ptr.downgrade());
                             debug_assert!(edge.left_grandson_dual_node.is_some());
                             edge.right_grandson_dual_node = edge.left_grandson_dual_node.clone();
                         } else {
                             edge.left_dual_node = Some(dual_node_internal_ptr.downgrade());
                             debug_assert!(edge.right_grandson_dual_node.is_some());
                             edge.left_grandson_dual_node = edge.right_grandson_dual_node.clone();
                         }
                     }
-                } else {  // keep other edges
+                } else {
+                    // keep other edges
                     self.updated_boundary.push((is_left, edge_weak.clone()));
                 }
             }
-            drop(dual_node_internal);  // unlock
-            // propagating nodes may be duplicated, but it's easy to check by `propagated_dual_node`
+            drop(dual_node_internal); // unlock
+                                      // propagating nodes may be duplicated, but it's easy to check by `propagated_dual_node`
             for (vertex_weak, grandson_dual_node) in self.propagating_vertices.iter() {
                 let vertex_ptr = vertex_weak.upgrade_force();
                 let mut vertex = vertex_ptr.write(active_timestamp);
                 if vertex.propagated_dual_node.is_none() {
                     vertex.propagated_dual_node = Some(dual_node_internal_ptr.downgrade());
                     vertex.propagated_grandson_dual_node = grandson_dual_node.clone();
                     // add to the sync list
                     if let Some(mirror_unit_weak) = &vertex.mirror_unit {
                         self.sync_requests.push(SyncRequest {
                             mirror_unit_weak: mirror_unit_weak.clone(),
                             vertex_index: vertex.vertex_index,
                             propagated_dual_node: vertex.propagated_dual_node.clone().map(|weak| {
                                 let dual_node_ptr = weak.upgrade_force();
                                 let dual_node = dual_node_ptr.read_recursive();
-                                (dual_node.origin.clone(), dual_node.dual_variable)
+                                (
+                                    dual_node.origin.clone(),
+                                    dual_node.dual_variable,
+                                    dual_node.origin.upgrade_force().get_representative_vertex(),
+                                )
                             }),
                             propagated_grandson_dual_node: vertex.propagated_grandson_dual_node.as_ref().map(|weak| {
                                 let dual_node_ptr = weak.upgrade_force();
                                 let dual_node = dual_node_ptr.read_recursive();
-                                (dual_node.origin.clone(), dual_node.dual_variable)
+                                (
+                                    dual_node.origin.clone(),
+                                    dual_node.dual_variable,
+                                    dual_node.origin.upgrade_force().get_representative_vertex(),
+                                )
                             }),
                         });
                     }
                     let mut count_newly_propagated_edge = 0;
                     for edge_weak in vertex.edges.iter() {
                         let edge_ptr = edge_weak.upgrade_force();
                         let (is_left, newly_propagated_edge) = {
@@ -1540,15 +1907,16 @@
                     }
                     if count_newly_propagated_edge == 0 {
                         lock_write!(dual_node_internal, dual_node_internal_ptr);
                         dual_node_internal.overgrown_stack.push((vertex_ptr.downgrade(), 0));
                     }
                 }
             }
-        } else {  // gracefully update the boundary to ease shrinking
+        } else {
+            // gracefully update the boundary to ease shrinking
             self.clear_edge_dedup();
             {
                 lock_write!(dual_node_internal, dual_node_internal_ptr);
                 while !dual_node_internal.overgrown_stack.is_empty() {
                     let last_index = dual_node_internal.overgrown_stack.len() - 1;
                     let (_, overgrown) = &dual_node_internal.overgrown_stack[last_index];
                     if *overgrown == 0 {
@@ -1569,75 +1937,110 @@
                                 });
                             }
                             for edge_weak in vertex.edges.iter() {
                                 let edge_ptr = edge_weak.upgrade_force();
                                 let mut edge = edge_ptr.write(active_timestamp);
                                 let is_left = vertex_ptr.downgrade() == edge.left;
                                 if self.unit_module_info.is_none() {
-                                    debug_assert!(if is_left {
-                                        edge.left_dual_node == Some(dual_node_internal_ptr.downgrade()) && edge.left_grandson_dual_node.is_some()
-                                    } else {
-                                        edge.right_dual_node == Some(dual_node_internal_ptr.downgrade()) && edge.right_grandson_dual_node.is_some()
-                                    }, "overgrown vertices must be surrounded by the same propagated dual node");
+                                    debug_assert!(
+                                        if is_left {
+                                            edge.left_dual_node == Some(dual_node_internal_ptr.downgrade())
+                                                && edge.left_grandson_dual_node.is_some()
+                                        } else {
+                                            edge.right_dual_node == Some(dual_node_internal_ptr.downgrade())
+                                                && edge.right_grandson_dual_node.is_some()
+                                        },
+                                        "overgrown vertices must be surrounded by the same propagated dual node"
+                                    );
                                 }
                                 if is_left {
                                     edge.left_dual_node = None;
                                     edge.left_grandson_dual_node = None;
                                 } else {
                                     edge.right_dual_node = None;
                                     edge.right_grandson_dual_node = None;
                                 }
-                                if (if !is_left { edge.dedup_timestamp.0 } else { edge.dedup_timestamp.1 }) != self.edge_dedup_timestamp {
-                                    if !is_left { edge.dedup_timestamp.0 = self.edge_dedup_timestamp; } else { edge.dedup_timestamp.1 = self.edge_dedup_timestamp; }
-                                    self.updated_boundary.push((!is_left, edge_weak.clone()));  // boundary has the opposite end
+                                if (if !is_left {
+                                    edge.dedup_timestamp.0
+                                } else {
+                                    edge.dedup_timestamp.1
+                                }) != self.edge_dedup_timestamp
+                                {
+                                    if !is_left {
+                                        edge.dedup_timestamp.0 = self.edge_dedup_timestamp;
+                                    } else {
+                                        edge.dedup_timestamp.1 = self.edge_dedup_timestamp;
+                                    }
+                                    self.updated_boundary.push((!is_left, edge_weak.clone()));
+                                    // boundary has the opposite end
                                 }
                             }
                         } else {
                             // this happens when sync request already vacate the vertex, thus no need to add edges to the boundary
                             // in fact, this will cause duplicate boundary edges if not skipped, leading to exceptions when creating blossoms
                             debug_assert!(self.unit_module_info.is_some(), "serial module itself cannot happen");
                         }
                     } else {
-                        break  // found non-negative overgrown in the stack
+                        break; // found non-negative overgrown in the stack
                     }
                 }
             }
             let dual_node_internal = dual_node_internal_ptr.read_recursive();
             for (is_left, edge_weak) in dual_node_internal.boundary.iter() {
                 let edge_ptr = edge_weak.upgrade_force();
                 let is_left = *is_left;
                 let mut edge = edge_ptr.write(active_timestamp);
-                let this_growth = if is_left {
-                    edge.left_growth
-                } else {
-                    edge.right_growth
-                };
+                let this_growth = if is_left { edge.left_growth } else { edge.right_growth };
                 if this_growth == 0 {
                     // need to shrink before this vertex
                     let this_vertex_ptr = if is_left {
                         edge.left.upgrade_force()
                     } else {
                         edge.right.upgrade_force()
                     };
                     // to avoid already occupied node being propagated
                     let this_vertex = this_vertex_ptr.read_recursive(active_timestamp);
-                    if this_vertex.is_defect {  // never shrink from the syndrome itself
-                        if (if is_left { edge.dedup_timestamp.0 } else { edge.dedup_timestamp.1 }) != self.edge_dedup_timestamp {
-                            if is_left { edge.dedup_timestamp.0 = self.edge_dedup_timestamp; } else { edge.dedup_timestamp.1 = self.edge_dedup_timestamp; }
+                    if this_vertex.is_defect {
+                        // never shrink from the syndrome itself
+                        if (if is_left {
+                            edge.dedup_timestamp.0
+                        } else {
+                            edge.dedup_timestamp.1
+                        }) != self.edge_dedup_timestamp
+                        {
+                            if is_left {
+                                edge.dedup_timestamp.0 = self.edge_dedup_timestamp;
+                            } else {
+                                edge.dedup_timestamp.1 = self.edge_dedup_timestamp;
+                            }
                             self.updated_boundary.push((is_left, edge_weak.clone()));
                         }
                     } else {
-                        if edge.weight > 0 && self.unit_module_info.is_none() {  // do not check for 0-weight edges
-                            debug_assert!(this_vertex.propagated_dual_node.is_some(), "unexpected shrink into an empty vertex");
+                        if edge.weight > 0 && self.unit_module_info.is_none() {
+                            // do not check for 0-weight edges
+                            debug_assert!(
+                                this_vertex.propagated_dual_node.is_some(),
+                                "unexpected shrink into an empty vertex"
+                            );
                         }
                         self.propagating_vertices.push((this_vertex_ptr.downgrade(), None));
                     }
-                } else {  // keep other edges
-                    if (if is_left { edge.dedup_timestamp.0 } else { edge.dedup_timestamp.1 }) != self.edge_dedup_timestamp {
-                        if is_left { edge.dedup_timestamp.0 = self.edge_dedup_timestamp; } else { edge.dedup_timestamp.1 = self.edge_dedup_timestamp; }
+                } else {
+                    // keep other edges
+                    if (if is_left {
+                        edge.dedup_timestamp.0
+                    } else {
+                        edge.dedup_timestamp.1
+                    }) != self.edge_dedup_timestamp
+                    {
+                        if is_left {
+                            edge.dedup_timestamp.0 = self.edge_dedup_timestamp;
+                        } else {
+                            edge.dedup_timestamp.1 = self.edge_dedup_timestamp;
+                        }
                         self.updated_boundary.push((is_left, edge_weak.clone()));
                     }
                 }
             }
             // propagating nodes may be duplicated, but it's easy to check by `propagated_dual_node`
             for (vertex_weak, _) in self.propagating_vertices.iter() {
                 let vertex_ptr = vertex_weak.upgrade_force();
@@ -1655,43 +2058,69 @@
                         });
                     }
                     for edge_weak in vertex.edges.iter() {
                         let edge_ptr = edge_weak.upgrade_force();
                         let (is_left, newly_propagated_edge) = {
                             let edge = edge_ptr.read_recursive(active_timestamp);
                             let is_left = vertex_ptr.downgrade() == edge.left;
-                            debug_assert!(if is_left { edge.right != vertex_ptr.downgrade() } else { edge.right == vertex_ptr.downgrade() });
+                            debug_assert!(if is_left {
+                                edge.right != vertex_ptr.downgrade()
+                            } else {
+                                edge.right == vertex_ptr.downgrade()
+                            });
                             // fully grown edge is where to shrink
                             let newly_propagated_edge = edge.left_dual_node == Some(dual_node_internal_ptr.downgrade())
                                 && edge.right_dual_node == Some(dual_node_internal_ptr.downgrade())
                                 && edge.left_growth + edge.right_growth >= edge.weight;
-                            debug_assert!({
-                                newly_propagated_edge || {
-                                    if is_left { edge.left_growth == 0  } else { edge.right_growth == 0 }
-                                }
-                            }, "an edge must be either newly propagated or to be removed");
+                            debug_assert!(
+                                {
+                                    newly_propagated_edge || {
+                                        if is_left {
+                                            edge.left_growth == 0
+                                        } else {
+                                            edge.right_growth == 0
+                                        }
+                                    }
+                                },
+                                "an edge must be either newly propagated or to be removed"
+                            );
                             (is_left, newly_propagated_edge)
                         };
                         if newly_propagated_edge {
                             let mut edge = edge_ptr.write(active_timestamp);
-                            if (if !is_left { edge.dedup_timestamp.0 } else { edge.dedup_timestamp.1 }) != self.edge_dedup_timestamp {
-                                if !is_left { edge.dedup_timestamp.0 = self.edge_dedup_timestamp; } else { edge.dedup_timestamp.1 = self.edge_dedup_timestamp; }
+                            if (if !is_left {
+                                edge.dedup_timestamp.0
+                            } else {
+                                edge.dedup_timestamp.1
+                            }) != self.edge_dedup_timestamp
+                            {
+                                if !is_left {
+                                    edge.dedup_timestamp.0 = self.edge_dedup_timestamp;
+                                } else {
+                                    edge.dedup_timestamp.1 = self.edge_dedup_timestamp;
+                                }
                                 self.updated_boundary.push((!is_left, edge_weak.clone()));
-                            }  // otherwise it's duplicate and should not be added to the boundary list
+                            } // otherwise it's duplicate and should not be added to the boundary list
                             if edge.weight == 0 {
                                 newly_propagated_edge_has_zero_weight = true;
                             }
                             if is_left {
                                 debug_assert!(edge.right_dual_node.is_some(), "unexpected shrinking to empty edge");
-                                debug_assert!(edge.right_dual_node.as_ref().unwrap() == &dual_node_internal_ptr.downgrade(), "shrinking edge should be same tree node");
+                                debug_assert!(
+                                    edge.right_dual_node.as_ref().unwrap() == &dual_node_internal_ptr.downgrade(),
+                                    "shrinking edge should be same tree node"
+                                );
                                 edge.left_dual_node = None;
                                 edge.left_grandson_dual_node = None;
                             } else {
                                 debug_assert!(edge.left_dual_node.is_some(), "unexpected shrinking to empty edge");
-                                debug_assert!(edge.left_dual_node.as_ref().unwrap() == &dual_node_internal_ptr.downgrade(), "shrinking edge should be same tree node");
+                                debug_assert!(
+                                    edge.left_dual_node.as_ref().unwrap() == &dual_node_internal_ptr.downgrade(),
+                                    "shrinking edge should be same tree node"
+                                );
                                 edge.right_dual_node = None;
                                 edge.right_grandson_dual_node = None;
                             };
                         } else {
                             let mut edge = edge_ptr.write(active_timestamp);
                             if is_left {
                                 edge.left_dual_node = None;
@@ -1706,277 +2135,446 @@
             }
         }
         // update the boundary
         lock_write!(dual_node_internal, dual_node_internal_ptr);
         std::mem::swap(&mut self.updated_boundary, &mut dual_node_internal.boundary);
         // println!("{} boundary: {:?}", tree_node.boundary.len(), tree_node.boundary);
         if self.unit_module_info.is_none() {
-            debug_assert!(!dual_node_internal.boundary.is_empty(), "the boundary of a dual cluster is never empty");
+            debug_assert!(
+                !dual_node_internal.boundary.is_empty(),
+                "the boundary of a dual cluster is never empty"
+            );
         }
         newly_propagated_edge_has_zero_weight
     }
 
     /// adjust the boundary of each dual node to fit into the need of growing (`length` > 0) or shrinking (`length` < 0)
     pub fn prepare_dual_node_growth(&mut self, dual_node_ptr: &DualNodePtr, is_grow: bool) {
         let mut need_another = self.prepare_dual_node_growth_single(dual_node_ptr, is_grow);
-        while need_another {  // when there are 0 weight edges, one may need to run multiple iterations to get it prepared in a proper state
+        while need_another {
+            // when there are 0 weight edges, one may need to run multiple iterations to get it prepared in a proper state
             need_another = self.prepare_dual_node_growth_single(dual_node_ptr, is_grow);
         }
     }
-
 }
 
 #[cfg(test)]
 mod tests {
-    use super::*;
     use super::super::example_codes::*;
     use super::super::primal_module_serial::tests::*;
+    use super::*;
 
     #[allow(dead_code)]
     fn debug_print_dual_node(dual_module: &DualModuleSerial, dual_node_ptr: &DualNodePtr) {
         println!("boundary:");
         let dual_node_internal_ptr = dual_module.get_dual_node_internal_ptr(dual_node_ptr);
         let dual_node_internal = dual_node_internal_ptr.read_recursive();
         for (is_left, edge_weak) in dual_node_internal.boundary.iter() {
             let edge_ptr = edge_weak.upgrade_force();
             let edge = edge_ptr.read_recursive_force();
             println!("    {} {:?}", if *is_left { " left" } else { "right" }, edge);
         }
     }
 
     #[test]
-    fn dual_module_serial_basics() {  // cargo test dual_module_serial_basics -- --nocapture
+    fn dual_module_serial_basics() {
+        // cargo test dual_module_serial_basics -- --nocapture
         let visualize_filename = format!("dual_module_serial_basics.json");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(7, 0.1, half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // try to work on a simple syndrome
         code.vertices[19].is_defect = true;
         code.vertices[25].is_defect = true;
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
-        visualizer.snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // create dual nodes and grow them by half length
         let dual_node_19_ptr = interface_ptr.read_recursive().nodes[0].clone().unwrap();
         let dual_node_25_ptr = interface_ptr.read_recursive().nodes[1].clone().unwrap();
         dual_module.grow_dual_node(&dual_node_19_ptr, half_weight);
         dual_module.grow_dual_node(&dual_node_25_ptr, half_weight);
-        visualizer.snapshot_combined(format!("grow to 0.5"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow to 0.5"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         dual_module.grow_dual_node(&dual_node_19_ptr, half_weight);
         dual_module.grow_dual_node(&dual_node_25_ptr, half_weight);
-        visualizer.snapshot_combined(format!("grow to 1"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow to 1"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         dual_module.grow_dual_node(&dual_node_19_ptr, half_weight);
         dual_module.grow_dual_node(&dual_node_25_ptr, half_weight);
-        visualizer.snapshot_combined(format!("grow to 1.5"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow to 1.5"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         dual_module.grow_dual_node(&dual_node_19_ptr, -half_weight);
         dual_module.grow_dual_node(&dual_node_25_ptr, -half_weight);
-        visualizer.snapshot_combined(format!("shrink to 1"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("shrink to 1"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         dual_module.grow_dual_node(&dual_node_19_ptr, -half_weight);
         dual_module.grow_dual_node(&dual_node_25_ptr, -half_weight);
-        visualizer.snapshot_combined(format!("shrink to 0.5"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("shrink to 0.5"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         dual_module.grow_dual_node(&dual_node_19_ptr, -half_weight);
         dual_module.grow_dual_node(&dual_node_25_ptr, -half_weight);
-        visualizer.snapshot_combined(format!("shrink to 0"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("shrink to 0"), vec![&interface_ptr, &dual_module])
+            .unwrap();
     }
 
     #[test]
-    fn dual_module_serial_blossom_basics() {  // cargo test dual_module_serial_blossom_basics -- --nocapture
+    fn dual_module_serial_blossom_basics() {
+        // cargo test dual_module_serial_blossom_basics -- --nocapture
         let visualize_filename = format!("dual_module_serial_blossom_basics.json");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(7, 0.1, half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // try to work on a simple syndrome
         code.vertices[19].is_defect = true;
         code.vertices[26].is_defect = true;
         code.vertices[35].is_defect = true;
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
-        visualizer.snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // create dual nodes and grow them by half length
         let dual_node_19_ptr = interface_ptr.read_recursive().nodes[0].clone().unwrap();
         let dual_node_26_ptr = interface_ptr.read_recursive().nodes[1].clone().unwrap();
         let dual_node_35_ptr = interface_ptr.read_recursive().nodes[2].clone().unwrap();
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 6 * half_weight);
-        visualizer.snapshot_combined(format!("before create blossom"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("before create blossom"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         let nodes_circle = vec![dual_node_19_ptr.clone(), dual_node_26_ptr.clone(), dual_node_35_ptr.clone()];
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         let dual_node_blossom = interface_ptr.create_blossom(nodes_circle, vec![], &mut dual_module);
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 7 * half_weight);
-        visualizer.snapshot_combined(format!("blossom grow half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("blossom grow half weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 8 * half_weight);
-        visualizer.snapshot_combined(format!("blossom grow half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("blossom grow half weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 9 * half_weight);
-        visualizer.snapshot_combined(format!("blossom grow half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("blossom grow half weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         interface_ptr.set_grow_state(&dual_node_blossom, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 8 * half_weight);
-        visualizer.snapshot_combined(format!("blossom shrink half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("blossom shrink half weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 6 * half_weight);
-        visualizer.snapshot_combined(format!("blossom shrink weight"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("blossom shrink weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         interface_ptr.expand_blossom(dual_node_blossom, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_19_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_35_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 3 * half_weight);
-        visualizer.snapshot_combined(format!("individual shrink half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("individual shrink half weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
     }
 
     #[test]
-    fn dual_module_serial_stop_reason_1() {  // cargo test dual_module_serial_stop_reason_1 -- --nocapture
+    fn dual_module_serial_stop_reason_1() {
+        // cargo test dual_module_serial_stop_reason_1 -- --nocapture
         let visualize_filename = format!("dual_module_serial_stop_reason_1.json");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(7, 0.1, half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // try to work on a simple syndrome
         code.vertices[19].is_defect = true;
         code.vertices[25].is_defect = true;
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
-        visualizer.snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // create dual nodes and grow them by half length
         let dual_node_19_ptr = interface_ptr.read_recursive().nodes[0].clone().unwrap();
         let dual_node_25_ptr = interface_ptr.read_recursive().nodes[1].clone().unwrap();
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 4 * half_weight);
-        visualizer.snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 6 * half_weight);
-        visualizer.snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().is_conflicting(&dual_node_19_ptr, &dual_node_25_ptr), "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length
+                .peek()
+                .unwrap()
+                .is_conflicting(&dual_node_19_ptr, &dual_node_25_ptr),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
     }
 
     #[test]
-    fn dual_module_serial_stop_reason_2() {  // cargo test dual_module_serial_stop_reason_2 -- --nocapture
+    fn dual_module_serial_stop_reason_2() {
+        // cargo test dual_module_serial_stop_reason_2 -- --nocapture
         let visualize_filename = format!("dual_module_serial_stop_reason_2.json");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(7, 0.1, half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // try to work on a simple syndrome
         code.vertices[18].is_defect = true;
         code.vertices[26].is_defect = true;
         code.vertices[34].is_defect = true;
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
-        visualizer.snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // create dual nodes and grow them by half length
         let dual_node_18_ptr = interface_ptr.read_recursive().nodes[0].clone().unwrap();
         let dual_node_26_ptr = interface_ptr.read_recursive().nodes[1].clone().unwrap();
         let dual_node_34_ptr = interface_ptr.read_recursive().nodes[2].clone().unwrap();
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 3 * half_weight);
-        visualizer.snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().is_conflicting(&dual_node_18_ptr, &dual_node_26_ptr)
-            || group_max_update_length.peek().unwrap().is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr), "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length
+                .peek()
+                .unwrap()
+                .is_conflicting(&dual_node_18_ptr, &dual_node_26_ptr)
+                || group_max_update_length
+                    .peek()
+                    .unwrap()
+                    .is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // first match 18 and 26
         interface_ptr.set_grow_state(&dual_node_18_ptr, DualNodeGrowState::Stay, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Stay, &mut dual_module);
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr)
-            , "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length
+                .peek()
+                .unwrap()
+                .is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // 34 touches 26, so it will grow the tree by absorbing 18 and 26
         interface_ptr.set_grow_state(&dual_node_18_ptr, DualNodeGrowState::Grow, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 4 * half_weight);
-        visualizer.snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().is_conflicting(&dual_node_18_ptr, &dual_node_34_ptr), "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length
+                .peek()
+                .unwrap()
+                .is_conflicting(&dual_node_18_ptr, &dual_node_34_ptr),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // for a blossom because 18 and 34 come from the same alternating tree
-        let dual_node_blossom = interface_ptr.create_blossom(vec![dual_node_18_ptr.clone(), dual_node_26_ptr.clone(), dual_node_34_ptr.clone()], vec![], &mut dual_module);
+        let dual_node_blossom = interface_ptr.create_blossom(
+            vec![dual_node_18_ptr.clone(), dual_node_26_ptr.clone(), dual_node_34_ptr.clone()],
+            vec![],
+            &mut dual_module,
+        );
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 6 * half_weight);
-        visualizer.snapshot_combined(format!("grow blossom"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow blossom"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 8 * half_weight);
-        visualizer.snapshot_combined(format!("grow blossom"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow blossom"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 23))
-            || group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 39))
-            , "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 23))
+                || group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 39)),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // blossom touches virtual boundary, so it's matched
         interface_ptr.set_grow_state(&dual_node_blossom, DualNodeGrowState::Stay, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.is_empty(), "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length.is_empty(),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // also test the reverse procedure: shrinking and expanding blossom
         interface_ptr.set_grow_state(&dual_node_blossom, DualNodeGrowState::Shrink, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 6 * half_weight);
-        visualizer.snapshot_combined(format!("shrink blossom"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("shrink blossom"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // before expand
         interface_ptr.set_grow_state(&dual_node_blossom, DualNodeGrowState::Shrink, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 4 * half_weight);
-        visualizer.snapshot_combined(format!("shrink blossom"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("shrink blossom"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // cannot shrink anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap() == &MaxUpdateLength::BlossomNeedExpand(dual_node_blossom.clone())
-            , "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length.peek().unwrap() == &MaxUpdateLength::BlossomNeedExpand(dual_node_blossom.clone()),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // expand blossom
         interface_ptr.expand_blossom(dual_node_blossom, &mut dual_module);
         // regain access to underlying nodes
         interface_ptr.set_grow_state(&dual_node_18_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Grow, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_34_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 2 * half_weight);
-        visualizer.snapshot_combined(format!("shrink"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("shrink"), vec![&interface_ptr, &dual_module])
+            .unwrap();
     }
 
     /// this test helps observe bugs of fast clear, by removing snapshot: snapshot will do the clear automatically
     #[test]
-    fn dual_module_serial_fast_clear_1() {  // cargo test dual_module_serial_fast_clear_1 -- --nocapture
+    fn dual_module_serial_fast_clear_1() {
+        // cargo test dual_module_serial_fast_clear_1 -- --nocapture
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(7, 0.1, half_weight);
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // try to work on a simple syndrome
         code.vertices[18].is_defect = true;
@@ -1985,162 +2583,272 @@
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
         // create dual nodes and grow them by half length
         let dual_node_18_ptr = interface_ptr.read_recursive().nodes[0].clone().unwrap();
         let dual_node_26_ptr = interface_ptr.read_recursive().nodes[1].clone().unwrap();
         let dual_node_34_ptr = interface_ptr.read_recursive().nodes[2].clone().unwrap();
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 3 * half_weight);
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().is_conflicting(&dual_node_18_ptr, &dual_node_26_ptr)
-            || group_max_update_length.peek().unwrap().is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr), "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length
+                .peek()
+                .unwrap()
+                .is_conflicting(&dual_node_18_ptr, &dual_node_26_ptr)
+                || group_max_update_length
+                    .peek()
+                    .unwrap()
+                    .is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // first match 18 and 26
         interface_ptr.set_grow_state(&dual_node_18_ptr, DualNodeGrowState::Stay, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Stay, &mut dual_module);
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr)
-            , "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length
+                .peek()
+                .unwrap()
+                .is_conflicting(&dual_node_26_ptr, &dual_node_34_ptr),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // 34 touches 26, so it will grow the tree by absorbing 18 and 26
         interface_ptr.set_grow_state(&dual_node_18_ptr, DualNodeGrowState::Grow, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 4 * half_weight);
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().is_conflicting(&dual_node_18_ptr, &dual_node_34_ptr), "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length
+                .peek()
+                .unwrap()
+                .is_conflicting(&dual_node_18_ptr, &dual_node_34_ptr),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // for a blossom because 18 and 34 come from the same alternating tree
-        let dual_node_blossom = interface_ptr.create_blossom(vec![dual_node_18_ptr.clone(), dual_node_26_ptr.clone(), dual_node_34_ptr.clone()], vec![], &mut dual_module);
+        let dual_node_blossom = interface_ptr.create_blossom(
+            vec![dual_node_18_ptr.clone(), dual_node_26_ptr.clone(), dual_node_34_ptr.clone()],
+            vec![],
+            &mut dual_module,
+        );
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         // grow the maximum
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         // cannot grow anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 23))
-            || group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 39))
-            , "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 23))
+                || group_max_update_length.peek().unwrap().get_touching_virtual() == Some((dual_node_blossom.clone(), 39)),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // blossom touches virtual boundary, so it's matched
         interface_ptr.set_grow_state(&dual_node_blossom, DualNodeGrowState::Stay, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.is_empty(), "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length.is_empty(),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // also test the reverse procedure: shrinking and expanding blossom
         interface_ptr.set_grow_state(&dual_node_blossom, DualNodeGrowState::Shrink, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         // before expand
         interface_ptr.set_grow_state(&dual_node_blossom, DualNodeGrowState::Shrink, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         // cannot shrink anymore, find out the reason
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert!(group_max_update_length.peek().unwrap() == &MaxUpdateLength::BlossomNeedExpand(dual_node_blossom.clone())
-            , "unexpected: {:?}", group_max_update_length);
+        assert!(
+            group_max_update_length.peek().unwrap() == &MaxUpdateLength::BlossomNeedExpand(dual_node_blossom.clone()),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         // expand blossom
         interface_ptr.expand_blossom(dual_node_blossom, &mut dual_module);
         // regain access to underlying nodes
         interface_ptr.set_grow_state(&dual_node_18_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_26_ptr, DualNodeGrowState::Grow, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_34_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         let group_max_update_length = dual_module.compute_maximum_update_length();
-        assert_eq!(group_max_update_length.get_none_zero_growth(), Some(2 * half_weight), "unexpected: {:?}", group_max_update_length);
+        assert_eq!(
+            group_max_update_length.get_none_zero_growth(),
+            Some(2 * half_weight),
+            "unexpected: {:?}",
+            group_max_update_length
+        );
         interface_ptr.grow(2 * half_weight, &mut dual_module);
         assert_eq!(interface_ptr.sum_dual_variables(), 2 * half_weight);
     }
 
     #[test]
-    fn dual_module_grow_iterative_1() {  // cargo test dual_module_grow_iterative_1 -- --nocapture
+    fn dual_module_grow_iterative_1() {
+        // cargo test dual_module_grow_iterative_1 -- --nocapture
         let visualize_filename = format!("dual_module_grow_iterative_1.json");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(11, 0.1, half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // try to work on a simple syndrome
         code.vertices[39].is_defect = true;
         code.vertices[65].is_defect = true;
         code.vertices[87].is_defect = true;
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
-        visualizer.snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // create dual nodes and grow them by half length
         interface_ptr.grow_iterative(4 * half_weight, &mut dual_module);
-        visualizer.snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         assert_eq!(interface_ptr.sum_dual_variables(), 3 * 4 * half_weight);
         let dual_node_39_ptr = interface_ptr.read_recursive().nodes[0].clone().unwrap();
         let dual_node_65_ptr = interface_ptr.read_recursive().nodes[1].clone().unwrap();
         let dual_node_87_ptr = interface_ptr.read_recursive().nodes[2].clone().unwrap();
         interface_ptr.set_grow_state(&dual_node_39_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_65_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.set_grow_state(&dual_node_87_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         interface_ptr.grow_iterative(4 * half_weight, &mut dual_module);
-        visualizer.snapshot_combined(format!("shrink"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("shrink"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         assert_eq!(interface_ptr.sum_dual_variables(), 0);
     }
 
     #[test]
-    fn dual_module_debug_1() {  // cargo test dual_module_debug_1 -- --nocapture
+    fn dual_module_debug_1() {
+        // cargo test dual_module_debug_1 -- --nocapture
         let visualize_filename = format!("dual_module_debug_1.json");
-        let defect_vertices = vec![6, 7, 17, 18, 21, 27, 28, 42, 43, 49, 51, 52, 54, 55, 61, 63, 65, 67, 76, 78, 80, 86, 103, 110, 113, 114, 116, 122, 125, 127];
+        let defect_vertices = vec![
+            6, 7, 17, 18, 21, 27, 28, 42, 43, 49, 51, 52, 54, 55, 61, 63, 65, 67, 76, 78, 80, 86, 103, 110, 113, 114, 116,
+            122, 125, 127,
+        ];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 23);
     }
 
     #[test]
-    fn dual_module_debug_2() {  // cargo test dual_module_debug_2 -- --nocapture
+    fn dual_module_debug_2() {
+        // cargo test dual_module_debug_2 -- --nocapture
         let visualize_filename = format!("dual_module_debug_2.json");
-        let defect_vertices = vec![5, 12, 16, 19, 21, 38, 42, 43, 49, 56, 61, 67, 72, 73, 74, 75, 76, 88, 89, 92, 93, 99, 105, 112, 117, 120, 124, 129];
+        let defect_vertices = vec![
+            5, 12, 16, 19, 21, 38, 42, 43, 49, 56, 61, 67, 72, 73, 74, 75, 76, 88, 89, 92, 93, 99, 105, 112, 117, 120, 124,
+            129,
+        ];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 22);
     }
 
     #[test]
-    fn dual_module_erasure_1() {  // cargo test dual_module_erasure_1 -- --nocapture
+    fn dual_module_erasure_1() {
+        // cargo test dual_module_erasure_1 -- --nocapture
         let visualize_filename = format!("dual_module_erasure_1.json");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(11, 0.1, half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // try to work on a simple syndrome
         code.vertices[64].is_defect = true;
         code.set_erasures(&vec![110, 78, 57, 142, 152, 163, 164]);
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
-        visualizer.snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("syndrome"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // create dual nodes and grow them by half length
         for _ in 0..3 {
             interface_ptr.grow_iterative(2 * half_weight, &mut dual_module);
-            visualizer.snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module])
+                .unwrap();
         }
         // set them to shrink
         let dual_node_ptr = interface_ptr.read_recursive().nodes[0].clone().unwrap();
         interface_ptr.set_grow_state(&dual_node_ptr, DualNodeGrowState::Shrink, &mut dual_module);
         // shrink them back, to make sure the operation is reversible
         for _ in 0..3 {
             interface_ptr.grow_iterative(2 * half_weight, &mut dual_module);
-            visualizer.snapshot_combined(format!("shrink"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("shrink"), vec![&interface_ptr, &dual_module])
+                .unwrap();
         }
         // cancel the erasures and grow the dual module in normal case, this should automatically clear the erasures
         dual_module.clear();
-         // no erasures this time, to test if the module recovers correctly
-        let interface_ptr = DualModuleInterfacePtr::new_load(&SyndromePattern::new_vertices(code.get_syndrome().defect_vertices), &mut dual_module);
-        visualizer.snapshot_combined(format!("after clear"), vec![&interface_ptr, &dual_module]).unwrap();
+        // no erasures this time, to test if the module recovers correctly
+        let interface_ptr = DualModuleInterfacePtr::new_load(
+            &SyndromePattern::new_vertices(code.get_syndrome().defect_vertices),
+            &mut dual_module,
+        );
+        visualizer
+            .snapshot_combined(format!("after clear"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         for _ in 0..3 {
             interface_ptr.grow_iterative(2 * half_weight, &mut dual_module);
-            visualizer.snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("grow"), vec![&interface_ptr, &dual_module])
+                .unwrap();
         }
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/src/example_codes.rs` & `fusion_blossom-0.2.5/src/example_codes.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 //! Example Decoding
-//! 
+//!
 //! This module contains several abstract decoding graph and it's randomized simulator utilities.
-//! This helps to debug, but it doesn't corresponds to real error model, nor it's capable of simulating circuit-level noise model.
-//! For complex error model and simulator functionality, please see <https://github.com/yuewuo/QEC-Playground>
-//! 
-//! Note that these examples are not optimized for cache coherency for simplicity.
-//! To maximize code efficiency, user should design how to group vertices such that memory coherency is preserved for arbitrary large code distance.
-//! 
+//! This helps to debug, but it doesn't corresponds to real noise model, nor it's capable of simulating circuit-level noise model.
+//! For complex noise model and simulator functionality, please see <https://github.com/yuewuo/QEC-Playground>
+//!
+//! Note that these examples are not optimized for cache for simplicity.
+//! To maximize code efficiency, user should design how to group vertices such that memory speed is constant for arbitrary large code distance.
+//!
 
-use super::visualize::*;
+use super::pointers::*;
 use super::util::*;
-use std::collections::HashMap;
-use crate::serde_json;
-use crate::rand_xoshiro::rand_core::SeedableRng;
+use super::visualize::*;
 use crate::derivative::Derivative;
-use std::fs::File;
-use std::io::{self, BufRead};
+use crate::rand_xoshiro::rand_core::SeedableRng;
 use crate::rayon::prelude::*;
-use super::pointers::*;
-#[cfg(feature="python_binding")]
+use crate::serde_json;
+#[cfg(feature = "python_binding")]
 use pyo3::prelude::*;
-
+use std::collections::HashMap;
+use std::fs::File;
+use std::io::{self, BufRead};
 
 /// Vertex corresponds to a stabilizer measurement bit
 #[derive(Derivative, Clone)]
 #[derivative(Debug)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct CodeVertex {
@@ -42,15 +41,17 @@
     pub is_defect: bool,
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl CodeVertex {
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 /// Edge flips the measurement result of two vertices
 #[derive(Derivative, Clone)]
 #[derivative(Debug)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
@@ -82,32 +83,35 @@
             p: 0.,
             pe: 0.,
             half_weight: 0,
             is_erasure: false,
         }
     }
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 /// default function for computing (pre-scaled) weight from probability
 #[cfg_attr(feature = "python_binding", pyfunction)]
 pub fn weight_of_p(p: f64) -> f64 {
     assert!((0. ..=0.5).contains(&p), "p must be a reasonable value between 0 and 50%");
     ((1. - p) / p).ln()
 }
 
 pub trait ExampleCode {
-
     /// get mutable references to vertices and edges
     fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>);
     fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>);
 
     /// get the number of vertices
-    fn vertex_num(&self) -> VertexNum { self.immutable_vertices_edges().0.len() as VertexNum }
+    fn vertex_num(&self) -> VertexNum {
+        self.immutable_vertices_edges().0.len() as VertexNum
+    }
 
     /// generic method that automatically computes integer weights from probabilities,
     /// scales such that the maximum integer weight is 10000 and the minimum is 1
     fn compute_weights(&mut self, max_half_weight: Weight) {
         let (_vertices, edges) = self.vertices_edges();
         let mut max_weight = 0.;
         for edge in edges.iter() {
@@ -117,15 +121,15 @@
             }
         }
         assert!(max_weight > 0., "max weight is not expected to be 0.");
         // scale all weights but set the smallest to 1
         for edge in edges.iter_mut() {
             let weight = weight_of_p(edge.p);
             let half_weight: Weight = ((max_half_weight as f64) * weight / max_weight).round() as Weight;
-            edge.half_weight = if half_weight == 0 { 1 } else { half_weight };  // weight is required to be even
+            edge.half_weight = if half_weight == 0 { 1 } else { half_weight }; // weight is required to be even
         }
     }
 
     /// sanity check to avoid duplicate edges that are hard to debug
     fn sanity_check(&self) -> Result<(), String> {
         let (vertices, edges) = self.immutable_vertices_edges();
         // check the graph is reasonable
@@ -135,15 +139,18 @@
         // check duplicated edges
         let mut existing_edges = HashMap::<(VertexIndex, VertexIndex), EdgeIndex>::with_capacity(edges.len() * 2);
         for (edge_idx, edge) in edges.iter().enumerate() {
             let (v1, v2) = edge.vertices;
             let unique_edge = if v1 < v2 { (v1, v2) } else { (v2, v1) };
             if existing_edges.contains_key(&unique_edge) {
                 let previous_idx = existing_edges[&unique_edge];
-                return Err(format!("duplicate edge {} and {} with incident vertices {} and {}", previous_idx, edge_idx, v1, v2));
+                return Err(format!(
+                    "duplicate edge {} and {} with incident vertices {} and {}",
+                    previous_idx, edge_idx, v1, v2
+                ));
             }
             existing_edges.insert(unique_edge, edge_idx as EdgeIndex);
         }
         // check duplicated referenced edge from each vertex
         for (vertex_idx, vertex) in vertices.iter().enumerate() {
             let mut existing_edges = HashMap::<EdgeIndex, ()>::new();
             if vertex.neighbor_edges.is_empty() {
@@ -172,14 +179,15 @@
         let (_vertices, edges) = self.vertices_edges();
         for edge in edges.iter_mut() {
             edge.pe = pe;
         }
     }
 
     /// automatically create vertices given edges
+    #[allow(clippy::unnecessary_cast)]
     fn fill_vertices(&mut self, vertex_num: VertexNum) {
         let (vertices, edges) = self.vertices_edges();
         vertices.clear();
         vertices.reserve(vertex_num as usize);
         for _ in 0..vertex_num {
             vertices.push(CodeVertex {
                 position: VisualizePosition::new(0., 0., 0.),
@@ -223,28 +231,30 @@
         SolverInitializer {
             vertex_num,
             weighted_edges,
             virtual_vertices,
         }
     }
 
-    /// set defect vertices (non-trivial measurement result in case of single round of measurement, 
+    /// set defect vertices (non-trivial measurement result in case of single round of measurement,
     /// or different result from the previous round in case of multiple rounds of measurement)
+    #[allow(clippy::unnecessary_cast)]
     fn set_defect_vertices(&mut self, defect_vertices: &[VertexIndex]) {
         let (vertices, _edges) = self.vertices_edges();
         for vertex in vertices.iter_mut() {
             vertex.is_defect = false;
         }
         for vertex_idx in defect_vertices.iter() {
             let vertex = &mut vertices[*vertex_idx as usize];
             vertex.is_defect = true;
         }
     }
 
     /// set erasure edges
+    #[allow(clippy::unnecessary_cast)]
     fn set_erasures(&mut self, erasures: &[EdgeIndex]) {
         let (_vertices, edges) = self.vertices_edges();
         for edge in edges.iter_mut() {
             edge.is_erasure = false;
         }
         for edge_idx in erasures.iter() {
             let edge = &mut edges[*edge_idx as usize];
@@ -284,24 +294,25 @@
 
     /// get current syndrome
     fn get_syndrome(&self) -> SyndromePattern {
         SyndromePattern::new(self.get_defect_vertices(), self.get_erasures())
     }
 
     /// generate random errors based on the edge probabilities and a seed for pseudo number generator
+    #[allow(clippy::unnecessary_cast)]
     fn generate_random_errors(&mut self, seed: u64) -> SyndromePattern {
         let mut rng = DeterministicRng::seed_from_u64(seed);
         let (vertices, edges) = self.vertices_edges();
         for vertex in vertices.iter_mut() {
             vertex.is_defect = false;
         }
         for edge in edges.iter_mut() {
             let p = if rng.next_f64() < edge.pe {
                 edge.is_erasure = true;
-                0.5  // when erasure happens, there are 50% chance of error
+                0.5 // when erasure happens, there are 50% chance of error
             } else {
                 edge.is_erasure = false;
                 edge.p
             };
             if rng.next_f64() < p {
                 let (v1, v2) = edge.vertices;
                 let vertex_1 = &mut vertices[v1 as usize];
@@ -313,95 +324,175 @@
                     vertex_2.is_defect = !vertex_2.is_defect;
                 }
             }
         }
         self.get_syndrome()
     }
 
+    #[allow(clippy::unnecessary_cast)]
+    fn generate_errors(&mut self, edge_indices: &[EdgeIndex]) -> SyndromePattern {
+        let (vertices, edges) = self.vertices_edges();
+        for &edge_index in edge_indices {
+            let edge = &mut edges.get_mut(edge_index as usize).unwrap();
+            let (v1, v2) = edge.vertices;
+            let vertex_1 = &mut vertices[v1 as usize];
+            if !vertex_1.is_virtual {
+                vertex_1.is_defect = !vertex_1.is_defect;
+            }
+            let vertex_2 = &mut vertices[v2 as usize];
+            if !vertex_2.is_virtual {
+                vertex_2.is_defect = !vertex_2.is_defect;
+            }
+        }
+        self.get_syndrome()
+    }
+
+    fn clear_errors(&mut self) {
+        let (vertices, edges) = self.vertices_edges();
+        for vertex in vertices.iter_mut() {
+            vertex.is_defect = false;
+        }
+        for edge in edges.iter_mut() {
+            edge.is_erasure = true;
+        }
+    }
+
     fn is_virtual(&self, vertex_idx: usize) -> bool {
         let (vertices, _edges) = self.immutable_vertices_edges();
         vertices[vertex_idx].is_virtual
     }
 
     fn is_defect(&self, vertex_idx: usize) -> bool {
         let (vertices, _edges) = self.immutable_vertices_edges();
         vertices[vertex_idx].is_defect
     }
 
     /// reorder the vertices such that new vertices (the indices of the old order) is sequential
+    #[allow(clippy::unnecessary_cast)]
     fn reorder_vertices(&mut self, sequential_vertices: &Vec<VertexIndex>) {
         let (vertices, edges) = self.vertices_edges();
         assert_eq!(vertices.len(), sequential_vertices.len(), "amount of vertices must be same");
         let old_to_new = build_old_to_new(sequential_vertices);
         // change the vertices numbering
-        *vertices = (0..vertices.len()).map(|new_index| {
-            vertices[sequential_vertices[new_index] as usize].clone()
-        }).collect();
+        *vertices = (0..vertices.len())
+            .map(|new_index| vertices[sequential_vertices[new_index] as usize].clone())
+            .collect();
         for edge in edges.iter_mut() {
             let (old_left, old_right) = edge.vertices;
-            edge.vertices = (old_to_new[old_left as usize].unwrap(), old_to_new[old_right as usize].unwrap());
+            edge.vertices = (
+                old_to_new[old_left as usize].unwrap(),
+                old_to_new[old_right as usize].unwrap(),
+            );
         }
     }
-
 }
 
-#[cfg(feature="python_binding")]
-use rand::{Rng, thread_rng};
+#[cfg(feature = "python_binding")]
+use rand::{thread_rng, Rng};
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 macro_rules! bind_trait_example_code {
     ($struct_name:ident) => {
         #[pymethods]
         impl $struct_name {
-            fn __repr__(&self) -> String { format!("{:?}", self) }
+            fn __repr__(&self) -> String {
+                format!("{:?}", self)
+            }
             #[pyo3(name = "vertex_num")]
-            fn trait_vertex_num(&self) -> VertexNum { self.vertex_num() }
+            fn trait_vertex_num(&self) -> VertexNum {
+                self.vertex_num()
+            }
             #[pyo3(name = "compute_weights")]
-            fn trait_compute_weights(&mut self, max_half_weight: Weight) { self.compute_weights(max_half_weight) }
+            fn trait_compute_weights(&mut self, max_half_weight: Weight) {
+                self.compute_weights(max_half_weight)
+            }
             #[pyo3(name = "sanity_check")]
-            fn trait_sanity_check(&self) -> Option<String> { self.sanity_check().err() }
+            fn trait_sanity_check(&self) -> Option<String> {
+                self.sanity_check().err()
+            }
             #[pyo3(name = "set_probability")]
-            fn trait_set_probability(&mut self, p: f64) { self.set_probability(p) }
+            fn trait_set_probability(&mut self, p: f64) {
+                self.set_probability(p)
+            }
             #[pyo3(name = "set_erasure_probability")]
-            fn trait_set_erasure_probability(&mut self, p: f64) { self.set_erasure_probability(p) }
+            fn trait_set_erasure_probability(&mut self, p: f64) {
+                self.set_erasure_probability(p)
+            }
             #[pyo3(name = "fill_vertices")]
-            fn trait_fill_vertices(&mut self, vertex_num: VertexNum) { self.fill_vertices(vertex_num) }
+            fn trait_fill_vertices(&mut self, vertex_num: VertexNum) {
+                self.fill_vertices(vertex_num)
+            }
             #[pyo3(name = "get_positions")]
-            fn trait_get_positions(&self) -> Vec<VisualizePosition> { self.get_positions() }
+            fn trait_get_positions(&self) -> Vec<VisualizePosition> {
+                self.get_positions()
+            }
             #[pyo3(name = "get_initializer")]
-            fn trait_get_initializer(&self) -> SolverInitializer { self.get_initializer() }
+            fn trait_get_initializer(&self) -> SolverInitializer {
+                self.get_initializer()
+            }
             #[pyo3(name = "set_defect_vertices")]
-            fn trait_set_defect_vertices(&mut self, defect_vertices: Vec<VertexIndex>) { self.set_defect_vertices(&defect_vertices) }
+            fn trait_set_defect_vertices(&mut self, defect_vertices: Vec<VertexIndex>) {
+                self.set_defect_vertices(&defect_vertices)
+            }
             #[pyo3(name = "set_erasures")]
-            fn trait_set_erasures(&mut self, erasures: Vec<EdgeIndex>) { self.set_erasures(&erasures) }
+            fn trait_set_erasures(&mut self, erasures: Vec<EdgeIndex>) {
+                self.set_erasures(&erasures)
+            }
             #[pyo3(name = "set_syndrome")]
-            fn trait_set_syndrome(&mut self, syndrome_pattern: &SyndromePattern) { self.set_syndrome(syndrome_pattern) }
+            fn trait_set_syndrome(&mut self, syndrome_pattern: &SyndromePattern) {
+                self.set_syndrome(syndrome_pattern)
+            }
             #[pyo3(name = "get_defect_vertices")]
-            fn trait_get_defect_vertices(&self) -> Vec<VertexIndex> { self.get_defect_vertices() }
+            fn trait_get_defect_vertices(&self) -> Vec<VertexIndex> {
+                self.get_defect_vertices()
+            }
             #[pyo3(name = "get_erasures")]
-            fn trait_get_erasures(&self) -> Vec<EdgeIndex> { self.get_erasures() }
+            fn trait_get_erasures(&self) -> Vec<EdgeIndex> {
+                self.get_erasures()
+            }
             #[pyo3(name = "get_syndrome")]
-            fn trait_get_syndrome(&self) -> SyndromePattern { self.get_syndrome() }
-            #[pyo3(name = "generate_random_errors")]
-            #[args(seed = "thread_rng().gen()")]
-            fn trait_generate_random_errors(&mut self, seed: u64) -> SyndromePattern { self.generate_random_errors(seed) }
+            fn trait_get_syndrome(&self) -> SyndromePattern {
+                self.get_syndrome()
+            }
+            #[pyo3(name = "generate_random_errors", signature = (seed=thread_rng().gen()))]
+            fn trait_generate_random_errors(&mut self, seed: u64) -> SyndromePattern {
+                self.generate_random_errors(seed)
+            }
+            #[pyo3(name = "generate_errors")]
+            fn trait_generate_errors(&mut self, edge_indices: Vec<EdgeIndex>) -> SyndromePattern {
+                self.generate_errors(&edge_indices)
+            }
+            #[pyo3(name = "clear_errors")]
+            fn trait_clear_errors(&mut self) {
+                self.clear_errors()
+            }
             #[pyo3(name = "is_virtual")]
-            fn trait_is_virtual(&mut self, vertex_idx: usize) -> bool { self.is_virtual(vertex_idx) }
+            fn trait_is_virtual(&mut self, vertex_idx: usize) -> bool {
+                self.is_virtual(vertex_idx)
+            }
             #[pyo3(name = "is_defect")]
-            fn trait_is_defect(&mut self, vertex_idx: usize) -> bool { self.is_defect(vertex_idx) }
+            fn trait_is_defect(&mut self, vertex_idx: usize) -> bool {
+                self.is_defect(vertex_idx)
+            }
             #[pyo3(name = "reorder_vertices")]
-            fn trait_reorder_vertices(&mut self, sequential_vertices: Vec<VertexIndex>) { self.reorder_vertices(&sequential_vertices) }
-            #[pyo3(name = "snapshot")]
-            #[args(abbrev = "true")]
-            fn trait_snapshot(&mut self, abbrev: bool) -> PyObject { json_to_pyobject(self.snapshot(abbrev)) }
+            fn trait_reorder_vertices(&mut self, sequential_vertices: Vec<VertexIndex>) {
+                self.reorder_vertices(&sequential_vertices)
+            }
+            #[pyo3(name = "snapshot", signature = (abbrev=true))]
+            fn trait_snapshot(&mut self, abbrev: bool) -> PyObject {
+                json_to_pyobject(self.snapshot(abbrev))
+            }
         }
     };
 }
 
-impl<T> FusionVisualizer for T where T: ExampleCode {
+impl<T> FusionVisualizer for T
+where
+    T: ExampleCode,
+{
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         let (self_vertices, self_edges) = self.immutable_vertices_edges();
         let mut vertices = Vec::<serde_json::Value>::new();
         for vertex in self_vertices.iter() {
             vertices.push(json!({
                 if abbrev { "v" } else { "is_virtual" }: i32::from(vertex.is_virtual),
                 if abbrev { "s" } else { "is_defect" }: i32::from(vertex.is_defect),
@@ -433,63 +524,66 @@
     pub vertices: Vec<CodeVertex>,
     /// nearest-neighbor edges in the decoding graph
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub edges: Vec<CodeEdge>,
 }
 
 impl ExampleCode for CodeCapacityRepetitionCode {
-    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) { (&mut self.vertices, &mut self.edges) }
-    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) { (&self.vertices, &self.edges) }
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        (&mut self.vertices, &mut self.edges)
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        (&self.vertices, &self.edges)
+    }
 }
 
-#[cfg(feature="python_binding")]
-bind_trait_example_code!{CodeCapacityRepetitionCode}
+#[cfg(feature = "python_binding")]
+bind_trait_example_code! {CodeCapacityRepetitionCode}
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl CodeCapacityRepetitionCode {
-
     #[cfg_attr(feature = "python_binding", new)]
-    #[cfg_attr(feature = "python_binding", args(max_half_weight = "500"))]
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (d, p, max_half_weight = 500)))]
     pub fn new(d: VertexNum, p: f64, max_half_weight: Weight) -> Self {
         let mut code = Self::create_code(d);
         code.set_probability(p);
         code.compute_weights(max_half_weight);
         code
     }
 
     #[cfg_attr(feature = "python_binding", staticmethod)]
+    #[allow(clippy::unnecessary_cast)]
     pub fn create_code(d: VertexNum) -> Self {
         assert!(d >= 3 && d % 2 == 1, "d must be odd integer >= 3");
-        let vertex_num = (d - 1) + 2;  // two virtual vertices at left and right
-        // create edges
+        let vertex_num = (d - 1) + 2; // two virtual vertices at left and right
+                                      // create edges
         let mut edges = Vec::new();
-        for i in 0..d-1 {
-            edges.push(CodeEdge::new(i, i+1));
+        for i in 0..d - 1 {
+            edges.push(CodeEdge::new(i, i + 1));
         }
-        edges.push(CodeEdge::new(0, d));  // tje left-most edge
+        edges.push(CodeEdge::new(0, d)); // tje left-most edge
         let mut code = Self {
             vertices: Vec::new(),
             edges,
         };
         // create vertices
         code.fill_vertices(vertex_num);
-        code.vertices[d as usize -1].is_virtual = true;
+        code.vertices[d as usize - 1].is_virtual = true;
         code.vertices[d as usize].is_virtual = true;
         let mut positions = Vec::new();
         for i in 0..d {
             positions.push(VisualizePosition::new(0., i as f64, 0.));
         }
         positions.push(VisualizePosition::new(0., -1., 0.));
         for (i, position) in positions.into_iter().enumerate() {
             code.vertices[i].position = position;
         }
         code
     }
-
 }
 
 /// code capacity noise model is a single measurement round with perfect stabilizer measurements;
 /// e.g. this is the decoding graph of a CSS surface code (standard one, not rotated one) with X-type stabilizers
 #[derive(Clone, Debug)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
@@ -499,49 +593,53 @@
     pub vertices: Vec<CodeVertex>,
     /// nearest-neighbor edges in the decoding graph
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub edges: Vec<CodeEdge>,
 }
 
 impl ExampleCode for CodeCapacityPlanarCode {
-    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) { (&mut self.vertices, &mut self.edges) }
-    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) { (&self.vertices, &self.edges) }
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        (&mut self.vertices, &mut self.edges)
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        (&self.vertices, &self.edges)
+    }
 }
 
-#[cfg(feature="python_binding")]
-bind_trait_example_code!{CodeCapacityPlanarCode}
+#[cfg(feature = "python_binding")]
+bind_trait_example_code! {CodeCapacityPlanarCode}
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl CodeCapacityPlanarCode {
-
     #[cfg_attr(feature = "python_binding", new)]
-    #[cfg_attr(feature = "python_binding", args(max_half_weight = "500"))]
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (d, p, max_half_weight = 500)))]
     pub fn new(d: VertexNum, p: f64, max_half_weight: Weight) -> Self {
         let mut code = Self::create_code(d);
         code.set_probability(p);
         code.compute_weights(max_half_weight);
         code
     }
 
     #[cfg_attr(feature = "python_binding", staticmethod)]
+    #[allow(clippy::unnecessary_cast)]
     pub fn create_code(d: VertexNum) -> Self {
         assert!(d >= 3 && d % 2 == 1, "d must be odd integer >= 3");
-        let row_vertex_num = (d-1) + 2;  // two virtual nodes at left and right
-        let vertex_num = row_vertex_num * d;  // `d` rows
-        // create edges
+        let row_vertex_num = (d - 1) + 2; // two virtual nodes at left and right
+        let vertex_num = row_vertex_num * d; // `d` rows
+                                             // create edges
         let mut edges = Vec::new();
         for row in 0..d {
             let bias = row * row_vertex_num;
-            for i in 0..d-1 {
-                edges.push(CodeEdge::new(bias + i, bias + i+1));
+            for i in 0..d - 1 {
+                edges.push(CodeEdge::new(bias + i, bias + i + 1));
             }
-            edges.push(CodeEdge::new(bias, bias + d));  // left most edge
+            edges.push(CodeEdge::new(bias, bias + d)); // left most edge
             if row + 1 < d {
-                for i in 0..d-1 {
+                for i in 0..d - 1 {
                     edges.push(CodeEdge::new(bias + i, bias + i + row_vertex_num));
                 }
             }
         }
         let mut code = Self {
             vertices: Vec::new(),
             edges,
@@ -562,15 +660,14 @@
             positions.push(VisualizePosition::new(pos_i, -1., 0.));
         }
         for (i, position) in positions.into_iter().enumerate() {
             code.vertices[i].position = position;
         }
         code
     }
-
 }
 
 /// phenomenological noise model is multiple measurement rounds adding only measurement errors
 /// e.g. this is the decoding graph of a CSS surface code (standard one, not rotated one) with X-type stabilizers
 #[derive(Clone, Debug)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
@@ -580,62 +677,66 @@
     pub vertices: Vec<CodeVertex>,
     /// nearest-neighbor edges in the decoding graph
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub edges: Vec<CodeEdge>,
 }
 
 impl ExampleCode for PhenomenologicalPlanarCode {
-    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) { (&mut self.vertices, &mut self.edges) }
-    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) { (&self.vertices, &self.edges) }
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        (&mut self.vertices, &mut self.edges)
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        (&self.vertices, &self.edges)
+    }
 }
 
-#[cfg(feature="python_binding")]
-bind_trait_example_code!{PhenomenologicalPlanarCode}
+#[cfg(feature = "python_binding")]
+bind_trait_example_code! {PhenomenologicalPlanarCode}
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl PhenomenologicalPlanarCode {
-
     #[cfg_attr(feature = "python_binding", new)]
-    #[cfg_attr(feature = "python_binding", args(max_half_weight = "500"))]
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (d, noisy_measurements, p, max_half_weight = 500)))]
     pub fn new(d: VertexNum, noisy_measurements: VertexNum, p: f64, max_half_weight: Weight) -> Self {
         let mut code = Self::create_code(d, noisy_measurements);
         code.set_probability(p);
         code.compute_weights(max_half_weight);
         code
     }
 
     #[cfg_attr(feature = "python_binding", staticmethod)]
+    #[allow(clippy::unnecessary_cast)]
     pub fn create_code(d: VertexNum, noisy_measurements: VertexNum) -> Self {
         assert!(d >= 3 && d % 2 == 1, "d must be odd integer >= 3");
-        let row_vertex_num = (d-1) + 2;  // two virtual nodes at left and right
-        let t_vertex_num = row_vertex_num * d;  // `d` rows
-        let td = noisy_measurements + 1;  // a perfect measurement round is capped at the end
-        let vertex_num = t_vertex_num * td;  // `td` layers
-        // create edges
+        let row_vertex_num = (d - 1) + 2; // two virtual nodes at left and right
+        let t_vertex_num = row_vertex_num * d; // `d` rows
+        let td = noisy_measurements + 1; // a perfect measurement round is capped at the end
+        let vertex_num = t_vertex_num * td; // `td` layers
+                                            // create edges
         let mut edges = Vec::new();
         for t in 0..td {
             let t_bias = t * t_vertex_num;
             for row in 0..d {
                 let bias = t_bias + row * row_vertex_num;
-                for i in 0..d-1 {
-                    edges.push(CodeEdge::new(bias + i, bias + i+1));
+                for i in 0..d - 1 {
+                    edges.push(CodeEdge::new(bias + i, bias + i + 1));
                 }
-                edges.push(CodeEdge::new(bias, bias + d));  // left most edge
+                edges.push(CodeEdge::new(bias, bias + d)); // left most edge
                 if row + 1 < d {
-                    for i in 0..d-1 {
+                    for i in 0..d - 1 {
                         edges.push(CodeEdge::new(bias + i, bias + i + row_vertex_num));
                     }
                 }
             }
             // inter-layer connection
             if t + 1 < td {
                 for row in 0..d {
                     let bias = t_bias + row * row_vertex_num;
-                    for i in 0..d-1 {
+                    for i in 0..d - 1 {
                         edges.push(CodeEdge::new(bias + i, bias + i + t_vertex_num));
                     }
                 }
             }
         }
         let mut code = Self {
             vertices: Vec::new(),
@@ -663,15 +764,14 @@
             }
         }
         for (i, position) in positions.into_iter().enumerate() {
             code.vertices[i].position = position;
         }
         code
     }
-
 }
 
 /// (not accurate) circuit-level noise model is multiple measurement rounds with errors between each two-qubit gates
 /// e.g. this is the decoding graph of a CSS surface code (standard one, not rotated one) with X-type stabilizers
 #[derive(Clone, Debug)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
@@ -681,38 +781,48 @@
     pub vertices: Vec<CodeVertex>,
     /// nearest-neighbor edges in the decoding graph
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub edges: Vec<CodeEdge>,
 }
 
 impl ExampleCode for CircuitLevelPlanarCode {
-    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) { (&mut self.vertices, &mut self.edges) }
-    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) { (&self.vertices, &self.edges) }
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        (&mut self.vertices, &mut self.edges)
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        (&self.vertices, &self.edges)
+    }
 }
 
-#[cfg(feature="python_binding")]
-bind_trait_example_code!{CircuitLevelPlanarCode}
+#[cfg(feature = "python_binding")]
+bind_trait_example_code! {CircuitLevelPlanarCode}
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl CircuitLevelPlanarCode {
-
     /// by default diagonal edge has error rate p/3 to mimic the behavior of unequal weights
     #[cfg_attr(feature = "python_binding", new)]
-    #[cfg_attr(feature = "python_binding", args(max_half_weight = "500"))]
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (d, noisy_measurements, p, max_half_weight = 500)))]
     pub fn new(d: VertexNum, noisy_measurements: VertexNum, p: f64, max_half_weight: Weight) -> Self {
-        Self::new_diagonal(d, noisy_measurements, p, max_half_weight, p/3.)
+        Self::new_diagonal(d, noisy_measurements, p, max_half_weight, Some(p / 3.))
     }
 
     #[cfg_attr(feature = "python_binding", staticmethod)]
-    #[cfg_attr(feature = "python_binding", args(max_half_weight = "500"))]
-    pub fn new_diagonal(d: VertexNum, noisy_measurements: VertexNum, p: f64, max_half_weight: Weight, diagonal_p: f64) -> Self {
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (d, noisy_measurements, p, max_half_weight = 500, diagonal_p = None)))]
+    #[allow(clippy::unnecessary_cast)]
+    pub fn new_diagonal(
+        d: VertexNum,
+        noisy_measurements: VertexNum,
+        p: f64,
+        max_half_weight: Weight,
+        diagonal_p: Option<f64>,
+    ) -> Self {
         let mut code = Self::create_code(d, noisy_measurements);
         code.set_probability(p);
-        if diagonal_p != p {
+        if let Some(diagonal_p) = diagonal_p {
             let (vertices, edges) = code.vertices_edges();
             for edge in edges.iter_mut() {
                 let (v1, v2) = edge.vertices;
                 let v1p = &vertices[v1 as usize].position;
                 let v2p = &vertices[v2 as usize].position;
                 let manhattan_distance = (v1p.i - v2p.i).abs() + (v1p.j - v2p.j).abs() + (v1p.t - v2p.t).abs();
                 if manhattan_distance > 1. {
@@ -721,47 +831,48 @@
             }
         }
         code.compute_weights(max_half_weight);
         code
     }
 
     #[cfg_attr(feature = "python_binding", staticmethod)]
+    #[allow(clippy::unnecessary_cast)]
     pub fn create_code(d: VertexNum, noisy_measurements: VertexNum) -> Self {
         assert!(d >= 3 && d % 2 == 1, "d must be odd integer >= 3");
-        let row_vertex_num = (d-1) + 2;  // two virtual nodes at left and right
-        let t_vertex_num = row_vertex_num * d;  // `d` rows
-        let td = noisy_measurements + 1;  // a perfect measurement round is capped at the end
-        let vertex_num = t_vertex_num * td;  // `td` layers
-        // create edges
+        let row_vertex_num = (d - 1) + 2; // two virtual nodes at left and right
+        let t_vertex_num = row_vertex_num * d; // `d` rows
+        let td = noisy_measurements + 1; // a perfect measurement round is capped at the end
+        let vertex_num = t_vertex_num * td; // `td` layers
+                                            // create edges
         let mut edges = Vec::new();
         for t in 0..td {
             let t_bias = t * t_vertex_num;
             for row in 0..d {
                 let bias = t_bias + row * row_vertex_num;
-                for i in 0..d-1 {
-                    edges.push(CodeEdge::new(bias + i, bias + i+1));
+                for i in 0..d - 1 {
+                    edges.push(CodeEdge::new(bias + i, bias + i + 1));
                 }
-                edges.push(CodeEdge::new(bias, bias + d));  // left most edge
+                edges.push(CodeEdge::new(bias, bias + d)); // left most edge
                 if row + 1 < d {
-                    for i in 0..d-1 {
+                    for i in 0..d - 1 {
                         edges.push(CodeEdge::new(bias + i, bias + i + row_vertex_num));
                     }
                 }
             }
             // inter-layer connection
             if t + 1 < td {
                 for row in 0..d {
                     let bias = t_bias + row * row_vertex_num;
-                    for i in 0..d-1 {
+                    for i in 0..d - 1 {
                         edges.push(CodeEdge::new(bias + i, bias + i + t_vertex_num));
                         let diagonal_diffs: Vec<(isize, isize)> = vec![(0, 1), (1, 0), (1, 1)];
                         for (di, dj) in diagonal_diffs {
-                            let new_row = row as isize + di;  // row corresponds to `i`
-                            let new_i = i as isize + dj;  // i corresponds to `j`
-                            if new_row >= 0 && new_i >= 0 && new_row < d as isize && new_i < (d-1) as isize {
+                            let new_row = row as isize + di; // row corresponds to `i`
+                            let new_i = i as isize + dj; // i corresponds to `j`
+                            if new_row >= 0 && new_i >= 0 && new_row < d as isize && new_i < (d - 1) as isize {
                                 let new_bias = t_bias + (new_row as VertexNum) * row_vertex_num + t_vertex_num;
                                 edges.push(CodeEdge::new(bias + i, new_bias + new_i as VertexNum));
                             }
                         }
                     }
                 }
             }
@@ -792,15 +903,222 @@
             }
         }
         for (i, position) in positions.into_iter().enumerate() {
             code.vertices[i].position = position;
         }
         code
     }
+}
+
+/// CSS surface code (the rotated one) with X-type stabilizers
+#[derive(Clone, Debug)]
+#[cfg_attr(feature = "python_binding", cfg_eval)]
+#[cfg_attr(feature = "python_binding", pyclass)]
+pub struct CodeCapacityRotatedCode {
+    /// vertices in the code
+    #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    pub vertices: Vec<CodeVertex>,
+    /// nearest-neighbor edges in the decoding graph
+    #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    pub edges: Vec<CodeEdge>,
+}
+
+impl ExampleCode for CodeCapacityRotatedCode {
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        (&mut self.vertices, &mut self.edges)
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        (&self.vertices, &self.edges)
+    }
+}
+
+#[cfg(feature = "python_binding")]
+bind_trait_example_code! {CodeCapacityRotatedCode}
+
+#[cfg_attr(feature = "python_binding", cfg_eval)]
+#[cfg_attr(feature = "python_binding", pymethods)]
+impl CodeCapacityRotatedCode {
+    #[cfg_attr(feature = "python_binding", new)]
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (d, p, max_half_weight = 500)))]
+    pub fn new(d: VertexNum, p: f64, max_half_weight: Weight) -> Self {
+        let mut code = Self::create_code(d);
+        code.set_probability(p);
+        code.compute_weights(max_half_weight);
+        code
+    }
+
+    #[cfg_attr(feature = "python_binding", staticmethod)]
+    #[allow(clippy::unnecessary_cast)]
+    pub fn create_code(d: VertexNum) -> Self {
+        assert!(d >= 3 && d % 2 == 1, "d must be odd integer >= 3");
+        let row_vertex_num = (d - 1) / 2 + 1; // a virtual node at either left or right
+        let vertex_num = row_vertex_num * (d + 1); // d+1 rows
+                                                   // create edges
+        let mut edges = Vec::new();
+        for row in 0..d {
+            let bias = row * row_vertex_num;
+            if row % 2 == 0 {
+                for i in 0..d {
+                    if i % 2 == 0 {
+                        edges.push(CodeEdge::new(bias + i / 2, bias + row_vertex_num + i / 2));
+                    } else {
+                        edges.push(CodeEdge::new(bias + (i - 1) / 2, bias + row_vertex_num + (i + 1) / 2));
+                    }
+                }
+            } else {
+                for i in 0..d {
+                    if i % 2 == 0 {
+                        edges.push(CodeEdge::new(bias + i / 2, bias + row_vertex_num + i / 2));
+                    } else {
+                        edges.push(CodeEdge::new(bias + (i + 1) / 2, bias + row_vertex_num + (i - 1) / 2));
+                    }
+                }
+            }
+        }
+        let mut code = Self {
+            vertices: Vec::new(),
+            edges,
+        };
+        // create vertices
+        code.fill_vertices(vertex_num);
+        for row in 0..d + 1 {
+            let bias = row * row_vertex_num;
+            if row % 2 == 0 {
+                code.vertices[(bias + row_vertex_num - 1) as usize].is_virtual = true;
+            } else {
+                code.vertices[(bias) as usize].is_virtual = true;
+            }
+        }
+        let mut positions = Vec::new();
+        for row in 0..d + 1 {
+            let pos_i = row as f64;
+            for i in 0..row_vertex_num {
+                let pos_bias = (row % 2 == 0) as VertexNum;
+                positions.push(VisualizePosition::new(pos_i, (i * 2 + pos_bias) as f64, 0.));
+            }
+        }
+        for (i, position) in positions.into_iter().enumerate() {
+            code.vertices[i].position = position;
+        }
+        code
+    }
+}
 
+/// CSS surface code (the rotated one) with X-type stabilizers
+#[derive(Clone, Debug)]
+#[cfg_attr(feature = "python_binding", cfg_eval)]
+#[cfg_attr(feature = "python_binding", pyclass)]
+pub struct PhenomenologicalRotatedCode {
+    /// vertices in the code
+    #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    pub vertices: Vec<CodeVertex>,
+    /// nearest-neighbor edges in the decoding graph
+    #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    pub edges: Vec<CodeEdge>,
+}
+
+impl ExampleCode for PhenomenologicalRotatedCode {
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        (&mut self.vertices, &mut self.edges)
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        (&self.vertices, &self.edges)
+    }
+}
+
+#[cfg(feature = "python_binding")]
+bind_trait_example_code! {PhenomenologicalRotatedCode}
+
+#[cfg_attr(feature = "python_binding", cfg_eval)]
+#[cfg_attr(feature = "python_binding", pymethods)]
+impl PhenomenologicalRotatedCode {
+    #[cfg_attr(feature = "python_binding", new)]
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (d, noisy_measurements, p, max_half_weight = 500)))]
+    pub fn new(d: VertexNum, noisy_measurements: VertexNum, p: f64, max_half_weight: Weight) -> Self {
+        let mut code = Self::create_code(d, noisy_measurements);
+        code.set_probability(p);
+        code.compute_weights(max_half_weight);
+        code
+    }
+
+    #[cfg_attr(feature = "python_binding", staticmethod)]
+    #[allow(clippy::unnecessary_cast)]
+    pub fn create_code(d: VertexNum, noisy_measurements: VertexNum) -> Self {
+        assert!(d >= 3 && d % 2 == 1, "d must be odd integer >= 3");
+        let row_vertex_num = (d - 1) / 2 + 1; // a virtual node at either left or right
+        let t_vertex_num = row_vertex_num * (d + 1); // d+1 rows
+        let td = noisy_measurements + 1; // a perfect measurement round is capped at the end
+        let vertex_num = t_vertex_num * td; // `td` layers
+                                            // create edges
+        let mut edges = Vec::new();
+        for t in 0..td {
+            let t_bias = t * t_vertex_num;
+            for row in 0..d {
+                let bias = t_bias + row * row_vertex_num;
+                if row % 2 == 0 {
+                    for i in 0..d {
+                        if i % 2 == 0 {
+                            edges.push(CodeEdge::new(bias + i / 2, bias + row_vertex_num + i / 2));
+                        } else {
+                            edges.push(CodeEdge::new(bias + (i - 1) / 2, bias + row_vertex_num + (i + 1) / 2));
+                        }
+                    }
+                } else {
+                    for i in 0..d {
+                        if i % 2 == 0 {
+                            edges.push(CodeEdge::new(bias + i / 2, bias + row_vertex_num + i / 2));
+                        } else {
+                            edges.push(CodeEdge::new(bias + (i + 1) / 2, bias + row_vertex_num + (i - 1) / 2));
+                        }
+                    }
+                }
+            }
+            // inter-layer connection
+            if t + 1 < td {
+                for row in 0..d + 1 {
+                    let bias = t_bias + row * row_vertex_num;
+                    for i in 0..row_vertex_num {
+                        edges.push(CodeEdge::new(bias + i, bias + i + t_vertex_num));
+                    }
+                }
+            }
+        }
+        let mut code = Self {
+            vertices: Vec::new(),
+            edges,
+        };
+        // create vertices
+        code.fill_vertices(vertex_num);
+        for t in 0..td {
+            let t_bias = t * t_vertex_num;
+            for row in 0..d + 1 {
+                let bias = t_bias + row * row_vertex_num;
+                if row % 2 == 0 {
+                    code.vertices[(bias + row_vertex_num - 1) as usize].is_virtual = true;
+                } else {
+                    code.vertices[(bias) as usize].is_virtual = true;
+                }
+            }
+        }
+        let mut positions = Vec::new();
+        for t in 0..td {
+            let pos_t = t as f64 * 2f64.sqrt();
+            for row in 0..d + 1 {
+                let pos_i = row as f64;
+                for i in 0..row_vertex_num {
+                    let pos_bias = (row % 2 == 0) as VertexNum;
+                    positions.push(VisualizePosition::new(pos_i, (i * 2 + pos_bias) as f64, pos_t));
+                }
+            }
+        }
+        for (i, position) in positions.into_iter().enumerate() {
+            code.vertices[i].position = position;
+        }
+        code
+    }
 }
 
 /// read from file, including the error patterns;
 /// the point is to avoid bad cache performance, because generating random error requires iterating over a large memory space,
 /// invalidating all cache. also, this can reduce the time of decoding by prepare the data before hand and could be shared between
 /// different partition configurations
 #[cfg_attr(feature = "python_binding", cfg_eval)]
@@ -814,52 +1132,74 @@
     pub edges: Vec<CodeEdge>,
     /// pre-generated syndrome patterns
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub syndrome_patterns: Vec<SyndromePattern>,
     /// cursor of current errors
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub defect_index: usize,
+    #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    pub cyclic_syndrome: bool,
 }
 
 impl ExampleCode for ErrorPatternReader {
-    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) { (&mut self.vertices, &mut self.edges) }
-    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) { (&self.vertices, &self.edges) }
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        (&mut self.vertices, &mut self.edges)
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        (&self.vertices, &self.edges)
+    }
     fn generate_random_errors(&mut self, _seed: u64) -> SyndromePattern {
-        assert!(self.defect_index < self.syndrome_patterns.len(), "reading syndrome pattern more than in the file, consider generate the file with more data points");
+        if self.cyclic_syndrome {
+            if self.defect_index >= self.syndrome_patterns.len() {
+                self.defect_index = 0; // cyclic
+            }
+        } else {
+            assert!(
+                self.defect_index < self.syndrome_patterns.len(),
+                "reading syndrome pattern more than in the file, consider generate the file with more data points"
+            );
+        }
         let syndrome_pattern = self.syndrome_patterns[self.defect_index].clone();
         self.defect_index += 1;
         syndrome_pattern
     }
 }
 
 impl ErrorPatternReader {
-
+    #[allow(clippy::unnecessary_cast)]
     pub fn new(mut config: serde_json::Value) -> Self {
         let mut filename = "tmp/syndrome_patterns.txt".to_string();
         let config = config.as_object_mut().expect("config must be JSON object");
         if let Some(value) = config.remove("filename") {
             filename = value.as_str().expect("filename string").to_string();
         }
-        if !config.is_empty() { panic!("unknown config keys: {:?}", config.keys().collect::<Vec<&String>>()); }
+        let cyclic_syndrome = if let Some(cyclic_syndrome) = config.remove("cyclic_syndrome") {
+            cyclic_syndrome.as_bool().expect("cyclic_syndrome: bool")
+        } else {
+            false
+        }; // by default not enable cyclic syndrome, to avoid problem
+        if !config.is_empty() {
+            panic!("unknown config keys: {:?}", config.keys().collect::<Vec<&String>>());
+        }
         let file = File::open(filename).unwrap();
         let mut syndrome_patterns = vec![];
         let mut initializer: Option<SolverInitializer> = None;
         let mut positions: Option<Vec<VisualizePosition>> = None;
         for (line_index, line) in io::BufReader::new(file).lines().enumerate() {
             if let Ok(value) = line {
                 match line_index {
                     0 => {
                         assert!(value.starts_with("Syndrome Pattern v1.0 "), "incompatible file version");
-                    },
+                    }
                     1 => {
                         initializer = Some(serde_json::from_str(&value).unwrap());
-                    },
+                    }
                     2 => {
                         positions = Some(serde_json::from_str(&value).unwrap());
-                    },
+                    }
                     _ => {
                         let syndrome_pattern: SyndromePattern = serde_json::from_str(&value).unwrap();
                         syndrome_patterns.push(syndrome_pattern);
                     }
                 }
             }
         }
@@ -867,37 +1207,37 @@
         let positions = positions.expect("positions not present in file");
         assert_eq!(positions.len(), initializer.vertex_num as usize);
         let mut code = Self {
             vertices: Vec::with_capacity(initializer.vertex_num as usize),
             edges: Vec::with_capacity(initializer.weighted_edges.len()),
             syndrome_patterns,
             defect_index: 0,
+            cyclic_syndrome,
         };
         for (left_vertex, right_vertex, weight) in initializer.weighted_edges.iter() {
             assert!(weight % 2 == 0, "weight must be even number");
             code.edges.push(CodeEdge {
                 vertices: (*left_vertex, *right_vertex),
                 p: 0.,  // doesn't matter
-                pe: 0.,  // doesn't matter
+                pe: 0., // doesn't matter
                 half_weight: weight / 2,
-                is_erasure: false,  // doesn't matter
+                is_erasure: false, // doesn't matter
             });
         }
         // automatically create the vertices and nearest-neighbor connection
         code.fill_vertices(initializer.vertex_num);
         // set virtual vertices and positions
         for (vertex_index, position) in positions.into_iter().enumerate() {
             code.vertices[vertex_index].position = position;
         }
         for vertex_index in initializer.virtual_vertices {
             code.vertices[vertex_index as usize].is_virtual = true;
         }
         code
     }
-
 }
 
 /// generate error patterns in parallel by hold multiple instances of the same code type
 pub struct ExampleCodeParallel<CodeType: ExampleCode + Sync + Send + Clone> {
     /// used to provide graph
     pub example: CodeType,
     /// list of codes
@@ -920,78 +1260,121 @@
             syndrome_patterns: vec![],
             code_index: 0,
         }
     }
 }
 
 impl<CodeType: ExampleCode + Sync + Send + Clone> ExampleCode for ExampleCodeParallel<CodeType> {
-    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) { self.example.vertices_edges() }
-    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) { self.example.immutable_vertices_edges() }
+    fn vertices_edges(&mut self) -> (&mut Vec<CodeVertex>, &mut Vec<CodeEdge>) {
+        self.example.vertices_edges()
+    }
+    fn immutable_vertices_edges(&self) -> (&Vec<CodeVertex>, &Vec<CodeEdge>) {
+        self.example.immutable_vertices_edges()
+    }
     fn generate_random_errors(&mut self, seed: u64) -> SyndromePattern {
         if self.code_index == 0 {
             // run generator in parallel
-            (0..self.codes.len()).into_par_iter().map(|code_index| {
-                self.codes[code_index].write().generate_random_errors(seed + (code_index * 1_000_000_000) as u64)
-            }).collect_into_vec(&mut self.syndrome_patterns);
+            (0..self.codes.len())
+                .into_par_iter()
+                .map(|code_index| {
+                    self.codes[code_index]
+                        .write()
+                        .generate_random_errors(seed + (code_index * 1_000_000_000) as u64)
+                })
+                .collect_into_vec(&mut self.syndrome_patterns);
         }
         let syndrome_pattern = self.syndrome_patterns[self.code_index].clone();
         self.code_index = (self.code_index + 1) % self.codes.len();
         syndrome_pattern
     }
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 #[pyfunction]
 pub(crate) fn register(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<CodeVertex>()?;
     m.add_class::<CodeEdge>()?;
     m.add_function(wrap_pyfunction!(weight_of_p, m)?)?;
     m.add_class::<CodeCapacityRepetitionCode>()?;
     m.add_class::<CodeCapacityPlanarCode>()?;
     m.add_class::<PhenomenologicalPlanarCode>()?;
     m.add_class::<CircuitLevelPlanarCode>()?;
+    m.add_class::<CodeCapacityRotatedCode>()?;
+    m.add_class::<PhenomenologicalRotatedCode>()?;
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     fn visualize_code(code: &mut impl ExampleCode, visualize_filename: String) {
         print_visualize_link(visualize_filename.clone());
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         visualizer.snapshot(format!("code"), code).unwrap();
         for round in 0..3 {
             code.generate_random_errors(round);
             visualizer.snapshot(format!("syndrome {}", round + 1), code).unwrap();
         }
     }
 
     #[test]
-    fn example_code_capacity_repetition_code() {  // cargo test example_code_capacity_repetition_code -- --nocapture
+    fn example_code_capacity_repetition_code() {
+        // cargo test example_code_capacity_repetition_code -- --nocapture
         let mut code = CodeCapacityRepetitionCode::new(7, 0.2, 500);
         code.sanity_check().unwrap();
         visualize_code(&mut code, format!("example_code_capacity_repetition_code.json"));
     }
 
     #[test]
-    fn example_code_capacity_planar_code() {  // cargo test example_code_capacity_planar_code -- --nocapture
+    fn example_code_capacity_planar_code() {
+        // cargo test example_code_capacity_planar_code -- --nocapture
         let mut code = CodeCapacityPlanarCode::new(7, 0.1, 500);
         code.sanity_check().unwrap();
         visualize_code(&mut code, format!("example_code_capacity_planar_code.json"));
     }
 
     #[test]
-    fn example_phenomenological_planar_code() {  // cargo test example_phenomenological_planar_code -- --nocapture
+    fn example_phenomenological_planar_code() {
+        // cargo test example_phenomenological_planar_code -- --nocapture
         let mut code = PhenomenologicalPlanarCode::new(7, 7, 0.01, 500);
         code.sanity_check().unwrap();
         visualize_code(&mut code, format!("example_phenomenological_planar_code.json"));
     }
 
     #[test]
-    fn example_circuit_level_planar_code() {  // cargo test example_circuit_level_planar_code -- --nocapture
+    fn example_large_phenomenological_planar_code() {
+        // cargo test example_large_phenomenological_planar_code -- --nocapture
+        let mut code = PhenomenologicalPlanarCode::new(7, 30, 0.01, 500);
+        code.sanity_check().unwrap();
+        visualize_code(&mut code, format!("example_large_phenomenological_planar_code.json"));
+    }
+
+    #[test]
+    fn example_circuit_level_planar_code() {
+        // cargo test example_circuit_level_planar_code -- --nocapture
         let mut code = CircuitLevelPlanarCode::new(7, 7, 0.01, 500);
         code.sanity_check().unwrap();
         visualize_code(&mut code, format!("example_circuit_level_planar_code.json"));
     }
 
+    #[test]
+    fn example_code_capacity_rotated_code() {
+        // cargo test example_code_capacity_rotated_code -- --nocapture
+        let mut code = CodeCapacityRotatedCode::new(5, 0.1, 500);
+        code.sanity_check().unwrap();
+        visualize_code(&mut code, format!("example_code_capacity_rotated_code.json"));
+    }
+
+    #[test]
+    fn example_code_phenomenological_rotated_code() {
+        // cargo test example_code_phenomenological_rotated_code -- --nocapture
+        let mut code = PhenomenologicalRotatedCode::new(5, 5, 0.01, 500);
+        code.sanity_check().unwrap();
+        visualize_code(&mut code, format!("example_code_phenomenological_rotated_code.json"));
+    }
 }
```

### Comparing `fusion_blossom-0.2.2/src/helper.py` & `fusion_blossom-0.2.5/src/helper.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/src/lib.rs` & `fusion_blossom-0.2.5/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,121 @@
-#![cfg_attr(
-    feature="unsafe_pointer",
-    feature(get_mut_unchecked)
-)]
-#![cfg_attr(
-    feature="unsafe_pointer",
-    allow(unused_mut)
-)]
-#![cfg_attr(
-    feature="python_binding",
-    feature(cfg_eval)
-)]
+#![cfg_attr(feature = "unsafe_pointer", feature(get_mut_unchecked))]
+#![cfg_attr(feature = "unsafe_pointer", allow(unused_mut))]
+#![cfg_attr(feature = "python_binding", feature(cfg_eval))]
 
-extern crate libc;
 extern crate cfg_if;
-extern crate rand_xoshiro;
-extern crate priority_queue;
+extern crate libc;
 extern crate parking_lot;
+extern crate priority_queue;
+extern crate rand_xoshiro;
 extern crate serde;
-#[macro_use] extern crate serde_json;
+#[macro_use]
+extern crate serde_json;
 extern crate chrono;
+extern crate clap;
+extern crate core_affinity;
 extern crate derivative;
-extern crate urlencoding;
+extern crate pbr;
+#[cfg(test)]
+extern crate petgraph;
+#[cfg(feature = "python_binding")]
+extern crate pyo3;
+#[cfg(feature = "qecp_integrate")]
+extern crate qecp;
+extern crate rand;
 extern crate rayon;
+extern crate urlencoding;
 extern crate weak_table;
-extern crate rand;
-extern crate core_affinity;
-#[cfg(feature="python_binding")]
-extern crate pyo3;
 
 pub mod blossom_v;
-pub mod util;
+pub mod cli;
 pub mod complete_graph;
-pub mod union_find;
-pub mod visualize;
-pub mod example_codes;
 pub mod dual_module;
-pub mod dual_module_serial;
-pub mod primal_module;
-pub mod primal_module_serial;
-pub mod mwpm_solver;
 pub mod dual_module_parallel;
-pub mod primal_module_parallel;
+pub mod dual_module_serial;
+pub mod example_codes;
 pub mod example_partition;
+pub mod mwpm_solver;
 pub mod pointers;
-#[cfg(feature="python_binding")]
+pub mod primal_module;
+pub mod primal_module_parallel;
+pub mod primal_module_serial;
+pub mod util;
+pub mod visualize;
+#[cfg(feature = "python_binding")]
 use pyo3::prelude::*;
 
-use util::*;
 use complete_graph::*;
+use util::*;
 
-
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 #[pymodule]
 fn fusion_blossom(py: Python<'_>, m: &PyModule) -> PyResult<()> {
     util::register(py, m)?;
     mwpm_solver::register(py, m)?;
     example_codes::register(py, m)?;
     visualize::register(py, m)?;
     primal_module::register(py, m)?;
     let helper_code = include_str!(concat!(env!("CARGO_MANIFEST_DIR"), "/src/helper.py"));
     let helper_module = PyModule::from_code(py, helper_code, "helper", "helper")?;
     helper_module.add("visualizer_website", generate_visualizer_website(py))?;
-    let bottle_code = include_str!(concat!(env!("CARGO_MANIFEST_DIR"), "/src/bottle.py"));  // embed bottle
+    let bottle_code = include_str!(concat!(env!("CARGO_MANIFEST_DIR"), "/src/bottle.py")); // embed bottle
     helper_module.add_submodule(PyModule::from_code(py, bottle_code, "bottle", "bottle")?)?;
     m.add_submodule(helper_module)?;
     let helper_register = helper_module.getattr("register")?;
-    helper_register.call1((m, ))?;
+    helper_register.call1((m,))?;
     Ok(())
 }
 
 /// use fusion blossom to solve MWPM (to optimize speed, consider reuse a [`mwpm_solver::SolverSerial`] object)
+#[allow(clippy::unnecessary_cast)]
 pub fn fusion_mwpm(initializer: &SolverInitializer, syndrome_pattern: &SyndromePattern) -> Vec<VertexIndex> {
     // sanity check
     assert!(initializer.vertex_num > 1, "at least one vertex required");
     let max_safe_weight = ((Weight::MAX as usize) / initializer.vertex_num as usize) as Weight;
     for (i, j, weight) in initializer.weighted_edges.iter() {
         if weight > &max_safe_weight {
-            panic!("edge {}-{} has weight {} > max safe weight {}, it may cause fusion blossom to overflow", i, j, weight, max_safe_weight);
+            panic!(
+                "edge {}-{} has weight {} > max safe weight {}, it may cause fusion blossom to overflow",
+                i, j, weight, max_safe_weight
+            );
         }
     }
     // by default use serial implementation fusion blossom
     mwpm_solver::LegacySolverSerial::mwpm_solve(initializer, syndrome_pattern)
 }
 
 /// fall back to use blossom V library to solve MWPM (install blossom V required)
+#[allow(clippy::unnecessary_cast)]
 pub fn blossom_v_mwpm(initializer: &SolverInitializer, defect_vertices: &Vec<VertexIndex>) -> Vec<VertexIndex> {
     // this feature will be automatically enabled if you install blossom V source code, see README.md for more information
     if cfg!(not(feature = "blossom_v")) {
         panic!("need blossom V library, see README.md")
     }
     // sanity check
     assert!(initializer.vertex_num > 1, "at least one vertex required");
     let max_safe_weight = ((i32::MAX as usize) / initializer.vertex_num as usize) as Weight;
     for (i, j, weight) in initializer.weighted_edges.iter() {
         if weight > &max_safe_weight {
-            panic!("edge {}-{} has weight {} > max safe weight {}, it may cause blossom V library to overflow", i, j, weight, max_safe_weight);
+            panic!(
+                "edge {}-{} has weight {} > max safe weight {}, it may cause blossom V library to overflow",
+                i, j, weight, max_safe_weight
+            );
         }
     }
     let mut complete_graph = CompleteGraph::new(initializer.vertex_num, &initializer.weighted_edges);
     blossom_v_mwpm_reuse(&mut complete_graph, initializer, defect_vertices)
 }
 
-pub fn blossom_v_mwpm_reuse(complete_graph: &mut CompleteGraph, initializer: &SolverInitializer, defect_vertices: &Vec<VertexIndex>) -> Vec<VertexIndex> {
+#[allow(clippy::unnecessary_cast)]
+pub fn blossom_v_mwpm_reuse(
+    complete_graph: &mut CompleteGraph,
+    initializer: &SolverInitializer,
+    defect_vertices: &Vec<VertexIndex>,
+) -> Vec<VertexIndex> {
     // first collect virtual vertices and real vertices
     let mut is_virtual: Vec<bool> = (0..initializer.vertex_num).map(|_| false).collect();
     let mut is_defect: Vec<bool> = (0..initializer.vertex_num).map(|_| false).collect();
     for &virtual_vertex in initializer.virtual_vertices.iter() {
         assert!(virtual_vertex < initializer.vertex_num, "invalid input");
         assert!(!is_virtual[virtual_vertex as usize], "same virtual vertex appears twice");
         is_virtual[virtual_vertex as usize] = true;
@@ -131,61 +141,77 @@
                 boundary = Some((peer, weight));
             }
         }
         if let Some((_, weight)) = boundary {
             // connect this real vertex to it's corresponding virtual vertex
             legacy_weighted_edges.push((i, i + defect_num, weight as u32));
         }
-        boundaries.push(boundary);  // save for later resolve legacy matchings
+        boundaries.push(boundary); // save for later resolve legacy matchings
         for (&peer, &(_, weight)) in complete_graph_edges.iter() {
             if is_defect[peer as usize] {
                 let j = mapping_to_defect_vertices[peer as usize];
-                if i < j {  // remove duplicated edges
+                if i < j {
+                    // remove duplicated edges
                     legacy_weighted_edges.push((i, j, weight as u32));
                     // println!{"edge {} {} {} ", i, j, weight};
                 }
             }
         }
-        for j in (i+1)..defect_num {
+        for j in (i + 1)..defect_num {
             // virtual boundaries are always fully connected with weight 0
             legacy_weighted_edges.push((i + defect_num, j + defect_num, 0));
         }
     }
     // run blossom V to get matchings
     // println!("[debug] legacy_vertex_num: {:?}", legacy_vertex_num);
     // println!("[debug] legacy_weighted_edges: {:?}", legacy_weighted_edges);
     let matchings = blossom_v::safe_minimum_weight_perfect_matching(legacy_vertex_num, &legacy_weighted_edges);
     let mut mwpm_result = Vec::new();
     for i in 0..defect_num {
         let j = matchings[i];
-        if j < defect_num {  // match to a real vertex
+        if j < defect_num {
+            // match to a real vertex
             mwpm_result.push(defect_vertices[j]);
         } else {
-            assert_eq!(j, i + defect_num, "if not matched to another real vertex, it must match to it's corresponding virtual vertex");
-            mwpm_result.push(boundaries[i].as_ref().expect("boundary must exist if match to virtual vertex").0);
+            assert_eq!(
+                j,
+                i + defect_num,
+                "if not matched to another real vertex, it must match to it's corresponding virtual vertex"
+            );
+            mwpm_result.push(
+                boundaries[i]
+                    .as_ref()
+                    .expect("boundary must exist if match to virtual vertex")
+                    .0,
+            );
         }
     }
     mwpm_result
 }
 
 #[allow(dead_code)]
 #[derive(Debug, Clone)]
 pub struct DetailedMatching {
     /// must be a real vertex
-    pub a: SyndromeIndex,
+    pub a: DefectIndex,
     /// might be a virtual vertex, but if it's a real vertex, then b > a stands
-    pub b: SyndromeIndex,
+    pub b: DefectIndex,
     /// every vertex in between this pair, in the order `a -> path[0].0 -> path[1].0 -> .... -> path[-1].0` and it's guaranteed that path[-1].0 = b; might be empty if a and b are adjacent
-    pub path: Vec<(SyndromeIndex, Weight)>,
+    pub path: Vec<(DefectIndex, Weight)>,
     /// the overall weight of this path
     pub weight: Weight,
 }
 
 /// compute detailed matching information, note that the output will not include duplicated matched pairs
-pub fn detailed_matching(initializer: &SolverInitializer, defect_vertices: &Vec<SyndromeIndex>, mwpm_result: &Vec<SyndromeIndex>) -> Vec<DetailedMatching> {
+#[allow(clippy::unnecessary_cast)]
+pub fn detailed_matching(
+    initializer: &SolverInitializer,
+    defect_vertices: &Vec<DefectIndex>,
+    mwpm_result: &Vec<DefectIndex>,
+) -> Vec<DetailedMatching> {
     let defect_num = defect_vertices.len();
     let mut is_defect: Vec<bool> = (0..initializer.vertex_num).map(|_| false).collect();
     for &defect_vertex in defect_vertices.iter() {
         assert!(defect_vertex < initializer.vertex_num, "invalid input");
         assert!(!is_defect[defect_vertex as usize], "same syndrome vertex appears twice");
         is_defect[defect_vertex as usize] = true;
     }
@@ -193,39 +219,42 @@
     let mut complete_graph = complete_graph::CompleteGraph::new(initializer.vertex_num, &initializer.weighted_edges);
     let mut details = Vec::new();
     for i in 0..defect_num {
         let a = defect_vertices[i];
         let b = mwpm_result[i];
         if !is_defect[b as usize] || a < b {
             let (path, weight) = complete_graph.get_path(a, b);
-            let detail = DetailedMatching {
-                a,
-                b,
-                path,
-                weight,
-            };
+            let detail = DetailedMatching { a, b, path, weight };
             details.push(detail);
         }
     }
     details
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 macro_rules! include_visualize_file {
     ($mapping:ident, $filepath:expr) => {
         $mapping.insert($filepath.to_string(), include_str!(concat!(env!("CARGO_MANIFEST_DIR"), "/visualize/", $filepath)).to_string());
     };
     ($mapping:ident, $filepath:expr, $($other_filepath:expr),+) => {
         include_visualize_file!($mapping, $filepath);
         include_visualize_file!($mapping, $($other_filepath),+);
     };
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 fn generate_visualizer_website(py: Python<'_>) -> &pyo3::types::PyDict {
     use pyo3::types::IntoPyDict;
     let mut mapping = std::collections::BTreeMap::<String, String>::new();
-    include_visualize_file!(mapping, "gui3d.js", "index.js", "patches.js", "primal.js", "cmd.js", "mocker.js");
+    include_visualize_file!(
+        mapping,
+        "gui3d.js",
+        "index.js",
+        "patches.js",
+        "primal.js",
+        "cmd.js",
+        "mocker.js"
+    );
     include_visualize_file!(mapping, "index.html", "partition-profile.html", "icon.svg");
     include_visualize_file!(mapping, "package.json", "package-lock.json");
     mapping.into_py_dict(py)
 }
```

### Comparing `fusion_blossom-0.2.2/src/main.rs` & `fusion_blossom-0.2.5/src/cli.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,106 @@
-extern crate clap;
-extern crate pbr;
-
-use fusion_blossom::example_codes::*;
-use fusion_blossom::util::*;
-use fusion_blossom::visualize::*;
-use fusion_blossom::dual_module::*;
-use fusion_blossom::primal_module::*;
-use fusion_blossom::example_partition;
-use fusion_blossom::mwpm_solver::*;
+use super::dual_module::*;
+use super::example_codes::*;
+use super::example_partition;
+use super::mwpm_solver::*;
+use super::primal_module::*;
+use super::util::*;
+use super::visualize::*;
+#[cfg(feature = "qecp_integrate")]
+use crate::qecp;
+use clap::{Parser, Subcommand, ValueEnum};
 use pbr::ProgressBar;
-use rand::{Rng, thread_rng};
-
-use clap::{ValueEnum, Parser, Subcommand};
+use rand::{thread_rng, Rng};
 use serde::Serialize;
 use serde_json::json;
 use std::env;
 
-
 const TEST_EACH_ROUNDS: usize = 100;
 
-pub fn main() {
-
-    Cli::parse().run();
-
-}
-
 #[derive(Parser, Clone)]
 #[clap(author = clap::crate_authors!(", "))]
 #[clap(version = env!("CARGO_PKG_VERSION"))]
 #[clap(about = "Fusion Blossom Algorithm for fast Quantum Error Correction Decoding")]
 #[clap(color = clap::ColorChoice::Auto)]
 #[clap(propagate_version = true)]
 #[clap(subcommand_required = true)]
 #[clap(arg_required_else_help = true)]
 pub struct Cli {
     #[clap(subcommand)]
     command: Commands,
 }
 
+#[derive(Parser, Clone)]
+pub struct BenchmarkParameters {
+    /// code distance
+    #[clap(value_parser)]
+    d: VertexNum,
+    /// physical error rate: the probability of each edge to
+    #[clap(value_parser)]
+    p: f64,
+    /// rounds of noisy measurement, valid only when multiple rounds
+    #[clap(short = 'e', long, default_value_t = 0.)]
+    pe: f64,
+    /// rounds of noisy measurement, valid only when multiple rounds
+    #[clap(short = 'n', long, default_value_t = 0)]
+    noisy_measurements: VertexNum,
+    /// maximum half weight of edges
+    #[clap(long, default_value_t = 500)]
+    max_half_weight: Weight,
+    /// example code type
+    #[clap(short = 'c', long, value_enum, default_value_t = ExampleCodeType::CodeCapacityPlanarCode)]
+    code_type: ExampleCodeType,
+    /// the configuration of the code builder
+    #[clap(long, default_value_t = ("{}").to_string())]
+    code_config: String,
+    /// logging to the default visualizer file at visualize/data/visualizer.json
+    #[clap(long, action)]
+    enable_visualizer: bool,
+    /// print syndrome patterns
+    #[clap(long, action)]
+    print_syndrome_pattern: bool,
+    /// the method to verify the correctness of the decoding result
+    #[clap(long, value_enum, default_value_t = Verifier::BlossomV)]
+    verifier: Verifier,
+    /// the number of iterations to run
+    #[clap(short = 'r', long, default_value_t = 1000)]
+    total_rounds: usize,
+    /// select the combination of primal and dual module
+    #[clap(short = 'p', long, value_enum, default_value_t = PrimalDualType::Serial)]
+    primal_dual_type: PrimalDualType,
+    /// the configuration of primal and dual module
+    #[clap(long, default_value_t = ("{}").to_string())]
+    primal_dual_config: String,
+    /// partition strategy
+    #[clap(long, value_enum, default_value_t = PartitionStrategy::None)]
+    partition_strategy: PartitionStrategy,
+    /// the configuration of the partition strategy
+    #[clap(long, default_value_t = ("{}").to_string())]
+    partition_config: String,
+    /// message on the progress bar
+    #[clap(long, default_value_t = format!(""))]
+    pb_message: String,
+    /// use deterministic seed for debugging purpose
+    #[clap(long, action)]
+    use_deterministic_seed: bool,
+    /// the benchmark profile output file path
+    #[clap(long)]
+    benchmark_profiler_output: Option<String>,
+    /// skip some iterations, useful when debugging
+    #[clap(long, default_value_t = 0)]
+    starting_iteration: usize,
+}
+
 #[derive(Subcommand, Clone)]
 #[allow(clippy::large_enum_variant)]
 enum Commands {
     /// benchmark the speed (and also correctness if enabled)
-    Benchmark {
-        /// code distance
-        #[clap(value_parser)]
-        d: VertexNum,
-        /// physical error rate: the probability of each edge to 
-        #[clap(value_parser)]
-        p: f64,
-        /// rounds of noisy measurement, valid only when multiple rounds
-        #[clap(short = 'e', long, default_value_t = 0.)]
-        pe: f64,
-        /// rounds of noisy measurement, valid only when multiple rounds
-        #[clap(short = 'n', long, default_value_t = 0)]
-        noisy_measurements: VertexNum,
-        /// maximum half weight of edges
-        #[clap(long, default_value_t = 500)]
-        max_half_weight: Weight,
-        /// example code type
-        #[clap(short = 'c', long, value_enum, default_value_t = ExampleCodeType::CodeCapacityPlanarCode)]
-        code_type: ExampleCodeType,
-        /// the configuration of the code builder
-        #[clap(long, default_value_t = json!({}))]
-        code_config: serde_json::Value,
-        /// logging to the default visualizer file at visualize/data/visualizer.json
-        #[clap(long, action)]
-        enable_visualizer: bool,
-        /// print syndrome patterns
-        #[clap(long, action)]
-        print_syndrome_pattern: bool,
-        /// the method to verify the correctness of the decoding result
-        #[clap(long, value_enum, default_value_t = Verifier::BlossomV)]
-        verifier: Verifier,
-        /// the number of iterations to run
-        #[clap(short = 'r', long, default_value_t = 1000)]
-        total_rounds: usize,
-        /// select the combination of primal and dual module
-        #[clap(short = 'p', long, value_enum, default_value_t = PrimalDualType::Serial)]
-        primal_dual_type: PrimalDualType,
-        /// the configuration of primal and dual module
-        #[clap(long, default_value_t = json!({}))]
-        primal_dual_config: serde_json::Value,
-        /// partition strategy
-        #[clap(long, value_enum, default_value_t = PartitionStrategy::None)]
-        partition_strategy: PartitionStrategy,
-        /// the configuration of the partition strategy
-        #[clap(long, default_value_t = json!({}))]
-        partition_config: serde_json::Value,
-        /// message on the progress bar
-        #[clap(long, default_value_t = format!(""))]
-        pb_message: String,
-        /// use deterministic seed for debugging purpose
-        #[clap(long, action)]
-        use_deterministic_seed: bool,
-        /// the benchmark profile output file path
-        #[clap(long)]
-        benchmark_profiler_output: Option<String>,
-        /// skip some iterations, useful when debugging
-        #[clap(long, default_value_t = 0)]
-        starting_iteration: usize,
-    },
+    Benchmark(BenchmarkParameters),
+    #[cfg(feature = "qecp_integrate")]
+    Qecp(qecp::cli::BenchmarkParameters),
     /// built-in tests
     Test {
         #[clap(subcommand)]
         command: TestCommands,
     },
 }
 
@@ -159,56 +155,64 @@
 
 /// note that these code type is only for example, to test and demonstrate the correctness of the algorithm, but not for real QEC simulation;
 /// for real simulation, please refer to <https://github.com/yuewuo/QEC-Playground>
 #[derive(Copy, Clone, PartialEq, Eq, PartialOrd, Ord, ValueEnum, Serialize, Debug)]
 pub enum ExampleCodeType {
     /// quantum repetition code with perfect stabilizer measurement
     CodeCapacityRepetitionCode,
-    /// quantum repetition code with phenomenological error model
+    /// quantum repetition code with phenomenological noise model
     PhenomenologicalRepetitionCode,
     /// quantum repetition code with circuit-level noise model
     CircuitLevelRepetitionCode,
     /// planar surface code with perfect stabilizer measurement
     CodeCapacityPlanarCode,
-    /// planar surface code with phenomenological error model
+    /// planar surface code with phenomenological noise model
     PhenomenologicalPlanarCode,
     /// parallel version
     PhenomenologicalPlanarCodeParallel,
     /// planar surface code with circuit-level noise model
     CircuitLevelPlanarCode,
     /// parallel version
     CircuitLevelPlanarCodeParallel,
     /// read from error pattern file, generated using option `--primal-dual-type error-pattern-logger`
     ErrorPatternReader,
+    /// rotated surface code with perfect stabilizer measurement
+    CodeCapacityRotatedCode,
+    /// rotated surface code with phenomenological noise model
+    PhenomenologicalRotatedCode,
 }
 
 #[derive(Copy, Clone, PartialEq, Eq, PartialOrd, Ord, ValueEnum, Serialize, Debug)]
 pub enum PartitionStrategy {
     /// no partition
     None,
     /// partition a planar code into top half and bottom half
     CodeCapacityPlanarCodeVerticalPartitionHalf,
     /// partition a planar code into 4 pieces: top left and right, bottom left and right
     CodeCapacityPlanarCodeVerticalPartitionFour,
     /// partition a repetition code into left and right half
     CodeCapacityRepetitionCodePartitionHalf,
     /// partition a phenomenological (or circuit-level) planar code with time axis
     PhenomenologicalPlanarCodeTimePartition,
+    /// partition a phenomenological (or circuit-level) rotated code with time axis
+    PhenomenologicalRotatedCodeTimePartition,
 }
 
 #[derive(Copy, Clone, PartialEq, Eq, PartialOrd, Ord, ValueEnum, Serialize, Debug)]
 pub enum PrimalDualType {
     /// serial primal and dual
     Serial,
     /// parallel dual and serial primal
     DualParallel,
     /// parallel primal and dual
     Parallel,
     /// log error into a file for later fetch
     ErrorPatternLogger,
+    /// solver using traditional blossom V
+    BlossomV,
 }
 
 #[derive(Copy, Clone, PartialEq, Eq, PartialOrd, Ord, ValueEnum, Serialize, Debug)]
 pub enum Verifier {
     /// disable verifier
     None,
     /// use blossom V library to verify the correctness of result
@@ -216,34 +220,62 @@
     /// use the serial version of fusion algorithm to verify the correctness of result
     FusionSerial,
 }
 
 impl Cli {
     pub fn run(self) {
         match self.command {
-            Commands::Benchmark { d, p, pe, noisy_measurements, max_half_weight, code_type, enable_visualizer, verifier, total_rounds, primal_dual_type
-                    , partition_strategy, pb_message, primal_dual_config, code_config, partition_config, use_deterministic_seed
-                    , benchmark_profiler_output, print_syndrome_pattern, starting_iteration } => {
+            Commands::Benchmark(BenchmarkParameters {
+                d,
+                p,
+                pe,
+                noisy_measurements,
+                max_half_weight,
+                code_type,
+                enable_visualizer,
+                verifier,
+                total_rounds,
+                primal_dual_type,
+                partition_strategy,
+                pb_message,
+                primal_dual_config,
+                code_config,
+                partition_config,
+                use_deterministic_seed,
+                benchmark_profiler_output,
+                print_syndrome_pattern,
+                starting_iteration,
+                ..
+            }) => {
+                let code_config: serde_json::Value = serde_json::from_str(&code_config).unwrap();
+                let primal_dual_config: serde_json::Value = serde_json::from_str(&primal_dual_config).unwrap();
+                let partition_config: serde_json::Value = serde_json::from_str(&partition_config).unwrap();
                 // check for dependency early
                 if matches!(verifier, Verifier::BlossomV) && cfg!(not(feature = "blossom_v")) {
                     panic!("need blossom V library, see README.md")
                 }
                 // whether to disable progress bar, useful when running jobs in background
                 let disable_progress_bar = env::var("DISABLE_PROGRESS_BAR").is_ok();
                 let mut code: Box<dyn ExampleCode> = code_type.build(d, p, noisy_measurements, max_half_weight, code_config);
-                if pe != 0. { code.set_erasure_probability(pe); }
-                if enable_visualizer {  // print visualizer file path only once
+                if pe != 0. {
+                    code.set_erasure_probability(pe);
+                }
+                if enable_visualizer {
+                    // print visualizer file path only once
                     print_visualize_link(static_visualize_data_filename());
                 }
                 // create initializer and solver
-                let (initializer, partition_config) = partition_strategy.build(&mut *code, d, noisy_measurements, partition_config);
+                let (initializer, partition_config) =
+                    partition_strategy.build(&mut *code, d, noisy_measurements, partition_config);
                 let partition_info = partition_config.info();
-                let mut primal_dual_solver = primal_dual_type.build(&initializer, &partition_info, &*code, primal_dual_config);
+                let mut primal_dual_solver =
+                    primal_dual_type.build(&initializer, &partition_info, &*code, primal_dual_config);
                 let mut result_verifier = verifier.build(&initializer);
-                let mut benchmark_profiler = BenchmarkProfiler::new(noisy_measurements, benchmark_profiler_output.map(|x| (x, &partition_info)));
+                let mut benchmark_profiler =
+                    BenchmarkProfiler::new(noisy_measurements, benchmark_profiler_output.map(|x| (x, &partition_info)));
                 // prepare progress bar display
                 let mut pb = if !disable_progress_bar {
                     let mut pb = ProgressBar::on(std::io::stderr(), total_rounds as u64);
                     pb.message(format!("{pb_message} ").as_str());
                     Some(pb)
                 } else {
                     if !pb_message.is_empty() {
@@ -258,215 +290,420 @@
                     let syndrome_pattern = code.generate_random_errors(seed);
                     if print_syndrome_pattern {
                         println!("syndrome_pattern: {:?}", syndrome_pattern);
                     }
                     // create a new visualizer each round
                     let mut visualizer = None;
                     if enable_visualizer {
-                        let new_visualizer = Visualizer::new(Some(visualize_data_folder() + static_visualize_data_filename().as_str())
-                            , code.get_positions(), true).unwrap();
+                        let new_visualizer = Visualizer::new(
+                            Some(visualize_data_folder() + static_visualize_data_filename().as_str()),
+                            code.get_positions(),
+                            true,
+                        )
+                        .unwrap();
                         visualizer = Some(new_visualizer);
                     }
                     benchmark_profiler.begin(&syndrome_pattern);
                     primal_dual_solver.solve_visualizer(&syndrome_pattern, visualizer.as_mut());
                     benchmark_profiler.event("decoded".to_string());
                     result_verifier.verify(&mut primal_dual_solver, &syndrome_pattern, visualizer.as_mut());
                     benchmark_profiler.event("verified".to_string());
-                    primal_dual_solver.clear();  // also count the clear operation
+                    primal_dual_solver.clear(); // also count the clear operation
                     benchmark_profiler.end(Some(&*primal_dual_solver));
                     if let Some(pb) = pb.as_mut() {
                         if pb_message.is_empty() {
                             pb.message(format!("{} ", benchmark_profiler.brief()).as_str());
                         }
                     }
                 }
-                if disable_progress_bar {  // always print out brief
+                if disable_progress_bar {
+                    // always print out brief
                     println!("{}", benchmark_profiler.brief());
                 } else {
-                    if let Some(pb) = pb.as_mut() { pb.finish() }
+                    if let Some(pb) = pb.as_mut() {
+                        pb.finish()
+                    }
                     println!();
                 }
-            },
+            }
             Commands::Test { command } => {
                 match command {
-                    TestCommands::Serial { print_command, enable_visualizer, disable_blossom, print_syndrome_pattern } => {
+                    TestCommands::Serial {
+                        print_command,
+                        enable_visualizer,
+                        disable_blossom,
+                        print_syndrome_pattern,
+                    } => {
                         let mut parameters = vec![];
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-repetition-code")
-                                    , format!("--pb-message"), format!("repetition {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-repetition-code"),
+                                    format!("--pb-message"),
+                                    format!("repetition {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-planar-code")
-                                    , format!("--pb-message"), format!("planar {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-planar-code"),
+                                    format!("--pb-message"),
+                                    format!("planar {d} {p}"),
+                                ]);
                             }
                         }
-                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {  // test erasures
+                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
+                            // test erasures
                             for d in [3, 7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-planar-code")
-                                    , format!("--pe"), format!("{p}")
-                                    , format!("--pb-message"), format!("mixed erasure planar {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-planar-code"),
+                                    format!("--pe"),
+                                    format!("{p}"),
+                                    format!("--pb-message"),
+                                    format!("mixed erasure planar {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("phenomenological-planar-code")
-                                    , format!("--noisy-measurements"), format!("{d}")
-                                    , format!("--pb-message"), format!("phenomenological {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("phenomenological-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{d}"),
+                                    format!("--pb-message"),
+                                    format!("phenomenological {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("circuit-level-planar-code")
-                                    , format!("--noisy-measurements"), format!("{d}")
-                                    , format!("--pb-message"), format!("circuit-level {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("circuit-level-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{d}"),
+                                    format!("--pb-message"),
+                                    format!("circuit-level {d} {p}"),
+                                ]);
                             }
                         }
                         let command_head = vec![format!(""), format!("benchmark")];
                         let mut command_tail = vec!["--total-rounds".to_string(), format!("{TEST_EACH_ROUNDS}")];
-                        if !disable_blossom { command_tail.append(&mut vec![format!("--verifier"), format!("blossom-v")]); }
-                        if enable_visualizer { command_tail.append(&mut vec![format!("--enable-visualizer")]); }
-                        if print_syndrome_pattern { command_tail.append(&mut vec![format!("--print-syndrome-pattern")]); }
+                        if !disable_blossom {
+                            command_tail.append(&mut vec![format!("--verifier"), format!("blossom-v")]);
+                        } else {
+                            command_tail.append(&mut vec![format!("--verifier"), format!("none")]);
+                        }
+                        if enable_visualizer {
+                            command_tail.append(&mut vec![format!("--enable-visualizer")]);
+                        }
+                        if print_syndrome_pattern {
+                            command_tail.append(&mut vec![format!("--print-syndrome-pattern")]);
+                        }
                         for parameter in parameters.iter() {
-                            execute_in_cli(command_head.iter().chain(parameter.iter()).chain(command_tail.iter()), print_command);
+                            execute_in_cli(
+                                command_head.iter().chain(parameter.iter()).chain(command_tail.iter()),
+                                print_command,
+                            );
                         }
-                    },
-                    TestCommands::DualParallel { print_command, enable_visualizer, disable_blossom, print_syndrome_pattern } => {
+                    }
+                    TestCommands::DualParallel {
+                        print_command,
+                        enable_visualizer,
+                        disable_blossom,
+                        print_syndrome_pattern,
+                    } => {
                         let mut parameters = vec![];
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-repetition-code")
-                                    , format!("--partition-strategy"), format!("code-capacity-repetition-code-partition-half")
-                                    , format!("--pb-message"), format!("dual-parallel 2-partition repetition {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-repetition-code"),
+                                    format!("--partition-strategy"),
+                                    format!("code-capacity-repetition-code-partition-half"),
+                                    format!("--pb-message"),
+                                    format!("dual-parallel 2-partition repetition {d} {p}"),
+                                ]);
                             }
                         }
-                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {  // simple partition into top and bottom
+                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
+                            // simple partition into top and bottom
                             for d in [7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-planar-code")
-                                    , format!("--partition-strategy"), format!("code-capacity-planar-code-vertical-partition-half")
-                                    , format!("--pb-message"), format!("dual-parallel 2-partition planar {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-planar-code"),
+                                    format!("--partition-strategy"),
+                                    format!("code-capacity-planar-code-vertical-partition-half"),
+                                    format!("--pb-message"),
+                                    format!("dual-parallel 2-partition planar {d} {p}"),
+                                ]);
                             }
                         }
-                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {  // complex partition into 4 blocks
+                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
+                            // complex partition into 4 blocks
                             for d in [7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-planar-code")
-                                    , format!("--partition-strategy"), format!("code-capacity-planar-code-vertical-partition-four")
-                                    , format!("--pb-message"), format!("dual-parallel 4-partition planar {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-planar-code"),
+                                    format!("--partition-strategy"),
+                                    format!("code-capacity-planar-code-vertical-partition-four"),
+                                    format!("--pb-message"),
+                                    format!("dual-parallel 4-partition planar {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("phenomenological-planar-code")
-                                    , format!("--noisy-measurements"), format!("{d}")
-                                    , format!("--partition-strategy"), format!("phenomenological-planar-code-time-partition")
-                                    , format!("--partition-config"), "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string()
-                                    , format!("--pb-message"), format!("dual-parallel 2-partition phenomenological {d} {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("phenomenological-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{d}"),
+                                    format!("--partition-strategy"),
+                                    format!("phenomenological-planar-code-time-partition"),
+                                    format!("--partition-config"),
+                                    "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string(),
+                                    format!("--pb-message"),
+                                    format!("dual-parallel 2-partition phenomenological {d} {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("circuit-level-planar-code")
-                                    , format!("--noisy-measurements"), format!("{d}")
-                                    , format!("--partition-strategy"), format!("phenomenological-planar-code-time-partition")
-                                    , format!("--partition-config"), "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string()
-                                    , format!("--pb-message"), format!("dual-parallel 2-partition circuit-level {d} {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("circuit-level-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{d}"),
+                                    format!("--partition-strategy"),
+                                    format!("phenomenological-planar-code-time-partition"),
+                                    format!("--partition-config"),
+                                    "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string(),
+                                    format!("--pb-message"),
+                                    format!("dual-parallel 2-partition circuit-level {d} {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
-                            for partition_num in [2, 3, 4, 5, 6, 7, 8, 9, 10] {  // test large number of fusion without tree fusion
+                            for partition_num in [2, 3, 4, 5, 6, 7, 8, 9, 10] {
+                                // test large number of fusion without tree fusion
                                 let d = 5;
                                 let noisy_measurement = 20;
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("circuit-level-planar-code")
-                                    , format!("--noisy-measurements"), format!("{noisy_measurement}")
-                                    , format!("--partition-strategy"), format!("phenomenological-planar-code-time-partition")
-                                    , format!("--partition-config"), format!("{{\"partition_num\":{partition_num},\"enable_tree_fusion\":false}}")
-                                    , format!("--pb-message"), format!("dual-parallel {partition_num}-partition circuit-level {d} {noisy_measurement} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("circuit-level-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{noisy_measurement}"),
+                                    format!("--partition-strategy"),
+                                    format!("phenomenological-planar-code-time-partition"),
+                                    format!("--partition-config"),
+                                    format!("{{\"partition_num\":{partition_num},\"enable_tree_fusion\":false}}"),
+                                    format!("--pb-message"),
+                                    format!(
+                                        "dual-parallel {partition_num}-partition circuit-level {d} {noisy_measurement} {p}"
+                                    ),
+                                ]);
                             }
                         }
                         let command_head = vec![format!(""), format!("benchmark")];
-                        let mut command_tail = vec![format!("--primal-dual-type"), format!("dual-parallel")
-                            , "--total-rounds".to_string(), format!("{TEST_EACH_ROUNDS}")];
-                        if !disable_blossom { command_tail.append(&mut vec![format!("--verifier"), format!("blossom-v")]); }
-                        if enable_visualizer { command_tail.append(&mut vec![format!("--enable-visualizer")]); }
-                        if print_syndrome_pattern { command_tail.append(&mut vec![format!("--print-syndrome-pattern")]); }
+                        let mut command_tail = vec![
+                            format!("--primal-dual-type"),
+                            format!("dual-parallel"),
+                            "--total-rounds".to_string(),
+                            format!("{TEST_EACH_ROUNDS}"),
+                        ];
+                        if !disable_blossom {
+                            command_tail.append(&mut vec![format!("--verifier"), format!("blossom-v")]);
+                        } else {
+                            command_tail.append(&mut vec![format!("--verifier"), format!("none")]);
+                        }
+                        if enable_visualizer {
+                            command_tail.append(&mut vec![format!("--enable-visualizer")]);
+                        }
+                        if print_syndrome_pattern {
+                            command_tail.append(&mut vec![format!("--print-syndrome-pattern")]);
+                        }
                         for parameter in parameters.iter() {
-                            execute_in_cli(command_head.iter().chain(parameter.iter()).chain(command_tail.iter()), print_command);
+                            execute_in_cli(
+                                command_head.iter().chain(parameter.iter()).chain(command_tail.iter()),
+                                print_command,
+                            );
                         }
-                    },
-                    TestCommands::Parallel { print_command, enable_visualizer, disable_blossom, print_syndrome_pattern } => {
+                    }
+                    TestCommands::Parallel {
+                        print_command,
+                        enable_visualizer,
+                        disable_blossom,
+                        print_syndrome_pattern,
+                    } => {
                         let mut parameters = vec![];
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-repetition-code")
-                                    , format!("--partition-strategy"), format!("code-capacity-repetition-code-partition-half")
-                                    , format!("--pb-message"), format!("parallel 2-partition repetition {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-repetition-code"),
+                                    format!("--partition-strategy"),
+                                    format!("code-capacity-repetition-code-partition-half"),
+                                    format!("--pb-message"),
+                                    format!("parallel 2-partition repetition {d} {p}"),
+                                ]);
                             }
                         }
-                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {  // simple partition into top and bottom
+                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
+                            // simple partition into top and bottom
                             for d in [7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-planar-code")
-                                    , format!("--partition-strategy"), format!("code-capacity-planar-code-vertical-partition-half")
-                                    , format!("--pb-message"), format!("parallel 2-partition planar {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-planar-code"),
+                                    format!("--partition-strategy"),
+                                    format!("code-capacity-planar-code-vertical-partition-half"),
+                                    format!("--pb-message"),
+                                    format!("parallel 2-partition planar {d} {p}"),
+                                ]);
                             }
                         }
-                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {  // complex partition into 4 blocks
+                        for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
+                            // complex partition into 4 blocks
                             for d in [7, 11, 15, 19] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("code-capacity-planar-code")
-                                    , format!("--partition-strategy"), format!("code-capacity-planar-code-vertical-partition-four")
-                                    , format!("--pb-message"), format!("parallel 4-partition planar {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("code-capacity-planar-code"),
+                                    format!("--partition-strategy"),
+                                    format!("code-capacity-planar-code-vertical-partition-four"),
+                                    format!("--pb-message"),
+                                    format!("parallel 4-partition planar {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("phenomenological-planar-code")
-                                    , format!("--noisy-measurements"), format!("{d}")
-                                    , format!("--partition-strategy"), format!("phenomenological-planar-code-time-partition")
-                                    , format!("--partition-config"), "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string()
-                                    , format!("--pb-message"), format!("parallel 2-partition phenomenological {d} {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("phenomenological-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{d}"),
+                                    format!("--partition-strategy"),
+                                    format!("phenomenological-planar-code-time-partition"),
+                                    format!("--partition-config"),
+                                    "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string(),
+                                    format!("--pb-message"),
+                                    format!("parallel 2-partition phenomenological {d} {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
                             for d in [3, 7, 11] {
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("circuit-level-planar-code")
-                                    , format!("--noisy-measurements"), format!("{d}")
-                                    , format!("--partition-strategy"), format!("phenomenological-planar-code-time-partition")
-                                    , format!("--partition-config"), "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string()
-                                    , format!("--pb-message"), format!("parallel 2-partition circuit-level {d} {d} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("circuit-level-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{d}"),
+                                    format!("--partition-strategy"),
+                                    format!("phenomenological-planar-code-time-partition"),
+                                    format!("--partition-config"),
+                                    "{\"partition_num\":2,\"enable_tree_fusion\":true}".to_string(),
+                                    format!("--pb-message"),
+                                    format!("parallel 2-partition circuit-level {d} {d} {p}"),
+                                ]);
                             }
                         }
                         for p in [0.001, 0.003, 0.01, 0.03, 0.1, 0.3, 0.499] {
-                            for partition_num in [2, 3, 4, 5, 6, 7, 8, 9, 10] {  // test large number of fusion without tree fusion
+                            for partition_num in [2, 3, 4, 5, 6, 7, 8, 9, 10] {
+                                // test large number of fusion without tree fusion
                                 let d = 5;
                                 let noisy_measurement = 20;
-                                parameters.push(vec![format!("{d}"), format!("{p}"), format!("--code-type"), format!("circuit-level-planar-code")
-                                    , format!("--noisy-measurements"), format!("{noisy_measurement}")
-                                    , format!("--partition-strategy"), format!("phenomenological-planar-code-time-partition")
-                                    , format!("--partition-config"), format!("{{\"partition_num\":{partition_num},\"enable_tree_fusion\":false}}")
-                                    , format!("--pb-message"), format!("parallel {partition_num}-partition circuit-level {d} {noisy_measurement} {p}")]);
+                                parameters.push(vec![
+                                    format!("{d}"),
+                                    format!("{p}"),
+                                    format!("--code-type"),
+                                    format!("circuit-level-planar-code"),
+                                    format!("--noisy-measurements"),
+                                    format!("{noisy_measurement}"),
+                                    format!("--partition-strategy"),
+                                    format!("phenomenological-planar-code-time-partition"),
+                                    format!("--partition-config"),
+                                    format!("{{\"partition_num\":{partition_num},\"enable_tree_fusion\":false}}"),
+                                    format!("--pb-message"),
+                                    format!("parallel {partition_num}-partition circuit-level {d} {noisy_measurement} {p}"),
+                                ]);
                             }
                         }
                         let command_head = vec![format!(""), format!("benchmark")];
-                        let mut command_tail = vec![format!("--primal-dual-type"), format!("parallel")
-                            , "--total-rounds".to_string(), format!("{TEST_EACH_ROUNDS}")];
-                        if !disable_blossom { command_tail.append(&mut vec![format!("--verifier"), format!("blossom-v")]); }
-                        if enable_visualizer { command_tail.append(&mut vec![format!("--enable-visualizer")]); }
-                        if print_syndrome_pattern { command_tail.append(&mut vec![format!("--print-syndrome-pattern")]); }
+                        let mut command_tail = vec![
+                            format!("--primal-dual-type"),
+                            format!("parallel"),
+                            "--total-rounds".to_string(),
+                            format!("{TEST_EACH_ROUNDS}"),
+                        ];
+                        if !disable_blossom {
+                            command_tail.append(&mut vec![format!("--verifier"), format!("blossom-v")]);
+                        } else {
+                            command_tail.append(&mut vec![format!("--verifier"), format!("none")]);
+                        }
+                        if enable_visualizer {
+                            command_tail.append(&mut vec![format!("--enable-visualizer")]);
+                        }
+                        if print_syndrome_pattern {
+                            command_tail.append(&mut vec![format!("--print-syndrome-pattern")]);
+                        }
                         for parameter in parameters.iter() {
-                            execute_in_cli(command_head.iter().chain(parameter.iter()).chain(command_tail.iter()), print_command);
+                            execute_in_cli(
+                                command_head.iter().chain(parameter.iter()).chain(command_tail.iter()),
+                                print_command,
+                            );
                         }
-                    },
+                    }
                 }
-            },
+            }
+            #[cfg(feature = "qecp_integrate")]
+            Commands::Qecp(benchmark_parameters) => {
+                benchmark_parameters.run().unwrap();
+            }
         }
     }
 }
 
-pub fn execute_in_cli<'a>(iter: impl Iterator<Item=&'a String> + Clone, print_command: bool) {
+pub fn execute_in_cli<'a>(iter: impl Iterator<Item = &'a String> + Clone, print_command: bool) {
     if print_command {
         print!("[command]");
         for word in iter.clone() {
             if word.contains(char::is_whitespace) {
                 print!("'{word}' ")
             } else {
                 print!("{word} ")
@@ -474,187 +711,284 @@
         }
         println!();
     }
     Cli::parse_from(iter).run();
 }
 
 impl ExampleCodeType {
-    fn build(&self, d: VertexNum, p: f64, noisy_measurements: VertexNum, max_half_weight: Weight, mut code_config: serde_json::Value) -> Box<dyn ExampleCode> {
+    fn build(
+        &self,
+        d: VertexNum,
+        p: f64,
+        noisy_measurements: VertexNum,
+        max_half_weight: Weight,
+        mut code_config: serde_json::Value,
+    ) -> Box<dyn ExampleCode> {
         match self {
             Self::CodeCapacityRepetitionCode => {
                 assert_eq!(code_config, json!({}), "config not supported");
                 Box::new(CodeCapacityRepetitionCode::new(d, p, max_half_weight))
-            },
+            }
             Self::CodeCapacityPlanarCode => {
                 assert_eq!(code_config, json!({}), "config not supported");
                 Box::new(CodeCapacityPlanarCode::new(d, p, max_half_weight))
-            },
+            }
             Self::PhenomenologicalPlanarCode => {
                 assert_eq!(code_config, json!({}), "config not supported");
                 Box::new(PhenomenologicalPlanarCode::new(d, noisy_measurements, p, max_half_weight))
-            },
+            }
             Self::PhenomenologicalPlanarCodeParallel => {
                 let mut code_count = 1;
                 let config = code_config.as_object_mut().expect("config must be JSON object");
                 if let Some(value) = config.remove("code_count") {
                     code_count = value.as_u64().expect("code_count number") as usize;
                 }
-                Box::new(ExampleCodeParallel::new(PhenomenologicalPlanarCode::new(d, noisy_measurements, p, max_half_weight), code_count))
-            },
+                Box::new(ExampleCodeParallel::new(
+                    PhenomenologicalPlanarCode::new(d, noisy_measurements, p, max_half_weight),
+                    code_count,
+                ))
+            }
             Self::CircuitLevelPlanarCode => {
                 assert_eq!(code_config, json!({}), "config not supported");
                 Box::new(CircuitLevelPlanarCode::new(d, noisy_measurements, p, max_half_weight))
-            },
+            }
             Self::CircuitLevelPlanarCodeParallel => {
                 let mut code_count = 1;
                 let config = code_config.as_object_mut().expect("config must be JSON object");
                 if let Some(value) = config.remove("code_count") {
                     code_count = value.as_u64().expect("code_count number") as usize;
                 }
-                Box::new(ExampleCodeParallel::new(CircuitLevelPlanarCode::new(d, noisy_measurements, p, max_half_weight), code_count))
-            },
-            Self::ErrorPatternReader => {
-                Box::new(ErrorPatternReader::new(code_config))
-            },
-            _ => unimplemented!()
+                Box::new(ExampleCodeParallel::new(
+                    CircuitLevelPlanarCode::new(d, noisy_measurements, p, max_half_weight),
+                    code_count,
+                ))
+            }
+            Self::ErrorPatternReader => Box::new(ErrorPatternReader::new(code_config)),
+            Self::CodeCapacityRotatedCode => {
+                assert_eq!(code_config, json!({}), "config not supported");
+                Box::new(CodeCapacityRotatedCode::new(d, p, max_half_weight))
+            }
+            Self::PhenomenologicalRotatedCode => {
+                assert_eq!(code_config, json!({}), "config not supported");
+                Box::new(PhenomenologicalRotatedCode::new(d, noisy_measurements, p, max_half_weight))
+            }
+            _ => unimplemented!(),
         }
     }
 }
 
 impl PartitionStrategy {
-    fn build(&self, code: &mut dyn ExampleCode, d: VertexNum, noisy_measurements: VertexNum, mut partition_config: serde_json::Value) -> (SolverInitializer, PartitionConfig) {
+    fn build(
+        &self,
+        code: &mut dyn ExampleCode,
+        d: VertexNum,
+        noisy_measurements: VertexNum,
+        mut partition_config: serde_json::Value,
+    ) -> (SolverInitializer, PartitionConfig) {
         use example_partition::*;
         let partition_config = match self {
             Self::None => {
                 assert_eq!(partition_config, json!({}), "config not supported");
                 NoPartition::new().build_apply(code)
-            },
+            }
             Self::CodeCapacityPlanarCodeVerticalPartitionHalf => {
                 assert_eq!(partition_config, json!({}), "config not supported");
                 CodeCapacityPlanarCodeVerticalPartitionHalf::new(d, d / 2).build_apply(code)
-            },
+            }
             Self::CodeCapacityPlanarCodeVerticalPartitionFour => {
                 assert_eq!(partition_config, json!({}), "config not supported");
                 CodeCapacityPlanarCodeVerticalPartitionFour::new(d, d / 2, d / 2).build_apply(code)
-            },
+            }
             Self::CodeCapacityRepetitionCodePartitionHalf => {
                 assert_eq!(partition_config, json!({}), "config not supported");
                 CodeCapacityRepetitionCodePartitionHalf::new(d, d / 2).build_apply(code)
-            },
+            }
             Self::PhenomenologicalPlanarCodeTimePartition => {
                 let config = partition_config.as_object_mut().expect("config must be JSON object");
                 let mut partition_num = 10;
                 let mut enable_tree_fusion = false;
                 let mut maximum_tree_leaf_size = usize::MAX;
                 if let Some(value) = config.remove("partition_num") {
                     partition_num = value.as_u64().expect("partition_num: usize") as usize;
                 }
                 if let Some(value) = config.remove("enable_tree_fusion") {
                     enable_tree_fusion = value.as_bool().expect("enable_tree_fusion: bool");
                 }
                 if let Some(value) = config.remove("maximum_tree_leaf_size") {
                     maximum_tree_leaf_size = value.as_u64().expect("maximum_tree_leaf_size: usize") as usize;
                 }
-                if !config.is_empty() { panic!("unknown config keys: {:?}", config.keys().collect::<Vec<&String>>()); }
-                PhenomenologicalPlanarCodeTimePartition::new_tree(d, noisy_measurements, partition_num
-                        , enable_tree_fusion, maximum_tree_leaf_size).build_apply(code)
-            },
+                if !config.is_empty() {
+                    panic!("unknown config keys: {:?}", config.keys().collect::<Vec<&String>>());
+                }
+                PhenomenologicalPlanarCodeTimePartition::new_tree(
+                    d,
+                    noisy_measurements,
+                    partition_num,
+                    enable_tree_fusion,
+                    maximum_tree_leaf_size,
+                )
+                .build_apply(code)
+            }
+            Self::PhenomenologicalRotatedCodeTimePartition => {
+                let config = partition_config.as_object_mut().expect("config must be JSON object");
+                let mut partition_num = 10;
+                let mut enable_tree_fusion = false;
+                let mut maximum_tree_leaf_size = usize::MAX;
+                if let Some(value) = config.remove("partition_num") {
+                    partition_num = value.as_u64().expect("partition_num: usize") as usize;
+                }
+                if let Some(value) = config.remove("enable_tree_fusion") {
+                    enable_tree_fusion = value.as_bool().expect("enable_tree_fusion: bool");
+                }
+                if let Some(value) = config.remove("maximum_tree_leaf_size") {
+                    maximum_tree_leaf_size = value.as_u64().expect("maximum_tree_leaf_size: usize") as usize;
+                }
+                if !config.is_empty() {
+                    panic!("unknown config keys: {:?}", config.keys().collect::<Vec<&String>>());
+                }
+                PhenomenologicalRotatedCodeTimePartition::new_tree(
+                    d,
+                    noisy_measurements,
+                    partition_num,
+                    enable_tree_fusion,
+                    maximum_tree_leaf_size,
+                )
+                .build_apply(code)
+            }
         };
         (code.get_initializer(), partition_config)
     }
 }
 
 impl PrimalDualType {
-    fn build(&self, initializer: &SolverInitializer, partition_info: &PartitionInfo, code: &dyn ExampleCode
-            , primal_dual_config: serde_json::Value) -> Box<dyn PrimalDualSolver> {
+    fn build(
+        &self,
+        initializer: &SolverInitializer,
+        partition_info: &PartitionInfo,
+        code: &dyn ExampleCode,
+        primal_dual_config: serde_json::Value,
+    ) -> Box<dyn PrimalDualSolver> {
         match self {
             Self::Serial => {
                 assert_eq!(primal_dual_config, json!({}));
-                assert_eq!(partition_info.config.partitions.len(), 1, "no partition is supported by serial algorithm, consider using other primal-dual-type");
+                assert_eq!(
+                    partition_info.config.partitions.len(),
+                    1,
+                    "no partition is supported by serial algorithm, consider using other primal-dual-type"
+                );
                 Box::new(SolverSerial::new(initializer))
-            },
-            Self::DualParallel => {
-                Box::new(SolverDualParallel::new(initializer, partition_info, primal_dual_config))
-            },
-            Self::Parallel => {
-                Box::new(SolverParallel::new(initializer, partition_info, primal_dual_config))
-            },
-            Self::ErrorPatternLogger => {
-                Box::new(SolverErrorPatternLogger::new(initializer, code, primal_dual_config))
-            },
+            }
+            Self::DualParallel => Box::new(SolverDualParallel::new(initializer, partition_info, primal_dual_config)),
+            Self::Parallel => Box::new(SolverParallel::new(initializer, partition_info, primal_dual_config)),
+            Self::ErrorPatternLogger => Box::new(SolverErrorPatternLogger::new(
+                initializer,
+                &code.get_positions(),
+                primal_dual_config,
+            )),
+            Self::BlossomV => Box::new(SolverBlossomV::new(initializer)),
         }
     }
 }
 
 impl Verifier {
     fn build(&self, initializer: &SolverInitializer) -> Box<dyn ResultVerifier> {
         match self {
-            Self::None => Box::new(VerifierNone { }),
-            Self::BlossomV => Box::new(VerifierBlossomV { 
+            Self::None => Box::new(VerifierNone {}),
+            Self::BlossomV => Box::new(VerifierBlossomV {
                 initializer: initializer.clone(),
                 subgraph_builder: SubGraphBuilder::new(initializer),
             }),
-            _ => unimplemented!()
+            _ => unimplemented!(),
         }
     }
 }
 
 trait ResultVerifier {
-    fn verify(&mut self, primal_dual_solver: &mut Box<dyn PrimalDualSolver>, syndrome_pattern: &SyndromePattern, visualizer: Option<&mut Visualizer>);
+    fn verify(
+        &mut self,
+        primal_dual_solver: &mut Box<dyn PrimalDualSolver>,
+        syndrome_pattern: &SyndromePattern,
+        visualizer: Option<&mut Visualizer>,
+    );
 }
 
-struct VerifierNone { }
+struct VerifierNone {}
 
 impl ResultVerifier for VerifierNone {
-    fn verify(&mut self, _primal_dual_solver: &mut Box<dyn PrimalDualSolver>, _syndrome_pattern: &SyndromePattern, _visualizer: Option<&mut Visualizer>) { }
+    fn verify(
+        &mut self,
+        _primal_dual_solver: &mut Box<dyn PrimalDualSolver>,
+        _syndrome_pattern: &SyndromePattern,
+        _visualizer: Option<&mut Visualizer>,
+    ) {
+    }
 }
 
 struct VerifierBlossomV {
     initializer: SolverInitializer,
     subgraph_builder: SubGraphBuilder,
 }
 
 impl ResultVerifier for VerifierBlossomV {
-    fn verify(&mut self, primal_dual_solver: &mut Box<dyn PrimalDualSolver>, syndrome_pattern: &SyndromePattern, visualizer: Option<&mut Visualizer>) {
+    #[allow(clippy::unnecessary_cast)]
+    fn verify(
+        &mut self,
+        primal_dual_solver: &mut Box<dyn PrimalDualSolver>,
+        syndrome_pattern: &SyndromePattern,
+        visualizer: Option<&mut Visualizer>,
+    ) {
         // prepare modified weighted edges
         let mut edge_modifier = EdgeWeightModifier::new();
         for edge_index in syndrome_pattern.erasures.iter() {
             let (vertex_idx_1, vertex_idx_2, original_weight) = &self.initializer.weighted_edges[*edge_index as usize];
             edge_modifier.push_modified_edge(*edge_index, *original_weight);
             self.initializer.weighted_edges[*edge_index as usize] = (*vertex_idx_1, *vertex_idx_2, 0);
         }
         // use blossom V to compute ground truth
-        let blossom_mwpm_result = fusion_blossom::blossom_v_mwpm(&self.initializer, &syndrome_pattern.defect_vertices);
-        let blossom_details = fusion_blossom::detailed_matching(&self.initializer, &syndrome_pattern.defect_vertices, &blossom_mwpm_result);
+        let blossom_mwpm_result = super::blossom_v_mwpm(&self.initializer, &syndrome_pattern.defect_vertices);
+        let blossom_details =
+            super::detailed_matching(&self.initializer, &syndrome_pattern.defect_vertices, &blossom_mwpm_result);
         let mut blossom_total_weight = 0;
         for detail in blossom_details.iter() {
             blossom_total_weight += detail.weight;
         }
         // if blossom_total_weight > 0 { println!("w {} {}", primal_dual_solver.sum_dual_variables(), blossom_total_weight); }
-        assert_eq!(primal_dual_solver.sum_dual_variables(), blossom_total_weight, "unexpected final dual variable sum");
+        assert_eq!(
+            primal_dual_solver.sum_dual_variables(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
         // also construct the perfect matching from fusion blossom to compare them
         let fusion_mwpm = primal_dual_solver.perfect_matching();
         let fusion_mwpm_result = fusion_mwpm.legacy_get_mwpm_result(syndrome_pattern.defect_vertices.clone());
-        let fusion_details = fusion_blossom::detailed_matching(&self.initializer, &syndrome_pattern.defect_vertices, &fusion_mwpm_result);
+        let fusion_details =
+            super::detailed_matching(&self.initializer, &syndrome_pattern.defect_vertices, &fusion_mwpm_result);
         let mut fusion_total_weight = 0;
         for detail in fusion_details.iter() {
             fusion_total_weight += detail.weight;
         }
         // compare with ground truth from the blossom V algorithm
-        assert_eq!(fusion_total_weight, blossom_total_weight, "unexpected final dual variable sum");
+        assert_eq!(
+            fusion_total_weight, blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
         // recover those weighted_edges
         while edge_modifier.has_modified_edges() {
             let (edge_index, original_weight) = edge_modifier.pop_modified_edge();
             let (vertex_idx_1, vertex_idx_2, _) = &self.initializer.weighted_edges[edge_index as usize];
             self.initializer.weighted_edges[edge_index as usize] = (*vertex_idx_1, *vertex_idx_2, original_weight);
         }
         // also test subgraph builder
         self.subgraph_builder.clear();
         self.subgraph_builder.load_erasures(&syndrome_pattern.erasures);
         self.subgraph_builder.load_perfect_matching(&fusion_mwpm);
         // println!("blossom_total_weight: {blossom_total_weight} = {} = {fusion_total_weight}", self.subgraph_builder.total_weight());
-        assert_eq!(self.subgraph_builder.total_weight(), blossom_total_weight, "unexpected final dual variable sum");
+        assert_eq!(
+            self.subgraph_builder.total_weight(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
         if visualizer.is_some() {
             primal_dual_solver.subgraph_visualizer(visualizer);
         }
     }
 }
```

### Comparing `fusion_blossom-0.2.2/src/pointers.rs` & `fusion_blossom-0.2.5/src/pointers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 //! Pointer Types
-//! 
+//!
 //! Since fusion blossom requires no synchronization with mutex, it's inefficient to wrap everything in a mutex.
 //! At the same time, I want to enjoy the safety check provided by Rust compiler, so I want to limit unsafe code to minimum.
 //! The solution is to write everything in safe Rust, and debug them.
 //! After this, one can enable the feature `unsafe_pointer` to remove the unnecessary locks, thus improving the performance.
-//! 
+//!
 
-
-use std::sync::{Arc, Weak};
-use crate::parking_lot::{RwLock, RawRwLock};
-use crate::parking_lot::lock_api::{RwLockReadGuard, RwLockWriteGuard};
 use super::util::*;
-
+use crate::parking_lot::lock_api::{RwLockReadGuard, RwLockWriteGuard};
+use crate::parking_lot::{RawRwLock, RwLock};
+use std::sync::{Arc, Weak};
 
 /// allows fast reset of vector of objects without iterating over all objects each time: dynamically clear it
 pub trait FastClear {
-
     /// user provided method to actually clear the fields
     fn hard_clear(&mut self);
 
     /// get timestamp
     fn get_timestamp(&self) -> FastClearTimestamp;
 
     /// set timestamp
@@ -33,48 +30,53 @@
             self.set_timestamp(active_timestamp);
         }
     }
 
     /// when debugging your program, you can put this function every time you obtained a lock of a new object
     #[inline(always)]
     fn debug_assert_dynamic_cleared(&self, active_timestamp: FastClearTimestamp) {
-        debug_assert!(self.get_timestamp() == active_timestamp, "bug detected: not dynamically cleared, expected timestamp: {}, current timestamp: {}"
-            , active_timestamp, self.get_timestamp());
+        debug_assert!(
+            self.get_timestamp() == active_timestamp,
+            "bug detected: not dynamically cleared, expected timestamp: {}, current timestamp: {}",
+            active_timestamp,
+            self.get_timestamp()
+        );
     }
-
 }
 
-pub trait FastClearRwLockPtr<ObjType> where ObjType: FastClear {
-
+pub trait FastClearRwLockPtr<ObjType>
+where
+    ObjType: FastClear,
+{
     fn new_ptr(ptr: Arc<RwLock<ObjType>>) -> Self;
 
     fn new_value(obj: ObjType) -> Self;
 
     fn ptr(&self) -> &Arc<RwLock<ObjType>>;
 
     fn ptr_mut(&mut self) -> &mut Arc<RwLock<ObjType>>;
 
     #[inline(always)]
     fn read_recursive(&self, active_timestamp: FastClearTimestamp) -> RwLockReadGuard<RawRwLock, ObjType> {
         let ret = self.ptr().read_recursive();
-        ret.debug_assert_dynamic_cleared(active_timestamp);  // only assert during debug modes
+        ret.debug_assert_dynamic_cleared(active_timestamp); // only assert during debug modes
         ret
     }
 
-    /// without sanity check: this data might be outdated, so only use when you're read those immutable fields 
+    /// without sanity check: this data might be outdated, so only use when you're read those immutable fields
     #[inline(always)]
     fn read_recursive_force(&self) -> RwLockReadGuard<RawRwLock, ObjType> {
         let ret = self.ptr().read_recursive();
         ret
     }
 
     #[inline(always)]
     fn write(&self, active_timestamp: FastClearTimestamp) -> RwLockWriteGuard<RawRwLock, ObjType> {
         let ret = self.ptr().write();
-        ret.debug_assert_dynamic_cleared(active_timestamp);  // only assert during debug modes
+        ret.debug_assert_dynamic_cleared(active_timestamp); // only assert during debug modes
         ret
     }
 
     /// without sanity check: useful only in implementing hard_clear
     #[inline(always)]
     fn write_force(&self) -> RwLockWriteGuard<RawRwLock, ObjType> {
         let ret = self.ptr().write();
@@ -87,19 +89,17 @@
         let mut value = self.write_force();
         value.dynamic_clear(active_timestamp);
     }
 
     fn ptr_eq(&self, other: &Self) -> bool {
         Arc::ptr_eq(self.ptr(), other.ptr())
     }
-
 }
 
 pub trait RwLockPtr<ObjType> {
-
     fn new_ptr(ptr: Arc<RwLock<ObjType>>) -> Self;
 
     fn new_value(obj: ObjType) -> Self;
 
     fn ptr(&self) -> &Arc<RwLock<ObjType>>;
 
     fn ptr_mut(&mut self) -> &mut Arc<RwLock<ObjType>>;
@@ -115,74 +115,87 @@
         let ret = self.ptr().write();
         ret
     }
 
     fn ptr_eq(&self, other: &Self) -> bool {
         Arc::ptr_eq(self.ptr(), other.ptr())
     }
-
 }
 
 pub struct ArcRwLock<T> {
     ptr: Arc<RwLock<T>>,
 }
 
 pub struct WeakRwLock<T> {
     ptr: Weak<RwLock<T>>,
 }
 
 impl<T> ArcRwLock<T> {
     pub fn downgrade(&self) -> WeakRwLock<T> {
         WeakRwLock::<T> {
-            ptr: Arc::downgrade(&self.ptr)
+            ptr: Arc::downgrade(&self.ptr),
         }
     }
 }
 
 impl<T> WeakRwLock<T> {
     pub fn upgrade_force(&self) -> ArcRwLock<T> {
         ArcRwLock::<T> {
-            ptr: self.ptr.upgrade().unwrap()
+            ptr: self.ptr.upgrade().unwrap(),
         }
     }
     pub fn upgrade(&self) -> Option<ArcRwLock<T>> {
         self.ptr.upgrade().map(|x| ArcRwLock::<T> { ptr: x })
     }
 }
 
 impl<T> Clone for ArcRwLock<T> {
     fn clone(&self) -> Self {
         Self::new_ptr(Arc::clone(self.ptr()))
     }
 }
 
 impl<T> RwLockPtr<T> for ArcRwLock<T> {
-    fn new_ptr(ptr: Arc<RwLock<T>>) -> Self { Self { ptr }  }
-    fn new_value(obj: T) -> Self { Self::new_ptr(Arc::new(RwLock::new(obj))) }
-    #[inline(always)] fn ptr(&self) -> &Arc<RwLock<T>> { &self.ptr }
-    #[inline(always)] fn ptr_mut(&mut self) -> &mut Arc<RwLock<T>> { &mut self.ptr }
+    fn new_ptr(ptr: Arc<RwLock<T>>) -> Self {
+        Self { ptr }
+    }
+    fn new_value(obj: T) -> Self {
+        Self::new_ptr(Arc::new(RwLock::new(obj)))
+    }
+    #[inline(always)]
+    fn ptr(&self) -> &Arc<RwLock<T>> {
+        &self.ptr
+    }
+    #[inline(always)]
+    fn ptr_mut(&mut self) -> &mut Arc<RwLock<T>> {
+        &mut self.ptr
+    }
 }
 
 impl<T> PartialEq for ArcRwLock<T> {
-    fn eq(&self, other: &Self) -> bool { self.ptr_eq(other) }
+    fn eq(&self, other: &Self) -> bool {
+        self.ptr_eq(other)
+    }
 }
 
-impl<T> Eq for ArcRwLock<T> { }
+impl<T> Eq for ArcRwLock<T> {}
 
 impl<T> Clone for WeakRwLock<T> {
     fn clone(&self) -> Self {
         Self { ptr: self.ptr.clone() }
     }
 }
 
 impl<T> PartialEq for WeakRwLock<T> {
-    fn eq(&self, other: &Self) -> bool { self.ptr.ptr_eq(&other.ptr) }
+    fn eq(&self, other: &Self) -> bool {
+        self.ptr.ptr_eq(&other.ptr)
+    }
 }
 
-impl<T> Eq for WeakRwLock<T> { }
+impl<T> Eq for WeakRwLock<T> {}
 
 impl<T> std::ops::Deref for ArcRwLock<T> {
     type Target = RwLock<T>;
     fn deref(&self) -> &Self::Target {
         &self.ptr
     }
 }
@@ -207,60 +220,74 @@
 pub struct FastClearWeakRwLock<T: FastClear> {
     ptr: Weak<RwLock<T>>,
 }
 
 impl<T: FastClear> FastClearArcRwLock<T> {
     pub fn downgrade(&self) -> FastClearWeakRwLock<T> {
         FastClearWeakRwLock::<T> {
-            ptr: Arc::downgrade(&self.ptr)
+            ptr: Arc::downgrade(&self.ptr),
         }
     }
 }
 
 impl<T: FastClear> FastClearWeakRwLock<T> {
     pub fn upgrade_force(&self) -> FastClearArcRwLock<T> {
         FastClearArcRwLock::<T> {
-            ptr: self.ptr.upgrade().unwrap()
+            ptr: self.ptr.upgrade().unwrap(),
         }
     }
     pub fn upgrade(&self) -> Option<FastClearArcRwLock<T>> {
         self.ptr.upgrade().map(|x| FastClearArcRwLock::<T> { ptr: x })
     }
 }
 
 impl<T: FastClear> Clone for FastClearArcRwLock<T> {
     fn clone(&self) -> Self {
         Self::new_ptr(Arc::clone(self.ptr()))
     }
 }
 
 impl<T: FastClear> FastClearRwLockPtr<T> for FastClearArcRwLock<T> {
-    fn new_ptr(ptr: Arc<RwLock<T>>) -> Self { Self { ptr }  }
-    fn new_value(obj: T) -> Self { Self::new_ptr(Arc::new(RwLock::new(obj))) }
-    #[inline(always)] fn ptr(&self) -> &Arc<RwLock<T>> { &self.ptr }
-    #[inline(always)] fn ptr_mut(&mut self) -> &mut Arc<RwLock<T>> { &mut self.ptr }
+    fn new_ptr(ptr: Arc<RwLock<T>>) -> Self {
+        Self { ptr }
+    }
+    fn new_value(obj: T) -> Self {
+        Self::new_ptr(Arc::new(RwLock::new(obj)))
+    }
+    #[inline(always)]
+    fn ptr(&self) -> &Arc<RwLock<T>> {
+        &self.ptr
+    }
+    #[inline(always)]
+    fn ptr_mut(&mut self) -> &mut Arc<RwLock<T>> {
+        &mut self.ptr
+    }
 }
 
 impl<T: FastClear> PartialEq for FastClearArcRwLock<T> {
-    fn eq(&self, other: &Self) -> bool { self.ptr_eq(other) }
+    fn eq(&self, other: &Self) -> bool {
+        self.ptr_eq(other)
+    }
 }
 
-impl<T: FastClear> Eq for FastClearArcRwLock<T> { }
+impl<T: FastClear> Eq for FastClearArcRwLock<T> {}
 
 impl<T: FastClear> Clone for FastClearWeakRwLock<T> {
     fn clone(&self) -> Self {
         Self { ptr: self.ptr.clone() }
     }
 }
 
 impl<T: FastClear> PartialEq for FastClearWeakRwLock<T> {
-    fn eq(&self, other: &Self) -> bool { self.ptr.ptr_eq(&other.ptr) }
+    fn eq(&self, other: &Self) -> bool {
+        self.ptr.ptr_eq(&other.ptr)
+    }
 }
 
-impl<T: FastClear> Eq for FastClearWeakRwLock<T> { }
+impl<T: FastClear> Eq for FastClearWeakRwLock<T> {}
 
 impl<T: FastClear> std::ops::Deref for FastClearArcRwLock<T> {
     type Target = RwLock<T>;
     fn deref(&self) -> &Self::Target {
         &self.ptr
     }
 }
@@ -274,15 +301,14 @@
         self.upgrade()
     }
     fn clone(view: &Self::Strong) -> Self::Strong {
         view.clone()
     }
 }
 
-  
 /*
  * unsafe APIs, used for production environment where speed matters
  */
 
 cfg_if::cfg_if! {
     if #[cfg(feature="unsafe_pointer")] {
 
@@ -299,15 +325,15 @@
             #[inline(always)]
             fn read_recursive(&self, active_timestamp: FastClearTimestamp) -> &ObjType {
                 let ret = self.ptr();
                 ret.debug_assert_dynamic_cleared(active_timestamp);  // only assert during debug modes
                 ret
             }
 
-            /// without sanity check: this data might be outdated, so only use when you're read those immutable fields 
+            /// without sanity check: this data might be outdated, so only use when you're read those immutable fields
             #[inline(always)]
             fn read_recursive_force(&self) -> &ObjType {
                 self.ptr()
             }
 
             #[inline(always)]
             fn write(&self, active_timestamp: FastClearTimestamp) -> &mut ObjType {
@@ -555,15 +581,15 @@
                 unsafe {
                     let ret = &*self.ptr();
                     ret.debug_assert_dynamic_cleared(active_timestamp);  // only assert during debug modes
                     ret
                 }
             }
 
-            /// without sanity check: this data might be outdated, so only use when you're read those immutable fields 
+            /// without sanity check: this data might be outdated, so only use when you're read those immutable fields
             #[inline(always)]
             fn read_recursive_force(&self) -> &ObjType {
                 unsafe {
                     &*self.ptr()
                 }
             }
 
@@ -609,15 +635,15 @@
 
         pub struct FastClearWeakUnsafeDangerous<T: FastClear> {
             raw_ptr: *const T,
         }
 
         unsafe impl<T: FastClear> Send for FastClearArcUnsafeDangerous<T> {}
         unsafe impl<T: FastClear> Sync for FastClearArcUnsafeDangerous<T> {}
-    
+
         unsafe impl<T: FastClear> Send for FastClearWeakUnsafeDangerous<T> {}
         unsafe impl<T: FastClear> Sync for FastClearWeakUnsafeDangerous<T> {}
 
         impl<T: FastClear> FastClearArcUnsafeDangerous<T> {
             #[inline(always)]
             pub fn downgrade(&self) -> FastClearWeakUnsafeDangerous<T> {
                 FastClearWeakUnsafeDangerous::<T> {
@@ -748,15 +774,14 @@
         }
         #[allow(unused_imports)] pub use lock_write;
         pub type FastClearArcManualSafeLockDangerous<T> = FastClearArcRwLock<T>;
         pub type FastClearWeakManualSafeLockDangerous<T> = FastClearWeakRwLock<T>;
     }
 }
 
-
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[derive(Debug)]
     struct Tester {
         idx: usize,
@@ -775,42 +800,42 @@
     impl std::fmt::Debug for TesterWeak {
         fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
             self.upgrade_force().fmt(f)
         }
     }
 
     #[test]
-    fn pointers_test_1() {  // cargo test pointers_test_1 -- --nocapture
+    fn pointers_test_1() {
+        // cargo test pointers_test_1 -- --nocapture
         let ptr = TesterPtr::new_value(Tester { idx: 0 });
         let weak = ptr.downgrade();
         ptr.write().idx = 1;
         assert_eq!(weak.upgrade_force().read_recursive().idx, 1);
         weak.upgrade_force().write().idx = 2;
         assert_eq!(ptr.read_recursive().idx, 2);
     }
 
-cfg_if::cfg_if! {
-    if #[cfg(feature="unsafe_pointer")] {
+    cfg_if::cfg_if! {
+        if #[cfg(feature="unsafe_pointer")] {
 
-        type TesterUnsafePtr = ArcRwLock<Tester>;
+            type TesterUnsafePtr = ArcRwLock<Tester>;
 
-        #[test]
-        fn pointers_test_2() {  // cargo test pointers_test_2 --features unsafe_pointer -- --nocapture
-            let ptr = TesterUnsafePtr::new_value(Tester { idx: 0 });
-            let weak = ptr.downgrade();
-            ptr.write().idx = 1;
-            assert_eq!(weak.upgrade_force().read_recursive().idx, 1);
-            weak.upgrade_force().write().idx = 2;
-            assert_eq!(ptr.read_recursive().idx, 2);
-        }
-
-        #[test]
-        fn pointers_test_3() {  // cargo test pointers_test_3 --features dangerous_pointer -- --nocapture
-            println!("{}", std::mem::size_of::<ArcManualSafeLock<Tester>>());
-            println!("{}", std::mem::size_of::<Arc<Tester>>());
-            println!("{}", std::mem::size_of::<*const Tester>());
-        }
+            #[test]
+            fn pointers_test_2() {  // cargo test pointers_test_2 --features unsafe_pointer -- --nocapture
+                let ptr = TesterUnsafePtr::new_value(Tester { idx: 0 });
+                let weak = ptr.downgrade();
+                ptr.write().idx = 1;
+                assert_eq!(weak.upgrade_force().read_recursive().idx, 1);
+                weak.upgrade_force().write().idx = 2;
+                assert_eq!(ptr.read_recursive().idx, 2);
+            }
+
+            #[test]
+            fn pointers_test_3() {  // cargo test pointers_test_3 --features dangerous_pointer -- --nocapture
+                println!("{}", std::mem::size_of::<ArcManualSafeLock<Tester>>());
+                println!("{}", std::mem::size_of::<Arc<Tester>>());
+                println!("{}", std::mem::size_of::<*const Tester>());
+            }
 
+        }
     }
 }
-
-}
```

### Comparing `fusion_blossom-0.2.2/src/primal_module.rs` & `fusion_blossom-0.2.5/src/primal_module.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 //! Primal Module
-//! 
+//!
 //! Generics for primal modules, defining the necessary interfaces for a primal module
 //!
 
-use super::util::*;
-use super::dual_module::*;
-use crate::derivative::Derivative;
-use std::collections::{BTreeMap, BTreeSet, HashMap};
+#![cfg_attr(feature = "unsafe_pointer", allow(dropping_references))]
 use super::complete_graph::*;
-use super::visualize::*;
+use super::dual_module::*;
 use super::pointers::*;
-#[cfg(feature="python_binding")]
+use super::util::*;
+use super::visualize::*;
+use crate::derivative::Derivative;
+#[cfg(feature = "python_binding")]
 use pyo3::prelude::*;
-
+use std::collections::{BTreeMap, BTreeSet, HashMap};
 
 #[derive(Derivative)]
 #[derivative(Debug)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct IntermediateMatching {
     /// matched pairs; note that each pair will only appear once. (node_1, touching_1), (node_2, touching_2)
@@ -34,122 +34,192 @@
     pub peer_matchings: Vec<(DualNodePtr, DualNodePtr)>,
     /// those nodes matched to the boundary. (syndrome node, virtual_vertex)
     pub virtual_matchings: Vec<(DualNodePtr, VertexIndex)>,
 }
 
 /// common trait that must be implemented for each implementation of primal module
 pub trait PrimalModuleImpl {
-
     /// create a primal module given the dual module
     fn new_empty(solver_initializer: &SolverInitializer) -> Self;
 
     /// clear all states; however this method is not necessarily called when load a new decoding problem, so you need to call it yourself
     fn clear(&mut self);
 
     fn load_defect_dual_node(&mut self, dual_node_ptr: &DualNodePtr);
 
     /// load a single syndrome and update the dual module and the interface
-    fn load_defect<D: DualModuleImpl>(&mut self, defect_vertex: VertexIndex, interface_ptr: &DualModuleInterfacePtr, dual_module: &mut D) {
+    fn load_defect<D: DualModuleImpl>(
+        &mut self,
+        defect_vertex: VertexIndex,
+        interface_ptr: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) {
         interface_ptr.create_defect_node(defect_vertex, dual_module);
         let interface = interface_ptr.read_recursive();
         let index = interface.nodes_length - 1;
-        self.load_defect_dual_node(interface.nodes[index].as_ref().expect("must load a fresh dual module interface, found empty node"))
+        self.load_defect_dual_node(
+            interface.nodes[index]
+                .as_ref()
+                .expect("must load a fresh dual module interface, found empty node"),
+        )
     }
 
     /// load a new decoding problem given dual interface: note that all nodes MUST be syndrome node
+    #[allow(clippy::unnecessary_cast)]
     fn load(&mut self, interface_ptr: &DualModuleInterfacePtr) {
         let interface = interface_ptr.read_recursive();
         debug_assert!(interface.parent.is_none(), "cannot load an interface that is already fused");
-        debug_assert!(interface.children.is_none(), "please customize load function if interface is fused");
+        debug_assert!(
+            interface.children.is_none(),
+            "please customize load function if interface is fused"
+        );
         for index in 0..interface.nodes_length as NodeIndex {
             let node = &interface.nodes[index as usize];
             debug_assert!(node.is_some(), "must load a fresh dual module interface, found empty node");
             let node_ptr = node.as_ref().unwrap();
             let node = node_ptr.read_recursive();
-            debug_assert!(matches!(node.class, DualNodeClass::DefectVertex{ .. }), "must load a fresh dual module interface, found a blossom");
-            debug_assert_eq!(node.index, index, "must load a fresh dual module interface, found index out of order");
+            debug_assert!(
+                matches!(node.class, DualNodeClass::DefectVertex { .. }),
+                "must load a fresh dual module interface, found a blossom"
+            );
+            debug_assert_eq!(
+                node.index, index,
+                "must load a fresh dual module interface, found index out of order"
+            );
             self.load_defect_dual_node(node_ptr);
         }
     }
 
     /// analyze the reason why dual module cannot further grow, update primal data structure (alternating tree, temporary matches, etc)
     /// and then tell dual module what to do to resolve these conflicts;
     /// note that this function doesn't necessarily resolve all the conflicts, but can return early if some major change is made.
     /// when implementing this function, it's recommended that you resolve as many conflicts as possible.
-    fn resolve<D: DualModuleImpl>(&mut self, group_max_update_length: GroupMaxUpdateLength, interface: &DualModuleInterfacePtr, dual_module: &mut D);
+    fn resolve<D: DualModuleImpl>(
+        &mut self,
+        group_max_update_length: GroupMaxUpdateLength,
+        interface: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    );
 
     /// return a matching that can possibly include blossom nodes: this does not affect dual module
-    fn intermediate_matching<D: DualModuleImpl>(&mut self, interface: &DualModuleInterfacePtr, dual_module: &mut D) -> IntermediateMatching;
+    fn intermediate_matching<D: DualModuleImpl>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) -> IntermediateMatching;
 
     /// break down the blossoms to find the final matching; this function will take more time on the dual module
-    fn perfect_matching<D: DualModuleImpl>(&mut self, interface: &DualModuleInterfacePtr, dual_module: &mut D) -> PerfectMatching {
+    fn perfect_matching<D: DualModuleImpl>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) -> PerfectMatching {
         let intermediate_matching = self.intermediate_matching(interface, dual_module);
         intermediate_matching.get_perfect_matching()
     }
 
-    fn solve<D: DualModuleImpl>(&mut self, interface: &DualModuleInterfacePtr, syndrome_pattern: &SyndromePattern, dual_module: &mut D) {
+    fn solve<D: DualModuleImpl>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        syndrome_pattern: &SyndromePattern,
+        dual_module: &mut D,
+    ) {
         self.solve_step_callback(interface, syndrome_pattern, dual_module, |_, _, _, _| {})
     }
 
-    fn solve_visualizer<D: DualModuleImpl + FusionVisualizer>(&mut self, interface: &DualModuleInterfacePtr, syndrome_pattern: &SyndromePattern, dual_module: &mut D
-            , visualizer: Option<&mut Visualizer>) where Self: FusionVisualizer + Sized {
+    fn solve_visualizer<D: DualModuleImpl + FusionVisualizer>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        syndrome_pattern: &SyndromePattern,
+        dual_module: &mut D,
+        visualizer: Option<&mut Visualizer>,
+    ) where
+        Self: FusionVisualizer + Sized,
+    {
         if let Some(visualizer) = visualizer {
-            self.solve_step_callback(interface, syndrome_pattern, dual_module, |interface, dual_module, primal_module, group_max_update_length| {
-                if cfg!(debug_assertions) {
-                    println!("group_max_update_length: {:?}", group_max_update_length);
-                }
-                if let Some(length) = group_max_update_length.get_none_zero_growth() {
-                    visualizer.snapshot_combined(format!("grow {length}"), vec![interface, dual_module, primal_module]).unwrap();
-                } else {
-                    let first_conflict = format!("{:?}", group_max_update_length.peek().unwrap());
-                    visualizer.snapshot_combined(format!("resolve {first_conflict}"), vec![interface, dual_module, primal_module]).unwrap();
-                };
-            });
-            visualizer.snapshot_combined("solved".to_string(), vec![interface, dual_module, self]).unwrap();
+            self.solve_step_callback(
+                interface,
+                syndrome_pattern,
+                dual_module,
+                |interface, dual_module, primal_module, group_max_update_length| {
+                    if cfg!(debug_assertions) {
+                        println!("group_max_update_length: {:?}", group_max_update_length);
+                    }
+                    if let Some(length) = group_max_update_length.get_none_zero_growth() {
+                        visualizer
+                            .snapshot_combined(format!("grow {length}"), vec![interface, dual_module, primal_module])
+                            .unwrap();
+                    } else {
+                        let first_conflict = format!("{:?}", group_max_update_length.peek().unwrap());
+                        visualizer
+                            .snapshot_combined(
+                                format!("resolve {first_conflict}"),
+                                vec![interface, dual_module, primal_module],
+                            )
+                            .unwrap();
+                    };
+                },
+            );
+            visualizer
+                .snapshot_combined("solved".to_string(), vec![interface, dual_module, self])
+                .unwrap();
         } else {
             self.solve(interface, syndrome_pattern, dual_module);
         }
     }
 
-    fn solve_step_callback<D: DualModuleImpl, F>(&mut self, interface: &DualModuleInterfacePtr, syndrome_pattern: &SyndromePattern, dual_module: &mut D, callback: F)
-            where F: FnMut(&DualModuleInterfacePtr, &mut D, &mut Self, &GroupMaxUpdateLength) {
+    fn solve_step_callback<D: DualModuleImpl, F>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        syndrome_pattern: &SyndromePattern,
+        dual_module: &mut D,
+        callback: F,
+    ) where
+        F: FnMut(&DualModuleInterfacePtr, &mut D, &mut Self, &GroupMaxUpdateLength),
+    {
         interface.load(syndrome_pattern, dual_module);
         self.load(interface);
         self.solve_step_callback_interface_loaded(interface, dual_module, callback);
     }
 
-    fn solve_step_callback_interface_loaded<D: DualModuleImpl, F>(&mut self, interface: &DualModuleInterfacePtr, dual_module: &mut D, mut callback: F)
-            where F: FnMut(&DualModuleInterfacePtr, &mut D, &mut Self, &GroupMaxUpdateLength) {
+    fn solve_step_callback_interface_loaded<D: DualModuleImpl, F>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+        mut callback: F,
+    ) where
+        F: FnMut(&DualModuleInterfacePtr, &mut D, &mut Self, &GroupMaxUpdateLength),
+    {
         let mut group_max_update_length = dual_module.compute_maximum_update_length();
         while !group_max_update_length.is_empty() {
             callback(interface, dual_module, self, &group_max_update_length);
             if let Some(length) = group_max_update_length.get_none_zero_growth() {
                 interface.grow(length, dual_module);
             } else {
                 self.resolve(group_max_update_length, interface, dual_module);
             }
             group_max_update_length = dual_module.compute_maximum_update_length();
         }
     }
 
     /// performance profiler report
-    fn generate_profiler_report(&self) -> serde_json::Value { json!({}) }
-
+    fn generate_profiler_report(&self) -> serde_json::Value {
+        json!({})
+    }
 }
 
 impl Default for IntermediateMatching {
     fn default() -> Self {
         Self::new()
     }
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl IntermediateMatching {
-
     #[cfg_attr(feature = "python_binding", new)]
     pub fn new() -> Self {
         Self {
             peer_matchings: vec![],
             virtual_matchings: vec![],
         }
     }
@@ -162,49 +232,69 @@
     /// expand the intermediate matching into a perfect matching with only syndrome nodes
     pub fn get_perfect_matching(&self) -> PerfectMatching {
         let mut perfect_matching = PerfectMatching::new();
         // handle peer matchings
         for ((dual_node_ptr_1, touching_weak_1), (dual_node_ptr_2, touching_weak_2)) in self.peer_matchings.iter() {
             let touching_ptr_1 = touching_weak_1.upgrade_force();
             let touching_ptr_2 = touching_weak_2.upgrade_force();
-            perfect_matching.peer_matchings.extend(Self::expand_peer_matching(dual_node_ptr_1, &touching_ptr_1, dual_node_ptr_2, &touching_ptr_2));
+            perfect_matching.peer_matchings.extend(Self::expand_peer_matching(
+                dual_node_ptr_1,
+                &touching_ptr_1,
+                dual_node_ptr_2,
+                &touching_ptr_2,
+            ));
         }
         // handle virtual matchings
         for ((dual_node_ptr, touching_weak), virtual_vertex) in self.virtual_matchings.iter() {
             let touching_ptr = touching_weak.upgrade_force();
-            perfect_matching.peer_matchings.extend(Self::expand_blossom(dual_node_ptr, &touching_ptr));
+            perfect_matching
+                .peer_matchings
+                .extend(Self::expand_blossom(dual_node_ptr, &touching_ptr));
             perfect_matching.virtual_matchings.push((touching_ptr, *virtual_vertex));
         }
         perfect_matching
     }
 
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 
     #[cfg(feature = "python_binding")]
     #[getter]
     pub fn get_peer_matchings(&self) -> Vec<((NodeIndex, NodeIndex), (NodeIndex, NodeIndex))> {
-        self.peer_matchings.iter().map(|((a, b), (c, d))|
-            ((a.updated_index(), b.upgrade_force().updated_index()), (c.updated_index(), d.upgrade_force().updated_index()))).collect()
+        self.peer_matchings
+            .iter()
+            .map(|((a, b), (c, d))| {
+                (
+                    (a.updated_index(), b.upgrade_force().updated_index()),
+                    (c.updated_index(), d.upgrade_force().updated_index()),
+                )
+            })
+            .collect()
     }
 
     #[cfg(feature = "python_binding")]
     #[getter]
     pub fn get_virtual_matchings(&self) -> Vec<((NodeIndex, NodeIndex), VertexIndex)> {
-        self.virtual_matchings.iter().map(|((a, b), c)|
-            ((a.updated_index(), b.upgrade_force().updated_index()), *c)).collect()
+        self.virtual_matchings
+            .iter()
+            .map(|((a, b), c)| ((a.updated_index(), b.upgrade_force().updated_index()), *c))
+            .collect()
     }
-
 }
 
 impl IntermediateMatching {
-
     /// break down a single matched pair to find the perfect matching
-    pub fn expand_peer_matching(dual_node_ptr_1: &DualNodePtr, touching_ptr_1: &DualNodePtr, dual_node_ptr_2: &DualNodePtr
-            , touching_ptr_2: &DualNodePtr) -> Vec<(DualNodePtr, DualNodePtr)> {
+    pub fn expand_peer_matching(
+        dual_node_ptr_1: &DualNodePtr,
+        touching_ptr_1: &DualNodePtr,
+        dual_node_ptr_2: &DualNodePtr,
+        touching_ptr_2: &DualNodePtr,
+    ) -> Vec<(DualNodePtr, DualNodePtr)> {
         // println!("expand_peer_matching ({:?}, {:?}), ({:?}, {:?}) {{", dual_node_ptr_1, touching_ptr_1, dual_node_ptr_2, touching_ptr_2);
         let mut perfect_matching = vec![];
         perfect_matching.extend(Self::expand_blossom(dual_node_ptr_1, touching_ptr_1));
         perfect_matching.extend(Self::expand_blossom(dual_node_ptr_2, touching_ptr_2));
         perfect_matching.push((touching_ptr_1.clone(), touching_ptr_2.clone()));
         // println!("}},");
         perfect_matching
@@ -217,111 +307,141 @@
         let mut child_ptr = touching_ptr.clone();
         while &child_ptr != blossom_ptr {
             let child_weak = child_ptr.downgrade();
             let child = child_ptr.read_recursive();
             if let Some(parent_blossom_weak) = child.parent_blossom.as_ref() {
                 let parent_blossom_ptr = parent_blossom_weak.upgrade_force();
                 let parent_blossom = parent_blossom_ptr.read_recursive();
-                if let DualNodeClass::Blossom{ nodes_circle, touching_children } = &parent_blossom.class {
-                    let idx = nodes_circle.iter().position(|ptr| ptr == &child_weak).expect("should find child");
-                    debug_assert!(nodes_circle.len() % 2 == 1 && nodes_circle.len() >= 3, "must be a valid blossom");
-                    for i in (0..(nodes_circle.len()-1)).step_by(2) {
+                if let DualNodeClass::Blossom {
+                    nodes_circle,
+                    touching_children,
+                } = &parent_blossom.class
+                {
+                    let idx = nodes_circle
+                        .iter()
+                        .position(|ptr| ptr == &child_weak)
+                        .expect("should find child");
+                    debug_assert!(
+                        nodes_circle.len() % 2 == 1 && nodes_circle.len() >= 3,
+                        "must be a valid blossom"
+                    );
+                    for i in (0..(nodes_circle.len() - 1)).step_by(2) {
                         let idx_1 = (idx + i + 1) % nodes_circle.len();
                         let idx_2 = (idx + i + 2) % nodes_circle.len();
                         let dual_node_ptr_1 = nodes_circle[idx_1].upgrade_force();
                         let dual_node_ptr_2 = nodes_circle[idx_2].upgrade_force();
-                        let touching_ptr_1 = touching_children[idx_1].1.upgrade_force();  // match to right
-                        let touching_ptr_2 = touching_children[idx_2].0.upgrade_force();  // match to left
+                        let touching_ptr_1 = touching_children[idx_1].1.upgrade_force(); // match to right
+                        let touching_ptr_2 = touching_children[idx_2].0.upgrade_force(); // match to left
                         perfect_matching.extend(Self::expand_peer_matching(
-                            &dual_node_ptr_1, &touching_ptr_1, &dual_node_ptr_2, &touching_ptr_2
+                            &dual_node_ptr_1,
+                            &touching_ptr_1,
+                            &dual_node_ptr_2,
+                            &touching_ptr_2,
                         ))
                     }
                 }
                 drop(child);
                 child_ptr = parent_blossom_ptr.clone();
-            } else { panic!("cannot find parent of {}", child.index) }
+            } else {
+                panic!("cannot find parent of {}", child.index)
+            }
         }
         // println!("}},");
         perfect_matching
     }
-
 }
 
 impl Default for PerfectMatching {
     fn default() -> Self {
         Self::new()
     }
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl PerfectMatching {
-
     #[cfg_attr(feature = "python_binding", new)]
     pub fn new() -> Self {
         Self {
             peer_matchings: vec![],
             virtual_matchings: vec![],
         }
     }
 
     /// this interface is not very optimized, but is compatible with blossom V algorithm's result
-    pub fn legacy_get_mwpm_result(&self, defect_vertices: Vec<VertexIndex>) -> Vec<SyndromeIndex> {
+    pub fn legacy_get_mwpm_result(&self, defect_vertices: Vec<VertexIndex>) -> Vec<DefectIndex> {
         let mut peer_matching_maps = BTreeMap::<VertexIndex, VertexIndex>::new();
         for (ptr_1, ptr_2) in self.peer_matchings.iter() {
             let a_vid = {
                 let node = ptr_1.read_recursive();
-                if let DualNodeClass::DefectVertex{ defect_index } = &node.class { *defect_index } else { unreachable!("can only be syndrome") }
+                if let DualNodeClass::DefectVertex { defect_index } = &node.class {
+                    *defect_index
+                } else {
+                    unreachable!("can only be syndrome")
+                }
             };
             let b_vid = {
                 let node = ptr_2.read_recursive();
-                if let DualNodeClass::DefectVertex{ defect_index } = &node.class { *defect_index } else { unreachable!("can only be syndrome") }
+                if let DualNodeClass::DefectVertex { defect_index } = &node.class {
+                    *defect_index
+                } else {
+                    unreachable!("can only be syndrome")
+                }
             };
             peer_matching_maps.insert(a_vid, b_vid);
             peer_matching_maps.insert(b_vid, a_vid);
         }
         let mut virtual_matching_maps = BTreeMap::<VertexIndex, VertexIndex>::new();
         for (ptr, virtual_vertex) in self.virtual_matchings.iter() {
             let a_vid = {
                 let node = ptr.read_recursive();
-                if let DualNodeClass::DefectVertex{ defect_index } = &node.class { *defect_index } else { unreachable!("can only be syndrome") }
+                if let DualNodeClass::DefectVertex { defect_index } = &node.class {
+                    *defect_index
+                } else {
+                    unreachable!("can only be syndrome")
+                }
             };
             virtual_matching_maps.insert(a_vid, *virtual_vertex);
         }
         let mut mwpm_result = Vec::with_capacity(defect_vertices.len());
         for defect_vertex in defect_vertices.iter() {
             if let Some(a) = peer_matching_maps.get(defect_vertex) {
                 mwpm_result.push(*a);
             } else if let Some(v) = virtual_matching_maps.get(defect_vertex) {
                 mwpm_result.push(*v);
-            } else { panic!("cannot find defect vertex {}", defect_vertex) }
+            } else {
+                panic!("cannot find defect vertex {}", defect_vertex)
+            }
         }
         mwpm_result
     }
 
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 
     #[cfg(feature = "python_binding")]
     #[getter]
     pub fn get_peer_matchings(&self) -> Vec<(NodeIndex, NodeIndex)> {
-        self.peer_matchings.iter().map(|(a, b)|
-            (a.updated_index(), b.updated_index())).collect()
+        self.peer_matchings
+            .iter()
+            .map(|(a, b)| (a.updated_index(), b.updated_index()))
+            .collect()
     }
 
     #[cfg(feature = "python_binding")]
     #[getter]
     pub fn get_virtual_matchings(&self) -> Vec<(NodeIndex, VertexIndex)> {
-        self.virtual_matchings.iter().map(|(a, b)|
-            (a.updated_index(), *b)).collect()
+        self.virtual_matchings.iter().map(|(a, b)| (a.updated_index(), *b)).collect()
     }
-
 }
 
 impl FusionVisualizer for PerfectMatching {
+    #[allow(clippy::unnecessary_cast)]
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         let primal_nodes = if self.peer_matchings.is_empty() && self.virtual_matchings.is_empty() {
             vec![]
         } else {
             let mut maximum_node_index = 0;
             for (ptr_1, ptr_2) in self.peer_matchings.iter() {
                 maximum_node_index = std::cmp::max(maximum_node_index, ptr_1.get_ancestor_blossom().read_recursive().index);
@@ -375,15 +495,14 @@
     /// an instance of complete graph to compute minimum-weight path between any pair of vertices
     pub complete_graph: CompleteGraph,
     /// current subgraph, assuming edges are not very much
     pub subgraph: BTreeSet<EdgeIndex>,
 }
 
 impl SubGraphBuilder {
-
     pub fn new(initializer: &SolverInitializer) -> Self {
         let mut vertex_pair_edges = HashMap::with_capacity(initializer.weighted_edges.len());
         for (edge_index, (i, j, _)) in initializer.weighted_edges.iter().enumerate() {
             let id = if i < j { (*i, *j) } else { (*j, *i) };
             vertex_pair_edges.insert(id, edge_index as EdgeIndex);
         }
         Self {
@@ -400,32 +519,48 @@
     }
 
     /// temporarily set some edges to 0 weight, and when it resets, those edges will be reverted back to the original weight
     pub fn load_erasures(&mut self, erasures: &[EdgeIndex]) {
         self.complete_graph.load_erasures(erasures);
     }
 
+    pub fn load_dynamic_weights(&mut self, dynamic_weights: &[(EdgeIndex, Weight)]) {
+        self.complete_graph.load_dynamic_weights(dynamic_weights);
+    }
+
     /// load perfect matching to the subgraph builder
     pub fn load_perfect_matching(&mut self, perfect_matching: &PerfectMatching) {
         self.subgraph.clear();
         for (ptr_1, ptr_2) in perfect_matching.peer_matchings.iter() {
             let a_vid = {
                 let node = ptr_1.read_recursive();
-                if let DualNodeClass::DefectVertex{ defect_index } = &node.class { *defect_index } else { unreachable!("can only be syndrome") }
+                if let DualNodeClass::DefectVertex { defect_index } = &node.class {
+                    *defect_index
+                } else {
+                    unreachable!("can only be syndrome")
+                }
             };
             let b_vid = {
                 let node = ptr_2.read_recursive();
-                if let DualNodeClass::DefectVertex{ defect_index } = &node.class { *defect_index } else { unreachable!("can only be syndrome") }
+                if let DualNodeClass::DefectVertex { defect_index } = &node.class {
+                    *defect_index
+                } else {
+                    unreachable!("can only be syndrome")
+                }
             };
             self.add_matching(a_vid, b_vid);
         }
         for (ptr, virtual_vertex) in perfect_matching.virtual_matchings.iter() {
             let a_vid = {
                 let node = ptr.read_recursive();
-                if let DualNodeClass::DefectVertex{ defect_index } = &node.class { *defect_index } else { unreachable!("can only be syndrome") }
+                if let DualNodeClass::DefectVertex { defect_index } = &node.class {
+                    *defect_index
+                } else {
+                    unreachable!("can only be syndrome")
+                }
             };
             self.add_matching(a_vid, *virtual_vertex);
         }
     }
 
     /// add a matching, finding the minimum path and XOR them into the subgraph (if adding the same pair twice, they will cancel each other)
     pub fn add_matching(&mut self, vertex_1: VertexIndex, vertex_2: VertexIndex) {
@@ -441,50 +576,48 @@
                 self.subgraph.insert(edge_index);
             }
             a = b;
         }
     }
 
     /// get the total weight of the subgraph
+    #[allow(clippy::unnecessary_cast)]
     pub fn total_weight(&self) -> Weight {
         let mut weight = 0;
         for edge_index in self.subgraph.iter() {
             weight += self.complete_graph.weighted_edges[*edge_index as usize].2;
         }
         weight
     }
 
     /// get subgraph as a vec
     pub fn get_subgraph(&self) -> Vec<EdgeIndex> {
         self.subgraph.iter().copied().collect()
     }
-
 }
 
 /// to visualize subgraph
 pub struct VisualizeSubgraph<'a> {
     pub subgraph: &'a Vec<EdgeIndex>,
 }
 
 impl<'a> VisualizeSubgraph<'a> {
     pub fn new(subgraph: &'a Vec<EdgeIndex>) -> Self {
-        Self {
-            subgraph
-        }
+        Self { subgraph }
     }
 }
 
 impl FusionVisualizer for VisualizeSubgraph<'_> {
     fn snapshot(&self, _abbrev: bool) -> serde_json::Value {
         json!({
             "subgraph": self.subgraph,
         })
     }
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 #[pyfunction]
 pub(crate) fn register(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<IntermediateMatching>()?;
     m.add_class::<PerfectMatching>()?;
     Ok(())
 }
```

### Comparing `fusion_blossom-0.2.2/src/primal_module_parallel.rs` & `fusion_blossom-0.2.5/src/primal_module_parallel.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 //! Parallel Primal Module
-//! 
+//!
 //! A parallel implementation of the primal module, by calling functions provided by the serial primal module
 //!
 
-use super::util::*;
-use serde::{Serialize, Deserialize};
-use crate::rayon::prelude::*;
+#![cfg_attr(feature = "unsafe_pointer", allow(dropping_references))]
+use super::dual_module::*;
+use super::dual_module_parallel::*;
+use super::pointers::*;
 use super::primal_module::*;
 use super::primal_module_serial::*;
-use super::dual_module_parallel::*;
+use super::util::*;
 use super::visualize::*;
-use super::dual_module::*;
-use std::sync::{Arc, Mutex, Condvar};
+use crate::rayon::prelude::*;
+use serde::{Deserialize, Serialize};
 use std::ops::DerefMut;
-use std::time::Instant;
-use super::pointers::*;
-
+use std::sync::{Arc, Condvar, Mutex};
+use std::time::{Duration, Instant};
 
 pub struct PrimalModuleParallel {
     /// the basic wrapped serial modules at the beginning, afterwards the fused units are appended after them
     pub units: Vec<PrimalModuleParallelUnitPtr>,
     /// local configuration
     pub config: PrimalModuleParallelConfig,
     /// partition information generated by the config
     pub partition_info: Arc<PartitionInfo>,
     /// thread pool used to execute async functions in parallel
     pub thread_pool: Arc<rayon::ThreadPool>,
     /// the time of calling [`PrimalModuleParallel::parallel_solve_step_callback`] method
-    pub last_solve_start_time: Instant,
+    pub last_solve_start_time: ArcRwLock<Instant>,
 }
 
 pub struct PrimalModuleParallelUnit {
     /// the index
     pub unit_index: usize,
     /// the dual module interface, for constant-time clear
     pub interface_ptr: DualModuleInterfacePtr,
@@ -43,14 +43,16 @@
     pub serial_module: PrimalModuleSerialPtr,
     /// left and right children dual modules
     pub children: Option<(PrimalModuleParallelUnitWeak, PrimalModuleParallelUnitWeak)>,
     /// parent dual module
     pub parent: Option<PrimalModuleParallelUnitWeak>,
     /// record the time of events
     pub event_time: Option<PrimalModuleParallelUnitEventTime>,
+    /// streaming decode mocker, if exists, base partition will wait until specified time and then start decoding
+    pub streaming_decode_mocker: Option<StreamingDecodeMocker>,
 }
 
 pub type PrimalModuleParallelUnitPtr = ArcManualSafeLock<PrimalModuleParallelUnit>;
 pub type PrimalModuleParallelUnitWeak = WeakManualSafeLock<PrimalModuleParallelUnit>;
 
 impl std::fmt::Debug for PrimalModuleParallelUnitPtr {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
@@ -100,85 +102,132 @@
     pub thread_pool_size: usize,
     /// debug by sequentially run the fusion tasks, user must enable this for visualizer to work properly during the execution
     #[serde(default = "primal_module_parallel_default_configs::debug_sequential")]
     pub debug_sequential: bool,
     /// schedule base partition tasks in the front
     #[serde(default = "primal_module_parallel_default_configs::prioritize_base_partition")]
     pub prioritize_base_partition: bool,
+    #[serde(default = "primal_module_parallel_default_configs::interleaving_base_fusion")]
+    pub interleaving_base_fusion: usize,
     /// pin threads to cores sequentially
     #[serde(default = "primal_module_parallel_default_configs::pin_threads_to_cores")]
     pub pin_threads_to_cores: bool,
+    /// streaming decode mocker
+    pub streaming_decode_mock_measure_interval: Option<f64>,
+    /// streaming decoder using spin lock instead of threads.sleep to avoid context switch
+    #[serde(default = "primal_module_parallel_default_configs::streaming_decode_use_spin_lock")]
+    pub streaming_decode_use_spin_lock: bool,
 }
 
 impl Default for PrimalModuleParallelConfig {
-    fn default() -> Self { serde_json::from_value(json!({})).unwrap() }
+    fn default() -> Self {
+        serde_json::from_value(json!({})).unwrap()
+    }
 }
 
 pub mod primal_module_parallel_default_configs {
-    pub fn thread_pool_size() -> usize { 0 }  // by default to the number of CPU cores
-    // pub fn thread_pool_size() -> usize { 1 }  // debug: use a single core
-    pub fn debug_sequential() -> bool { false }  // by default enabled: only disable when you need to debug and get visualizer to work
-    pub fn pin_threads_to_cores() -> bool { false }  // pin threads to cores to achieve most stable results
-    pub fn prioritize_base_partition() -> bool { true }  // by default enable because this is faster by placing time-consuming tasks in the front
+    pub fn thread_pool_size() -> usize {
+        0
+    } // by default to the number of CPU cores
+      // pub fn thread_pool_size() -> usize { 1 }  // debug: use a single core
+    pub fn debug_sequential() -> bool {
+        false
+    } // by default enabled: only disable when you need to debug and get visualizer to work
+    pub fn pin_threads_to_cores() -> bool {
+        false
+    } // pin threads to cores to achieve most stable results
+    pub fn prioritize_base_partition() -> bool {
+        true
+    } // by default enable because this is faster by placing time-consuming tasks in the front
+    pub fn interleaving_base_fusion() -> usize {
+        usize::MAX
+    } // starts interleaving base and fusion after this unit_index
+    pub fn streaming_decode_use_spin_lock() -> bool {
+        false
+    } // by default use threads.sleep; enable only when benchmarking latency
 }
 
-impl PrimalModuleParallel {
+pub struct StreamingDecodeMocker {
+    /// indicating the syndrome ready time = `last_solve_start_time` + bias
+    pub bias: Duration,
+}
 
+impl PrimalModuleParallel {
     /// recommended way to create a new instance, given a customized configuration
-    pub fn new_config(initializer: &SolverInitializer, partition_info: &PartitionInfo, config: PrimalModuleParallelConfig) -> Self {
+    pub fn new_config(
+        initializer: &SolverInitializer,
+        partition_info: &PartitionInfo,
+        config: PrimalModuleParallelConfig,
+    ) -> Self {
         let partition_info = Arc::new(partition_info.clone());
         let mut thread_pool_builder = rayon::ThreadPoolBuilder::new();
         if config.thread_pool_size != 0 {
             thread_pool_builder = thread_pool_builder.num_threads(config.thread_pool_size);
         }
         if config.pin_threads_to_cores {
             let core_ids = core_affinity::get_core_ids().unwrap();
             // println!("core_ids: {core_ids:?}");
             thread_pool_builder = thread_pool_builder.start_handler(move |thread_index| {
                 // https://stackoverflow.com/questions/7274585/linux-find-out-hyper-threaded-core-id
                 if thread_index < core_ids.len() {
                     crate::core_affinity::set_for_current(core_ids[thread_index]);
-                }  // otherwise let OS decide which core to execute
+                } // otherwise let OS decide which core to execute
             });
         }
         let thread_pool = thread_pool_builder.build().expect("creating thread pool failed");
         let mut units = vec![];
         let unit_count = partition_info.units.len();
         thread_pool.scope(|_| {
-            (0..unit_count).into_par_iter().map(|unit_index| {
-                // println!("unit_index: {unit_index}");
-                let primal_module = PrimalModuleSerialPtr::new_empty(initializer);
-                PrimalModuleParallelUnitPtr::new_wrapper(primal_module, unit_index, Arc::clone(&partition_info))
-            }).collect_into_vec(&mut units);
+            (0..unit_count)
+                .into_par_iter()
+                .map(|unit_index| {
+                    // println!("unit_index: {unit_index}");
+                    let primal_module = PrimalModuleSerialPtr::new_empty(initializer);
+                    PrimalModuleParallelUnitPtr::new_wrapper(primal_module, unit_index, Arc::clone(&partition_info))
+                })
+                .collect_into_vec(&mut units);
         });
         // fill in the children and parent references
         for unit_index in 0..unit_count {
             let mut unit = units[unit_index].write();
             if let Some((left_children_index, right_children_index)) = &partition_info.units[unit_index].children {
-                unit.children = Some((units[*left_children_index].downgrade(), units[*right_children_index].downgrade()))
+                unit.children = Some((
+                    units[*left_children_index].downgrade(),
+                    units[*right_children_index].downgrade(),
+                ))
             }
             if let Some(parent_index) = &partition_info.units[unit_index].parent {
                 unit.parent = Some(units[*parent_index].downgrade());
             }
+            if let Some(measure_interval) = config.streaming_decode_mock_measure_interval {
+                if unit_index < partition_info.config.partitions.len() {
+                    // only base partition is blocked by mock hardware syndrome measurement
+                    unit.streaming_decode_mocker = Some(StreamingDecodeMocker {
+                        bias: Duration::from_secs_f64(measure_interval * (unit_index + 1) as f64),
+                    })
+                }
+            }
         }
         Self {
             units,
             config,
             partition_info,
             thread_pool: Arc::new(thread_pool),
-            last_solve_start_time: Instant::now(),
+            last_solve_start_time: ArcRwLock::new_value(Instant::now()),
         }
     }
-
 }
 
 impl PrimalModuleImpl for PrimalModuleParallel {
-
     fn new_empty(initializer: &SolverInitializer) -> Self {
-        Self::new_config(initializer, &PartitionConfig::new(initializer.vertex_num).info(), PrimalModuleParallelConfig::default())
+        Self::new_config(
+            initializer,
+            &PartitionConfig::new(initializer.vertex_num).info(),
+            PrimalModuleParallelConfig::default(),
+        )
     }
 
     #[inline(never)]
     fn clear(&mut self) {
         self.thread_pool.scope(|_| {
             self.units.par_iter().enumerate().for_each(|(unit_idx, unit_ptr)| {
                 let mut unit = unit_ptr.write();
@@ -190,298 +239,497 @@
         });
     }
 
     fn load_defect_dual_node(&mut self, _dual_node_ptr: &DualNodePtr) {
         panic!("load interface directly into the parallel primal module is forbidden, use `parallel_solve` instead");
     }
 
-    fn resolve<D: DualModuleImpl>(&mut self, _group_max_update_length: GroupMaxUpdateLength, _interface: &DualModuleInterfacePtr, _dual_module: &mut D) {
+    fn resolve<D: DualModuleImpl>(
+        &mut self,
+        _group_max_update_length: GroupMaxUpdateLength,
+        _interface: &DualModuleInterfacePtr,
+        _dual_module: &mut D,
+    ) {
         panic!("parallel primal module cannot handle global resolve requests, use `parallel_solve` instead");
     }
 
-    fn intermediate_matching<D: DualModuleImpl>(&mut self, interface: &DualModuleInterfacePtr, dual_module: &mut D) -> IntermediateMatching {
+    fn intermediate_matching<D: DualModuleImpl>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) -> IntermediateMatching {
         let mut intermediate_matching = IntermediateMatching::new();
         for unit_ptr in self.units.iter() {
             lock_write!(unit, unit_ptr);
-            if !unit.is_active { continue }  // do not visualize inactive units
+            if !unit.is_active {
+                continue;
+            } // do not visualize inactive units
             intermediate_matching.append(&mut unit.serial_module.intermediate_matching(interface, dual_module));
         }
         intermediate_matching
     }
 
     fn generate_profiler_report(&self) -> serde_json::Value {
         let event_time_vec: Vec<_> = self.units.iter().map(|ptr| ptr.read_recursive().event_time.clone()).collect();
         json!({
             "event_time_vec": event_time_vec,
         })
     }
-
 }
 
 impl PrimalModuleParallel {
-
-    pub fn parallel_solve<DualSerialModule: DualModuleImpl + Send + Sync>
-            (&mut self, syndrome_pattern: &SyndromePattern, parallel_dual_module: &mut DualModuleParallel<DualSerialModule>) {
+    pub fn parallel_solve<DualSerialModule: DualModuleImpl + Send + Sync>(
+        &mut self,
+        syndrome_pattern: &SyndromePattern,
+        parallel_dual_module: &mut DualModuleParallel<DualSerialModule>,
+    ) {
         self.parallel_solve_step_callback(syndrome_pattern, parallel_dual_module, |_, _, _, _| {})
     }
 
-    pub fn parallel_solve_visualizer<DualSerialModule: DualModuleImpl + Send + Sync + FusionVisualizer>
-            (&mut self, syndrome_pattern: &SyndromePattern, parallel_dual_module: &mut DualModuleParallel<DualSerialModule>
-            , visualizer: Option<&mut Visualizer>) {
+    pub fn parallel_solve_visualizer<DualSerialModule: DualModuleImpl + Send + Sync + FusionVisualizer>(
+        &mut self,
+        syndrome_pattern: &SyndromePattern,
+        parallel_dual_module: &mut DualModuleParallel<DualSerialModule>,
+        visualizer: Option<&mut Visualizer>,
+    ) {
         if let Some(visualizer) = visualizer {
-            self.parallel_solve_step_callback(syndrome_pattern, parallel_dual_module
-                , |interface_ptr, dual_module, primal_module, group_max_update_length| {
+            self.parallel_solve_step_callback(
+                syndrome_pattern,
+                parallel_dual_module,
+                |interface_ptr, dual_module, primal_module, group_max_update_length| {
                     if let Some(group_max_update_length) = group_max_update_length {
                         if cfg!(debug_assertions) {
                             println!("group_max_update_length: {:?}", group_max_update_length);
                         }
                         if let Some(length) = group_max_update_length.get_none_zero_growth() {
-                            visualizer.snapshot_combined(format!("grow {length}"), vec![interface_ptr, dual_module, primal_module]).unwrap();
+                            visualizer
+                                .snapshot_combined(format!("grow {length}"), vec![interface_ptr, dual_module, primal_module])
+                                .unwrap();
                         } else {
                             let first_conflict = format!("{:?}", group_max_update_length.peek().unwrap());
-                            visualizer.snapshot_combined(format!("resolve {first_conflict}"), vec![interface_ptr, dual_module, primal_module]).unwrap();
+                            visualizer
+                                .snapshot_combined(
+                                    format!("resolve {first_conflict}"),
+                                    vec![interface_ptr, dual_module, primal_module],
+                                )
+                                .unwrap();
                         };
                     } else {
-                        visualizer.snapshot_combined("unit solved".to_string(), vec![interface_ptr, dual_module, primal_module]).unwrap();
+                        visualizer
+                            .snapshot_combined("unit solved".to_string(), vec![interface_ptr, dual_module, primal_module])
+                            .unwrap();
                     }
-                });
+                },
+            );
             let last_unit = self.units.last().unwrap().read_recursive();
-            visualizer.snapshot_combined("solved".to_string(), vec![&last_unit.interface_ptr, parallel_dual_module, self]).unwrap();
+            visualizer
+                .snapshot_combined(
+                    "solved".to_string(),
+                    vec![&last_unit.interface_ptr, parallel_dual_module, self],
+                )
+                .unwrap();
         } else {
             self.parallel_solve(syndrome_pattern, parallel_dual_module);
         }
     }
 
-    pub fn parallel_solve_step_callback<DualSerialModule: DualModuleImpl + Send + Sync, F: Send + Sync>
-            (&mut self, syndrome_pattern: &SyndromePattern, parallel_dual_module: &mut DualModuleParallel<DualSerialModule>, mut callback: F)
-            where F: FnMut(&DualModuleInterfacePtr, &DualModuleParallelUnit<DualSerialModule>, &PrimalModuleSerialPtr, Option<&GroupMaxUpdateLength>) {
+    pub fn parallel_solve_step_callback<DualSerialModule: DualModuleImpl + Send + Sync, F: Send + Sync>(
+        &mut self,
+        syndrome_pattern: &SyndromePattern,
+        parallel_dual_module: &mut DualModuleParallel<DualSerialModule>,
+        mut callback: F,
+    ) where
+        F: FnMut(
+            &DualModuleInterfacePtr,
+            &DualModuleParallelUnit<DualSerialModule>,
+            &PrimalModuleSerialPtr,
+            Option<&GroupMaxUpdateLength>,
+        ),
+    {
         let thread_pool = Arc::clone(&self.thread_pool);
-        self.last_solve_start_time = Instant::now();
+        *self.last_solve_start_time.write() = Instant::now();
         if self.config.prioritize_base_partition {
             if self.config.debug_sequential {
                 for unit_index in 0..self.partition_info.units.len() {
                     let unit_ptr = self.units[unit_index].clone();
-                    unit_ptr.children_ready_solve::<DualSerialModule, F>(self, PartitionedSyndromePattern::new(syndrome_pattern)
-                        , parallel_dual_module, &mut Some(&mut callback));
+                    unit_ptr.children_ready_solve::<DualSerialModule, F>(
+                        self,
+                        PartitionedSyndromePattern::new(syndrome_pattern),
+                        parallel_dual_module,
+                        &mut Some(&mut callback),
+                    );
                 }
             } else {
+                use std::sync::atomic::{AtomicUsize, Ordering};
                 let ready_vec: Vec<_> = {
-                    (0..self.partition_info.units.len()).map(|_| Arc::new((Mutex::new(false), Condvar::new()))).collect()
+                    (0..self.partition_info.units.len())
+                        .map(|_| Arc::new((Mutex::new(false), Condvar::new(), Arc::new(AtomicUsize::new(0)))))
+                        .collect()
                 };
                 thread_pool.scope_fifo(|s| {
-                    for unit_index in 0..self.partition_info.units.len() {
+                    let issue_unit = |unit_index: usize| {
                         let ready_vec = &ready_vec;
                         let units = &self.units;
                         let partition_info = &self.partition_info;
                         let parallel_unit = &self;
                         let parallel_dual_module = &parallel_dual_module;
+                        let streaming_decode_use_spin_lock = self.config.streaming_decode_use_spin_lock;
                         s.spawn_fifo(move |_| {
                             let ready_pair = ready_vec[unit_index].clone();
-                            let &(ref ready, ref condvar) = &*ready_pair;
-                            let mut is_ready = ready.lock().unwrap();
-                            let unit_ptr = units[unit_index].clone();
-                            if unit_index >= partition_info.config.partitions.len() {  // wait for children to complete
-                                let fusion_index = unit_index - partition_info.config.partitions.len();
-                                let (left_unit_index, right_unit_index) = partition_info.config.fusions[fusion_index];
-                                for child_unit_index in [left_unit_index, right_unit_index] {
-                                    let child_ready_pair = ready_vec[child_unit_index].clone();
-                                    let &(ref child_ready, ref child_condvar) = &*child_ready_pair;
-                                    let mut child_is_ready = child_ready.lock().unwrap();
-                                    while !*child_is_ready {  // hopefully this asserts false at the beginning
-                                        child_is_ready = child_condvar.wait(child_is_ready).unwrap();
+                            let (ready, condvar, spin_ready) = &*ready_pair;
+                            if streaming_decode_use_spin_lock {
+                                let unit_ptr = units[unit_index].clone();
+                                if unit_index >= partition_info.config.partitions.len() {
+                                    // wait for children to complete
+                                    let fusion_index = unit_index - partition_info.config.partitions.len();
+                                    let (left_unit_index, right_unit_index) = partition_info.config.fusions[fusion_index];
+                                    for child_unit_index in [left_unit_index, right_unit_index] {
+                                        let child_ready_pair = ready_vec[child_unit_index].clone();
+                                        let (_, _, child_spin_ready) = &*child_ready_pair;
+                                        while child_spin_ready.load(Ordering::SeqCst) != 1 {
+                                            // hopefully this asserts false at the beginning
+                                            std::hint::spin_loop();
+                                            // println!("spin_loop");
+                                        }
+                                    }
+                                }
+                                unit_ptr.children_ready_solve::<DualSerialModule, F>(
+                                    parallel_unit,
+                                    PartitionedSyndromePattern::new(syndrome_pattern),
+                                    parallel_dual_module,
+                                    &mut None,
+                                );
+                                spin_ready.store(1, Ordering::SeqCst);
+                            } else {
+                                let mut is_ready = ready.lock().unwrap();
+                                let unit_ptr = units[unit_index].clone();
+                                if unit_index >= partition_info.config.partitions.len() {
+                                    // wait for children to complete
+                                    let fusion_index = unit_index - partition_info.config.partitions.len();
+                                    let (left_unit_index, right_unit_index) = partition_info.config.fusions[fusion_index];
+                                    for child_unit_index in [left_unit_index, right_unit_index] {
+                                        let child_ready_pair = ready_vec[child_unit_index].clone();
+                                        let (child_ready, child_condvar, _) = &*child_ready_pair;
+                                        let mut child_is_ready = child_ready.lock().unwrap();
+                                        while !*child_is_ready {
+                                            // hopefully this asserts false at the beginning
+                                            child_is_ready = child_condvar.wait(child_is_ready).unwrap();
+                                        }
                                     }
                                 }
+                                unit_ptr.children_ready_solve::<DualSerialModule, F>(
+                                    parallel_unit,
+                                    PartitionedSyndromePattern::new(syndrome_pattern),
+                                    parallel_dual_module,
+                                    &mut None,
+                                );
+                                *is_ready = true;
+                                condvar.notify_one();
                             }
-                            unit_ptr.children_ready_solve::<DualSerialModule, F>(parallel_unit, PartitionedSyndromePattern::new(syndrome_pattern)
-                                , parallel_dual_module, &mut None);
-                            *is_ready = true;
-                            condvar.notify_one();
                         })
+                    };
+                    if self.config.interleaving_base_fusion >= self.partition_info.config.fusions.len() {
+                        for unit_index in 0..self.partition_info.units.len() {
+                            issue_unit(unit_index);
+                        }
+                    } else {
+                        for unit_index in 0..self.partition_info.config.partitions.len() {
+                            if unit_index >= self.config.interleaving_base_fusion {
+                                let fusion_index = self.partition_info.config.partitions.len()
+                                    + (unit_index - self.config.interleaving_base_fusion);
+                                issue_unit(fusion_index);
+                            }
+                            issue_unit(unit_index);
+                        }
+                        for bias_index in 1..self.config.interleaving_base_fusion {
+                            issue_unit(self.partition_info.units.len() - self.config.interleaving_base_fusion + bias_index);
+                        }
                     }
                 });
             }
         } else {
             let last_unit_ptr = self.units.last().unwrap().clone();
             thread_pool.scope(|_| {
-                last_unit_ptr.iterative_solve_step_callback(self, PartitionedSyndromePattern::new(syndrome_pattern), parallel_dual_module, &mut Some(&mut callback))
+                last_unit_ptr.iterative_solve_step_callback(
+                    self,
+                    PartitionedSyndromePattern::new(syndrome_pattern),
+                    parallel_dual_module,
+                    &mut Some(&mut callback),
+                )
             })
         }
     }
-
 }
 
 impl FusionVisualizer for PrimalModuleParallel {
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         // do the sanity check first before taking snapshot
         // self.sanity_check().unwrap();
         let mut value = json!({});
         for unit_ptr in self.units.iter() {
             let unit = unit_ptr.read_recursive();
-            if !unit.is_active { continue }  // do not visualize inactive units
+            if !unit.is_active {
+                continue;
+            } // do not visualize inactive units
             let value_2 = unit.snapshot(abbrev);
             snapshot_combine_values(&mut value, value_2, abbrev);
         }
         value
     }
 }
 
 impl FusionVisualizer for PrimalModuleParallelUnit {
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         self.serial_module.snapshot(abbrev)
     }
 }
 
 impl PrimalModuleParallelUnitPtr {
-
     /// create a simple wrapper over a serial dual module
     pub fn new_wrapper(serial_module: PrimalModuleSerialPtr, unit_index: usize, partition_info: Arc<PartitionInfo>) -> Self {
         let partition_unit_info = &partition_info.units[unit_index];
         let is_active = partition_unit_info.children.is_none();
         let interface_ptr = DualModuleInterfacePtr::new_empty();
         interface_ptr.write().unit_index = unit_index;
         Self::new_value(PrimalModuleParallelUnit {
             unit_index,
             interface_ptr,
             partition_info,
-            is_active,  // only activate the leaves in the dependency tree
+            is_active, // only activate the leaves in the dependency tree
             serial_module,
-            children: None,  // to be filled later
-            parent: None,  // to be filled later
+            children: None, // to be filled later
+            parent: None,   // to be filled later
             event_time: None,
+            streaming_decode_mocker: None,
         })
     }
 
     /// call this only if children is guaranteed to be ready and solved
-    fn children_ready_solve<DualSerialModule: DualModuleImpl + Send + Sync, F: Send + Sync>(&self, primal_module_parallel: &PrimalModuleParallel
-                , partitioned_syndrome_pattern: PartitionedSyndromePattern, parallel_dual_module: &DualModuleParallel<DualSerialModule>, callback: &mut Option<&mut F>)
-            where F: FnMut(&DualModuleInterfacePtr, &DualModuleParallelUnit<DualSerialModule>, &PrimalModuleSerialPtr, Option<&GroupMaxUpdateLength>) {
-        let mut event_time = PrimalModuleParallelUnitEventTime::new();
-        event_time.start = primal_module_parallel.last_solve_start_time.elapsed().as_secs_f64();
+    #[allow(clippy::unnecessary_cast)]
+    fn children_ready_solve<DualSerialModule: DualModuleImpl + Send + Sync, F: Send + Sync>(
+        &self,
+        primal_module_parallel: &PrimalModuleParallel,
+        partitioned_syndrome_pattern: PartitionedSyndromePattern,
+        parallel_dual_module: &DualModuleParallel<DualSerialModule>,
+        callback: &mut Option<&mut F>,
+    ) where
+        F: FnMut(
+            &DualModuleInterfacePtr,
+            &DualModuleParallelUnit<DualSerialModule>,
+            &PrimalModuleSerialPtr,
+            Option<&GroupMaxUpdateLength>,
+        ),
+    {
         let mut primal_unit = self.write();
+        if let Some(mocker) = &primal_unit.streaming_decode_mocker {
+            if primal_module_parallel.config.streaming_decode_use_spin_lock {
+                while primal_module_parallel.last_solve_start_time.read_recursive().elapsed() < mocker.bias {
+                    std::hint::spin_loop(); // spin to avoid context switch
+                }
+            } else {
+                let mut elapsed = primal_module_parallel.last_solve_start_time.read_recursive().elapsed();
+                while elapsed < mocker.bias {
+                    std::thread::sleep(mocker.bias - elapsed);
+                    elapsed = primal_module_parallel.last_solve_start_time.read_recursive().elapsed();
+                }
+            }
+        }
+        let mut event_time = PrimalModuleParallelUnitEventTime::new();
+        event_time.start = primal_module_parallel
+            .last_solve_start_time
+            .read_recursive()
+            .elapsed()
+            .as_secs_f64();
         let dual_module_ptr = parallel_dual_module.get_unit(primal_unit.unit_index);
         let mut dual_unit = dual_module_ptr.write();
         let partition_unit_info = &primal_unit.partition_info.units[primal_unit.unit_index];
         let (owned_defect_range, _) = partitioned_syndrome_pattern.partition(partition_unit_info);
         let interface_ptr = primal_unit.interface_ptr.clone();
         if let Some((left_child_weak, right_child_weak)) = primal_unit.children.as_ref() {
-            {  // set children to inactive to avoid being solved twice
+            {
+                // set children to inactive to avoid being solved twice
                 for child_weak in [left_child_weak, right_child_weak] {
                     let child_ptr = child_weak.upgrade_force();
                     let mut child = child_ptr.write();
                     debug_assert!(child.is_active, "cannot fuse inactive children");
                     child.is_active = false;
                 }
             }
             primal_unit.fuse(&mut dual_unit);
-            if let Some(callback) = callback.as_mut() {  // do callback before actually breaking the matched pairs, for ease of visualization
+            if let Some(callback) = callback.as_mut() {
+                // do callback before actually breaking the matched pairs, for ease of visualization
                 callback(&primal_unit.interface_ptr, &dual_unit, &primal_unit.serial_module, None);
             }
             primal_unit.break_matching_with_mirror(dual_unit.deref_mut());
             for defect_index in owned_defect_range.whole_defect_range.iter() {
                 let defect_vertex = partitioned_syndrome_pattern.syndrome_pattern.defect_vertices[defect_index as usize];
-                primal_unit.serial_module.load_defect(defect_vertex, &interface_ptr, dual_unit.deref_mut());
-            }
-            primal_unit.serial_module.solve_step_callback_interface_loaded(&interface_ptr, dual_unit.deref_mut()
-                , |interface, dual_module, primal_module, group_max_update_length| {
+                primal_unit
+                    .serial_module
+                    .load_defect(defect_vertex, &interface_ptr, dual_unit.deref_mut());
+            }
+            primal_unit.serial_module.solve_step_callback_interface_loaded(
+                &interface_ptr,
+                dual_unit.deref_mut(),
+                |interface, dual_module, primal_module, group_max_update_length| {
                     if let Some(callback) = callback.as_mut() {
                         callback(interface, dual_module, primal_module, Some(group_max_update_length));
                     }
-                });
+                },
+            );
             if let Some(callback) = callback.as_mut() {
                 callback(&primal_unit.interface_ptr, &dual_unit, &primal_unit.serial_module, None);
             }
         } else {
             debug_assert!(primal_unit.is_active, "leaf must be active to be solved");
             let syndrome_pattern = owned_defect_range.expand();
-            primal_unit.serial_module.solve_step_callback(&interface_ptr, &syndrome_pattern, dual_unit.deref_mut()
-                , |interface, dual_module, primal_module, group_max_update_length| {
+            primal_unit.serial_module.solve_step_callback(
+                &interface_ptr,
+                &syndrome_pattern,
+                dual_unit.deref_mut(),
+                |interface, dual_module, primal_module, group_max_update_length| {
                     if let Some(callback) = callback.as_mut() {
                         callback(interface, dual_module, primal_module, Some(group_max_update_length));
                     }
-                });
+                },
+            );
             if let Some(callback) = callback.as_mut() {
                 callback(&primal_unit.interface_ptr, &dual_unit, &primal_unit.serial_module, None);
             }
         }
         primal_unit.is_active = true;
-        event_time.end = primal_module_parallel.last_solve_start_time.elapsed().as_secs_f64();
+        event_time.end = primal_module_parallel
+            .last_solve_start_time
+            .read_recursive()
+            .elapsed()
+            .as_secs_f64();
         primal_unit.event_time = Some(event_time);
     }
 
     /// call on the last primal node, and it will spawn tasks on the previous ones
-    fn iterative_solve_step_callback<DualSerialModule: DualModuleImpl + Send + Sync, F: Send + Sync>(&self, primal_module_parallel: &PrimalModuleParallel
-                , partitioned_syndrome_pattern: PartitionedSyndromePattern, parallel_dual_module: &DualModuleParallel<DualSerialModule>, callback: &mut Option<&mut F>)
-            where F: FnMut(&DualModuleInterfacePtr, &DualModuleParallelUnit<DualSerialModule>, &PrimalModuleSerialPtr, Option<&GroupMaxUpdateLength>) {
+    fn iterative_solve_step_callback<DualSerialModule: DualModuleImpl + Send + Sync, F: Send + Sync>(
+        &self,
+        primal_module_parallel: &PrimalModuleParallel,
+        partitioned_syndrome_pattern: PartitionedSyndromePattern,
+        parallel_dual_module: &DualModuleParallel<DualSerialModule>,
+        callback: &mut Option<&mut F>,
+    ) where
+        F: FnMut(
+            &DualModuleInterfacePtr,
+            &DualModuleParallelUnit<DualSerialModule>,
+            &PrimalModuleSerialPtr,
+            Option<&GroupMaxUpdateLength>,
+        ),
+    {
         let primal_unit = self.read_recursive();
         // only when sequentially running the tasks will the callback take effect, otherwise it's unsafe to execute it from multiple threads
         let debug_sequential = primal_module_parallel.config.debug_sequential;
-        if let Some((left_child_weak, right_child_weak)) = primal_unit.children.as_ref() {  // make children ready
-            debug_assert!(!primal_unit.is_active, "parent must be inactive at the time of solving children");
+        if let Some((left_child_weak, right_child_weak)) = primal_unit.children.as_ref() {
+            // make children ready
+            debug_assert!(
+                !primal_unit.is_active,
+                "parent must be inactive at the time of solving children"
+            );
             let partition_unit_info = &primal_unit.partition_info.units[primal_unit.unit_index];
             let (_, (left_partitioned, right_partitioned)) = partitioned_syndrome_pattern.partition(partition_unit_info);
             if debug_sequential {
-                left_child_weak.upgrade_force().iterative_solve_step_callback(primal_module_parallel, left_partitioned
-                    , parallel_dual_module, callback);
-                right_child_weak.upgrade_force().iterative_solve_step_callback(primal_module_parallel, right_partitioned
-                    , parallel_dual_module, callback);
+                left_child_weak.upgrade_force().iterative_solve_step_callback(
+                    primal_module_parallel,
+                    left_partitioned,
+                    parallel_dual_module,
+                    callback,
+                );
+                right_child_weak.upgrade_force().iterative_solve_step_callback(
+                    primal_module_parallel,
+                    right_partitioned,
+                    parallel_dual_module,
+                    callback,
+                );
             } else {
-                rayon::join(|| {
-                    left_child_weak.upgrade_force().iterative_solve_step_callback::<DualSerialModule, F>(primal_module_parallel, left_partitioned
-                        , parallel_dual_module, &mut None)
-                }, || {
-                    right_child_weak.upgrade_force().iterative_solve_step_callback::<DualSerialModule, F>(primal_module_parallel, right_partitioned
-                        , parallel_dual_module, &mut None)
-                });
+                rayon::join(
+                    || {
+                        left_child_weak
+                            .upgrade_force()
+                            .iterative_solve_step_callback::<DualSerialModule, F>(
+                                primal_module_parallel,
+                                left_partitioned,
+                                parallel_dual_module,
+                                &mut None,
+                            )
+                    },
+                    || {
+                        right_child_weak
+                            .upgrade_force()
+                            .iterative_solve_step_callback::<DualSerialModule, F>(
+                                primal_module_parallel,
+                                right_partitioned,
+                                parallel_dual_module,
+                                &mut None,
+                            )
+                    },
+                );
             };
         }
         drop(primal_unit);
-        self.children_ready_solve(primal_module_parallel, partitioned_syndrome_pattern, parallel_dual_module, callback);
+        self.children_ready_solve(
+            primal_module_parallel,
+            partitioned_syndrome_pattern,
+            parallel_dual_module,
+            callback,
+        );
     }
-
 }
 
 impl PrimalModuleParallelUnit {
-
     /// fuse two units together, by copying the right child's content into the left child's content and resolve index;
     /// note that this operation doesn't update on the dual module, call [`Self::break_matching_with_mirror`] if needed
-    pub fn fuse<DualSerialModule: DualModuleImpl + Send + Sync>(&mut self, dual_unit: &mut DualModuleParallelUnit<DualSerialModule>) {
-        let (left_child_ptr, right_child_ptr) = (self.children.as_ref().unwrap().0.upgrade_force(), self.children.as_ref().unwrap().1.upgrade_force());
+    pub fn fuse<DualSerialModule: DualModuleImpl + Send + Sync>(
+        &mut self,
+        dual_unit: &mut DualModuleParallelUnit<DualSerialModule>,
+    ) {
+        let (left_child_ptr, right_child_ptr) = (
+            self.children.as_ref().unwrap().0.upgrade_force(),
+            self.children.as_ref().unwrap().1.upgrade_force(),
+        );
         let left_child = left_child_ptr.read_recursive();
         let right_child = right_child_ptr.read_recursive();
         dual_unit.fuse(&self.interface_ptr, (&left_child.interface_ptr, &right_child.interface_ptr));
         self.serial_module.fuse(&left_child.serial_module, &right_child.serial_module);
     }
 
     /// break the matched pairs of interface vertices
+    #[allow(clippy::unnecessary_cast)]
     pub fn break_matching_with_mirror(&mut self, dual_module: &mut impl DualModuleImpl) {
         // use `possible_break` to efficiently break those
         let mut possible_break = vec![];
         let module = self.serial_module.read_recursive();
         for node_index in module.possible_break.iter() {
             let primal_node_ptr = module.get_node(*node_index);
             if let Some(primal_node_ptr) = primal_node_ptr {
                 let mut primal_node = primal_node_ptr.write();
                 if let Some((MatchTarget::VirtualVertex(vertex_index), _)) = &primal_node.temporary_match {
                     if self.partition_info.vertex_to_owning_unit[*vertex_index as usize] == self.unit_index {
                         primal_node.temporary_match = None;
-                        self.interface_ptr.set_grow_state(&primal_node.origin.upgrade_force(), DualNodeGrowState::Grow, dual_module);
-                    } else {  // still possible break
+                        self.interface_ptr.set_grow_state(
+                            &primal_node.origin.upgrade_force(),
+                            DualNodeGrowState::Grow,
+                            dual_module,
+                        );
+                    } else {
+                        // still possible break
                         possible_break.push(*node_index);
                     }
                 }
             }
         }
         drop(module);
         self.serial_module.write().possible_break = possible_break;
     }
-
 }
 
 impl PrimalModuleImpl for PrimalModuleParallelUnit {
-
     fn new_empty(_initializer: &SolverInitializer) -> Self {
         panic!("creating parallel unit directly from initializer is forbidden, use `PrimalModuleParallel::new` instead");
     }
 
     fn clear(&mut self) {
         self.serial_module.clear();
         self.interface_ptr.clear();
@@ -491,267 +739,380 @@
         self.serial_module.load(interface_ptr)
     }
 
     fn load_defect_dual_node(&mut self, dual_node_ptr: &DualNodePtr) {
         self.serial_module.load_defect_dual_node(dual_node_ptr)
     }
 
-    fn resolve<D: DualModuleImpl>(&mut self, group_max_update_length: GroupMaxUpdateLength, interface: &DualModuleInterfacePtr, dual_module: &mut D) {
+    fn resolve<D: DualModuleImpl>(
+        &mut self,
+        group_max_update_length: GroupMaxUpdateLength,
+        interface: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) {
         self.serial_module.resolve(group_max_update_length, interface, dual_module)
     }
 
-    fn intermediate_matching<D: DualModuleImpl>(&mut self, interface: &DualModuleInterfacePtr, dual_module: &mut D) -> IntermediateMatching {
+    fn intermediate_matching<D: DualModuleImpl>(
+        &mut self,
+        interface: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) -> IntermediateMatching {
         self.serial_module.intermediate_matching(interface, dual_module)
     }
-
 }
 
 #[cfg(test)]
 pub mod tests {
-    use super::*;
-    use super::super::example_codes::*;
     use super::super::dual_module_serial::*;
+    use super::super::example_codes::*;
+    use super::*;
 
-    pub fn primal_module_parallel_basic_standard_syndrome_optional_viz<F>(mut code: impl ExampleCode, visualize_filename: Option<String>
-            , mut defect_vertices: Vec<VertexIndex>, final_dual: Weight, partition_func: F, reordered_vertices: Option<Vec<VertexIndex>>)
-            -> (PrimalModuleParallel, DualModuleParallel<DualModuleSerial>) where F: Fn(&SolverInitializer, &mut PartitionConfig) {
+    pub fn primal_module_parallel_basic_standard_syndrome_optional_viz<F>(
+        mut code: impl ExampleCode,
+        visualize_filename: Option<String>,
+        mut defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+        partition_func: F,
+        reordered_vertices: Option<Vec<VertexIndex>>,
+    ) -> (PrimalModuleParallel, DualModuleParallel<DualModuleSerial>)
+    where
+        F: Fn(&SolverInitializer, &mut PartitionConfig),
+    {
         println!("{defect_vertices:?}");
         if let Some(reordered_vertices) = &reordered_vertices {
             code.reorder_vertices(reordered_vertices);
             defect_vertices = translated_defect_to_reordered(reordered_vertices, &defect_vertices);
         }
         let mut visualizer = match visualize_filename.as_ref() {
             Some(visualize_filename) => {
-                let visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+                let visualizer = Visualizer::new(
+                    Some(visualize_data_folder() + visualize_filename.as_str()),
+                    code.get_positions(),
+                    true,
+                )
+                .unwrap();
                 print_visualize_link(visualize_filename.clone());
                 Some(visualizer)
-            }, None => None
+            }
+            None => None,
         };
         let initializer = code.get_initializer();
         let mut partition_config = PartitionConfig::new(initializer.vertex_num);
         partition_func(&initializer, &mut partition_config);
         let partition_info = partition_config.info();
-        let mut dual_module = DualModuleParallel::new_config(&initializer, &partition_info, DualModuleParallelConfig::default());
+        let mut dual_module =
+            DualModuleParallel::new_config(&initializer, &partition_info, DualModuleParallelConfig::default());
         let mut primal_config = PrimalModuleParallelConfig::default();
         primal_config.debug_sequential = true;
         let mut primal_module = PrimalModuleParallel::new_config(&initializer, &partition_info, primal_config);
         code.set_defect_vertices(&defect_vertices);
         primal_module.parallel_solve_visualizer(&code.get_syndrome(), &mut dual_module, visualizer.as_mut());
-        let useless_interface_ptr = DualModuleInterfacePtr::new_empty();  // don't actually use it
+        let useless_interface_ptr = DualModuleInterfacePtr::new_empty(); // don't actually use it
         let perfect_matching = primal_module.perfect_matching(&useless_interface_ptr, &mut dual_module);
         let mut subgraph_builder = SubGraphBuilder::new(&initializer);
         subgraph_builder.load_perfect_matching(&perfect_matching);
         let subgraph = subgraph_builder.get_subgraph();
         if let Some(visualizer) = visualizer.as_mut() {
             let last_interface_ptr = &primal_module.units.last().unwrap().read_recursive().interface_ptr;
-            visualizer.snapshot_combined("perfect matching and subgraph".to_string(), vec![last_interface_ptr, &dual_module
-                , &perfect_matching, &VisualizeSubgraph::new(&subgraph)]).unwrap();
+            visualizer
+                .snapshot_combined(
+                    "perfect matching and subgraph".to_string(),
+                    vec![
+                        last_interface_ptr,
+                        &dual_module,
+                        &perfect_matching,
+                        &VisualizeSubgraph::new(&subgraph),
+                    ],
+                )
+                .unwrap();
         }
-        let sum_dual_variables = primal_module.units.last().unwrap().read_recursive().interface_ptr.sum_dual_variables();
-        assert_eq!(sum_dual_variables, subgraph_builder.total_weight(), "unmatched sum dual variables");
+        let sum_dual_variables = primal_module
+            .units
+            .last()
+            .unwrap()
+            .read_recursive()
+            .interface_ptr
+            .sum_dual_variables();
+        assert_eq!(
+            sum_dual_variables,
+            subgraph_builder.total_weight(),
+            "unmatched sum dual variables"
+        );
         assert_eq!(sum_dual_variables, final_dual * 2, "unexpected final dual variable sum");
         (primal_module, dual_module)
     }
 
-    pub fn primal_module_parallel_standard_syndrome<F>(code: impl ExampleCode, visualize_filename: String, defect_vertices: Vec<VertexIndex>
-            , final_dual: Weight, partition_func: F, reordered_vertices: Option<Vec<VertexIndex>>)
-            -> (PrimalModuleParallel, DualModuleParallel<DualModuleSerial>) where F: Fn(&SolverInitializer, &mut PartitionConfig) {
-        primal_module_parallel_basic_standard_syndrome_optional_viz(code, Some(visualize_filename), defect_vertices, final_dual, partition_func, reordered_vertices)
+    pub fn primal_module_parallel_standard_syndrome<F>(
+        code: impl ExampleCode,
+        visualize_filename: String,
+        defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+        partition_func: F,
+        reordered_vertices: Option<Vec<VertexIndex>>,
+    ) -> (PrimalModuleParallel, DualModuleParallel<DualModuleSerial>)
+    where
+        F: Fn(&SolverInitializer, &mut PartitionConfig),
+    {
+        primal_module_parallel_basic_standard_syndrome_optional_viz(
+            code,
+            Some(visualize_filename),
+            defect_vertices,
+            final_dual,
+            partition_func,
+            reordered_vertices,
+        )
     }
 
     /// test a simple case
     #[test]
-    fn primal_module_parallel_basic_1() {  // cargo test primal_module_parallel_basic_1 -- --nocapture
+    fn primal_module_parallel_basic_1() {
+        // cargo test primal_module_parallel_basic_1 -- --nocapture
         let visualize_filename = format!("primal_module_parallel_basic_1.json");
         let defect_vertices = vec![39, 52, 63, 90, 100];
         let half_weight = 500;
-        primal_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |initializer, _config| {
-            println!("initializer: {initializer:?}");
-        }, None);
+        primal_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |initializer, _config| {
+                println!("initializer: {initializer:?}");
+            },
+            None,
+        );
     }
 
     /// split into 2, with no syndrome vertex on the interface
     #[test]
-    fn primal_module_parallel_basic_2() {  // cargo test primal_module_parallel_basic_2 -- --nocapture
+    fn primal_module_parallel_basic_2() {
+        // cargo test primal_module_parallel_basic_2 -- --nocapture
         let visualize_filename = format!("primal_module_parallel_basic_2.json");
         let defect_vertices = vec![39, 52, 63, 90, 100];
         let half_weight = 500;
-        primal_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 72),    // unit 0
-                VertexRange::new(84, 132),  // unit 1
-            ];
-            config.fusions = vec![
-                (0, 1),  // unit 2, by fusing 0 and 1
-            ];
-        }, None);
+        primal_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 72),   // unit 0
+                    VertexRange::new(84, 132), // unit 1
+                ];
+                config.fusions = vec![
+                    (0, 1), // unit 2, by fusing 0 and 1
+                ];
+            },
+            None,
+        );
     }
 
     /// split into 2, with a syndrome vertex on the interface
     #[test]
-    fn primal_module_parallel_basic_3() {  // cargo test primal_module_parallel_basic_3 -- --nocapture
+    fn primal_module_parallel_basic_3() {
+        // cargo test primal_module_parallel_basic_3 -- --nocapture
         let visualize_filename = format!("primal_module_parallel_basic_3.json");
         let defect_vertices = vec![39, 52, 63, 90, 100];
         let half_weight = 500;
-        primal_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 60),    // unit 0
-                VertexRange::new(72, 132),  // unit 1
-            ];
-            config.fusions = vec![
-                (0, 1),  // unit 2, by fusing 0 and 1
-            ];
-        }, None);
+        primal_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 60),   // unit 0
+                    VertexRange::new(72, 132), // unit 1
+                ];
+                config.fusions = vec![
+                    (0, 1), // unit 2, by fusing 0 and 1
+                ];
+            },
+            None,
+        );
     }
 
     /// split into 4, with no syndrome vertex on the interface
     #[test]
-    fn primal_module_parallel_basic_4() {  // cargo test primal_module_parallel_basic_4 -- --nocapture
+    fn primal_module_parallel_basic_4() {
+        // cargo test primal_module_parallel_basic_4 -- --nocapture
         let visualize_filename = format!("primal_module_parallel_basic_4.json");
         // reorder vertices to enable the partition;
-        let defect_vertices = vec![39, 52, 63, 90, 100];  // indices are before the reorder
+        let defect_vertices = vec![39, 52, 63, 90, 100]; // indices are before the reorder
         let half_weight = 500;
-        primal_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 36),
-                VertexRange::new(42, 72),
-                VertexRange::new(84, 108),
-                VertexRange::new(112, 132),
-            ];
-            config.fusions = vec![
-                (0, 1),
-                (2, 3),
-                (4, 5),
-            ];
-        }, Some((|| {
-            let mut reordered_vertices = vec![];
-            let split_horizontal = 6;
-            let split_vertical = 5;
-            for i in 0..split_horizontal {  // left-top block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
-                }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in 0..split_horizontal {  // interface between the left-top block and the right-top block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in 0..split_horizontal {  // right-top block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
-                }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            {  // the big interface between top and bottom
-                for j in 0..12 {
-                    reordered_vertices.push(split_horizontal * 12 + j);
-                }
-            }
-            for i in (split_horizontal+1)..11 {  // left-bottom block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
-                }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in (split_horizontal+1)..11 {  // interface between the left-bottom block and the right-bottom block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in (split_horizontal+1)..11 {  // right-bottom block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
+        primal_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 36),
+                    VertexRange::new(42, 72),
+                    VertexRange::new(84, 108),
+                    VertexRange::new(112, 132),
+                ];
+                config.fusions = vec![(0, 1), (2, 3), (4, 5)];
+            },
+            Some((|| {
+                let mut reordered_vertices = vec![];
+                let split_horizontal = 6;
+                let split_vertical = 5;
+                for i in 0..split_horizontal {
+                    // left-top block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
                 }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            reordered_vertices
-        })()));
+                for i in 0..split_horizontal {
+                    // interface between the left-top block and the right-top block
+                    reordered_vertices.push(i * 12 + split_vertical);
+                }
+                for i in 0..split_horizontal {
+                    // right-top block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
+                }
+                {
+                    // the big interface between top and bottom
+                    for j in 0..12 {
+                        reordered_vertices.push(split_horizontal * 12 + j);
+                    }
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // left-bottom block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // interface between the left-bottom block and the right-bottom block
+                    reordered_vertices.push(i * 12 + split_vertical);
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // right-bottom block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
+                }
+                reordered_vertices
+            })()),
+        );
     }
 
     /// split into 4, with 2 defect vertices on parent interfaces
     #[test]
-    fn primal_module_parallel_basic_5() {  // cargo test primal_module_parallel_basic_5 -- --nocapture
+    fn primal_module_parallel_basic_5() {
+        // cargo test primal_module_parallel_basic_5 -- --nocapture
         let visualize_filename = format!("primal_module_parallel_basic_5.json");
         // reorder vertices to enable the partition;
-        let defect_vertices = vec![39, 52, 63, 90, 100];  // indices are before the reorder
+        let defect_vertices = vec![39, 52, 63, 90, 100]; // indices are before the reorder
         let half_weight = 500;
-        primal_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(11, 0.1, half_weight), visualize_filename, defect_vertices, 9 * half_weight, |_initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, 25),
-                VertexRange::new(30, 60),
-                VertexRange::new(72, 97),
-                VertexRange::new(102, 132),
-            ];
-            config.fusions = vec![
-                (0, 1),
-                (2, 3),
-                (4, 5),
-            ];
-        }, Some((|| {
-            let mut reordered_vertices = vec![];
-            let split_horizontal = 5;
-            let split_vertical = 4;
-            for i in 0..split_horizontal {  // left-top block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
-                }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in 0..split_horizontal {  // interface between the left-top block and the right-top block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in 0..split_horizontal {  // right-top block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
-                }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            {  // the big interface between top and bottom
-                for j in 0..12 {
-                    reordered_vertices.push(split_horizontal * 12 + j);
-                }
-            }
-            for i in (split_horizontal+1)..11 {  // left-bottom block
-                for j in 0..split_vertical {
-                    reordered_vertices.push(i * 12 + j);
-                }
-                reordered_vertices.push(i * 12 + 11);
-            }
-            for i in (split_horizontal+1)..11 {  // interface between the left-bottom block and the right-bottom block
-                reordered_vertices.push(i * 12 + split_vertical);
-            }
-            for i in (split_horizontal+1)..11 {  // right-bottom block
-                for j in (split_vertical+1)..10 {
-                    reordered_vertices.push(i * 12 + j);
+        primal_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(11, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            9 * half_weight,
+            |_initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, 25),
+                    VertexRange::new(30, 60),
+                    VertexRange::new(72, 97),
+                    VertexRange::new(102, 132),
+                ];
+                config.fusions = vec![(0, 1), (2, 3), (4, 5)];
+            },
+            Some((|| {
+                let mut reordered_vertices = vec![];
+                let split_horizontal = 5;
+                let split_vertical = 4;
+                for i in 0..split_horizontal {
+                    // left-top block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
                 }
-                reordered_vertices.push(i * 12 + 10);
-            }
-            reordered_vertices
-        })()));
+                for i in 0..split_horizontal {
+                    // interface between the left-top block and the right-top block
+                    reordered_vertices.push(i * 12 + split_vertical);
+                }
+                for i in 0..split_horizontal {
+                    // right-top block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
+                }
+                {
+                    // the big interface between top and bottom
+                    for j in 0..12 {
+                        reordered_vertices.push(split_horizontal * 12 + j);
+                    }
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // left-bottom block
+                    for j in 0..split_vertical {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 11);
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // interface between the left-bottom block and the right-bottom block
+                    reordered_vertices.push(i * 12 + split_vertical);
+                }
+                for i in (split_horizontal + 1)..11 {
+                    // right-bottom block
+                    for j in (split_vertical + 1)..10 {
+                        reordered_vertices.push(i * 12 + j);
+                    }
+                    reordered_vertices.push(i * 12 + 10);
+                }
+                reordered_vertices
+            })()),
+        );
     }
 
-    fn primal_module_parallel_debug_planar_code_common(d: VertexNum, visualize_filename: String, defect_vertices: Vec<VertexIndex>, final_dual: Weight) {
+    fn primal_module_parallel_debug_planar_code_common(
+        d: VertexNum,
+        visualize_filename: String,
+        defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+    ) {
         let half_weight = 500;
         let split_horizontal = (d + 1) / 2;
         let row_count = d + 1;
-        primal_module_parallel_standard_syndrome(CodeCapacityPlanarCode::new(d, 0.1, half_weight), visualize_filename, defect_vertices, final_dual * half_weight, |initializer, config| {
-            config.partitions = vec![
-                VertexRange::new(0, split_horizontal * row_count),
-                VertexRange::new((split_horizontal + 1) * row_count, initializer.vertex_num),
-            ];
-            config.fusions = vec![
-                (0, 1),
-            ];
-        }, None);
+        primal_module_parallel_standard_syndrome(
+            CodeCapacityPlanarCode::new(d, 0.1, half_weight),
+            visualize_filename,
+            defect_vertices,
+            final_dual * half_weight,
+            |initializer, config| {
+                config.partitions = vec![
+                    VertexRange::new(0, split_horizontal * row_count),
+                    VertexRange::new((split_horizontal + 1) * row_count, initializer.vertex_num),
+                ];
+                config.fusions = vec![(0, 1)];
+            },
+            None,
+        );
     }
 
     /// 68000 vs 69000 dual variable: probably missing some interface node
     /// panicked at 'vacating a non-boundary vertex is forbidden', src/dual_module_serial.rs:899:25
     /// reason: when executing sync events, I forgot to add the new propagated dual module to the active list;
     /// why it didn't show up before: because usually a node is created when executing sync event, in which case it's automatically in the active list
-    /// if this node already exists before, and it's again synchronized, then it's not in the active list, leading to strange growth 
+    /// if this node already exists before, and it's again synchronized, then it's not in the active list, leading to strange growth
     #[test]
-    fn primal_module_parallel_debug_1() {  // cargo test primal_module_parallel_debug_1 -- --nocapture
+    fn primal_module_parallel_debug_1() {
+        // cargo test primal_module_parallel_debug_1 -- --nocapture
         let visualize_filename = format!("primal_module_parallel_debug_1.json");
-        let defect_vertices = vec![88, 89, 102, 103, 105, 106, 118, 120, 122, 134, 138];  // indices are before the reorder
+        let defect_vertices = vec![88, 89, 102, 103, 105, 106, 118, 120, 122, 134, 138]; // indices are before the reorder
         primal_module_parallel_debug_planar_code_common(15, visualize_filename, defect_vertices, 10);
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/src/primal_module_serial.rs` & `fusion_blossom-0.2.5/src/primal_module_serial.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 //! Serial Primal Module
-//! 
+//!
 //! A serial implementation of the primal module. This is the very basic fusion blossom algorithm that aims at debugging and as a ground truth
 //! where traditional matching is too time consuming because of their |E| = O(|V|^2) scaling.
 //!
 
-use super::util::*;
-use crate::derivative::Derivative;
+#![cfg_attr(feature = "unsafe_pointer", allow(dropping_references))]
+use super::dual_module::*;
+use super::pointers::*;
 use super::primal_module::*;
+use super::util::*;
 use super::visualize::*;
-use super::dual_module::*;
+use crate::derivative::Derivative;
 use std::cmp::Ordering;
-use super::pointers::*;
-
 
 #[derive(Derivative)]
 #[derivative(Debug)]
 pub struct PrimalModuleSerial {
     /// unit index of this interface, default to 0
     pub unit_index: usize,
     /// nodes internal information
@@ -90,56 +90,60 @@
 }
 
 pub type PrimalNodeInternalPtr = ArcManualSafeLock<PrimalNodeInternal>;
 pub type PrimalNodeInternalWeak = WeakManualSafeLock<PrimalNodeInternal>;
 
 impl std::fmt::Debug for PrimalNodeInternalPtr {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
-        self.update();  // to make sure index is up-to-date
+        self.update(); // to make sure index is up-to-date
         let primal_node_internal = self.read_recursive();
         write!(f, "{}", primal_node_internal.index)
     }
 }
 
 impl std::fmt::Debug for PrimalNodeInternalWeak {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         self.upgrade_force().fmt(f)
     }
 }
 
 impl PrimalNodeInternal {
-
     /// check if in the cache, this node is a free node
     pub fn is_free(&self) -> bool {
-        debug_assert!({
-            let origin_ptr = self.origin.upgrade_force();
-            let node = origin_ptr.read_recursive();
-            node.parent_blossom.is_none()
-        }, "do not call this function to a internal node, consider call PrimalModuleSerial::get_outer_node");
-        if self.tree_node.is_some() { return false }  // this node belongs to an alternating tree
-        if self.temporary_match.is_some() { return false }  // already temporarily matched
+        debug_assert!(
+            {
+                let origin_ptr = self.origin.upgrade_force();
+                let node = origin_ptr.read_recursive();
+                node.parent_blossom.is_none()
+            },
+            "do not call this function to a internal node, consider call PrimalModuleSerial::get_outer_node"
+        );
+        if self.tree_node.is_some() {
+            return false;
+        } // this node belongs to an alternating tree
+        if self.temporary_match.is_some() {
+            return false;
+        } // already temporarily matched
         true
     }
 
     /// modify the depth and root of a sub-tree using DFS
     pub fn change_sub_tree_root(&mut self, depth: usize, root: PrimalNodeInternalPtr) {
         let tree_node = self.tree_node.as_mut().unwrap();
         tree_node.depth = depth;
         tree_node.root = root.downgrade();
         for (child_weak, _) in tree_node.children.iter() {
             let child_ptr = child_weak.upgrade_force();
             lock_write!(child, child_ptr);
             child.change_sub_tree_root(depth + 1, root.clone());
         }
     }
-
 }
 
 impl PrimalNodeInternalPtr {
-
     /// when fused, primal node may be outdated; refresh here
     pub fn update(&self) -> &Self {
         let mut current_belonging = self.read_recursive().belonging.upgrade_force();
         let mut bias = 0;
         let mut node = self.write();
         while current_belonging.read_recursive().parent.is_some() {
             let belonging_module = current_belonging.read_recursive();
@@ -148,128 +152,187 @@
             drop(belonging_module);
             current_belonging = new_current_belonging;
         }
         node.belonging = current_belonging.downgrade();
         node.index += bias;
         self
     }
-
 }
 
 impl PrimalModuleImpl for PrimalModuleSerialPtr {
-
     fn new_empty(_initializer: &SolverInitializer) -> Self {
         Self::new_value(PrimalModuleSerial {
-            unit_index: 0,  // if necessary, manually change it
+            unit_index: 0, // if necessary, manually change it
             nodes: vec![],
             nodes_length: 0,
             is_fusion: false,
             possible_break: vec![],
             debug_resolve_only_one: false,
             parent: None,
             index_bias: 0,
             children: None,
         })
     }
 
     fn clear(&mut self) {
         let mut module = self.write();
-        module.nodes_length = 0;  // without actually dropping all the nodes, to enable constant time clear
+        module.nodes_length = 0; // without actually dropping all the nodes, to enable constant time clear
         module.possible_break.clear();
         module.is_fusion = false;
         module.parent = None;
         module.index_bias = 0;
         module.children = None;
     }
 
     fn load_defect_dual_node(&mut self, dual_node_ptr: &DualNodePtr) {
         let belonging = self.downgrade();
         let node = dual_node_ptr.read_recursive();
-        debug_assert!(matches!(node.class, DualNodeClass::DefectVertex{ .. }), "must load a fresh dual module interface, found a blossom");
+        debug_assert!(
+            matches!(node.class, DualNodeClass::DefectVertex { .. }),
+            "must load a fresh dual module interface, found a blossom"
+        );
         let mut module = self.write();
         let local_node_index = module.nodes_length;
         let node_index = module.nodes_count();
         debug_assert_eq!(node.index, node_index, "must load in order");
-        let primal_node_internal_ptr = if !module.is_fusion && local_node_index < module.nodes.len() && module.nodes[local_node_index].is_some() {
-            let node_ptr = module.nodes[local_node_index].take().unwrap();
-            let mut node = node_ptr.write();
-            node.origin = dual_node_ptr.downgrade();
-            node.index = node_index;
-            node.tree_node = None;
-            node.temporary_match = None;
-            node.belonging = belonging;
-            drop(node);
-            node_ptr
-        } else {
-            PrimalNodeInternalPtr::new_value(PrimalNodeInternal {
-                origin: dual_node_ptr.downgrade(),
-                index: node_index,
-                tree_node: None,
-                temporary_match: None,
-                belonging,
-            })
-        };
+        let primal_node_internal_ptr =
+            if !module.is_fusion && local_node_index < module.nodes.len() && module.nodes[local_node_index].is_some() {
+                let node_ptr = module.nodes[local_node_index].take().unwrap();
+                let mut node = node_ptr.write();
+                node.origin = dual_node_ptr.downgrade();
+                node.index = node_index;
+                node.tree_node = None;
+                node.temporary_match = None;
+                node.belonging = belonging;
+                drop(node);
+                node_ptr
+            } else {
+                PrimalNodeInternalPtr::new_value(PrimalNodeInternal {
+                    origin: dual_node_ptr.downgrade(),
+                    index: node_index,
+                    tree_node: None,
+                    temporary_match: None,
+                    belonging,
+                })
+            };
         module.nodes_length += 1;
         if module.nodes.len() < module.nodes_length {
             module.nodes.push(None);
         }
         module.nodes[local_node_index] = Some(primal_node_internal_ptr);
     }
 
     #[allow(clippy::collapsible_else_if)]
-    fn resolve<D: DualModuleImpl>(&mut self, mut group_max_update_length: GroupMaxUpdateLength, interface_ptr: &DualModuleInterfacePtr, dual_module: &mut D) {
+    fn resolve<D: DualModuleImpl>(
+        &mut self,
+        mut group_max_update_length: GroupMaxUpdateLength,
+        interface_ptr: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) {
         debug_assert!(!group_max_update_length.is_empty() && group_max_update_length.get_none_zero_growth().is_none());
         let mut current_conflict_index = 0;
         let debug_resolve_only_one = self.read_recursive().debug_resolve_only_one;
         while let Some(conflict) = group_max_update_length.pop() {
             current_conflict_index += 1;
-            if debug_resolve_only_one && current_conflict_index > 1 {  // debug mode
-                break
+            if debug_resolve_only_one && current_conflict_index > 1 {
+                // debug mode
+                break;
             }
             // println!("conflict: {conflict:?}");
             match conflict {
                 MaxUpdateLength::Conflicting((node_ptr_1, touching_ptr_1), (node_ptr_2, touching_ptr_2)) => {
-                    debug_assert!(node_ptr_1 != node_ptr_2, "one cannot conflict with itself, double check to avoid deadlock");
-                    if self.get_primal_node_internal_ptr_option(&node_ptr_1).is_none() { continue }  // ignore out-of-date event
-                    if self.get_primal_node_internal_ptr_option(&node_ptr_2).is_none() { continue }  // ignore out-of-date event
-                    // always use outer node in case it's already wrapped into a blossom
+                    debug_assert!(
+                        node_ptr_1 != node_ptr_2,
+                        "one cannot conflict with itself, double check to avoid deadlock"
+                    );
+                    if self.get_primal_node_internal_ptr_option(&node_ptr_1).is_none() {
+                        continue;
+                    } // ignore out-of-date event
+                    if self.get_primal_node_internal_ptr_option(&node_ptr_2).is_none() {
+                        continue;
+                    } // ignore out-of-date event
+                      // always use outer node in case it's already wrapped into a blossom
                     let primal_node_internal_ptr_1 = self.get_outer_node(self.get_primal_node_internal_ptr(&node_ptr_1));
                     let primal_node_internal_ptr_2 = self.get_outer_node(self.get_primal_node_internal_ptr(&node_ptr_2));
                     if primal_node_internal_ptr_1 == primal_node_internal_ptr_2 {
-                        debug_assert!(current_conflict_index != 1, "the first conflict cannot be ignored, otherwise may cause hidden infinite loop");
-                        continue  // this is no longer a conflict because both of them belongs to a single blossom
+                        debug_assert!(
+                            current_conflict_index != 1,
+                            "the first conflict cannot be ignored, otherwise may cause hidden infinite loop"
+                        );
+                        continue; // this is no longer a conflict because both of them belongs to a single blossom
                     }
                     let mut primal_node_internal_1 = primal_node_internal_ptr_1.write();
                     let mut primal_node_internal_2 = primal_node_internal_ptr_2.write();
                     let grow_state_1 = primal_node_internal_1.origin.upgrade_force().read_recursive().grow_state;
                     let grow_state_2 = primal_node_internal_2.origin.upgrade_force().read_recursive().grow_state;
                     if !grow_state_1.is_against(&grow_state_2) {
-                        debug_assert!(current_conflict_index != 1, "the first conflict cannot be ignored, otherwise may cause hidden infinite loop");
-                        continue  // this is no longer a conflict
+                        debug_assert!(
+                            current_conflict_index != 1,
+                            "the first conflict cannot be ignored, otherwise may cause hidden infinite loop"
+                        );
+                        continue; // this is no longer a conflict
                     }
                     // this is the most probable case, so put it in the front
                     let (free_1, free_2) = (primal_node_internal_1.is_free(), primal_node_internal_2.is_free());
                     if free_1 && free_2 {
                         // simply match them temporarily
-                        primal_node_internal_1.temporary_match = Some((MatchTarget::Peer(primal_node_internal_ptr_2.downgrade()), touching_ptr_1.downgrade()));
-                        primal_node_internal_2.temporary_match = Some((MatchTarget::Peer(primal_node_internal_ptr_1.downgrade()), touching_ptr_2.downgrade()));
+                        primal_node_internal_1.temporary_match = Some((
+                            MatchTarget::Peer(primal_node_internal_ptr_2.downgrade()),
+                            touching_ptr_1.downgrade(),
+                        ));
+                        primal_node_internal_2.temporary_match = Some((
+                            MatchTarget::Peer(primal_node_internal_ptr_1.downgrade()),
+                            touching_ptr_2.downgrade(),
+                        ));
                         // update dual module interface
-                        interface_ptr.set_grow_state(&primal_node_internal_1.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
-                        interface_ptr.set_grow_state(&primal_node_internal_2.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
-                        continue
+                        interface_ptr.set_grow_state(
+                            &primal_node_internal_1.origin.upgrade_force(),
+                            DualNodeGrowState::Stay,
+                            dual_module,
+                        );
+                        interface_ptr.set_grow_state(
+                            &primal_node_internal_2.origin.upgrade_force(),
+                            DualNodeGrowState::Stay,
+                            dual_module,
+                        );
+                        continue;
                     }
                     // second probable case: single node touches a temporary matched pair and become an alternating tree
-                    if (free_1 && primal_node_internal_2.temporary_match.is_some()) || (free_2 && primal_node_internal_1.temporary_match.is_some()) {
-                        let (free_node_internal_ptr, free_touching_ptr, mut free_node_internal, matched_node_internal_ptr, matched_touching_ptr, mut matched_node_internal) = if free_1 {
-                            (primal_node_internal_ptr_1.clone(), touching_ptr_1.clone(), primal_node_internal_1, primal_node_internal_ptr_2.clone(), touching_ptr_2.clone(), primal_node_internal_2)
+                    if (free_1 && primal_node_internal_2.temporary_match.is_some())
+                        || (free_2 && primal_node_internal_1.temporary_match.is_some())
+                    {
+                        let (
+                            free_node_internal_ptr,
+                            free_touching_ptr,
+                            mut free_node_internal,
+                            matched_node_internal_ptr,
+                            matched_touching_ptr,
+                            mut matched_node_internal,
+                        ) = if free_1 {
+                            (
+                                primal_node_internal_ptr_1.clone(),
+                                touching_ptr_1.clone(),
+                                primal_node_internal_1,
+                                primal_node_internal_ptr_2.clone(),
+                                touching_ptr_2.clone(),
+                                primal_node_internal_2,
+                            )
                         } else {
-                            (primal_node_internal_ptr_2.clone(), touching_ptr_2.clone(), primal_node_internal_2, primal_node_internal_ptr_1.clone(), touching_ptr_1.clone(), primal_node_internal_1)
+                            (
+                                primal_node_internal_ptr_2.clone(),
+                                touching_ptr_2.clone(),
+                                primal_node_internal_2,
+                                primal_node_internal_ptr_1.clone(),
+                                touching_ptr_1.clone(),
+                                primal_node_internal_1,
+                            )
                         };
                         // creating an alternating tree: free node becomes the root, matched node becomes child
-                        let (match_target, matched_touching_grandson) = matched_node_internal.temporary_match.as_ref().unwrap().clone();
+                        let (match_target, matched_touching_grandson) =
+                            matched_node_internal.temporary_match.as_ref().unwrap().clone();
                         match &match_target {
                             MatchTarget::Peer(leaf_node_internal_weak) => {
                                 let leaf_node_internal_ptr = leaf_node_internal_weak.upgrade_force();
                                 let mut leaf_node_internal = leaf_node_internal_ptr.write();
                                 free_node_internal.tree_node = Some(AlternatingTreeNode {
                                     root: free_node_internal_ptr.downgrade(),
                                     parent: None,
@@ -281,176 +344,314 @@
                                     parent: Some((free_node_internal_ptr.downgrade(), matched_touching_ptr.downgrade())),
                                     children: vec![(leaf_node_internal_weak.clone(), matched_touching_grandson)],
                                     depth: 1,
                                 });
                                 matched_node_internal.temporary_match = None;
                                 leaf_node_internal.tree_node = Some(AlternatingTreeNode {
                                     root: free_node_internal_ptr.downgrade(),
-                                    parent: Some((matched_node_internal_ptr.downgrade(), leaf_node_internal.temporary_match.as_ref().unwrap().1.clone())),
+                                    parent: Some((
+                                        matched_node_internal_ptr.downgrade(),
+                                        leaf_node_internal.temporary_match.as_ref().unwrap().1.clone(),
+                                    )),
                                     children: vec![],
                                     depth: 2,
                                 });
                                 leaf_node_internal.temporary_match = None;
                                 // update dual module interface
-                                interface_ptr.set_grow_state(&free_node_internal.origin.upgrade_force(), DualNodeGrowState::Grow, dual_module);
-                                interface_ptr.set_grow_state(&matched_node_internal.origin.upgrade_force(), DualNodeGrowState::Shrink, dual_module);
-                                interface_ptr.set_grow_state(&leaf_node_internal.origin.upgrade_force(), DualNodeGrowState::Grow, dual_module);
-                                continue
-                            },
+                                interface_ptr.set_grow_state(
+                                    &free_node_internal.origin.upgrade_force(),
+                                    DualNodeGrowState::Grow,
+                                    dual_module,
+                                );
+                                interface_ptr.set_grow_state(
+                                    &matched_node_internal.origin.upgrade_force(),
+                                    DualNodeGrowState::Shrink,
+                                    dual_module,
+                                );
+                                interface_ptr.set_grow_state(
+                                    &leaf_node_internal.origin.upgrade_force(),
+                                    DualNodeGrowState::Grow,
+                                    dual_module,
+                                );
+                                continue;
+                            }
                             MatchTarget::VirtualVertex(_) => {
                                 // virtual boundary doesn't have to be matched, so in this case simply match these two nodes together
-                                free_node_internal.temporary_match = Some((MatchTarget::Peer(matched_node_internal_ptr.downgrade()), free_touching_ptr.downgrade()));
-                                matched_node_internal.temporary_match = Some((MatchTarget::Peer(free_node_internal_ptr.downgrade()), matched_touching_ptr.downgrade()));
+                                free_node_internal.temporary_match = Some((
+                                    MatchTarget::Peer(matched_node_internal_ptr.downgrade()),
+                                    free_touching_ptr.downgrade(),
+                                ));
+                                matched_node_internal.temporary_match = Some((
+                                    MatchTarget::Peer(free_node_internal_ptr.downgrade()),
+                                    matched_touching_ptr.downgrade(),
+                                ));
                                 // update dual module interface
-                                interface_ptr.set_grow_state(&free_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
-                                interface_ptr.set_grow_state(&matched_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
-                                continue
+                                interface_ptr.set_grow_state(
+                                    &free_node_internal.origin.upgrade_force(),
+                                    DualNodeGrowState::Stay,
+                                    dual_module,
+                                );
+                                interface_ptr.set_grow_state(
+                                    &matched_node_internal.origin.upgrade_force(),
+                                    DualNodeGrowState::Stay,
+                                    dual_module,
+                                );
+                                continue;
                             }
                         }
                     }
                     // third probable case: tree touches single vertex
-                    if (free_1 && primal_node_internal_2.tree_node.is_some()) || (primal_node_internal_1.tree_node.is_some() && free_2) {
-                        let (tree_node_internal_ptr, tree_touching_ptr, tree_node_internal, free_node_internal_ptr, free_touching_ptr, mut free_node_internal) = 
-                            if primal_node_internal_1.tree_node.is_some() {
-                                (primal_node_internal_ptr_1.clone(), touching_ptr_1.clone(), primal_node_internal_1, primal_node_internal_ptr_2.clone(), touching_ptr_2.clone(), primal_node_internal_2)
-                            } else {
-                                (primal_node_internal_ptr_2.clone(), touching_ptr_2.clone(), primal_node_internal_2, primal_node_internal_ptr_1.clone(), touching_ptr_1.clone(), primal_node_internal_1)
-                            };
-                        free_node_internal.temporary_match = Some((MatchTarget::Peer(tree_node_internal_ptr.downgrade()), free_touching_ptr.downgrade()));
-                        interface_ptr.set_grow_state(&free_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
-                        drop(tree_node_internal);  // unlock
-                        Self::augment_tree_given_matched(tree_node_internal_ptr, free_node_internal_ptr, tree_touching_ptr.downgrade(), interface_ptr, dual_module);
-                        continue
+                    if (free_1 && primal_node_internal_2.tree_node.is_some())
+                        || (primal_node_internal_1.tree_node.is_some() && free_2)
+                    {
+                        let (
+                            tree_node_internal_ptr,
+                            tree_touching_ptr,
+                            tree_node_internal,
+                            free_node_internal_ptr,
+                            free_touching_ptr,
+                            mut free_node_internal,
+                        ) = if primal_node_internal_1.tree_node.is_some() {
+                            (
+                                primal_node_internal_ptr_1.clone(),
+                                touching_ptr_1.clone(),
+                                primal_node_internal_1,
+                                primal_node_internal_ptr_2.clone(),
+                                touching_ptr_2.clone(),
+                                primal_node_internal_2,
+                            )
+                        } else {
+                            (
+                                primal_node_internal_ptr_2.clone(),
+                                touching_ptr_2.clone(),
+                                primal_node_internal_2,
+                                primal_node_internal_ptr_1.clone(),
+                                touching_ptr_1.clone(),
+                                primal_node_internal_1,
+                            )
+                        };
+                        free_node_internal.temporary_match = Some((
+                            MatchTarget::Peer(tree_node_internal_ptr.downgrade()),
+                            free_touching_ptr.downgrade(),
+                        ));
+                        interface_ptr.set_grow_state(
+                            &free_node_internal.origin.upgrade_force(),
+                            DualNodeGrowState::Stay,
+                            dual_module,
+                        );
+                        drop(tree_node_internal); // unlock
+                        Self::augment_tree_given_matched(
+                            tree_node_internal_ptr,
+                            free_node_internal_ptr,
+                            tree_touching_ptr.downgrade(),
+                            interface_ptr,
+                            dual_module,
+                        );
+                        continue;
                     }
                     // fourth probable case: tree touches matched pair
                     if (primal_node_internal_1.tree_node.is_some() && primal_node_internal_2.temporary_match.is_some())
-                            || (primal_node_internal_1.temporary_match.is_some() && primal_node_internal_2.tree_node.is_some()) {
-                        let (tree_node_internal_ptr, tree_touching_ptr, mut tree_node_internal, matched_node_internal_ptr, matched_touching_ptr, mut matched_node_internal) = 
-                            if primal_node_internal_1.tree_node.is_some() {
-                                (primal_node_internal_ptr_1.clone(), touching_ptr_1.clone(), primal_node_internal_1, primal_node_internal_ptr_2.clone(), touching_ptr_2.clone(), primal_node_internal_2)
-                            } else {
-                                (primal_node_internal_ptr_2.clone(), touching_ptr_2.clone(), primal_node_internal_2, primal_node_internal_ptr_1.clone(), touching_ptr_1.clone(), primal_node_internal_1)
-                            };
+                        || (primal_node_internal_1.temporary_match.is_some() && primal_node_internal_2.tree_node.is_some())
+                    {
+                        let (
+                            tree_node_internal_ptr,
+                            tree_touching_ptr,
+                            mut tree_node_internal,
+                            matched_node_internal_ptr,
+                            matched_touching_ptr,
+                            mut matched_node_internal,
+                        ) = if primal_node_internal_1.tree_node.is_some() {
+                            (
+                                primal_node_internal_ptr_1.clone(),
+                                touching_ptr_1.clone(),
+                                primal_node_internal_1,
+                                primal_node_internal_ptr_2.clone(),
+                                touching_ptr_2.clone(),
+                                primal_node_internal_2,
+                            )
+                        } else {
+                            (
+                                primal_node_internal_ptr_2.clone(),
+                                touching_ptr_2.clone(),
+                                primal_node_internal_2,
+                                primal_node_internal_ptr_1.clone(),
+                                touching_ptr_1.clone(),
+                                primal_node_internal_1,
+                            )
+                        };
                         let match_target = matched_node_internal.temporary_match.as_ref().unwrap().0.clone();
                         match &match_target {
                             MatchTarget::Peer(leaf_node_internal_weak) => {
                                 let leaf_node_internal_ptr = leaf_node_internal_weak.upgrade_force();
                                 let tree_node = tree_node_internal.tree_node.as_mut().unwrap();
                                 debug_assert!(tree_node.depth % 2 == 0, "conflicting one must be + node");
                                 // simply add this matched pair to the children
-                                tree_node.children.push((matched_node_internal_ptr.downgrade(), tree_touching_ptr.downgrade()));
+                                tree_node
+                                    .children
+                                    .push((matched_node_internal_ptr.downgrade(), tree_touching_ptr.downgrade()));
                                 // link children to parent
                                 matched_node_internal.tree_node = Some(AlternatingTreeNode {
                                     root: tree_node.root.clone(),
                                     parent: Some((tree_node_internal_ptr.downgrade(), matched_touching_ptr.downgrade())),
-                                    children: vec![(leaf_node_internal_weak.clone(), matched_node_internal.temporary_match.as_ref().unwrap().1.clone())],
+                                    children: vec![(
+                                        leaf_node_internal_weak.clone(),
+                                        matched_node_internal.temporary_match.as_ref().unwrap().1.clone(),
+                                    )],
                                     depth: tree_node.depth + 1,
                                 });
                                 matched_node_internal.temporary_match = None;
                                 let mut leaf_node_internal = leaf_node_internal_ptr.write();
                                 leaf_node_internal.tree_node = Some(AlternatingTreeNode {
                                     root: tree_node.root.clone(),
-                                    parent: Some((matched_node_internal_ptr.downgrade(), leaf_node_internal.temporary_match.as_ref().unwrap().1.clone())),
+                                    parent: Some((
+                                        matched_node_internal_ptr.downgrade(),
+                                        leaf_node_internal.temporary_match.as_ref().unwrap().1.clone(),
+                                    )),
                                     children: vec![],
                                     depth: tree_node.depth + 2,
                                 });
                                 leaf_node_internal.temporary_match = None;
                                 // update dual module interface
-                                interface_ptr.set_grow_state(&matched_node_internal.origin.upgrade_force(), DualNodeGrowState::Shrink, dual_module);
-                                interface_ptr.set_grow_state(&leaf_node_internal.origin.upgrade_force(), DualNodeGrowState::Grow, dual_module);
-                                continue
-                            },
+                                interface_ptr.set_grow_state(
+                                    &matched_node_internal.origin.upgrade_force(),
+                                    DualNodeGrowState::Shrink,
+                                    dual_module,
+                                );
+                                interface_ptr.set_grow_state(
+                                    &leaf_node_internal.origin.upgrade_force(),
+                                    DualNodeGrowState::Grow,
+                                    dual_module,
+                                );
+                                continue;
+                            }
                             MatchTarget::VirtualVertex(_) => {
                                 // virtual boundary doesn't have to be matched, so in this case remove it and augment the tree
-                                matched_node_internal.temporary_match = Some((MatchTarget::Peer(tree_node_internal_ptr.downgrade()), matched_touching_ptr.downgrade()));
-                                drop(matched_node_internal);  // unlock
-                                drop(tree_node_internal);  // unlock
-                                Self::augment_tree_given_matched(tree_node_internal_ptr, matched_node_internal_ptr, tree_touching_ptr.downgrade(), interface_ptr, dual_module);
-                                continue
+                                matched_node_internal.temporary_match = Some((
+                                    MatchTarget::Peer(tree_node_internal_ptr.downgrade()),
+                                    matched_touching_ptr.downgrade(),
+                                ));
+                                drop(matched_node_internal); // unlock
+                                drop(tree_node_internal); // unlock
+                                Self::augment_tree_given_matched(
+                                    tree_node_internal_ptr,
+                                    matched_node_internal_ptr,
+                                    tree_touching_ptr.downgrade(),
+                                    interface_ptr,
+                                    dual_module,
+                                );
+                                continue;
                             }
                         }
                     }
                     // much less probable case: two trees touch and both are augmented
                     if primal_node_internal_1.tree_node.is_some() && primal_node_internal_2.tree_node.is_some() {
                         let root_1 = primal_node_internal_1.tree_node.as_ref().unwrap().root.clone();
                         let root_2 = primal_node_internal_2.tree_node.as_ref().unwrap().root.clone();
                         // form a blossom inside an alternating tree
                         if root_1 == root_2 {
                             // drop writer lock to allow reader locks
                             drop(primal_node_internal_1);
                             drop(primal_node_internal_2);
                             // find LCA of two nodes, two paths are from child to parent
-                            let (lca_ptr, path_1, path_2) = self.find_lowest_common_ancestor(primal_node_internal_ptr_1.clone(), primal_node_internal_ptr_2.clone());
+                            let (lca_ptr, path_1, path_2) = self.find_lowest_common_ancestor(
+                                primal_node_internal_ptr_1.clone(),
+                                primal_node_internal_ptr_2.clone(),
+                            );
                             let nodes_circle = {
-                                let mut nodes_circle: Vec<DualNodePtr> = path_1.iter().map(|ptr| ptr.read_recursive().origin.upgrade_force()).collect();
+                                let mut nodes_circle: Vec<DualNodePtr> =
+                                    path_1.iter().map(|ptr| ptr.read_recursive().origin.upgrade_force()).collect();
                                 nodes_circle.push(lca_ptr.read_recursive().origin.upgrade_force());
-                                for i in (0..path_2.len()).rev() { nodes_circle.push(path_2[i].read_recursive().origin.upgrade_force()); }
+                                for i in (0..path_2.len()).rev() {
+                                    nodes_circle.push(path_2[i].read_recursive().origin.upgrade_force());
+                                }
                                 nodes_circle
                             };
                             // build `touching_children`
                             let touching_children = {
                                 let mut touching_children = Vec::<(DualNodeWeak, DualNodeWeak)>::new();
                                 if !path_1.is_empty() {
                                     for (idx, ptr) in path_1.iter().enumerate() {
                                         let node = ptr.read_recursive();
                                         let tree_node = node.tree_node.as_ref().unwrap();
                                         let left_touching_ptr = if idx == 0 {
                                             touching_ptr_1.downgrade()
                                         } else {
-                                            let last_ptr = path_1[idx-1].downgrade();
-                                            let idx = tree_node.children.iter().position(|(ptr, _)| ptr == &last_ptr).expect("should find child");
+                                            let last_ptr = path_1[idx - 1].downgrade();
+                                            let idx = tree_node
+                                                .children
+                                                .iter()
+                                                .position(|(ptr, _)| ptr == &last_ptr)
+                                                .expect("should find child");
                                             tree_node.children[idx].1.clone()
                                         };
                                         let right_touching_ptr = tree_node.parent.as_ref().unwrap().1.clone();
                                         touching_children.push((left_touching_ptr, right_touching_ptr));
                                     }
                                 }
-                                { // the lca
+                                {
+                                    // the lca
                                     let node = lca_ptr.read_recursive();
                                     let tree_node = node.tree_node.as_ref().unwrap();
                                     let left_touching_ptr = if path_1.is_empty() {
                                         touching_ptr_1.downgrade()
                                     } else {
                                         let left_ptr = path_1[path_1.len() - 1].downgrade();
-                                        let left_idx = tree_node.children.iter().position(|(ptr, _)| ptr == &left_ptr).expect("should find child");
+                                        let left_idx = tree_node
+                                            .children
+                                            .iter()
+                                            .position(|(ptr, _)| ptr == &left_ptr)
+                                            .expect("should find child");
                                         tree_node.children[left_idx].1.clone()
                                     };
                                     let right_touching_ptr = if path_2.is_empty() {
                                         touching_ptr_2.downgrade()
                                     } else {
                                         let right_ptr = path_2[path_2.len() - 1].downgrade();
-                                        let right_idx = tree_node.children.iter().position(|(ptr, _)| ptr == &right_ptr).expect("should find child");
+                                        let right_idx = tree_node
+                                            .children
+                                            .iter()
+                                            .position(|(ptr, _)| ptr == &right_ptr)
+                                            .expect("should find child");
                                         tree_node.children[right_idx].1.clone()
                                     };
                                     touching_children.push((left_touching_ptr, right_touching_ptr));
                                 }
                                 if !path_2.is_empty() {
                                     for (idx, ptr) in path_2.iter().enumerate().rev() {
                                         let node = ptr.read_recursive();
                                         let tree_node = node.tree_node.as_ref().unwrap();
                                         let left_touching_ptr = tree_node.parent.as_ref().unwrap().1.clone();
                                         let right_touching_ptr = if idx == 0 {
                                             touching_ptr_2.downgrade()
                                         } else {
-                                            let last_ptr = path_2[idx-1].downgrade();
-                                            let idx = tree_node.children.iter().position(|(ptr, _)| ptr == &last_ptr).expect("should find child");
+                                            let last_ptr = path_2[idx - 1].downgrade();
+                                            let idx = tree_node
+                                                .children
+                                                .iter()
+                                                .position(|(ptr, _)| ptr == &last_ptr)
+                                                .expect("should find child");
                                             tree_node.children[idx].1.clone()
                                         };
                                         touching_children.push((left_touching_ptr, right_touching_ptr));
                                     }
                                 }
                                 touching_children
                             };
-                            let blossom_node_ptr = interface_ptr.create_blossom(nodes_circle, touching_children, dual_module);
-                            let primal_node_internal_blossom_ptr = {  // create the corresponding primal node
+                            let blossom_node_ptr =
+                                interface_ptr.create_blossom(nodes_circle, touching_children, dual_module);
+                            let primal_node_internal_blossom_ptr = {
+                                // create the corresponding primal node
                                 let belonging = self.downgrade();
                                 let mut module = self.write();
                                 let local_node_index = module.nodes_length;
                                 let node_index = module.nodes_count();
-                                let primal_node_internal_blossom_ptr = if !module.is_fusion && local_node_index < module.nodes.len() && module.nodes[local_node_index].is_some() {
+                                let primal_node_internal_blossom_ptr = if !module.is_fusion
+                                    && local_node_index < module.nodes.len()
+                                    && module.nodes[local_node_index].is_some()
+                                {
                                     let node_ptr = module.nodes[local_node_index].take().unwrap();
                                     let mut node = node_ptr.write();
                                     node.origin = blossom_node_ptr.downgrade();
                                     node.index = node_index;
                                     node.tree_node = None;
                                     node.temporary_match = None;
                                     node.belonging = belonging;
@@ -466,15 +667,15 @@
                                     })
                                 };
                                 module.nodes_length += 1;
                                 if module.nodes.len() < module.nodes_length {
                                     module.nodes.push(None);
                                 }
                                 let cloned_primal_node_internal_blossom_ptr = primal_node_internal_blossom_ptr.clone();
-                                module.nodes[local_node_index] = Some(primal_node_internal_blossom_ptr);  // feature `dangerous_pointer`: must push the owner
+                                module.nodes[local_node_index] = Some(primal_node_internal_blossom_ptr); // feature `dangerous_pointer`: must push the owner
                                 cloned_primal_node_internal_blossom_ptr
                             };
                             // handle other part of the tree structure
                             let mut children = vec![];
                             for path in [&path_1, &path_2] {
                                 if !path.is_empty() {
                                     let mut last_ptr = path[0].downgrade();
@@ -485,321 +686,513 @@
                                             for (child_ptr, child_touching_ptr) in tree_node.children.iter() {
                                                 children.push((child_ptr.clone(), child_touching_ptr.clone()));
                                             }
                                         } else {
                                             if height % 2 == 0 {
                                                 let tree_node = node.tree_node.as_ref().unwrap();
                                                 for (child_ptr, child_touching_ptr) in tree_node.children.iter() {
-                                                    if child_ptr != &last_ptr {  // not in the blossom circle
+                                                    if child_ptr != &last_ptr {
+                                                        // not in the blossom circle
                                                         children.push((child_ptr.clone(), child_touching_ptr.clone()));
                                                     }
                                                 }
                                             }
                                         }
-                                        node.tree_node = None;  // this path is going to be part of the blossom, no longer in the tree
+                                        node.tree_node = None; // this path is going to be part of the blossom, no longer in the tree
                                         last_ptr = ptr.downgrade();
                                     }
                                 }
                             }
                             let mut lca = lca_ptr.write();
                             let lca_tree_node = lca.tree_node.as_ref().unwrap();
-                            {  // add children of lca_ptr
+                            {
+                                // add children of lca_ptr
                                 for (child_ptr, child_touching_ptr) in lca_tree_node.children.iter() {
-                                    if !path_1.is_empty() && &path_1[path_1.len() - 1].downgrade() == child_ptr { continue }
-                                    if !path_2.is_empty() && &path_2[path_2.len() - 1].downgrade() == child_ptr { continue }
+                                    if !path_1.is_empty() && &path_1[path_1.len() - 1].downgrade() == child_ptr {
+                                        continue;
+                                    }
+                                    if !path_2.is_empty() && &path_2[path_2.len() - 1].downgrade() == child_ptr {
+                                        continue;
+                                    }
                                     children.push((child_ptr.clone(), child_touching_ptr.clone()));
                                 }
                             }
                             if lca_tree_node.parent.is_some() || !children.is_empty() {
                                 let mut primal_node_internal_blossom = primal_node_internal_blossom_ptr.write();
-                                let new_tree_root = if lca_tree_node.depth == 0 { primal_node_internal_blossom_ptr.clone() } else { lca_tree_node.root.upgrade_force() };
+                                let new_tree_root = if lca_tree_node.depth == 0 {
+                                    primal_node_internal_blossom_ptr.clone()
+                                } else {
+                                    lca_tree_node.root.upgrade_force()
+                                };
                                 let tree_node = AlternatingTreeNode {
                                     root: new_tree_root.downgrade(),
                                     parent: lca_tree_node.parent.clone(),
                                     children,
                                     depth: lca_tree_node.depth,
                                 };
                                 if lca_tree_node.parent.is_some() {
                                     let (parent_weak, _) = lca_tree_node.parent.as_ref().unwrap();
                                     let parent_ptr = parent_weak.upgrade_force();
                                     lock_write!(parent, parent_ptr);
                                     let parent_tree_node = parent.tree_node.as_mut().unwrap();
-                                    debug_assert!(parent_tree_node.children.len() == 1, "lca's parent should be a - node with only one child");
-                                    let touching_ptr = parent_tree_node.children[0].1.clone();  // the touching grandson is not changed when forming blossom
+                                    debug_assert!(
+                                        parent_tree_node.children.len() == 1,
+                                        "lca's parent should be a - node with only one child"
+                                    );
+                                    let touching_ptr = parent_tree_node.children[0].1.clone(); // the touching grandson is not changed when forming blossom
                                     parent_tree_node.children.clear();
-                                    parent_tree_node.children.push((primal_node_internal_blossom_ptr.downgrade(), touching_ptr));
+                                    parent_tree_node
+                                        .children
+                                        .push((primal_node_internal_blossom_ptr.downgrade(), touching_ptr));
                                 }
                                 if !tree_node.children.is_empty() {
                                     // connect this blossom to the new alternating tree
                                     for (child_weak, _) in tree_node.children.iter() {
                                         let child_ptr = child_weak.upgrade_force();
                                         lock_write!(child, child_ptr);
                                         let child_tree_node = child.tree_node.as_mut().unwrap();
                                         debug_assert!(child_tree_node.parent.is_some(), "child should have a parent");
-                                        let touching_ptr = child_tree_node.parent.as_ref().unwrap().1.clone();  // the touching grandson is not changed when forming blossom
-                                        child_tree_node.parent = Some((primal_node_internal_blossom_ptr.downgrade(), touching_ptr));
+                                        let touching_ptr = child_tree_node.parent.as_ref().unwrap().1.clone(); // the touching grandson is not changed when forming blossom
+                                        child_tree_node.parent =
+                                            Some((primal_node_internal_blossom_ptr.downgrade(), touching_ptr));
                                     }
                                     primal_node_internal_blossom.tree_node = Some(tree_node);
                                     primal_node_internal_blossom.change_sub_tree_root(lca_tree_node.depth, new_tree_root);
                                 } else {
                                     primal_node_internal_blossom.tree_node = Some(tree_node);
                                 }
                             }
                             lca.tree_node = None;
-                            continue
+                            continue;
                         } else {
-                            drop(primal_node_internal_1);  // unlock
-                            drop(primal_node_internal_2);  // unlock
-                            Self::augment_tree_given_matched(primal_node_internal_ptr_1.clone(), primal_node_internal_ptr_2.clone(), touching_ptr_1.downgrade()
-                                , interface_ptr, dual_module);
-                            Self::augment_tree_given_matched(primal_node_internal_ptr_2.clone(), primal_node_internal_ptr_1.clone(), touching_ptr_2.downgrade()
-                                , interface_ptr, dual_module);
-                            continue
+                            drop(primal_node_internal_1); // unlock
+                            drop(primal_node_internal_2); // unlock
+                            Self::augment_tree_given_matched(
+                                primal_node_internal_ptr_1.clone(),
+                                primal_node_internal_ptr_2.clone(),
+                                touching_ptr_1.downgrade(),
+                                interface_ptr,
+                                dual_module,
+                            );
+                            Self::augment_tree_given_matched(
+                                primal_node_internal_ptr_2.clone(),
+                                primal_node_internal_ptr_1.clone(),
+                                touching_ptr_2.downgrade(),
+                                interface_ptr,
+                                dual_module,
+                            );
+                            continue;
                         }
                     }
                     unreachable!()
-                },
+                }
                 MaxUpdateLength::TouchingVirtual((node_ptr, touching_ptr), (virtual_vertex_index, is_mirror)) => {
-                    if self.get_primal_node_internal_ptr_option(&node_ptr).is_none() { continue }  // ignore out-of-date event
+                    if self.get_primal_node_internal_ptr_option(&node_ptr).is_none() {
+                        continue;
+                    } // ignore out-of-date event
                     let primal_node_internal_ptr = self.get_outer_node(self.get_primal_node_internal_ptr(&node_ptr));
                     let mut primal_node_internal = primal_node_internal_ptr.write();
                     let grow_state = primal_node_internal.origin.upgrade_force().read_recursive().grow_state;
                     if grow_state != DualNodeGrowState::Grow {
-                        debug_assert!(current_conflict_index != 1, "the first conflict cannot be ignored, otherwise may cause hidden infinite loop");
-                        continue  // this is no longer a conflict
+                        debug_assert!(
+                            current_conflict_index != 1,
+                            "the first conflict cannot be ignored, otherwise may cause hidden infinite loop"
+                        );
+                        continue; // this is no longer a conflict
                     }
                     // this is the most probable case, so put it in the front
                     if primal_node_internal.is_free() {
-                        primal_node_internal.temporary_match = Some((MatchTarget::VirtualVertex(virtual_vertex_index), touching_ptr.downgrade()));
+                        primal_node_internal.temporary_match =
+                            Some((MatchTarget::VirtualVertex(virtual_vertex_index), touching_ptr.downgrade()));
                         if is_mirror {
                             lock_write!(module, self);
                             module.possible_break.push(primal_node_internal.index);
                         }
-                        interface_ptr.set_grow_state(&primal_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
-                        continue
+                        interface_ptr.set_grow_state(
+                            &primal_node_internal.origin.upgrade_force(),
+                            DualNodeGrowState::Stay,
+                            dual_module,
+                        );
+                        continue;
                     }
                     // tree touching virtual boundary will just augment the whole tree
                     if primal_node_internal.tree_node.is_some() {
                         if is_mirror {
                             lock_write!(module, self);
                             module.possible_break.push(primal_node_internal.index);
                         }
                         drop(primal_node_internal);
-                        self.augment_tree_given_virtual_vertex(primal_node_internal_ptr, virtual_vertex_index, touching_ptr.downgrade(), interface_ptr, dual_module);
-                        continue
+                        self.augment_tree_given_virtual_vertex(
+                            primal_node_internal_ptr,
+                            virtual_vertex_index,
+                            touching_ptr.downgrade(),
+                            interface_ptr,
+                            dual_module,
+                        );
+                        continue;
                     }
                     unreachable!()
-                },
+                }
                 MaxUpdateLength::BlossomNeedExpand(node_ptr) => {
-                    if self.get_primal_node_internal_ptr_option(&node_ptr).is_none() { continue }  // ignore out-of-date event
-                    // blossom breaking is assumed to be very rare given our multiple-tree approach, so don't need to optimize for it
-                    // first, isolate this blossom from its alternating tree
+                    if self.get_primal_node_internal_ptr_option(&node_ptr).is_none() {
+                        continue;
+                    } // ignore out-of-date event
+                      // blossom breaking is assumed to be very rare given our multiple-tree approach, so don't need to optimize for it
+                      // first, isolate this blossom from its alternating tree
                     let primal_node_internal_ptr = self.get_primal_node_internal_ptr(&node_ptr);
                     let outer_primal_node_internal_ptr = self.get_outer_node(primal_node_internal_ptr.clone());
                     if outer_primal_node_internal_ptr != primal_node_internal_ptr {
                         // this blossom is now wrapped into another blossom, so we don't need to expand it anymore
-                        debug_assert!(current_conflict_index != 1, "the first conflict cannot be ignored, otherwise may cause hidden infinite loop");
-                        continue
+                        debug_assert!(
+                            current_conflict_index != 1,
+                            "the first conflict cannot be ignored, otherwise may cause hidden infinite loop"
+                        );
+                        continue;
                     }
                     let primal_node_internal = primal_node_internal_ptr.read_recursive();
                     let grow_state = primal_node_internal.origin.upgrade_force().read_recursive().grow_state;
                     if grow_state != DualNodeGrowState::Shrink {
-                        debug_assert!(current_conflict_index != 1, "the first conflict cannot be ignored, otherwise may cause hidden infinite loop");
-                        continue  // this is no longer a conflict
+                        debug_assert!(
+                            current_conflict_index != 1,
+                            "the first conflict cannot be ignored, otherwise may cause hidden infinite loop"
+                        );
+                        continue; // this is no longer a conflict
                     }
                     // copy the nodes circle
                     let (nodes_circle, touching_children) = {
                         let blossom = node_ptr.read_recursive();
                         match &blossom.class {
-                            DualNodeClass::Blossom{ nodes_circle, touching_children } => (nodes_circle.clone(), touching_children.clone()),
-                            _ => unreachable!("the expanding node is not a blossom")
+                            DualNodeClass::Blossom {
+                                nodes_circle,
+                                touching_children,
+                            } => (nodes_circle.clone(), touching_children.clone()),
+                            _ => unreachable!("the expanding node is not a blossom"),
                         }
                     };
-                    debug_assert!(primal_node_internal.tree_node.is_some(), "expanding blossom must belong to an alternating tree");
+                    debug_assert!(
+                        primal_node_internal.tree_node.is_some(),
+                        "expanding blossom must belong to an alternating tree"
+                    );
                     let tree_node = primal_node_internal.tree_node.as_ref().unwrap();
-                    debug_assert!(tree_node.depth % 2 == 1, "expanding blossom must a '-' node in an alternating tree");
-                    let (parent_ptr, parent_touching_ptr, parent_touching_child_ptr) = {  // remove it from it's parent's tree
+                    debug_assert!(
+                        tree_node.depth % 2 == 1,
+                        "expanding blossom must a '-' node in an alternating tree"
+                    );
+                    let (parent_ptr, parent_touching_ptr, parent_touching_child_ptr) = {
+                        // remove it from it's parent's tree
                         let (parent_weak, parent_touching_child_ptr) = &tree_node.parent.as_ref().unwrap();
                         let parent_ptr = parent_weak.upgrade_force();
                         lock_write!(parent, parent_ptr);
                         let parent_tree_node = parent.tree_node.as_mut().unwrap();
-                        let idx = parent_tree_node.children.iter().position(|ptr| ptr.0 == primal_node_internal_ptr.downgrade()).expect("should find");
+                        let idx = parent_tree_node
+                            .children
+                            .iter()
+                            .position(|ptr| ptr.0 == primal_node_internal_ptr.downgrade())
+                            .expect("should find");
                         let parent_touching_ptr = parent_tree_node.children[idx].1.clone();
                         parent_tree_node.children.remove(idx);
-                        parent_tree_node.children.retain(|ptr| ptr.0 != primal_node_internal_ptr.downgrade());
-                        (parent_ptr.clone(), parent_touching_ptr, parent_touching_child_ptr.upgrade_force().get_secondary_ancestor_blossom().downgrade())
+                        parent_tree_node
+                            .children
+                            .retain(|ptr| ptr.0 != primal_node_internal_ptr.downgrade());
+                        (
+                            parent_ptr.clone(),
+                            parent_touching_ptr,
+                            parent_touching_child_ptr
+                                .upgrade_force()
+                                .get_secondary_ancestor_blossom()
+                                .downgrade(),
+                        )
                     };
-                    let (child_ptr, child_touching_ptr, child_touching_child_ptr) = {  // make children independent trees
+                    let (child_ptr, child_touching_ptr, child_touching_child_ptr) = {
+                        // make children independent trees
                         debug_assert!(tree_node.children.len() == 1, "a - node must have exactly ONE child");
                         let child_weak = &tree_node.children[0].0;
-                        let child_touching_child_ptr = tree_node.children[0].1.upgrade_force().get_secondary_ancestor_blossom().downgrade();
+                        let child_touching_child_ptr = tree_node.children[0]
+                            .1
+                            .upgrade_force()
+                            .get_secondary_ancestor_blossom()
+                            .downgrade();
                         let child_ptr = child_weak.upgrade_force();
                         let child = child_ptr.read_recursive();
                         let child_tree_node = child.tree_node.as_ref().unwrap();
                         // find which blossom-child is touching this child
-                        (child_ptr.clone(), child_tree_node.parent.as_ref().unwrap().1.clone(), child_touching_child_ptr)
+                        (
+                            child_ptr.clone(),
+                            child_tree_node.parent.as_ref().unwrap().1.clone(),
+                            child_touching_child_ptr,
+                        )
                     };
                     interface_ptr.expand_blossom(node_ptr, dual_module);
                     // now we need to re-connect all the expanded nodes, by analyzing the relationship of nodes_circle, parent_touching_ptr and child_touching_ptr
-                    let parent_touching_index = nodes_circle.iter().position(|ptr| ptr == &parent_touching_child_ptr).expect("touching node should be in the blossom circle");
-                    let child_touching_index = nodes_circle.iter().position(|ptr| ptr == &child_touching_child_ptr).expect("touching node should be in the blossom circle");
+                    let parent_touching_index = nodes_circle
+                        .iter()
+                        .position(|ptr| ptr == &parent_touching_child_ptr)
+                        .expect("touching node should be in the blossom circle");
+                    let child_touching_index = nodes_circle
+                        .iter()
+                        .position(|ptr| ptr == &child_touching_child_ptr)
+                        .expect("touching node should be in the blossom circle");
                     let mut is_tree_sequence_ascending = true;
-                    let (match_sequence, tree_sequence) = {  // tree sequence is from parent to child
+                    let (match_sequence, tree_sequence) = {
+                        // tree sequence is from parent to child
                         let mut match_sequence = Vec::new();
                         let mut tree_sequence = Vec::new();
                         match parent_touching_index.cmp(&child_touching_index) {
                             Ordering::Equal => {
                                 tree_sequence.push(parent_touching_index);
-                                for i in parent_touching_index+1 .. nodes_circle.len() { match_sequence.push(i); }
-                                for i in 0 .. parent_touching_index { match_sequence.push(i); }
-                            },
+                                for i in parent_touching_index + 1..nodes_circle.len() {
+                                    match_sequence.push(i);
+                                }
+                                for i in 0..parent_touching_index {
+                                    match_sequence.push(i);
+                                }
+                            }
                             Ordering::Greater => {
-                                if (parent_touching_index - child_touching_index) % 2 == 0 {  // [... c <----- p ...]
-                                    for i in (child_touching_index .. parent_touching_index+1).rev() { tree_sequence.push(i); }
+                                if (parent_touching_index - child_touching_index) % 2 == 0 {
+                                    // [... c <----- p ...]
+                                    for i in (child_touching_index..parent_touching_index + 1).rev() {
+                                        tree_sequence.push(i);
+                                    }
                                     is_tree_sequence_ascending = false;
-                                    for i in parent_touching_index+1 .. nodes_circle.len() { match_sequence.push(i); }
-                                    for i in 0 .. child_touching_index { match_sequence.push(i); }
-                                } else {  // [--> c ...... p ---]
-                                    for i in parent_touching_index .. nodes_circle.len() { tree_sequence.push(i); }
-                                    for i in 0 .. child_touching_index+1 { tree_sequence.push(i); }
-                                    for i in child_touching_index+1 .. parent_touching_index { match_sequence.push(i); }
+                                    for i in parent_touching_index + 1..nodes_circle.len() {
+                                        match_sequence.push(i);
+                                    }
+                                    for i in 0..child_touching_index {
+                                        match_sequence.push(i);
+                                    }
+                                } else {
+                                    // [--> c ...... p ---]
+                                    for i in parent_touching_index..nodes_circle.len() {
+                                        tree_sequence.push(i);
+                                    }
+                                    for i in 0..child_touching_index + 1 {
+                                        tree_sequence.push(i);
+                                    }
+                                    for i in child_touching_index + 1..parent_touching_index {
+                                        match_sequence.push(i);
+                                    }
                                 }
-                            },
+                            }
                             Ordering::Less => {
-                                if (child_touching_index - parent_touching_index) % 2 == 0 {  // [... p -----> c ...]
-                                    for i in parent_touching_index .. child_touching_index+1 { tree_sequence.push(i); }
-                                    for i in child_touching_index+1 .. nodes_circle.len() { match_sequence.push(i); }
-                                    for i in 0 .. parent_touching_index { match_sequence.push(i); }
-                                } else {  // [--- p ...... c <--]
-                                    for i in (0 .. parent_touching_index+1).rev() { tree_sequence.push(i); }
-                                    for i in (child_touching_index .. nodes_circle.len()).rev() { tree_sequence.push(i); }
+                                if (child_touching_index - parent_touching_index) % 2 == 0 {
+                                    // [... p -----> c ...]
+                                    for i in parent_touching_index..child_touching_index + 1 {
+                                        tree_sequence.push(i);
+                                    }
+                                    for i in child_touching_index + 1..nodes_circle.len() {
+                                        match_sequence.push(i);
+                                    }
+                                    for i in 0..parent_touching_index {
+                                        match_sequence.push(i);
+                                    }
+                                } else {
+                                    // [--- p ...... c <--]
+                                    for i in (0..parent_touching_index + 1).rev() {
+                                        tree_sequence.push(i);
+                                    }
+                                    for i in (child_touching_index..nodes_circle.len()).rev() {
+                                        tree_sequence.push(i);
+                                    }
                                     is_tree_sequence_ascending = false;
-                                    for i in parent_touching_index+1 .. child_touching_index { match_sequence.push(i); }
+                                    for i in parent_touching_index + 1..child_touching_index {
+                                        match_sequence.push(i);
+                                    }
                                 }
-                            },
+                            }
                         }
                         (match_sequence, tree_sequence)
                     };
-                    debug_assert!(match_sequence.len() % 2 == 0 && tree_sequence.len() % 2 == 1, "parity of sequence wrong");
+                    debug_assert!(
+                        match_sequence.len() % 2 == 0 && tree_sequence.len() % 2 == 1,
+                        "parity of sequence wrong"
+                    );
                     // match the nodes in the match sequence
                     for i in (0..match_sequence.len()).step_by(2) {
-                        let primal_node_internal_ptr_1 = self.get_primal_node_internal_ptr(&nodes_circle[match_sequence[i]].upgrade_force());
-                        let primal_node_internal_ptr_2 = self.get_primal_node_internal_ptr(&nodes_circle[match_sequence[i+1]].upgrade_force());
-                        debug_assert!((match_sequence[i] + 1) % nodes_circle.len() == match_sequence[i+1], "match sequence should be ascending");
-                        let touching_ptr_1 = touching_children[match_sequence[i]].1.clone();  // assuming ascending match sequence
-                        let touching_ptr_2 = touching_children[match_sequence[i+1]].0.clone();  // assuming ascending match sequence
+                        let primal_node_internal_ptr_1 =
+                            self.get_primal_node_internal_ptr(&nodes_circle[match_sequence[i]].upgrade_force());
+                        let primal_node_internal_ptr_2 =
+                            self.get_primal_node_internal_ptr(&nodes_circle[match_sequence[i + 1]].upgrade_force());
+                        debug_assert!(
+                            (match_sequence[i] + 1) % nodes_circle.len() == match_sequence[i + 1],
+                            "match sequence should be ascending"
+                        );
+                        let touching_ptr_1 = touching_children[match_sequence[i]].1.clone(); // assuming ascending match sequence
+                        let touching_ptr_2 = touching_children[match_sequence[i + 1]].0.clone(); // assuming ascending match sequence
                         let mut primal_node_internal_1 = primal_node_internal_ptr_1.write();
                         let mut primal_node_internal_2 = primal_node_internal_ptr_2.write();
-                        primal_node_internal_1.temporary_match = Some((MatchTarget::Peer(primal_node_internal_ptr_2.downgrade()), touching_ptr_1));
-                        primal_node_internal_2.temporary_match = Some((MatchTarget::Peer(primal_node_internal_ptr_1.downgrade()), touching_ptr_2));
-                        interface_ptr.set_grow_state(&primal_node_internal_1.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
-                        interface_ptr.set_grow_state(&primal_node_internal_2.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
+                        primal_node_internal_1.temporary_match =
+                            Some((MatchTarget::Peer(primal_node_internal_ptr_2.downgrade()), touching_ptr_1));
+                        primal_node_internal_2.temporary_match =
+                            Some((MatchTarget::Peer(primal_node_internal_ptr_1.downgrade()), touching_ptr_2));
+                        interface_ptr.set_grow_state(
+                            &primal_node_internal_1.origin.upgrade_force(),
+                            DualNodeGrowState::Stay,
+                            dual_module,
+                        );
+                        interface_ptr.set_grow_state(
+                            &primal_node_internal_2.origin.upgrade_force(),
+                            DualNodeGrowState::Stay,
+                            dual_module,
+                        );
                     }
                     // connect the nodes in the tree sequence to the alternating tree, note that the tree sequence is from parent to child
                     for (idx, current_i) in tree_sequence.iter().enumerate() {
-                        debug_assert!({
-                            if idx + 1 < tree_sequence.len() {
-                                if is_tree_sequence_ascending { (tree_sequence[idx] + 1) % nodes_circle.len() == tree_sequence[idx+1] }
-                                else { (tree_sequence[idx+1] + 1) % nodes_circle.len() == tree_sequence[idx] }
-                            } else { true }
-                        }, "tree sequence orientation must be consistent");
-                        let current_parent_ptr = if idx == 0 { parent_ptr.clone() } else { self.get_primal_node_internal_ptr(&nodes_circle[tree_sequence[idx - 1]].upgrade_force()) };
+                        debug_assert!(
+                            {
+                                if idx + 1 < tree_sequence.len() {
+                                    if is_tree_sequence_ascending {
+                                        (tree_sequence[idx] + 1) % nodes_circle.len() == tree_sequence[idx + 1]
+                                    } else {
+                                        (tree_sequence[idx + 1] + 1) % nodes_circle.len() == tree_sequence[idx]
+                                    }
+                                } else {
+                                    true
+                                }
+                            },
+                            "tree sequence orientation must be consistent"
+                        );
+                        let current_parent_ptr = if idx == 0 {
+                            parent_ptr.clone()
+                        } else {
+                            self.get_primal_node_internal_ptr(&nodes_circle[tree_sequence[idx - 1]].upgrade_force())
+                        };
                         let current_parent_touching_ptr = if idx == 0 {
                             tree_node.parent.as_ref().unwrap().1.clone()
                         } else {
-                            if is_tree_sequence_ascending { touching_children[*current_i].0.clone() } else { touching_children[*current_i].1.clone() }
+                            if is_tree_sequence_ascending {
+                                touching_children[*current_i].0.clone()
+                            } else {
+                                touching_children[*current_i].1.clone()
+                            }
+                        };
+                        let current_child_ptr = if idx == tree_sequence.len() - 1 {
+                            child_ptr.clone()
+                        } else {
+                            self.get_primal_node_internal_ptr(&nodes_circle[tree_sequence[idx + 1]].upgrade_force())
                         };
-                        let current_child_ptr = if idx == tree_sequence.len() - 1 { child_ptr.clone() }
-                            else { self.get_primal_node_internal_ptr(&nodes_circle[tree_sequence[idx + 1]].upgrade_force()) };
                         let current_child_touching_ptr = if idx == tree_sequence.len() - 1 {
                             tree_node.children[0].1.clone()
                         } else {
-                            if is_tree_sequence_ascending { touching_children[*current_i].1.clone() } else { touching_children[*current_i].0.clone() }
+                            if is_tree_sequence_ascending {
+                                touching_children[*current_i].1.clone()
+                            } else {
+                                touching_children[*current_i].0.clone()
+                            }
                         };
                         let current_ptr = self.get_primal_node_internal_ptr(&nodes_circle[*current_i].upgrade_force());
                         let mut current = current_ptr.write();
                         current.tree_node = Some(AlternatingTreeNode {
                             root: tree_node.root.clone(),
                             parent: Some((current_parent_ptr.downgrade(), current_parent_touching_ptr)),
                             children: vec![(current_child_ptr.downgrade(), current_child_touching_ptr)],
                             depth: tree_node.depth + idx,
                         });
-                        interface_ptr.set_grow_state(&current.origin.upgrade_force(), if idx % 2 == 0 { DualNodeGrowState::Shrink } else { DualNodeGrowState::Grow }, dual_module);
+                        interface_ptr.set_grow_state(
+                            &current.origin.upgrade_force(),
+                            if idx % 2 == 0 {
+                                DualNodeGrowState::Shrink
+                            } else {
+                                DualNodeGrowState::Grow
+                            },
+                            dual_module,
+                        );
                     }
-                    {  // connect parent
+                    {
+                        // connect parent
                         lock_write!(parent, parent_ptr);
                         let parent_tree_node = parent.tree_node.as_mut().unwrap();
                         let child_ptr = self.get_primal_node_internal_ptr(&nodes_circle[tree_sequence[0]].upgrade_force());
                         parent_tree_node.children.push((child_ptr.downgrade(), parent_touching_ptr));
                     }
-                    {  // connect child and fix the depth information of the child
+                    {
+                        // connect child and fix the depth information of the child
                         lock_write!(child, child_ptr);
                         let child_tree_node = child.tree_node.as_mut().unwrap();
-                        let parent_ptr = self.get_primal_node_internal_ptr(&nodes_circle[tree_sequence[tree_sequence.len()-1]].upgrade_force());
+                        let parent_ptr = self.get_primal_node_internal_ptr(
+                            &nodes_circle[tree_sequence[tree_sequence.len() - 1]].upgrade_force(),
+                        );
                         child_tree_node.parent = Some((parent_ptr.downgrade(), child_touching_ptr));
                         child.change_sub_tree_root(tree_node.depth + tree_sequence.len(), tree_node.root.upgrade_force());
                     }
-                    {  // remove it from nodes
+                    {
+                        // remove it from nodes
                         lock_write!(module, self);
-                        debug_assert_eq!(module.get_node(primal_node_internal.index), Some(primal_node_internal_ptr.clone()), "index wrong");
+                        debug_assert_eq!(
+                            module.get_node(primal_node_internal.index),
+                            Some(primal_node_internal_ptr.clone()),
+                            "index wrong"
+                        );
                         module.remove_node(primal_node_internal.index);
                     }
-                },
-                MaxUpdateLength::VertexShrinkStop(_node_ptr) => {
+                }
+                MaxUpdateLength::VertexShrinkStop(_) => {
                     if current_conflict_index == 1 {
                         // if this happens, then debug the sorting of conflict events and also check alternating tree: a vertex should never be a floating "-" node
                         unreachable!("VertexShrinkStop conflict cannot be solved by primal module, and should be sorted to the last of the heap")
                     }
                     // just skip and wait for the next round to resolve it, if it's not being resolved already
                 }
-                _ => unreachable!("should not resolve these issues")
+                _ => unreachable!("should not resolve these issues"),
             }
         }
     }
 
-    fn intermediate_matching<D: DualModuleImpl>(&mut self, _interface: &DualModuleInterfacePtr, _dual_module: &mut D) -> IntermediateMatching {
+    fn intermediate_matching<D: DualModuleImpl>(
+        &mut self,
+        _interface: &DualModuleInterfacePtr,
+        _dual_module: &mut D,
+    ) -> IntermediateMatching {
         let mut immediate_matching = IntermediateMatching::new();
         let mut flattened_nodes = vec![];
         self.flatten_nodes(&mut flattened_nodes);
         for primal_node_internal_ptr in flattened_nodes.iter().flatten() {
             let primal_node_internal = primal_node_internal_ptr.read_recursive();
-            debug_assert!(primal_node_internal.tree_node.is_none(), "cannot compute perfect matching with active alternating tree");
+            debug_assert!(
+                primal_node_internal.tree_node.is_none(),
+                "cannot compute perfect matching with active alternating tree"
+            );
             let origin_ptr = primal_node_internal.origin.upgrade_force();
             let interface_node = origin_ptr.read_recursive();
             if interface_node.parent_blossom.is_some() {
-                debug_assert_eq!(primal_node_internal.temporary_match, None, "blossom internal nodes should not be matched");
-                continue  // do not handle this blossom at this level
+                debug_assert_eq!(
+                    primal_node_internal.temporary_match, None,
+                    "blossom internal nodes should not be matched"
+                );
+                continue; // do not handle this blossom at this level
             }
             if let Some((match_target, match_touching_ptr)) = primal_node_internal.temporary_match.as_ref() {
                 match match_target {
                     MatchTarget::Peer(peer_internal_weak) => {
                         let peer_internal_ptr = peer_internal_weak.upgrade_force();
                         let peer_internal = peer_internal_ptr.read_recursive();
-                        if primal_node_internal.index < peer_internal.index {  // to avoid duplicate matched pairs
+                        if primal_node_internal.index < peer_internal.index {
+                            // to avoid duplicate matched pairs
                             let peer_touching_ptr = peer_internal.temporary_match.as_ref().unwrap().1.clone();
                             immediate_matching.peer_matchings.push((
-                                (primal_node_internal.origin.upgrade_force(), match_touching_ptr.clone()), 
-                                (peer_internal.origin.upgrade_force(), peer_touching_ptr)
+                                (primal_node_internal.origin.upgrade_force(), match_touching_ptr.clone()),
+                                (peer_internal.origin.upgrade_force(), peer_touching_ptr),
                             ));
                         }
-                    },
+                    }
                     MatchTarget::VirtualVertex(virtual_vertex) => {
                         immediate_matching.virtual_matchings.push((
-                            (primal_node_internal.origin.upgrade_force(), match_touching_ptr.clone())
-                            , *virtual_vertex
+                            (primal_node_internal.origin.upgrade_force(), match_touching_ptr.clone()),
+                            *virtual_vertex,
                         ));
-                    },
+                    }
                 }
             } else {
-                panic!("cannot compute final matching with unmatched outer node {:?}", primal_node_internal_ptr);
+                panic!(
+                    "cannot compute final matching with unmatched outer node {:?}",
+                    primal_node_internal_ptr
+                );
             }
         }
         immediate_matching
     }
-
 }
 
 impl FusionVisualizer for PrimalModuleSerialPtr {
     fn snapshot(&self, abbrev: bool) -> serde_json::Value {
         // do the sanity check first before taking snapshot
         let flattened_nodes = self.sanity_check().unwrap();
         let mut primal_nodes = Vec::<serde_json::Value>::new();
@@ -840,80 +1233,88 @@
         json!({
             "primal_nodes": primal_nodes,
         })
     }
 }
 
 impl PrimalModuleSerial {
-
     /// return the count of all nodes including those of the children interfaces
     pub fn nodes_count(&self) -> NodeNum {
         let mut count = self.nodes_length as NodeNum;
         if let Some(((_, left_count), (_, right_count))) = &self.children {
             count += left_count + right_count;
         }
         count
     }
 
     /// get node ptr by index; if calling from the ancestor module, node_index is absolute, otherwise it's relative
+    #[allow(clippy::unnecessary_cast)]
     pub fn get_node(&self, relative_node_index: NodeIndex) -> Option<PrimalNodeInternalPtr> {
         debug_assert!(relative_node_index < self.nodes_count(), "cannot find node in this module");
         let mut bias = 0;
         if let Some(((left_weak, left_count), (right_weak, right_count))) = &self.children {
             if relative_node_index < *left_count {
                 // this node belongs to the left
                 return left_weak.upgrade_force().read_recursive().get_node(relative_node_index);
             } else if relative_node_index < *left_count + *right_count {
                 // this node belongs to the right
-                return right_weak.upgrade_force().read_recursive().get_node(relative_node_index - *left_count);
+                return right_weak
+                    .upgrade_force()
+                    .read_recursive()
+                    .get_node(relative_node_index - *left_count);
             }
             bias = left_count + right_count;
         }
         self.nodes[(relative_node_index - bias) as usize].clone()
     }
 
     /// set the corresponding node index to None
+    #[allow(clippy::unnecessary_cast)]
     pub fn remove_node(&mut self, relative_node_index: NodeIndex) {
         debug_assert!(relative_node_index < self.nodes_count(), "cannot find node in this module");
         let mut bias = 0;
         if let Some(((left_weak, left_count), (right_weak, right_count))) = &self.children {
             if relative_node_index < *left_count {
                 // this node belongs to the left
                 left_weak.upgrade_force().write().remove_node(relative_node_index);
-                return
+                return;
             } else if relative_node_index < *left_count + *right_count {
                 // this node belongs to the right
-                right_weak.upgrade_force().write().remove_node(relative_node_index - *left_count);
-                return
+                right_weak
+                    .upgrade_force()
+                    .write()
+                    .remove_node(relative_node_index - *left_count);
+                return;
             }
             bias = left_count + right_count;
         }
         self.nodes[(relative_node_index - bias) as usize] = None;
     }
-
 }
 
 impl PrimalModuleSerialPtr {
-
     pub fn get_primal_node_internal_ptr_option(&self, dual_node_ptr: &DualNodePtr) -> Option<PrimalNodeInternalPtr> {
         let module = self.read_recursive();
         let dual_node = dual_node_ptr.read_recursive();
         let primal_node_internal_ptr = module.get_node(dual_node.index);
         if let Some(primal_node_internal_ptr) = &primal_node_internal_ptr {
             if module.is_fusion {
-                primal_node_internal_ptr.update();  // every time it's accessed, make sure it's update-to-date
+                primal_node_internal_ptr.update(); // every time it's accessed, make sure it's update-to-date
             }
-            debug_assert!(dual_node_ptr == &primal_node_internal_ptr.read_recursive().origin.upgrade_force()
-                , "dual node and primal internal node must corresponds to each other");
+            debug_assert!(
+                dual_node_ptr == &primal_node_internal_ptr.read_recursive().origin.upgrade_force(),
+                "dual node and primal internal node must corresponds to each other"
+            );
         }
         primal_node_internal_ptr
     }
 
     pub fn get_primal_node_internal_ptr(&self, dual_node_ptr: &DualNodePtr) -> PrimalNodeInternalPtr {
-        self.get_primal_node_internal_ptr_option(dual_node_ptr).expect("internal primal node must exists")
+        self.get_primal_node_internal_ptr_option(dual_node_ptr)
+            .expect("internal primal node must exists")
     }
 
     /// get the outer node in the most up-to-date cache
     pub fn get_outer_node(&self, primal_node_internal_ptr: PrimalNodeInternalPtr) -> PrimalNodeInternalPtr {
         let node = primal_node_internal_ptr.read_recursive();
         let origin_ptr = node.origin.upgrade_force();
         let interface_node = origin_ptr.read_recursive();
@@ -923,53 +1324,56 @@
             self.get_outer_node(parent_primal_node_internal_ptr)
         } else {
             primal_node_internal_ptr.clone()
         }
     }
 
     /// find the lowest common ancestor (LCA) of two nodes in the alternating tree, return (LCA, path_1, path_2) where path includes leaf but exclude the LCA
-    pub fn find_lowest_common_ancestor(&self, mut primal_node_internal_ptr_1: PrimalNodeInternalPtr, mut primal_node_internal_ptr_2: PrimalNodeInternalPtr)
-            -> (PrimalNodeInternalPtr, Vec<PrimalNodeInternalPtr>, Vec<PrimalNodeInternalPtr>) {
+    pub fn find_lowest_common_ancestor(
+        &self,
+        mut primal_node_internal_ptr_1: PrimalNodeInternalPtr,
+        mut primal_node_internal_ptr_2: PrimalNodeInternalPtr,
+    ) -> (PrimalNodeInternalPtr, Vec<PrimalNodeInternalPtr>, Vec<PrimalNodeInternalPtr>) {
         let (depth_1, depth_2) = {
             let primal_node_internal_1 = primal_node_internal_ptr_1.read_recursive();
             let primal_node_internal_2 = primal_node_internal_ptr_2.read_recursive();
             let tree_node_1 = primal_node_internal_1.tree_node.as_ref().unwrap();
             let tree_node_2 = primal_node_internal_2.tree_node.as_ref().unwrap();
             debug_assert_eq!(tree_node_1.root, tree_node_2.root, "must belong to the same tree");
             (tree_node_1.depth, tree_node_2.depth)
         };
         let mut path_1 = vec![];
         let mut path_2 = vec![];
         match depth_1.cmp(&depth_2) {
-            Ordering::Greater => {
-                loop {
-                    let ptr = primal_node_internal_ptr_1.clone();
-                    let primal_node_internal = ptr.read_recursive();
-                    let tree_node = primal_node_internal.tree_node.as_ref().unwrap();
-                    if tree_node.depth == depth_2 { break }
-                    path_1.push(primal_node_internal_ptr_1.clone());
-                    primal_node_internal_ptr_1 = tree_node.parent.as_ref().unwrap().0.upgrade_force();
+            Ordering::Greater => loop {
+                let ptr = primal_node_internal_ptr_1.clone();
+                let primal_node_internal = ptr.read_recursive();
+                let tree_node = primal_node_internal.tree_node.as_ref().unwrap();
+                if tree_node.depth == depth_2 {
+                    break;
                 }
+                path_1.push(primal_node_internal_ptr_1.clone());
+                primal_node_internal_ptr_1 = tree_node.parent.as_ref().unwrap().0.upgrade_force();
             },
-            Ordering::Less => {
-                loop {
-                    let ptr = primal_node_internal_ptr_2.clone();
-                    let primal_node_internal = ptr.read_recursive();
-                    let tree_node = primal_node_internal.tree_node.as_ref().unwrap();
-                    if tree_node.depth == depth_1 { break }
-                    path_2.push(primal_node_internal_ptr_2.clone());
-                    primal_node_internal_ptr_2 = tree_node.parent.as_ref().unwrap().0.upgrade_force();
+            Ordering::Less => loop {
+                let ptr = primal_node_internal_ptr_2.clone();
+                let primal_node_internal = ptr.read_recursive();
+                let tree_node = primal_node_internal.tree_node.as_ref().unwrap();
+                if tree_node.depth == depth_1 {
+                    break;
                 }
+                path_2.push(primal_node_internal_ptr_2.clone());
+                primal_node_internal_ptr_2 = tree_node.parent.as_ref().unwrap().0.upgrade_force();
             },
-            Ordering::Equal => { }
+            Ordering::Equal => {}
         }
         // now primal_node_internal_ptr_1 and primal_node_internal_ptr_2 has the same depth, compare them until they're equal
         loop {
             if primal_node_internal_ptr_1 == primal_node_internal_ptr_2 {
-                return (primal_node_internal_ptr_1, path_1, path_2)
+                return (primal_node_internal_ptr_1, path_1, path_2);
             }
             let ptr_1 = primal_node_internal_ptr_1.clone();
             let ptr_2 = primal_node_internal_ptr_2.clone();
             let primal_node_internal_1 = ptr_1.read_recursive();
             let primal_node_internal_2 = ptr_2.read_recursive();
             let tree_node_1 = primal_node_internal_1.tree_node.as_ref().unwrap();
             let tree_node_2 = primal_node_internal_2.tree_node.as_ref().unwrap();
@@ -977,105 +1381,188 @@
             path_2.push(primal_node_internal_ptr_2.clone());
             primal_node_internal_ptr_1 = tree_node_1.parent.as_ref().unwrap().0.upgrade_force();
             primal_node_internal_ptr_2 = tree_node_2.parent.as_ref().unwrap().0.upgrade_force();
         }
     }
 
     /// for any - node, match the children by matching them with + node
-    pub fn match_subtree<D: DualModuleImpl>(tree_node_internal_ptr: PrimalNodeInternalPtr, interface_ptr: &DualModuleInterfacePtr, dual_module: &mut D) {
+    pub fn match_subtree<D: DualModuleImpl>(
+        tree_node_internal_ptr: PrimalNodeInternalPtr,
+        interface_ptr: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) {
         let mut tree_node_internal = tree_node_internal_ptr.write();
         let tree_node = tree_node_internal.tree_node.as_ref().unwrap();
         debug_assert!(tree_node.depth % 2 == 1, "only match - node is possible");
         let child_node_internal_ptr = tree_node.children[0].0.upgrade_force();
-        tree_node_internal.temporary_match = Some((MatchTarget::Peer(child_node_internal_ptr.downgrade()), tree_node.children[0].1.clone()));
-        interface_ptr.set_grow_state(&tree_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
+        tree_node_internal.temporary_match = Some((
+            MatchTarget::Peer(child_node_internal_ptr.downgrade()),
+            tree_node.children[0].1.clone(),
+        ));
+        interface_ptr.set_grow_state(
+            &tree_node_internal.origin.upgrade_force(),
+            DualNodeGrowState::Stay,
+            dual_module,
+        );
         tree_node_internal.tree_node = None;
         let mut child_node_internal = child_node_internal_ptr.write();
-        let child_touching_ptr = child_node_internal.tree_node.as_ref().unwrap().parent.as_ref().unwrap().1.clone();
-        child_node_internal.temporary_match = Some((MatchTarget::Peer(tree_node_internal_ptr.downgrade()), child_touching_ptr));
+        let child_touching_ptr = child_node_internal
+            .tree_node
+            .as_ref()
+            .unwrap()
+            .parent
+            .as_ref()
+            .unwrap()
+            .1
+            .clone();
+        child_node_internal.temporary_match =
+            Some((MatchTarget::Peer(tree_node_internal_ptr.downgrade()), child_touching_ptr));
         let child_tree_node = child_node_internal.tree_node.as_ref().unwrap();
-        interface_ptr.set_grow_state(&child_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
+        interface_ptr.set_grow_state(
+            &child_node_internal.origin.upgrade_force(),
+            DualNodeGrowState::Stay,
+            dual_module,
+        );
         for (grandson_ptr, _) in child_tree_node.children.iter() {
             Self::match_subtree(grandson_ptr.upgrade_force(), interface_ptr, dual_module);
         }
         child_node_internal.tree_node = None;
     }
 
     /// for any + node, match it with another node will augment the whole tree, breaking out into several matched pairs;
     /// `tree_grandson_ptr` is the grandson of tree_node_internal_ptr that touches `match_node_internal_ptr`
-    pub fn augment_tree_given_matched<D: DualModuleImpl>(tree_node_internal_ptr: PrimalNodeInternalPtr, match_node_internal_ptr: PrimalNodeInternalPtr
-            , tree_touching_ptr: DualNodeWeak, interface_ptr: &DualModuleInterfacePtr, dual_module: &mut D) {
+    pub fn augment_tree_given_matched<D: DualModuleImpl>(
+        tree_node_internal_ptr: PrimalNodeInternalPtr,
+        match_node_internal_ptr: PrimalNodeInternalPtr,
+        tree_touching_ptr: DualNodeWeak,
+        interface_ptr: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) {
         let mut tree_node_internal = tree_node_internal_ptr.write();
-        tree_node_internal.temporary_match = Some((MatchTarget::Peer(match_node_internal_ptr.downgrade()), tree_touching_ptr));
-        interface_ptr.set_grow_state(&tree_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
+        tree_node_internal.temporary_match =
+            Some((MatchTarget::Peer(match_node_internal_ptr.downgrade()), tree_touching_ptr));
+        interface_ptr.set_grow_state(
+            &tree_node_internal.origin.upgrade_force(),
+            DualNodeGrowState::Stay,
+            dual_module,
+        );
         let tree_node = tree_node_internal.tree_node.as_ref().unwrap();
         debug_assert!(tree_node.depth % 2 == 0, "only augment + node is possible");
         for (child_ptr, _) in tree_node.children.iter() {
             if child_ptr != &match_node_internal_ptr.downgrade() {
                 Self::match_subtree(child_ptr.upgrade_force(), interface_ptr, dual_module);
             }
         }
-        if tree_node.depth != 0 {  // it's not root, then we need to match parent to grandparent
+        if tree_node.depth != 0 {
+            // it's not root, then we need to match parent to grandparent
             let parent_node_internal_weak = tree_node.parent.as_ref().unwrap().0.clone();
             let parent_node_internal_ptr = parent_node_internal_weak.upgrade_force();
-            let grandparent_node_internal_ptr = {  // must unlock parent
+            let grandparent_node_internal_ptr = {
+                // must unlock parent
                 let mut parent_node_internal = parent_node_internal_ptr.write();
                 let parent_tree_node = parent_node_internal.tree_node.as_ref().unwrap();
                 let grandparent_node_internal_weak = parent_tree_node.parent.as_ref().unwrap().0.clone();
-                parent_node_internal.temporary_match = Some((MatchTarget::Peer(grandparent_node_internal_weak.clone()), parent_tree_node.parent.as_ref().unwrap().1.clone()));
+                parent_node_internal.temporary_match = Some((
+                    MatchTarget::Peer(grandparent_node_internal_weak.clone()),
+                    parent_tree_node.parent.as_ref().unwrap().1.clone(),
+                ));
                 parent_node_internal.tree_node = None;
-                interface_ptr.set_grow_state(&parent_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
+                interface_ptr.set_grow_state(
+                    &parent_node_internal.origin.upgrade_force(),
+                    DualNodeGrowState::Stay,
+                    dual_module,
+                );
                 grandparent_node_internal_weak.upgrade_force()
             };
             let grandparent_touching_ptr = {
                 let grandparent_node_internal = grandparent_node_internal_ptr.read_recursive();
                 let grandparent_tree_node = grandparent_node_internal.tree_node.as_ref().unwrap();
-                let idx = grandparent_tree_node.children.iter().position(|(ptr, _)| ptr == &parent_node_internal_weak).expect("should find child");
+                let idx = grandparent_tree_node
+                    .children
+                    .iter()
+                    .position(|(ptr, _)| ptr == &parent_node_internal_weak)
+                    .expect("should find child");
                 grandparent_tree_node.children[idx].1.clone()
             };
-            Self::augment_tree_given_matched(grandparent_node_internal_ptr, parent_node_internal_ptr, grandparent_touching_ptr, interface_ptr, dual_module);
+            Self::augment_tree_given_matched(
+                grandparent_node_internal_ptr,
+                parent_node_internal_ptr,
+                grandparent_touching_ptr,
+                interface_ptr,
+                dual_module,
+            );
         }
         tree_node_internal.tree_node = None;
     }
 
     /// for any + node, match it with virtual boundary will augment the whole tree, breaking out into several matched pairs
-    pub fn augment_tree_given_virtual_vertex<D: DualModuleImpl>(&self, tree_node_internal_ptr: PrimalNodeInternalPtr, virtual_vertex_index: VertexIndex
-            , tree_touching_ptr: DualNodeWeak, interface_ptr: &DualModuleInterfacePtr, dual_module: &mut D) {
+    pub fn augment_tree_given_virtual_vertex<D: DualModuleImpl>(
+        &self,
+        tree_node_internal_ptr: PrimalNodeInternalPtr,
+        virtual_vertex_index: VertexIndex,
+        tree_touching_ptr: DualNodeWeak,
+        interface_ptr: &DualModuleInterfacePtr,
+        dual_module: &mut D,
+    ) {
         let mut tree_node_internal = tree_node_internal_ptr.write();
         tree_node_internal.temporary_match = Some((MatchTarget::VirtualVertex(virtual_vertex_index), tree_touching_ptr));
-        interface_ptr.set_grow_state(&tree_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
+        interface_ptr.set_grow_state(
+            &tree_node_internal.origin.upgrade_force(),
+            DualNodeGrowState::Stay,
+            dual_module,
+        );
         let tree_node = tree_node_internal.tree_node.as_ref().unwrap();
         debug_assert!(tree_node.depth % 2 == 0, "only augment + node is possible");
         for (child_ptr, _) in tree_node.children.iter() {
             Self::match_subtree(child_ptr.upgrade_force(), interface_ptr, dual_module);
         }
-        if tree_node.depth != 0 {  // it's not root, then we need to match parent to grandparent
+        if tree_node.depth != 0 {
+            // it's not root, then we need to match parent to grandparent
             let parent_node_internal_weak = tree_node.parent.as_ref().unwrap().0.clone();
             let parent_node_internal_ptr = parent_node_internal_weak.upgrade_force();
-            let grandparent_node_internal_ptr = {  // must unlock parent
+            let grandparent_node_internal_ptr = {
+                // must unlock parent
                 let mut parent_node_internal = parent_node_internal_ptr.write();
                 let parent_tree_node = parent_node_internal.tree_node.as_ref().unwrap();
                 let grandparent_node_internal_weak = parent_tree_node.parent.as_ref().unwrap().0.clone();
-                parent_node_internal.temporary_match = Some((MatchTarget::Peer(grandparent_node_internal_weak.clone()), parent_tree_node.parent.as_ref().unwrap().1.clone()));
+                parent_node_internal.temporary_match = Some((
+                    MatchTarget::Peer(grandparent_node_internal_weak.clone()),
+                    parent_tree_node.parent.as_ref().unwrap().1.clone(),
+                ));
                 parent_node_internal.tree_node = None;
-                interface_ptr.set_grow_state(&parent_node_internal.origin.upgrade_force(), DualNodeGrowState::Stay, dual_module);
+                interface_ptr.set_grow_state(
+                    &parent_node_internal.origin.upgrade_force(),
+                    DualNodeGrowState::Stay,
+                    dual_module,
+                );
                 grandparent_node_internal_weak.upgrade_force()
             };
             let grandparent_touching_ptr = {
                 let grandparent_node_internal = grandparent_node_internal_ptr.read_recursive();
                 let grandparent_tree_node = grandparent_node_internal.tree_node.as_ref().unwrap();
-                let idx = grandparent_tree_node.children.iter().position(|(ptr, _)| ptr == &parent_node_internal_weak).expect("should find child");
+                let idx = grandparent_tree_node
+                    .children
+                    .iter()
+                    .position(|(ptr, _)| ptr == &parent_node_internal_weak)
+                    .expect("should find child");
                 grandparent_tree_node.children[idx].1.clone()
             };
-            Self::augment_tree_given_matched(grandparent_node_internal_ptr, parent_node_internal_ptr, grandparent_touching_ptr, interface_ptr, dual_module);
+            Self::augment_tree_given_matched(
+                grandparent_node_internal_ptr,
+                parent_node_internal_ptr,
+                grandparent_touching_ptr,
+                interface_ptr,
+                dual_module,
+            );
         }
         tree_node_internal.tree_node = None;
     }
 
     /// DFS flatten the nodes
+    #[allow(clippy::unnecessary_cast)]
     pub fn flatten_nodes(&self, flattened_nodes: &mut Vec<Option<PrimalNodeInternalPtr>>) {
         let module = self.read_recursive();
         let flattened_nodes_length = flattened_nodes.len();
         // the order matters: left -> right -> myself
         if let Some(((left_child_weak, _), (right_child_weak, _))) = &module.children {
             left_child_weak.upgrade_force().flatten_nodes(flattened_nodes);
             right_child_weak.upgrade_force().flatten_nodes(flattened_nodes);
@@ -1088,20 +1575,21 @@
             }
             flattened_nodes.push(primal_node_internal_ptr.clone());
         }
         debug_assert_eq!(flattened_nodes.len() - flattened_nodes_length, module.nodes_count() as usize);
     }
 
     /// fuse two modules by copying the nodes in `other` into myself
+    #[allow(clippy::unnecessary_cast)]
     pub fn slow_fuse(&self, left: &Self, right: &Self) {
         let mut module = self.write();
-        module.is_fusion = true;  // for safety
+        module.is_fusion = true; // for safety
         for other in [left, right] {
             let mut other_module = other.write();
-            other_module.is_fusion = true;  // enable pointer update
+            other_module.is_fusion = true; // enable pointer update
             let bias = module.nodes_length as NodeIndex;
             for other_node_index in 0..other_module.nodes_length as NodeIndex {
                 let node_ptr = &other_module.nodes[other_node_index as usize];
                 if let Some(node_ptr) = node_ptr {
                     let mut node = node_ptr.write();
                     debug_assert_eq!(node.index, other_node_index);
                     node.index += bias;
@@ -1121,28 +1609,28 @@
 
     /// fuse two modules by (virtually) copying the nodes in `other` into myself, with O(1) time complexity
     pub fn fuse(&self, left: &Self, right: &Self) {
         let parent_weak = self.downgrade();
         let left_weak = left.downgrade();
         let right_weak = right.downgrade();
         let mut module = self.write();
-        module.is_fusion = true;  // for safety
+        module.is_fusion = true; // for safety
         debug_assert_eq!(module.nodes_length, 0, "fast fuse doesn't support non-empty fuse");
         debug_assert!(module.children.is_none(), "cannot fuse twice");
         let mut left_module = left.write();
         let mut right_module = right.write();
         debug_assert!(left_module.parent.is_none(), "cannot fuse an module twice");
         debug_assert!(right_module.parent.is_none(), "cannot fuse an module twice");
         left_module.parent = Some(parent_weak.clone());
         right_module.parent = Some(parent_weak);
         left_module.index_bias = 0;
         right_module.index_bias = left_module.nodes_count();
         module.children = Some((
             (left_weak, left_module.nodes_count()),
-            (right_weak, right_module.nodes_count())
+            (right_weak, right_module.nodes_count()),
         ));
         // the possible_break should be a small subset, thus copying them is fine
         for other_module in [left_module, right_module] {
             for node_index in other_module.possible_break.iter() {
                 module.possible_break.push(*node_index + other_module.index_bias);
             }
         }
@@ -1152,280 +1640,400 @@
     #[allow(clippy::collapsible_else_if)]
     pub fn sanity_check(&self) -> Result<Vec<Option<PrimalNodeInternalPtr>>, String> {
         let mut flattened_nodes = vec![];
         self.flatten_nodes(&mut flattened_nodes);
         for (index, primal_module_internal_ptr) in flattened_nodes.iter().enumerate() {
             if let Some(primal_module_internal_ptr) = primal_module_internal_ptr {
                 let primal_module_internal = primal_module_internal_ptr.read_recursive();
-                if primal_module_internal.index != index as NodeIndex { return Err(format!("primal node index wrong: expected {}, actual {}", index, primal_module_internal.index)) }
+                if primal_module_internal.index != index as NodeIndex {
+                    return Err(format!(
+                        "primal node index wrong: expected {}, actual {}",
+                        index, primal_module_internal.index
+                    ));
+                }
                 let origin_ptr = primal_module_internal.origin.upgrade_force();
                 let origin_node = origin_ptr.read_recursive();
-                if origin_node.index != primal_module_internal.index { return Err(format!("origin index wrong: expected {}, actual {}", index, origin_node.index)) }
+                if origin_node.index != primal_module_internal.index {
+                    return Err(format!(
+                        "origin index wrong: expected {}, actual {}",
+                        index, origin_node.index
+                    ));
+                }
                 if primal_module_internal.temporary_match.is_some() && primal_module_internal.tree_node.is_some() {
-                    return Err(format!("{} temporary match and tree node cannot both exists", index))
+                    return Err(format!("{} temporary match and tree node cannot both exists", index));
                 }
                 if origin_node.parent_blossom.is_some() {
-                    if primal_module_internal.tree_node.is_some() { return Err(format!("blossom internal node {index} is still in a tree")) }
-                    if primal_module_internal.temporary_match.is_some() { return Err(format!("blossom internal node {index} is still matched")) }
+                    if primal_module_internal.tree_node.is_some() {
+                        return Err(format!("blossom internal node {index} is still in a tree"));
+                    }
+                    if primal_module_internal.temporary_match.is_some() {
+                        return Err(format!("blossom internal node {index} is still matched"));
+                    }
                 }
                 if let Some((match_target, _)) = primal_module_internal.temporary_match.as_ref() {
-                    if origin_node.grow_state != DualNodeGrowState::Stay { return Err(format!("matched node {index} is not set to Stay")) }
+                    if origin_node.grow_state != DualNodeGrowState::Stay {
+                        return Err(format!("matched node {index} is not set to Stay"));
+                    }
                     match match_target {
                         MatchTarget::Peer(peer_weak) => {
                             let peer_ptr = peer_weak.upgrade_force();
                             let peer = peer_ptr.read_recursive();
                             if let Some((peer_match_target, _)) = peer.temporary_match.as_ref() {
                                 if peer_match_target != &MatchTarget::Peer(primal_module_internal_ptr.downgrade()) {
-                                    return Err(format!("match peer {} is not matched with {}, instead it's {:?}", peer.index, index, peer_match_target))
+                                    return Err(format!(
+                                        "match peer {} is not matched with {}, instead it's {:?}",
+                                        peer.index, index, peer_match_target
+                                    ));
                                 }
                             } else {
-                                return Err("match peer is not marked as matched".to_string())
+                                return Err("match peer is not marked as matched".to_string());
                             }
-                        },
-                        MatchTarget::VirtualVertex(_vertex_idx) => { },  // nothing to check
+                        }
+                        MatchTarget::VirtualVertex(_vertex_idx) => {} // nothing to check
                     }
                 }
                 if let Some(tree_node) = primal_module_internal.tree_node.as_ref() {
                     // first check if every child's parent is myself
                     for (child_weak, _) in tree_node.children.iter() {
                         let child_ptr = child_weak.upgrade_force();
                         let child = child_ptr.read_recursive();
                         if let Some(child_tree_node) = child.tree_node.as_ref() {
-                            if child_tree_node.parent.as_ref().map(|x| &x.0) != Some(&primal_module_internal_ptr.downgrade()) {
-                                return Err(format!("{}'s child {} has a different parent, link broken", index, child.index))
+                            if child_tree_node.parent.as_ref().map(|x| &x.0) != Some(&primal_module_internal_ptr.downgrade())
+                            {
+                                return Err(format!(
+                                    "{}'s child {} has a different parent, link broken",
+                                    index, child.index
+                                ));
                             }
-                        } else { return Err(format!("{}'s child {} doesn't belong to any tree, link broken", index, child.index)) }
+                        } else {
+                            return Err(format!(
+                                "{}'s child {} doesn't belong to any tree, link broken",
+                                index, child.index
+                            ));
+                        }
                         // check if child is still tracked, i.e. inside self.nodes
                         let module = self.read_recursive();
                         if child.index >= module.nodes_count() || module.get_node(child.index).is_none() {
-                            return Err(format!("child's index {} is not in the interface", child.index))
+                            return Err(format!("child's index {} is not in the interface", child.index));
                         }
                         let tracked_child_ptr = module.get_node(child.index).unwrap();
                         if tracked_child_ptr != child_ptr {
-                            return Err(format!("the tracked ptr of child {} is not what's being pointed", child.index))
+                            return Err(format!(
+                                "the tracked ptr of child {} is not what's being pointed",
+                                child.index
+                            ));
                         }
                     }
                     // then check if I'm my parent's child
                     if let Some((parent_weak, _)) = tree_node.parent.as_ref() {
                         let parent_ptr = parent_weak.upgrade_force();
                         let parent = parent_ptr.read_recursive();
                         if let Some(parent_tree_node) = parent.tree_node.as_ref() {
                             let mut found_match_count = 0;
                             for (node_ptr, _) in parent_tree_node.children.iter() {
                                 if node_ptr == &primal_module_internal_ptr.downgrade() {
                                     found_match_count += 1;
                                 }
                             }
                             if found_match_count != 1 {
-                                return Err(format!("{} is the parent of {} but the child only presents {} times", parent.index, index, found_match_count))
+                                return Err(format!(
+                                    "{} is the parent of {} but the child only presents {} times",
+                                    parent.index, index, found_match_count
+                                ));
                             }
-                        } else { return Err(format!("{}'s parent {} doesn't belong to any tree, link broken", index, parent.index)) }
+                        } else {
+                            return Err(format!(
+                                "{}'s parent {} doesn't belong to any tree, link broken",
+                                index, parent.index
+                            ));
+                        }
                         // check if parent is still tracked, i.e. inside self.nodes
                         let module = self.read_recursive();
                         if parent.index >= module.nodes_count() || module.get_node(parent.index).is_none() {
-                            return Err(format!("parent's index {} is not in the interface", parent.index))
+                            return Err(format!("parent's index {} is not in the interface", parent.index));
                         }
                         let tracked_parent_ptr = module.get_node(parent.index).unwrap();
                         if tracked_parent_ptr != parent_ptr {
-                            return Err(format!("the tracked ptr of child {} is not what's being pointed", parent.index))
+                            return Err(format!(
+                                "the tracked ptr of child {} is not what's being pointed",
+                                parent.index
+                            ));
                         }
                     } else {
                         if tree_node.root != primal_module_internal_ptr.downgrade() {
-                            return Err(format!("{} is not the root of the tree, yet it has no parent", index))
+                            return Err(format!("{} is not the root of the tree, yet it has no parent", index));
                         }
                     }
                     // then check if the root and the depth is correct
                     let mut current_ptr = primal_module_internal_ptr.clone();
                     let mut current_up = 0;
                     loop {
                         let current = current_ptr.read_recursive();
                         // check if current is still tracked, i.e. inside self.nodes
                         let module = self.read_recursive();
                         if current.index >= module.nodes_count() || module.get_node(current.index).is_none() {
-                            return Err(format!("current's index {} is not in the interface", current.index))
+                            return Err(format!("current's index {} is not in the interface", current.index));
                         }
                         let tracked_current_ptr = module.get_node(current.index).unwrap();
                         if tracked_current_ptr != current_ptr {
-                            return Err(format!("the tracked ptr of current {} is not what's being pointed", current.index))
+                            return Err(format!(
+                                "the tracked ptr of current {} is not what's being pointed",
+                                current.index
+                            ));
                         }
                         // go to parent
                         if let Some(current_tree_node) = current.tree_node.as_ref() {
                             if let Some((current_parent_ptr, _)) = current_tree_node.parent.as_ref() {
                                 let current_parent_ptr = current_parent_ptr.clone();
                                 drop(current);
                                 current_ptr = current_parent_ptr.upgrade_force();
                                 current_up += 1;
                             } else {
                                 // confirm this is root and then break the loop
                                 if current_tree_node.root != current_ptr.downgrade() {
-                                    return Err(format!("current {} is not the root of the tree, yet it has no parent", current.index))
+                                    return Err(format!(
+                                        "current {} is not the root of the tree, yet it has no parent",
+                                        current.index
+                                    ));
                                 }
-                                break
+                                break;
                             }
-                        } else { return Err(format!("climbing up from {} to {} but it doesn't belong to a tree anymore", index, current.index)) }
+                        } else {
+                            return Err(format!(
+                                "climbing up from {} to {} but it doesn't belong to a tree anymore",
+                                index, current.index
+                            ));
+                        }
                     }
                     if current_up != tree_node.depth {
-                        return Err(format!("{} is marked with depth {} but the real depth is {}", index, tree_node.depth, current_up))
+                        return Err(format!(
+                            "{} is marked with depth {} but the real depth is {}",
+                            index, tree_node.depth, current_up
+                        ));
                     }
                     if current_ptr.downgrade() != tree_node.root {
-                        return Err(format!("{} is marked with root {:?} but the real root is {:?}", index, tree_node.root, current_ptr))
+                        return Err(format!(
+                            "{} is marked with root {:?} but the real root is {:?}",
+                            index, tree_node.root, current_ptr
+                        ));
                     }
                 }
             }
         }
         Ok(flattened_nodes)
     }
-
 }
 
-
 #[cfg(test)]
 pub mod tests {
-    use super::*;
-    use super::super::example_codes::*;
     use super::super::dual_module_serial::*;
+    use super::super::example_codes::*;
     use super::super::*;
+    use super::*;
 
-    pub fn primal_module_serial_basic_standard_syndrome_optional_viz(d: VertexNum, visualize_filename: Option<String>, defect_vertices: Vec<VertexIndex>, final_dual: Weight)
-            -> (DualModuleInterfacePtr, PrimalModuleSerialPtr, DualModuleSerial) {
+    pub fn primal_module_serial_basic_standard_syndrome_optional_viz(
+        d: VertexNum,
+        visualize_filename: Option<String>,
+        defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+    ) -> (DualModuleInterfacePtr, PrimalModuleSerialPtr, DualModuleSerial) {
         println!("{defect_vertices:?}");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(d, 0.1, half_weight);
         let mut visualizer = match visualize_filename.as_ref() {
             Some(visualize_filename) => {
-                let visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+                let visualizer = Visualizer::new(
+                    Some(visualize_data_folder() + visualize_filename.as_str()),
+                    code.get_positions(),
+                    true,
+                )
+                .unwrap();
                 print_visualize_link(visualize_filename.clone());
                 Some(visualizer)
-            }, None => None
+            }
+            None => None,
         };
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // create primal module
         let mut primal_module = PrimalModuleSerialPtr::new_empty(&initializer);
-        primal_module.write().debug_resolve_only_one = true;  // to enable debug mode
-        // try to work on a simple syndrome
+        primal_module.write().debug_resolve_only_one = true; // to enable debug mode
+                                                             // try to work on a simple syndrome
         code.set_defect_vertices(&defect_vertices);
         let interface_ptr = DualModuleInterfacePtr::new_empty();
         primal_module.solve_visualizer(&interface_ptr, &code.get_syndrome(), &mut dual_module, visualizer.as_mut());
         let perfect_matching = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         let mut subgraph_builder = SubGraphBuilder::new(&initializer);
         subgraph_builder.load_perfect_matching(&perfect_matching);
         let subgraph = subgraph_builder.get_subgraph();
         if let Some(visualizer) = visualizer.as_mut() {
-            visualizer.snapshot_combined("perfect matching and subgraph".to_string(), vec![&interface_ptr, &dual_module
-                , &perfect_matching, &VisualizeSubgraph::new(&subgraph)]).unwrap();
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), subgraph_builder.total_weight(), "unmatched sum dual variables");
-        assert_eq!(interface_ptr.sum_dual_variables(), final_dual * 2 * half_weight, "unexpected final dual variable sum");
+            visualizer
+                .snapshot_combined(
+                    "perfect matching and subgraph".to_string(),
+                    vec![
+                        &interface_ptr,
+                        &dual_module,
+                        &perfect_matching,
+                        &VisualizeSubgraph::new(&subgraph),
+                    ],
+                )
+                .unwrap();
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            subgraph_builder.total_weight(),
+            "unmatched sum dual variables"
+        );
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            final_dual * 2 * half_weight,
+            "unexpected final dual variable sum"
+        );
         (interface_ptr, primal_module, dual_module)
     }
 
-    pub fn primal_module_serial_basic_standard_syndrome(d: VertexNum, visualize_filename: String, defect_vertices: Vec<VertexIndex>, final_dual: Weight)
-            -> (DualModuleInterfacePtr, PrimalModuleSerialPtr, DualModuleSerial) {
+    pub fn primal_module_serial_basic_standard_syndrome(
+        d: VertexNum,
+        visualize_filename: String,
+        defect_vertices: Vec<VertexIndex>,
+        final_dual: Weight,
+    ) -> (DualModuleInterfacePtr, PrimalModuleSerialPtr, DualModuleSerial) {
         primal_module_serial_basic_standard_syndrome_optional_viz(d, Some(visualize_filename), defect_vertices, final_dual)
     }
 
     /// test a simple blossom
     #[test]
-    fn primal_module_serial_basic_1() {  // cargo test primal_module_serial_basic_1 -- --nocapture
+    fn primal_module_serial_basic_1() {
+        // cargo test primal_module_serial_basic_1 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_1.json");
         let defect_vertices = vec![18, 26, 34];
         primal_module_serial_basic_standard_syndrome(7, visualize_filename, defect_vertices, 4);
     }
 
     /// test a free node conflict with a virtual boundary
     #[test]
-    fn primal_module_serial_basic_2() {  // cargo test primal_module_serial_basic_2 -- --nocapture
+    fn primal_module_serial_basic_2() {
+        // cargo test primal_module_serial_basic_2 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_2.json");
         let defect_vertices = vec![16];
         primal_module_serial_basic_standard_syndrome(7, visualize_filename, defect_vertices, 1);
     }
 
     /// test a free node conflict with a matched node (with virtual boundary)
     #[test]
-    fn primal_module_serial_basic_3() {  // cargo test primal_module_serial_basic_3 -- --nocapture
+    fn primal_module_serial_basic_3() {
+        // cargo test primal_module_serial_basic_3 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_3.json");
         let defect_vertices = vec![16, 26];
         primal_module_serial_basic_standard_syndrome(7, visualize_filename, defect_vertices, 3);
     }
 
     /// test blossom shrinking and expanding
     #[test]
-    fn primal_module_serial_basic_4() {  // cargo test primal_module_serial_basic_4 -- --nocapture
+    fn primal_module_serial_basic_4() {
+        // cargo test primal_module_serial_basic_4 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_4.json");
         let defect_vertices = vec![16, 52, 65, 76, 112];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 10);
     }
 
     /// test blossom conflicts with vertex
     #[test]
-    fn primal_module_serial_basic_5() {  // cargo test primal_module_serial_basic_5 -- --nocapture
+    fn primal_module_serial_basic_5() {
+        // cargo test primal_module_serial_basic_5 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_5.json");
         let defect_vertices = vec![39, 51, 61, 62, 63, 64, 65, 75, 87, 67];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 6);
     }
 
     /// test cascaded blossom
     #[test]
-    fn primal_module_serial_basic_6() {  // cargo test primal_module_serial_basic_6 -- --nocapture
+    fn primal_module_serial_basic_6() {
+        // cargo test primal_module_serial_basic_6 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_6.json");
         let defect_vertices = vec![39, 51, 61, 62, 63, 64, 65, 75, 87];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 6);
     }
 
     /// test two alternating trees conflict with each other
     #[test]
-    fn primal_module_serial_basic_7() {  // cargo test primal_module_serial_basic_7 -- --nocapture
+    fn primal_module_serial_basic_7() {
+        // cargo test primal_module_serial_basic_7 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_7.json");
         let defect_vertices = vec![37, 61, 63, 66, 68, 44];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 7);
     }
 
     /// test an alternating tree touches a virtual boundary
     #[test]
-    fn primal_module_serial_basic_8() {  // cargo test primal_module_serial_basic_8 -- --nocapture
+    fn primal_module_serial_basic_8() {
+        // cargo test primal_module_serial_basic_8 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_8.json");
         let defect_vertices = vec![61, 64, 67];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 5);
     }
 
     /// test a matched node (with virtual boundary) conflicts with an alternating tree
     #[test]
-    fn primal_module_serial_basic_9() {  // cargo test primal_module_serial_basic_9 -- --nocapture
+    fn primal_module_serial_basic_9() {
+        // cargo test primal_module_serial_basic_9 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_9.json");
         let defect_vertices = vec![60, 63, 66, 30];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 6);
     }
 
     /// test the error pattern in the paper
     #[test]
-    fn primal_module_serial_basic_10() {  // cargo test primal_module_serial_basic_10 -- --nocapture
+    fn primal_module_serial_basic_10() {
+        // cargo test primal_module_serial_basic_10 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_10.json");
         let defect_vertices = vec![39, 52, 63, 90, 100];
         primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 9);
     }
 
+    /// test the error pattern in the paper
+    #[test]
+    fn primal_module_serial_default_example() {
+        // cargo test primal_module_serial_default_example -- --nocapture
+        let visualize_filename = static_visualize_data_filename();
+        let defect_vertices = vec![39, 52, 63, 90, 100];
+        primal_module_serial_basic_standard_syndrome(11, visualize_filename, defect_vertices, 9);
+    }
+
     /// debug a case of deadlock after changing the strategy of detecting conflicts around VertexShrinkStop;
     /// reason: forget to check whether conflicting nodes are growing: only growing one should be reported
     #[test]
-    fn primal_module_serial_basic_11() {  // cargo test primal_module_serial_basic_11 -- --nocapture
+    fn primal_module_serial_basic_11() {
+        // cargo test primal_module_serial_basic_11 -- --nocapture
         let visualize_filename = format!("primal_module_serial_basic_11.json");
-        let defect_vertices = vec![13, 29, 52, 53, 58, 60, 71, 74, 76, 87, 96, 107, 112, 118, 121, 122, 134, 137, 141, 145, 152, 153, 154, 156, 157, 169, 186, 202, 203, 204, 230, 231];
+        let defect_vertices = vec![
+            13, 29, 52, 53, 58, 60, 71, 74, 76, 87, 96, 107, 112, 118, 121, 122, 134, 137, 141, 145, 152, 153, 154, 156,
+            157, 169, 186, 202, 203, 204, 230, 231,
+        ];
         primal_module_serial_basic_standard_syndrome(15, visualize_filename, defect_vertices, 20);
     }
 
     /// debug a case where it disagree with blossom V library, mine reports 11866, blossom V reports 12284
     #[test]
-    fn primal_module_debug_1() {  // cargo test primal_module_debug_1 -- --nocapture
+    fn primal_module_debug_1() {
+        // cargo test primal_module_debug_1 -- --nocapture
         let visualize_filename = format!("primal_module_debug_1.json");
-        let defect_vertices = vec![34, 35, 84, 89, 92, 100, 141, 145, 149, 164, 193, 201, 205, 220, 235, 242, 243, 260, 261, 290, 300, 308, 309, 315, 317];
+        let defect_vertices = vec![
+            34, 35, 84, 89, 92, 100, 141, 145, 149, 164, 193, 201, 205, 220, 235, 242, 243, 260, 261, 290, 300, 308, 309,
+            315, 317,
+        ];
         let max_half_weight = 500;
         let mut code = CircuitLevelPlanarCode::new(7, 7, 0.01, max_half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         let initializer = code.get_initializer();
         // blossom V ground truth
         let blossom_mwpm_result = blossom_v_mwpm(&initializer, &defect_vertices);
         println!("blossom_mwpm_result: {blossom_mwpm_result:?}");
         let blossom_details = detailed_matching(&initializer, &defect_vertices, &blossom_mwpm_result);
         let mut blossom_total_weight = 0;
@@ -1433,176 +2041,254 @@
             println!("    {detail:?}");
             blossom_total_weight += detail.weight;
         }
         // create dual module
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // create primal module
         let mut primal_module = PrimalModuleSerialPtr::new_empty(&initializer);
-        primal_module.write().debug_resolve_only_one = true;  // to enable debug mode
-        // try to work on a simple syndrome
+        primal_module.write().debug_resolve_only_one = true; // to enable debug mode
+                                                             // try to work on a simple syndrome
         code.set_defect_vertices(&defect_vertices);
         let interface_ptr = DualModuleInterfacePtr::new_empty();
         primal_module.solve_visualizer(&interface_ptr, &code.get_syndrome(), &mut dual_module, Some(&mut visualizer));
         let fusion_mwpm = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         let fusion_mwpm_result = fusion_mwpm.legacy_get_mwpm_result(defect_vertices.clone());
         let fusion_details = detailed_matching(&initializer, &defect_vertices, &fusion_mwpm_result);
         let mut fusion_total_weight = 0;
         for detail in fusion_details.iter() {
             println!("    {detail:?}");
             fusion_total_weight += detail.weight;
         }
-        assert_eq!(fusion_total_weight, blossom_total_weight, "unexpected final dual variable sum");
-        {  // also test subgraph builder
+        assert_eq!(
+            fusion_total_weight, blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
+        {
+            // also test subgraph builder
             let mut subgraph_builder = SubGraphBuilder::new(&initializer);
             subgraph_builder.load_perfect_matching(&fusion_mwpm);
-            assert_eq!(subgraph_builder.total_weight(), blossom_total_weight, "unexpected final dual variable sum");
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), blossom_total_weight, "unexpected final dual variable sum");
+            assert_eq!(
+                subgraph_builder.total_weight(),
+                blossom_total_weight,
+                "unexpected final dual variable sum"
+            );
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
     }
 
     /// debug a case where it disagree with blossom V library, mine reports 33000, blossom V reports 34000
     #[test]
-    fn primal_module_debug_2() {  // cargo test primal_module_debug_2 -- --nocapture
+    fn primal_module_debug_2() {
+        // cargo test primal_module_debug_2 -- --nocapture
         let visualize_filename = format!("primal_module_debug_2.json");
-        let defect_vertices = vec![7, 8, 10, 22, 23, 24, 25, 37, 38, 39, 40, 42, 43, 69, 57, 59, 60, 72, 76, 93, 109, 121, 123, 125, 135, 136, 137, 138, 139, 140, 141, 150, 151, 153, 154, 155, 166, 171, 172, 181, 183, 184, 188, 200, 204, 219, 233];
+        let defect_vertices = vec![
+            7, 8, 10, 22, 23, 24, 25, 37, 38, 39, 40, 42, 43, 69, 57, 59, 60, 72, 76, 93, 109, 121, 123, 125, 135, 136, 137,
+            138, 139, 140, 141, 150, 151, 153, 154, 155, 166, 171, 172, 181, 183, 184, 188, 200, 204, 219, 233,
+        ];
         let max_half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(15, 0.3, max_half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         let initializer = code.get_initializer();
         // blossom V ground truth
         let blossom_mwpm_result = blossom_v_mwpm(&initializer, &defect_vertices);
         let blossom_details = detailed_matching(&initializer, &defect_vertices, &blossom_mwpm_result);
         let mut blossom_total_weight = 0;
         for detail in blossom_details.iter() {
             println!("    {detail:?}");
             blossom_total_weight += detail.weight;
         }
         // create dual module
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // create primal module
         let mut primal_module = PrimalModuleSerialPtr::new_empty(&initializer);
-        primal_module.write().debug_resolve_only_one = true;  // to enable debug mode
-        // try to work on a simple syndrome
+        primal_module.write().debug_resolve_only_one = true; // to enable debug mode
+                                                             // try to work on a simple syndrome
         code.set_defect_vertices(&defect_vertices);
         let interface_ptr = DualModuleInterfacePtr::new_empty();
         primal_module.solve_visualizer(&interface_ptr, &code.get_syndrome(), &mut dual_module, Some(&mut visualizer));
         let fusion_mwpm = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         let fusion_mwpm_result = fusion_mwpm.legacy_get_mwpm_result(defect_vertices.clone());
         let fusion_details = detailed_matching(&initializer, &defect_vertices, &fusion_mwpm_result);
         let mut fusion_total_weight = 0;
         for detail in fusion_details.iter() {
             println!("    {detail:?}");
             fusion_total_weight += detail.weight;
         }
-        assert_eq!(fusion_total_weight, blossom_total_weight, "unexpected final dual variable sum");
-        {  // also test subgraph builder
+        assert_eq!(
+            fusion_total_weight, blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
+        {
+            // also test subgraph builder
             let mut subgraph_builder = SubGraphBuilder::new(&initializer);
             subgraph_builder.load_perfect_matching(&fusion_mwpm);
-            assert_eq!(subgraph_builder.total_weight(), blossom_total_weight, "unexpected final dual variable sum");
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), blossom_total_weight, "unexpected final dual variable sum");
+            assert_eq!(
+                subgraph_builder.total_weight(),
+                blossom_total_weight,
+                "unexpected final dual variable sum"
+            );
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
     }
 
     /// debug a case where it disagree with blossom V library, mine reports 16000, blossom V reports 17000
     #[test]
-    fn primal_module_debug_3() {  // cargo test primal_module_debug_3 -- --nocapture
+    fn primal_module_debug_3() {
+        // cargo test primal_module_debug_3 -- --nocapture
         let visualize_filename = format!("primal_module_debug_3.json");
-        let defect_vertices = vec![17, 34, 36, 54, 55, 74, 95, 96, 112, 113, 114, 115, 116, 130, 131, 132, 134, 150, 151, 154, 156, 171, 172, 173, 190];
+        let defect_vertices = vec![
+            17, 34, 36, 54, 55, 74, 95, 96, 112, 113, 114, 115, 116, 130, 131, 132, 134, 150, 151, 154, 156, 171, 172, 173,
+            190,
+        ];
         let max_half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(19, 0.499, max_half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         let initializer = code.get_initializer();
         // blossom V ground truth
         let blossom_mwpm_result = blossom_v_mwpm(&initializer, &defect_vertices);
         let blossom_details = detailed_matching(&initializer, &defect_vertices, &blossom_mwpm_result);
         let mut blossom_total_weight = 0;
         for detail in blossom_details.iter() {
             println!("    {detail:?}");
             blossom_total_weight += detail.weight;
         }
         // create dual module
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // create primal module
         let mut primal_module = PrimalModuleSerialPtr::new_empty(&initializer);
-        primal_module.write().debug_resolve_only_one = true;  // to enable debug mode
-        // try to work on a simple syndrome
+        primal_module.write().debug_resolve_only_one = true; // to enable debug mode
+                                                             // try to work on a simple syndrome
         code.set_defect_vertices(&defect_vertices);
         let interface_ptr = DualModuleInterfacePtr::new_empty();
         primal_module.solve_visualizer(&interface_ptr, &code.get_syndrome(), &mut dual_module, Some(&mut visualizer));
         let fusion_mwpm = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         let fusion_mwpm_result = fusion_mwpm.legacy_get_mwpm_result(defect_vertices.clone());
         let fusion_details = detailed_matching(&initializer, &defect_vertices, &fusion_mwpm_result);
         let mut fusion_total_weight = 0;
         for detail in fusion_details.iter() {
             println!("    {detail:?}");
             fusion_total_weight += detail.weight;
         }
-        assert_eq!(fusion_total_weight, blossom_total_weight, "unexpected final dual variable sum");
-        {  // also test subgraph builder
+        assert_eq!(
+            fusion_total_weight, blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
+        {
+            // also test subgraph builder
             let mut subgraph_builder = SubGraphBuilder::new(&initializer);
             subgraph_builder.load_perfect_matching(&fusion_mwpm);
-            assert_eq!(subgraph_builder.total_weight(), blossom_total_weight, "unexpected final dual variable sum");
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), blossom_total_weight, "unexpected final dual variable sum");
+            assert_eq!(
+                subgraph_builder.total_weight(),
+                blossom_total_weight,
+                "unexpected final dual variable sum"
+            );
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
     }
 
     /// debug a case where it disagree with blossom V library, mine reports 9000, blossom V reports 7000
     #[test]
-    fn primal_module_debug_4() {  // cargo test primal_module_debug_4 -- --nocapture
+    fn primal_module_debug_4() {
+        // cargo test primal_module_debug_4 -- --nocapture
         let visualize_filename = format!("primal_module_debug_4.json");
         let defect_vertices = vec![1, 3, 6, 8, 9, 11, 13];
         let max_half_weight = 500;
         let mut code = CodeCapacityRepetitionCode::new(15, 0.499, max_half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         let initializer = code.get_initializer();
         // blossom V ground truth
         let blossom_mwpm_result = blossom_v_mwpm(&initializer, &defect_vertices);
         let blossom_details = detailed_matching(&initializer, &defect_vertices, &blossom_mwpm_result);
         let mut blossom_total_weight = 0;
         for detail in blossom_details.iter() {
             println!("    {detail:?}");
             blossom_total_weight += detail.weight;
         }
         // create dual module
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         // create primal module
         let mut primal_module = PrimalModuleSerialPtr::new_empty(&initializer);
-        primal_module.write().debug_resolve_only_one = true;  // to enable debug mode
-        // try to work on a simple syndrome
+        primal_module.write().debug_resolve_only_one = true; // to enable debug mode
+                                                             // try to work on a simple syndrome
         code.set_defect_vertices(&defect_vertices);
         let interface_ptr = DualModuleInterfacePtr::new_empty();
         primal_module.solve_visualizer(&interface_ptr, &code.get_syndrome(), &mut dual_module, Some(&mut visualizer));
         let fusion_mwpm = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         let fusion_mwpm_result = fusion_mwpm.legacy_get_mwpm_result(defect_vertices.clone());
         let fusion_details = detailed_matching(&initializer, &defect_vertices, &fusion_mwpm_result);
         let mut fusion_total_weight = 0;
         for detail in fusion_details.iter() {
             println!("    {detail:?}");
             fusion_total_weight += detail.weight;
         }
-        assert_eq!(fusion_total_weight, blossom_total_weight, "unexpected final dual variable sum");
-        {  // also test subgraph builder
+        assert_eq!(
+            fusion_total_weight, blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
+        {
+            // also test subgraph builder
             let mut subgraph_builder = SubGraphBuilder::new(&initializer);
             subgraph_builder.load_perfect_matching(&fusion_mwpm);
-            assert_eq!(subgraph_builder.total_weight(), blossom_total_weight, "unexpected final dual variable sum");
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), blossom_total_weight, "unexpected final dual variable sum");
+            assert_eq!(
+                subgraph_builder.total_weight(),
+                blossom_total_weight,
+                "unexpected final dual variable sum"
+            );
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
     }
 
     /// debug a case of being stuck after disable the flag `debug_resolve_only_one` for faster speed
     #[test]
-    fn primal_module_debug_5() {  // cargo test primal_module_debug_5 -- --nocapture
+    fn primal_module_debug_5() {
+        // cargo test primal_module_debug_5 -- --nocapture
         let visualize_filename = format!("primal_module_debug_5.json");
         let defect_vertices = vec![0, 1, 3, 8, 9];
         let max_half_weight = 500;
         let mut code = CodeCapacityRepetitionCode::new(11, 0.03, max_half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         let initializer = code.get_initializer();
         // blossom V ground truth
         let blossom_mwpm_result = blossom_v_mwpm(&initializer, &defect_vertices);
         let blossom_details = detailed_matching(&initializer, &defect_vertices, &blossom_mwpm_result);
         let mut blossom_total_weight = 0;
         for detail in blossom_details.iter() {
@@ -1621,43 +2307,63 @@
         let fusion_mwpm_result = fusion_mwpm.legacy_get_mwpm_result(defect_vertices.clone());
         let fusion_details = detailed_matching(&initializer, &defect_vertices, &fusion_mwpm_result);
         let mut fusion_total_weight = 0;
         for detail in fusion_details.iter() {
             println!("    {detail:?}");
             fusion_total_weight += detail.weight;
         }
-        assert_eq!(fusion_total_weight, blossom_total_weight, "unexpected final dual variable sum");
-        {  // also test subgraph builder
+        assert_eq!(
+            fusion_total_weight, blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
+        {
+            // also test subgraph builder
             let mut subgraph_builder = SubGraphBuilder::new(&initializer);
             subgraph_builder.load_perfect_matching(&fusion_mwpm);
-            assert_eq!(subgraph_builder.total_weight(), blossom_total_weight, "unexpected final dual variable sum");
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), blossom_total_weight, "unexpected final dual variable sum");
+            assert_eq!(
+                subgraph_builder.total_weight(),
+                blossom_total_weight,
+                "unexpected final dual variable sum"
+            );
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
     }
 
     #[test]
-    fn primal_module_serial_perfect_matching_1() {  // cargo test primal_module_serial_perfect_matching_1 -- --nocapture
+    fn primal_module_serial_perfect_matching_1() {
+        // cargo test primal_module_serial_perfect_matching_1 -- --nocapture
         let defect_vertices = vec![39, 51, 61, 62, 63, 64, 65, 75, 87, 67];
-        let (interface_ptr, mut primal_module, mut dual_module) = primal_module_serial_basic_standard_syndrome_optional_viz(11, None, defect_vertices, 6);
+        let (interface_ptr, mut primal_module, mut dual_module) =
+            primal_module_serial_basic_standard_syndrome_optional_viz(11, None, defect_vertices, 6);
         let intermediate_matching = primal_module.intermediate_matching(&interface_ptr, &mut dual_module);
         println!("intermediate_matching: {intermediate_matching:?}");
         let perfect_matching = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         println!("perfect_matching: {perfect_matching:?}");
     }
 
     /// debug a case of non-zero weight given pure erasure
     #[test]
-    fn primal_module_debug_6() {  // cargo test primal_module_debug_6 -- --nocapture
+    fn primal_module_debug_6() {
+        // cargo test primal_module_debug_6 -- --nocapture
         let visualize_filename = format!("primal_module_debug_6.json");
         let defect_vertices = vec![13, 34, 87, 107, 276, 296];
         let erasures = vec![13, 33, 174, 516];
         let max_half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(19, 0., max_half_weight);
         code.set_erasure_probability(0.003);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         let mut initializer = code.get_initializer();
         for edge_index in erasures.iter() {
             let (vertex_idx_1, vertex_idx_2, _) = &initializer.weighted_edges[*edge_index];
             initializer.weighted_edges[*edge_index] = (*vertex_idx_1, *vertex_idx_2, 0);
         }
         // blossom V ground truth
@@ -1680,17 +2386,28 @@
         let fusion_mwpm_result = fusion_mwpm.legacy_get_mwpm_result(defect_vertices.clone());
         let fusion_details = detailed_matching(&initializer, &defect_vertices, &fusion_mwpm_result);
         let mut fusion_total_weight = 0;
         for detail in fusion_details.iter() {
             println!("    {detail:?}");
             fusion_total_weight += detail.weight;
         }
-        assert_eq!(fusion_total_weight, blossom_total_weight, "unexpected final dual variable sum");
-        {  // also test subgraph builder
+        assert_eq!(
+            fusion_total_weight, blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
+        {
+            // also test subgraph builder
             let mut subgraph_builder = SubGraphBuilder::new(&initializer);
             subgraph_builder.load_perfect_matching(&fusion_mwpm);
-            assert_eq!(subgraph_builder.total_weight(), blossom_total_weight, "unexpected final dual variable sum");
-        }
-        assert_eq!(interface_ptr.sum_dual_variables(), blossom_total_weight, "unexpected final dual variable sum");
+            assert_eq!(
+                subgraph_builder.total_weight(),
+                blossom_total_weight,
+                "unexpected final dual variable sum"
+            );
+        }
+        assert_eq!(
+            interface_ptr.sum_dual_variables(),
+            blossom_total_weight,
+            "unexpected final dual variable sum"
+        );
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/src/util.rs` & `fusion_blossom-0.2.5/src/util.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+use super::mwpm_solver::PrimalDualSolver;
+use super::pointers::*;
 use super::rand_xoshiro;
 use crate::rand_xoshiro::rand_core::RngCore;
-use serde::{Serialize, Deserialize};
+#[cfg(feature = "python_binding")]
+use pyo3::prelude::*;
+use serde::{Deserialize, Serialize};
 use std::collections::BTreeSet;
-use std::time::Instant;
 use std::fs::File;
 use std::io::prelude::*;
-use super::mwpm_solver::PrimalDualSolver;
-use super::pointers::*;
-#[cfg(feature="python_binding")]
-use pyo3::prelude::*;
-
+use std::time::Instant;
 
 cfg_if::cfg_if! {
     if #[cfg(feature="i32_weight")] {
         /// use i32 to store weight to be compatible with blossom V library (c_int)
         pub type Weight = i32;
     } else {
         pub type Weight = i64;
@@ -22,24 +21,24 @@
 
 cfg_if::cfg_if! {
     if #[cfg(feature="u32_index")] {
         // use u32 to store index, for less memory usage
         pub type EdgeIndex = u32;
         pub type VertexIndex = u32;  // the vertex index in the decoding graph
         pub type NodeIndex = VertexIndex;
-        pub type SyndromeIndex = VertexIndex;
-        pub type VertexNodeIndex = VertexIndex;  // must be same as VertexIndex, NodeIndex, SyndromeIndex
+        pub type DefectIndex = VertexIndex;
+        pub type VertexNodeIndex = VertexIndex;  // must be same as VertexIndex, NodeIndex, DefectIndex
         pub type VertexNum = VertexIndex;
         pub type NodeNum = VertexIndex;
     } else {
         pub type EdgeIndex = usize;
         pub type VertexIndex = usize;
         pub type NodeIndex = VertexIndex;
-        pub type SyndromeIndex = VertexIndex;
-        pub type VertexNodeIndex = VertexIndex;  // must be same as VertexIndex, NodeIndex, SyndromeIndex
+        pub type DefectIndex = VertexIndex;
+        pub type VertexNodeIndex = VertexIndex;  // must be same as VertexIndex, NodeIndex, DefectIndex
         pub type VertexNum = VertexIndex;
         pub type NodeNum = VertexIndex;
     }
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
@@ -59,100 +58,136 @@
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct SyndromePattern {
     /// the vertices corresponding to defect measurements
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub defect_vertices: Vec<VertexIndex>,
-    /// the edges that experience erasures, i.e. known errors
+    /// the edges that experience erasures, i.e. known errors;
+    /// note that erasure decoding can also be implemented using `dynamic_weights`,
+    /// but for user convenience we keep this interface
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub erasures: Vec<EdgeIndex>,
+    /// general dynamically weighted edges
+    #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    pub dynamic_weights: Vec<(EdgeIndex, Weight)>,
 }
 
 impl SyndromePattern {
     pub fn new(defect_vertices: Vec<VertexIndex>, erasures: Vec<EdgeIndex>) -> Self {
-        Self { defect_vertices, erasures }
+        Self {
+            defect_vertices,
+            erasures,
+            dynamic_weights: vec![],
+        }
+    }
+    pub fn new_dynamic_weights(
+        defect_vertices: Vec<VertexIndex>,
+        erasures: Vec<EdgeIndex>,
+        dynamic_weights: Vec<(EdgeIndex, Weight)>,
+    ) -> Self {
+        Self {
+            defect_vertices,
+            erasures,
+            dynamic_weights,
+        }
     }
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl SyndromePattern {
     #[cfg_attr(feature = "python_binding", new)]
-    #[cfg_attr(feature = "python_binding", args(defect_vertices="vec![]", erasures="vec![]"))]
-    pub fn py_new(mut defect_vertices: Vec<VertexIndex>, erasures: Vec<EdgeIndex>, syndrome_vertices: Option<Vec<VertexIndex>>) -> Self {
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (defect_vertices=vec![], erasures=vec![], dynamic_weights=vec![], syndrome_vertices=None)))]
+    pub fn py_new(
+        mut defect_vertices: Vec<VertexIndex>,
+        erasures: Vec<EdgeIndex>,
+        dynamic_weights: Vec<(EdgeIndex, Weight)>,
+        syndrome_vertices: Option<Vec<VertexIndex>>,
+    ) -> Self {
         if let Some(syndrome_vertices) = syndrome_vertices {
-            assert!(defect_vertices.is_empty(), "do not pass both `syndrome_vertices` and `defect_vertices` since they're aliasing");
+            assert!(
+                defect_vertices.is_empty(),
+                "do not pass both `syndrome_vertices` and `defect_vertices` since they're aliasing"
+            );
             defect_vertices = syndrome_vertices;
         }
-        Self { defect_vertices, erasures }
+        assert!(
+            erasures.is_empty() || dynamic_weights.is_empty(),
+            "erasures and dynamic_weights cannot be provided at the same time"
+        );
+        Self::new_dynamic_weights(defect_vertices, erasures, dynamic_weights)
     }
     #[cfg_attr(feature = "python_binding", staticmethod)]
     pub fn new_vertices(defect_vertices: Vec<VertexIndex>) -> Self {
         Self::new(defect_vertices, vec![])
     }
     #[cfg_attr(feature = "python_binding", staticmethod)]
     pub fn new_empty() -> Self {
         Self::new(vec![], vec![])
     }
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 /// an efficient representation of partitioned vertices and erasures when they're ordered
 #[derive(Debug, Clone, Serialize)]
 pub struct PartitionedSyndromePattern<'a> {
     /// the original syndrome pattern to be partitioned
     pub syndrome_pattern: &'a SyndromePattern,
     /// the defect range of this partition: it must be continuous if the defect vertices are ordered
-    pub whole_defect_range: SyndromeRange,
+    pub whole_defect_range: DefectRange,
 }
 
 impl<'a> PartitionedSyndromePattern<'a> {
-
     pub fn new(syndrome_pattern: &'a SyndromePattern) -> Self {
-        assert!(syndrome_pattern.erasures.is_empty(), "erasure partition not supported yet;
+        assert!(
+            syndrome_pattern.erasures.is_empty(),
+            "erasure partition not supported yet;
         even if the edges in the erasure is well ordered, they may not be able to be represented as
-        a single range simply because the partition is vertex-based. need more consideration");
+        a single range simply because the partition is vertex-based. need more consideration"
+        );
         Self {
             syndrome_pattern,
-            whole_defect_range: SyndromeRange::new(0, syndrome_pattern.defect_vertices.len() as SyndromeIndex),
+            whole_defect_range: DefectRange::new(0, syndrome_pattern.defect_vertices.len() as DefectIndex),
         }
     }
-
 }
 
 #[derive(Debug, Clone, Copy, Serialize, Deserialize, PartialEq, Eq)]
 #[serde(transparent)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct IndexRange {
     pub range: [VertexNodeIndex; 2],
 }
 
 // just to distinguish them in code, essentially nothing different
 pub type VertexRange = IndexRange;
 pub type NodeRange = IndexRange;
-pub type SyndromeRange = IndexRange;
+pub type DefectRange = IndexRange;
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl IndexRange {
     #[cfg_attr(feature = "python_binding", new)]
     pub fn new(start: VertexNodeIndex, end: VertexNodeIndex) -> Self {
         debug_assert!(end >= start, "invalid range [{}, {})", start, end);
-        Self { range: [start, end], }
+        Self { range: [start, end] }
     }
     #[cfg_attr(feature = "python_binding", staticmethod)]
     pub fn new_length(start: VertexNodeIndex, length: VertexNodeIndex) -> Self {
         Self::new(start, start + length)
     }
     pub fn is_empty(&self) -> bool {
         self.range[1] == self.range[0]
     }
+    #[allow(clippy::unnecessary_cast)]
     pub fn len(&self) -> usize {
         (self.range[1] - self.range[0]) as usize
     }
     pub fn start(&self) -> VertexNodeIndex {
         self.range[0]
     }
     pub fn end(&self) -> VertexNodeIndex {
@@ -172,33 +207,38 @@
         vertex_index >= self.start() && vertex_index < self.end()
     }
     /// fuse two ranges together, returning (the whole range, the interfacing range)
     pub fn fuse(&self, other: &Self) -> (Self, Self) {
         self.sanity_check();
         other.sanity_check();
         assert!(self.range[1] <= other.range[0], "only lower range can fuse higher range");
-        (Self::new(self.range[0], other.range[1]), Self::new(self.range[1], other.range[0]))
+        (
+            Self::new(self.range[0], other.range[1]),
+            Self::new(self.range[1], other.range[0]),
+        )
     }
     #[cfg(feature = "python_binding")]
     #[pyo3(name = "contains_any")]
     pub fn python_contains_any(&self, vertex_indices: Vec<VertexNodeIndex>) -> bool {
         self.contains_any(&vertex_indices)
     }
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 impl IndexRange {
     pub fn iter(&self) -> std::ops::Range<VertexNodeIndex> {
-        self.range[0].. self.range[1]
+        self.range[0]..self.range[1]
     }
     pub fn contains_any(&self, vertex_indices: &[VertexNodeIndex]) -> bool {
         for vertex_index in vertex_indices.iter() {
             if self.contains(*vertex_index) {
-                return true
+                return true;
             }
         }
         false
     }
 }
 
 /// a general partition unit that could contain mirrored vertices
@@ -212,15 +252,20 @@
 
 pub type PartitionUnitPtr = ArcManualSafeLock<PartitionUnit>;
 pub type PartitionUnitWeak = WeakManualSafeLock<PartitionUnit>;
 
 impl std::fmt::Debug for PartitionUnitPtr {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         let partition_unit = self.read_recursive();
-        write!(f, "{}{}", if partition_unit.enabled { "E" } else { "D" }, partition_unit.unit_index)
+        write!(
+            f,
+            "{}{}",
+            if partition_unit.enabled { "E" } else { "D" },
+            partition_unit.unit_index
+        )
     }
 }
 
 impl std::fmt::Debug for PartitionUnitWeak {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         self.upgrade_force().fmt(f)
     }
@@ -242,43 +287,59 @@
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub fusions: Vec<(usize, usize)>,
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl PartitionConfig {
-
     #[cfg_attr(feature = "python_binding", new)]
     pub fn new(vertex_num: VertexNum) -> Self {
         Self {
             vertex_num,
             partitions: vec![VertexRange::new(0, vertex_num as VertexIndex)],
             fusions: vec![],
         }
     }
 
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 
+    #[allow(clippy::unnecessary_cast)]
     pub fn info(&self) -> PartitionInfo {
         assert!(!self.partitions.is_empty(), "at least one partition must exist");
         let mut whole_ranges = vec![];
         let mut owning_ranges = vec![];
         for &partition in self.partitions.iter() {
             partition.sanity_check();
-            assert!(partition.end() <= self.vertex_num as VertexIndex, "invalid vertex index {} in partitions", partition.end());
+            assert!(
+                partition.end() <= self.vertex_num as VertexIndex,
+                "invalid vertex index {} in partitions",
+                partition.end()
+            );
             whole_ranges.push(partition);
             owning_ranges.push(partition);
         }
         let unit_count = self.partitions.len() + self.fusions.len();
         let mut parents: Vec<Option<usize>> = (0..unit_count).map(|_| None).collect();
         for (fusion_index, (left_index, right_index)) in self.fusions.iter().enumerate() {
             let unit_index = fusion_index + self.partitions.len();
-            assert!(*left_index < unit_index, "dependency wrong, {} depending on {}", unit_index, left_index);
-            assert!(*right_index < unit_index, "dependency wrong, {} depending on {}", unit_index, right_index);
+            assert!(
+                *left_index < unit_index,
+                "dependency wrong, {} depending on {}",
+                unit_index,
+                left_index
+            );
+            assert!(
+                *right_index < unit_index,
+                "dependency wrong, {} depending on {}",
+                unit_index,
+                right_index
+            );
             assert!(parents[*left_index].is_none(), "cannot fuse {} twice", left_index);
             assert!(parents[*right_index].is_none(), "cannot fuse {} twice", right_index);
             parents[*left_index] = Some(unit_index);
             parents[*right_index] = Some(unit_index);
             // fusing range
             let (whole_range, interface_range) = whole_ranges[*left_index].fuse(&whole_ranges[*right_index]);
             whole_ranges.push(whole_range);
@@ -286,28 +347,39 @@
         }
         // check that all nodes except for the last one has been merged
         for (unit_index, parent) in parents.iter().enumerate().take(unit_count - 1) {
             assert!(parent.is_some(), "found unit {} without being fused", unit_index);
         }
         // check that the final node has the full range
         let last_unit_index = self.partitions.len() + self.fusions.len() - 1;
-        assert!(whole_ranges[last_unit_index].start() == 0, "final range not covering all vertices {:?}", whole_ranges[last_unit_index]);
-        assert!(whole_ranges[last_unit_index].end() == self.vertex_num as VertexIndex
-            , "final range not covering all vertices {:?}", whole_ranges[last_unit_index]);
+        assert!(
+            whole_ranges[last_unit_index].start() == 0,
+            "final range not covering all vertices {:?}",
+            whole_ranges[last_unit_index]
+        );
+        assert!(
+            whole_ranges[last_unit_index].end() == self.vertex_num as VertexIndex,
+            "final range not covering all vertices {:?}",
+            whole_ranges[last_unit_index]
+        );
         // construct partition info
-        let mut partition_unit_info: Vec<_> = (0..self.partitions.len() + self.fusions.len()).map(|i| {
-            PartitionUnitInfo {
+        let mut partition_unit_info: Vec<_> = (0..self.partitions.len() + self.fusions.len())
+            .map(|i| PartitionUnitInfo {
                 whole_range: whole_ranges[i],
                 owning_range: owning_ranges[i],
-                children: if i >= self.partitions.len() { Some(self.fusions[i - self.partitions.len()]) } else { None },
+                children: if i >= self.partitions.len() {
+                    Some(self.fusions[i - self.partitions.len()])
+                } else {
+                    None
+                },
                 parent: parents[i],
                 leaves: if i < self.partitions.len() { vec![i] } else { vec![] },
                 descendants: BTreeSet::new(),
-            }
-        }).collect();
+            })
+            .collect();
         // build descendants
         for (fusion_index, (left_index, right_index)) in self.fusions.iter().enumerate() {
             let unit_index = fusion_index + self.partitions.len();
             let mut leaves = vec![];
             leaves.extend(partition_unit_info[*left_index].leaves.iter());
             leaves.extend(partition_unit_info[*right_index].leaves.iter());
             partition_unit_info[unit_index].leaves.extend(leaves.iter());
@@ -326,15 +398,14 @@
         }
         PartitionInfo {
             config: self.clone(),
             units: partition_unit_info,
             vertex_to_owning_unit,
         }
     }
-
 }
 
 #[derive(Debug, Clone)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct PartitionInfo {
     /// the initial configuration that creates this info
@@ -347,35 +418,36 @@
     /// used for loading syndrome to the holding units
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub vertex_to_owning_unit: Vec<usize>,
 }
 
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl PartitionInfo {
-
     /// split a sequence of syndrome into multiple parts, each corresponds to a unit;
     /// this is a slow method and should only be used when the syndrome pattern is not well-ordered
+    #[allow(clippy::unnecessary_cast)]
     pub fn partition_syndrome_unordered(&self, syndrome_pattern: &SyndromePattern) -> Vec<SyndromePattern> {
         let mut partitioned_syndrome: Vec<_> = (0..self.units.len()).map(|_| SyndromePattern::new_empty()).collect();
         for defect_vertex in syndrome_pattern.defect_vertices.iter() {
             let unit_index = self.vertex_to_owning_unit[*defect_vertex as usize];
             partitioned_syndrome[unit_index].defect_vertices.push(*defect_vertex);
         }
         // TODO: partition edges
         partitioned_syndrome
     }
 
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
-
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 impl<'a> PartitionedSyndromePattern<'a> {
-
     /// partition the syndrome pattern into 2 partitioned syndrome pattern and my whole range
+    #[allow(clippy::unnecessary_cast)]
     pub fn partition(&self, partition_unit_info: &PartitionUnitInfo) -> (Self, (Self, Self)) {
         // first binary search the start of owning defect vertices
         let owning_start_index = {
             let mut left_index = self.whole_defect_range.start();
             let mut right_index = self.whole_defect_range.end();
             while left_index != right_index {
                 let mid_index = (left_index + right_index) / 2;
@@ -399,34 +471,40 @@
                     left_index = mid_index + 1;
                 } else {
                     right_index = mid_index;
                 }
             }
             left_index
         };
-        (Self {
-            syndrome_pattern: self.syndrome_pattern,
-            whole_defect_range: SyndromeRange::new(owning_start_index, owning_end_index),
-        }, (Self {
-            syndrome_pattern: self.syndrome_pattern,
-            whole_defect_range: SyndromeRange::new(self.whole_defect_range.start(), owning_start_index),
-        }, Self {
-            syndrome_pattern: self.syndrome_pattern,
-            whole_defect_range: SyndromeRange::new(owning_end_index, self.whole_defect_range.end()),
-        }))
+        (
+            Self {
+                syndrome_pattern: self.syndrome_pattern,
+                whole_defect_range: DefectRange::new(owning_start_index, owning_end_index),
+            },
+            (
+                Self {
+                    syndrome_pattern: self.syndrome_pattern,
+                    whole_defect_range: DefectRange::new(self.whole_defect_range.start(), owning_start_index),
+                },
+                Self {
+                    syndrome_pattern: self.syndrome_pattern,
+                    whole_defect_range: DefectRange::new(owning_end_index, self.whole_defect_range.end()),
+                },
+            ),
+        )
     }
 
+    #[allow(clippy::unnecessary_cast)]
     pub fn expand(&self) -> SyndromePattern {
         let mut defect_vertices = Vec::with_capacity(self.whole_defect_range.len());
         for defect_index in self.whole_defect_range.iter() {
             defect_vertices.push(self.syndrome_pattern.defect_vertices[defect_index as usize]);
         }
         SyndromePattern::new(defect_vertices, vec![])
     }
-
 }
 
 #[derive(Debug, Clone)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct PartitionUnitInfo {
     /// the whole range of units
@@ -448,15 +526,17 @@
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub descendants: BTreeSet<usize>,
 }
 
 #[cfg(feature = "python_binding")]
 #[pymethods]
 impl PartitionUnitInfo {
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 #[derive(Debug, Clone)]
 pub struct PartitionedSolverInitializer {
     /// unit index
     pub unit_index: usize,
     /// the number of all vertices (including those partitioned into other serial modules)
@@ -467,58 +547,69 @@
     pub owning_range: VertexRange,
     /// applicable when all the owning vertices are partitioned (i.e. this belongs to a fusion unit)
     pub owning_interface: Option<PartitionUnitWeak>,
     /// if applicable, parent interface comes first, then the grandparent interface, ... note that some ancestor might be skipped because it has no mirrored vertices;
     /// we skip them because if the partition is in a chain, most of them would only have to know two interfaces on the left and on the right; nothing else necessary.
     /// (unit_index, list of vertices owned by this ancestor unit and should be mirrored at this partition and whether it's virtual)
     pub interfaces: Vec<(PartitionUnitWeak, Vec<(VertexIndex, bool)>)>,
-    /// weighted edges, where the first vertex index is within the range [vertex_index_bias, vertex_index_bias + vertex_num) and 
-    /// the second is either in [vertex_index_bias, vertex_index_bias + vertex_num) or inside 
+    /// weighted edges, where the first vertex index is within the range [vertex_index_bias, vertex_index_bias + vertex_num) and
+    /// the second is either in [vertex_index_bias, vertex_index_bias + vertex_num) or inside
     pub weighted_edges: Vec<(VertexIndex, VertexIndex, Weight, EdgeIndex)>,
     /// the virtual vertices
     pub virtual_vertices: Vec<VertexIndex>,
 }
 
 /// perform index transformation
+#[allow(clippy::unnecessary_cast)]
 pub fn build_old_to_new(reordered_vertices: &Vec<VertexIndex>) -> Vec<Option<VertexIndex>> {
     let mut old_to_new: Vec<Option<VertexIndex>> = (0..reordered_vertices.len()).map(|_| None).collect();
     for (new_index, old_index) in reordered_vertices.iter().enumerate() {
         assert_eq!(old_to_new[*old_index as usize], None, "duplicate vertex found {}", old_index);
         old_to_new[*old_index as usize] = Some(new_index as VertexIndex);
     }
     old_to_new
 }
 
 /// translate defect vertices into the current new index given reordered_vertices
-pub fn translated_defect_to_reordered(reordered_vertices: &Vec<VertexIndex>, old_defect_vertices: &[VertexIndex]) -> Vec<VertexIndex> {
+#[allow(clippy::unnecessary_cast)]
+pub fn translated_defect_to_reordered(
+    reordered_vertices: &Vec<VertexIndex>,
+    old_defect_vertices: &[VertexIndex],
+) -> Vec<VertexIndex> {
     let old_to_new = build_old_to_new(reordered_vertices);
-    old_defect_vertices.iter().map(|old_index| {
-        old_to_new[*old_index as usize].unwrap()
-    }).collect()
+    old_defect_vertices
+        .iter()
+        .map(|old_index| old_to_new[*old_index as usize].unwrap())
+        .collect()
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl SolverInitializer {
     #[cfg_attr(feature = "python_binding", new)]
-    pub fn new(vertex_num: VertexNum, weighted_edges: Vec<(VertexIndex, VertexIndex, Weight)>, virtual_vertices: Vec<VertexIndex>) -> SolverInitializer {
+    pub fn new(
+        vertex_num: VertexNum,
+        weighted_edges: Vec<(VertexIndex, VertexIndex, Weight)>,
+        virtual_vertices: Vec<VertexIndex>,
+    ) -> SolverInitializer {
         SolverInitializer {
             vertex_num,
             weighted_edges,
             virtual_vertices,
         }
     }
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 /// timestamp type determines how many fast clear before a hard clear is required, see [`FastClear`]
 pub type FastClearTimestamp = usize;
 
-
 #[allow(dead_code)]
 /// use Xoshiro256StarStar for deterministic random number generator
 pub type DeterministicRng = rand_xoshiro::Xoshiro256StarStar;
 
 pub trait F64Rng {
     fn next_f64(&mut self) -> f64;
 }
@@ -543,19 +634,25 @@
     pub benchmark_profiler_output: Option<File>,
 }
 
 impl BenchmarkProfiler {
     pub fn new(noisy_measurements: VertexNum, detail_log_file: Option<(String, &PartitionInfo)>) -> Self {
         let benchmark_profiler_output = detail_log_file.map(|(filename, partition_info)| {
             let mut file = File::create(filename).unwrap();
-            file.write_all(serde_json::to_string(&partition_info.config).unwrap().as_bytes()).unwrap();
+            file.write_all(serde_json::to_string(&partition_info.config).unwrap().as_bytes())
+                .unwrap();
             file.write_all(b"\n").unwrap();
-            file.write_all(serde_json::to_string(&json!({
-                "noisy_measurements": noisy_measurements,
-            })).unwrap().as_bytes()).unwrap();
+            file.write_all(
+                serde_json::to_string(&json!({
+                    "noisy_measurements": noisy_measurements,
+                }))
+                .unwrap()
+                .as_bytes(),
+            )
+            .unwrap();
             file.write_all(b"\n").unwrap();
             file
         });
         Self {
             records: vec![],
             sum_round_time: 0.,
             sum_syndrome: 0,
@@ -563,27 +660,36 @@
             benchmark_profiler_output,
         }
     }
     /// record the beginning of a decoding procedure
     pub fn begin(&mut self, syndrome_pattern: &SyndromePattern) {
         // sanity check last entry, if exists, is complete
         if let Some(last_entry) = self.records.last() {
-            assert!(last_entry.is_complete(), "the last benchmark profiler entry is not complete, make sure to call `begin` and `end` in pairs");
+            assert!(
+                last_entry.is_complete(),
+                "the last benchmark profiler entry is not complete, make sure to call `begin` and `end` in pairs"
+            );
         }
         let entry = BenchmarkProfilerEntry::new(syndrome_pattern);
         self.records.push(entry);
         self.records.last_mut().unwrap().record_begin();
     }
     pub fn event(&mut self, event_name: String) {
-        let last_entry = self.records.last_mut().expect("last entry not exists, call `begin` before `end`");
+        let last_entry = self
+            .records
+            .last_mut()
+            .expect("last entry not exists, call `begin` before `end`");
         last_entry.record_event(event_name);
     }
     /// record the ending of a decoding procedure
     pub fn end(&mut self, solver: Option<&dyn PrimalDualSolver>) {
-        let last_entry = self.records.last_mut().expect("last entry not exists, call `begin` before `end`");
+        let last_entry = self
+            .records
+            .last_mut()
+            .expect("last entry not exists, call `begin` before `end`");
         last_entry.record_end();
         self.sum_round_time += last_entry.round_time.unwrap();
         self.sum_syndrome += last_entry.syndrome_pattern.defect_vertices.len();
         if let Some(file) = self.benchmark_profiler_output.as_mut() {
             let mut events = serde_json::Map::new();
             for (event_name, time) in last_entry.events.iter() {
                 events.insert(event_name.clone(), json!(time));
@@ -591,26 +697,29 @@
             let mut value = json!({
                 "round_time": last_entry.round_time.unwrap(),
                 "defect_num": last_entry.syndrome_pattern.defect_vertices.len(),
                 "events": events,
             });
             if let Some(solver) = solver {
                 let solver_profile = solver.generate_profiler_report();
-                value.as_object_mut().unwrap().insert("solver_profile".to_string(), solver_profile);
+                value
+                    .as_object_mut()
+                    .unwrap()
+                    .insert("solver_profile".to_string(), solver_profile);
             }
             file.write_all(serde_json::to_string(&value).unwrap().as_bytes()).unwrap();
             file.write_all(b"\n").unwrap();
         }
     }
     /// print out a brief one-line statistics
     pub fn brief(&self) -> String {
         let total = self.sum_round_time / (self.records.len() as f64);
         let per_round = total / (1. + self.noisy_measurements as f64);
         let per_defect = self.sum_round_time / (self.sum_syndrome as f64);
-        format!("total: {total:.3e}, round: {per_round:.3e}, syndrome: {per_defect:.3e},")
+        format!("total: {total:.3e}, round: {per_round:.3e}, defect: {per_defect:.3e},")
     }
 }
 
 pub struct BenchmarkProfilerEntry {
     /// the syndrome pattern of this decoding problem
     pub syndrome_pattern: SyndromePattern,
     /// the time of beginning a decoding procedure
@@ -633,51 +742,57 @@
     /// record the beginning of a decoding procedure
     pub fn record_begin(&mut self) {
         assert_eq!(self.begin_time, None, "do not call `record_begin` twice on the same entry");
         self.begin_time = Some(Instant::now());
     }
     /// record the ending of a decoding procedure
     pub fn record_end(&mut self) {
-        let begin_time = self.begin_time.as_ref().expect("make sure to call `record_begin` before calling `record_end`");
+        let begin_time = self
+            .begin_time
+            .as_ref()
+            .expect("make sure to call `record_begin` before calling `record_end`");
         self.round_time = Some(begin_time.elapsed().as_secs_f64());
     }
     pub fn record_event(&mut self, event_name: String) {
-        let begin_time = self.begin_time.as_ref().expect("make sure to call `record_begin` before calling `record_end`");
+        let begin_time = self
+            .begin_time
+            .as_ref()
+            .expect("make sure to call `record_begin` before calling `record_end`");
         self.events.push((event_name, begin_time.elapsed().as_secs_f64()));
     }
     pub fn is_complete(&self) -> bool {
         self.round_time.is_some()
     }
 }
 
 /**
  * If you want to modify a field of a Rust struct, it will return a copy of it to avoid memory unsafety.
  * Thus, typical way of modifying a python field doesn't work, e.g. `obj.a.b.c = 1` won't actually modify `obj`.
  * This helper class is used to modify a field easier; but please note this can be very time consuming if not optimized well.
- * 
+ *
  * Example:
  * with PyMut(code, "vertices") as vertices:
  *     with fb.PyMut(vertices[0], "position") as position:
  *         position.i = 100
 */
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 #[pyclass]
 pub struct PyMut {
     /// the python object that provides getter and setter function for the attribute
     #[pyo3(get, set)]
     object: PyObject,
     /// the name of the attribute
     #[pyo3(get, set)]
     attr_name: String,
     /// the python attribute object that is taken from `object[attr_name]`
     #[pyo3(get, set)]
     attr_object: Option<PyObject>,
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 #[pymethods]
 impl PyMut {
     #[new]
     pub fn new(object: PyObject, attr_name: String) -> Self {
         Self {
             object,
             attr_name,
@@ -690,132 +805,142 @@
             let attr_object = self.object.getattr(py, self.attr_name.as_str()).unwrap();
             self.attr_object = Some(attr_object.clone_ref(py));
             attr_object
         })
     }
     pub fn __exit__(&mut self, _exc_type: PyObject, _exc_val: PyObject, _exc_tb: PyObject) {
         Python::with_gil(|py| {
-            self.object.setattr(py, self.attr_name.as_str(), self.attr_object.take().unwrap()).unwrap()
+            self.object
+                .setattr(py, self.attr_name.as_str(), self.attr_object.take().unwrap())
+                .unwrap()
         })
     }
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 pub fn json_to_pyobject_locked<'py>(value: serde_json::Value, py: Python<'py>) -> PyObject {
     match value {
         serde_json::Value::Null => py.None(),
         serde_json::Value::Bool(value) => value.to_object(py).into(),
         serde_json::Value::Number(value) => {
             if value.is_i64() {
                 value.as_i64().to_object(py).into()
             } else {
                 value.as_f64().to_object(py).into()
             }
-        },
+        }
         serde_json::Value::String(value) => value.to_object(py).into(),
         serde_json::Value::Array(array) => {
             let elements: Vec<PyObject> = array.into_iter().map(|value| json_to_pyobject_locked(value, py)).collect();
             pyo3::types::PyList::new(py, elements).into()
-        },
+        }
         serde_json::Value::Object(map) => {
             let pydict = pyo3::types::PyDict::new(py);
             for (key, value) in map.into_iter() {
                 let pyobject = json_to_pyobject_locked(value, py);
                 pydict.set_item(key, pyobject).unwrap();
             }
             pydict.into()
-        },
+        }
     }
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 pub fn json_to_pyobject(value: serde_json::Value) -> PyObject {
-    Python::with_gil(|py| {
-        json_to_pyobject_locked(value, py)
-    })
+    Python::with_gil(|py| json_to_pyobject_locked(value, py))
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 pub fn pyobject_to_json_locked<'py>(value: PyObject, py: Python<'py>) -> serde_json::Value {
     let value: &PyAny = value.as_ref(py);
     if value.is_none() {
         serde_json::Value::Null
     } else if value.is_instance_of::<pyo3::types::PyBool>().unwrap() {
         json!(value.extract::<bool>().unwrap())
     } else if value.is_instance_of::<pyo3::types::PyInt>().unwrap() {
         json!(value.extract::<i64>().unwrap())
     } else if value.is_instance_of::<pyo3::types::PyFloat>().unwrap() {
         json!(value.extract::<f64>().unwrap())
     } else if value.is_instance_of::<pyo3::types::PyString>().unwrap() {
         json!(value.extract::<String>().unwrap())
     } else if value.is_instance_of::<pyo3::types::PyList>().unwrap() {
-        let elements: Vec<serde_json::Value> = value.extract::<Vec<PyObject>>().unwrap()
-            .into_iter().map(|object| pyobject_to_json_locked(object, py)).collect();
+        let elements: Vec<serde_json::Value> = value
+            .extract::<Vec<PyObject>>()
+            .unwrap()
+            .into_iter()
+            .map(|object| pyobject_to_json_locked(object, py))
+            .collect();
         json!(elements)
     } else if value.is_instance_of::<pyo3::types::PyDict>().unwrap() {
-        let map: &pyo3::types::PyDict = value.cast_as().unwrap();
+        let map: &pyo3::types::PyDict = value.downcast().unwrap();
         let mut json_map = serde_json::Map::new();
         for (key, value) in map.iter() {
-            json_map.insert(key.extract::<String>().unwrap(), pyobject_to_json_locked(value.to_object(py), py));
+            json_map.insert(
+                key.extract::<String>().unwrap(),
+                pyobject_to_json_locked(value.to_object(py), py),
+            );
         }
         serde_json::Value::Object(json_map)
     } else {
         unimplemented!("unsupported python type, should be (cascaded) dict, list and basic numerical types")
     }
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 pub fn pyobject_to_json(value: PyObject) -> serde_json::Value {
-    Python::with_gil(|py| {
-        pyobject_to_json_locked(value, py)
-    })
+    Python::with_gil(|py| pyobject_to_json_locked(value, py))
 }
 
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 #[pyfunction]
 pub(crate) fn register(py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<SolverInitializer>()?;
     m.add_class::<PyMut>()?;
     m.add_class::<PartitionUnitInfo>()?;
     m.add_class::<PartitionInfo>()?;
     m.add_class::<PartitionConfig>()?;
     m.add_class::<SyndromePattern>()?;
     use crate::pyo3::PyTypeInfo;
     // m.add_class::<IndexRange>()?;
     m.add("VertexRange", VertexRange::type_object(py))?;
-    m.add("SyndromeRange", SyndromeRange::type_object(py))?;
+    m.add("DefectRange", DefectRange::type_object(py))?;
+    m.add("SyndromeRange", DefectRange::type_object(py))?; // backward compatibility
     m.add("NodeRange", NodeRange::type_object(py))?;
     Ok(())
 }
 
 #[cfg(test)]
 pub mod tests {
     use super::*;
 
     /// test syndrome partition utilities
     #[test]
-    fn util_partitioned_syndrome_pattern_1() {  // cargo test util_partitioned_syndrome_pattern_1 -- --nocapture
+    fn util_partitioned_syndrome_pattern_1() {
+        // cargo test util_partitioned_syndrome_pattern_1 -- --nocapture
         let mut partition_config = PartitionConfig::new(132);
         partition_config.partitions = vec![
-            VertexRange::new(0, 72),    // unit 0
-            VertexRange::new(84, 132),  // unit 1
+            VertexRange::new(0, 72),   // unit 0
+            VertexRange::new(84, 132), // unit 1
         ];
         partition_config.fusions = vec![
-            (0, 1),  // unit 2, by fusing 0 and 1
+            (0, 1), // unit 2, by fusing 0 and 1
         ];
         let partition_info = partition_config.info();
         let tests = vec![
-            (vec![10, 11, 12, 71, 72, 73, 84, 85, 111], SyndromeRange::new(4, 6)),
-            (vec![10, 11, 12, 13, 71, 72, 73, 84, 85, 111], SyndromeRange::new(5, 7)),
-            (vec![10, 11, 12, 71, 72, 73, 83, 84, 85, 111], SyndromeRange::new(4, 7)),
-            (vec![10, 11, 12, 71, 72, 73, 84, 85, 100, 101, 102, 103, 111], SyndromeRange::new(4, 6)),
+            (vec![10, 11, 12, 71, 72, 73, 84, 85, 111], DefectRange::new(4, 6)),
+            (vec![10, 11, 12, 13, 71, 72, 73, 84, 85, 111], DefectRange::new(5, 7)),
+            (vec![10, 11, 12, 71, 72, 73, 83, 84, 85, 111], DefectRange::new(4, 7)),
+            (
+                vec![10, 11, 12, 71, 72, 73, 84, 85, 100, 101, 102, 103, 111],
+                DefectRange::new(4, 6),
+            ),
         ];
         for (defect_vertices, expected_defect_range) in tests.into_iter() {
             let syndrome_pattern = SyndromePattern::new(defect_vertices, vec![]);
             let partitioned_syndrome_pattern = PartitionedSyndromePattern::new(&syndrome_pattern);
-            let (owned_partitioned, (_left_partitioned, _right_partitioned)) = partitioned_syndrome_pattern.partition(&partition_info.units[2]);
+            let (owned_partitioned, (_left_partitioned, _right_partitioned)) =
+                partitioned_syndrome_pattern.partition(&partition_info.units[2]);
             println!("defect_range: {:?}", owned_partitioned.whole_defect_range);
             assert_eq!(owned_partitioned.whole_defect_range, expected_defect_range);
         }
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/src/visualize.rs` & `fusion_blossom-0.2.5/src/visualize.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 //! Visualizer
-//! 
+//!
 //! This module helps visualize the progress of a fusion blossom algorithm
-//! 
+//!
 
-use crate::serde_json;
-use std::fs::File;
-use crate::serde::{Serialize, Deserialize};
-use std::io::{Write, Seek, SeekFrom};
 use crate::chrono::Local;
+use crate::serde::{Deserialize, Serialize};
+use crate::serde_json;
 use crate::urlencoding;
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
+use crate::util::*;
+#[cfg(feature = "python_binding")]
 use pyo3::prelude::*;
-
+use std::fs::File;
+use std::io::{Seek, SeekFrom, Write};
 
 pub trait FusionVisualizer {
     /// take a snapshot, set `abbrev` to true to save space
     fn snapshot(&self, abbrev: bool) -> serde_json::Value;
 }
 
+#[macro_export]
+macro_rules! bind_trait_fusion_visualizer {
+    ($struct_name:ident) => {
+        #[cfg(feature = "python_binding")]
+        #[pymethods]
+        impl $struct_name {
+            #[pyo3(name = "snapshot", signature = (abbrev = true))]
+            fn trait_snapshot(&self, abbrev: bool) -> PyObject {
+                json_to_pyobject(self.snapshot(abbrev))
+            }
+        }
+    };
+}
+#[allow(unused_imports)]
+pub use bind_trait_fusion_visualizer;
+
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct VisualizePosition {
     /// vertical axis, -i is up, +i is down (left-up corner is smallest i,j)
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub i: f64,
@@ -35,20 +52,20 @@
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl VisualizePosition {
     /// create a visualization position
     #[cfg_attr(feature = "python_binding", new)]
     pub fn new(i: f64, j: f64, t: f64) -> Self {
-        Self {
-            i, j, t
-        }
+        Self { i, j, t }
     }
     #[cfg(feature = "python_binding")]
-    fn __repr__(&self) -> String { format!("{:?}", self) }
+    fn __repr__(&self) -> String {
+        format!("{:?}", self)
+    }
 }
 
 #[derive(Debug)]
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pyclass)]
 pub struct Visualizer {
     /// save to file if applicable
@@ -59,95 +76,133 @@
     #[cfg_attr(feature = "python_binding", pyo3(get))]
     pub snapshots: Vec<String>,
 }
 
 pub fn snapshot_fix_missing_fields(value: &mut serde_json::Value, abbrev: bool) {
     let value = value.as_object_mut().expect("snapshot must be an object");
     // fix vertices missing fields
-    let vertices = value.get_mut("vertices").expect("missing unrecoverable field").as_array_mut().expect("vertices must be an array");
+    let vertices = value
+        .get_mut("vertices")
+        .expect("missing unrecoverable field")
+        .as_array_mut()
+        .expect("vertices must be an array");
     for vertex in vertices {
-        if vertex.is_null() { continue }  // vertex not present, probably currently don't care
+        if vertex.is_null() {
+            continue;
+        } // vertex not present, probably currently don't care
         let vertex = vertex.as_object_mut().expect("each vertex must be an object");
         let key_is_virtual = if abbrev { "v" } else { "is_virtual" };
         let key_is_defect = if abbrev { "s" } else { "is_defect" };
         // recover
         assert!(vertex.contains_key(key_is_virtual), "missing unrecoverable field");
         if !vertex.contains_key(key_is_defect) {
-            vertex.insert(key_is_defect.to_string(), json!(0));  // by default no syndrome
+            vertex.insert(key_is_defect.to_string(), json!(0)); // by default no syndrome
         }
     }
     // fix edges missing fields
-    let edges = value.get_mut("edges").expect("missing unrecoverable field").as_array_mut().expect("edges must be an array");
+    let edges = value
+        .get_mut("edges")
+        .expect("missing unrecoverable field")
+        .as_array_mut()
+        .expect("edges must be an array");
     for edge in edges {
-        if edge.is_null() { continue }  // edge not present, probably currently don't care
+        if edge.is_null() {
+            continue;
+        } // edge not present, probably currently don't care
         let edge = edge.as_object_mut().expect("each edge must be an object");
         let key_weight = if abbrev { "w" } else { "weight" };
         let key_left = if abbrev { "l" } else { "left" };
         let key_right = if abbrev { "r" } else { "right" };
         let key_left_growth = if abbrev { "lg" } else { "left_growth" };
         let key_right_growth = if abbrev { "rg" } else { "right_growth" };
         // recover
         assert!(edge.contains_key(key_weight), "missing unrecoverable field");
         assert!(edge.contains_key(key_left), "missing unrecoverable field");
         assert!(edge.contains_key(key_right), "missing unrecoverable field");
         if !edge.contains_key(key_left_growth) {
-            edge.insert(key_left_growth.to_string(), json!(0));  // by default no growth
+            edge.insert(key_left_growth.to_string(), json!(0)); // by default no growth
         }
         if !edge.contains_key(key_right_growth) {
-            edge.insert(key_right_growth.to_string(), json!(0));  // by default no growth
+            edge.insert(key_right_growth.to_string(), json!(0)); // by default no growth
         }
     }
 }
 
 pub type ObjectMap = serde_json::Map<String, serde_json::Value>;
 pub fn snapshot_combine_object_known_key(obj: &mut ObjectMap, obj_2: &mut ObjectMap, key: &str) {
     match (obj.contains_key(key), obj_2.contains_key(key)) {
-        (_, false) => { },  // do nothing
-        (false, true) => { obj.insert(key.to_string(), obj_2.remove(key).unwrap()); }
+        (_, false) => {} // do nothing
+        (false, true) => {
+            obj.insert(key.to_string(), obj_2.remove(key).unwrap());
+        }
         (true, true) => {
             // println!("[snapshot_combine_object_known_key] {}: {:?} == {:?}", key, obj[key], obj_2[key]);
-            assert_eq!(obj[key], obj_2[key], "cannot combine different values: please make sure values don't conflict");
+            assert_eq!(
+                obj[key], obj_2[key],
+                "cannot combine different values: please make sure values don't conflict"
+            );
             obj_2.remove(key).unwrap();
         }
     }
 }
 
 pub fn snapshot_copy_remaining_fields(obj: &mut ObjectMap, obj_2: &mut ObjectMap) {
     let mut keys = Vec::<String>::new();
     for key in obj_2.keys() {
         keys.push(key.clone());
     }
     for key in keys.iter() {
         match obj.contains_key(key) {
-            false => { obj.insert(key.to_string(), obj_2.remove(key).unwrap()); }
+            false => {
+                obj.insert(key.to_string(), obj_2.remove(key).unwrap());
+            }
             true => {
                 // println!("[snapshot_copy_remaining_fields] {}: {:?} == {:?}", key, obj[key], obj_2[key]);
                 // println!("obj: {obj:?}");
                 // println!("obj_2: {obj_2:?}");
-                assert_eq!(obj[key], obj_2[key], "cannot combine unknown fields: don't know what to do, please modify `snapshot_combine_values` function");
+                assert_eq!(
+                    obj[key], obj_2[key],
+                    "cannot combine unknown fields: don't know what to do, please modify `snapshot_combine_values` function"
+                );
                 obj_2.remove(key).unwrap();
             }
         }
     }
 }
 
 pub fn snapshot_combine_values(value: &mut serde_json::Value, mut value_2: serde_json::Value, abbrev: bool) {
     let value = value.as_object_mut().expect("snapshot must be an object");
     let value_2 = value_2.as_object_mut().expect("snapshot must be an object");
     match (value.contains_key("vertices"), value_2.contains_key("vertices")) {
-        (_, false) => { },  // do nothing
-        (false, true) => { value.insert("vertices".to_string(), value_2.remove("vertices").unwrap()); }
-        (true, true) => {  // combine
-            let vertices = value.get_mut("vertices").unwrap().as_array_mut().expect("vertices must be an array");
-            let vertices_2 = value_2.get_mut("vertices").unwrap().as_array_mut().expect("vertices must be an array");
+        (_, false) => {} // do nothing
+        (false, true) => {
+            value.insert("vertices".to_string(), value_2.remove("vertices").unwrap());
+        }
+        (true, true) => {
+            // combine
+            let vertices = value
+                .get_mut("vertices")
+                .unwrap()
+                .as_array_mut()
+                .expect("vertices must be an array");
+            let vertices_2 = value_2
+                .get_mut("vertices")
+                .unwrap()
+                .as_array_mut()
+                .expect("vertices must be an array");
             assert!(vertices.len() == vertices_2.len(), "vertices must be compatible");
             for (vertex_idx, vertex) in vertices.iter_mut().enumerate() {
                 let vertex_2 = &mut vertices_2[vertex_idx];
-                if vertex_2.is_null() { continue }
-                if vertex.is_null() { *vertex = vertex_2.clone(); continue }
+                if vertex_2.is_null() {
+                    continue;
+                }
+                if vertex.is_null() {
+                    *vertex = vertex_2.clone();
+                    continue;
+                }
                 // println!("vertex_idx: {vertex_idx}");
                 let vertex = vertex.as_object_mut().expect("each vertex must be an object");
                 let vertex_2 = vertex_2.as_object_mut().expect("each vertex must be an object");
                 // list known keys
                 let key_is_virtual = if abbrev { "v" } else { "is_virtual" };
                 let key_is_defect = if abbrev { "s" } else { "is_defect" };
                 let known_keys = [key_is_virtual, key_is_defect];
@@ -157,24 +212,40 @@
                 snapshot_copy_remaining_fields(vertex, vertex_2);
                 assert_eq!(vertex_2.len(), 0, "there should be nothing left");
             }
             value_2.remove("vertices").unwrap();
         }
     }
     match (value.contains_key("edges"), value_2.contains_key("edges")) {
-        (_, false) => { },  // do nothing
-        (false, true) => { value.insert("edges".to_string(), value_2.remove("edges").unwrap()); }
-        (true, true) => {  // combine
-            let edges = value.get_mut("edges").unwrap().as_array_mut().expect("edges must be an array");
-            let edges_2 = value_2.get_mut("edges").unwrap().as_array_mut().expect("edges must be an array");
+        (_, false) => {} // do nothing
+        (false, true) => {
+            value.insert("edges".to_string(), value_2.remove("edges").unwrap());
+        }
+        (true, true) => {
+            // combine
+            let edges = value
+                .get_mut("edges")
+                .unwrap()
+                .as_array_mut()
+                .expect("edges must be an array");
+            let edges_2 = value_2
+                .get_mut("edges")
+                .unwrap()
+                .as_array_mut()
+                .expect("edges must be an array");
             assert!(edges.len() == edges_2.len(), "edges must be compatible");
             for (edge_idx, edge) in edges.iter_mut().enumerate() {
                 let edge_2 = &mut edges_2[edge_idx];
-                if edge_2.is_null() { continue }
-                if edge.is_null() { *edge = edge_2.clone(); continue }
+                if edge_2.is_null() {
+                    continue;
+                }
+                if edge.is_null() {
+                    *edge = edge_2.clone();
+                    continue;
+                }
                 let edge = edge.as_object_mut().expect("each edge must be an object");
                 let edge_2 = edge_2.as_object_mut().expect("each edge must be an object");
                 // list known keys
                 let key_weight = if abbrev { "w" } else { "weight" };
                 let key_left = if abbrev { "l" } else { "left" };
                 let key_right = if abbrev { "r" } else { "right" };
                 let key_left_growth = if abbrev { "lg" } else { "left_growth" };
@@ -186,37 +257,59 @@
                 snapshot_copy_remaining_fields(edge, edge_2);
                 assert_eq!(edge_2.len(), 0, "there should be nothing left");
             }
             value_2.remove("edges").unwrap();
         }
     }
     match (value.contains_key("dual_nodes"), value_2.contains_key("dual_nodes")) {
-        (_, false) => { },  // do nothing
-        (false, true) => { value.insert("dual_nodes".to_string(), value_2.remove("dual_nodes").unwrap()); }
-        (true, true) => {  // combine
-            let dual_nodes = value.get_mut("dual_nodes").unwrap().as_array_mut().expect("dual_nodes must be an array");
-            let dual_nodes_2 = value_2.get_mut("dual_nodes").unwrap().as_array_mut().expect("dual_nodes must be an array");
+        (_, false) => {} // do nothing
+        (false, true) => {
+            value.insert("dual_nodes".to_string(), value_2.remove("dual_nodes").unwrap());
+        }
+        (true, true) => {
+            // combine
+            let dual_nodes = value
+                .get_mut("dual_nodes")
+                .unwrap()
+                .as_array_mut()
+                .expect("dual_nodes must be an array");
+            let dual_nodes_2 = value_2
+                .get_mut("dual_nodes")
+                .unwrap()
+                .as_array_mut()
+                .expect("dual_nodes must be an array");
             assert!(dual_nodes.len() == dual_nodes_2.len(), "dual_nodes must be compatible");
             for (dual_node_idx, dual_node) in dual_nodes.iter_mut().enumerate() {
                 let dual_node_2 = &mut dual_nodes_2[dual_node_idx];
                 if dual_node.is_null() {
-                    assert!(dual_node_2.is_null(), "dual node must be simultaneously be null, if necessary");
-                    continue
+                    assert!(
+                        dual_node_2.is_null(),
+                        "dual node must be simultaneously be null, if necessary"
+                    );
+                    continue;
                 }
                 let dual_node = dual_node.as_object_mut().expect("each dual_node must be an object");
                 let dual_node_2 = dual_node_2.as_object_mut().expect("each dual_node must be an object");
                 // list known keys
                 let key_boundary = if abbrev { "b" } else { "boundary" };
                 let key_dual_variable = if abbrev { "d" } else { "dual_variable" };
                 let key_blossom = if abbrev { "o" } else { "blossom" };
                 let key_defect_vertex = if abbrev { "s" } else { "defect_vertex" };
                 let key_grow_state = if abbrev { "g" } else { "grow_state" };
                 let key_unit_growth = if abbrev { "u" } else { "unit_growth" };
                 let key_parent_blossom = if abbrev { "p" } else { "parent_blossom" };
-                let known_keys = [key_boundary, key_dual_variable, key_blossom, key_defect_vertex, key_grow_state, key_unit_growth, key_parent_blossom];
+                let known_keys = [
+                    key_boundary,
+                    key_dual_variable,
+                    key_blossom,
+                    key_defect_vertex,
+                    key_grow_state,
+                    key_unit_growth,
+                    key_parent_blossom,
+                ];
                 for key in known_keys {
                     snapshot_combine_object_known_key(dual_node, dual_node_2, key);
                 }
                 snapshot_copy_remaining_fields(dual_node, dual_node_2);
                 assert_eq!(dual_node_2.len(), 0, "there should be nothing left");
             }
             value_2.remove("dual_nodes").unwrap();
@@ -231,112 +324,193 @@
         let mut max_i = positions[0].i;
         let mut min_i = positions[0].i;
         let mut max_j = positions[0].j;
         let mut min_j = positions[0].j;
         let mut max_t = positions[0].t;
         let mut min_t = positions[0].t;
         for position in positions.iter_mut() {
-            if position.i > max_i { max_i = position.i; }
-            if position.j > max_j { max_j = position.j; }
-            if position.t > max_t { max_t = position.t; }
-            if position.i < min_i { min_i = position.i; }
-            if position.j < min_j { min_j = position.j; }
-            if position.t < min_t { min_t = position.t; }
+            if position.i > max_i {
+                max_i = position.i;
+            }
+            if position.j > max_j {
+                max_j = position.j;
+            }
+            if position.t > max_t {
+                max_t = position.t;
+            }
+            if position.i < min_i {
+                min_i = position.i;
+            }
+            if position.j < min_j {
+                min_j = position.j;
+            }
+            if position.t < min_t {
+                min_t = position.t;
+            }
         }
         let (ci, cj, ct) = ((max_i + min_i) / 2., (max_j + min_j) / 2., (max_t + min_t) / 2.);
         for position in positions.iter_mut() {
             position.i -= ci;
             position.j -= cj;
             position.t -= ct;
         }
     }
     positions
 }
 
 #[cfg_attr(feature = "python_binding", cfg_eval)]
 #[cfg_attr(feature = "python_binding", pymethods)]
 impl Visualizer {
-
     /// create a new visualizer with target filename and node layout
     #[cfg_attr(feature = "python_binding", new)]
-    #[cfg_attr(feature = "python_binding", args(positions = "vec![]", center = "true"))]
+    #[cfg_attr(feature = "python_binding", pyo3(signature = (filepath, positions=vec![], center=true)))]
     pub fn new(mut filepath: Option<String>, mut positions: Vec<VisualizePosition>, center: bool) -> std::io::Result<Self> {
         if cfg!(feature = "disable_visualizer") {
-            filepath = None;  // do not open file
+            filepath = None; // do not open file
         }
         if center {
             positions = center_positions(positions);
         }
         let mut file = match filepath {
             Some(filepath) => Some(File::create(filepath)?),
             None => None,
         };
         if let Some(file) = file.as_mut() {
-            file.set_len(0)?;  // truncate the file
-            file.seek(SeekFrom::Start(0))?;  // move the cursor to the front
-            file.write_all(format!("{{\"format\":\"fusion_blossom\",\"version\":\"{}\"", env!("CARGO_PKG_VERSION")).as_bytes())?;
+            file.set_len(0)?; // truncate the file
+            file.seek(SeekFrom::Start(0))?; // move the cursor to the front
+            file.write_all(
+                format!(
+                    "{{\"format\":\"fusion_blossom\",\"version\":\"{}\"",
+                    env!("CARGO_PKG_VERSION")
+                )
+                .as_bytes(),
+            )?;
             file.write_all(b",\"positions\":")?;
             file.write_all(json!(positions).to_string().as_bytes())?;
             file.write_all(b",\"snapshots\":[]}")?;
             file.sync_all()?;
         }
         Ok(Self {
             file,
             empty_snapshot: true,
             snapshots: vec![],
         })
     }
 
+    #[cfg(feature = "python_binding")]
+    #[pyo3(name = "snapshot_combined")]
+    pub fn snapshot_combined_py(&mut self, name: String, object_pys: Vec<&PyAny>) -> std::io::Result<()> {
+        if cfg!(feature = "disable_visualizer") {
+            return Ok(());
+        }
+        let mut values = Vec::<serde_json::Value>::with_capacity(object_pys.len());
+        for object_py in object_pys.into_iter() {
+            values.push(pyobject_to_json(object_py.call_method0("snapshot")?.extract::<PyObject>()?));
+        }
+        self.snapshot_combined_value(name, values)
+    }
+
+    #[cfg(feature = "python_binding")]
+    #[pyo3(name = "snapshot")]
+    pub fn snapshot_py(&mut self, name: String, object_py: &PyAny) -> std::io::Result<()> {
+        if cfg!(feature = "disable_visualizer") {
+            return Ok(());
+        }
+        let value = pyobject_to_json(object_py.call_method0("snapshot")?.extract::<PyObject>()?);
+        self.snapshot_value(name, value)
+    }
+
+    #[cfg(feature = "python_binding")]
+    #[pyo3(name = "snapshot_combined_value")]
+    pub fn snapshot_combined_value_py(&mut self, name: String, value_pys: Vec<PyObject>) -> std::io::Result<()> {
+        if cfg!(feature = "disable_visualizer") {
+            return Ok(());
+        }
+        let values: Vec<_> = value_pys.into_iter().map(|value_py| pyobject_to_json(value_py)).collect();
+        self.snapshot_combined_value(name, values)
+    }
+
+    #[cfg(feature = "python_binding")]
+    #[pyo3(name = "snapshot_value")]
+    pub fn snapshot_value_py(&mut self, name: String, value_py: PyObject) -> std::io::Result<()> {
+        if cfg!(feature = "disable_visualizer") {
+            return Ok(());
+        }
+        let value = pyobject_to_json(value_py);
+        self.snapshot_value(name, value)
+    }
 }
 
 impl Visualizer {
-
     pub fn incremental_save(&mut self, name: String, value: serde_json::Value) -> std::io::Result<()> {
         if let Some(file) = self.file.as_mut() {
             self.snapshots.push(name.clone());
-            file.seek(SeekFrom::End(-2))?;  // move the cursor before the ending ]}
+            file.seek(SeekFrom::End(-2))?; // move the cursor before the ending ]}
             if !self.empty_snapshot {
                 file.write_all(b",")?;
             }
             self.empty_snapshot = false;
             file.write_all(json!((name, value)).to_string().as_bytes())?;
             file.write_all(b"]}")?;
             file.sync_all()?;
         }
         Ok(())
     }
 
-    /// append another snapshot of the fusion type, and also update the file in case 
+    /// append another snapshot of the fusion type, and also update the file in case
     pub fn snapshot_combined(&mut self, name: String, fusion_algorithms: Vec<&dyn FusionVisualizer>) -> std::io::Result<()> {
         if cfg!(feature = "disable_visualizer") {
-            return Ok(())
+            return Ok(());
         }
         let abbrev = true;
         let mut value = json!({});
         for fusion_algorithm in fusion_algorithms.iter() {
             let value_2 = fusion_algorithm.snapshot(abbrev);
             snapshot_combine_values(&mut value, value_2, abbrev);
         }
         snapshot_fix_missing_fields(&mut value, abbrev);
         self.incremental_save(name, value)?;
         Ok(())
     }
 
-    /// append another snapshot of the fusion type, and also update the file in case 
+    /// append another snapshot of the fusion type, and also update the file in case
     pub fn snapshot(&mut self, name: String, fusion_algorithm: &impl FusionVisualizer) -> std::io::Result<()> {
         if cfg!(feature = "disable_visualizer") {
-            return Ok(())
+            return Ok(());
         }
         let abbrev = true;
         let mut value = fusion_algorithm.snapshot(abbrev);
         snapshot_fix_missing_fields(&mut value, abbrev);
         self.incremental_save(name, value)?;
         Ok(())
     }
 
+    pub fn snapshot_combined_value(&mut self, name: String, values: Vec<serde_json::Value>) -> std::io::Result<()> {
+        if cfg!(feature = "disable_visualizer") {
+            return Ok(());
+        }
+        let abbrev = true;
+        let mut value = json!({});
+        for value_2 in values.into_iter() {
+            snapshot_combine_values(&mut value, value_2, abbrev);
+        }
+        snapshot_fix_missing_fields(&mut value, abbrev);
+        self.incremental_save(name, value)?;
+        Ok(())
+    }
+
+    pub fn snapshot_value(&mut self, name: String, mut value: serde_json::Value) -> std::io::Result<()> {
+        if cfg!(feature = "disable_visualizer") {
+            return Ok(());
+        }
+        let abbrev = true;
+        snapshot_fix_missing_fields(&mut value, abbrev);
+        self.incremental_save(name, value)?;
+        Ok(())
+    }
 }
 
 const DEFAULT_VISUALIZE_DATA_FOLDER: &str = concat!(env!("CARGO_MANIFEST_DIR"), "/visualize/data/");
 
 // only used locally, because this is compile time directory
 pub fn visualize_data_folder() -> String {
     DEFAULT_VISUALIZE_DATA_FOLDER.to_string()
@@ -359,135 +533,158 @@
     for (key, value) in parameters.iter() {
         link.push('&');
         link.push_str(&urlencoding::encode(key));
         link.push('=');
         link.push_str(&urlencoding::encode(value));
     }
     if cfg!(feature = "python_binding") {
-        println!("opening link {} (use `fusion_blossom.open_visualizer(filename)` to start a server and open it in browser)", link)
+        println!(
+            "opening link {} (use `fusion_blossom.open_visualizer(filename)` to start a server and open it in browser)",
+            link
+        )
     } else {
         println!("opening link {} (start local server by running ./visualize/server.sh) or call `node index.js <link>` to render locally", link)
     }
 }
 
 #[cfg_attr(feature = "python_binding", pyfunction)]
 pub fn print_visualize_link(filename: String) {
     print_visualize_link_with_parameters(filename, Vec::new())
 }
 
-
-#[cfg(feature="python_binding")]
+#[cfg(feature = "python_binding")]
 #[pyfunction]
 pub(crate) fn register(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<VisualizePosition>()?;
     m.add_class::<Visualizer>()?;
     m.add_function(wrap_pyfunction!(static_visualize_data_filename, m)?)?;
     m.add_function(wrap_pyfunction!(auto_visualize_data_filename, m)?)?;
     m.add_function(wrap_pyfunction!(print_visualize_link_with_parameters, m)?)?;
     m.add_function(wrap_pyfunction!(print_visualize_link, m)?)?;
     m.add_function(wrap_pyfunction!(center_positions, m)?)?;
     Ok(())
 }
 
-
 #[cfg(test)]
 mod tests {
-    use super::*;
-    use super::super::*;
-    use super::super::example_codes::*;
-    use super::super::dual_module_serial::*;
     use super::super::dual_module::*;
+    use super::super::dual_module_serial::*;
+    use super::super::example_codes::*;
     use super::super::pointers::*;
-    use super::super::primal_module_serial::*;
     use super::super::primal_module::*;
-
+    use super::super::primal_module_serial::*;
+    use super::super::*;
+    use super::*;
 
     #[test]
-    fn visualize_test_1() {  // cargo test visualize_test_1 -- --nocapture
+    fn visualize_test_1() {
+        // cargo test visualize_test_1 -- --nocapture
         let visualize_filename = format!("visualize_test_1.json");
         let half_weight = 500;
         let mut code = CodeCapacityPlanarCode::new(11, 0.2, half_weight);
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
+        let mut visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            code.get_positions(),
+            true,
+        )
+        .unwrap();
         print_visualize_link(visualize_filename.clone());
         // create dual module
         let initializer = code.get_initializer();
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
         let defect_vertices = vec![39, 63, 52, 100, 90];
         for defect_vertex in defect_vertices.iter() {
             code.vertices[*defect_vertex].is_defect = true;
         }
         let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
-        visualizer.snapshot_combined(format!("initial"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("initial"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // create dual nodes and grow them by half length
         // test basic grow and shrink of a single tree node
         for _ in 0..4 {
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), half_weight);
-            visualizer.snapshot_combined(format!("grow half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("grow half weight"), vec![&interface_ptr, &dual_module])
+                .unwrap();
         }
         for _ in 0..4 {
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), -half_weight);
-            visualizer.snapshot_combined(format!("shrink half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("shrink half weight"), vec![&interface_ptr, &dual_module])
+                .unwrap();
+        }
+        for _ in 0..3 {
+            dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), half_weight);
         }
-        for _ in 0..3 { dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), half_weight); }
-        visualizer.snapshot_combined(format!("grow 3 half weight"), vec![&interface_ptr, &dual_module]).unwrap();
-        for _ in 0..3 { dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), -half_weight); }
-        visualizer.snapshot_combined(format!("shrink 3 half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("grow 3 half weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
+        for _ in 0..3 {
+            dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), -half_weight);
+        }
+        visualizer
+            .snapshot_combined(format!("shrink 3 half weight"), vec![&interface_ptr, &dual_module])
+            .unwrap();
         // test all
         for i in 0..interface_ptr.read_recursive().nodes_length {
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[i].clone().unwrap(), half_weight);
-            visualizer.snapshot_combined(format!("grow half weight"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("grow half weight"), vec![&interface_ptr, &dual_module])
+                .unwrap();
         }
     }
 
     #[test]
-    fn visualize_paper_weighted_union_find_decoder() {  // cargo test visualize_paper_weighted_union_find_decoder -- --nocapture
+    fn visualize_paper_weighted_union_find_decoder() {
+        // cargo test visualize_paper_weighted_union_find_decoder -- --nocapture
         let visualize_filename = format!("visualize_paper_weighted_union_find_decoder.json");
         let d: VertexNum = 3;
         let td: VertexNum = 4;
         let p = 0.2f64;
-        let row_vertex_num = (d-1) + 2;  // two virtual vertices at left and right
-        let t_vertex_num = row_vertex_num * d;  // `d` rows
-        let half_vertex_num = t_vertex_num * td;  // `td` layers
-        let vertex_num = half_vertex_num * 2;  // both X and Z type stabilizers altogether
+        let row_vertex_num = (d - 1) + 2; // two virtual vertices at left and right
+        let t_vertex_num = row_vertex_num * d; // `d` rows
+        let half_vertex_num = t_vertex_num * td; // `td` layers
+        let vertex_num = half_vertex_num * 2; // both X and Z type stabilizers altogether
         let half_weight: Weight = (10000. * ((1. - p).ln() - p.ln())).max(1.) as Weight;
-        let weight = half_weight * 2;  // to make sure weight is even number for ease of this test function
+        let weight = half_weight * 2; // to make sure weight is even number for ease of this test function
         let weighted_edges = {
             let mut weighted_edges: Vec<(VertexIndex, VertexIndex, Weight)> = Vec::new();
             for is_z in [true, false] {
                 for t in 0..td {
                     let t_bias = t * t_vertex_num + if is_z { 0 } else { half_vertex_num };
                     for row in 0..d {
                         let bias = t_bias + row * row_vertex_num;
-                        for i in 0..d-1 {
-                            weighted_edges.push((bias + i, bias + i+1, weight));
+                        for i in 0..d - 1 {
+                            weighted_edges.push((bias + i, bias + i + 1, weight));
                         }
-                        weighted_edges.push((bias + 0, bias + d, weight));  // left most edge
+                        weighted_edges.push((bias + 0, bias + d, weight)); // left most edge
                         if row + 1 < d {
-                            for i in 0..d-1 {
+                            for i in 0..d - 1 {
                                 weighted_edges.push((bias + i, bias + i + row_vertex_num, weight));
                             }
                         }
                     }
                     // inter-layer connection
                     if t + 1 < td {
                         for row in 0..d {
                             let bias = t_bias + row * row_vertex_num;
-                            for i in 0..d-1 {
+                            for i in 0..d - 1 {
                                 weighted_edges.push((bias + i, bias + i + t_vertex_num, weight));
                                 // diagonal edges
                                 let diagonal_diffs: Vec<(isize, isize)> = if is_z {
                                     vec![(0, 1), (1, 0), (1, 1)]
                                 } else {
                                     // i and j are reversed if x stabilizer, not vec![(0, -2), (2, 0), (2, -2)]
                                     vec![(-1, 0), (0, 1), (-1, 1)]
                                 };
                                 for (di, dj) in diagonal_diffs {
-                                    let new_row = row as isize + di;  // row corresponds to `i`
-                                    let new_i = i as isize + dj;  // i corresponds to `j`
-                                    if new_row >= 0 && new_i >= 0 && new_row < d as isize && new_i < (d-1) as isize {
+                                    let new_row = row as isize + di; // row corresponds to `i`
+                                    let new_i = i as isize + dj; // i corresponds to `j`
+                                    if new_row >= 0 && new_i >= 0 && new_row < d as isize && new_i < (d - 1) as isize {
                                         let new_bias = t_bias + (new_row as VertexNum) * row_vertex_num + t_vertex_num;
                                         weighted_edges.push((bias + i, new_bias + new_i as VertexNum, weight));
                                     }
                                 }
                             }
                         }
                     }
@@ -509,15 +706,18 @@
             }
             virtual_vertices
         };
         // hardcode syndrome
         let defect_vertices = vec![16, 29, 88, 72, 32, 44, 20, 21, 68, 69];
         let grow_edges = vec![48, 156, 169, 81, 38, 135];
         // run single-thread fusion blossom algorithm
-        print_visualize_link_with_parameters(visualize_filename.clone(), vec![(format!("patch"), format!("visualize_paper_weighted_union_find_decoder"))]);
+        print_visualize_link_with_parameters(
+            visualize_filename.clone(),
+            vec![(format!("patch"), format!("visualize_paper_weighted_union_find_decoder"))],
+        );
         let mut positions = Vec::new();
         let scale = 2f64;
         for is_z in [true, false] {
             for t in 0..td {
                 let pos_t = t as f64;
                 for row in 0..d {
                     let pos_i = row as f64;
@@ -532,116 +732,169 @@
                         positions.push(VisualizePosition::new(pos_i * scale, (-1. + 0.5) * scale, pos_t * scale));
                     } else {
                         positions.push(VisualizePosition::new((-1. + 0.5) * scale, pos_i * scale, pos_t * scale));
                     }
                 }
             }
         }
-        let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), positions, true).unwrap();
+        let mut visualizer =
+            Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), positions, true).unwrap();
         let initializer = SolverInitializer::new(vertex_num, weighted_edges, virtual_vertices);
         let mut dual_module = DualModuleSerial::new_empty(&initializer);
-        let interface_ptr = DualModuleInterfacePtr::new_load(&SyndromePattern::new_vertices(defect_vertices), &mut dual_module);
+        let interface_ptr =
+            DualModuleInterfacePtr::new_load(&SyndromePattern::new_vertices(defect_vertices), &mut dual_module);
         // grow edges
         for &edge_index in grow_edges.iter() {
             let mut edge = dual_module.edges[edge_index].write_force();
             edge.left_growth = edge.weight;
         }
         // save snapshot
-        visualizer.snapshot_combined(format!("initial"), vec![&interface_ptr, &dual_module]).unwrap();
+        visualizer
+            .snapshot_combined(format!("initial"), vec![&interface_ptr, &dual_module])
+            .unwrap();
     }
 
     #[test]
-    fn visualize_rough_idea_fusion_blossom() {  // cargo test visualize_rough_idea_fusion_blossom -- --nocapture
+    fn visualize_rough_idea_fusion_blossom() {
+        // cargo test visualize_rough_idea_fusion_blossom -- --nocapture
         let quarter_weight = 250;
         let half_weight = 2 * quarter_weight;
         for is_circuit_level in [false, true] {
             let visualize_filename = if is_circuit_level {
                 format!("visualize_rough_idea_fusion_blossom_circuit_level.json")
             } else {
                 format!("visualize_rough_idea_fusion_blossom.json")
             };
             let mut code: Box<dyn ExampleCode> = if is_circuit_level {
-                Box::new(CircuitLevelPlanarCode::new_diagonal(7, 7, 0.2, half_weight, 0.2))
+                Box::new(CircuitLevelPlanarCode::new_diagonal(7, 7, 0.2, half_weight, None))
             } else {
                 Box::new(PhenomenologicalPlanarCode::new(7, 7, 0.2, half_weight))
             };
-            let mut visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), code.get_positions(), true).unwrap();
-            print_visualize_link_with_parameters(visualize_filename, vec![(format!("patch"), format!("visualize_rough_idea_fusion_blossom"))]);
+            let mut visualizer = Visualizer::new(
+                Some(visualize_data_folder() + visualize_filename.as_str()),
+                code.get_positions(),
+                true,
+            )
+            .unwrap();
+            print_visualize_link_with_parameters(
+                visualize_filename,
+                vec![(format!("patch"), format!("visualize_rough_idea_fusion_blossom"))],
+            );
             // create dual module
             let initializer = code.get_initializer();
             let mut dual_module = DualModuleSerial::new_empty(&initializer);
             // hardcode syndrome          1   2   0   3    5    4    6    7
             let defect_vertices = vec![25, 33, 20, 76, 203, 187, 243, 315];
             code.set_defect_vertices(&defect_vertices);
             // create dual nodes and grow them by half length
             let interface_ptr = DualModuleInterfacePtr::new_load(&code.get_syndrome(), &mut dual_module);
             // save snapshot
-            visualizer.snapshot_combined(format!("initial"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("initial"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             // first layer grow first
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), quarter_weight);
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[1].clone().unwrap(), quarter_weight);
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[2].clone().unwrap(), quarter_weight);
-            visualizer.snapshot_combined(format!("grow a quarter"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("grow a quarter"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             // merge and match
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), quarter_weight);
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[1].clone().unwrap(), quarter_weight);
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[2].clone().unwrap(), quarter_weight);
-            visualizer.snapshot_combined(format!("find a match"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("find a match"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             // grow to boundary
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[0].clone().unwrap(), half_weight);
-            visualizer.snapshot_combined(format!("touch temporal boundary"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("touch temporal boundary"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             // add more measurement rounds
-            visualizer.snapshot_combined(format!("add measurement #2"), vec![&interface_ptr, &dual_module]).unwrap();
-            visualizer.snapshot_combined(format!("add measurement #3"), vec![&interface_ptr, &dual_module]).unwrap();
-            visualizer.snapshot_combined(format!("add measurement #4"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("add measurement #2"), vec![&interface_ptr, &dual_module])
+                .unwrap();
+            visualizer
+                .snapshot_combined(format!("add measurement #3"), vec![&interface_ptr, &dual_module])
+                .unwrap();
+            visualizer
+                .snapshot_combined(format!("add measurement #4"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             // handle errors at measurement round 4
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[5].clone().unwrap(), half_weight);
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[4].clone().unwrap(), half_weight);
-            visualizer.snapshot_combined(format!("grow a half"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("grow a half"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[5].clone().unwrap(), half_weight);
             dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[4].clone().unwrap(), half_weight);
-            visualizer.snapshot_combined(format!("temporary match"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("temporary match"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             // handle errors at measurement round 5
-            visualizer.snapshot_combined(format!("add measurement #5"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("add measurement #5"), vec![&interface_ptr, &dual_module])
+                .unwrap();
             for _ in 0..4 {
                 dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[4].clone().unwrap(), -quarter_weight);
                 dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[5].clone().unwrap(), quarter_weight);
                 dual_module.grow_dual_node(&interface_ptr.read_recursive().nodes[6].clone().unwrap(), quarter_weight);
-                visualizer.snapshot_combined(format!("grow or shrink a quarter"), vec![&interface_ptr, &dual_module]).unwrap();
+                visualizer
+                    .snapshot_combined(format!("grow or shrink a quarter"), vec![&interface_ptr, &dual_module])
+                    .unwrap();
             }
-            visualizer.snapshot_combined(format!("add measurement #6"), vec![&interface_ptr, &dual_module]).unwrap();
-            visualizer.snapshot_combined(format!("add measurement #7"), vec![&interface_ptr, &dual_module]).unwrap();
-            visualizer.snapshot_combined(format!("add measurement #8"), vec![&interface_ptr, &dual_module]).unwrap();
+            visualizer
+                .snapshot_combined(format!("add measurement #6"), vec![&interface_ptr, &dual_module])
+                .unwrap();
+            visualizer
+                .snapshot_combined(format!("add measurement #7"), vec![&interface_ptr, &dual_module])
+                .unwrap();
+            visualizer
+                .snapshot_combined(format!("add measurement #8"), vec![&interface_ptr, &dual_module])
+                .unwrap();
         }
     }
 
     #[test]
-    fn visualize_example_syndrome_graph() {  // cargo test visualize_example_syndrome_graph -- --nocapture
+    fn visualize_example_syndrome_graph() {
+        // cargo test visualize_example_syndrome_graph -- --nocapture
         let visualize_filename = format!("visualize_example_syndrome_graph.json");
         // let defect_vertices = vec![39, 52, 63, 90, 100];
         //                        0   1   2   3   4   5   6   7   8    9
         //                        A  vA   B  vB   C  vC   D  vD   E   vE
-        let kept_vertices = vec![39, 47, 52, 59, 63, 71, 90, 94, 100, 107];  // including some virtual vertices
-        let mut old_to_new = std::collections::BTreeMap::<SyndromeIndex, SyndromeIndex>::new();
+        let kept_vertices = vec![39, 47, 52, 59, 63, 71, 90, 94, 100, 107]; // including some virtual vertices
+        let mut old_to_new = std::collections::BTreeMap::<DefectIndex, DefectIndex>::new();
         for (new_index, defect_vertex) in kept_vertices.iter().enumerate() {
-            old_to_new.insert(*defect_vertex, new_index as SyndromeIndex);
+            old_to_new.insert(*defect_vertex, new_index as DefectIndex);
         }
         println!("{old_to_new:?}");
         let d = 11;
         let half_weight = 500;
         let code = CodeCapacityPlanarCode::new(d, 0.1, half_weight);
         let positions = code.get_positions();
-        let (ci, cj) = ((positions[131].i + positions[11].i) / 2., (positions[10].j + positions[11].j) / 2.);
-        let syndrome_graph_positions: Vec<_> = kept_vertices.iter().map(|i| {
-            let mut position = positions[*i as usize].clone();
-            position.i -= ci;
-            position.j -= cj;
-            position
-        }).collect();
-        let visualizer = Visualizer::new(Some(visualize_data_folder() + visualize_filename.as_str()), syndrome_graph_positions, false).unwrap();
+        let (ci, cj) = (
+            (positions[131].i + positions[11].i) / 2.,
+            (positions[10].j + positions[11].j) / 2.,
+        );
+        let syndrome_graph_positions: Vec<_> = kept_vertices
+            .iter()
+            .map(|i| {
+                let mut position = positions[*i as usize].clone();
+                position.i -= ci;
+                position.j -= cj;
+                position
+            })
+            .collect();
+        let visualizer = Visualizer::new(
+            Some(visualize_data_folder() + visualize_filename.as_str()),
+            syndrome_graph_positions,
+            false,
+        )
+        .unwrap();
         let mut visualizer = Some(visualizer);
         print_visualize_link(visualize_filename.clone());
         let syndrome_graph_edges = vec![
             // virtual to real edges
             (0, 1, 4000),
             (2, 3, 5000),
             (4, 5, 4000),
@@ -655,26 +908,40 @@
             (2, 4, 2000),
             (2, 6, 5000),
             (2, 8, 4000),
             (4, 6, 5000),
             (4, 8, 4000),
             (6, 8, 3000),
         ];
-        let syndrome_graph_initializer = SolverInitializer::new(kept_vertices.len() as VertexNum, syndrome_graph_edges, vec![1,3,5,7,9]);
+        let syndrome_graph_initializer =
+            SolverInitializer::new(kept_vertices.len() as VertexNum, syndrome_graph_edges, vec![1, 3, 5, 7, 9]);
         println!("syndrome_graph_initializer: {syndrome_graph_initializer:?}");
         let mut dual_module = DualModuleSerial::new_empty(&syndrome_graph_initializer);
         // create primal module
         let mut primal_module = PrimalModuleSerialPtr::new_empty(&syndrome_graph_initializer);
         let interface_ptr = DualModuleInterfacePtr::new_empty();
-        let syndrome_graph_syndrome = SyndromePattern::new(vec![0,2,4,6,8], vec![]);
-        primal_module.solve_visualizer(&interface_ptr, &syndrome_graph_syndrome, &mut dual_module, visualizer.as_mut());
+        let syndrome_graph_syndrome = SyndromePattern::new(vec![0, 2, 4, 6, 8], vec![]);
+        primal_module.solve_visualizer(
+            &interface_ptr,
+            &syndrome_graph_syndrome,
+            &mut dual_module,
+            visualizer.as_mut(),
+        );
         let perfect_matching = primal_module.perfect_matching(&interface_ptr, &mut dual_module);
         let mut subgraph_builder = SubGraphBuilder::new(&syndrome_graph_initializer);
         subgraph_builder.load_perfect_matching(&perfect_matching);
         let subgraph = subgraph_builder.get_subgraph();
         if let Some(visualizer) = visualizer.as_mut() {
-            visualizer.snapshot_combined("perfect matching and subgraph".to_string(), vec![&interface_ptr, &dual_module
-                , &perfect_matching, &VisualizeSubgraph::new(&subgraph)]).unwrap();
+            visualizer
+                .snapshot_combined(
+                    "perfect matching and subgraph".to_string(),
+                    vec![
+                        &interface_ptr,
+                        &dual_module,
+                        &perfect_matching,
+                        &VisualizeSubgraph::new(&subgraph),
+                    ],
+                )
+                .unwrap();
         }
     }
-
 }
```

### Comparing `fusion_blossom-0.2.2/test.sh` & `fusion_blossom-0.2.5/test.sh`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/test_build.sh` & `fusion_blossom-0.2.5/test_check.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/bin/sh
 set -ex
 
-cargo clean
-cargo clippy  # A collection of lints to catch common mistakes and improve your Rust code.
+cargo fmt --check
+cargo clippy -- -Dwarnings  # A collection of lints to catch common mistakes and improve your Rust code.
 
 # check this first because it's easy to have errors
-cargo build --features u32_index
-cargo build --features u32_index --release
+cargo check --features u32_index
+cargo check --features u32_index --release
+cargo check --features disable_visualizer,u32_index --release
+cargo check --features qecp_integrate
 
-cargo build
-cargo build --release
-cargo build --features unsafe_pointer
-cargo build --features unsafe_pointer --release
-cargo build --features i32_weight
-cargo build --features i32_weight --release
-cargo build --features disable_visualizer
-cargo build --features disable_visualizer --release
-# cargo build --features python_binding
-# cargo build --features python_binding --release
+cargo check --release
+cargo check --features unsafe_pointer
+cargo check --features unsafe_pointer --release
+cargo check --features i32_weight
+cargo check --features i32_weight --release
+cargo check --features disable_visualizer
+cargo check --features disable_visualizer --release
+# cargo check --features python_binding
+# cargo check --features python_binding --release
```

### Comparing `fusion_blossom-0.2.2/visualize/cmd.js` & `fusion_blossom-0.2.5/visualize/cmd.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/data/filter_data.py` & `fusion_blossom-0.2.5/visualize/data/filter_data.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/gui3d.js` & `fusion_blossom-0.2.5/visualize/gui3d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -370,20 +370,14 @@
             vertex_caches.push({
                 position: {
                     center: compute_vector3(position),
                 }
             })
         }
         // draw vertices
-        let subgraph_set = {}
-        if (snapshot.subgraph != null) {
-            for (let edge_index of snapshot.subgraph) {
-                subgraph_set[edge_index] = true
-            }
-        }
         for (let [i, vertex] of snapshot.vertices.entries()) {
             if (vertex == null) {
                 if (i < vertex_meshes.length) { // hide
                     vertex_meshes[i].visible = false
                 }
                 continue
             }
@@ -411,14 +405,20 @@
             }
             vertex_mesh.visible = true
         }
         for (let i = snapshot.vertices.length; i < vertex_meshes.length; ++i) {
             vertex_meshes[i].visible = false
         }
         // draw edges
+        let subgraph_set = {}
+        if (snapshot.subgraph != null) {
+            for (let edge_index of snapshot.subgraph) {
+                subgraph_set[edge_index] = true
+            }
+        }
         let edge_offset = 0
         if (scaled_edge_radius.value < scaled_vertex_outline_radius.value) {
             edge_offset = Math.sqrt(Math.pow(scaled_vertex_outline_radius.value, 2) - Math.pow(scaled_edge_radius.value, 2))
         }
         edge_caches = [] // clear cache
         for (let [i, edge] of snapshot.edges.entries()) {
             if (edge == null) {
@@ -535,79 +535,81 @@
             }
             vertex_outline_mesh.visible = true
         }
         for (let i = snapshot.vertices.length; i < vertex_meshes.length; ++i) {
             vertex_outline_meshes[i].visible = false
         }
         // draw convex
-        for (let blossom_convex_mesh of blossom_convex_meshes) {
-            scene.remove(blossom_convex_mesh)
-            blossom_convex_mesh.geometry.dispose()
-        }
-        for (let [i, dual_node] of snapshot.dual_nodes.entries()) {
-            if (dual_node == null) {
-                continue
-            }
-            if (snapshot.subgraph != null) {
-                continue
-            } // do not display convex if subgraph is displayed
-            // for child node in a blossom, this will not display properly; we should avoid plotting child nodes
-            let display_node = dual_node.p == null && (dual_node.d > 0 || dual_node.o != null)
-            if (display_node) { // no parent and (positive dual variable or it's a blossom)
-                let points = []
-                if (dual_node.b != null) {
-                    for (let [is_left, edge_index] of dual_node.b) {
-                        let cached_position = edge_caches[edge_index].position
-                        const edge = snapshot.edges[edge_index]
-                        if (edge.ld == edge.rd && edge.lg + edge.rg >= edge.w) {
-                            continue // do not draw this edge, this is an internal edge
-                        }
-                        if (is_left) {
-                            if (edge.lg == edge.w) {
-                                points.push(vertex_caches[edge.r].position.center.clone())
-                            } else if (edge.lg == 0) {
-                                points.push(vertex_caches[edge.l].position.center.clone())
-                            } else {
-                                points.push(cached_position.left_end.clone())
+        if (snapshot.dual_nodes != null) {
+            for (let blossom_convex_mesh of blossom_convex_meshes) {
+                scene.remove(blossom_convex_mesh)
+                blossom_convex_mesh.geometry.dispose()
+            }
+            for (let [i, dual_node] of snapshot.dual_nodes.entries()) {
+                if (dual_node == null) {
+                    continue
+                }
+                if (snapshot.subgraph != null) {
+                    continue
+                } // do not display convex if subgraph is displayed
+                // for child node in a blossom, this will not display properly; we should avoid plotting child nodes
+                let display_node = dual_node.p == null && (dual_node.d > 0 || dual_node.o != null)
+                if (display_node) { // no parent and (positive dual variable or it's a blossom)
+                    let points = []
+                    if (dual_node.b != null) {
+                        for (let [is_left, edge_index] of dual_node.b) {
+                            let cached_position = edge_caches[edge_index].position
+                            const edge = snapshot.edges[edge_index]
+                            if (edge.ld == edge.rd && edge.lg + edge.rg >= edge.w) {
+                                continue // do not draw this edge, this is an internal edge
                             }
-                        } else {
-                            if (edge.rg == edge.w) {
-                                points.push(vertex_caches[edge.l].position.center.clone())
-                            } else if (edge.rg == 0) {
-                                points.push(vertex_caches[edge.r].position.center.clone())
+                            if (is_left) {
+                                if (edge.lg == edge.w) {
+                                    points.push(vertex_caches[edge.r].position.center.clone())
+                                } else if (edge.lg == 0) {
+                                    points.push(vertex_caches[edge.l].position.center.clone())
+                                } else {
+                                    points.push(cached_position.left_end.clone())
+                                }
                             } else {
-                                points.push(cached_position.right_end.clone())
+                                if (edge.rg == edge.w) {
+                                    points.push(vertex_caches[edge.l].position.center.clone())
+                                } else if (edge.rg == 0) {
+                                    points.push(vertex_caches[edge.r].position.center.clone())
+                                } else {
+                                    points.push(cached_position.right_end.clone())
+                                }
                             }
                         }
                     }
-                }
-                if (points.length >= 3) { // only display if points is more than 3
-                    if (window.is_vertices_2d_plane) {
-                        // special optimization for 2D points, because ConvexGeometry doesn't work well on them
-                        const points_2d = []
-                        for (let point of points) {
-                            points_2d.push([point.x, point.z])
-                        }
-                        const hull_points = hull(points_2d, 1)
-                        const shape_points = []
-                        for (let hull_point of hull_points) {
-                            shape_points.push(new THREE.Vector2(hull_point[0], hull_point[1]));
+                    if (points.length >= 3) { // only display if points is more than 3
+                        if (window.is_vertices_2d_plane) {
+                            // special optimization for 2D points, because ConvexGeometry doesn't work well on them
+                            const points_2d = []
+                            for (let point of points) {
+                                points_2d.push([point.x, point.z])
+                            }
+                            const hull_points = hull(points_2d, 1)
+                            const shape_points = []
+                            for (let hull_point of hull_points) {
+                                shape_points.push(new THREE.Vector2(hull_point[0], hull_point[1]));
+                            }
+                            const shape = new THREE.Shape(shape_points)
+                            const geometry = new THREE.ShapeGeometry(shape)
+                            const blossom_convex_mesh = new THREE.Mesh(geometry, blossom_convex_material_2d)
+                            blossom_convex_mesh.position.set(0, -0.2, 0) // place the plane to slightly below the vertices for better viz
+                            blossom_convex_mesh.rotation.set(Math.PI / 2, 0, 0);
+                            scene.add(blossom_convex_mesh)
+                            blossom_convex_meshes.push(blossom_convex_mesh)
+                        } else {
+                            const geometry = new ConvexGeometry(points)
+                            const blossom_convex_mesh = new THREE.Mesh(geometry, blossom_convex_material)
+                            scene.add(blossom_convex_mesh)
+                            blossom_convex_meshes.push(blossom_convex_mesh)
                         }
-                        const shape = new THREE.Shape(shape_points)
-                        const geometry = new THREE.ShapeGeometry(shape)
-                        const blossom_convex_mesh = new THREE.Mesh(geometry, blossom_convex_material_2d)
-                        blossom_convex_mesh.position.set(0, -0.2, 0) // place the plane to slightly below the vertices for better viz
-                        blossom_convex_mesh.rotation.set(Math.PI / 2, 0, 0);
-                        scene.add(blossom_convex_mesh)
-                        blossom_convex_meshes.push(blossom_convex_mesh)
-                    } else {
-                        const geometry = new ConvexGeometry(points)
-                        const blossom_convex_mesh = new THREE.Mesh(geometry, blossom_convex_material)
-                        scene.add(blossom_convex_mesh)
-                        blossom_convex_meshes.push(blossom_convex_mesh)
                     }
                 }
             }
         }
         // reset select
         await Vue.nextTick()
         if (is_user_data_valid(current_selected_value)) {
@@ -703,24 +705,24 @@
 controller.virtual_vertex_color = vertex_folder.addColor(conf, 'virtual_vertex_color').onChange(function(value) {
     virtual_vertex_material.color = value
 })
 controller.virtual_vertex_opacity = vertex_folder.add(conf, 'virtual_vertex_opacity', 0, 1).onChange(function(value) {
     virtual_vertex_material.opacity = Number(value)
 })
 const vertex_outline_folder = gui.addFolder('vertex outline')
-controller.vertex_outline_color = vertex_outline_folder.addColor(conf, 'defect_vertex_outline_color').onChange(function(value) {
+controller.defect_vertex_outline_color = vertex_outline_folder.addColor(conf, 'defect_vertex_outline_color').onChange(function(value) {
     defect_vertex_outline_material.color = value
 })
-controller.vertex_outline_opacity = vertex_outline_folder.add(conf, 'defect_vertex_outline_opacity', 0, 1).onChange(function(value) {
+controller.defect_vertex_outline_opacity = vertex_outline_folder.add(conf, 'defect_vertex_outline_opacity', 0, 1).onChange(function(value) {
     defect_vertex_outline_material.opacity = Number(value)
 })
-controller.vertex_outline_color = vertex_outline_folder.addColor(conf, 'real_vertex_outline_color').onChange(function(value) {
+controller.real_vertex_outline_color = vertex_outline_folder.addColor(conf, 'real_vertex_outline_color').onChange(function(value) {
     real_vertex_outline_material.color = value
 })
-controller.vertex_outline_opacity = vertex_outline_folder.add(conf, 'real_vertex_outline_opacity', 0, 1).onChange(function(value) {
+controller.real_vertex_outline_opacity = vertex_outline_folder.add(conf, 'real_vertex_outline_opacity', 0, 1).onChange(function(value) {
     real_vertex_outline_material.opacity = Number(value)
 })
 controller.virtual_vertex_outline_color = vertex_outline_folder.addColor(conf, 'virtual_vertex_outline_color').onChange(function(value) {
     virtual_vertex_outline_material.color = value
 })
 controller.virtual_vertex_outline_opacity = vertex_outline_folder.add(conf, 'virtual_vertex_outline_opacity', 0, 1).onChange(function(value) {
     virtual_vertex_outline_material.opacity = Number(value)
```

### Comparing `fusion_blossom-0.2.2/visualize/img/basic_CSS_3D_bottom_image.png` & `fusion_blossom-0.2.5/visualize/img/basic_CSS_3D_bottom_image.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/img/parallel_circuit_level.png` & `fusion_blossom-0.2.5/visualize/img/parallel_circuit_level.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/img/parallel_phenomenological.png` & `fusion_blossom-0.2.5/visualize/img/parallel_phenomenological.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/img/parallel_simple.png` & `fusion_blossom-0.2.5/visualize/img/parallel_simple.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/img/serial_example.png` & `fusion_blossom-0.2.5/visualize/img/serial_example.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/img/serial_random.png` & `fusion_blossom-0.2.5/visualize/img/serial_random.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/img/serial_simple.png` & `fusion_blossom-0.2.5/visualize/img/serial_simple.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/index.html` & `fusion_blossom-0.2.5/visualize/index.html`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/index.js` & `fusion_blossom-0.2.5/visualize/index.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/mocker.js` & `fusion_blossom-0.2.5/visualize/mocker.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/package-lock.json` & `fusion_blossom-0.2.5/visualize/package-lock.json`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/partition-profile.html` & `fusion_blossom-0.2.5/visualize/partition-profile.html`

 * *Files 2% similar despite different names*

```diff
@@ -226,24 +226,24 @@
                     :x="left_panel + margin + length_scale * event_time.start" :y="job_y_bias + event_time.thread_index * (job_height + margin)"
                     style="fill:lightblue;" rx="10" ry="10"/>
                 <rect v-if="!info.is_base_partition" :width="length_scale * (event_time.end - event_time.start)" :height="job_height"
                     :x="left_panel + margin + length_scale * event_time.start" :y="job_y_bias + event_time.thread_index * (job_height + margin)"
                     style="fill:lightgreen;"/>
             </g>
             <!-- left panel -->
-            <text :x="left_panel + margin - 3" :y="job_y_bias - 20" text-anchor="end">thread index</text>
+            <text :x="left_panel + margin - 3" :y="job_y_bias - margin * 2" text-anchor="end">thread index</text>
             <g v-for="thread_index in selected_profile_statistics.max_thread_index + 1">
                 <text :x="left_panel + margin - 10" :y="job_y_bias + (thread_index - 0.5) * (job_height + margin)"
                     text-anchor="end">{{ thread_index - 1 }}</text>
             </g>
             <!-- time information -->
             <text :x="left_panel + length_scale * selected_profile.round_time" :y="margin + decoding_time_height / 2 + 5" 
                 text-anchor="end">{{ Number.parseFloat(selected_profile.round_time).toExponential(3) }} (s)</text>
             <g v-for="([event_time, info], _) in display_info_vec">
-                <text v-if="info.is_base_partition" :x="left_panel + length_scale * event_time.end"
+                <text v-if="show_unit_index && info.is_base_partition" :x="left_panel + length_scale * event_time.end"
                     :y="job_y_bias + event_time.thread_index * (job_height + margin) + job_height / 2 + 5"
                     text-anchor="end">{{ info.unit_index }}</text>
             </g>
         </svg>
     </q-scroll-area>
 </div>
 <div class="control-bar">
@@ -279,14 +279,15 @@
                 <q-slider v-model="relative_scale_log" :min="-1.2" :max="1.2" :step="0.01" snap color="deep-orange"
                     thumb-size="25px" track-size="8px"></q-slider>
             </div>
         </div>
         <div class="flex-center-div">
             <div><q-toggle color="green" v-model="thread_view" label="thread view" size="md"/></div>
             <div><q-toggle color="green" v-model="show_dependency" label="show_dependency" size="md"/></div>
+            <div><q-toggle color="green" v-model="show_unit_index" label="show_unit_index" size="md"/></div>
         </div>
         <q-card bordered class="select-info-div" v-if="selected_profile != null">
             <q-card-section class="bg-cyan text-white">
                 <div class="text-h6">Profile {{ round_select }}</div>
             </q-card-section>
             <q-separator inset></q-separator>
             <q-card-section>
@@ -408,30 +409,31 @@
             round_select: ref(null),
             round_select_label: ref(0),
             round_labels: reactive([]),
             // job select
             current_selected: ref(null),
             selected_profile: computed(() => app.round_profiles[app.round_select.value]),
             // svg configurations
-            margin: 10,
+            margin: parseInt(urlParams.get('margin') || 10),
             decoding_time_height: 20,
-            job_height: 30,
+            job_height: parseInt(urlParams.get('job_height') || 30),
             left_panel: 100,  // display text information
             job_y_bias: computed(() => app.decoding_time_height + 2 * app.margin),
             svg_width: computed(() => app.length_scale.value * app.selected_profile.value.round_time + 2 * app.margin + app.left_panel),
             svg_height: computed(() => (app.job_height + app.margin) * app.selected_profile.value.solver_profile.primal.event_time_vec.length + app.job_y_bias.value),
             base_length_scale: ref(100),  // how many pixels for each second
-            relative_scale_log: ref(0),
+            relative_scale_log: ref(parseInt(urlParams.get('relative_scale_log') || 0)),
             length_scale: computed(() => app.base_length_scale.value * Math.pow(10, app.relative_scale_log.value)),
             adaptive_scale: ref(true),
-            length_scale_selected: ref("adaptive"),
+            length_scale_selected: ref(urlParams.get('length_scale_selected') || "adaptive"),
             length_scale_options: reactive([{label:"adaptive",value:"adaptive"}
                 , {label:"1us",value:1e-6}, {label:"10us",value:1e-5}, {label:"100us",value:1e-4}
                 , {label:"1ms",value:1e-3}, {label:"10ms",value:1e-2}, {label:"100ms",value:1e-1}
                 , {label:"1s",value:1}, {label:"10s",value:10}, {label:"100s",value:100}, {label:"1000s",value:1000}]),
+            show_unit_index: ref(true),
         }
         return app
     },
     async mounted() {
         // after Vue is loaded, make the page visible
         document.documentElement.style.setProperty('--control-visibility', 'visible')
         // fetch profile
```

#### html2text {}

```diff
@@ -90,15 +90,16 @@
 width="length_scale * (event_time.end - event_time.start)" :height="job_height"
 :x="left_panel + margin + length_scale * event_time.start" :y="job_y_bias +
 event_time.thread_index * (job_height + margin)" style="fill:lightblue;"
 rx="10" ry="10"/>
 width="length_scale * (event_time.end - event_time.start)" :height="job_height"
 :x="left_panel + margin + length_scale * event_time.start" :y="job_y_bias +
 event_time.thread_index * (job_height + margin)" style="fill:lightgreen;"/>
-x="left_panel + margin - 3" :y="job_y_bias - 20" text-anchor="end">thread index
+x="left_panel + margin - 3" :y="job_y_bias - margin * 2" text-
+anchor="end">thread index
 x="left_panel + margin - 10" :y="job_y_bias + (thread_index - 0.5) *
 (job_height + margin)" text-anchor="end">{{ thread_index - 1 }}
 x="left_panel + length_scale * selected_profile.round_time" :y="margin +
 decoding_time_height / 2 + 5" text-anchor="end">{{ Number.parseFloat
 (selected_profile.round_time).toExponential(3) }} (s)
 x="left_panel + length_scale * event_time.end" :y="job_y_bias +
 event_time.thread_index * (job_height + margin) + job_height / 2 + 5" text-
```

### Comparing `fusion_blossom-0.2.2/visualize/patches.js` & `fusion_blossom-0.2.5/visualize/patches.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/primal.js` & `fusion_blossom-0.2.5/visualize/primal.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/visualize/server.py` & `fusion_blossom-0.2.5/visualize/server.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.2/PKG-INFO` & `fusion_blossom-0.2.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,163 +1,113 @@
-Metadata-Version: 2.1
-Name: fusion_blossom
-Version: 0.2.2
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet
-License-File: LICENSE
-Summary: A fast minimum-weight perfect matching solver for quantum error correction
-Keywords: QEC,quantum-computing,error-correction,visualization
-Home-Page: https://fusionblossom.com
-Author: Yue Wu <wuyue16pku@gmail.com>
-Author-email: Yue Wu <wuyue16pku@gmail.com>
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/yuewuo/fusion-blossom
-
 ![Build Status](https://jenkins.fusionblossom.com/buildStatus/icon?job=FusionBlossomBuild&subject=build&style=flat-square)
 ![Test Status](https://jenkins.fusionblossom.com/buildStatus/icon?job=FusionBlossomCI&subject=test&style=flat-square)
 <!-- ![Build Python Binding](https://github.com/yuewuo/fusion-blossom/actions/workflows/wheels.yml/badge.svg) -->
 
 # Fusion Blossom
 A fast Minimum-Weight Perfect Matching (MWPM) solver for Quantum Error Correction (QEC)
 
 Please see [our tutorial for a quick explanation and some Python demos](https://tutorial.fusionblossom.com).
 
+Our paper is out on arXiv! [https://arxiv.org/abs/2305.08307](https://arxiv.org/abs/2305.08307)
+
 ## Key Features
 
 - **Correctness**: This is an exact MWPM solver, verified against the [Blossom V library](https://pub.ist.ac.at/~vnk/software.html) with millions of randomized test cases .
-- **Linear Complexity**: The decoding time is roughly $O(N)$ given small physical error rate, proportional to the number of defect vertices $N$.
+- **Linear Complexity**: The average decoding time is roughly $O(N)$ given small physical error rate, proportional to the number of defect vertices $N$.
 - **Parallelism**: A single MWPM decoding problem can be partitioned and solved in parallel, then *fused* together to find an **exact** global MWPM solution.
-- **Simple Interface**: The graph problem is abstracted and easy-to-use for QEC applications.
+- **Simple Interface**: The graph problem is abstracted and easy-to-use for QEC applications. Especially, it supports decoding erasure errors (by setting some edge weights to 0 on the fly).
 
 ## Benchmark Highlights
 
-- In phenomenological noise model with **$p$ = 0.005**, code distance **$d$ = 21**, planar code with $d(d-1)$ = 420 $Z$ stabilizers, 100000 measurement rounds
-  - single-thread: **2.4us per defect vertex** or 29us per measurement round
-  - 64-threads: 58ns per defect vertex or **0.7us per measurement round**
+- In circuit-level noise model with **$p$ = 0.001**, code distance **$d$ = 21**, rotated CSS code, 100000 measurement rounds
+  - single-thread: **3.9us per defect vertex** or 13us per measurement round
+  - 64-threads: 95ns per defect vertex or **0.3us per measurement round**
+  - in streaming mode, the latency is **0.7ms regardless of rounds of measurement**
 
 ## Background and Key Ideas
 
 MWPM decoders are widely known for its high accuracy [[1]](#fowler2012topological) and several optimizations that further improves its accuracy [[2]](#criger2018multi). However, there weren't many publications that improve the speed of the MWPM decoder over the past 10 years. Fowler implemented an $O(N)$ asymptotic complexity MWPM decoder in [[3]](#fowler2012towards) and proposed an $O(1)$ complexity parallel MWPM decoder in [[4]](#fowler2013minimum), but none of these are publicly available to our best knowledge. Higgott implemented a fast but approximate MWPM decoder (namely "local matching") with roughly $O(N)$ complexity in [[5]](#higgott2022pymatching). With recent experiments of successful QEC on real hardware, it's time for a fast and accurate MWPM decoder to become available to the community.
 
 Our idea comes from our study on the Union-Find (UF) decoder [[6]](#delfosse2021almost). UF decoder is a fast decoder with $O(N)$ worst-case time complexity, at the cost of being less accurate compared to the MWPM decoder. Inspired by the Fowler's diagram [[3]](#fowler2012towards), we found a relationship between the UF decoder [[7]](#wu2022interpretation). This [nice animation](https://us.wuyue98.cn/aps2022/#/3/1) (press space to trigger animation) could help people see the analogy between UF and MWPM decoders. With this interpretation, we're able to combind the strength of UF and MWPM decoders together.
 
 - From the UF decoder, we learnt to use a sparse decoding graph representation for fast speed
 - From the MWPM decoder, we learnt to find an exact minimum-weight perfect matching for high accuracy
 
-We shall note that Oscar Higgott and Craig Gidney independently reach the same approach of using sparse decoding graph to solve MWPM more efficiently in PyMatching V2 [[8]](#pymatchingv2). It's impressive to see that they have much better single-thread performance than fusion-blossom (about 5x-20x speedup). They use more optimizations like priority queue and single-tree strategy that appears in existing literature of blossom algorithms  (possibly some other novel techniques, looking forward to their paper!). Also, they use C++ language rather than Rust programming language. Rust enforces memory safety which adds some runtime overhead (like vector boundary check and unnecessary locks in parallel programming). We use `unsafe` Rust to improve the speed by 1.5x-3x but these features are not yet enabled in the Python library and only available when using the native Rust library. In fact, PyMatching V2's optimizations and fusion-blossom's parallel computation (fusion operation) are compatible with each other. With their impressive work, we're looking forward to another 5x-20x speed of the parallel MWPM decoder if combined together. For now, user should use PyMatching for better CPU efficiency in large-scale simulations, and use fusion-blossom library as an educational tool with [visualization tool](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json) and [entry-level tutorials](https://tutorial.fusionblossom.com).
+We shall note that Oscar Higgott and Craig Gidney independently reach the same approach of using sparse decoding graph to solve MWPM more efficiently in PyMatching V2 [[8]](#pymatchingv2). It's impressive to see that they have much better single-thread performance than fusion-blossom (about 5x-20x speedup). They use more optimizations like priority queue that appears in existing literature of blossom algorithms (check their paper at [[9]](#higgott2023sparse)). Also, they use C++ language rather than Rust programming language. Rust enforces memory safety which adds some runtime overhead (like vector boundary check and unnecessary locks in parallel programming). We use `unsafe` Rust to improve the speed by 1.5x-3x but these features are not yet enabled in the Python library and only available when using the native Rust library. In fact, PyMatching V2's optimizations and fusion-blossom's parallel computation (fusion operation) are compatible with each other. With their impressive work, we're looking forward to another 5x-20x speed of the parallel MWPM decoder if combined together. For now, user should use PyMatching for better CPU efficiency in large-scale simulations, and use fusion-blossom library as an educational tool with [visualization tool](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json) and [entry-level tutorials](https://tutorial.fusionblossom.com).
 
 ## Demo
 
 We highly suggest you watch through several demos here to get a sense of how the algorithm works. All our demos are captured from real algorithm execution. In fact, we're showing you the visualized debugger tool we wrote for fusion blossom. The demo is a 3D website and you can control the view point as you like.
 
-For more details of why it finds an exact MWPM, please read our paper [coming soon 💪].
-
 Click the demo image below to view the corresponding demo
 
 #### Serial Execution
 
-[<img src="https://visualize.fusionblossom.com/img/serial_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_1.json)
-[<img src="https://visualize.fusionblossom.com/img/serial_example.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json)
-[<img src="https://visualize.fusionblossom.com/img/serial_random.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_11.json)
+[<img src="./visualize/img/serial_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_1.json)
+[<img src="./visualize/img/serial_example.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_10.json)
+[<img src="./visualize/img/serial_random.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_serial_basic_11.json)
 
 #### Parallel Execution (Shown in Serial For Better Visual)
 
-[<img src="https://visualize.fusionblossom.com/img/parallel_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_parallel_basic_3.json)
-[<img src="https://visualize.fusionblossom.com/img/parallel_phenomenological.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_1.json)
-[<img src="https://visualize.fusionblossom.com/img/parallel_circuit_level.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_2.json)
+[<img src="./visualize/img/parallel_simple.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=primal_module_parallel_basic_3.json)
+[<img src="./visualize/img/parallel_phenomenological.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_1.json)
+[<img src="./visualize/img/parallel_circuit_level.png" width="30%"/>](https://visualize.fusionblossom.com/?filename=example_partition_demo_2.json)
 
 ## Usage
 
-Our code is written in [Rust](https://www.rust-lang.org/) programming language for speed and memory safety, but it's hardly a easy language to learn. To make the decoder more accessible, we bind the library to Python and user can simply install the library using `pip3 install fusion-blossom`.
+Our code is written in [Rust](https://www.rust-lang.org/) programming language for speed and memory safety, but it's hardly an easy language to learn. To make the decoder more accessible, we bind the library to Python and user can simply install the library using `pip3 install fusion-blossom`.
 
 We have several Python demos at [the tutorial website](https://tutorial.fusionblossom.com/demo/example-qec-codes.html) . Also there is a simple example for decoder, and you can run it by cloning the project and run `python3 scripts/demo.py`.
 
-For parallel solver, it needs user to provide a partition strategy. Please wait for our paper for a thorough description of how partition works.
-
-## Evaluation
-
-We use Intel(R) Xeon(R) Platinum 8375C CPU for evaluation, with 64 physical cores and 128 threads. Note that Apple m1max CPU has roughly 2x single-core decoding speed, but it has limited number of cores so we do not use data from m1max. The benchmark scripts can be found in `benchmark` folder, running in Rust native binary (not the Python package, which has fewer optimization features enabled). By default, we test phenomenological noise model with **$p$ = 0.005**, code distance **$d$ = 21**, planar code with $d(d-1)$ = 420 $Z$ stabilizers, 100000 measurement rounds.
-
-First of all, the number of partitions will effect the speed. Intuitively, the more partitions there are, the more overhead because fusing two partitions consumes more computation than solving them as a whole. But in practice, memory access is not always at the same speed. If cache cannot hold the data, then solving big partition may consume even more time than solving small ones. We test on a single-thread decoder, and try different partition numbers. At partition number = 2000, we get roughly the minimum decoding time of 2.4us per defect vertex. This corresponds to each partition hosting 50 measurement rounds (decoding blocks of 49 * 21 * 20).
-
-![](https://visualize.fusionblossom.com/data/benchmark/paper_parallel_fusion_blossom/partition_num_single_thread_2_tree/decoding_time_per_defect.svg)
-
-Given the optimal partition number of a single thread, we keep the partition number the same and try increasing the number of threads. Note that the partition number may not be optimal for large number of threads, but even in this case, we reach 41x speed up given 64 physical cores. The decoding time is pushed to 58ns per sydnrome or 0.7us per measurement round. This can catch up with the 1us measurement round of a superconducting circuit. Interestingly, we found that hyperthreading won't help much in this case, perhaps because this decoder is memory-bounded, meaning memory throughput is the bottleneck. Although the number of defect vertices is only a small portion, they are randomly distributed so every time a new syndrome is given, the memory is almost always cold and incur large cache miss panelty.
-
-![](https://visualize.fusionblossom.com/data/benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/decoding_time_per_defect.svg)
-
-In order to understand the bottleneck of  parallel execution, we wrote a visualization tool to display the execution windows of base partitions and fusion operations on multiple threads. Blue blocks is the base partition and green blocks is the fusion operation. Fusion operation only scales with the size of the fusion boundary and the depth of active partitions, irrelevant to the base partition's size. We'll study different partition and fusion strategies in our paper. Below shows the parallel execution on 64 threads. Blue blocks are base partitions, each is a 49 * 21 * 20 decoding graph block. Green blocks are fusion blocks, each is a 1 * 21 * 20 decoding graph block sandwiched by two neighbor base partitions. You can click the image which jumps to this interactive visualization tool.
-
-[<img src="https://visualize.fusionblossom.com/data/benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/64.svg"/>](https://visualize.fusionblossom.com/partition-profile.html?filename=benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/tmp/64.profile)
+For parallel solver, it needs user to provide a partition strategy. Please check our paper for a thorough description of how partition works.
 
 ## Interface
 
 #### Sparse Decoding Graph and Integer Weights
 
 The weights in QEC decoding graph are computed by taking the log of error probability, e.g. $w_e = \log\{(1-p)/p\}$ or roughly $w_e = -\log{p}$, we can safely use integers to save weights by e.g. multiplying the weights by 1e6 and truncate to nearest integer. In this way, the truncation error $\Delta w_e = 1$ of integer weights corresponds to relative error $\Delta p /{p}=10^{-6}$ which is small enough. Suppose physical error rate $p$ is in the range of a positive `f64` variable (2.2e-308 to 1), the maximum weight is 7e7,which is well below the maximum value of a `u32` variable (4.3e9). Since weights only sum up in our algorithm (no multiplication), `u32` is large enough and accurate enough. By default we use `usize` which is platform dependent (usually 64 bits), but you can 
 
 We use integer also for ease of migrating to FPGA implementation. In order to fit more vertices into a single FPGA, it's necessary to reduce the resource usage for each vertex. Integers are much cheaper than floating-point numbers, and also it allows flexible trade-off between resource usage and accuracy, e.g. if all weights are equal, we can simply use a 2 bit integer.
 
 Note that other libraries of MWPM solver like [Blossom V](https://doi.org/10.1007/s12532-009-0002-8) also default to integer weights as well. Although one can change the macro to use floating-point weights, it's not recommended because "the code may even get stuck due to rounding errors".
 
-## Installation
-
-Here is an example installation on Ubuntu20.04.
-
-```sh
-# install rust compiler and package manager
-curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
-# install build dependencies
-sudo apt install build-essential
-```
-
 ## Tests
 
-In order to test the correctness of our MWPM solver, we need a ground-truth MWPM solver. [Blossom V](https://doi.org/10.1007/s12532-009-0002-8) is widely-used in existing MWPM decoders, but according to the license we cannot embed it in this library. To run the test cases with ground truth comparison or enable the functions like `blossom_v_mwpm`, you need to download this library [at this website](https://pub.ist.ac.at/~vnk/software.html) to a folder named `blossomV` at the root directory of this git repo.
+In order to test the correctness of our MWPM solver, we need a ground-truth MWPM solver. [Blossom V](https://doi.org/10.1007/s12532-009-0002-8) is widely-used in existing MWPM decoders, but according to the license we cannot embed it in this library.To run the test cases with ground truth comparison or enable the functions like `blossom_v_mwpm`, you need to download this library [at this website](https://pub.ist.ac.at/~vnk/software.html) to a folder named `blossomV` at the root directory of this git repo.
 
 ```shell
 wget -c https://pub.ist.ac.at/~vnk/software/blossom5-v2.05.src.tar.gz -O - | tar -xz
 cp -r blossom5-v2.05.src/* blossomV/
 rm -r blossom5-v2.05.src
 ```
 
-# Visualize
+# Visualization
+
+## Visualize the solving procedure of a single decoding problem
 
 To start a server, run the following
 ```sh
 cd visualize
-npm install  # to download packages
-# you can choose to render locally or to view it in a browser interactively
-# interactive: open url using a browser (Chrome recommended)
-node index.js <url> <width> <height>  # local render
+python3 server.py  # server
 
-# for example you can run the following command to get url
+# to view it in a browser interactively, you can run the following command to get url
 cd ..
 cargo test visualize_paper_weighted_union_find_decoder -- --nocapture
+
+# alternatively, you can choose to render locally
+npm install  # to download packages
+node index.js <url> <width> <height>  # local render
 ```
 
+## Visualize parallel execution of multiple decoding problems
+
+In order to understand the bottleneck of  parallel execution, we wrote a visualization tool to display the execution windows of base partitions and fusion operations on multiple threads. Fusion operation only scales with the size of the fusion boundary and the depth of active partitions, irrelevant to the base partition's size. We study different partition and fusion strategies in our paper. Below shows the parallel execution on 64 threads. Blue blocks are base partitions, each consists of 49 rounds of measurement. Green blocks are fusion operations, a single round of measurement sandwiched by two neighbor base partitions. You can click the image which jumps to this interactive visualization tool.
+
+[<img src="./benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/64.svg"/>](https://visualize.fusionblossom.com/partition-profile.html?filename=benchmark/paper_parallel_fusion_blossom/thread_pool_size_partition_2k/tmp/64.profile)
+
 # TODOs
 
 - [ ] support erasures in parallel solver
 
 # Acknowledgements
 
 This project is funded by [NSF MRI: Development of PARAGON: Control Instrument for Post NISQ Quantum Computing](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2216030)
@@ -176,8 +126,9 @@
 
 <a id="delfosse2021almost">[6]</a> Delfosse, Nicolas, and Naomi H. Nickerson. "Almost-linear time decoding algorithm for topological codes." Quantum 5 (2021): 595.
 
 <a id="wu2022interpretation">[7]</a> Wu, Yue. APS 2022 March Meeting Talk "Interpretation of Union-Find Decoder on Weighted Graphs and Application to XZZX Surface Code". Slides: [https://us.wuyue98.cn/aps2022](https://us.wuyue98.cn/aps2022), Video: [https://youtu.be/BbhqUHKPdQk](https://youtu.be/BbhqUHKPdQk)
 
 <a id="pymatchingv2">[8]</a> Higgott, Oscar. PyMatching v2 https://github.com/oscarhiggott/PyMatching
 
+<a id="higgott2023sparse">[9]</a> Higgott, Oscar, and Craig Gidney. "Sparse Blossom: correcting a million errors per core second with minimum-weight matching." arXiv preprint arXiv:2303.15933 (2023).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

