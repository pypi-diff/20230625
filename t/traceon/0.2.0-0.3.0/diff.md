# Comparing `tmp/traceon-0.2.0.tar.gz` & `tmp/traceon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceon-0.2.0.tar", last modified: Sun Apr  9 21:05:32 2023, max compression
+gzip compressed data, was "traceon-0.3.0.tar", last modified: Sun Jun 25 20:18:33 2023, max compression
```

## Comparing `traceon-0.2.0.tar` & `traceon-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.803852 traceon-0.2.0/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    34524 2023-03-21 09:42:58.000000 traceon-0.2.0/LICENSE.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       27 2023-04-09 12:34:12.000000 traceon-0.2.0/MANIFEST.in
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3542 2023-04-09 21:05:32.803852 traceon-0.2.0/PKG-INFO
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2380 2023-04-09 12:34:12.000000 traceon-0.2.0/README.md
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       38 2023-04-09 21:05:32.803852 traceon-0.2.0/setup.cfg
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     1435 2023-04-09 21:04:38.000000 traceon-0.2.0/setup.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.799852 traceon-0.2.0/traceon/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2764 2023-04-09 13:50:35.000000 traceon-0.2.0/traceon/__init__.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.799852 traceon-0.2.0/traceon/backend/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    16334 2023-04-09 21:01:54.000000 traceon-0.2.0/traceon/backend/__init__.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    43174 2023-04-09 20:53:56.000000 traceon-0.2.0/traceon/backend/traceon-backend.c
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.803852 traceon-0.2.0/traceon/data/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)  1023104 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8128 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/data/radial-series-3D-thetas.npy
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8406 2023-04-09 13:45:50.000000 traceon-0.2.0/traceon/excitation.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    13830 2023-04-09 13:28:24.000000 traceon-0.2.0/traceon/geometry.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     6781 2023-04-09 13:28:24.000000 traceon-0.2.0/traceon/plotting.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    26699 2023-04-09 13:41:52.000000 traceon-0.2.0/traceon/solver.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8192 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/tracing.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2204 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/util.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.799852 traceon-0.2.0/traceon.egg-info/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3542 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/PKG-INFO
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)      497 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/SOURCES.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)        1 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/dependency_links.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       48 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/requires.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)        8 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/top_level.txt
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.757537 traceon-0.3.0/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    34524 2023-03-21 09:42:58.000000 traceon-0.3.0/LICENSE.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       27 2023-04-09 12:34:12.000000 traceon-0.3.0/MANIFEST.in
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3838 2023-06-25 20:18:33.757537 traceon-0.3.0/PKG-INFO
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2628 2023-06-03 10:58:58.000000 traceon-0.3.0/README.md
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       38 2023-06-25 20:18:33.757537 traceon-0.3.0/setup.cfg
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     1818 2023-06-25 20:08:19.000000 traceon-0.3.0/setup.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.749536 traceon-0.3.0/traceon/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2876 2023-06-03 11:00:26.000000 traceon-0.3.0/traceon/__init__.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.749536 traceon-0.3.0/traceon/backend/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    19456 2023-06-25 19:37:04.000000 traceon-0.3.0/traceon/backend/__init__.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    46186 2023-06-25 20:09:32.000000 traceon-0.3.0/traceon/backend/traceon-backend.c
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.753536 traceon-0.3.0/traceon/data/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)  1023104 2023-04-09 12:34:12.000000 traceon-0.3.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8128 2023-04-09 12:34:12.000000 traceon-0.3.0/traceon/data/radial-series-3D-thetas.npy
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     9224 2023-06-25 19:56:56.000000 traceon-0.3.0/traceon/excitation.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    18750 2023-06-25 20:02:06.000000 traceon-0.3.0/traceon/geometry.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8160 2023-06-25 11:54:05.000000 traceon-0.3.0/traceon/plotting.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    27673 2023-06-25 20:04:57.000000 traceon-0.3.0/traceon/solver.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    11829 2023-06-25 19:49:23.000000 traceon-0.3.0/traceon/tracing.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2204 2023-05-20 08:55:03.000000 traceon-0.3.0/traceon/util.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.749536 traceon-0.3.0/traceon.egg-info/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3838 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/PKG-INFO
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)      497 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/SOURCES.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)        1 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/dependency_links.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       53 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/requires.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)        8 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/top_level.txt
```

### Comparing `traceon-0.2.0/LICENSE.txt` & `traceon-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `traceon-0.2.0/PKG-INFO` & `traceon-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceon
-Version: 0.2.0
+Version: 0.3.0
 Summary: Solver and tracer for electrostatic problems
 Home-page: https://github.com/leon-vv/Traceon
 Author: Léon van Velzen
 Author-email: leonvanvelzen@protonmail.com
 License: AGPLv3
 Project-URL: Documentation, https://leon.science/traceon
 Project-URL: Code, https://github.com/leon-vv/traceon
@@ -22,15 +22,15 @@
         [API documentation](https://leon.science/traceon/index.html)
         
         ## Citation
         
         Please cite the software as follows:
         
         ```
-        L.B. van Velzen. Traceon software (version 0.1.3). 2023. https://doi.org/10.5281/zenodo.7773697
+        L.B. van Velzen. Traceon software (version 0.2.0). 2023. https://doi.org/10.5281/zenodo.7812232
         ```
         
         ## Installation
         
         Install using the Python package manager:
         ```
         pip install traceon
@@ -62,14 +62,20 @@
         
         ## Gallery
         
         ![Image of 3D deflector](https://raw.githubusercontent.com/leon-vv/traceon/main/images/deflector-image.png)
         
         ## Features
         
+        v0.2.0:
+        - Use higher order charge distribution on line elements in radial symmetry
+        - Use higher order line elements (polynomials) in radial symmetry
+        - Better integration techniques, especially with regards to the logarithmic singularities
+        
+        v0.1.0:
         - Uses the powerful [GMSH library](https://gmsh.info/) for meshing
         - Solve for surface charge distribution using BEM
         - General 3D geometries and radially symmetric geometries
         - Dielectrics
         - Floating conductors
         - Accurate electron tracing using adaptive time steps
         - Field/potential calculation by integration over surface charges
```

### Comparing `traceon-0.2.0/README.md` & `traceon-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [API documentation](https://leon.science/traceon/index.html)
 
 ## Citation
 
 Please cite the software as follows:
 
 ```
-L.B. van Velzen. Traceon software (version 0.1.3). 2023. https://doi.org/10.5281/zenodo.7773697
+L.B. van Velzen. Traceon software (version 0.2.0). 2023. https://doi.org/10.5281/zenodo.7812232
 ```
 
 ## Installation
 
 Install using the Python package manager:
 ```
 pip install traceon
@@ -51,14 +51,20 @@
 
 ## Gallery
 
 ![Image of 3D deflector](https://raw.githubusercontent.com/leon-vv/traceon/main/images/deflector-image.png)
 
 ## Features
 
+v0.2.0:
+- Use higher order charge distribution on line elements in radial symmetry
+- Use higher order line elements (polynomials) in radial symmetry
+- Better integration techniques, especially with regards to the logarithmic singularities
+
+v0.1.0:
 - Uses the powerful [GMSH library](https://gmsh.info/) for meshing
 - Solve for surface charge distribution using BEM
 - General 3D geometries and radially symmetric geometries
 - Dielectrics
 - Floating conductors
 - Accurate electron tracing using adaptive time steps
 - Field/potential calculation by integration over surface charges
```

### Comparing `traceon-0.2.0/setup.py` & `traceon-0.3.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 from setuptools import setup, Extension
 import platform
 
+VCPKG_DIR = 'C:\\Users\\leonv\\vcpkg'
 
 if platform.system() in ['Linux', 'Darwin']:
-    compiler_kwargs = dict(extra_compile_args=['-O3', '-mavx', '-ffast-math'], extra_link_args=['-lm'])
+    compiler_kwargs = dict(extra_compile_args=['-O3', '-mavx', '-ffast-math', '-DNDEBUG'], extra_link_args=['-lm', '-lgsl'])
+    extra_objects = []
+    include_dirs = []
 elif platform.system() == 'Windows':
-    compiler_kwargs = dict(extra_compile_args=['/fp:fast', '/Ox', '/Ob3', '/Oi', '/GL', '/arch:AVX'])
+    compiler_kwargs = dict(extra_compile_args=['/fp:fast', '/Ox', '/Ob3', '/Oi', '/GL', '/arch:AVX', '-I .\\traceon\\backend\\'])
+    extra_objects = [VCPKG_DIR + '\\packages\\gsl_x64-windows-static-release\\lib\\gsl.lib']
+    include_dirs = VCPKG_DIR + '\\packages\\gsl_x64-windows-static-release\\include'
 
 
 backend_extension = Extension(
     name='traceon.backend.traceon_backend',
     sources=['traceon/backend/traceon-backend.c'],
+    extra_objects=extra_objects,
     **compiler_kwargs)
 
 setup(
     name='traceon',
-    version='0.2.0',
+    version='0.3.0',
     description='Solver and tracer for electrostatic problems',
     url='https://github.com/leon-vv/Traceon',
     author='Léon van Velzen',
     author_email='leonvanvelzen@protonmail.com',
     keywords=['boundary element method', 'BEM', 'electrostatic', 'electromagnetic', 'electron microscope', 'electron', 'tracing', 'particle', 'tracer', 'electron optics'],
     license='AGPLv3',
     ext_modules=[backend_extension],
     packages=['traceon', 'traceon.backend'],
     include_package_data=True,
     long_description = open('README.md').read(),
     long_description_content_type='text/markdown',
-    install_requires=['matplotlib', 'numpy', 'gmsh>=4.9', 'pygmsh>=7.1.13', 'scipy'],
+    install_requires=['matplotlib', 'vedo', 'numpy', 'gmsh>=4.9', 'pygmsh>=7.1.13', 'scipy'],
     project_urls = {
         'Documentation': "https://leon.science/traceon",
         'Code': "https://github.com/leon-vv/traceon",
         'Issues': "https://github.com/leon-vv/traceon/issues"
-    }
+    },
+    include_dirs=include_dirs,
 )
```

### Comparing `traceon-0.2.0/traceon/__init__.py` & `traceon-0.3.0/traceon/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,18 @@
 |                	|          	|
 
 To keep the charge values from becoming very small, the charge values are always saved as \( \\frac{ \\sigma}{ \\epsilon_0 \\pi} \). Since this term appears
 in the formulas for the potential (and thus also in the formulas for the electric field) the actual \( \\sigma \) values themselves are never computed.
 
 """
 
+import warnings
+
 __pdoc__ = {}
 __pdoc__['traceon.util'] = False
 __pdoc__['traceon.backend'] = False
 __pdoc__['traceon.data'] = False
 __pdoc__['traceon.tracing.Tracer.__call__'] = True
 
+warnings.filterwarnings('ignore', '.*The value of the smallest subnormal for.* type is zero.')
```

### Comparing `traceon-0.2.0/traceon/backend/__init__.py` & `traceon-0.3.0/traceon/backend/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,79 +38,92 @@
 
 
 TRACING_BLOCK_SIZE = C.c_size_t.in_dll(backend_lib, 'TRACING_BLOCK_SIZE').value
 
 DERIV_2D_MAX = C.c_int.in_dll(backend_lib, 'DERIV_2D_MAX_SYM').value
 
 N_QUAD_2D = C.c_int.in_dll(backend_lib, 'N_QUAD_2D_SYM').value
+N_TRIANGLE_QUAD = C.c_int.in_dll(backend_lib, 'N_TRIANGLE_QUAD_SYM').value
 
 NU_MAX = C.c_int.in_dll(backend_lib, 'NU_MAX_SYM').value
 M_MAX = C.c_int.in_dll(backend_lib, 'M_MAX_SYM').value
 
 # Pass numpy array to C
 def arr(*args, dtype=np.float64, **kwargs):
     return ndpointer(*args, dtype=dtype, flags=('C_CONTIGUOUS', 'ALIGNED'), **kwargs);
 
 # Pass one dimensional Numpy array to C
 v2 = arr(shape=(2,))
 v3 = arr(shape=(3,))
 
 dbl = C.c_double
+dbl_p = C.POINTER(dbl)
 vp = C.c_void_p
 sz = C.c_size_t
 
 integration_cb_2d = C.CFUNCTYPE(dbl, dbl, dbl, dbl, dbl, vp)
 integration_cb_3d = C.CFUNCTYPE(dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp)
 field_fun = C.CFUNCTYPE(None, C.POINTER(dbl), C.POINTER(dbl), vp);
 
 vertices = arr(ndim=3)
 lines = arr(ndim=3)
 charges_3d = arr(ndim=1)
-charges_2d = arr(ndim=2)
+charges_2d = arr(ndim=1)
 z_values = arr(ndim=1)
 
+jac_buffer_3d = arr(ndim=2)
+pos_buffer_3d = arr(ndim=3)
+
+jac_buffer_2d = arr(ndim=2)
+pos_buffer_2d = arr(ndim=3)
+
 bounds = arr(shape=(3, 2))
 
 times_block = arr(shape=(TRACING_BLOCK_SIZE,))
 tracing_block = arr(shape=(TRACING_BLOCK_SIZE, 6))
 
 backend_functions = {
+    'ellipkm1' : (dbl, dbl),
     'ellipk' : (dbl, dbl),
+    'ellipem1' : (dbl, dbl),
     'ellipe': (dbl, dbl),
     'normal_2d': (None, v2, v2, v2),
-    'normal_3d': (None, v3, v3, v3),
-    'triangle_integral': (dbl, v3, v3, v3, v3, integration_cb_3d, C.c_void_p),
+    'higher_order_normal_radial': (None, dbl, v2, v2, v2, v2, v2),
+    'normal_3d': (None, v3, v3, v3, v3),
+    'position_and_jacobian_3d': (None, dbl, dbl, arr(ndim=2), v3, dbl_p),
+    'position_and_jacobian_radial': (None, dbl, v2, v2, v2, v2, v2, dbl_p),
     'trace_particle': (sz, times_block, tracing_block, field_fun, bounds, dbl, vp),
     'potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
     'dr1_potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
     'dz1_potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
-    'axial_derivatives_radial_ring': (None, arr(ndim=2), lines, charges_2d, sz, z_values, sz),
-    'potential_radial': (dbl, v3, vertices, charges_2d, sz),
+    'axial_derivatives_radial_ring': (None, arr(ndim=2), charges_2d, jac_buffer_2d, pos_buffer_2d, sz, z_values, sz),
+    'potential_radial': (dbl, v3, charges_2d, jac_buffer_2d, pos_buffer_2d, sz),
     'potential_radial_derivs': (dbl, v2, z_values, arr(ndim=3), sz),
-    'charge_radial': (dbl, arr(ndim=2), arr(ndim=1)),
-    'field_radial': (None, v3, v3, vertices, charges_2d, sz),
-    'trace_particle_radial': (sz, times_block, tracing_block, bounds, dbl, vertices, charges_2d, sz),
+    'charge_radial': (dbl, arr(ndim=2), dbl),
+    'field_radial': (None, v3, v3, charges_2d, jac_buffer_2d, pos_buffer_2d, sz),
+    'trace_particle_radial': (sz, times_block, tracing_block, bounds, dbl, charges_2d, jac_buffer_2d, pos_buffer_2d, sz, dbl_p),
     'field_radial_derivs': (None, v3, v3, z_values, arr(ndim=3), sz),
     'trace_particle_radial_derivs': (sz, times_block, tracing_block, bounds, dbl, z_values, arr(ndim=3), sz),
     'dx1_potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
     'dy1_potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
     'dz1_potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
     'potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
-    'axial_coefficients_3d': (None, vertices, charges_3d, sz, z_values, arr(ndim=4), sz, arr(ndim=1), arr(ndim=4), sz),
-    'potential_3d': (dbl, v3, vertices, charges_3d, sz),
+    'axial_coefficients_3d': (None, charges_3d, jac_buffer_3d, pos_buffer_3d, sz, z_values, arr(ndim=4), sz, arr(ndim=1), arr(ndim=4), sz),
+    'potential_3d': (dbl, v3, charges_3d, jac_buffer_3d, pos_buffer_3d, sz),
     'potential_3d_derivs': (dbl, v3, z_values, arr(ndim=5), sz),
-    'field_3d': (None, v3, v3, vertices, charges_3d, sz),
-    'trace_particle_3d': (sz, times_block, tracing_block, bounds, dbl, vertices, charges_3d, sz),
+    'field_3d': (None, v3, v3, charges_3d, jac_buffer_3d, pos_buffer_3d, sz),
+    'trace_particle_3d': (sz, times_block, tracing_block, bounds, dbl, charges_3d, jac_buffer_3d, pos_buffer_3d, sz, dbl_p),
     'field_3d_derivs': (None, v3, v3, z_values, arr(ndim=5), sz),
     'trace_particle_3d_derivs': (sz, times_block, tracing_block, bounds, dbl, z_values, arr(ndim=5), sz),
-    'add_floating_conductor_constraints_radial': (None, arr(ndim=2), lines, sz, arr(dtype=np.int64), sz, sz),
-    'fill_matrix_radial': (None, arr(ndim=2), lines, arr(dtype=C.c_uint8, ndim=1), arr(ndim=1), sz, sz, C.c_int, C.c_int),
-    'fill_matrix_3d': (None, arr(ndim=2), vertices, arr(dtype=C.c_uint8, ndim=1), arr(ndim=1), sz, sz, C.c_int, C.c_int),
-    'xy_plane_intersection_2d': (C.c_bool, arr(ndim=2), sz, arr(shape=(4,)), dbl),
-    'xy_plane_intersection_3d': (C.c_bool, arr(ndim=2), sz, arr(shape=(6,)), dbl)
+    'fill_jacobian_buffer_radial': (None, jac_buffer_2d, pos_buffer_2d, vertices, sz),
+    'fill_matrix_radial': (None, arr(ndim=2), lines, arr(dtype=C.c_uint8, ndim=1), arr(ndim=1), jac_buffer_2d, pos_buffer_2d, sz, sz, C.c_int, C.c_int),
+    'fill_jacobian_buffer_3d': (None, jac_buffer_3d, pos_buffer_3d, vertices, sz),
+    'fill_matrix_3d': (None, arr(ndim=2), vertices, arr(dtype=C.c_uint8, ndim=1), arr(ndim=1), jac_buffer_3d, pos_buffer_3d, sz, sz, C.c_int, C.c_int),
+    'plane_intersection': (bool, v3, v3, arr(ndim=2), sz, arr(shape=(6,))),
+    'line_intersection': (bool, v2, v2, arr(ndim=2), sz, arr(shape=(4,)))
 }
 
 
 for (fun, (res, *args)) in backend_functions.items():
     libfun = getattr(backend_lib, fun)
 
     def backend_check_numpy_requirements_wrapper(*args, _cfun_reference=libfun, _cfun_name=fun):
@@ -130,37 +143,41 @@
         return _cfun_reference(*new_args)
       
     setattr(backend_lib, fun, backend_check_numpy_requirements_wrapper)
      
     libfun.restype = res
     libfun.argtypes = args
 
+ellipkm1 = np.frompyfunc(backend_lib.ellipkm1, 1, 1)
 ellipk = np.frompyfunc(backend_lib.ellipk, 1, 1)
+ellipem1 = np.frompyfunc(backend_lib.ellipem1, 1, 1)
 ellipe = np.frompyfunc(backend_lib.ellipe, 1, 1)
 
+def higher_order_normal_radial(alpha, vertices):
+    normal = np.zeros(2)
+    backend_lib.higher_order_normal_radial(alpha, vertices[0, :2], vertices[2, :2], vertices[3, :2], vertices[1, :2], normal)
+    assert np.isclose(np.linalg.norm(normal), 1.0)
+    return normal
+    
 def normal_2d(p1, p2):
     normal = np.zeros( (2,) )
     backend_lib.normal_2d(p1, p2, normal)
     return normal
 
 # Remove the last argument, which is usually a void pointer to optional data
 # passed to the function. In Python we don't need this functionality
 # as we can simply use closures.
 def remove_arg(fun):
     return lambda *args: fun(*args[:-1])
 
 def normal_3d(p1, p2, p3):
     normal = np.zeros( (3,) )
-    backend_lib.normal_2d(p1, p2, normal)
+    backend_lib.normal_3d(p1, p2, p3, normal)
     return normal
    
-def triangle_integral(point, v1, v2, v3, callback):
-    assert point.shape == (3,) and v1.shape == (3,) and v2.shape == (3,) and v3.shape == (3,)
-    return backend_lib.triangle_integral(point, v1, v2, v3, integration_cb_3d(remove_arg(callback)), None)
-
 def _vec_2d_to_3d(vec):
     assert vec.shape == (2,) or vec.shape == (3,)
      
     if vec.shape == (2,):
         return np.array([vec[0], vec[1], 0.0])
     
     return vec
@@ -211,30 +228,60 @@
         assert field.shape == (3,)
         result[0] = field[0]
         result[1] = field[1]
         result[2] = field[2]
     
     return field_fun(wrapper)
 
+def position_and_jacobian_3d(alpha, beta, triangle):
+    assert triangle.shape == (6, 3)
+     
+    pos = np.zeros(3)
+    jac = C.c_double(0.0)
+     
+    backend_lib.position_and_jacobian_3d(alpha, beta, triangle, pos, C.pointer(jac))
+        
+    return jac.value, pos
+
+
+def position_and_jacobian_radial(alpha, v1, v2, v3, v4):
+    assert v1.shape == (2,) or v1.shape == (3,)
+    assert v2.shape == (2,) or v2.shape == (3,)
+    assert v3.shape == (2,) or v3.shape == (3,)
+    assert v4.shape == (2,) or v4.shape == (3,)
+    
+    pos = np.zeros(2)
+    jac = C.c_double(0.0)
+     
+    backend_lib.position_and_jacobian_radial(alpha, v1[:2], v2[:2], v3[:2], v4[:2], pos, C.pointer(jac))
+    
+    return jac.value, pos
+
+
 def trace_particle(position, velocity, field, bounds, atol):
     bounds = np.array(bounds)
     
     return trace_particle_wrapper(position, velocity,
         lambda T, P: backend_lib.trace_particle(T, P, wrap_field_fun(field), bounds, atol, None))
 
-def trace_particle_radial(position, velocity, bounds, atol, vertices, charges):
-    assert vertices.shape == (len(charges), 4, 3)
-    assert charges.shape == (len(charges), N_QUAD_2D)
-    bounds = np.array(bounds)
+def trace_particle_radial(position, velocity, bounds, atol, charges, jac_buffer, pos_buffer, field_bounds=None):
+    assert jac_buffer.shape == (len(charges), N_QUAD_2D)
+    assert pos_buffer.shape == (len(charges), N_QUAD_2D, 2)
+    assert charges.shape == (len(charges),)
+    assert field_bounds is None or field_bounds.shape == (2,2)
     
+    bounds = np.array(bounds)
+     
     if bounds.shape[0] == 2:
         bounds = np.array([bounds[0], bounds[1], [-1.0, 0.0]])
+
+    field_bounds = field_bounds.ctypes.data_as(dbl_p) if field_bounds is not None else None
      
     times, positions = trace_particle_wrapper(position, velocity,
-        lambda T, P: backend_lib.trace_particle_radial(T, P, bounds, atol, vertices, charges, len(charges)))
+        lambda T, P: backend_lib.trace_particle_radial(T, P, bounds, atol, charges, jac_buffer, pos_buffer, len(charges), field_bounds))
     
     return times, positions[:, [0,1,3,4]]
 
 def trace_particle_radial_derivs(position, velocity, bounds, atol, z, coeffs):
     assert coeffs.shape == (len(z)-1, DERIV_2D_MAX, 6)
     bounds = np.array(bounds)
 
@@ -242,178 +289,197 @@
         bounds = np.array([bounds[0], bounds[1], [-1.0, 0.0]])
     
     times, positions = trace_particle_wrapper(position, velocity,
         lambda T, P: backend_lib.trace_particle_radial_derivs(T, P, bounds, atol, z, coeffs, len(z)))
     
     return times, positions[:, [0,1,3,4]]
 
-def trace_particle_3d(position, velocity, bounds, atol, vertices, charges):
+def trace_particle_3d(position, velocity, bounds, atol, charges, jac_buffer, pos_buffer, field_bounds=None):
+    N = len(charges)
     assert position.shape == (3,)
     assert velocity.shape == (3,)
-    assert vertices.shape == (len(charges), 3, 3)
+    assert jac_buffer.shape == (N, N_TRIANGLE_QUAD)
+    assert pos_buffer.shape == (N, N_TRIANGLE_QUAD, 3)
+    assert field_bounds is None or field_bounds.shape == (3,2)
+    
     bounds = np.array(bounds)
     
+    field_bounds = field_bounds.ctypes.data_as(dbl_p) if field_bounds is not None else None
+     
     return trace_particle_wrapper(position, velocity,
-        lambda T, P: backend_lib.trace_particle_3d(T, P, bounds, atol, vertices, charges, len(charges)))
+        lambda T, P: backend_lib.trace_particle_3d(T, P, bounds, atol, charges, jac_buffer, pos_buffer, len(charges), field_bounds))
 
 def trace_particle_3d_derivs(position, velocity, bounds, atol, z, coeffs):
     assert position.shape == (3,)
     assert velocity.shape == (3,)
     assert coeffs.shape == (len(z)-1, 2, NU_MAX, M_MAX, 4)
     bounds = np.array(bounds)
      
     return trace_particle_wrapper(position, velocity,
         lambda T, P: backend_lib.trace_particle_3d_derivs(T, P, bounds, atol, z, coeffs, len(z)))
 
 potential_radial_ring = lambda *args: backend_lib.potential_radial_ring(*args, None)
 dr1_potential_radial_ring = lambda *args: backend_lib.dr1_potential_radial_ring(*args, None)
 dz1_potential_radial_ring = lambda *args: backend_lib.dz1_potential_radial_ring(*args, None)
 
-def axial_derivatives_radial_ring(z, lines, charges):
+def axial_derivatives_radial_ring(z, charges, jac_buffer, pos_buffer):
     derivs = np.zeros( (z.size, DERIV_2D_MAX) )
-    assert lines.shape == (len(charges), 4, 3)
-    assert len(lines) == len(charges)
-    assert charges.shape == (len(charges), N_QUAD_2D)
     
-    backend_lib.axial_derivatives_radial_ring(derivs, lines, charges, len(lines), z, len(z))
+    assert jac_buffer.shape == (len(charges), N_QUAD_2D)
+    assert pos_buffer.shape == (len(charges), N_QUAD_2D, 2)
+    assert charges.shape == (len(charges),)
+     
+    backend_lib.axial_derivatives_radial_ring(derivs,charges, jac_buffer, pos_buffer, len(charges), z, len(z))
     return derivs
 
-def potential_radial(point, vertices, charges):
+def potential_radial(point, charges, jac_buffer, pos_buffer):
     point = _vec_2d_to_3d(point)
-    assert vertices.shape == (len(charges), 4, 3)
-    assert charges.shape == (len(vertices), N_QUAD_2D)
-    return backend_lib.potential_radial(point, vertices, charges, len(charges))
+    assert jac_buffer.shape == (len(charges), N_QUAD_2D)
+    assert pos_buffer.shape == (len(charges), N_QUAD_2D, 2)
+    return backend_lib.potential_radial(point, charges, jac_buffer, pos_buffer, len(charges))
 
 def potential_radial_derivs(point, z, coeffs):
     assert coeffs.shape == (len(z)-1, DERIV_2D_MAX, 6)
     return backend_lib.potential_radial_derivs(point, z, coeffs, len(z))
 
-def charge_radial(vertices, charges):
-    assert vertices.shape == (len(charges), 3)
-    assert charges.shape == (len(vertices),)
-
-    return backend_lib.charge_radial(vertices, charges)
+def charge_radial(vertices, charge):
+    assert vertices.shape == (len(vertices), 3)
+    return backend_lib.charge_radial(vertices, charge)
 
-def field_radial(point, vertices, charges):
+def field_radial(point, charges, jac_buffer, pos_buffer):
     point = _vec_2d_to_3d(point)
-    assert vertices.shape == (len(charges), 4, 3)
-    assert charges.shape == (len(charges), N_QUAD_2D)
-     
+    assert jac_buffer.shape == (len(charges), N_QUAD_2D)
+    assert pos_buffer.shape == (len(charges), N_QUAD_2D, 2)
+    assert charges.shape == (len(charges),)
     field = np.zeros( (3,) )
-    backend_lib.field_radial(point, field, vertices, charges, len(charges))
+    backend_lib.field_radial(point, field, charges, jac_buffer, pos_buffer, len(charges))
     return field[:2]
 
 def field_radial_derivs(point, z, coeffs):
     point = _vec_2d_to_3d(point)
     assert coeffs.shape == (len(z)-1, DERIV_2D_MAX, 6)
     field = np.zeros( (3,) )
     backend_lib.field_radial_derivs(point, field, z, coeffs, len(z))
     return field[:2]
 
 dx1_potential_3d_point = remove_arg(backend_lib.dx1_potential_3d_point)
 dy1_potential_3d_point = remove_arg(backend_lib.dy1_potential_3d_point)
 dz1_potential_3d_point = remove_arg(backend_lib.dz1_potential_3d_point)
 potential_3d_point = remove_arg(backend_lib.potential_3d_point)
 
-def axial_coefficients_3d(vertices, charges, z, thetas, theta_interpolation):
-    assert vertices.shape == (len(charges), 3, 3)
+def axial_coefficients_3d(charges, jacobian_buffer, pos_buffer, z, thetas, theta_interpolation):
+    assert jacobian_buffer.shape == (len(charges), N_TRIANGLE_QUAD)
+    assert pos_buffer.shape == (len(charges), N_TRIANGLE_QUAD, 3)
     assert theta_interpolation.shape == (len(thetas)-1, NU_MAX, M_MAX, 4)
 
     output_coeffs = np.zeros( (len(z), 2, NU_MAX, M_MAX) )
     
-    backend_lib.axial_coefficients_3d(vertices, charges, len(vertices),
+    backend_lib.axial_coefficients_3d(charges, 
+        jacobian_buffer, pos_buffer,
+        len(charges),
         z, output_coeffs, len(z),
         thetas, theta_interpolation, len(thetas))
-    
+     
     return output_coeffs
 
-def potential_3d(point, vertices, charges):
-    assert vertices.shape == (len(charges), 3, 3)
+def potential_3d(point, charges, jac_buffer, pos_buffer):
     assert point.shape == (3,)
-     
-    return backend_lib.potential_3d(point, vertices, charges, len(charges))
+    N = len(charges)
+    assert charges.shape == (N,)
+    assert jac_buffer.shape == (N, N_TRIANGLE_QUAD)
+    assert pos_buffer.shape == (N, N_TRIANGLE_QUAD, 3)
+    
+    return backend_lib.potential_3d(point, charges, jac_buffer, pos_buffer, N)
 
 def potential_3d_derivs(point, z, coeffs):
-    assert coeffs.shape == (len(z)-1, NU_MAX, M_MAX, 4)
+    assert coeffs.shape == (len(z)-1, 2, NU_MAX, M_MAX, 4)
     assert point.shape == (3,)
     
     return backend_lib.potential_3d_derivs(point, z, coeffs, len(z))
 
-def field_3d(point, vertices, charges):
-    assert vertices.shape == (len(charges), 3, 3)
+def field_3d(point, charges, jacobian_buffer, position_buffer):
+    N = len(charges)
     assert point.shape == (3,)
-
+    assert jacobian_buffer.shape == (N, N_TRIANGLE_QUAD)
+    assert position_buffer.shape == (N, N_TRIANGLE_QUAD, 3)
+     
     field = np.zeros( (3,) )
-    backend_lib.field_3d(point, field, vertices, charges, len(vertices))
+    backend_lib.field_3d(point, field, charges, jacobian_buffer, position_buffer, N)
     return field
 
 def field_3d_derivs(point, z, coeffs):
     assert point.shape == (3,)
-    assert coeffs.shape == (len(z)-1, NU_MAX, M_MAX, 4)
+    assert coeffs.shape == (len(z)-1, 2, NU_MAX, M_MAX, 4)
 
     field = np.zeros( (3,) )
     backend_lib.field_3d_derivs(point, field, z, coeffs, len(z))
 
-def add_floating_conductor_constraints_radial(matrix, vertices, indices, row):
-    N_matrix = matrix.shape[0]
-    assert all(N_QUAD_2D*i < N_matrix for i in indices)
-    assert matrix.shape[0] == matrix.shape[1]
-
-    return backend_lib.add_floating_conductor_constraints_radial(matrix, vertices, N_matrix, indices.astype(np.int64), len(indices), row)
-
+def fill_jacobian_buffer_radial(vertices):
+    N = len(vertices)
+    jac_buffer = np.zeros( (N, N_QUAD_2D) )
+    pos_buffer = np.zeros( (N, N_QUAD_2D, 2) )
+     
+    backend_lib.fill_jacobian_buffer_radial(jac_buffer, pos_buffer, vertices, N)
+    
+    return jac_buffer, pos_buffer
 
-def fill_matrix_radial(matrix, lines, excitation_types, excitation_values, start_index, end_index):
+def fill_matrix_radial(matrix, lines, excitation_types, excitation_values, jac_buffer, pos_buffer, start_index, end_index):
     N = len(lines)
-    N_quad = N_QUAD_2D*N
-    
     # Due to floating conductor constraints the matrix might actually be bigger than NxN
-    assert matrix.shape[0] >= N_quad and matrix.shape[1] >= N_quad and matrix.shape[0] == matrix.shape[1]
+    assert matrix.shape[0] >= N and matrix.shape[1] >= N and matrix.shape[0] == matrix.shape[1]
     assert lines.shape == (N, 4, 3)
     assert excitation_types.shape == (N,)
     assert excitation_values.shape == (N,)
+    assert jac_buffer.shape == (N, N_QUAD_2D)
+    assert pos_buffer.shape == (N, N_QUAD_2D, 2)
     assert 0 <= start_index < N and 0 <= end_index < N and start_index < end_index
      
-    backend_lib.fill_matrix_radial(matrix, lines, excitation_types, excitation_values, N, matrix.shape[0], start_index, end_index)
+    backend_lib.fill_matrix_radial(matrix, lines, excitation_types, excitation_values, jac_buffer, pos_buffer, N, matrix.shape[0], start_index, end_index)
+
+def fill_jacobian_buffer_3d(vertices):
+    N = len(vertices)
+    jac_buffer = np.zeros( (N, N_TRIANGLE_QUAD) )
+    pos_buffer = np.zeros( (N, N_TRIANGLE_QUAD, 3) )
+    
+    backend_lib.fill_jacobian_buffer_3d(jac_buffer, pos_buffer, vertices, N)
 
-def fill_matrix_3d(matrix, vertices, excitation_types, excitation_values, start_index, end_index):
+    return jac_buffer, pos_buffer
+
+def fill_matrix_3d(matrix, vertices, excitation_types, excitation_values, jac_buffer, pos_buffer, start_index, end_index):
     N = len(vertices)
     # Due to floating conductor constraints the matrix might actually be bigger than NxN
     assert matrix.shape[0] >= N and matrix.shape[1] >= N and matrix.shape[0] == matrix.shape[1]
-    assert vertices.shape == (N, 3, 3)
+    assert vertices.shape == (N, 6, 3)
     assert excitation_types.shape == (N,)
     assert excitation_values.shape == (N,)
+    assert jac_buffer.shape == (N, N_TRIANGLE_QUAD)
+    assert pos_buffer.shape == (N, N_TRIANGLE_QUAD, 3)
     assert 0 <= start_index < N and 0 <= end_index < N and start_index < end_index
-    
-    backend_lib.fill_matrix_3d(matrix, vertices, excitation_types, excitation_values, N, matrix.shape[0], start_index, end_index)
+     
+    backend_lib.fill_matrix_3d(matrix, vertices, excitation_types, excitation_values, jac_buffer, pos_buffer, N, matrix.shape[0], start_index, end_index)
 
-def xy_plane_intersection(positions, z):
+def plane_intersection(positions, p0, normal):
+    assert p0.shape == (3,)
+    assert normal.shape == (3,)
+    assert positions.shape == (len(positions), 6)
     
-    assert positions.shape[1] == 4 or positions.shape[1] == 6
+    result = np.zeros(6)
+    found = backend_lib.plane_intersection(p0, normal, positions, len(positions), result)
     
-    positions = np.require(positions, dtype=np.float64, requirements=('C_CONTIGUOUS', 'ALIGNED'))
-     
-    if positions.shape[1] == 4:
-        result = np.zeros( (4,) )
-        found = backend_lib.xy_plane_intersection_2d(positions, len(positions), result, z)
-        
-        return result if found else None
-
-    if positions.shape[1] == 6:
-        result = np.zeros( (6,) )
-        found = backend_lib.xy_plane_intersection_3d(positions, len(positions), result, z)
-        
-        return result if found else None
-
+    return result if found else None
 
+def line_intersection(positions, p0, tangent):
+    assert p0.shape == (2,)
+    assert tangent.shape == (2,)
+    assert positions.shape == (len(positions), 4)
     
-
-
-
-
-
+    result = np.zeros(4)
+    found = backend_lib.line_intersection(p0, tangent, positions, len(positions), result)
+     
+    return result if found else None
```

### Comparing `traceon-0.2.0/traceon/backend/traceon-backend.c` & `traceon-0.3.0/traceon/backend/traceon-backend.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #include <stdio.h>
 #include <assert.h>
 #include <math.h>
 #include <stdlib.h>
 #include <stdint.h>
 #include <stdbool.h>
 
+#include <gsl/gsl_integration.h>
+
 #ifdef _MSC_VER
 #define EXPORT __declspec(dllexport)
 
 #include <Python.h>
 PyMODINIT_FUNC PyInit_traceon_backend(void) {
 	return NULL;
 }
 
 #else
 #define EXPORT extern
 #endif
 
+#define INLINE EXPORT inline
+
 #if defined(__clang__)
 	#define UNROLL _Pragma("clang loop unroll(full)")
 #elif defined(__GNUC__) || defined(__GNUG__)
 	#define UNROLL _Pragma("GCC unroll 100")
 #else
 	#define UNROLL
 #endif
@@ -35,49 +39,68 @@
 // the preprocessor will substitute their names. We can also not 
 // simply only use these symbols instead of the preprocessor variables
 // as the length of arrays need to be a compile time constant in C...
 EXPORT const int DERIV_2D_MAX_SYM = 9;
 EXPORT const int NU_MAX_SYM = NU_MAX;
 EXPORT const int M_MAX_SYM = M_MAX;
 
-#define N_TRIANGLE_QUAD 9
 
 #define TRACING_STEP_MAX 0.01
 #define MIN_DISTANCE_AXIS 1e-10
 
 #ifndef M_PI
     #define M_PI 3.14159265358979323846
 #endif
 
 
 EXPORT const size_t TRACING_BLOCK_SIZE = (size_t) 1e5;
 
-#define N_QUAD_2D 4
+#define N_QUAD_2D 16
 EXPORT const int N_QUAD_2D_SYM = N_QUAD_2D;
-const double GAUSS_QUAD_POINTS[N_QUAD_2D] = {-0.3399810435848563, 0.3399810435848563, -0.8611363115940526, 0.8611363115940526};
-const double GAUSS_QUAD_WEIGHTS[N_QUAD_2D] = {0.6521451548625461, 0.6521451548625461, 0.3478548451374538, 0.3478548451374538};
+const double GAUSS_QUAD_WEIGHTS[N_QUAD_2D] = {0.1894506104550685, 0.1894506104550685, 0.1826034150449236, 0.1826034150449236, 0.1691565193950025, 0.1691565193950025, 0.1495959888165767, 0.1495959888165767, 0.1246289712555339, 0.1246289712555339, 0.0951585116824928, 0.0951585116824928, 0.0622535239386479, 0.0622535239386479, 0.0271524594117541, 0.0271524594117541};
+const double GAUSS_QUAD_POINTS[N_QUAD_2D] = {-0.0950125098376374, 0.0950125098376374, -0.2816035507792589, 0.2816035507792589, -0.4580167776572274, 0.4580167776572274, -0.6178762444026438, 0.6178762444026438, -0.7554044083550030, 0.7554044083550030, -0.8656312023878318, 0.8656312023878318, -0.9445750230732326, 0.9445750230732326, -0.9894009349916499, 0.9894009349916499};
 
 
+// Triangle quadrature constants
+#define N_TRIANGLE_QUAD 33
+EXPORT const int N_TRIANGLE_QUAD_SYM = N_TRIANGLE_QUAD;
+const double QUAD_WEIGHTS[N_TRIANGLE_QUAD] = {0.03127061, 0.01424303, 0.02495917, 0.01213342, 0.00396582, 0.03127061, 0.01424303, 0.02495917, 0.01213342, 0.00396582, 0.03127061, 0.01424303, 0.02495917, 0.01213342, 0.00396582, 0.02161368, 0.00754184, 0.01089179, 0.02161368, 0.00754184, 0.01089179, 0.02161368, 0.00754184, 0.01089179, 0.02161368, 0.00754184, 0.01089179, 0.02161368, 0.00754184, 0.01089179, 0.02161368, 0.00754184, 0.01089179};
+const double QUAD_B1[N_TRIANGLE_QUAD] = {0.27146251, 0.10925783, 0.44011165, 0.48820375, 0.02464636, 0.27146251, 0.10925783, 0.44011165, 0.48820375, 0.02464636, 0.45707499, 0.78148434, 0.1197767 , 0.0235925 , 0.95070727, 0.11629602, 0.02138249, 0.02303416, 0.62824975, 0.85133779, 0.68531016, 0.25545423, 0.12727972, 0.29165568, 0.25545423, 0.12727972, 0.29165568, 0.62824975, 0.85133779, 0.68531016, 0.11629602, 0.02138249, 0.02303416};
+const double QUAD_B2[N_TRIANGLE_QUAD] = {0.27146251, 0.10925783, 0.44011165, 0.48820375, 0.02464636, 0.45707499, 0.78148434, 0.1197767 , 0.0235925 , 0.95070727, 0.27146251, 0.10925783, 0.44011165, 0.48820375, 0.02464636, 0.25545423, 0.12727972, 0.29165568, 0.11629602, 0.02138249, 0.02303416, 0.62824975, 0.85133779, 0.68531016, 0.11629602, 0.02138249, 0.02303416, 0.25545423, 0.12727972, 0.29165568, 0.62824975, 0.85133779, 0.68531016};
+
 //////////////////////////////// TYPEDEFS
 
+
 typedef double (*integration_cb_2d)(double, double, double, double, void*);
 typedef double (*vertices_2d)[4][3];
 typedef double (*charges_2d)[N_QUAD_2D];
 
+// See GMSH documentation
+typedef double triangle6[6][3];
+typedef double (*vertices_3d)[6][3];
+
+typedef double (*positions_3d)[6];
+
+typedef double (*jacobian_buffer_3d)[N_TRIANGLE_QUAD];
+typedef double (*position_buffer_3d)[N_TRIANGLE_QUAD][3];
+
+typedef double (*positions_2d)[4];
+
+typedef double (*jacobian_buffer_2d)[N_QUAD_2D];
+typedef double (*position_buffer_2d)[N_QUAD_2D][2];
+
 //////////////////////////////// ELLIPTIC FUNCTIONS
 
 // Chebyshev Approximations for the Complete Elliptic Integrals K and E.
 // W. J. Cody. 1965.
 //
 // Augmented with the tricks shown on the Scipy documentation for ellipe and ellipk.
+// https://docs.scipy.org/doc/scipy/reference/generated/scipy.special.ellipkm1.html#scipy.special.ellipkm1
 
-
-double ellipk_singularity(double k) {
-	double eta = 1 - k;
-	
+EXPORT double ellipkm1(double p) {
 	double A[] = {log(4.0),
 			9.65736020516771e-2,
 			3.08909633861795e-2,
 			1.52618320622534e-2,
 			1.25565693543211e-2,
 			1.68695685967517e-2,
 			1.09423810688623e-2,
@@ -88,32 +111,30 @@
 			7.03114105853296e-2,
 			4.87379510945218e-2,
 			3.57218443007327e-2,
 			2.09857677336790e-2,
 			5.81807961871996e-3,
 			3.42805719229748e-4};
 	
-	double L = log(1./eta);
+	double L = log(1./p);
 	double sum_ = 0.0;
 
 	for(int i = 0; i < 8; i++)
-		sum_ += (A[i] + L*B[i])*pow(eta, i);
+		sum_ += (A[i] + L*B[i])*pow(p, i);
 	
 	return sum_;
 }
 
 EXPORT double ellipk(double k) {
-	if(k > -1) return ellipk_singularity(k);
+	if(k > -1) return ellipkm1(1-k);
 	
-	return ellipk_singularity(1 - 1./(1-k))/sqrt(1-k);
+	return ellipkm1(1./(1-k))/sqrt(k);
 }
 
-double ellipe_01(double k) {
-	double eta = 1 - k;
-	
+EXPORT double ellipem1(double p) {
 	double A[] = {1,
         4.43147193467733e-1,
         5.68115681053803e-2,
         2.21862206993846e-2,
         1.56847700239786e-2,
         1.92284389022977e-2,
         1.21819481486695e-2,
@@ -124,40 +145,39 @@
         9.37488062098189e-2,
         5.84950297066166e-2,
         4.09074821593164e-2,
         2.35091602564984e-2,
         6.45682247315060e-3,
         3.78886487349367e-4};
 	
-	double L = log(1./eta);
+	double L = log(1./p);
 	double sum_ = 0.0;
 
 	for(int i = 0; i < 8; i++)
-		sum_ += (A[i] + L*B[i])*pow(eta, i);
+		sum_ += (A[i] + L*B[i])*pow(p, i);
 		
 	return sum_;
 }
 
 EXPORT double ellipe(double k) {
-	if (0 <= k && k <= 1) return ellipe_01(k);
+	if (0 <= k && k <= 1) return ellipem1(1-k);
 
-	return ellipe_01(k/(k-1.))*sqrt(1-k);
+	return ellipem1(-1/(k-1.))*sqrt(1-k);
 }
 
 
 //////////////////////////////// UTILITIES 2D
 
 
-
-EXPORT inline double
+INLINE double
 norm_2d(double x, double y) {
 	return sqrt(x*x + y*y);
 }
 
-EXPORT inline double
+INLINE double
 length_2d(double *v1, double *v2) {
 	return norm_2d(v2[0]-v1[0], v2[1]-v1[1]);
 }
 
 EXPORT void
 normal_2d(double *p1, double *p2, double *normal) {
 	double x1 = p1[0], y1 = p1[1];
@@ -167,15 +187,15 @@
 	double normal_x = tangent_y, normal_y = -tangent_x;
 	double length = norm_2d(normal_x, normal_y);
 
 	normal[0] = normal_x/length;
 	normal[1] = normal_y/length;
 }
 
-void
+EXPORT void
 higher_order_normal_radial(double alpha, double *v1, double *v2, double *v3, double *v4, double *normal) {
 
 	double v1x = v1[0], v1y = v1[1];
 	double v2x = v2[0], v2y = v2[1];
 	double v3x = v3[0], v3y = v3[1];
 	double v4x = v4[0], v4y = v4[1];
 		
@@ -187,15 +207,15 @@
 
 	double zero[2] = {0., 0.};
 	double vec[2] = {dx, dy};
 	normal_2d(zero, vec, normal);
 }
 
 
-EXPORT void inline position_and_jacobian_radial(double alpha, double *v1, double *v2, double *v3, double *v4, double *pos_out, double *jac) {
+INLINE void position_and_jacobian_radial(double alpha, double *v1, double *v2, double *v3, double *v4, double *pos_out, double *jac) {
 
 	double v1x = v1[0], v1y = v1[1];
 	double v2x = v2[0], v2y = v2[1];
 	double v3x = v3[0], v3y = v3[1];
 	double v4x = v4[0], v4y = v4[1];
 		
 	double a2 = pow(alpha, 2);
@@ -210,15 +230,15 @@
 }
 
 //////////////////////////////// UTILITIES 3D
 
 
 typedef double (*integration_cb_3d)(double, double, double, double, double, double, void*);
 
-EXPORT inline double
+INLINE double
 norm_3d(double x, double y, double z) {
 	return sqrt(x*x + y*y + z*z);
 }
 
 EXPORT void
 normal_3d(double *p1, double *p2, double *p3, double *normal) {
 	double x1 = p1[0], y1 = p1[1], z1 = p1[2];
@@ -231,81 +251,162 @@
 	double length = norm_3d(normal_x, normal_y, normal_z);
 	
 	normal[0] = normal_x/length;
 	normal[1] = normal_y/length;
 	normal[2] = normal_z/length;
 }
 
-// Triangle quadrature constants
-const double QUAD_B1[N_TRIANGLE_QUAD] = {0.124949503233232, 0.437525248383384, 0.437525248383384, 0.797112651860071, 0.797112651860071, 0.165409927389841, 0.165409927389841, 0.037477420750088, 0.037477420750088};
-const double QUAD_B2[N_TRIANGLE_QUAD] = {0.437525248383384, 0.124949503233232, 0.437525248383384, 0.165409927389841, 0.037477420750088, 0.797112651860071, 0.037477420750088, 0.797112651860071, 0.165409927389841};
-const double QUAD_WEIGHTS[N_TRIANGLE_QUAD] = {0.205950504760887, 0.205950504760887, 0.205950504760887, 0.063691414286223, 0.063691414286223, 0.063691414286223, 0.063691414286223, 0.063691414286223, 0.063691414286223};
+INLINE void barycentric_coefficients_higher_order_triangle_3d(double alpha, double beta,
+	double v0, double v1, double v2, double v3, double v4, double v5, double coeffs[6]) {
+    coeffs[0] = v0;
+	coeffs[1] = 4*v3-v1-3*v0;
+	coeffs[2] = 4*v5-v2-3*v0;
+	coeffs[3] = -4*v3+2*v1+2*v0;
+	coeffs[4] = -4*v5+4*v4-4*v3+4*v0;
+	coeffs[5] = -4*v5+2*v2+2*v0;
+}
 
-EXPORT double
-triangle_integral(double target[3], double v1[3], double v2[3], double v3[3], integration_cb_3d function, void *args) {
+INLINE double dot6(double *v1, double *v2) {
+	double sum = 0.0;
+	UNROLL
+	for(int i = 0; i < 6; i++) sum += v1[i]*v2[i];
+	return sum;
+}
+
+INLINE void
+cross_product_3d(double *v1, double *v2, double *out) {
 	double v1x = v1[0], v1y = v1[1], v1z = v1[2];
 	double v2x = v2[0], v2y = v2[1], v2z = v2[2];
-	double v3x = v3[0], v3y = v3[1], v3z = v3[2];
-		
-	double area = 0.5*sqrt(pow((v2y-v1y)*(v3z-v1z)-(v2z-v1z)*(v3y-v1y), 2) + pow((v2z-v1z)*(v3x-v1x)-(v2x-v1x)*(v3z-v1z), 2) + pow((v2x-v1x)*(v3y-v1y)-(v2y-v1y)*(v3x-v1x), 2));
+
+	out[0] = v1y*v2z-v1z*v2y;
+	out[1] = v1z*v2x-v1x*v2z;
+	out[2] = v1x*v2y-v1y*v2x;
+}
+
+INLINE double norm_cross_product_3d(double *v1, double *v2) {
+	double out[3];
+	cross_product_3d(v1, v2, out);
+	return norm_3d(out[0], out[1], out[2]);
+}
+
+INLINE void position_and_jacobian_3d(double alpha, double beta, triangle6 v, double *pos_out, double *jac) {
+
+	double coeffs_x[6], coeffs_y[6], coeffs_z[6];
+	barycentric_coefficients_higher_order_triangle_3d(alpha, beta, v[0][0], v[1][0], v[2][0], v[3][0], v[4][0], v[5][0], coeffs_x);
+	barycentric_coefficients_higher_order_triangle_3d(alpha, beta, v[0][1], v[1][1], v[2][1], v[3][1], v[4][1], v[5][1], coeffs_y);
+	barycentric_coefficients_higher_order_triangle_3d(alpha, beta, v[0][2], v[1][2], v[2][2], v[3][2], v[4][2], v[5][2], coeffs_z);
 	
-	double sum_ = 0.0;
+	double monomials[6] = {1, alpha, beta, pow(alpha,2), alpha*beta, pow(beta,2)};
+	double monomials_da[6] = {0, 1, 0, 2*alpha, beta, 0};
+	double monomials_db[6] = {0, 0, 1, 0, alpha, 2*beta};
+
+	pos_out[0] = dot6(coeffs_x, monomials);
+	pos_out[1] = dot6(coeffs_y, monomials);
+	pos_out[2] = dot6(coeffs_z, monomials);
+
+	double da[3] = {
+		dot6(coeffs_x, monomials_da),
+		dot6(coeffs_y, monomials_da),
+		dot6(coeffs_z, monomials_da),
+	};
 	
-	for (int k=0; k < N_TRIANGLE_QUAD; k++) {
-		double b1_ = QUAD_B1[k];
-		double b2_ = QUAD_B2[k];
-		double w = QUAD_WEIGHTS[k];
-			
-        double x = v1x + b1_*(v2x-v1x) + b2_*(v3x-v1x);
-        double y = v1y + b1_*(v2y-v1y) + b2_*(v3y-v1y);
-        double z = v1z + b1_*(v2z-v1z) + b2_*(v3z-v1z);
-			
-        sum_ += w*function(target[0], target[1], target[2], x, y, z, args);
-	}
-	      
-    return area*sum_;
-}
-
-// This is a bit of a hack.. we supply a triangle_integral function which is exactly
-// the same as above, except we inline the 'potential_3d_point' function directly. Weirdly this
-// seem to trigger some kind of optimization within GCC that makes building the matrix much faster. I was not
-// able to reproduce this behaviour simply by extensive use of the 'inline' keyword.
-EXPORT inline double potential_3d_point(double x0, double y0, double z0, double x, double y, double z, void *_) {
-	double r = norm_3d(x-x0, y-y0, z-z0);
-    return 1/(4*r);
+	double db[3] = {
+		dot6(coeffs_x, monomials_db),
+		dot6(coeffs_y, monomials_db),
+		dot6(coeffs_z, monomials_db),
+	};
+	
+	*jac = norm_cross_product_3d(da, db);
 }
 
+struct self_voltage_3d_args {
+	double beta;
+	double *target;
+	double *vertices;
+	integration_cb_3d cb_fun;
+	void *cb_args;	
+	gsl_integration_workspace *inner_workspace;
+};
+
 double
-triangle_integral_potential_3d_point(double target[3], double v1[3], double v2[3], double v3[3]) {
-	double v1x = v1[0], v1y = v1[1], v1z = v1[2];
-	double v2x = v2[0], v2y = v2[1], v2z = v2[2];
-	double v3x = v3[0], v3y = v3[1], v3z = v3[2];
-		
-	double area = 0.5*sqrt(pow((v2y-v1y)*(v3z-v1z)-(v2z-v1z)*(v3y-v1y), 2) + pow((v2z-v1z)*(v3x-v1x)-(v2x-v1x)*(v3z-v1z), 2) + pow((v2x-v1x)*(v3y-v1y)-(v2y-v1y)*(v3x-v1x), 2));
+triangle_integral_alpha(double alpha, void *args_p) {
+
+	struct self_voltage_3d_args *args = args_p;
+	double *target = args->target;
+	double beta = args->beta;
+
+	// Telles transformation
+	double B = 1-beta;
+	const int order = 5;
+	double eta = B*pow(alpha, order);
+	double Jeta = order*B*pow(alpha, order-1);
 	
-	double sum_ = 0.0;
+	double pos[3], jac;
+	double *v = args->vertices;
 	
-	for (int k=0; k < N_TRIANGLE_QUAD; k++) {
-		double b1_ = QUAD_B1[k];
-		double b2_ = QUAD_B2[k];
-		double w = QUAD_WEIGHTS[k];
-			
-        double x = v1x + b1_*(v2x-v1x) + b2_*(v3x-v1x);
-        double y = v1y + b1_*(v2y-v1y) + b2_*(v3y-v1y);
-        double z = v1z + b1_*(v2z-v1z) + b2_*(v3z-v1z);
-			
-        sum_ += w*potential_3d_point(target[0], target[1], target[2], x, y, z, NULL);
-	}
-	      
-    return area*sum_;
+	position_and_jacobian_3d(eta, beta, (double (*)[3]) args->vertices, pos, &jac);
+	
+	return Jeta*jac*args->cb_fun(target[0], target[1], target[2], pos[0], pos[1], pos[2], args->cb_args);
 }
 
+#define ADAPTIVE_MAX_ITERATION 5000
 
+double
+triangle_integral_beta(double beta, void *args_p) {
+
+	struct self_voltage_3d_args *args = args_p;
+	
+	// Telles transformation
+	const int order = 3;
+	double eta = pow(beta,order);
+	double Jeta = order*pow(beta,order-1);
+		
+	args->beta = eta;
+			
+    gsl_function F;
+    F.function = &triangle_integral_alpha;
+	F.params = args;
+		
+    double result, error;
+    gsl_integration_qags(&F, 0, 1, 0, 1e-5, ADAPTIVE_MAX_ITERATION, args->inner_workspace, &result, &error);
+		
+	return Jeta*result;
+}
 
+double
+triangle_integral_adaptive(double target[3], triangle6 vertices, integration_cb_3d function, void *args) {
+	// TODO: optimize this, put outside the loop over the matrix diagonal
+	gsl_integration_workspace * w = gsl_integration_workspace_alloc(ADAPTIVE_MAX_ITERATION);
+	gsl_integration_workspace * w_inner = gsl_integration_workspace_alloc(ADAPTIVE_MAX_ITERATION);
+	
+	struct self_voltage_3d_args integration_args = {
+		.target = target,
+		.cb_fun = function,
+		.cb_args = args,
+		.vertices = (double*) vertices,
+		.inner_workspace = w_inner
+	};
+		
+    gsl_function F;
+    F.function = &triangle_integral_beta;
+	F.params = &integration_args;
+		
+    double result, error;
+    gsl_integration_qags(&F, 0, 1, 0, 1e-5, ADAPTIVE_MAX_ITERATION, w, &result, &error);
+	
+    gsl_integration_workspace_free(w);
+    gsl_integration_workspace_free(w_inner);
+		
+	return result;
+}
 
+INLINE double potential_3d_point(double x0, double y0, double z0, double x, double y, double z, void *_) {
+	double r = norm_3d(x-x0, y-y0, z-z0);
+    return 1/(4*r);
+}
 
 //////////////////////////////// PARTICLE TRACING
 
 
 const double EM = -0.1758820022723908; // e/m units ns and mm
 
 const double A[]  = {0.0, 2./9., 1./3., 3./4., 1., 5./6.};	// https://en.wikipedia.org/wiki/Runge%E2%80%93Kutta%E2%80%93Fehlberg_method
@@ -405,133 +506,86 @@
 }
 
 
 
 //////////////////////////////// RADIAL RING POTENTIAL (DERIVATIVES)
 
 
-EXPORT double dr1_potential_radial_ring(double r_0, double z_0, double r, double z, void *_) {
+EXPORT double dr1_potential_radial_ring(double r0, double z0, double r, double z, void *_) {
 	
-	if (fabs(r_0) < MIN_DISTANCE_AXIS) return 0.0; // Prevent stepping into singularity
+	if(r0 < MIN_DISTANCE_AXIS) {
+		return 0.0;
+	}
 	
-    double s = norm_2d(z-z_0, r+r_0);
-    double s1 = (r_0 + r) / s;
-    double t = 4.0 * r * r_0 / pow(s, 2);
-    double A = ellipe(t);
-    double B = ellipk(t);
-    double ellipe_term = -(2.0 * r * r_0 * s1 - r * s) / (2.0 * r_0 * pow(s, 2) - 8.0 * pow(r_0, 2) * r);
-    double ellipk_term = -r / (2.0 * r_0 * s);
-    return A * ellipe_term + B * ellipk_term;
-}
-
-
-EXPORT double potential_radial_ring(double r_0, double z_0, double r, double z, void *_) {
-    double rz2 = pow(r + r_0, 2) + pow(z - z_0, 2);
-    double t = 4.0 * r * r_0 / rz2;
-    return ellipk(t) * r / sqrt(rz2);
-}
-
-EXPORT double dz1_potential_radial_ring(double r_0, double z_0, double r, double z, void *_) {
-    double rz2 = pow(r + r_0, 2) + pow(z - z_0, 2);
-    double t = 4.0 * r * r_0 / rz2;
-    double numerator = r * (z - z_0) * ellipe(t);
-    double denominator = ((pow(z - z_0, 2) + pow(r - r_0, 2)) * sqrt(rz2));
-    return numerator / denominator;
+	double delta_r = r - r0;
+	double delta_z = z - z0;
+    double common_arg = (delta_z * delta_z + delta_r * delta_r) / (4 * r * r - 4 * delta_r * r + delta_z * delta_z + delta_r * delta_r);
+    double denominator = ((-2 * delta_r * delta_r * r) + delta_z * delta_z * (2 * delta_r - 2 * r) + 2 * delta_r * delta_r * delta_r) * sqrt(4 * r * r - 4 * delta_r * r + delta_z * delta_z + delta_r * delta_r);
+    double ellipkm1_term = (delta_z * delta_z * r + delta_r * delta_r * r) * ellipkm1(common_arg);
+    double ellipem1_term = ((-2 * delta_r * r * r) - delta_z * delta_z * r + delta_r * delta_r * r) * ellipem1(common_arg);
+    return (ellipkm1_term + ellipem1_term) / denominator;
+}
+
+EXPORT double potential_radial_ring(double r0, double z0, double r, double z, void *_) {
+    double delta_z = z - z0;
+    double delta_r = r - r0;
+    double t = (pow(delta_z, 2) + pow(delta_r, 2)) / (pow(delta_z, 2) + pow(delta_r, 2) + 4 * r0 * delta_r + 4 * pow(r0, 2));
+    return ellipkm1(t) * (delta_r + r0) / sqrt(pow(delta_z, 2) + pow((delta_r + 2 * r0), 2));
+}
+
+EXPORT double dz1_potential_radial_ring(double r0, double z0, double r, double z, void *_) {
+	double delta_z = z - z0;
+    double delta_r = r - r0;
+    double common_arg = (delta_z * delta_z + delta_r * delta_r) / (4 * r0 * r0 + 4 * delta_r * r0 + delta_z * delta_z + delta_r * delta_r);
+    double denominator = (delta_z * delta_z + delta_r * delta_r) * sqrt(4 * r0 * r0 + 4 * delta_r * r0 + delta_z * delta_z + delta_r * delta_r);
+    double ellipem1_term = -delta_z * (r0 + delta_r) * ellipem1(common_arg);
+    return -ellipem1_term / denominator;
 }
 
 
 EXPORT void
-axial_derivatives_radial_ring(double *derivs_p, vertices_2d lines, charges_2d charges, size_t N_lines, double *z, size_t N_z) {
+axial_derivatives_radial_ring(double *derivs_p, double *charges, jacobian_buffer_2d jac_buffer, position_buffer_2d pos_buffer, size_t N_lines, double *z, size_t N_z) {
 
 	double (*derivs)[9] = (double (*)[9]) derivs_p;	
 		
 	for(int i = 0; i < N_z; i++) 
 	for(int j = 0; j < N_lines; j++)
 	for(int k = 0; k < N_QUAD_2D; k++) {
 		double z0 = z[i];
-
-		double *v1 = &lines[j][0][0];
-		double *v2 = &lines[j][2][0];
-		double *v3 = &lines[j][3][0];
-		double *v4 = &lines[j][1][0];
-			
-		double pos[2], jac;
-		position_and_jacobian_radial(GAUSS_QUAD_POINTS[k], v1, v2, v3, v4, pos, &jac);
-		double r = pos[0], z = pos[1];
+		double r = pos_buffer[j][k][0], z = pos_buffer[j][k][1];
 		
-		double weight = GAUSS_QUAD_WEIGHTS[k] * jac;
-			
 		double R = norm_2d(z0-z, r);
 		
 		double D[9] = {0.}; // Derivatives of the currently considered line element.
 		D[0] = 1/R;
 		D[1] = -(z0-z)/pow(R, 3);
 			
 		for(int n = 1; n+1 < DERIV_2D_MAX; n++)
 			D[n+1] = -1./pow(R,2) *( (2*n + 1)*(z0-z)*D[n] + pow(n,2)*D[n-1]);
 		
-		for(int l = 0; l < 9; l++) derivs[i][l] += weight * M_PI*r/2 * charges[j][k]*D[l];
+		for(int l = 0; l < 9; l++) derivs[i][l] += jac_buffer[j][k] * charges[j] * M_PI*r/2 * D[l];
 	}
 }
 
 //////////////////////////////// RADIAL SYMMETRY POTENTIAL EVALUATION
 
 
-
-// John A. Crow. Quadrature of Integrands with a Logarithmic Singularity. 1993.
-// Computed higher order points and weights with own Python code..
-#define N_LOG_QUAD_2D 12
-const double GAUSS_LOG_QUAD_POINTS[N_LOG_QUAD_2D] =
-					{0.000245284264977222214486999757349594712755863,
-					0.003593698020213691584953180874184458866517133,
-					0.01712292595159614370417434799786314278267083,
-					0.05020561232318819384573670241984682206686949,
-					0.1115235855573625644218104518656856812018872,
-					0.2060030029051239758752495945505766309866304,
-					0.3324626975136065400973675503604997045074356,
-					0.4826067009659319425485030383099190543511725,
-					0.6416794701239928589863342367708391692838668,
-					0.7907090871833554068663998987642233419999952,
-					0.9098838287655625921196627463680156613773641,
-					0.9823479377157619510221418912858930542857947};
-
-const double GAUSS_LOG_QUAD_WEIGHTS[N_LOG_QUAD_2D] =
-					{0.0009331998830671428063097434941623766739840873,
-					0.006977495915143715985530451759041482867494198,
-					0.02169468902199853397715717421909584842021132,
-					0.04597069439559112469266362311262695693833166,
-					0.07752703869583178458842135310107317470803586,
-					0.1112525181837396068263131383589812009329696,
-					0.1402731060085833332292272698216837072064324,
-					0.1575171300868296275541516485738687199310457,
-					0.1574083422236489759715520802610080785790687,
-					0.1372838327177858585860313716723887135089706,
-					0.09819669547418950067876642091789781881144955,
-					0.04496525739359079510387572470817192142199618};
-
-
-
 EXPORT double
-potential_radial(double point[3], vertices_2d vertices, charges_2d charges, size_t N_vertices) {
+potential_radial(double point[3], double* charges, jacobian_buffer_2d jacobian_buffer, position_buffer_2d position_buffer, size_t N_vertices) {
 
-	double sum_ = 0.0;
+	double sum_ = 0.0;  
 	
-	for(int i = 0; i < N_vertices; i++) {
-		double *v1 = &vertices[i][0][0];
-		double *v2 = &vertices[i][2][0]; // Strange ordering following from GMSH line4 element
-		double *v3 = &vertices[i][3][0]; // Strange ordering following from GMSH line4 element
-		double *v4 = &vertices[i][1][0];
-		
-		for(int j = 0; j < N_QUAD_2D; j++) {
-			double pos[2], jac;
-			position_and_jacobian_radial(GAUSS_QUAD_POINTS[j], v1, v2, v3, v4, pos, &jac);
-			sum_ += jac*GAUSS_QUAD_WEIGHTS[j] * charges[i][j] * potential_radial_ring(point[0], point[1], pos[0], pos[1], NULL);
+	for(int i = 0; i < N_vertices; i++) {  
+		for(int k = 0; k < N_QUAD_2D; k++) {
+			double *pos = &position_buffer[i][k][0];
+			double potential = potential_radial_ring(point[0], point[1], pos[0], pos[1], NULL);
+			sum_ += charges[i] * jacobian_buffer[i][k] * potential;
 		}
-	}
-
+	}  
+	
 	return sum_;
 }
 
 EXPORT double
 potential_radial_derivs(double point[2], double *z_inter, double *coeff_p, size_t N_z) {
 	
 	double (*coeff)[DERIV_2D_MAX][6] = (double (*)[DERIV_2D_MAX][6]) coeff_p;
@@ -577,15 +631,15 @@
 	double Ez = -dz1_potential_radial_ring(r0, z0, r, z, NULL);
 	
 	return factor*(args->normal[0]*Er + args->normal[1]*Ez);
 
 }
 
 EXPORT double
-charge_radial(double *vertices_p, double *charges) {
+charge_radial(double *vertices_p, double charge) {
 
 	double (*vertices)[3] = (double (*)[3]) vertices_p;
 		
 	double *v1 = &vertices[0][0];
 	double *v2 = &vertices[2][0]; // Strange ordering following from GMSH line4 element
 	double *v3 = &vertices[3][0];
 	double *v4 = &vertices[1][0];
@@ -597,65 +651,87 @@
 		double pos[2], jac;
 		position_and_jacobian_radial(GAUSS_QUAD_POINTS[k], v1, v2, v3, v4, pos, &jac);
 		
 		// Surface area is 2pi*r * charge_integral
 		// charge_integral is charge integrated over line element
 		// charge_integral is weight*dl*charge
 		// where dl is the jacobian
-		sum_ += 2*M_PI*pos[0]*GAUSS_QUAD_WEIGHTS[k]*jac*charges[k];
+		sum_ += 2*M_PI*pos[0]*GAUSS_QUAD_WEIGHTS[k]*jac*charge;
 	}
 
 	return sum_;
 }
 
 EXPORT void
-field_radial(double point[3], double result[3], vertices_2d vertices, charges_2d charges, size_t N_vertices) {
-		
+field_radial(double point[3], double result[3], double* charges, jacobian_buffer_2d jacobian_buffer, position_buffer_2d position_buffer, size_t N_vertices) {
+	
 	double Ex = 0.0, Ey = 0.0;
 	
-	for(int i = 0; i < N_vertices; i++) 
-	for(int k = 0; k < N_QUAD_2D; k++) {
-			
-		double *v1 = &vertices[i][0][0];
-		double *v2 = &vertices[i][2][0]; // Strange ordering following from GMSH line4 element
-		double *v3 = &vertices[i][3][0];
-		double *v4 = &vertices[i][1][0];
-		
-		double pos[2], jac;
-		position_and_jacobian_radial(GAUSS_QUAD_POINTS[k], v1, v2, v3, v4, pos, &jac);
-		
-		Ex -= GAUSS_QUAD_WEIGHTS[k] * jac * charges[i][k] * dr1_potential_radial_ring(point[0], point[1], pos[0], pos[1], NULL);
-		Ey -= GAUSS_QUAD_WEIGHTS[k] * jac * charges[i][k] * dz1_potential_radial_ring(point[0], point[1], pos[0], pos[1], NULL);
+	for(int i = 0; i < N_vertices; i++) {  
+		for(int k = 0; k < N_QUAD_2D; k++) {
+			double *pos = &position_buffer[i][k][0];
+			Ex -= charges[i] * jacobian_buffer[i][k] * dr1_potential_radial_ring(point[0], point[1], pos[0], pos[1], NULL);
+			Ey -= charges[i] * jacobian_buffer[i][k] * dz1_potential_radial_ring(point[0], point[1], pos[0], pos[1], NULL);
+		}
 	}
-		
+			
+	assert(!isnan(Ex));
+	assert(!isnan(Ey));
+	
 	result[0] = Ex;
 	result[1] = Ey;
 	result[2] = 0.0;
 }
 
 struct field_evaluation_args {
-	double *vertices;
 	double *charges;
+	double *jacobian_buffer;
+	double *position_buffer;
 	size_t N_vertices;
+	double *bounds;
 };
 
 void
-field_radial_traceable(double point[3], double result[3], void *args_p) {
+field_radial_traceable_bounds(double point[3], double result[3], void *args_p) {
 
 	struct field_evaluation_args *args = (struct field_evaluation_args*)args_p;
-	field_radial(point, result, (vertices_2d) args->vertices, (charges_2d) args->charges, args->N_vertices);
+
+	double (*bounds)[2] = (double (*)[2]) args->bounds;
+		
+	if( (bounds[0][0] < point[0]) && (point[0] < bounds[0][1])
+		&& (bounds[1][0] < point[1]) && (point[1] < bounds[1][1]) ) {
+		field_radial(point, result, args->charges, (jacobian_buffer_2d) args->jacobian_buffer, (position_buffer_2d) args->position_buffer, args->N_vertices);
+	}
+	else {
+		result[0] = 0.0;
+		result[1] = 0.0;
+		result[2] = 0.0;
+	}
+}
+
+void
+field_radial_traceable(double point[3], double result[3], void *args_p) {
+	
+	struct field_evaluation_args *args = (struct field_evaluation_args*)args_p;
+	
+	field_radial(point, result, args->charges, (jacobian_buffer_2d) args->jacobian_buffer, (position_buffer_2d) args->position_buffer, args->N_vertices);
 }
 
 EXPORT size_t
-trace_particle_radial(double *times_array, double *pos_array, double bounds[3][2], double atol,
-	double *vertices, double *charges, size_t N_vertices) {
+trace_particle_radial(double *times_array, double *pos_array, double tracer_bounds[3][2], double atol,
+	double *charges, jacobian_buffer_2d jac_buffer, position_buffer_2d pos_buffer, size_t N_vertices, double *field_bounds) {
 
-	struct field_evaluation_args args = { vertices, charges, N_vertices };
-				
-	return trace_particle(times_array, pos_array, field_radial_traceable, bounds, atol, (void*) &args);
+	struct field_evaluation_args args = {charges, (double*)jac_buffer, (double*)pos_buffer, N_vertices, field_bounds };
+		
+	if (field_bounds == NULL) {
+		return trace_particle(times_array, pos_array, field_radial_traceable, tracer_bounds, atol, (void*) &args);
+	}
+	else {
+		return trace_particle(times_array, pos_array, field_radial_traceable_bounds, tracer_bounds, atol, (void*) &args);
+	}
 }
 
 EXPORT void
 field_radial_derivs(double point[3], double field[3], double *z_inter, double *coeff_p, size_t N_z) {
 	
 	double (*coeff)[DERIV_2D_MAX][6] = (double (*)[DERIV_2D_MAX][6]) coeff_p;
 	
@@ -720,44 +796,36 @@
 
 EXPORT double dz1_potential_3d_point(double x0, double y0, double z0, double x, double y, double z, void *_) {
 	double r = norm_3d(x-x0, y-y0, z-z0);
     return (z-z0)/(4*pow(r, 3));
 }
 
 EXPORT void
-axial_coefficients_3d(double *restrict vertices_p, double *restrict charges, size_t N_v,
+axial_coefficients_3d(double *restrict charges,
+	jacobian_buffer_3d jacobian_buffer,
+	position_buffer_3d position_buffer,
+	size_t N_v,
 	double *restrict zs, double *restrict output_coeffs_p, size_t N_z,
 	double *restrict thetas, double *restrict theta_coeffs_p, size_t N_t) {
-	
-	double (*vertices)[3][3] = (double (*)[3][3]) vertices_p;
+		
 	double (*theta_coeffs)[NU_MAX][M_MAX][4] = (double (*)[NU_MAX][M_MAX][4]) theta_coeffs_p;
 	double (*output_coeffs)[2][NU_MAX][M_MAX] = (double (*)[2][NU_MAX][M_MAX]) output_coeffs_p;
-
+	
 	double theta0 = thetas[0];
 	double dtheta = thetas[1] - thetas[0];
 	
 	for(int h = 0; h < N_v; h++) {
-
-		double v1x = vertices[h][0][0], v1y = vertices[h][0][1], v1z = vertices[h][0][2];
-		double v2x = vertices[h][1][0], v2y = vertices[h][1][1], v2z = vertices[h][1][2];
-		double v3x = vertices[h][2][0], v3y = vertices[h][2][1], v3z = vertices[h][2][2];
-			
-		double area = 0.5*sqrt(pow((v2y-v1y)*(v3z-v1z)-(v2z-v1z)*(v3y-v1y), 2) + pow((v2z-v1z)*(v3x-v1x)-(v2x-v1x)*(v3z-v1z), 2) + pow((v2x-v1x)*(v3y-v1y)-(v2y-v1y)*(v3x-v1x), 2));
-		
         for (int i=0; i < N_z; i++) 
+		
 		UNROLL
 		for (int k=0; k < N_TRIANGLE_QUAD; k++) {
-			double b1_ = QUAD_B1[k];
-			double b2_ = QUAD_B2[k];
-			double w = QUAD_WEIGHTS[k];
-
-			double x = v1x + b1_*(v2x-v1x) + b2_*(v3x-v1x);
-			double y = v1y + b1_*(v2y-v1y) + b2_*(v3y-v1y);
-			double z = v1z + b1_*(v2z-v1z) + b2_*(v3z-v1z);
-
+			double x = position_buffer[h][k][0];
+			double y = position_buffer[h][k][1];
+			double z = position_buffer[h][k][2];
+			
 			double r = norm_3d(x, y, z-zs[i]);
 			double theta = atan2((z-zs[i]), norm_2d(x, y));
 			double mu = atan2(y, x);
 
 			int index = (int) ((theta-theta0)/dtheta);
 
 			double t = theta-thetas[index];
@@ -766,37 +834,43 @@
 			UNROLL
 			for (int nu=0; nu < NU_MAX; nu++)
 			UNROLL
 			for (int m=0; m < M_MAX; m++) {
 				double base = pow(t, 3)*C[nu][m][0] + pow(t, 2)*C[nu][m][1] + t*C[nu][m][2] + C[nu][m][3];
 				double r_dependence = pow(r, -2*nu - m - 1);
 					
-				output_coeffs[i][0][nu][m] += charges[h]*area*w*base*cos(m*mu)*r_dependence;
-				output_coeffs[i][1][nu][m] += charges[h]*area*w*base*sin(m*mu)*r_dependence;
+				double jac = jacobian_buffer[h][k];
+				
+				output_coeffs[i][0][nu][m] += charges[h]*jac*base*cos(m*mu)*r_dependence;
+				output_coeffs[i][1][nu][m] += charges[h]*jac*base*sin(m*mu)*r_dependence;
 			}
 		}
 	}
 }
 
 
 //////////////////////////////// 3D POINT POTENTIAL EVALUATION
 
-EXPORT double
-potential_3d(double point[3], double *vertices_p, double *charges, size_t N_vertices) {
-
-	double (*vertices)[3][3] = (double (*)[3][3]) vertices_p;	
-
-	double sum_ = 0.0;
+EXPORT double  
+potential_3d(double point[3], double *charges, jacobian_buffer_3d jacobian_buffer, position_buffer_3d position_buffer, size_t N_vertices) {  
 	
-	for(int i = 0; i < N_vertices; i++) {
-		sum_ += charges[i] * triangle_integral(point, vertices[i][0], vertices[i][1], vertices[i][2], potential_3d_point, NULL);
-	}
+	double sum_ = 0.0;  
+	
+	for(int i = 0; i < N_vertices; i++) {  
+		for(int k = 0; k < N_TRIANGLE_QUAD; k++) {
+			double *pos = &position_buffer[i][k][0];
+			double potential = potential_3d_point(point[0], point[1], point[2], pos[0], pos[1], pos[2], NULL);
+			
+			sum_ += charges[i] * jacobian_buffer[i][k] * potential;
+		}
+	}  
 	
 	return sum_;
-}
+}  
+
 
 EXPORT double
 potential_3d_derivs(double point[3], double *zs, double *coeffs_p, size_t N_z) {
 
 	double (*coeffs)[2][NU_MAX][M_MAX][4] = (double (*)[2][NU_MAX][M_MAX][4]) coeffs_p;
 	
 	double xp = point[0], yp = point[1], zp = point[2];
@@ -839,51 +913,77 @@
 	double Ez = -dz1_potential_3d_point(x0, y0, z0, x, y, z, NULL);
 	
 	double *normal = (double *)normal_p;
 	
     return normal[0]*Ex + normal[1]*Ey + normal[2]*Ez;
 }
 
-
 EXPORT void
-field_3d(double point[3], double result[3], double *vertices_p, double *charges, size_t N_vertices) {
-	
-		double (*vertices)[3][3] = (double (*)[3][3]) vertices_p;
-		
-		double Ex = 0.0, Ey = 0.0, Ez = 0.0;
+field_3d(double point[3], double result[3], double *charges,
+	jacobian_buffer_3d jacobian_buffer, position_buffer_3d position_buffer, size_t N_vertices) {
+
+	double Ex = 0.0, Ey = 0.0, Ez = 0.0;
+
+	for(int i = 0; i < N_vertices; i++) {
+		for(int k = 0; k < N_TRIANGLE_QUAD; k++) {
+			double *pos = &position_buffer[i][k][0];
+			double field_x = dx1_potential_3d_point(point[0], point[1], point[2], pos[0], pos[1], pos[2], NULL);
+			double field_y = dy1_potential_3d_point(point[0], point[1], point[2], pos[0], pos[1], pos[2], NULL);
+			double field_z = dz1_potential_3d_point(point[0], point[1], point[2], pos[0], pos[1], pos[2], NULL);
+		
+			Ex -= charges[i] * jacobian_buffer[i][k] * field_x;
+			Ey -= charges[i] * jacobian_buffer[i][k] * field_y;
+			Ez -= charges[i] * jacobian_buffer[i][k] * field_z;
+		}
+	}
 		
-		for(int i = 0; i < N_vertices; i++) {
-			
-			double *v1, *v2, *v3;
-			v1 = &vertices[i][0][0], v2 = &vertices[i][1][0], v3 = &vertices[i][2][0];
-			
-			Ex -= charges[i]*triangle_integral(point, v1, v2, v3, dx1_potential_3d_point, NULL);
-			Ey -= charges[i]*triangle_integral(point, v1, v2, v3, dy1_potential_3d_point, NULL);
-			Ez -= charges[i]*triangle_integral(point, v1, v2, v3, dz1_potential_3d_point, NULL);
-		} 
+	result[0] = Ex;
+	result[1] = Ey;
+	result[2] = Ez;
+}
+
+void
+field_3d_traceable_bounds(double point[3], double result[3], void *args_p) {
+
+	struct field_evaluation_args *args = (struct field_evaluation_args*)args_p;
 
-		result[0] = Ex;
-		result[1] = Ey;
-		result[2] = Ez;
+	double (*bounds)[2] = (double (*)[2]) args->bounds;
+	
+	if(	   (bounds[0][0] < point[0]) && (point[0] < bounds[0][1])
+		&& (bounds[1][0] < point[1]) && (point[1] < bounds[1][1])
+		&& (bounds[2][0] < point[2]) && (point[2] < bounds[2][1]) ) {
+
+		field_3d(point, result, args->charges, (jacobian_buffer_3d) args->jacobian_buffer, (position_buffer_3d) args->position_buffer, args->N_vertices);
+	}
+	else {
+		result[0] = 0.0;
+		result[1] = 0.0;
+		result[2] = 0.0;
+	}
 }
 
 void
 field_3d_traceable(double point[3], double result[3], void *args_p) {
 
 	struct field_evaluation_args *args = (struct field_evaluation_args*)args_p;
-	field_3d(point, result, args->vertices, args->charges, args->N_vertices);
+	field_3d(point, result, args->charges, (jacobian_buffer_3d) args->jacobian_buffer, (position_buffer_3d) args->position_buffer, args->N_vertices);
 }
 
 EXPORT size_t
-trace_particle_3d(double *times_array, double *pos_array, double bounds[3][2], double atol,
-	double *vertices, double *charges, size_t N_vertices) {
+trace_particle_3d(double *times_array, double *pos_array, double tracer_bounds[3][2], double atol,
+	double* charges, jacobian_buffer_3d jacobian_buffer, position_buffer_3d position_buffer, size_t N_vertices, double *field_bounds) {
 
-	struct field_evaluation_args args = { vertices, charges, N_vertices };
+	struct field_evaluation_args args = {charges, (double*) jacobian_buffer, (double*) position_buffer, N_vertices, field_bounds};
 				
-	return trace_particle(times_array, pos_array, field_3d_traceable, bounds, atol, (void*) &args);
+	if(field_bounds == NULL) {
+		return trace_particle(times_array, pos_array, field_3d_traceable, tracer_bounds, atol, (void*) &args);
+	}
+	else {
+		return trace_particle(times_array, pos_array, field_3d_traceable_bounds, tracer_bounds, atol, (void*) &args);
+	}
 }
 
 EXPORT void
 field_3d_derivs(double point[3], double field[3], double *restrict zs, double *restrict coeffs_p, size_t N_z) {
 	
 	double (*coeffs)[2][NU_MAX][M_MAX][4] = (double (*)[2][NU_MAX][M_MAX][4]) coeffs_p;
 
@@ -961,380 +1061,408 @@
 enum ExcitationType{
     VOLTAGE_FIXED = 1,
     VOLTAGE_FUN = 2,
     DIELECTRIC = 3,
     FLOATING_CONDUCTOR = 4};
 
 
-double legendre(int N, double x) {
-	switch(N) {
-		case 0:
-			return 1;
-		case 1:
-			return x;
-		case 2:
-			return (3*pow(x,2)-1)/2.;
-		case 3:
-			return (5*pow(x,3) -3*x)/2.;
-		case 4:
-			return (35*pow(x,4)-30*pow(x,2)+3)/8.;
-		case 5:
-			return (63*pow(x,5)-70*pow(x,3)+15*x)/8.;
-		case 6:
-			return (231*pow(x,6)-315*pow(x,4)+105*pow(x,2)-5)/16.;
-		case 7:
-			return (429*pow(x,7)-693*pow(x,5)+315*pow(x,3)-35*x)/16.;
-		case 8:
-			return (6435*pow(x,8) - 12012*pow(x,6) + 6930*pow(x,4) - 1260*pow(x,2) + 35) / 128;
-		/*case 9:
-			return (12155*pow(x,9) - 25740*pow(x,7) + 18018*pow(x,5) - 4620*pow(x,3) + 315*x) / 128;
-		case 10:
-			return (46189*pow(x,10) - 109395*pow(x,8) + 90090*pow(x,6) - 30030*pow(x,4) + 3465*pow(x,2) - 63) / 256;
-		case 11:
-			return (88179*pow(x,11) - 230945*pow(x,9) + 218790*pow(x,7) - 90090*pow(x,5) + 15015*pow(x,3) - 693*x) / 256;
-		case 12:
-			return (676039*pow(x,12) - 1939938*pow(x,10) + 2078505*pow(x,8) - 1021020*pow(x,6) + 225225*pow(x,4) - 18018*pow(x,2) + 231) / 1024;
-		case 13:
-			return (1300075*pow(x,13) - 4056234*pow(x,11) + 4849845*pow(x,9) - 2771340*pow(x,7) + 765765*pow(x,5) - 90090*pow(x,3) + 3003*x) / 1024;
-		case 14:
-			return (5014575*pow(x,14) - 16900975*pow(x,12) + 22309287*pow(x,10) - 14549535*pow(x,8) + 4849845*pow(x,6) - 765765*pow(x,4) + 45045*pow(x,2) - 429) / 2048;
-		case 15:
-			return (9694845*pow(x,15) - 35102025*pow(x,13) + 50702925*pow(x,11) - 37182145*pow(x,9) + 14549535*pow(x,7) - 2909907*pow(x,5) + 255255*pow(x,3) - 6435*x) / 2048;
-		case 16:
-			return (300540195*pow(x,16) - 1163381400*pow(x,14) + 1825305300*pow(x,12) - 1487285800*pow(x,10) + 669278610*pow(x,8) - 162954792*pow(x,6) + 19399380*pow(x,4) - 875160*pow(x,2) + 6435) / 32768;*/
-	}
-	exit(1);
-}
-
-
-// Modified weight taking into account that the charge contribution
-// is a sum of Legendre polynomials.
-double legendre_log_weight(int k, int l, double legendre_arg) {
-
-	double sum_ = 0.0;
-
-	for(int i = 0; i < N_QUAD_2D; i++)
-		sum_ += GAUSS_QUAD_WEIGHTS[k] * GAUSS_LOG_QUAD_WEIGHTS[l] * (2*i + 1)/2. * legendre(i, GAUSS_QUAD_POINTS[k]) * legendre(i, legendre_arg);
-	
-	return sum_;
-}
-
+struct self_voltage_radial_args {
+	double (*line_points)[3];
+	double *target;
+	integration_cb_2d cb_fun;
+	double *normal;
+	double K;
+};
 
-double log_integral(
-	double *v1,
-	double *v2,
-	double *v3,
-	double *v4,
-	int row, int k,
-	integration_cb_2d callback, void *args) {
+double self_voltage_radial(double alpha, void *args_p) {
 	
-	double s = GAUSS_QUAD_POINTS[row];
+	struct self_voltage_radial_args* args = (struct self_voltage_radial_args*) args_p;
 	
-	double spos[2], jac;
-	position_and_jacobian_radial(s, v1, v2, v3, v4, spos, &jac);
+	double *v1 = args->line_points[0];
+	double *v2 = args->line_points[2];
+	double *v3 = args->line_points[3];
+	double *v4 = args->line_points[1];
 	
-	double spos_left1[2];
-	position_and_jacobian_radial( -1 + 2*(s+1)/3., v1, v2, v3, v4, spos_left1, &jac);
+	double pos[2], jac;
+	position_and_jacobian_radial(alpha, v1, v2, v3, v4, pos, &jac);
 	
-	double spos_left2[2];
-	position_and_jacobian_radial( -1 + (s+1)/3., v1, v2, v3, v4, spos_left2, &jac);
+	struct {double *normal; double K;} cb_args = {args->normal, args->K};
 	
-	double spos_right1[2];
-	position_and_jacobian_radial( s + (1-s)/3, v1, v2, v3, v4, spos_right1, &jac);
-	
-	double spos_right2[2];
-	position_and_jacobian_radial( s + 2*(1-s)/3, v1, v2, v3, v4, spos_right2, &jac);
-
-	double integration_sum = 0.0;
-	
-	// Logarithmic integration using improved quadrature weights
-	// split the integration around the singularity
-	for(int l = 0; l < N_LOG_QUAD_2D; l++) {
-		
-		// To left direction
-		double local_alpha = 2*GAUSS_LOG_QUAD_POINTS[l] - 1;
-		double global_alpha = s + GAUSS_LOG_QUAD_POINTS[l]*(-s-1);
-		
-		assert( (-1<local_alpha) && (local_alpha<1) );
-		assert( (-1<global_alpha) && (global_alpha<1) );
-		
-		double pos[2], jac;
-		position_and_jacobian_radial(local_alpha, spos, spos_left1, spos_left2, v1, pos, &jac);
-		double pot_ring = callback(spos[0], spos[1], pos[0], pos[1], args);
-		integration_sum += 2*jac * legendre_log_weight(k, l, global_alpha) * pot_ring;
-		// To right direction
-		global_alpha = s + GAUSS_LOG_QUAD_POINTS[l]*(1-s);
-			
-		assert( (-1<local_alpha) && (local_alpha<1) );
-		assert( (-1<global_alpha) && (global_alpha<1) );
-		
-		position_and_jacobian_radial(local_alpha, spos, spos_right1, spos_right2, v4, pos, &jac);
-		pot_ring = callback(spos[0], spos[1], pos[0], pos[1], args);
-		integration_sum += 2*jac * legendre_log_weight(k, l, global_alpha) * pot_ring;
-	}
-	
-	return integration_sum;
+	//printf("normal: %f, %f\n", args->normal[0], args->normal[1]);	
+	return jac * args->cb_fun(args->target[0], args->target[1], pos[0], pos[1], &cb_args);
 }
 
-void fill_self_voltages(double *matrix, 
+void fill_self_voltages_radial(double *matrix, 
                         vertices_2d line_points,
 						uint8_t *excitation_types,
 						double *excitation_values,
 						size_t N_lines,
 						size_t N_matrix,
                         int lines_range_start, 
                         int lines_range_end) {
 	 
+	gsl_integration_workspace * w = gsl_integration_workspace_alloc(ADAPTIVE_MAX_ITERATION);
+	
 	for(int i = lines_range_start; i <= lines_range_end; i++) {
-		
 		double *v1 = &line_points[i][0][0];
 		double *v2 = &line_points[i][2][0];
 		double *v3 = &line_points[i][3][0];
 		double *v4 = &line_points[i][1][0];
 		
+		double target[2], jac;
+		position_and_jacobian_radial(0.0, v1, v2, v3, v4, target, &jac);
+		
+		double normal[2];
+		higher_order_normal_radial(0.0, v1, v2, v3, v4, normal);
+		//normal_2d(v1, v2, normal);
+			
 		enum ExcitationType type_ = excitation_types[i];
 			
-		if (type_ == VOLTAGE_FIXED || type_ == VOLTAGE_FUN || type_ == FLOATING_CONDUCTOR) {
-			for(int l = 0; l < N_QUAD_2D; l++) 
-			for(int k = 0; k < N_QUAD_2D; k++) {
+		//printf("Type: %d\n", type_);
+		struct self_voltage_radial_args integration_args = {
+			.target = target,
+			.line_points = &line_points[i][0],
+			.normal = normal,
+			.K = excitation_values[i],
+			.cb_fun = (type_ != DIELECTRIC) ? potential_radial_ring : field_dot_normal_radial
+		};
+			
+		gsl_function F;
+		F.function = &self_voltage_radial;
+		F.params = &integration_args;
+			
+		double result, error;
+		double singular_points[3] = {-1, 0, 1};
+		gsl_integration_qagp(&F, singular_points, 3, 1e-9, 5e-5, ADAPTIVE_MAX_ITERATION, w, &result, &error);
 
-				matrix[(N_QUAD_2D*i + l)*N_matrix + N_QUAD_2D*i + k] = log_integral(v1, v2, v3, v4, l, k, potential_radial_ring, NULL);
-			}
+		if(type_ == DIELECTRIC) {
+			matrix[N_matrix*i + i] = result - 1;
 		}
-		else if(type_ == DIELECTRIC) {
-			for(int l = 0; l < N_QUAD_2D; l++)  {
-				for(int k = 0; k < N_QUAD_2D; k++) {
-
-					double normal[2];
-					higher_order_normal_radial(GAUSS_QUAD_POINTS[l], v1, v2, v3, v4, normal);
-					double K = excitation_values[i];
-
-					struct {double *normal; double K;} args = {normal, K};
-
-					matrix[(N_QUAD_2D*i + l)*N_matrix + N_QUAD_2D*i + k] = log_integral(v1, v2, v3, v4, l, k, field_dot_normal_radial, &args);
-				}
-				// When working with dielectrics, the constraint is that
-				// the electric field normal must sum to the surface charge.
-				// The constraint is satisfied by subtracting the integral
-				// over the charge from the line element.
-				matrix[(N_QUAD_2D*i + l)*N_matrix + N_QUAD_2D*i + l] -= 1;
-			}
+		else {
+			matrix[N_matrix*i + i] = result;
 		}
 	}
+	
+	gsl_integration_workspace_free(w);
 }
 
-EXPORT void add_floating_conductor_constraints_radial(double *matrix, vertices_2d vertices, size_t N_matrix, int64_t *indices, size_t N_indices, int row) {
-	for(int j = 0; j < N_indices; j++) {
-		int i = indices[j];
-			
-		double *v1 = &vertices[i][0][0];
-		double *v2 = &vertices[i][2][0]; // Strange ordering following from GMSH line4 element
-		double *v3 = &vertices[i][3][0];
-		double *v4 = &vertices[i][1][0];
-			
-		// An extra unknown voltage is added to the matrix for every floating conductor.
-		// The column related to this unknown voltage is positioned at the rightmost edge of the matrix.
-		// If multiple floating conductors are present the column lives at -len(floating) + i
-		for(int k = 0; k < N_QUAD_2D; k++) {
-			double pos[2], jac;
-			position_and_jacobian_radial(GAUSS_QUAD_POINTS[k], v1, v2, v3, v4, pos, &jac);
+EXPORT void fill_jacobian_buffer_radial(
+	jacobian_buffer_2d jacobian_buffer,
+	position_buffer_2d pos_buffer,
+    vertices_2d line_points,
+    size_t N_lines) {
+	
+    for(int i = 0; i < N_lines; i++) {  
+        for (int k=0; k < N_QUAD_2D; k++) {  
+			double *v1 = &line_points[i][0][0];
+			double *v2 = &line_points[i][2][0];
+			double *v3 = &line_points[i][3][0];
+			double *v4 = &line_points[i][1][0];
+				
+            double pos[2], jac;  
 			
-			matrix[(N_QUAD_2D*i + k)*N_matrix + N_matrix - row - 1] = -1;
-			// See charge_radial function
-			matrix[(N_matrix - row - 1)*N_matrix + N_QUAD_2D*i + k] = 2*M_PI*pos[0]*GAUSS_QUAD_WEIGHTS[k]*jac;
-		}
-	}
+            position_and_jacobian_radial(GAUSS_QUAD_POINTS[k], v1, v2, v3, v4, pos, &jac);  
+			
+            jacobian_buffer[i][k] = GAUSS_QUAD_WEIGHTS[k]*jac;  
+            pos_buffer[i][k][0] = pos[0];  
+            pos_buffer[i][k][1] = pos[1];  
+        }  
+    }  
 }
 
 
-
 EXPORT void fill_matrix_radial(double *matrix, 
 						vertices_2d line_points,
                         uint8_t *excitation_types, 
                         double *excitation_values, 
+						jacobian_buffer_2d jacobian_buffer,
+						position_buffer_2d pos_buffer,
 						size_t N_lines,
 						size_t N_matrix,
                         int lines_range_start, 
                         int lines_range_end) {
     
 	assert(lines_range_start < N_lines && lines_range_end < N_lines);
-	assert(N_matrix >= N_QUAD_2D*N_lines);
+	assert(N_matrix >= N_lines);
 		
     for (int i = lines_range_start; i <= lines_range_end; i++) {
 		
 		double *target_v1 = &line_points[i][0][0];
 		double *target_v2 = &line_points[i][2][0];
 		double *target_v3 = &line_points[i][3][0];
 		double *target_v4 = &line_points[i][1][0];
 		
+		double target[2], jac;
+		position_and_jacobian_radial(0.0, target_v1, target_v2, target_v3, target_v4, target, &jac);
+		
 		enum ExcitationType type_ = excitation_types[i];
 			
 		if (type_ == VOLTAGE_FIXED || type_ == VOLTAGE_FUN || type_ == FLOATING_CONDUCTOR) {
 			for (int j = 0; j < N_lines; j++) {
 				
-				if (i == j) continue;
-					
-				double *v1 = &line_points[j][0][0];
-				double *v2 = &line_points[j][2][0]; // Strange ordering following from GMSH line4 element
-				double *v3 = &line_points[j][3][0];
-				double *v4 = &line_points[j][1][0];
-					
-				for(int l = 0; l < N_QUAD_2D; l++) {
-					double target[2], jac_t;
-					position_and_jacobian_radial(GAUSS_QUAD_POINTS[l], target_v1, target_v2, target_v3, target_v4, target, &jac_t);
-						
-					for(int k = 0; k < N_QUAD_2D; k++) {
-						
-						double pos[2], jac;
-						position_and_jacobian_radial(GAUSS_QUAD_POINTS[k], v1, v2, v3, v4, pos, &jac);
+				UNROLL
+				for(int k = 0; k < N_QUAD_2D; k++) {
 						
-						matrix[(N_QUAD_2D*i + l)*N_matrix + N_QUAD_2D*j + k] = GAUSS_QUAD_WEIGHTS[k]*jac*potential_radial_ring(target[0], target[1], pos[0], pos[1], NULL);
-					}
+					double *pos = pos_buffer[j][k];
+					double jac = jacobian_buffer[j][k];
+					matrix[i*N_matrix + j] += jac * potential_radial_ring(target[0], target[1], pos[0], pos[1], NULL);
 				}
-			} 
+            }
 		}
 		else if(type_ == DIELECTRIC) {
-			            
-            for (int j = 0; j < N_lines; j++) {
+			for (int j = 0; j < N_lines; j++) {
 
-				if(i == j) continue;
-					
-				double *v1 = &line_points[j][0][0];
-				double *v2 = &line_points[j][2][0]; // Strange ordering following from GMSH line4 element
-				double *v3 = &line_points[j][3][0];
-				double *v4 = &line_points[j][1][0];
-				
-				for(int l = 0; l < N_QUAD_2D; l++) {
-					
-					double normal[2];
-					higher_order_normal_radial(GAUSS_QUAD_POINTS[l], target_v1, target_v2, target_v3, target_v4, normal);
-					double K = excitation_values[i];
+				double normal[2];
+				//normal_2d(target_v1, target_v2, normal);
+				higher_order_normal_radial(0.0, target_v1, target_v2, target_v3, target_v4, normal);
 					
-					struct {double *normal; double K;} args = {normal, K};
-
-					double target[2], jac_t;
-					position_and_jacobian_radial(GAUSS_QUAD_POINTS[l], target_v1, target_v2, target_v3, target_v4, target, &jac_t);
+				struct {double *normal; double K;} args = {normal, excitation_values[i]};
 					
-					for(int k = 0; k < N_QUAD_2D; k++) {
+				UNROLL
+				for(int k = 0; k < N_QUAD_2D; k++) {
 						
-						double pos[2], jac;
-						position_and_jacobian_radial(GAUSS_QUAD_POINTS[k], v1, v2, v3, v4, pos, &jac);
-						matrix[(N_QUAD_2D*i + l)*N_matrix + N_QUAD_2D*j + k] = GAUSS_QUAD_WEIGHTS[k]*jac*field_dot_normal_radial(target[0], target[1], pos[0], pos[1], &args);
-					}
+					double *pos = pos_buffer[j][k];
+					double jac = jacobian_buffer[j][k];
+					matrix[i*N_matrix + j] += jac * field_dot_normal_radial(target[0], target[1], pos[0], pos[1], &args);
 				}
-            }
+			}
 		}
 		else {
 		    printf("ExcitationType unknown");
             exit(1);
 		}
 	}
 	
-	fill_self_voltages(matrix, line_points, excitation_types, excitation_values, N_lines, N_matrix, lines_range_start, lines_range_end);
+	fill_self_voltages_radial(matrix, line_points, excitation_types, excitation_values, N_lines, N_matrix, lines_range_start, lines_range_end);
+}
+
+void fill_self_voltages_3d(double *matrix, 
+                        vertices_3d triangle_points,
+						uint8_t *excitation_types,
+						double *excitation_values,
+						size_t N_lines,
+						size_t N_matrix,
+                        int lines_range_start, 
+                        int lines_range_end) {
+
+	for (int i = lines_range_start; i <= lines_range_end; i++) {
+		
+		double (*v)[3] = &triangle_points[i][0];
+				
+		// Target
+		double t[3], jac;
+		position_and_jacobian_3d(1/3., 1/3., &triangle_points[i][0], t, &jac);
+
+		double s0[3], s1[3], s2[3];
+		position_and_jacobian_3d(1/6., 1/6., &triangle_points[i][0], s0, &jac);
+		position_and_jacobian_3d(4/6., 1/6., &triangle_points[i][0], s1, &jac);
+		position_and_jacobian_3d(1/6., 4/6., &triangle_points[i][0], s2, &jac);
+					
+		triangle6 triangle1 = {
+			{ t[0], t[1], t[2] },
+			{ v[0][0], v[0][1], v[0][2] },
+			{ v[1][0], v[1][1], v[1][2] },
+			{ s0[0], s0[1], s0[2] },
+			{ v[3][0], v[3][1], v[3][2] },
+			{ s1[0], s1[1], s1[2] } };
+		
+		triangle6 triangle2 = {
+			{ t[0], t[1], t[2] },
+			{ v[1][0], v[1][1], v[1][2] },
+			{ v[2][0], v[2][1], v[2][2] },
+			{ s1[0], s1[1], s1[2] },
+			{ v[4][0], v[4][1], v[4][2] },
+			{ s2[0], s2[1], s2[2] } };
+			
+		triangle6 triangle3 = {
+			{ t[0], t[1], t[2] },
+			{ v[2][0], v[2][1], v[2][2] },
+			{ v[0][0], v[0][1], v[0][2] },
+			{ s2[0], s2[1], s2[2] },
+			{ v[5][0], v[5][1], v[5][2] },
+			{ s0[0], s0[1], s0[2] } };
+
+		if(excitation_types[i] != DIELECTRIC) {
+			matrix[i*N_matrix + i] = 0.0;
+			matrix[i*N_matrix + i] += triangle_integral_adaptive(t, triangle1, potential_3d_point, NULL);
+			matrix[i*N_matrix + i] += triangle_integral_adaptive(t, triangle2, potential_3d_point, NULL);
+			matrix[i*N_matrix + i] += triangle_integral_adaptive(t, triangle3, potential_3d_point, NULL);
+		}
+		else {
+			matrix[i*N_matrix + i] = -1.0;
+		}
+	}
 }
 
+EXPORT void fill_jacobian_buffer_3d(
+	jacobian_buffer_3d jacobian_buffer,
+	position_buffer_3d pos_buffer,
+    vertices_3d triangle_points,
+    size_t N_lines) {
+		
+    for(int i = 0; i < N_lines; i++) {  
+        for (int k=0; k < N_TRIANGLE_QUAD; k++) {  
+            double b1_ = QUAD_B1[k];  
+            double b2_ = QUAD_B2[k];  
+            double w = QUAD_WEIGHTS[k];  
+			
+            double pos[3], jac;  
+            position_and_jacobian_3d(b1_, b2_, &triangle_points[i][0], pos, &jac);  
+			
+            jacobian_buffer[i][k] = w*jac;  
+            pos_buffer[i][k][0] = pos[0];  
+            pos_buffer[i][k][1] = pos[1];  
+            pos_buffer[i][k][2] = pos[2];  
+        }
+    }
+}
 
-EXPORT void fill_matrix_3d(double *matrix, 
-                    double *triangle_points_p, 
+EXPORT void fill_matrix_3d(double *restrict matrix, 
+                    vertices_3d triangle_points, 
                     uint8_t *excitation_types, 
                     double *excitation_values, 
+					jacobian_buffer_3d jacobian_buffer,
+					position_buffer_3d pos_buffer,
 					size_t N_lines,
 					size_t N_matrix,
                     int lines_range_start, 
                     int lines_range_end) {
-    
+		
 	assert(lines_range_start < N_lines && lines_range_end < N_lines);
-	double (*triangle_points)[3][3] = (double (*)[3][3]) triangle_points_p;
 		
     for (int i = lines_range_start; i <= lines_range_end; i++) {
-		double *p1 = &triangle_points[i][0][0];
-		double *p2 = &triangle_points[i][1][0];
-		double *p3 = &triangle_points[i][2][0];
-		double target[3] = {(p1[0] + p2[0] + p3[0])/3, (p1[1] + p2[1] + p3[1])/3, (p1[2] + p2[2] + p3[2])/3};
+		// TODO: higher order
+		double target[3], jac;
+		position_and_jacobian_3d(1/3., 1/3., &triangle_points[i][0], target, &jac);
+			
         enum ExcitationType type_ = excitation_types[i];
 		 
         if (type_ == VOLTAGE_FIXED || type_ == VOLTAGE_FUN || type_ == FLOATING_CONDUCTOR) {
             for (int j = 0; j < N_lines; j++) {
-                double *v1 = &triangle_points[j][0][0];
-                double *v2 = &triangle_points[j][1][0];
-                double *v3 = &triangle_points[j][2][0];
-                matrix[i*N_matrix + j] = triangle_integral_potential_3d_point(target, v1, v2, v3);
+				
+				UNROLL
+				for(int k = 0; k < N_TRIANGLE_QUAD; k++) {
+						
+					double *pos = pos_buffer[j][k];
+					double jac = jacobian_buffer[j][k];
+					matrix[i*N_matrix + j] += jac * potential_3d_point(target[0], target[1], target[2], pos[0], pos[1], pos[2], NULL);
+				}
             }
         } 
-        else if (type_ == DIELECTRIC) {
-            double normal[3];
-            normal_3d(p1, p2, p3, normal);
-            double K = excitation_values[i];
-            
-            for (int j = 0; j < N_lines; j++) {
-				double *v1 = &triangle_points[j][0][0];
-                double *v2 = &triangle_points[j][1][0];
-                double *v3 = &triangle_points[j][2][0];
-				// See comments in 'fill_matrix_2d'.
-                double factor = (2*K - 2) / (M_PI*(1 + K));
-                matrix[i*N_matrix + j] = factor * triangle_integral(target, v1, v2, v3, field_dot_normal_3d, normal);
-				 
-                if (i == j) matrix[i*N_matrix + j] -= 1.0;
-            }
-        }
+		else if (type_ == DIELECTRIC) {  
+			double *p1 = &triangle_points[i][0][0];  
+			double *p2 = &triangle_points[i][1][0];  
+			double *p3 = &triangle_points[i][2][0];  
+
+			double normal[3];  
+			normal_3d(p1, p2, p3, normal);  
+			double K = excitation_values[i];  
+
+			double factor = (2*K - 2) / (M_PI*(1 + K));  
+
+			for (int j = 0; j < N_lines; j++) {  
+					
+				UNROLL  
+				for(int k = 0; k < N_TRIANGLE_QUAD; k++) {  
+					double *pos = pos_buffer[j][k];  
+					double jac = jacobian_buffer[j][k];  
+					
+					matrix[i*N_matrix + j] += factor * jac * field_dot_normal_3d(target[0], target[1], target[2], pos[0], pos[1], pos[2], normal);  
+				}  
+			}  
+		}  
         else {
             printf("ExcitationType unknown");
             exit(1);
         }
     }
+	
+	fill_self_voltages_3d(matrix, triangle_points, excitation_types, excitation_values, N_lines, N_matrix, lines_range_start, lines_range_end);
 }
 
 EXPORT bool
-xy_plane_intersection_2d(double *positions_p, size_t N_p, double result[4], double z) {
-
-	double (*positions)[4] = (double (*)[4]) positions_p;
+plane_intersection(double p0[3], double normal[3], positions_3d positions, size_t N_p, double result[6]) {
+	
+	assert(N_p > 1);
+		
+	double xp = p0[0], yp = p0[1], zp = p0[2];
+	double xn = normal[0], yn = normal[1], zn = normal[2];
 
-	for(int i = N_p-1; i > 0; i--) {
+	// Initial sign
+	int i = N_p-1;
 	
-		double z1 = positions[i-1][1];
-		double z2 = positions[i][1];
+	double x = positions[i][0], y = positions[i][1], z = positions[i][2];	
+	double prev_kappa = (zn*zp-z*zn+yn*yp-y*yn+xn*xp-x*xn)/norm_3d(xn, yn, zn);
 		
-		if(fmin(z1, z2) <= z && z <= fmax(z1, z2)) {
-			double ratio = fabs( (z-z1)/(z1-z2) );
+	i -= 1;
 			
-			for(int k = 0; k < 4; k++)
-				result[k] = positions[i-1][k] + ratio*(positions[i][k] - positions[i-1][k]);
+	for(; i >= 0; i--) {
+		double x = positions[i][0], y = positions[i][1], z = positions[i][2];	
+		double kappa = (zn*zp-z*zn+yn*yp-y*yn+xn*xp-x*xn)/norm_3d(xn, yn, zn);
+		
+		int sign_kappa = kappa > 0 ? 1 : -1;
+		int sign_prev = prev_kappa > 0 ? 1 : -1;
+		
+		if(sign_kappa != sign_prev) {
+			double diff = kappa - prev_kappa;
+			
+			double factor = -prev_kappa / diff;
+			double prev_factor = kappa / diff;
+			
+			for(int k = 0; k < 6; k++)
+				result[k] = prev_factor*positions[i+1][k] + factor*positions[i][k];
 
 			return true;
 		}
+		
+		prev_kappa = kappa;
 	}
-
+	
 	return false;
 }
 
 EXPORT bool
-xy_plane_intersection_3d(double *positions_p, size_t N_p, double result[6], double z) {
-
-	double (*positions)[6] = (double (*)[6]) positions_p;
+line_intersection(double p0[2], double tangent[2], positions_2d positions, size_t N_p, double result[4]) {
+	
+	assert(N_p > 1);
+		
+	double xp = p0[0], yp = p0[1];
+	// Normal components, perpendicular to tangent
+	double xn = tangent[1], yn = -tangent[0];
 
-	for(int i = N_p-1; i > 0; i--) {
+	// Initial sign
+	int i = N_p-1;
 	
-		double z1 = positions[i-1][2];
-		double z2 = positions[i][2];
+	double x = positions[i][0], y = positions[i][1];
+	double prev_kappa = (yn*yp-y*yn+xn*xp-x*xn)/norm_2d(xn, yn);
 		
-		if(fmin(z1, z2) <= z && z <= fmax(z1, z2)) {
-			double ratio = fabs( (z-z1)/(z1-z2) );
+	i -= 1;
 			
-			for(int k = 0; k < 6; k++)
-				result[k] = positions[i-1][k] + ratio*(positions[i][k] - positions[i-1][k]);
+	for(; i >= 0; i--) {
+		double x = positions[i][0], y = positions[i][1];
+		double kappa = (yn*yp-y*yn+xn*xp-x*xn)/norm_2d(xn, yn);
+			
+		int sign_kappa = kappa > 0 ? 1 : -1;
+		int sign_prev = prev_kappa > 0 ? 1 : -1;
+		
+		if(sign_kappa != sign_prev) {
+			double diff = kappa - prev_kappa;
+			
+			double factor = -prev_kappa / diff;
+			double prev_factor = kappa / diff;
+			
+			for(int k = 0; k < 4; k++)
+				result[k] = prev_factor*positions[i+1][k] + factor*positions[i][k];
 
 			return true;
 		}
+		
+		prev_kappa = kappa;
 	}
-
+	
 	return false;
 }
 
 
 
 
 
-
-
-
-
-
```

### Comparing `traceon-0.2.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy` & `traceon-0.3.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy`

 * *Files identical despite different names*

### Comparing `traceon-0.2.0/traceon/data/radial-series-3D-thetas.npy` & `traceon-0.3.0/traceon/data/radial-series-3D-thetas.npy`

 * *Files identical despite different names*

### Comparing `traceon-0.2.0/traceon/excitation.py` & `traceon-0.3.0/traceon/excitation.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,28 @@
             calling the function as `add_dielectric(spacer=2)` assign the relative dielectric constant of 2 to the `spacer` physical group.
          
         """
         for name, permittivity in kwargs.items():
             assert name in self.electrodes
             self.excitation_types[name] = (ExcitationType.DIELECTRIC, permittivity)
 
+    def add_boundary(self, *args):
+        """
+        Specify geometry elements as boundary elements. At the boundary we require E·n = 0 at every point on the boundary. This
+        is equivalent to stating that the directional derivative of the potential through the boundary is zero. Placing boundaries between
+        the spaces of electrodes usually helps convergence tremendously. Note that a boundary is equivalent to a dielectric with a dielectric
+        constant of zero. This is how a boundary is actually implemented internally.
+        
+        Parameters
+        ----------
+        *args: list of str
+            The geometry names that should be considered a boundary.
+        """
+        self.add_dielectric(**{a:0 for a in args})
+
     def add_floating_conductor(self, **kwargs):
         """
         Specify geometric elements as floating conductors, and specify the total charge on the conductor.
          
         Parameters
         ----------
         **kwargs : dict
@@ -99,21 +113,14 @@
             a total charge on its surface equal to 10. For the unit of charge, see the section 'Units' on the `traceon` page.
             
         """
         for name, charge in kwargs.items():
             assert name in self.electrodes
             self.excitation_types[name] = (ExcitationType.FLOATING_CONDUCTOR, charge)
      
-    def _get_element_type(self):
-        if self.mesh.symmetry == Symmetry.THREE_D:
-            return 'triangle'
-        else:
-            return 'line4'
-    
-        
     def _split_for_superposition(self):
         
         # Names that have a fixed voltage excitation, not equal to 0.0
         types = self.excitation_types
         non_zero_fixed = [n for n, (t, v) in types.items() if t == ExcitationType.VOLTAGE_FIXED and v != 0.0]
         
         excitations = []
@@ -136,58 +143,63 @@
             exc = Excitation(self.mesh)
             exc.excitation_types = new_types_dict
             excitations.append(exc)
 
         assert len(non_zero_fixed) == len(excitations)
         return {n:e for (n,e) in zip(non_zero_fixed, excitations)}
 
+    def get_active_element_mask(self):
+        inactive = np.full(len(self.mesh.elements), True)
+        names = {}
+         
+        for name in self.excitation_types.keys():
+            inactive[ self.mesh.physical_to_elements[name] ] = False
+        
+        return ~inactive
+     
     def get_active_elements(self):
         """Get elements in the mesh that are active, in the sense that
         an excitation to them has been applied. 
     
         Returns
         --------
         A tuple of two elements: (points, names). points is a Numpy array of shape (N, 4, 3) in the case of 2D and (N, 3, 3) in the case of 3D. \
         This array contains the vertices of the line elements or the triangles. \
         Multiple points per line elements are used in the case of 2D since higher order BEM is employed, in which the true position on the line \
         element is given by a polynomial interpolation of the points. \
         names is a dictionary, the keys being the names of the physical groups mentioned by this excitation, \
         while the values are Numpy arrays of indices that can be used to index the points array.
         """
-        type_ = self._get_element_type()
-        mesh = self.mesh.mesh
-        vertices = mesh.cells_dict[type_] # Indices making up the lines and triangles
-        inactive = np.full(len(vertices), True)
-        names = {}
-        
-        for name in self.excitation_types.keys():
-            inactive[ mesh.cell_sets_dict[name][type_] ] = False
-        
+        vertices = self.mesh.elements
+        inactive = ~self.get_active_element_mask() 
         map_index = np.arange(len(vertices)) - np.cumsum(inactive)
-        
-        for name in self.excitation_types.keys():
-            names[name] = map_index[mesh.cell_sets_dict[name][type_]]
-              
-        return mesh.points[ vertices[~inactive] ], names
+        names = {n:map_index[i] for n, i in self.mesh.physical_to_elements.items() if n in self.excitation_types}
+         
+        return self.mesh.points[ vertices[~inactive] ], names
     
     def get_number_of_active_elements(self):
         """Get elements in the mesh that are active, in the sense that
         an excitation to them has been applied. This is the length of the points
         array returned by the `Excitation.get_active_elements`.
 
         Returns
         --------
         int, giving the number of elements. """
-        type_ = self._get_element_type()
-        mesh = self.mesh.mesh
-        
-        return sum(len(mesh.cell_sets_dict[n][type_]) for n in self.excitation_types.keys())
+        return sum(len(self.mesh.physical_to_elements[n]) for n in self.excitation_types.keys())
 
     def get_number_of_matrix_elements(self):
-        
+        """Gets the number of elements along one axis of the matrix. If this function returns N, the
+        matrix will have size NxN. The matrix consists of 64bit float values. Therefore the size of the matrix
+        in bytes is 8·NxN.
+
+        Returns
+        ---------
+        integer number
+        """
+         
         Nfloating = len([name for name, (type_, _) in self.excitation_types.items() if type_ == ExcitationType.FLOATING_CONDUCTOR])
         Nelem = self.get_number_of_active_elements()
          
         if self.mesh.symmetry == Symmetry.RADIAL:
             return Nelem*N_QUAD_2D + Nfloating
         elif self.mesh.symmetry == Symmetry.THREE_D:
             return Nelem + Nfloating
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `traceon-0.2.0/traceon/plotting.py` & `traceon-0.3.0/traceon/plotting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,186 +1,222 @@
-"""The `traceon.plotting` module uses `matplotlib` to provide some convenience functions
+"""The `traceon.plotting` module uses the `vedo` plotting library to provide some convenience functions
 to show the line and triangle meshes generated by Traceon."""
 
-import matplotlib.tri as mtri
-import matplotlib.pyplot as plt
-from matplotlib.collections import LineCollection
+from math import sqrt
 from scipy.interpolate import *
 import numpy as np
+import vedo
 
 from . import backend
+from .geometry import Symmetry
 
 def _create_point_to_physical_dict(mesh):
     d = {}
+
+    for k, v in mesh.physical_to_elements.items():
+        for elm in v:
+            for p in mesh.elements[elm]:
+                d[p] = k
     
-    for k, v in mesh.cell_sets_dict.items():
-        
-        if 'triangle' in v: 
-            for p in mesh.cells_dict['triangle'][v['triangle']]:
-                a, b, c = p
-                d[a], d[b], d[c] = k, k, k
-        
-        if 'line4' in v:
-            for l in mesh.cells_dict['line4'][v['line4']]:
-                a, b, c, e = l
-                d[a], d[b], d[c], d[e] = k, k, k, k
-     
     return d
 
-# Taken from
-# https://stackoverflow.com/questions/13685386/matplotlib-equal-unit-length-with-equal-aspect-ratio-z-axis-is-not-equal-to
-def _set_axes_equal(ax):
-    """Set 3D plot axes to equal scale.
-
-    Make axes of 3D plot have equal scale so that spheres appear as
-    spheres and cubes as cubes.  Required since `ax.axis('equal')`
-    and `ax.set_aspect('equal')` don't work on 3D.
-    """
-    limits = np.array([
-        ax.get_xlim3d(),
-        ax.get_ylim3d(),
-        ax.get_zlim3d(),
-    ])
-    x, y, z = np.mean(limits, axis=1)
-    radius = 0.5 * np.max(np.abs(limits[:, 1] - limits[:, 0]))
-    ax.set_xlim3d([x - radius, x + radius])
-    ax.set_ylim3d([y - radius, y + radius])
-    ax.set_zlim3d([z - radius, z + radius])
 
-def plot_triangle_mesh(mesh, show_legend=True, **colors):
-    """Show a 3D mesh (mesh consisting of many triangles).
+def plot_mesh(mesh, *args, **kwargs):
+     
+    if mesh.symmetry == Symmetry.RADIAL:
+        return plot_line_mesh(mesh, *args, **kwargs)
+    elif mesh.symmetry == Symmetry.THREE_D:
+        return plot_triangle_mesh(mesh, *args, **kwargs)
 
-    Parameters
-    ----------
-    mesh: meshio mesh
-        The mesh to show.
+def plot_charge_density(excitation, field, *args, **kwargs):
+    
+    mesh = excitation.mesh 
+    
+    if mesh.symmetry == Symmetry.RADIAL:
+        return _plot_charge_density_2d(excitation, field, *args, **kwargs)
+    elif mesh.symmetry == Symmetry.THREE_D:
+        return _plot_charge_density_3d(excitation, field, *args, **kwargs)
 
-    show_legend: bool
-        Whether to show a legend, the colors will correspond to different physical groups.
+def _plot_charge_density_3d(excitation, field, density=False):
     
-    colors: dict
-        What colors to use for the different physical groups in the geometry. The keys in the dictionary correspond to the
-        physical group names, while the values can be any color understood by matplotlib.
-    """
-    plt.figure(figsize=(10, 13))
-    ax = plt.axes(projection='3d')
-    plt.plot([0, 0], [0, 0], [np.min(mesh.points[:, 2]), np.max(mesh.points[:, 2])], color='black', linestyle='dashed')
-    ax.set_box_aspect([1,1,1])
-    _set_axes_equal(ax)
-     
-    plt.rcParams.update({'font.size': 17})
+    all_vertices, name = excitation.get_active_elements()
+    
+    if density:
+        all_charges = field.charges
+    else:
+        all_charges = np.array([field.charge_on_element(i) for i in range(len(all_vertices))])
+    
+    charge_min, charge_max = np.min(all_charges), np.max(all_charges)
+    
+    plotter = vedo.Plotter()
+
+    for _, indices in name.items():
+        vertices = all_vertices[indices, :3]
+        
+        points = np.reshape(vertices, (3*len(vertices), 3))
+        p_indices = np.arange(3*len(vertices)).reshape( (len(vertices), 3) )
+        vm = vedo.Mesh([points, p_indices])
+        vm.linecolor('black').linewidth(2)
+        
+        vm.cellcolors = 255*vedo.colors.color_map(all_charges[indices], name='jet', vmin=charge_min, vmax=charge_max)
+        plotter.add(vm)
+    
+    plotter.show(viewup='z', axes={'xtitle': 'x (mm)', 'ytitle': 'y (mm)', 'ztitle': 'z (mm)'})
+
+def _plot_charge_density_2d(excitation, field, density=False):
+    all_vertices, name = excitation.get_active_elements()
+    all_charges = np.array([field.charge_on_element(i) for i in range(len(all_vertices))])
+    
+    if density:
+        lengths = np.linalg.norm(all_vertices[:, 1] - all_vertices[:, 0])
+        all_charges /= lengths
+    
+    assert len(all_vertices) == len(all_charges)
+    charge_min, charge_max = np.min(all_charges), np.max(all_charges)
+    
+    plotter = vedo.Plotter()
+    
+    for _, indices in name.items():
+        vertices = all_vertices[indices]
+        start_points = np.reshape(np.array( [(P1, P3, P4) for P1,_,P3,P4 in vertices] ), (len(vertices)*3, 3))
+        end_points = np.reshape(np.array([(P3, P4, P2) for _,P2,P3,P4 in vertices]), (len(vertices)*3, 3))
+        l = vedo.Lines(start_points, end_points, lw=3)
+        colors = np.repeat(all_charges[indices], 6)
+        l.cmap('jet', colors, vmin=charge_min, vmax=charge_max)
+        plotter.add(l)
+    
+    plotter.show(axes={'xtitle': 'x (mm)', 'ytitle': 'y (mm)'})
+    
+    
+
+def plot_triangle_mesh(mesh, show_legend=True, show_normals=False, **colors):
     
     dict_ = _create_point_to_physical_dict(mesh)
-    triangles = mesh.cells_dict['triangle']
+    triangles = mesh.elements
      
     triangles_to_plot = []
     colors_ = []
-    
-    for (A, B, C) in triangles:
-        color = '#CCC'
-        
-        if A in dict_ and B in dict_ and C in dict_:
-            phys1, phys2, phys3 = dict_[A], dict_[B], dict_[C]
-            if phys1 == phys2 and phys2 == phys3 and phys1 in colors:
-                color = colors[phys1]
-         
-        triangles_to_plot.append( [A, B, C] )
-        colors_.append(color)
      
-    colors_, triangles_to_plot = np.array(colors_), np.array(triangles_to_plot)
+    for (v0, v1, v2, v3, v4, v5) in triangles:
+        for A, B, C in [(v0, v3, v5), (v3, v4, v5), (v3, v1, v4), (v5, v4, v2)]:
+            color = '#CCCCC'
+            
+            if A in dict_ and B in dict_ and C in dict_:
+                phys1, phys2, phys3 = dict_[A], dict_[B], dict_[C]
+                if phys1 == phys2 and phys2 == phys3 and phys1 in colors:
+                    color = colors[phys1]
+            
+            triangles_to_plot.append( [A, B, C] )
+            colors_.append(color)
      
+    colors_, triangles_to_plot = np.array(colors_), np.array(triangles_to_plot)
+    plotter = vedo.Plotter()
+    meshes = []
+    
     for c in set(colors_):
         mask = colors_ == c
-        ax.plot_trisurf(mesh.points[:, 0], mesh.points[:, 1], mesh.points[:, 2], triangles=triangles_to_plot[mask], color=c)
-
-    # TODO: reimplement functionality
-    show_normals = False
+        vm = vedo.Mesh([mesh.points, triangles_to_plot[mask]], c)
+        vm.linecolor('black').linewidth(2)
+        
+        key = [k for k, col in colors.items() if c==col]
+        if len(key):
+            vm.legend(key[0])
+        
+        plotter += vm
+        meshes.append(vm)
+    
     if show_normals:
         normals = np.zeros( (len(triangles_to_plot), 6) )
         for i, t in enumerate(triangles_to_plot):
             v1, v2, v3 = mesh.points[t]
             middle = (v1 + v2 + v3)/3
-            normal = 0.1*backend.normal_3d(v1, v2, v3)
-            normals[i] = [*middle, *normal]
-         
-        ax.quiver(*normals.T)
+            area = 1/2*np.linalg.norm(np.cross(v2-v1, v3-v1))
+            side_length = sqrt( (4*area) / sqrt(3) ) # Equilateral triangle, side length with equal area
+            normal = 0.75*side_length*backend.normal_3d(v1, v2, v3)
+            normals[i] = [*middle, *(middle+normal)]
+        
+        arrows = vedo.shapes.Arrows(normals[:, :3], normals[:, 3:], res=20, c='black')
+        plotter.add(arrows)
      
-    if show_legend:
-        for l, c in colors.items():
-            plt.plot([], [], label=l, color=c)
-        plt.legend(loc='upper left')
+    lb = vedo.LegendBox(meshes)
+    plotter.add(lb)
      
-    plt.xlabel('x (mm)')
-    plt.ylabel('y (mm)')
-    ax.set_zlabel('z (mm)')
-    plt.show()
+    plotter.show(viewup='z', axes={'xtitle': 'x (mm)', 'ytitle': 'y (mm)', 'ztitle': 'z (mm)'})
 
 
-def plot_line_mesh(mesh, trajectory=None, show_legend=True, **colors):
+def plot_line_mesh(mesh, show_legend=True, show_normals=False, **colors):
     """Show a 2D mesh (mesh consisting of many line elements).
     
     Parameters
     ---------
     mesh: meshio object
         The mesh to show.
-    trajectory: (N, 2) np.ndarray
-        Optionally also show a trajectory inside the geometry. The trajectory
-        can simply be the position values returned when calling `traceon.tracing.Tracer`.
     show_legend: bool
         Whether to show a legend. The colors in the legend will correspond to the different physical
         groups present in the geometry.
     colors: dict
         The colors to use for the physical groups. The keys in the dictionary correspond to the
-        physical group names, while the values can be any color understood by matplotlib.
+        physical group names, while the values can be any color understood by vedo.
     """
-    plt.figure(figsize=(10, 13))
-    plt.rcParams.update({'font.size': 17})
-    plt.gca().set_aspect('equal')
-     
     dict_ = _create_point_to_physical_dict(mesh)
-    lines = mesh.cells_dict['line4']
-    
-    to_plot_x = []
-    to_plot_y = []
+    lines = mesh.elements
+     
+    start = []
+    end = []
     colors_ = []
+    normals = []
     
     for (P1, P2, P3, P4) in lines:
         for A, B in [(P1, P3), (P3, P4), (P4, P2)]:
-            color = '#CCC'
+            color = '#CCCCC'
 
             if A in dict_ and B in dict_:
                 phys1, phys2 = dict_[A], dict_[B]
                 if phys1 == phys2 and phys1 in colors:
                     color = colors[phys1]
             
             p1, p2 = mesh.points[A], mesh.points[B]
-            to_plot_x.append( [p1[0], p2[0]] )
-            to_plot_y.append( [p1[1], p2[1]] )
+            start.append(p1)
+            end.append(p2)
+            normals.append(backend.higher_order_normal_radial(0.0, mesh.points[np.array([P1, P2, P3, P4])]))
             colors_.append(color)
-     
+    
+    start, end = np.array(start), np.array(end)
     colors_ = np.array(colors_)
+    plotter = vedo.Plotter()
+    lines = []
      
     for c in set(colors_):
         mask = colors_ == c
-        plt.plot(np.array(to_plot_x)[mask].T, np.array(to_plot_y)[mask].T, color=c, linewidth=2)
-        plt.scatter(np.array(to_plot_x)[mask].T, np.array(to_plot_y)[mask].T, color=c, s=15)
-
-    if show_legend:
-        for l, c in colors.items():
-            plt.plot([], [], label=l, color=c)
-        plt.legend(loc='upper left')
-     
-    plt.xlabel('r (mm)')
-    plt.ylabel('z (mm)')
-    plt.axvline(0, color='black', linestyle='dashed')
-    plt.xlim(-0.25, None)
-
-    if trajectory is not None:
-        plt.plot(trajectory[:, 0], trajectory[:, 1])
-    plt.show()
+        l = vedo.Lines(start[mask], end[mask], lw=3, c=c)
+        
+        key = [k for k, col in colors.items() if c==col]
+        if len(key):
+            l.legend(key[0])
+         
+        plotter += l
+        lines.append(l)
+    
+    lb = vedo.LegendBox(lines)
+    plotter += lb
+    
+    if show_normals:
+        arrows_to_plot = np.zeros( (len(normals), 4) )
+        
+        for i, (v1, v2) in enumerate(zip(start, end)):
+            v1, v2 = v1[:2], v2[:2]
+            middle = (v1 + v2)/2
+            length = np.linalg.norm(v2-v1)
+            normal = 3*length*normals[i]
+            arrows_to_plot[i] = [*middle, *(middle+normal)]
+        
+        arrows = vedo.shapes.Arrows(arrows_to_plot[:, :2], arrows_to_plot[:, 2:], c='black')
+        plotter.add(arrows)
+    
+    plotter.show(axes={'xtitle': 'x (mm)', 'ytitle': 'y (mm)'})
 
 '''
 def show_charge_density(lines, charges):
     # See https://matplotlib.org/stable/gallery/lines_bars_and_markers/multicolored_line.html
     assert len(lines) == len(charges)
 
     plt.figure()
```

### Comparing `traceon-0.2.0/traceon/solver.py` & `traceon-0.3.0/traceon/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,98 +68,74 @@
 theta0 = thetas[0]
 dtheta = thetas[1]-thetas[0]
 
 thetas_interpolation_coefficients = np.load(coefficients_file)
 
 assert thetas_interpolation_coefficients.shape == (thetas.size-1, backend.NU_MAX, backend.M_MAX, 4)
 
-def _get_N_quad(exc):
-    if exc.mesh.symmetry == G.Symmetry.RADIAL:
-        return backend.N_QUAD_2D
-    elif exc.mesh.symmetry == G.Symmetry.THREE_D:
-        return 1
-
 def _get_floating_conductor_names(exc):
     return [n for n, (t, v) in exc.excitation_types.items() if t == E.ExcitationType.FLOATING_CONDUCTOR]
 
 def _excitation_to_right_hand_side(excitation, vertices, names):
     floating_names = _get_floating_conductor_names(excitation)
      
     N_floating = len(floating_names)
     N_lines = len(vertices)
-    N_quad = _get_N_quad(excitation)
-    N_matrix = N_quad*N_lines + N_floating # Every floating conductor adds one constraint
+    N_matrix = N_lines + N_floating # Every floating conductor adds one constraint
 
     F = np.zeros( (N_matrix) )
      
     for name, indices in names.items():
         type_, value  = excitation.excitation_types[name]
-
-        all_indices = np.concatenate( [N_quad*indices + i for i in range(N_quad)] )
-         
+        
         if type_ == E.ExcitationType.VOLTAGE_FIXED:
-            F[all_indices] = value
+            F[indices] = value
         elif type_ == E.ExcitationType.VOLTAGE_FUN:
-            for i in indices:
-                points = vertices[i]
-                middle = np.average(points, axis=0)
-                for q in range(N_quad):
-                    # TODO: use higher order BEM?
-                    F[N_quad*i + q] = value(*middle)
+            positions = [backend.position_and_jacobian_radial(0.5, vertices[i, 0], vertices[i, 2], vertices[i, 3], vertices[i, 1])[1] for i in indices]
+            F[indices] = [value(*p) for p in positions]
         elif type_ == E.ExcitationType.DIELECTRIC or \
                 type_ == E.ExcitationType.FLOATING_CONDUCTOR:
-            F[all_indices] = 0
+            F[indices] = 0
     
     # See comments in _add_floating_conductor_constraints_to_matrix
     for i, f in enumerate(floating_names):
         F[-N_floating+i] = excitation.excitation_types[f][1]
      
     assert np.all(np.isfinite(F))
     return F
 
-def _area(symmetry, points):
+def _area(symmetry, jacobian_buffer, pos_buffer, index):
     if symmetry == G.Symmetry.RADIAL:
-        middle = np.average(points, axis=0)
-        length = np.linalg.norm(points[1] - points[0])
-        return length*2*np.pi*middle[0]
+        return 2*np.pi*np.sum(jacobian_buffer[index] * pos_buffer[index, :, 0])
     elif symmetry == G.Symmetry.THREE_D:
-        v1, v2, v3 = points 
-        return 1/2*np.linalg.norm(np.cross(v2-v1, v3-v1))
-
+        return np.sum(jacobian_buffer[index])
 
-def _add_floating_conductor_constraints_to_matrix(matrix, vertices, names, excitation):
+def _add_floating_conductor_constraints_to_matrix(matrix, jac_buffer, pos_buffer, names, excitation):
     floating = _get_floating_conductor_names(excitation)
     N_matrix = matrix.shape[0]
     assert matrix.shape == (N_matrix, N_matrix)
      
     for i, f in enumerate(floating):
-        if excitation.mesh.symmetry == G.Symmetry.THREE_D: 
-            for index in names[f]:
-                # An extra unknown voltage is added to the matrix for every floating conductor.
-                # The column related to this unknown voltage is positioned at the rightmost edge of the matrix.
-                # If multiple floating conductors are present the column lives at -len(floating) + i
-                matrix[ index, -len(floating) + i] = -1
-                # The unknown voltage is determined by the constraint on the total charge of the conductor.
-                # This constraint lives at the bottom edge of the matrix.
-                # The surface area of the respective line element (or triangle) is multiplied by the surface charge (unknown)
-                # to arrive at the total specified charge (right hand side).
-                element = vertices[index]
-                matrix[ -len(floating) + i, index] = _area(excitation.mesh.symmetry, element)
-        elif excitation.mesh.symmetry == G.Symmetry.RADIAL:
-            indices = names[f]
-            backend.add_floating_conductor_constraints_radial(matrix, vertices, indices, i)
-                
+        for index in names[f]:
+            # An extra unknown voltage is added to the matrix for every floating conductor.
+            # The column related to this unknown voltage is positioned at the rightmost edge of the matrix.
+            # If multiple floating conductors are present the column lives at -len(floating) + i
+            matrix[ index, -len(floating) + i] = -1
+            # The unknown voltage is determined by the constraint on the total charge of the conductor.
+            # This constraint lives at the bottom edge of the matrix.
+            # The surface area of the respective line element (or triangle) is multiplied by the surface charge (unknown)
+            # to arrive at the total specified charge (right hand side).
+            matrix[ -len(floating) + i, index] = _area(excitation.mesh.symmetry, jac_buffer, pos_buffer, index)
 
 def _excitation_to_matrix(excitation, vertices, names):
     floating_names = _get_floating_conductor_names(excitation)
     
     N_floating = len(floating_names)
     N_lines = len(vertices)
-    N_quad = _get_N_quad(excitation)
-    N_matrix = N_quad*N_lines + N_floating # Every floating conductor adds one constraint
+    N_matrix = N_lines + N_floating # Every floating conductor adds one constraint
      
     excitation_types = np.zeros(N_lines, dtype=np.uint8)
     excitation_values = np.zeros(N_lines)
     
     for n, indices in names.items():
         excitation_types[indices] = int( excitation.excitation_types[n][0] )
         
@@ -167,52 +143,50 @@
             excitation_values[indices] = excitation.excitation_types[n][1]
      
     assert np.all(excitation_types != 0)
      
     st = time.time()
     matrix = np.zeros( (N_matrix, N_matrix) )
     print(f'Number of elements: {N_lines}, size of matrix: {N_matrix} ({matrix.nbytes/1e6:.0f} MB), symmetry: {excitation.mesh.symmetry}')
+
+    _3d = excitation.mesh.symmetry == G.Symmetry.THREE_D
+
+    jac_buffer, pos_buffer = backend.fill_jacobian_buffer_3d(vertices) if _3d else backend.fill_jacobian_buffer_radial(vertices)
+    fill_fun = backend.fill_matrix_3d if _3d else backend.fill_matrix_radial
      
-    fill_fun = backend.fill_matrix_radial if excitation.mesh.symmetry != G.Symmetry.THREE_D else backend.fill_matrix_3d
-    
     def fill_matrix_rows(rows):
-        fill_fun(matrix, vertices, excitation_types, excitation_values, rows[0], rows[-1])
-    
+        fill_fun(matrix, vertices, excitation_types, excitation_values, jac_buffer, pos_buffer, rows[0], rows[-1])
+     
     util.split_collect(fill_matrix_rows, np.arange(N_lines))    
 
     # Fill the difficult self voltages
     print(f'Time for building matrix: {(time.time()-st)*1000:.0f} ms')
-     
+
     assert np.all(np.isfinite(matrix))
     
-    _add_floating_conductor_constraints_to_matrix(matrix, vertices, names, excitation)
+    _add_floating_conductor_constraints_to_matrix(matrix, jac_buffer, pos_buffer, names, excitation)
         
-    return matrix
+    return matrix, jac_buffer, pos_buffer
 
 
-def _charges_to_field(excitation, charges, vertices, names):
+def _charges_to_field(excitation, charges, vertices, names, jac_buffer, pos_buffer):
     floating_names = _get_floating_conductor_names(excitation)
     N_floating = len(floating_names)
-    N_quad = _get_N_quad(excitation)
      
-    assert len(charges) == N_quad*len(vertices) + N_floating
+    assert len(charges) == len(vertices) + N_floating
     
     floating_voltages = {n:charges[-N_floating+i] for i, n in enumerate(floating_names)}
     if N_floating > 0:
         charges = charges[:-N_floating]
      
-    assert len(charges) == N_quad*len(vertices)
-
-    if N_quad > 1:
-        charges = np.reshape(charges, (len(vertices), N_quad))
-     
+    assert len(charges) == len(vertices)
+    
     field_class = FieldRadialBEM if excitation.mesh.symmetry != G.Symmetry.THREE_D else Field3D_BEM
-    return field_class(vertices, charges, floating_voltages=floating_voltages)
+    return field_class(vertices, charges, jac_buffer, pos_buffer, floating_voltages=floating_voltages)
     
-
 def solve_bem(excitation, superposition=False):
     """
     Solve for the charges on the surface of the geometry by using the Boundary Element Method (BEM) and taking
     into account the specified `excitation`. 
 
     Parameters
     ----------
@@ -234,32 +208,32 @@
     dimensional geometry `Field3D_BEM` is returned. Alternatively, when `superposition=True` a dictionary is returned, where the keys
     are the physical groups with unity excitation, and the values are the resulting fields.
     """
     
     vertices, names = excitation.get_active_elements()
      
     if not superposition:
-        matrix = _excitation_to_matrix(excitation, vertices, names)
+        matrix, jac_buffer, pos_buffer = _excitation_to_matrix(excitation, vertices, names)
         F = _excitation_to_right_hand_side(excitation, vertices, names)
         st = time.time()
         charges = np.linalg.solve(matrix, F)
         assert np.all(np.isfinite(charges))
         print(f'Time for solving matrix: {(time.time()-st)*1000:.0f} ms')
-
-        return _charges_to_field(excitation, charges, vertices, names)
+        
+        return _charges_to_field(excitation, charges, vertices, names, jac_buffer, pos_buffer)
      
     excs = excitation._split_for_superposition()
     superposed_names = excs.keys()
-    matrix = _excitation_to_matrix(excitation, vertices, names)
+    matrix, jac_buffer, pos_buffer = _excitation_to_matrix(excitation, vertices, names)
     F = np.array([_excitation_to_right_hand_side(excs[n], vertices, names) for n in superposed_names]).T
     st = time.time()
     charges = np.linalg.solve(matrix, F)
     print(f'Time for solving matrix: {(time.time()-st)*1000:.0f} ms')
     assert np.all(np.isfinite(charges))
-    return {n:_charges_to_field(excs[n], charges[:, i], vertices, names) for i, n in enumerate(superposed_names)}
+    return {n:_charges_to_field(excs[n], charges[:, i], vertices, names, jac_buffer, pos_buffer) for i, n in enumerate(superposed_names)}
 
 
 def _get_one_dimensional_high_order_ppoly(z, y, dydz, dydz2):
     bpoly = BPoly.from_derivatives(z, np.array([y, dydz, dydz2]).T)
     return PPoly.from_bernstein_basis(bpoly)
 
 def _quintic_spline_coefficients(z, derivs):
@@ -291,61 +265,104 @@
         return self.field_at_point(np.array(args))
 
 class FieldBEM(Field):
     """An electrostatic field (resulting from surface charges) as computed from the Boundary Element Method. You should
     not initialize this class yourself, but it is used as a base class for the fields returned by the `solve_bem` function. 
     This base class overloads the +,*,- operators so it is very easy to take a superposition of different fields."""
     
-    def __init__(self, vertices, charges, floating_voltages={}):
+    def __init__(self, vertices, charges, jac_buffer, pos_buffer, floating_voltages={}):
         assert len(vertices) == len(charges)
         self.vertices = vertices
         self.charges = charges
         self.floating_voltages = floating_voltages
+        self.jac_buffer = jac_buffer
+        self.pos_buffer = pos_buffer
+        self.field_bounds = None
+    
+    def set_bounds(self, bounds):
+        self.field_bounds = np.array(bounds)
 
     def __str__(self):
         name = self.__class__.__name__
         return f'<Traceon {name}, number of elements: {len(self.vertices)}>'
      
     def __add__(self, other):
         if isinstance(other, FieldBEM):
-            assert np.array_equal(self.vertices, other.vertices), "Cannot add Field3D_BEM if geometry is unequal."
-            assert self.charges.shape == other.charges.shape, "Cannot add Field3D_BEM if charges have not equal shape."
+            assert np.array_equal(self.vertices, other.vertices), "Cannot add FieldBEM if geometry is unequal."
+            assert np.array_equal(self.jac_buffer, other.jac_buffer), "Cannot add FieldBEM if geometry is unequal"
+            assert np.array_equal(self.pos_buffer, other.pos_buffer), "Cannot add FieldBEM if geometry is unequal"
+            assert self.charges.shape == other.charges.shape, "Cannot add FieldBEM if charges have not equal shape."
             assert set(self.floating_voltages.keys()) == set(other.floating_voltages.keys())
+            
             floating = {n:self.floating_voltages[n]+other.floating_voltages[n] for n in self.floating_voltages.keys()}
-            return self.__class__(self.vertices, self.charges+other.charges, floating)
+            return self.__class__(self.vertices, self.charges+other.charges, self.jac_buffer, self.pos_buffer, floating)
          
         return NotImpemented
     
     def __sub__(self, other):
         return self.__add__(-other)
      
     def __radd__(self, other):
         return self.__add__(other)
      
     def __mul__(self, other):
         if isinstance(other, int) or isinstance(other, float):
             floating = {n:v*other for n, v in self.floating_voltages.items()}
-            return self.__class__(self.vertices, other*self.charges, floating)
-        
+            return self.__class__(self.vertices, other*self.charges, self.jac_buffer, self.pos_buffer, floating)
+         
         return NotImpemented
 
     def __neg__(self):
         return -1*self
     
     def __rmul__(self, other):
         return self.__mul__(other)
+    
+    def area_of_elements(self, indices):
+        """Compute the total area of the elements at the given indices.
+        
+        Parameters
+        ------------
+        indices: int iterable
+            Indices giving which elements to include in the area calculation.
+
+        Returns
+        ---------------
+        The sum of the area of all elements with the given indices.
+        """
+        return sum(self.area_on_element(i) for i in indices) 
+    
+    def charge_on_element(self, i):
+        return self.area_of_element(i) * self.charges[i]
+    
+    def charge_on_elements(self, indices):
+        """Compute the sum of the charges present on the elements with the given indices. To
+        get the total charge of a physical group use `names['name']` for indices where `names` 
+        is returned by `traceon.excitation.Excitation.get_active_elements()`.
+
+        Parameters
+        ----------
+        indices: (N,) array of int
+            indices of the elements contributing to the charge sum. 
+         
+        Returns
+        -------
+        The sum of the charge. See the note about units on the front page."""
+        return sum(self.charge_on_element(i) for i in indices)
+
 
 
 class FieldRadialBEM(FieldBEM):
     """A radially symmetric electrostatic field. The field is a result of the surface charges as computed by the
     `solve_bem` function. See the comments in `FieldBEM`."""
     
-    def __init__(self, vertices, charges, floating_voltages={}):
-        super().__init__(vertices, charges, floating_voltages)
+    def __init__(self, vertices, charges, jac_buffer, pos_buffer, floating_voltages={}):
+        super().__init__(vertices, charges, jac_buffer, pos_buffer, floating_voltages)
         assert vertices.shape == (len(charges), 4, 3)
+        assert charges.shape == (len(charges),)
         
     def field_at_point(self, point):
         """
         Compute the electric field, \( \\vec{E} = -\\nabla \phi \)
         
         Parameters
         ----------
@@ -353,31 +370,31 @@
             Position at which to compute the field.
         
         Returns
         -------
         Numpy array containing the field strengths (in units of V/mm) in the r and z directions.   
         """
         assert point.shape == (2,) or point.shape == (3,)
-        return backend.field_radial(point, self.vertices, self.charges)
-    
+        return backend.field_radial(point, self.charges, self.jac_buffer, self.pos_buffer)
+     
     def potential_at_point(self, point):
         """
         Compute the potential.
 
         Parameters
         ----------
         point: (2,) array of float64
             Position at which to compute the field.
         
         Returns
         -------
         Potential as a float value (in units of V).
         """
         assert point.shape == (2,) or point.shape == (3,)
-        return backend.potential_radial(point, self.vertices, self.charges)
+        return backend.potential_radial(point, self.charges, self.jac_buffer, self.pos_buffer)
      
     def get_axial_potential_derivatives(self, z):
         """
         Compute the derivatives of the potential at a point on the optical axis (z-axis). 
          
         Parameters
         ----------
@@ -386,15 +403,15 @@
         
 
         Returns
         ------- 
         Numpy array of shape (N, 9) containing the derivatives. At index i one finds the i-th derivative (so
         at position 0 the potential itself is returned). The highest derivative returned is a 
         constant currently set to 9."""
-        return backend.axial_derivatives_radial_ring(z, self.vertices, self.charges)
+        return backend.axial_derivatives_radial_ring(z, self.charges, self.jac_buffer, self.pos_buffer)
      
     def axial_derivative_interpolation(self, zmin, zmax, N=None):
         """
         Use a radial series expansion based on the potential derivatives at the optical axis
         to allow very fast field evaluations.
         
         Parameters
@@ -421,40 +438,26 @@
         
         st = time.time()
         derivs = np.concatenate(util.split_collect(self.get_axial_potential_derivatives, z), axis=0)
         coeffs = _quintic_spline_coefficients(z, derivs.T)
         print(f'Computing derivative interpolation took {(time.time()-st)*1000:.2f} ms ({len(z)} items)')
         
         return FieldRadialAxial(z, coeffs)
-
-    def _charge_on_index(self, i):
-        return backend.charge_radial(self.vertices[i], self.charges[i])
-
-    def charge_on_elements(self, indices):
-        """Compute the sum of the charges present on the elements with the given indices. To
-        get the total charge of a physical group use `names['name']` for indices where `names` 
-        is returned by `traceon.excitation.Excitation.get_active_elements()`.
-
-        Parameters
-        ----------
-        indices: (N,) array of int
-            indices of the elements contributing to the charge sum. 
-         
-        Returns
-        -------
-        The sum of the charge. See the note about units on the front page."""
-        return sum(self._charge_on_index(i) for i in indices)
-
+    
+    def area_of_element(self, i):
+        return _area(G.Symmetry.RADIAL, self.jac_buffer, self.pos_buffer, i)
+    
+    
 class Field3D_BEM(FieldBEM):
     """An electrostatic field resulting from a general 3D geometry. The field is a result of the surface charges as computed by the
     `solve_bem` function. See the comments in `FieldBEM`."""
      
-    def __init__(self, vertices, charges, floating_voltages={}):
-        super().__init__(vertices, charges, floating_voltages)
-        assert vertices.shape == (len(charges), 3, 3)
+    def __init__(self, vertices, charges, jac_buffer, pos_buffer, floating_voltages={}):
+        super().__init__(vertices, charges, jac_buffer, pos_buffer, floating_voltages)
+        assert vertices.shape == (len(charges), 6, 3)
     
     def field_at_point(self, point):
         """
         Compute the electric field, \( \\vec{E} = -\\nabla \phi \)
         
         Parameters
         ----------
@@ -462,15 +465,15 @@
             Position at which to compute the field.
              
         Returns
         -------
         Numpy array containing the field strengths (in units of V/mm) in the x, y and z directions.
         """
         assert point.shape == (3,)
-        return backend.field_3d(point, self.vertices, self.charges)
+        return backend.field_3d(point, self.charges, self.jac_buffer, self.pos_buffer)
      
     def potential_at_point(self, point):
         """
         Compute the potential.
 
         Parameters
         ----------
@@ -478,15 +481,15 @@
             Position at which to compute the field.
         
         Returns
         -------
         Potential as a float value (in units of V).
         """
         assert point.shape == (3,)
-        return backend.potential_3d(point, self.vertices, self.charges)
+        return backend.potential_3d(point, self.charges, self.jac_buffer, self.pos_buffer)
     
     def axial_derivative_interpolation(self, zmin, zmax, N=None):
         """
         Use a radial series expansion around the optical axis to allow for very fast field
         evaluations. Constructing the radial series expansion in 3D is much more complicated
         than the radial symmetric case, but all details have been abstracted away from the user.
         
@@ -510,22 +513,29 @@
         assert zmax > zmin
 
         N = N if N is not None else int(FACTOR_AXIAL_DERIV_SAMPLING_3D*len(self.vertices))
         z = np.linspace(zmin, zmax, N)
         
         print(f'Number of points on z-axis: {len(z)}')
         st = time.time()
-        coeffs = util.split_collect(lambda z: backend.axial_coefficients_3d(self.vertices, self.charges, z, thetas, thetas_interpolation_coefficients), z)
+        jac_buffer, pos_buffer = self.jac_buffer, self.pos_buffer
+        coeffs = util.split_collect(lambda z: backend.axial_coefficients_3d(self.charges, jac_buffer, pos_buffer,  z, thetas, thetas_interpolation_coefficients), z)
         coeffs = np.concatenate(coeffs, axis=0)
         interpolated_coeffs = CubicSpline(z, coeffs).c
         interpolated_coeffs = np.moveaxis(interpolated_coeffs, 0, -1)
         interpolated_coeffs = np.require(interpolated_coeffs, requirements=('C_CONTIGUOUS', 'ALIGNED'))
         print(f'Time for calculating radial series expansion coefficients: {(time.time()-st)*1000:.0f} ms ({len(z)} items)')
 
         return Field3DAxial(z, interpolated_coeffs)
+    
+    def area_of_element(self, i):
+        return _area(G.Symmetry.THREE_D, self.jac_buffer, self.pos_buffer, i)
+    
+
+     
 
 class FieldAxial(Field):
     """An electrostatic field resulting from a radial series expansion around the optical axis. You should
     not initialize this class yourself, but it is used as a base class for the fields returned by the `axial_derivative_interpolation` methods. 
     This base class overloads the +,*,- operators so it is very easy to take a superposition of different fields."""
     
     def __init__(self, z, coeffs):
```

### Comparing `traceon-0.2.0/traceon/util.py` & `traceon-0.3.0/traceon/util.py`

 * *Files identical despite different names*

### Comparing `traceon-0.2.0/traceon.egg-info/PKG-INFO` & `traceon-0.3.0/traceon.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceon
-Version: 0.2.0
+Version: 0.3.0
 Summary: Solver and tracer for electrostatic problems
 Home-page: https://github.com/leon-vv/Traceon
 Author: Léon van Velzen
 Author-email: leonvanvelzen@protonmail.com
 License: AGPLv3
 Project-URL: Documentation, https://leon.science/traceon
 Project-URL: Code, https://github.com/leon-vv/traceon
@@ -22,15 +22,15 @@
         [API documentation](https://leon.science/traceon/index.html)
         
         ## Citation
         
         Please cite the software as follows:
         
         ```
-        L.B. van Velzen. Traceon software (version 0.1.3). 2023. https://doi.org/10.5281/zenodo.7773697
+        L.B. van Velzen. Traceon software (version 0.2.0). 2023. https://doi.org/10.5281/zenodo.7812232
         ```
         
         ## Installation
         
         Install using the Python package manager:
         ```
         pip install traceon
@@ -62,14 +62,20 @@
         
         ## Gallery
         
         ![Image of 3D deflector](https://raw.githubusercontent.com/leon-vv/traceon/main/images/deflector-image.png)
         
         ## Features
         
+        v0.2.0:
+        - Use higher order charge distribution on line elements in radial symmetry
+        - Use higher order line elements (polynomials) in radial symmetry
+        - Better integration techniques, especially with regards to the logarithmic singularities
+        
+        v0.1.0:
         - Uses the powerful [GMSH library](https://gmsh.info/) for meshing
         - Solve for surface charge distribution using BEM
         - General 3D geometries and radially symmetric geometries
         - Dielectrics
         - Floating conductors
         - Accurate electron tracing using adaptive time steps
         - Field/potential calculation by integration over surface charges
```

