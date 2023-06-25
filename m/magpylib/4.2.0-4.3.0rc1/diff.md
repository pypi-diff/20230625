# Comparing `tmp/magpylib-4.2.0.tar.gz` & `tmp/magpylib-4.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib-4.2.0.tar", last modified: Fri Jan 27 12:18:24 2023, max compression
+gzip compressed data, was "magpylib-4.3.0rc1.tar", last modified: Sun Jun 25 09:59:26 2023, max compression
```

## Comparing `magpylib-4.2.0.tar` & `magpylib-4.3.0rc1.tar`

### file list

```diff
@@ -1,126 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.457705 magpylib-4.2.0/
--rw-r--r--   0 root         (0) root         (0)    27499 2023-01-27 12:17:55.000000 magpylib-4.2.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1332 2023-01-27 12:17:55.000000 magpylib-4.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       68 2023-01-27 12:17:55.000000 magpylib-4.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4095 2023-01-27 12:18:24.457705 magpylib-4.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3085 2023-01-27 12:17:55.000000 magpylib-4.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.449705 magpylib-4.2.0/magpylib/
--rw-r--r--   0 root         (0) root         (0)     1582 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.449705 magpylib-4.2.0/magpylib/_src/
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.449705 magpylib-4.2.0/magpylib/_src/defaults/
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/defaults/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8402 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/defaults/defaults_classes.py
--rw-r--r--   0 root         (0) root         (0)    13933 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/defaults/defaults_utility.py
--rw-r--r--   0 root         (0) root         (0)     3134 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/defaults/defaults_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.449705 magpylib-4.2.0/magpylib/_src/display/
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6238 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/backend_matplotlib.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/backend_plotly.py
--rw-r--r--   0 root         (0) root         (0)     5486 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/backend_pyvista.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/display.py
--rw-r--r--   0 root         (0) root         (0)    10671 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/sensor_mesh.py
--rw-r--r--   0 root         (0) root         (0)    21607 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/traces_base.py
--rw-r--r--   0 root         (0) root         (0)    40026 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/traces_generic.py
--rw-r--r--   0 root         (0) root         (0)    15963 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/display/traces_utility.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/_src/fields/
--rw-r--r--   0 root         (0) root         (0)      146 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9322 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_cuboid.py
--rw-r--r--   0 root         (0) root         (0)    15908 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_cylinder.py
--rw-r--r--   0 root         (0) root         (0)    78106 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_cylinder_segment.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_dipole.py
--rw-r--r--   0 root         (0) root         (0)     6896 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_line.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_loop.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_sphere.py
--rw-r--r--   0 root         (0) root         (0)     4524 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_BH_triangle.py
--rw-r--r--   0 root         (0) root         (0)    33024 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/field_wrap_BH.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/special_cel.py
--rw-r--r--   0 root         (0) root         (0)    17660 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/fields/special_el3.py
--rw-r--r--   0 root         (0) root         (0)    21966 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/input_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/_src/obj_classes/
--rw-r--r--   0 root         (0) root         (0)       23 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3525 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseExcitations.py
--rw-r--r--   0 root         (0) root         (0)    12127 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseGeo.py
--rw-r--r--   0 root         (0) root         (0)    34373 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseTransform.py
--rw-r--r--   0 root         (0) root         (0)    26941 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_Collection.py
--rw-r--r--   0 root         (0) root         (0)     9839 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_Sensor.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_current_Line.py
--rw-r--r--   0 root         (0) root         (0)     3974 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_current_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4200 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Cuboid.py
--rw-r--r--   0 root         (0) root         (0)     4302 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Cylinder.py
--rw-r--r--   0 root         (0) root         (0)     6026 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
--rw-r--r--   0 root         (0) root         (0)     4009 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Sphere.py
--rw-r--r--   0 root         (0) root         (0)     5407 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_misc_CustomSource.py
--rw-r--r--   0 root         (0) root         (0)     4022 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_misc_Dipole.py
--rw-r--r--   0 root         (0) root         (0)     5147 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/obj_classes/class_misc_Triangle.py
--rw-r--r--   0 root         (0) root         (0)    60547 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/style.py
--rw-r--r--   0 root         (0) root         (0)    10606 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/_src/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/core/
--rw-r--r--   0 root         (0) root         (0)      980 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/current/
--rw-r--r--   0 root         (0) root         (0)      234 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/current/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/graphics/
--rw-r--r--   0 root         (0) root         (0)      231 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/graphics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/graphics/model3d/
--rw-r--r--   0 root         (0) root         (0)      557 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/graphics/model3d/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/graphics/style/
--rw-r--r--   0 root         (0) root         (0)      280 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/graphics/style/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/magnet/
--rw-r--r--   0 root         (0) root         (0)      529 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/magnet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.453705 magpylib-4.2.0/magpylib/misc/
--rw-r--r--   0 root         (0) root         (0)      335 2023-01-27 12:17:55.000000 magpylib-4.2.0/magpylib/misc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.449705 magpylib-4.2.0/magpylib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4095 2023-01-27 12:18:24.000000 magpylib-4.2.0/magpylib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3604 2023-01-27 12:18:24.000000 magpylib-4.2.0/magpylib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 12:18:24.000000 magpylib-4.2.0/magpylib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 12:18:21.000000 magpylib-4.2.0/magpylib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      142 2023-01-27 12:18:24.000000 magpylib-4.2.0/magpylib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-27 12:18:24.000000 magpylib-4.2.0/magpylib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-27 12:18:24.457705 magpylib-4.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3446 2023-01-27 12:17:55.000000 magpylib-4.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 12:18:24.457705 magpylib-4.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13101 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_BaseTransform.py
--rw-r--r--   0 root         (0) root         (0)     5458 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_Coumpound_setters.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_CustomSource.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test__missing_optional_modules.py
--rw-r--r--   0 root         (0) root         (0)    16990 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_core_field_functions.py
--rw-r--r--   0 root         (0) root         (0)     7074 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_default_utils.py
--rw-r--r--   0 root         (0) root         (0)    10685 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_defaults.py
--rw-r--r--   0 root         (0) root         (0)    11006 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_display_matplotlib.py
--rw-r--r--   0 root         (0) root         (0)    10505 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_display_plotly.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_display_pyvista.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_display_utility.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_elliptics.py
--rw-r--r--   0 root         (0) root         (0)     8671 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14085 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_field_cylinder.py
--rw-r--r--   0 root         (0) root         (0)    12136 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_getBH_dict.py
--rw-r--r--   0 root         (0) root         (0)     7627 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_getBH_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    17330 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_getBH_level2.py
--rw-r--r--   0 root         (0) root         (0)    24748 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_input_checks.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_misc.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_numerical_stability.py
--rw-r--r--   0 root         (0) root         (0)    17713 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_BaseGeo.py
--rw-r--r--   0 root         (0) root         (0)    12060 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_BaseGeo_v4motion.py
--rw-r--r--   0 root         (0) root         (0)    15492 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Collection.py
--rw-r--r--   0 root         (0) root         (0)    10144 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Collection_child_parent.py
--rw-r--r--   0 root         (0) root         (0)    23139 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Collection_v4motion.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Cuboid.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Cylinder.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_CylinderSegment.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Dipole.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Facet.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Line.py
--rw-r--r--   0 root         (0) root         (0)     1726 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Loop.py
--rw-r--r--   0 root         (0) root         (0)     3754 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Sensor.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Sphere.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_obj_Tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_path.py
--rw-r--r--   0 root         (0) root         (0)    10074 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_physics_consistency.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_utility.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-01-27 12:17:55.000000 magpylib-4.2.0/tests/test_vs_mag2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.644673 magpylib-4.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    28515 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-06-25 09:59:26.644673 magpylib-4.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.632673 magpylib-4.3.0rc1/magpylib/
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.632673 magpylib-4.3.0rc1/magpylib/_src/
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.632673 magpylib-4.3.0rc1/magpylib/_src/defaults/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/defaults/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8636 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_classes.py
+-rw-r--r--   0 root         (0) root         (0)    13988 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_utility.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.636673 magpylib-4.3.0rc1/magpylib/_src/display/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/backend_matplotlib.py
+-rw-r--r--   0 root         (0) root         (0)     8415 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/backend_plotly.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/backend_pyvista.py
+-rw-r--r--   0 root         (0) root         (0)     6764 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/display.py
+-rw-r--r--   0 root         (0) root         (0)    10671 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/sensor_mesh.py
+-rw-r--r--   0 root         (0) root         (0)    21826 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/traces_base.py
+-rw-r--r--   0 root         (0) root         (0)    46592 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/traces_generic.py
+-rw-r--r--   0 root         (0) root         (0)    19803 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/display/traces_utility.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.636673 magpylib-4.3.0rc1/magpylib/_src/fields/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9322 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cuboid.py
+-rw-r--r--   0 root         (0) root         (0)    15908 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cylinder.py
+-rw-r--r--   0 root         (0) root         (0)    78106 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cylinder_segment.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_dipole.py
+-rw-r--r--   0 root         (0) root         (0)     6896 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_line.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_loop.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_sphere.py
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_tetrahedron.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_triangle.py
+-rw-r--r--   0 root         (0) root         (0)    16435 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_triangularmesh.py
+-rw-r--r--   0 root         (0) root         (0)    33890 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/field_wrap_BH.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/special_cel.py
+-rw-r--r--   0 root         (0) root         (0)    17660 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/fields/special_el3.py
+-rw-r--r--   0 root         (0) root         (0)    22737 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/input_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.636673 magpylib-4.3.0rc1/magpylib/_src/obj_classes/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3990 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseExcitations.py
+-rw-r--r--   0 root         (0) root         (0)    12264 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseGeo.py
+-rw-r--r--   0 root         (0) root         (0)    34373 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseTransform.py
+-rw-r--r--   0 root         (0) root         (0)    26941 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_Collection.py
+-rw-r--r--   0 root         (0) root         (0)     9838 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_Sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_current_Line.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_current_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Cuboid.py
+-rw-r--r--   0 root         (0) root         (0)     4301 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Cylinder.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
+-rw-r--r--   0 root         (0) root         (0)     4008 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Sphere.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
+-rw-r--r--   0 root         (0) root         (0)    29813 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_CustomSource.py
+-rw-r--r--   0 root         (0) root         (0)     4022 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_Dipole.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_Triangle.py
+-rw-r--r--   0 root         (0) root         (0)    69917 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/style.py
+-rw-r--r--   0 root         (0) root         (0)    11184 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/_src/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.640673 magpylib-4.3.0rc1/magpylib/core/
+-rw-r--r--   0 root         (0) root         (0)      980 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.640673 magpylib-4.3.0rc1/magpylib/current/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/current/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.640673 magpylib-4.3.0rc1/magpylib/graphics/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/graphics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.640673 magpylib-4.3.0rc1/magpylib/graphics/model3d/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/graphics/model3d/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.640673 magpylib-4.3.0rc1/magpylib/graphics/style/
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/graphics/style/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.640673 magpylib-4.3.0rc1/magpylib/magnet/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/magnet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.640673 magpylib-4.3.0rc1/magpylib/misc/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/magpylib/misc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.632673 magpylib-4.3.0rc1/magpylib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-06-25 09:59:26.000000 magpylib-4.3.0rc1/magpylib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3745 2023-06-25 09:59:26.000000 magpylib-4.3.0rc1/magpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 09:59:26.000000 magpylib-4.3.0rc1/magpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 09:59:05.000000 magpylib-4.3.0rc1/magpylib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-25 09:59:26.000000 magpylib-4.3.0rc1/magpylib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-25 09:59:26.000000 magpylib-4.3.0rc1/magpylib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 09:59:26.644673 magpylib-4.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3481 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:59:26.644673 magpylib-4.3.0rc1/tests/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13101 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_BaseTransform.py
+-rw-r--r--   0 root         (0) root         (0)     5458 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_Coumpound_setters.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_CustomSource.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test__missing_optional_modules.py
+-rw-r--r--   0 root         (0) root         (0)    16997 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_core_field_functions.py
+-rw-r--r--   0 root         (0) root         (0)     7074 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_default_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10767 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_defaults.py
+-rw-r--r--   0 root         (0) root         (0)    13681 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_display_matplotlib.py
+-rw-r--r--   0 root         (0) root         (0)    10505 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_display_plotly.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_display_pyvista.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_display_utility.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_elliptics.py
+-rw-r--r--   0 root         (0) root         (0)     8671 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14085 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_field_cylinder.py
+-rw-r--r--   0 root         (0) root         (0)    12137 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_getBH_dict.py
+-rw-r--r--   0 root         (0) root         (0)     7627 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_getBH_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    17329 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_getBH_level2.py
+-rw-r--r--   0 root         (0) root         (0)    25228 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_input_checks.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_misc.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_numerical_stability.py
+-rw-r--r--   0 root         (0) root         (0)    18735 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_BaseGeo.py
+-rw-r--r--   0 root         (0) root         (0)    12060 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_BaseGeo_v4motion.py
+-rw-r--r--   0 root         (0) root         (0)    15492 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Collection.py
+-rw-r--r--   0 root         (0) root         (0)    10144 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Collection_child_parent.py
+-rw-r--r--   0 root         (0) root         (0)    23139 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Collection_v4motion.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Cuboid.py
+-rw-r--r--   0 root         (0) root         (0)     2839 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Cylinder.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_CylinderSegment.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Dipole.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Line.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Sphere.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Tetrahedron.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_Triangle.py
+-rw-r--r--   0 root         (0) root         (0)    14087 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_obj_TriangularMesh.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_path.py
+-rw-r--r--   0 root         (0) root         (0)    10074 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_physics_consistency.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_utility.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-06-25 09:58:55.000000 magpylib-4.3.0rc1/tests/test_vs_mag2.py
```

### Comparing `magpylib-4.2.0/CHANGELOG.md` & `magpylib-4.3.0rc1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 All notable changes to magpylib are documented here.
 
 
 # Releases
 
+## [4.3.0rc1] - 2023-06-25
+- New `TriangularMesh` magnet class added to conveniently work with triangular surface meshes instead of large collections of individual `Triangle` objects. The `TriangularMesh` class performs important checks (closed, connected, oriented) and can directly import pyvista objects and for convex hull bodies. ([#569](https://github.com/magpylib/magpylib/issues/569), [#598](https://github.com/magpylib/magpylib/pull/598)).
+- Added magnetization coloring for `matplotlib` backend ([#597](https://github.com/magpylib/magpylib/pull/597))
+- New automatic backend behavior, set to a dynamic default `auto` depending on the current environment and the given `canvas`, if provided. ([#617](https://github.com/magpylib/magpylib/pull/617))
+- Drop python 3.7 support, following python life cycle. ([#616](https://github.com/magpylib/magpylib/pull/616))
+
 ## [4.2.0] - 2023-01-27
-- (Re)introducing the powerful `misc.Triangle` class that can be used to compute magnetic fields of arbitrarily shaped bodies by approximating their surface with triangular facets. ([#568](https://github.com/magpylib/magpylib/issues/568))
+- (Re)introducing the powerful `misc.Triangle` class that can be used to compute magnetic fields of arbitrarily shaped bodies by approximating their surface with triangular faces. ([#568](https://github.com/magpylib/magpylib/issues/568))
 - Introducing the `magnet.Tetrahedron` class as a derivate of the Triangle class. ([#289](https://github.com/magpylib/magpylib/issues/289))
 - Change pyvista plotting defaults when using `show(backend='pyvista')` to fit better with other libraries. ([#551](https://github.com/magpylib/magpylib/issues/551))
 - Added code of conduct attempting to align with NumFocus standards ([#558](https://github.com/magpylib/magpylib/issues/558))
 - Improved Loop field computation in terms of performance and numerical stability ([#374](https://github.com/magpylib/magpylib/issues/374))
 - Add `magnetization.mode` style to allow showing magnetization direction for any backend [#576](https://github.com/magpylib/magpylib/pull/576))
 - Documentation changes:
     - Correct conda install command
@@ -401,14 +407,16 @@
    - Loop Current
    - Current Line
    - Dipole
 - Collection class
 
 ---
 
+[Unreleased]:https://github.com/magpylib/magpylib/compare/4.3.0rc1...HEAD
+[4.3.0rc1]:https://github.com/magpylib/magpylib/compare/4.2.0...4.3.0rc1
 [4.2.0]:https://github.com/magpylib/magpylib/compare/4.1.2...4.2.0
 [4.1.2]:https://github.com/magpylib/magpylib/compare/4.1.1...4.1.2
 [4.1.1]:https://github.com/magpylib/magpylib/compare/4.1.0...4.1.1
 [4.1.0]:https://github.com/magpylib/magpylib/compare/4.0.4...4.1.0
 [4.0.4]:https://github.com/magpylib/magpylib/compare/4.0.3...4.0.4
 [4.0.3]:https://github.com/magpylib/magpylib/compare/4.0.2...4.0.3
 [4.0.2]:https://github.com/magpylib/magpylib/compare/4.0.1...4.0.2
```

### Comparing `magpylib-4.2.0/LICENSE` & `magpylib-4.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/PKG-INFO` & `magpylib-4.3.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: magpylib
-Version: 4.2.0
+Version: 4.3.0rc1
 Summary: Free Python3 package to compute magnetic fields.
 Home-page: https://github.com/magpylib/magpylib
 Author: Michael Ortner
 Author-email: magpylib@gmail.com
 License: 2-Clause BSD License, Simplified BSD License, FreeBSD License
 Keywords: magnetism physics analytical parallel electromagnetic fields b-field
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 <p align="center"><img align="center" src=docs/_static/images/magpylib_flag.png ><p>
 
@@ -42,28 +42,24 @@
 <a href="https://opensource.org/licenses/BSD-2-Clause"> <img align='center' src="https://img.shields.io/badge/License-BSD_2--Clause-orange.svg"> </a>
 </p>
 
 <p align="center"> Test Coverage:
 <a href="https://codecov.io/gh/magpylib/magpylib">
   <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg" />
 
-</a>
-<a href="https://lgtm.com/projects/g/magpylib/magpylib/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/magpylib/magpylib.svg?logo=lgtm&logoWidth=18"/></a>
-</p>
 
 <p align="center"> Downloads:
 <a href="https://pypi.org/project/magpylib/">
 <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/downloads.svg" alt="Conda Cloud" height="18"></a>
- <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/installer/conda.svg" alt="Conda Cloud" height="18"></a>
-</p>
+
 
 <p align="center"> Try it online:
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.0.0?filepath=docs%2Fexamples">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0rc1?filepath=docs%2Fexamples">
 <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18"></a>
 </p>
 
 </div>
 
 ---
 
@@ -73,15 +69,15 @@
 <p align="center">
     <img align='center' src=docs/_static/images/index/source_fundamentals.png>
 </p>
 
 ---
 
 ### Dependencies:
-_Python3.7+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_
+_Python3.8+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_
 
 ---
 
 ### Documentation & Install:
 
 **Please check out our [documentation](https://magpylib.readthedocs.io/en/latest) for installation, examples and detailed information!**
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: magpylib Version: 4.2.0 Summary: Free Python3
+Metadata-Version: 2.1 Name: magpylib Version: 4.3.0rc1 Summary: Free Python3
 package to compute magnetic fields. Home-page: https://github.com/magpylib/
 magpylib Author: Michael Ortner Author-email: magpylib@gmail.com License: 2-
 Clause BSD License, Simplified BSD License, FreeBSD License Keywords: magnetism
 physics analytical parallel electromagnetic fields b-field Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Intended Audience :: Education Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.7 Description-Content-Type: text/markdown Provides-Extra:
+Requires-Python: ~=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                     [docs/_static/images/magpylib_flag.png]
 ---
    Builds: [https://anaconda.org/conda-forge/magpylib/badges/platforms.svg]
          [https://dev.azure.com/magpylib/magpylib/_apis/build/status/
      magpylib.magpylib?branchName=main] [https://circleci.com/gh/magpylib/
                             magpylib.svg?style=svg]
        Documentation: [https://readthedocs.org/projects/magpylib/badge/
      ?version=latest] [https://img.shields.io/badge/License-BSD_2--Clause-
                                   orange.svg]
-  Test Coverage: [https://codecov.io/gh/magpylib/magpylib/branch/main/graph/
-                      badge.svg] [Language_grade:_Python]
-      Downloads: [PyPI_version] [Conda_Cloud] [Conda_Cloud] [Conda_Cloud]
-                        Try it online: [MyBinder_link]
+                                Test Coverage:
+     [https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg]
+             Downloads:_[PyPI_version]_[Conda_Cloud]_[Conda_Cloud]
+                        Try_it_online:_[MyBinder_link]
 --- ### What is magpylib ? Magpylib is a Python package for calculating **3D
 static magnetic fields** of magnets, line currents and other sources. The
 computation is based on analytical expressions and therefore **extremely
 fast**. A **user friendly geometry interface** enables convenient relative
 positioning between sources and observers.
               [docs/_static/images/index/source_fundamentals.png]
---- ### Dependencies: _Python3.7+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_ --
+--- ### Dependencies: _Python3.8+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_ --
 - ### Documentation & Install: **Please check out our [documentation](https://
 magpylib.readthedocs.io/en/latest) for installation, examples and detailed
 information!** Magpylib is on PyPI and conda-forge. **Install using pip** (`pip
 install magpylib`) or **conda** (`conda install magpylib`) package managers.
```

### Comparing `magpylib-4.2.0/README.md` & `magpylib-4.3.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,24 @@
 <a href="https://opensource.org/licenses/BSD-2-Clause"> <img align='center' src="https://img.shields.io/badge/License-BSD_2--Clause-orange.svg"> </a>
 </p>
 
 <p align="center"> Test Coverage:
 <a href="https://codecov.io/gh/magpylib/magpylib">
   <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg" />
 
-</a>
-<a href="https://lgtm.com/projects/g/magpylib/magpylib/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/magpylib/magpylib.svg?logo=lgtm&logoWidth=18"/></a>
-</p>
 
 <p align="center"> Downloads:
 <a href="https://pypi.org/project/magpylib/">
 <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/downloads.svg" alt="Conda Cloud" height="18"></a>
- <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/installer/conda.svg" alt="Conda Cloud" height="18"></a>
-</p>
+
 
 <p align="center"> Try it online:
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.0.0?filepath=docs%2Fexamples">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0rc1?filepath=docs%2Fexamples">
 <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18"></a>
 </p>
 
 </div>
 
 ---
 
@@ -48,15 +44,15 @@
 <p align="center">
     <img align='center' src=docs/_static/images/index/source_fundamentals.png>
 </p>
 
 ---
 
 ### Dependencies:
-_Python3.7+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_
+_Python3.8+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_
 
 ---
 
 ### Documentation & Install:
 
 **Please check out our [documentation](https://magpylib.readthedocs.io/en/latest) for installation, examples and detailed information!**
```

#### html2text {}

```diff
@@ -3,22 +3,22 @@
    Builds: [https://anaconda.org/conda-forge/magpylib/badges/platforms.svg]
          [https://dev.azure.com/magpylib/magpylib/_apis/build/status/
      magpylib.magpylib?branchName=main] [https://circleci.com/gh/magpylib/
                             magpylib.svg?style=svg]
        Documentation: [https://readthedocs.org/projects/magpylib/badge/
      ?version=latest] [https://img.shields.io/badge/License-BSD_2--Clause-
                                   orange.svg]
-  Test Coverage: [https://codecov.io/gh/magpylib/magpylib/branch/main/graph/
-                      badge.svg] [Language_grade:_Python]
-      Downloads: [PyPI_version] [Conda_Cloud] [Conda_Cloud] [Conda_Cloud]
-                        Try it online: [MyBinder_link]
+                                Test Coverage:
+     [https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg]
+             Downloads:_[PyPI_version]_[Conda_Cloud]_[Conda_Cloud]
+                        Try_it_online:_[MyBinder_link]
 --- ### What is magpylib ? Magpylib is a Python package for calculating **3D
 static magnetic fields** of magnets, line currents and other sources. The
 computation is based on analytical expressions and therefore **extremely
 fast**. A **user friendly geometry interface** enables convenient relative
 positioning between sources and observers.
               [docs/_static/images/index/source_fundamentals.png]
---- ### Dependencies: _Python3.7+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_ --
+--- ### Dependencies: _Python3.8+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_ --
 - ### Documentation & Install: **Please check out our [documentation](https://
 magpylib.readthedocs.io/en/latest) for installation, examples and detailed
 information!** Magpylib is on PyPI and conda-forge. **Install using pip** (`pip
 install magpylib`) or **conda** (`conda install magpylib`) package managers.
```

### Comparing `magpylib-4.2.0/magpylib/__init__.py` & `magpylib-4.3.0rc1/magpylib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 The original software publication (version 2):
 
 https://www.sciencedirect.com/science/article/pii/S2352711020300170
 
 """
 # module level dunders
-__version__ = "4.2.0"
+__version__ = "4.3.0rc1"
 __author__ = "Michael Ortner & Alexandre Boisselet"
 __credits__ = "The Magpylib community"
 __all__ = [
     "magnet",
     "current",
     "misc",
     "getB",
```

### Comparing `magpylib-4.2.0/magpylib/_src/defaults/defaults_classes.py` & `magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,17 +83,18 @@
         """plotting backend to be used by default, if not explicitly set in the `display`
         function (e.g. 'matplotlib', 'plotly').
         Supported backends are defined in magpylib.SUPPORTED_PLOTTING_BACKENDS"""
         return self._backend
 
     @backend.setter
     def backend(self, val):
-        assert val is None or val in SUPPORTED_PLOTTING_BACKENDS, (
+        backends = [*SUPPORTED_PLOTTING_BACKENDS, "auto"]
+        assert val is None or val in backends, (
             f"the `backend` property of {type(self).__name__} must be one of"
-            f"{SUPPORTED_PLOTTING_BACKENDS}"
+            f"{backends}"
             f" but received {repr(val)} instead"
         )
         self._backend = val
 
     @property
     def colorsequence(self):
         """An iterable of color values used to cycle trough for every object displayed.
@@ -103,19 +104,27 @@
         - an hsl/hsla string (e.g. 'hsl(0,100%,50%)')
         - an hsv/hsva string (e.g. 'hsv(0,100%,100%)')
         - a named CSS color"""
         return self._colorsequence
 
     @colorsequence.setter
     def colorsequence(self, val):
-        assert val is None or all(color_validator(c, allow_None=False) for c in val), (
-            f"the `colorsequence` property of {type(self).__name__} must be one an iterable of"
-            f"color sequences"
-            f" but received {repr(val)} instead"
-        )
+        if val is not None:
+            name = type(self).__name__
+            try:
+                val = tuple(
+                    color_validator(c, allow_None=False, parent_name=f"{name}")
+                    for c in val
+                )
+            except TypeError as err:
+                raise ValueError(
+                    f"The `colorsequence` property of {name} must be an "
+                    f"iterable of colors but received {val!r} instead"
+                ) from err
+
         self._colorsequence = val
 
     @property
     def animation(self):
         """Animation properties used by the `plotly` plotting backend when `animation=True`
         in the `show` function."""
         return self._animation
```

### Comparing `magpylib-4.2.0/magpylib/_src/defaults/defaults_utility.py` & `magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """utilities for creating property classes"""
 import collections.abc
 from copy import deepcopy
+from functools import lru_cache
 
 from magpylib._src.defaults.defaults_values import DEFAULTS
 
-
 SUPPORTED_PLOTTING_BACKENDS = ("matplotlib", "plotly", "pyvista")
 
 
 SYMBOLS_MATPLOTLIB_TO_PLOTLY = {
     ".": "circle",
     "o": "circle",
     "+": "cross",
@@ -184,14 +184,15 @@
             for key, val in d.items():
                 dict_[f"{k}{separator}{key}"] = val
         else:
             dict_[k] = v
     return dict_
 
 
+@lru_cache(maxsize=1000)
 def color_validator(color_input, allow_None=True, parent_name=""):
     """validates color inputs based on chosen `backend', allows `None` by default.
 
     Parameters
     ----------
     color_input : str
         color input as string
@@ -228,15 +229,14 @@
                 raise ValueError(msg)
             c = int(c * 255)
             color_input = f"#{c:02x}{c:02x}{c:02x}"
         except:
             pass
 
         if isinstance(color_input, (tuple, list)):
-
             if len(color_input) == 4:  # do not allow opacity values for now
                 color_input = color_input[:-1]
             if len(color_input) != 3:
                 raise ValueError(
                     "Input color must be of shape (3,) or (4,)."
                     f"Instead received {color_input}"
                 )
```

### Comparing `magpylib-4.2.0/magpylib/_src/display/backend_matplotlib.py` & `magpylib-4.3.0rc1/magpylib/_src/display/backend_matplotlib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,56 @@
+import os
+
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.animation import FuncAnimation
 
 from magpylib._src.display.traces_generic import get_frames
 from magpylib._src.display.traces_utility import place_and_orient_model3d
 from magpylib._src.display.traces_utility import subdivide_mesh_by_facecolor
 
-# from magpylib._src.utility import format_obj_input
+# pylint: disable=too-many-branches
+# pylint: disable=import-outside-toplevel
+
+if os.getenv("MAGPYLIB_MPL_SVG") == "true":  # pragma: no cover
+    from matplotlib_inline.backend_inline import set_matplotlib_formats
+
+    set_matplotlib_formats("svg")
 
 SYMBOLS = {"circle": "o", "cross": "+", "diamond": "d", "square": "s", "x": "x"}
 
 LINE_STYLES = {
     "solid": "-",
     "dash": "--",
     "dashdot": "-.",
     "dot": (0, (1, 1)),
     "longdash": "loosely dotted",
     "longdashdot": "loosely dashdotted",
 }
 
 
-def generic_trace_to_matplotlib(trace):
+def generic_trace_to_matplotlib(trace, antialiased=True):
     """Transform a generic trace into a matplotlib trace"""
     traces_mpl = []
     if trace["type"] == "mesh3d":
         subtraces = [trace]
         if trace.get("facecolor", None) is not None:
             subtraces = subdivide_mesh_by_facecolor(trace)
         for subtrace in subtraces:
             x, y, z = np.array([subtrace[k] for k in "xyz"], dtype=float)
             triangles = np.array([subtrace[k] for k in "ijk"]).T
+            kwargs = {
+                "triangles": triangles,
+                "alpha": subtrace.get("opacity", None),
+                "color": subtrace.get("color", None),
+                "linewidth": 0,
+                "antialiased": antialiased,
+            }
             traces_mpl.append(
-                {
-                    "constructor": "plot_trisurf",
-                    "args": (x, y, z),
-                    "kwargs": {
-                        "triangles": triangles,
-                        "alpha": subtrace.get("opacity", None),
-                        "color": subtrace.get("color", None),
-                    },
-                }
+                {"constructor": "plot_trisurf", "args": (x, y, z), "kwargs": kwargs}
             )
     elif trace["type"] == "scatter3d":
         x, y, z = np.array([trace[k] for k in "xyz"], dtype=float)
         mode = trace.get("mode", None)
         props = {
             k: trace.get(v[0], {}).get(v[1], trace.get("_".join(v), None))
             for k, v in {
@@ -97,15 +104,15 @@
     model_kwargs.update(extr.kwargs() if callable(extr.kwargs) else extr.kwargs)
     model_args = extr.args() if callable(extr.args) else extr.args
     trace3d = {
         "constructor": extr.constructor,
         "kwargs": model_kwargs,
         "args": model_args,
     }
-    kwargs, args, = place_and_orient_model3d(
+    kwargs, args = place_and_orient_model3d(
         model_kwargs=model_kwargs,
         model_args=model_args,
         orientation=model["orientation"],
         position=model["position"],
         coordsargs=extr.coordsargs,
         scale=extr.scale,
         return_model_args=True,
@@ -120,17 +127,19 @@
     zoom=1,
     canvas=None,
     animation=False,
     repeat=False,
     colorsequence=None,
     return_fig=False,
     return_animation=False,
+    dpi=80,
+    figsize=(8, 8),
+    antialiased=True,
     **kwargs,
 ):
-
     """Display objects and paths graphically using the matplotlib library."""
     data = get_frames(
         objs=obj_list,
         colorsequence=colorsequence,
         zoom=zoom,
         animation=animation,
         mag_color_grad_apt=False,
@@ -139,23 +148,23 @@
     )
     frames = data["frames"]
     ranges = data["ranges"]
 
     for fr in frames:
         new_data = []
         for tr in fr["data"]:
-            new_data.extend(generic_trace_to_matplotlib(tr))
+            new_data.extend(generic_trace_to_matplotlib(tr, antialiased=antialiased))
         for model in fr["extra_backend_traces"]:
             new_data.append(process_extra_trace(model))
         fr["data"] = new_data
 
     show_canvas = False
     if canvas is None:
         show_canvas = True
-        fig = plt.figure(dpi=80, figsize=(8, 8))
+        fig = plt.figure(dpi=dpi, figsize=figsize)
         ax = fig.add_subplot(111, projection="3d")
         ax.set_box_aspect((1, 1, 1))
     else:
         ax = canvas
         fig = ax.get_figure()
 
     def draw_frame(ind):
@@ -170,14 +179,15 @@
         )
 
     def animate(ind):  # pragma: no cover
         plt.cla()
         draw_frame(ind)
         return [ax]
 
+    anim = None
     if len(frames) == 1:
         draw_frame(0)
     else:
         anim = FuncAnimation(
             fig,
             animate,
             frames=range(len(frames)),
```

### Comparing `magpylib-4.2.0/magpylib/_src/display/backend_plotly.py` & `magpylib-4.3.0rc1/magpylib/_src/display/backend_plotly.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     Returns
     -------
     None: NoneType
     """
     fig.update_scenes(
         **{
-            f"{k}axis": dict(range=ranges[i], autorange=False, title=f"{k} [mm]")
+            f"{k}axis": {"range": ranges[i], "autorange": False, "title": f"{k} [mm]"}
             for i, k in enumerate("xyz")
         },
         aspectratio={k: 1 for k in "xyz"},
         aspectmode="manual",
         camera_eye={"x": 1, "y": -1.5, "z": 1.4},
     )
 
@@ -201,15 +201,14 @@
     renderer=None,
     animation=False,
     colorsequence=None,
     return_fig=False,
     update_layout=True,
     **kwargs,
 ):
-
     """Display objects and paths graphically using the plotly library."""
 
     fig = canvas
     show_fig = False
     extra_data = False
     if fig is None:
         if not return_fig:
```

### Comparing `magpylib-4.2.0/magpylib/_src/display/backend_pyvista.py` & `magpylib-4.3.0rc1/magpylib/_src/display/backend_pyvista.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
     canvas=None,
     animation=False,
     colorsequence=None,
     return_fig=False,
     jupyter_backend=None,
     **kwargs,
 ):
-
     """Display objects and paths graphically using the pyvista library."""
 
     if animation is not False:
         warnings.warn(
             "The pyvista backend does not support animation at the moment.\n"
             "Use `backend=plotly` instead."
         )
```

### Comparing `magpylib-4.2.0/magpylib/_src/display/display.py` & `magpylib-4.3.0rc1/magpylib/_src/display/display.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,56 @@
 """ Display function codes"""
 from importlib import import_module
 
+from matplotlib.axes import Axes as mplAxes
+
 from magpylib._src.display.traces_generic import MagpyMarkers
 from magpylib._src.input_checks import check_dimensions
 from magpylib._src.input_checks import check_excitations
 from magpylib._src.input_checks import check_format_input_backend
 from magpylib._src.input_checks import check_format_input_vector
 from magpylib._src.input_checks import check_input_animation
 from magpylib._src.input_checks import check_input_zoom
 from magpylib._src.utility import format_obj_input
 from magpylib._src.utility import test_path_format
 
 
+def infer_backend(canvas):
+    """Infers the plotting backend from canvas and environment"""
+    # pylint: disable=import-outside-toplevel
+    backend = "matplotlib"
+    in_notebook = False
+    plotly_available = False
+    try:
+        from magpylib._src.utility import is_notebook
+        import plotly  # pylint: disable=unused-import
+
+        plotly_available = True
+        in_notebook = is_notebook()
+        if in_notebook:
+            backend = "plotly"
+    except ImportError:  # pragma: no cover
+        pass
+    if isinstance(canvas, mplAxes):
+        backend = "matplotlib"
+    elif plotly_available and isinstance(
+        canvas, (plotly.graph_objects.Figure, plotly.graph_objects.FigureWidget)
+    ):
+        backend = "plotly"
+    else:
+        try:
+            import pyvista  # pylint: disable=unused-import
+
+            if isinstance(canvas, pyvista.Plotter):
+                backend = "pyvista"
+        except ImportError:  # pragma: no cover
+            pass
+    return backend
+
+
 def show(
     *objects,
     zoom=0,
     animation=False,
     markers=None,
     backend=None,
     canvas=None,
@@ -40,25 +75,29 @@
         If input is a positive float, the animation time is set to the given value.
         This feature is only available for the plotly backend.
 
     markers: array_like, shape (n,3), default=`None`
         Display position markers in the global coordinate system.
 
     backend: string, default=`None`
-        Define plotting backend. Must be one of `'matplotlib'`, `'plotly'`. If not
-        set, parameter will default to `magpylib.defaults.display.backend` which is
-        `'matplotlib'` by installation default.
+        Define plotting backend. Must be one of `['auto', 'matplotlib', 'plotly', 'pyvista']`.
+        If not set, parameter will default to `magpylib.defaults.display.backend` which is
+        `'auto'` by installation default. With `'auto'`, the backend defaults to `'plotly'` if
+        plotly is installed and the function is called in an `IPython` environment, otherwise
+        defaults to `'matplotlib'` which comes installed with magpylib. If the `canvas` is set,
+        the backend defaults to the one corresponding to the canvas object (see canvas parameter).
 
     canvas: matplotlib.pyplot `AxesSubplot` or plotly `Figure` object, default=`None`
         Display graphical output on a given canvas:
-        - with matplotlib: `matplotlib.axes._subplots.AxesSubplot` with `projection=3d.
+        - with matplotlib: `matplotlib.axes.Axes` with `projection=3d.
         - with plotly: `plotly.graph_objects.Figure` or `plotly.graph_objects.FigureWidget`.
+        - with pyvista: `pyvista.Plotter`.
         By default a new canvas is created and immediately displayed.
 
-    canvas: bool, default=False
+    return_fig: bool, default=False
         If True, the function call returns the figure object.
         - with matplotlib: `matplotlib.figure.Figure`.
         - with plotly: `plotly.graph_objects.Figure` or `plotly.graph_objects.FigureWidget`.
         - with pyvista: `pyvista.Plotter`.
 
     Returns
     -------
@@ -123,16 +162,17 @@
         markers,
         dims=(2,),
         shape_m1=3,
         sig_name="markers",
         sig_type="array_like of shape (n,3)",
         allow_None=True,
     )
+    if backend == "auto":
+        backend = infer_backend(canvas)
 
-    # pylint: disable=import-outside-toplevel
     display_func = getattr(
         import_module(f"magpylib._src.display.backend_{backend}"), f"display_{backend}"
     )
 
     if markers is not None and markers:
         obj_list_semi_flat = list(obj_list_semi_flat) + [MagpyMarkers(*markers)]
```

### Comparing `magpylib-4.2.0/magpylib/_src/display/sensor_mesh.py` & `magpylib-4.3.0rc1/magpylib/_src/display/sensor_mesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/display/traces_base.py` & `magpylib-4.3.0rc1/magpylib/_src/display/traces_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from functools import partial
 
 import numpy as np
 from scipy.spatial import ConvexHull  # pylint: disable=no-name-in-module
 
 from magpylib._src.display.traces_utility import merge_mesh3d
 from magpylib._src.display.traces_utility import place_and_orient_model3d
+from magpylib._src.fields.field_BH_tetrahedron import check_chirality
 
 
 def base_validator(name, value, conditions):
     """Validates value based on dictionary of conditions"""
 
     msg = f"""Input {name} must be one of `{tuple(conditions.keys())},`
 received {value!r} instead.
@@ -20,15 +21,21 @@
 
 validate_pivot = partial(base_validator, "pivot")
 
 
 def get_model(trace, *, backend, show, scale, kwargs):
     """Returns model3d dict depending on backend"""
 
-    model = dict(constructor="Mesh3d", kwargs=trace, args=(), show=show, scale=scale)
+    model = {
+        "constructor": "Mesh3d",
+        "kwargs": trace,
+        "args": (),
+        "show": show,
+        "scale": scale,
+    }
     if backend == "matplotlib":
         x, y, z, i, j, k = (trace[k] for k in "xyzijk")
         triangles = np.array([i, j, k]).T
         model.update(
             constructor="plot_trisurf", args=(x, y, z), kwargs={"triangles": triangles}
         )
     model["kwargs"].update(kwargs)
@@ -81,22 +88,22 @@
     Returns
     -------
     3D-model: dict
         A dictionary with necessary key/value pairs with the necessary information to construct
         a 3D-model.
     """
     dimension = np.array(dimension, dtype=float)
-    trace = dict(
-        i=np.array([7, 0, 0, 0, 4, 4, 2, 6, 4, 0, 3, 7]),
-        j=np.array([0, 7, 1, 2, 6, 7, 1, 2, 5, 5, 2, 2]),
-        k=np.array([3, 4, 2, 3, 5, 6, 5, 5, 0, 1, 7, 6]),
-        x=np.array([-1, -1, 1, 1, -1, -1, 1, 1]) * 0.5 * dimension[0],
-        y=np.array([-1, 1, 1, -1, -1, 1, 1, -1]) * 0.5 * dimension[1],
-        z=np.array([-1, -1, -1, -1, 1, 1, 1, 1]) * 0.5 * dimension[2],
-    )
+    trace = {
+        "i": np.array([7, 0, 0, 0, 4, 4, 2, 6, 4, 0, 3, 7]),
+        "j": np.array([0, 7, 1, 2, 6, 7, 1, 2, 5, 5, 2, 2]),
+        "k": np.array([3, 4, 2, 3, 5, 6, 5, 5, 0, 1, 7, 6]),
+        "x": np.array([-1, -1, 1, 1, -1, -1, 1, 1]) * 0.5 * dimension[0],
+        "y": np.array([-1, 1, 1, -1, -1, 1, 1, -1]) * 0.5 * dimension[1],
+        "z": np.array([-1, -1, -1, -1, 1, 1, 1, 1]) * 0.5 * dimension[2],
+    }
 
     trace = place_and_orient_model3d(trace, orientation=orientation, position=position)
     return get_model(trace, backend=backend, show=show, scale=scale, kwargs=kwargs)
 
 
 def make_Prism(
     backend="generic",
@@ -179,15 +186,15 @@
 
     # k2&j2 and k3&j3 inverted because of face orientation
     i = np.concatenate([i1, i2, i3, i4])
     j = np.concatenate([j1, k2, k3, j4])
     k = np.concatenate([k1, j2, j3, k4])
 
     x, y, z = c.T
-    trace = dict(x=x, y=y, z=z, i=i, j=j, k=k)
+    trace = {"x": x, "y": y, "z": z, "i": i, "j": j, "k": k}
     trace = place_and_orient_model3d(trace, orientation=orientation, position=position)
     return get_model(trace, backend=backend, show=show, scale=scale, kwargs=kwargs)
 
 
 def make_Ellipsoid(
     backend="generic",
     dimension=(1.0, 1.0, 1.0),
@@ -242,33 +249,42 @@
     theta = np.linspace(-np.pi / 2, np.pi / 2, vert, endpoint=True)
     phi, theta = np.meshgrid(phi, theta)
 
     x = np.cos(theta) * np.sin(phi) * dimension[0] * 0.5
     y = np.cos(theta) * np.cos(phi) * dimension[1] * 0.5
     z = np.sin(theta) * dimension[2] * 0.5
 
-    x, y, z = x.flatten()[N - 1 :], y.flatten()[N - 1 :], z.flatten()[N - 1 :]
+    x, y, z = (
+        x.flatten()[N - 1 : -N + 1],
+        y.flatten()[N - 1 : -N + 1],
+        z.flatten()[N - 1 : -N + 1],
+    )
+    N2 = len(x) - 1
 
     i1 = [0] * N
-    j1 = np.array([N] + list(range(1, N)), dtype=int)
-    k1 = np.array(list(range(1, N)) + [N], dtype=int)
+    j1 = np.array([N, *range(1, N)], dtype=int)
+    k1 = np.array([*range(1, N), N], dtype=int)
 
-    i2 = np.concatenate([k1 + i * N for i in range(N - 2)])
-    j2 = np.concatenate([j1 + i * N for i in range(N - 2)])
-    k2 = np.concatenate([j1 + (i + 1) * N for i in range(N - 2)])
-
-    i3 = np.concatenate([k1 + i * N for i in range(N - 2)])
-    j3 = np.concatenate([j1 + (i + 1) * N for i in range(N - 2)])
-    k3 = np.concatenate([k1 + (i + 1) * N for i in range(N - 2)])
-
-    i = np.concatenate([i1, i2, i3])
-    j = np.concatenate([j1, j2, j3])
-    k = np.concatenate([k1, k2, k3])
+    i2 = np.concatenate([k1 + i * N for i in range(N - 3)])
+    j2 = np.concatenate([j1 + i * N for i in range(N - 3)])
+    k2 = np.concatenate([j1 + (i + 1) * N for i in range(N - 3)])
+
+    i3 = np.concatenate([k1 + i * N for i in range(N - 3)])
+    j3 = np.concatenate([j1 + (i + 1) * N for i in range(N - 3)])
+    k3 = np.concatenate([k1 + (i + 1) * N for i in range(N - 3)])
+
+    i4 = [N2] * N
+    j4 = k1 + N2 - N - 1
+    k4 = j1 + N2 - N - 1
 
-    trace = dict(x=x, y=y, z=z, i=i, j=j, k=k)
+    i = np.concatenate([i1, i2, i3, i4])
+    j = np.concatenate([j1, j2, j3, j4])
+    k = np.concatenate([k1, k2, k3, k4])
+
+    trace = {"x": x, "y": y, "z": z, "i": i, "j": j, "k": k}
     trace = place_and_orient_model3d(trace, orientation=orientation, position=position)
     return get_model(trace, backend=backend, show=show, scale=scale, kwargs=kwargs)
 
 
 def make_CylinderSegment(
     backend="generic",
     dimension=(1.0, 2.0, 1.0, 0.0, 90.0),
@@ -360,15 +376,15 @@
 
     if phi2 - phi1 != 360:
         i.extend([i5, i5 + N - 1])
         j.extend([k5, k5 + N - 1])
         k.extend([j5, j5 + N - 1])
     i, j, k = (np.hstack(l) for l in (i, j, k))
 
-    trace = dict(x=x, y=y, z=z, i=i, j=j, k=k)
+    trace = {"x": x, "y": y, "z": z, "i": i, "j": j, "k": k}
     trace = place_and_orient_model3d(trace, orientation=orientation, position=position)
     return get_model(trace, backend=backend, show=show, scale=scale, kwargs=kwargs)
 
 
 def make_Pyramid(
     backend="generic",
     base=3,
@@ -441,15 +457,15 @@
     c = c.T * np.array([diameter, diameter, height]) + np.array([0, 0, z_shift])
     x, y, z = c.T
 
     i = np.arange(N, dtype=int)
     j = i + 1
     j[-1] = 0
     k = np.array([N] * N, dtype=int)
-    trace = dict(x=x, y=y, z=z, i=i, j=j, k=k)
+    trace = {"x": x, "y": y, "z": z, "i": i, "j": j, "k": k}
     trace = place_and_orient_model3d(trace, orientation=orientation, position=position)
     return get_model(trace, backend=backend, show=show, scale=scale, kwargs=kwargs)
 
 
 def make_Arrow(
     backend="generic",
     base=3,
@@ -576,39 +592,26 @@
 
     Returns
     -------
     3D-model: dict
         A dictionary with necessary key/value pairs with the necessary information to construct
         a 3D-model.
     """
-    x, y, z = np.array(vertices).T
-    trace = dict(
-        i=np.array(
-            [
-                0,
-                0,
-                1,
-                2,
-            ]
-        ),
-        j=np.array([1, 1, 2, 0]),
-        k=np.array([2, 3, 3, 3]),
-        x=x,
-        y=y,
-        z=z,
-    )
-
+    # create triangles implying right vertices chirality
+    triangles = np.array([[0, 2, 1], [0, 3, 2], [1, 3, 0], [1, 2, 3]])
+    points = check_chirality(np.array([vertices]))[0]
+    trace = dict(zip("xyzijk", [*points.T, *triangles.T]))
     trace = place_and_orient_model3d(trace, orientation=orientation, position=position)
     return get_model(trace, backend=backend, show=show, scale=scale, kwargs=kwargs)
 
 
 def make_TriangularMesh(
     backend="generic",
     vertices=None,
-    triangles=None,
+    faces=None,
     position=None,
     orientation=None,
     show=True,
     scale=1,
     **kwargs,
 ) -> dict:
     """Provides the 3D-model parameters for a custom triangular mesh in dictionary form, based on
@@ -620,15 +623,15 @@
     backend : str
         Plotting backend corresponding to the trace. Can be one of `['matplotlib', 'plotly']`.
 
     vertices: ndarray, shape (4,3)
         Vertices (x1,y1,z1), (x2,y2,z2), (x3,y3,z3), (x4,y4,z4), in the relative
         coordinate system of the triangular mesh.
 
-    triangles: ndarray, shape (4,3)
+    faces: ndarray, shape (4,3)
         For each triangle, the indices of the three points that make up the triangle, ordered in an
         anticlockwise manner. If not specified, a `scipy.spatial.ConvexHull` triangulation is
         calculated.
 
     position : array_like, shape (3,), default=(0,0,0)
         Reference position of the vertices in the global CS. The zero position is
         in the barycenter of the vertices.
@@ -650,21 +653,14 @@
     -------
     3D-model: dict
         A dictionary with necessary key/value pairs with the necessary information to construct
         a 3D-model.
     """
     vertices = np.array(vertices)
     x, y, z = vertices.T
-    if triangles is None:
+    if faces is None:
         hull = ConvexHull(vertices)
-        triangles = hull.simplices
-    i, j, k = np.array(triangles).T
-    trace = dict(
-        i=i,
-        j=j,
-        k=k,
-        x=x,
-        y=y,
-        z=z,
-    )
+        faces = hull.simplices
+    i, j, k = np.array(faces).T
+    trace = {"x": x, "y": y, "z": z, "i": i, "j": j, "k": k}
     trace = place_and_orient_model3d(trace, orientation=orientation, position=position)
     return get_model(trace, backend=backend, show=show, scale=scale, kwargs=kwargs)
```

### Comparing `magpylib-4.2.0/magpylib/_src/display/traces_generic.py` & `magpylib-4.3.0rc1/magpylib/_src/display/traces_generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Generic trace drawing functionalities"""
 # pylint: disable=C0302
 # pylint: disable=too-many-branches
+# pylint: disable=too-many-nested-blocks
 # pylint: disable=cyclic-import
+# pylint: disable=too-many-statements
 import numbers
 import warnings
 from itertools import combinations
+from itertools import cycle
 from typing import Tuple
 
 import numpy as np
+from scipy.spatial import distance
 from scipy.spatial.transform import Rotation as RotScipy
 
 import magpylib as magpy
 from magpylib import _src
 from magpylib._src.defaults.defaults_classes import default_settings as Config
 from magpylib._src.defaults.defaults_utility import linearize_dict
 from magpylib._src.display.sensor_mesh import get_sensor_mesh
@@ -35,91 +39,86 @@
 from magpylib._src.display.traces_utility import get_scene_ranges
 from magpylib._src.display.traces_utility import getColorscale
 from magpylib._src.display.traces_utility import getIntensity
 from magpylib._src.display.traces_utility import group_traces
 from magpylib._src.display.traces_utility import merge_mesh3d
 from magpylib._src.display.traces_utility import merge_traces
 from magpylib._src.display.traces_utility import place_and_orient_model3d
+from magpylib._src.display.traces_utility import slice_mesh_from_colorscale
 from magpylib._src.display.traces_utility import triangles_area
 from magpylib._src.input_checks import check_excitations
+from magpylib._src.style import DefaultMarkers
 from magpylib._src.style import get_style
-from magpylib._src.style import Markers
 from magpylib._src.utility import format_obj_input
 from magpylib._src.utility import unit_prefix
 
 
 class MagpyMarkers:
     """A class that stores markers 3D-coordinates."""
 
     def __init__(self, *markers):
-        self.style = Markers()
+        self.style = DefaultMarkers()
         self.markers = np.array(markers)
 
     def _draw_func(self, color=None, style=None, **kwargs):
         """Create the plotly mesh3d parameters for a Sensor object in a dictionary based on the
         provided arguments."""
         style = self.style if style is None else style
         x, y, z = self.markers.T
         marker_kwargs = {
             f"marker_{k}": v
             for k, v in style.marker.as_dict(flatten=True, separator="_").items()
         }
         marker_kwargs["marker_color"] = (
             style.marker.color if style.marker.color is not None else color
         )
-        trace = dict(
-            type="scatter3d",
-            x=x,
-            y=y,
-            z=z,
-            mode="markers",
+        trace = {
+            "type": "scatter3d",
+            "x": x,
+            "y": y,
+            "z": z,
+            "mode": "markers",
             **marker_kwargs,
             **kwargs,
-        )
+        }
         default_name = "Marker" if len(x) == 1 else "Markers"
         default_suffix = "" if len(x) == 1 else f" ({len(x)} points)"
         update_trace_name(trace, default_name, default_suffix, style)
         return trace
 
 
 def make_DefaultTrace(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     **kwargs,
 ) -> dict:
     """
     Creates the plotly scatter3d parameters for an object with no specifically supported
     representation. The object will be represented by a scatter point and text above with object
     name.
     """
     style = obj.style if style is None else style
-    trace = dict(
-        type="scatter3d",
-        x=[0.0],
-        y=[0.0],
-        z=[0.0],
-        mode="markers+text",
-        marker_size=10,
-        marker_color=color,
-        marker_symbol="diamond",
-    )
+    trace = {
+        "type": "scatter3d",
+        "x": [0.0],
+        "y": [0.0],
+        "z": [0.0],
+        "mode": "markers+text",
+        "marker_size": 10,
+        "marker_color": color,
+        "marker_symbol": "diamond",
+    }
     update_trace_name(trace, f"{type(obj).__name__}", "", style)
     trace["text"] = trace["name"]
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_Line(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     **kwargs,
 ) -> dict:
     """
     Creates the plotly scatter3d parameters for a Line current in a dictionary based on the
     provided arguments.
@@ -130,38 +129,34 @@
     show_arrows = style.arrow.show
     arrow_size = style.arrow.size
     if show_arrows:
         vertices = draw_arrow_from_vertices(vertices, current, arrow_size)
     else:
         vertices = np.array(vertices).T
     x, y, z = vertices
-    trace = dict(
-        type="scatter3d",
-        x=x,
-        y=y,
-        z=z,
-        mode="lines",
-        line_width=style.arrow.width,
-        line_color=color,
-    )
+    trace = {
+        "type": "scatter3d",
+        "x": x,
+        "y": y,
+        "z": z,
+        "mode": "lines",
+        "line_width": style.arrow.width,
+        "line_color": color,
+    }
     default_suffix = (
         f" ({unit_prefix(current)}A)"
         if current is not None
         else " (Current not initialized)"
     )
     update_trace_name(trace, "Line", default_suffix, style)
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_Loop(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     vertices=50,
     **kwargs,
 ):
     """
     Creates the plotly scatter3d parameters for a Loop current in a dictionary based on the
@@ -169,38 +164,34 @@
     """
     style = obj.style if style is None else style
     current = obj.current
     diameter = obj.diameter
     arrow_size = style.arrow.size if style.arrow.show else 0
     vertices = draw_arrowed_circle(current, diameter, arrow_size, vertices)
     x, y, z = vertices
-    trace = dict(
-        type="scatter3d",
-        x=x,
-        y=y,
-        z=z,
-        mode="lines",
-        line_width=style.arrow.width,
-        line_color=color,
-    )
+    trace = {
+        "type": "scatter3d",
+        "x": x,
+        "y": y,
+        "z": z,
+        "mode": "lines",
+        "line_width": style.arrow.width,
+        "line_color": color,
+    }
     default_suffix = (
         f" ({unit_prefix(current)}A)"
         if current is not None
         else " (Current not initialized)"
     )
     update_trace_name(trace, "Loop", default_suffix, style)
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_Dipole(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     autosize=None,
     **kwargs,
 ) -> dict:
     """
     Create the plotly mesh3d parameters for a dipole in a dictionary based on the
@@ -229,18 +220,96 @@
     if n == 0:
         n = 1
         cross = np.array([-np.sign(nvec[-1]), 0, 0])
     dot = np.dot(nvec, zaxis)
     t = np.arccos(dot)
     vec = -t * cross / n
     mag_orient = RotScipy.from_rotvec(vec)
-    orientation = orientation * mag_orient
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    trace = place_and_orient_model3d(trace, orientation=mag_orient, **kwargs)
+    return {**trace, **kwargs}
+
+
+def make_mesh_lines(
+    obj,
+    pos_orient_inds,
+    mode,
+    label=None,
+    style=None,
+    color=None,  # pylint: disable=unused-argument
+    **kwargs,
+):
+    """Draw open or self-intersecting mesh lines and vertices"""
+    # pylint: disable=protected-access
+    style = obj.style if style is None else style
+    mesh = getattr(style.mesh, mode)
+    marker, line = mesh.marker, mesh.line
+    tr, vert = obj.faces, obj.vertices
+    if mode == "disconnected":
+        subsets = obj.get_faces_subsets()
+        lines = get_closest_vertices(subsets, vert)
+    else:
+        edges = np.concatenate([tr[:, 0:2], tr[:, 1:3], tr[:, ::2]], axis=0)
+        # make sure unique pairs are found regardless of order
+        edges = np.sort(edges, axis=1)
+        edges_uniq, edges_counts = np.unique(edges, axis=0, return_counts=True)
+        if mode == "open":
+            lines = vert[edges_uniq[edges_counts != 2]]
+        else:
+            lines = vert[edges_uniq]
+
+    out = {}
+    if lines.size != 0:
+        label = f"{obj}" if label is None else label
+        lines = np.insert(lines, 2, None, axis=1).reshape(-1, 3)
+        traces = []
+        for ind in pos_orient_inds:
+            x, y, z = (obj._orientation[ind].apply(lines) + obj._position[ind]).T
+            trace = {
+                "type": "scatter3d",
+                "x": x,
+                "y": y,
+                "z": z,
+                "marker_color": marker.color,
+                "marker_size": marker.size,
+                "marker_symbol": marker.symbol,
+                "line_color": line.color,
+                "line_width": line.width,
+                "line_dash": line.style,
+                "legendgroup": f"{obj}{mode}edges",
+                "name": f"{label} - {mode}-edges",
+            }
+            traces.append(trace)
+        out = {**merge_traces(*traces), **kwargs}
+    return out
+
+
+def get_closest_vertices(faces_subsets, vertices):
+    """Get closest pairs of points between disconnected subsets of faces indices"""
+    nparts = len(faces_subsets)
+    inds_subsets = [np.unique(v) for v in faces_subsets]
+    closest_verts_list = []
+    if nparts > 1:
+        connected = [np.min(inds_subsets[0])]
+        while len(connected) < nparts:
+            prev_min = float("inf")
+            for i in connected:
+                for j in range(nparts):
+                    if j not in connected:
+                        tr1, tr2 = inds_subsets[i], inds_subsets[j]
+                        c1, c2 = vertices[tr1], vertices[tr2]
+                        dist = distance.cdist(c1, c2)
+                        i1, i2 = divmod(dist.argmin(), dist.shape[1])
+                        min_dist = dist[i1, i2]
+                        if min_dist < prev_min:
+                            prev_min = min_dist
+                            closest_verts = [c1[i1], c2[i2]]
+                            connected_ind = j
+            connected.append(connected_ind)
+            closest_verts_list.append(closest_verts)
+    return np.array(closest_verts_list)
 
 
 def make_triangle_orientations(
     obj,
     pos_orient_inds,
     style=None,
     color=None,
@@ -255,80 +324,72 @@
     """
     # pylint: disable=protected-access
     style = obj.style if style is None else style
     color = color if style.orientation.color is None else style.orientation.color
     size = size if style.orientation.size is None else style.orientation.size
     offset = offset if style.orientation.offset is None else style.orientation.offset
     symbol = symbol if style.orientation.symbol is None else style.orientation.symbol
-    vert = obj.vertices
-    vec = np.cross(vert[1] - vert[0], vert[2] - vert[1])
-    nvec = vec / np.linalg.norm(vec)
-    # arrow length proportional to square root of triangle
-    length = np.sqrt(triangles_area(np.expand_dims(vert, axis=0))[0]) * 0.2
-    zaxis = np.array([0, 0, 1])
-    cross = np.cross(nvec, zaxis)
-    n = np.linalg.norm(cross)
-    if n == 0:
-        n = 1
-        cross = np.array([-np.sign(nvec[-1]), 0, 0])
-    dot = np.dot(nvec, zaxis)
-    t = np.arccos(dot)
-    vec = -t * cross / n
-    orient = RotScipy.from_rotvec(vec)
+    vertices = obj.mesh if hasattr(obj, "mesh") else [obj.vertices]
     traces = []
-    make_fn = make_BasePyramid if symbol == "cone" else make_BaseArrow
-    vmean = np.mean(vert, axis=0)
-    vmean -= (1 - offset) * length * nvec * size
-    for ind in pos_orient_inds:
-        tr = make_fn(
-            "plotly-dict",
-            base=10,
-            diameter=0.5 * size * length,
-            height=size * length,
-            pivot="tail",
-            color=color,
-            position=obj._orientation[ind].apply(vmean) + obj._position[ind],
-            orientation=obj._orientation[ind] * orient,
-            **kwargs,
-        )
-        traces.append(tr)
+    for vert in vertices:
+        vec = np.cross(vert[1] - vert[0], vert[2] - vert[1])
+        nvec = vec / np.linalg.norm(vec)
+        # arrow length proportional to square root of triangle
+        length = np.sqrt(triangles_area(np.expand_dims(vert, axis=0))[0]) * 0.2
+        zaxis = np.array([0, 0, 1])
+        cross = np.cross(nvec, zaxis)
+        n = np.linalg.norm(cross)
+        if n == 0:
+            n = 1
+            cross = np.array([-np.sign(nvec[-1]), 0, 0])
+        dot = np.dot(nvec, zaxis)
+        t = np.arccos(dot)
+        vec = -t * cross / n
+        orient = RotScipy.from_rotvec(vec)
+        make_fn = make_BasePyramid if symbol == "cone" else make_BaseArrow
+        vmean = np.mean(vert, axis=0)
+        vmean -= (1 - offset) * length * nvec * size
+        for ind in pos_orient_inds:
+            tr = make_fn(
+                "plotly-dict",
+                base=10,
+                diameter=0.5 * size * length,
+                height=size * length,
+                pivot="tail",
+                color=color,
+                position=obj._orientation[ind].apply(vmean) + obj._position[ind],
+                orientation=obj._orientation[ind] * orient,
+                **kwargs,
+            )
+            traces.append(tr)
     trace = merge_mesh3d(*traces)
     return trace
 
 
 def make_Cuboid(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     **kwargs,
 ) -> dict:
     """
     Create the plotly mesh3d parameters for a Cuboid Magnet in a dictionary based on the
     provided arguments.
     """
     style = obj.style if style is None else style
     dimension = obj.dimension
     d = [unit_prefix(d / 1000) for d in dimension]
     trace = make_BaseCuboid("plotly-dict", dimension=dimension, color=color)
     default_suffix = f" ({d[0]}m|{d[1]}m|{d[2]}m)"
     update_trace_name(trace, "Cuboid", default_suffix, style)
-    update_magnet_mesh(
-        trace, mag_style=style.magnetization, magnetization=obj.magnetization
-    )
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_Cylinder(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     base=50,
     **kwargs,
 ) -> dict:
     """
     Create the plotly mesh3d parameters for a Cylinder Magnet in a dictionary based on the
@@ -338,26 +399,19 @@
     diameter, height = obj.dimension
     d = [unit_prefix(d / 1000) for d in (diameter, height)]
     trace = make_BasePrism(
         "plotly-dict", base=base, diameter=diameter, height=height, color=color
     )
     default_suffix = f" (D={d[0]}m, H={d[1]}m)"
     update_trace_name(trace, "Cylinder", default_suffix, style)
-    update_magnet_mesh(
-        trace, mag_style=style.magnetization, magnetization=obj.magnetization
-    )
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_CylinderSegment(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     vertices=25,
     **kwargs,
 ):
     """
     Create the plotly mesh3d parameters for a Cylinder Segment Magnet in a dictionary based on the
@@ -367,26 +421,19 @@
     dimension = obj.dimension
     d = [unit_prefix(d / (1000 if i < 3 else 1)) for i, d in enumerate(dimension)]
     trace = make_BaseCylinderSegment(
         "plotly-dict", dimension=dimension, vert=vertices, color=color
     )
     default_suffix = f" (r={d[0]}m|{d[1]}m, h={d[2]}m, φ={d[3]}°|{d[4]}°)"
     update_trace_name(trace, "CylinderSegment", default_suffix, style)
-    update_magnet_mesh(
-        trace, mag_style=style.magnetization, magnetization=obj.magnetization
-    )
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_Sphere(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     vertices=15,
     **kwargs,
 ) -> dict:
     """
     Create the plotly mesh3d parameters for a Sphere Magnet in a dictionary based on the
@@ -396,86 +443,89 @@
     diameter = obj.diameter
     vertices = min(max(vertices, 3), 20)
     trace = make_BaseEllipsoid(
         "plotly-dict", vert=vertices, dimension=[diameter] * 3, color=color
     )
     default_suffix = f" (D={unit_prefix(diameter / 1000)}m)"
     update_trace_name(trace, "Sphere", default_suffix, style)
-    update_magnet_mesh(
-        trace, mag_style=style.magnetization, magnetization=obj.magnetization
-    )
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_Tetrahedron(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     **kwargs,
 ) -> dict:
     """
     Create the plotly mesh3d parameters for a Tetrahedron Magnet in a dictionary based on the
     provided arguments.
     """
     style = obj.style if style is None else style
     trace = make_BaseTetrahedron("plotly-dict", vertices=obj.vertices, color=color)
     update_trace_name(trace, "Tetrahedron", "", style)
-    update_magnet_mesh(
-        trace, mag_style=style.magnetization, magnetization=obj.magnetization
-    )
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
 def make_Triangle(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     **kwargs,
 ) -> dict:
     """
-    Creates the plotly mesh3d parameters for a TriangularMesh Magnet in a dictionary based on the
+    Creates the plotly mesh3d parameters for a Trianglular facet in a dictionary based on the
     provided arguments.
     """
     vert = obj.vertices
     vec = np.cross(vert[1] - vert[0], vert[2] - vert[1])
-    triangles = np.array([[0, 1, 2]])
+    faces = np.array([[0, 1, 2]])
     # if magnetization is normal to the triangle, add a second triangle slightly above to enable
     # proper color gradient visualization. Otherwise only the middle color is shown.
     if np.all(np.cross(obj.magnetization, vec) == 0):
         epsilon = 1e-3 * vec
         vert = np.concatenate([vert - epsilon, vert + epsilon])
-        side_triangles = [
+        side_faces = [
             [0, 1, 3],
             [1, 2, 4],
             [2, 0, 5],
             [1, 4, 3],
             [2, 5, 4],
             [0, 3, 5],
         ]
-        triangles = np.concatenate([triangles, [[3, 4, 5]], side_triangles])
+        faces = np.concatenate([faces, [[3, 4, 5]], side_faces])
 
     style = obj.style if style is None else style
     trace = make_BaseTriangularMesh(
-        "plotly-dict", vertices=vert, triangles=triangles, color=color
-    )
-    update_trace_name(trace, "Triangle", "", style)
-    update_magnet_mesh(
-        trace, mag_style=style.magnetization, magnetization=obj.magnetization
+        "plotly-dict", vertices=vert, faces=faces, color=color
     )
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
+    update_trace_name(trace, obj.__class__.__name__, "", style)
+    return {**trace, **kwargs}
+
+
+def make_TriangularMesh(
+    obj,
+    color=None,
+    style=None,
+    **kwargs,
+) -> dict:
+    """
+    Creates the plotly mesh3d parameters for a Trianglular facet mesh in a dictionary based on the
+    provided arguments.
+    """
+    style = obj.style if style is None else style
+    trace = make_BaseTriangularMesh(
+        "plotly-dict", vertices=obj.vertices, faces=obj.faces, color=color
     )
+    ntri = len(obj.faces)
+    default_suffix = f" ({ntri} face{'s'[:ntri^1]})"
+    update_trace_name(trace, obj.__class__.__name__, default_suffix, style)
+    # make edges sharper in plotly
+    trace.update(flatshading=True, lighting_facenormalsepsilon=0, lighting_ambient=0.7)
+    return {**trace, **kwargs}
 
 
 def make_Pixels(positions, size=1) -> dict:
     """
     Create the plotly mesh3d parameters for Sensor pixels based on pixel positions and chosen size
     For now, only "cube" shape is provided.
     """
@@ -484,16 +534,14 @@
         for p in positions
     ]
     return merge_mesh3d(*pixels)
 
 
 def make_Sensor(
     obj,
-    position=(0.0, 0.0, 0.0),
-    orientation=None,
     color=None,
     style=None,
     autosize=None,
     **kwargs,
 ):
     """
     Create the plotly mesh3d parameters for a Sensor object in a dictionary based on the
@@ -503,93 +551,110 @@
         A positive number. Adjusts automatic display size of sensor pixels. When set to 0,
         pixels will be hidden, when greater than 0, pixels will occupy half the ratio of the minimum
         distance between any pixel of the same sensor, equal to `size_pixel`.
     """
     style = obj.style if style is None else style
     dimension = getattr(obj, "dimension", style.size)
     pixel = obj.pixel
-    pixel = np.array(pixel).reshape((-1, 3))
+    pixel = np.unique(np.array(pixel).reshape((-1, 3)), axis=0)
     style_arrows = style.arrows.as_dict(flatten=True, separator="_")
     sensor = get_sensor_mesh(**style_arrows, center_color=color)
     vertices = np.array([sensor[k] for k in "xyz"]).T
     if color is not None:
         sensor["facecolor"][sensor["facecolor"] == "rgb(238,238,238)"] = color
     dim = np.array(
         [dimension] * 3 if isinstance(dimension, (float, int)) else dimension[:3],
         dtype=float,
     )
+    no_pix = pixel.shape[0] == 1 and (pixel == 0).all()
+    one_pix = pixel.shape[0] == 1 and not (pixel == 0).all()
     if autosize is not None:
         dim *= autosize
-    if pixel.shape[0] == 1:
+    if no_pix:
         dim_ext = dim
     else:
+        if one_pix:
+            pixel = np.concatenate([[[0, 0, 0]], pixel])
         hull_dim = pixel.max(axis=0) - pixel.min(axis=0)
         dim_ext = max(np.mean(dim), np.min(hull_dim))
     cube_mask = (vertices < 1).all(axis=1)
     vertices[cube_mask] = 0 * vertices[cube_mask]
     vertices[~cube_mask] = dim_ext * vertices[~cube_mask]
     vertices /= 2  # sensor_mesh vertices are of length 2
     x, y, z = vertices.T
     sensor.update(x=x, y=y, z=z)
     meshes_to_merge = [sensor]
-    if pixel.shape[0] != 1:
+    if not no_pix:
         pixel_color = style.pixel.color
         pixel_size = style.pixel.size
         combs = np.array(list(combinations(pixel, 2)))
         vecs = np.diff(combs, axis=1)
         dists = np.linalg.norm(vecs, axis=2)
-        pixel_dim = np.min(dists) / 2
+        min_dist = np.min(dists)
+        pixel_dim = dim_ext / 5 if min_dist == 0 else min_dist / 2
         if pixel_size > 0:
             pixel_dim *= pixel_size
-            pixels_mesh = make_Pixels(positions=pixel, size=pixel_dim)
+            poss = pixel[1:] if one_pix else pixel
+            pixels_mesh = make_Pixels(positions=poss, size=pixel_dim)
             pixels_mesh["facecolor"] = np.repeat(pixel_color, len(pixels_mesh["i"]))
             meshes_to_merge.append(pixels_mesh)
         hull_pos = 0.5 * (pixel.max(axis=0) + pixel.min(axis=0))
         hull_dim[hull_dim == 0] = pixel_dim / 2
         hull_mesh = make_BaseCuboid(
             "plotly-dict", position=hull_pos, dimension=hull_dim
         )
         hull_mesh["facecolor"] = np.repeat(color, len(hull_mesh["i"]))
         meshes_to_merge.append(hull_mesh)
     trace = merge_mesh3d(*meshes_to_merge)
     default_suffix = (
-        f""" ({'x'.join(str(p) for p in pixel.shape[:-1])} pixels)"""
-        if pixel.ndim != 1
+        f" ({'x'.join(str(p) for p in obj.pixel.shape[:-1])} pixels)"
+        if obj.pixel.ndim != 1
+        else f" ({pixel[1:].shape[0]} pixel)"
+        if one_pix
         else ""
     )
     update_trace_name(trace, "Sensor", default_suffix, style)
-    return place_and_orient_model3d(
-        trace, orientation=orientation, position=position, **kwargs
-    )
+    return {**trace, **kwargs}
 
 
-def update_magnet_mesh(mesh_dict, mag_style=None, magnetization=None):
+def update_magnet_mesh(
+    mesh_dict, mag_style=None, magnetization=None, color_slicing=False
+):
     """
     Updates an existing plotly mesh3d dictionary of an object which has a magnetic vector. The
     object gets colorized, positioned and oriented based on provided arguments.
+    Slicing allows for matplotlib to show colorgradients approximations by slicing the mesh into
+    the colorscales colors, remesh it and merge with assigning facecolor for each part.
     """
     mag_color = mag_style.color
     if magnetization is not None and mag_style.show:
         vertices = np.array([mesh_dict[k] for k in "xyz"]).T
         color_middle = mag_color.middle
         if mag_color.mode == "tricycle":
             color_middle = mesh_dict["color"]
         elif mag_color.mode == "bicolor":
             color_middle = False
-        mesh_dict["colorscale"] = getColorscale(
-            color_transition=mag_color.transition,
+        ct = mag_color.transition
+        cs = getColorscale(
+            color_transition=0 if color_slicing else ct,
             color_north=mag_color.north,
             color_middle=color_middle,
             color_south=mag_color.south,
         )
-        mesh_dict["intensity"] = getIntensity(
-            vertices=vertices,
-            axis=magnetization,
-        )
+        if color_slicing:
+            tr = slice_mesh_from_colorscale(mesh_dict, magnetization, cs)
+            mesh_dict.update(tr)
+        else:
+            mesh_dict["colorscale"] = cs
+            mesh_dict["intensity"] = getIntensity(
+                vertices=vertices,
+                axis=magnetization,
+            )
         mesh_dict["showscale"] = False
+        mesh_dict.pop("color_slicing", None)
     return mesh_dict
 
 
 def update_trace_name(trace, default_name, default_suffix, style):
     """provides legend entry based on name and suffix"""
     name = default_name if style.label is None else style.label
     if style.description.show and style.description.text is None:
@@ -614,14 +679,16 @@
     # pylint: disable=protected-access
 
     # vector length, color and magnetization
     if hasattr(obj, "diameter"):
         length = obj.diameter  # Sphere
     elif isinstance(obj, magpy.misc.Triangle):
         length = np.amax(obj.vertices) - np.amin(obj.vertices)
+    elif hasattr(obj, "mesh"):
+        length = np.amax(np.ptp(obj.mesh.reshape(-1, 3), axis=0))
     elif hasattr(obj, "vertices"):
         length = np.amax(np.ptp(obj.vertices, axis=0))
     else:  # Cuboid, Cylinder, CylinderSegment
         length = np.amax(obj.dimension[:3])
     length *= 1.8 * style.magnetization.size
     mag = obj.magnetization
     # collect all draw positions and directions
@@ -662,27 +729,27 @@
     marker = style.path.marker.as_dict()
     marker["symbol"] = marker["symbol"]
     marker["color"] = kwargs["color"] if marker["color"] is None else marker["color"]
     line = style.path.line.as_dict()
     line["dash"] = line["style"]
     line["color"] = kwargs["color"] if line["color"] is None else line["color"]
     line = {k: v for k, v in line.items() if k != "style"}
-    scatter_path = dict(
-        type="scatter3d",
-        x=x,
-        y=y,
-        z=z,
-        name=f"Path: {input_obj}",
-        showlegend=False,
-        legendgroup=legendgroup,
+    scatter_path = {
+        "type": "scatter3d",
+        "x": x,
+        "y": y,
+        "z": z,
+        "name": f"Path: {input_obj}",
+        "showlegend": False,
+        "legendgroup": legendgroup,
         **{f"marker_{k}": v for k, v in marker.items()},
         **{f"line_{k}": v for k, v in line.items()},
         **txt_kwargs,
-        opacity=kwargs["opacity"],
-    )
+        "opacity": kwargs["opacity"],
+    }
     return scatter_path
 
 
 def get_generic_traces(
     input_obj,
     color=None,
     autosize=None,
@@ -710,32 +777,33 @@
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     # pylint: disable=too-many-nested-blocks
     # pylint: disable=protected-access
     # pylint: disable=import-outside-toplevel
 
     from magpylib._src.obj_classes.class_misc_Triangle import Triangle
+    from magpylib._src.obj_classes.class_magnet_TriangularMesh import TriangularMesh
 
     # parse kwargs into style and non style args
     style = get_style(input_obj, Config, **kwargs)
     kwargs = {k: v for k, v in kwargs.items() if not k.startswith("style")}
     kwargs["style"] = style
     style_color = getattr(style, "color", None)
     kwargs["color"] = style_color if style_color is not None else color
     kwargs["opacity"] = style.opacity
     legendgroup = f"{input_obj}" if legendgroup is None else legendgroup
 
     is_mag_arrows = False
-    if getattr(input_obj, "magnetization", None) is not None:
-        mode = style.magnetization.mode
-        if style.magnetization.show:
-            if "arrow" in mode or not mag_color_grad_apt:
-                is_mag_arrows = True
-            if mag_color_grad_apt and "color" not in mode and mode != "auto":
-                style.magnetization.show = False  # disables color gradient only
+    is_mag = hasattr(input_obj, "magnetization")
+    if is_mag and style.magnetization.show:
+        mag = style.magnetization
+        if mag.mode == "auto":
+            mag.mode = "color"  # if mag_color_grad_apt else "arrow"
+        is_mag_arrows = "arrow" in mag.mode
+        mag.show = "color" in mag.mode
 
     # check excitations validity
     for param in ("magnetization", "arrow"):
         if getattr(getattr(style, param, None), "show", False):
             check_excitations([input_obj])
 
     label = getattr(getattr(input_obj, "style", None), "label", None)
@@ -758,19 +826,67 @@
             out += (path_traces_extra_specific_backend,)
         return out[0] if len(out) == 1 else out
 
     extra_model3d_traces = style.model3d.data if style.model3d.data is not None else []
     orientations, positions, pos_orient_inds = get_rot_pos_from_path(
         input_obj, style.path.frames
     )
+    obj_is_disconnected = False
+    if isinstance(input_obj, TriangularMesh):
+        for mode in ("open", "disconnected"):
+            show_mesh = getattr(style.mesh, mode).show
+            if mode == "open" and show_mesh:
+                if input_obj.status_open is None:
+                    warnings.warn(
+                        f"Unchecked open mesh status in {input_obj!r} detected, before attempting "
+                        "to show potential open edges, which may take a while to compute "
+                        "when the mesh has many faces, now applying operation..."
+                    )
+                    input_obj.check_open()
+            elif mode == "disconnected" and show_mesh:
+                if input_obj.status_disconnected is None:
+                    warnings.warn(
+                        f"Unchecked disconnected mesh status in {input_obj!r} detected, before "
+                        "attempting to show possible disconnected parts, which may take a while "
+                        "to compute when the mesh has many faces, now applying operation..."
+                    )
+                obj_is_disconnected = input_obj.check_disconnected()
+    disconnected_traces = []
     for pos_orient_enum, (orient, pos) in enumerate(zip(orientations, positions)):
         if style.model3d.showdefault and make_func is not None:
-            path_traces.append(
-                make_func(position=pos, orientation=orient, **make_func_kwargs)
-            )
+            if obj_is_disconnected:
+                tria_orig = input_obj._faces
+                mag_show = style.magnetization.show
+                for tri, dis_color in zip(
+                    input_obj.get_faces_subsets(),
+                    cycle(style.mesh.disconnected.colorsequence),
+                ):
+                    # temporary mutate faces from subset
+                    input_obj._faces = tri
+                    style.magnetization.show = False
+                    dis_tr = make_func(
+                        **{**make_func_kwargs, "color": dis_color},
+                    )
+                    dis_tr = place_and_orient_model3d(
+                        dis_tr, orientation=orient, position=pos
+                    )
+                    disconnected_traces.append(dis_tr)
+                input_obj._faces = tria_orig
+                style.magnetization.show = mag_show
+            else:  # if disconnnected, no mag slicing needed
+                p_tr = make_func(**make_func_kwargs)
+                if is_mag:
+                    p_tr = update_magnet_mesh(
+                        p_tr,
+                        mag_style=style.magnetization,
+                        magnetization=input_obj.magnetization,
+                        color_slicing=not mag_color_grad_apt,
+                    )
+                p_tr = place_and_orient_model3d(p_tr, orientation=orient, position=pos)
+                path_traces.append(p_tr)
         for extr in extra_model3d_traces:
             if extr.show:
                 extr.update(extr.updatefunc())
                 if extr.backend == "generic":
                     trace3d = {"opacity": kwargs["opacity"]}
                     ttype = extr.constructor.lower()
                     obj_extr_trace = (
@@ -844,29 +960,50 @@
                 "showlegend": True if showlegend is None else showlegend,
             }
         )
         if legendtext is not None:
             trace["name"] = legendtext
         traces.append(trace)
 
+    if disconnected_traces:
+        nsubsets = len(input_obj.get_faces_subsets())
+        for ind in range(nsubsets):
+            trace = merge_traces(*disconnected_traces[ind::nsubsets])
+            trace.update(
+                {
+                    "legendgroup": f"{legendgroup} - part_{ind+1:02d}",
+                    "showlegend": True if showlegend is None else showlegend,
+                }
+            )
+            lg = trace.get("name", "") if legendtext is None else legendtext
+            trace["name"] = f"{lg} - part_{ind+1:02d}"
+            traces.append(trace)
+
     if np.array(input_obj.position).ndim > 1 and style.path.show:
         scatter_path = make_path(input_obj, style, legendgroup, kwargs)
         traces.append(scatter_path)
 
     if is_mag_arrows:
         traces.append(
             make_mag_arrows(input_obj, pos_orient_inds, style, legendgroup, kwargs)
         )
-    if isinstance(input_obj, Triangle) and style.orientation.show:
+    if isinstance(input_obj, (Triangle, TriangularMesh)) and style.orientation.show:
         traces.append(
             make_triangle_orientations(
                 input_obj, pos_orient_inds, legendgroup=legendgroup, **kwargs
             )
         )
-
+    if isinstance(input_obj, TriangularMesh):
+        for mode in ("grid", "open", "disconnected"):
+            if getattr(style.mesh, mode).show:
+                trace = make_mesh_lines(
+                    input_obj, pos_orient_inds, mode, label, **kwargs
+                )
+                if trace:
+                    traces.append(trace)
     out = (traces,)
     if extra_backend is not False:
         out += (path_traces_extra_specific_backend,)
     return out[0] if len(out) == 1 else out
 
 
 def clean_legendgroups(frames):
@@ -1009,15 +1146,15 @@
     )
     for obj, params in flat_objs_props.items():
         params.update(kwargs)
         if isinstance(obj, (Dipole, Sensor)):
             traces_to_resize[obj] = {**params}
             # temporary coordinates to be able to calculate ranges
             x, y, z = obj._position.T
-            traces_out[obj] = [dict(x=x, y=y, z=z)]
+            traces_out[obj] = [{"x": x, "y": y, "z": z}]
         else:
             out_traces = get_generic_traces(
                 obj,
                 mag_color_grad_apt=mag_color_grad_apt,
                 extra_backend=extra_backend,
                 **params,
             )
@@ -1099,20 +1236,20 @@
             mag_color_grad_apt=mag_color_grad_apt,
             extra_backend=extra_backend,
             **kwargs,
         )
         if i == 0:  # get the dipoles and sensors autosize from first frame
             autosize = autosize_init
         frames.append(
-            dict(
-                data=traces,
-                name=str(ind + 1),
-                layout=dict(title=title_str),
-                extra_backend_traces=extra_backend_traces,
-            )
+            {
+                "data": traces,
+                "name": str(ind + 1),
+                "layout": {"title": title_str},
+                "extra_backend_traces": extra_backend_traces,
+            }
         )
 
     clean_legendgroups(frames)
     traces = [t for frame in frames for t in frame["data"]]
     ranges = get_scene_ranges(*traces, zoom=zoom)
     out = {
         "frames": frames,
```

### Comparing `magpylib-4.2.0/magpylib/_src/display/traces_utility.py` & `magpylib-4.3.0rc1/magpylib/_src/display/traces_utility.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     position = np.array(position, dtype=float)
     new_model_dict = {}
     if model_args is None:
         model_args = ()
     new_model_args = list(model_args)
     if model_args:
         if coordsargs is None:  # matplotlib default
-            coordsargs = dict(x="args[0]", y="args[1]", z="args[2]")
+            coordsargs = {"x": "args[0]", "y": "args[1]", "z": "args[2]"}
     vertices = []
     if coordsargs is None:
         coordsargs = {"x": "x", "y": "y", "z": "z"}
     useargs = False
     for k in "xyz":
         key = coordsargs[k]
         if key.startswith("args"):
@@ -373,21 +373,23 @@
     """
     Returns 3x2 array of the min and max ranges in x,y,z directions of input traces. Traces can be
     any plotly trace object or a dict, with x,y,z numbered parameters.
     """
     if traces:
         ranges = {k: [] for k in "xyz"}
         for t in traces:
-            for k, v in ranges.items():
-                v.extend(
-                    [
-                        np.nanmin(np.array(t[k], dtype=float)),
-                        np.nanmax(np.array(t[k], dtype=float)),
-                    ]
-                )
+            pts = np.array([t[k] for k in "xyz"], dtype="float64").T
+            try:  # for mesh3, use only vertices part of faces for range calculation
+                inds = np.array([t[k] for k in "ijk"], dtype="int64").T
+                pts = pts[inds].reshape(-1, 3)
+            except KeyError:
+                pass
+            min_max = np.nanmin(pts, axis=0), np.nanmax(pts, axis=0)
+            for v, min_, max_ in zip(ranges.values(), *min_max):
+                v.extend([min_, max_])
         r = np.array([[np.nanmin(v), np.nanmax(v)] for v in ranges.values()])
         size = np.diff(r, axis=1)
         size[size == 0] = 1
         m = size.max() / 2
         center = r.mean(axis=1)
         ranges = np.array([center - m * (1 + zoom), center + m * (1 + zoom)]).T
     else:
@@ -397,15 +399,15 @@
 
 def group_traces(*traces):
     """Group and merge mesh traces with similar properties. This drastically improves
     browser rendering performance when displaying a lot of mesh3d objects."""
     mesh_groups = {}
     common_keys = ["legendgroup", "opacity"]
     spec_keys = {
-        "mesh3d": ["colorscale", "color"],
+        "mesh3d": ["colorscale", "color", "facecolor"],
         "scatter3d": [
             "marker",
             "line_dash",
             "line_color",
             "line_width",
             "marker_color",
             "marker_symbol",
@@ -416,15 +418,18 @@
     for tr in traces:
         tr = linearize_dict(
             tr,
             separator="_",
         )
         gr = [tr["type"]]
         for k in common_keys + spec_keys[tr["type"]]:
-            v = tr.get(k, "")
+            if k == "facecolor":
+                v = tr.get(k, None) is None
+            else:
+                v = tr.get(k, "")
             gr.append(str(v))
         gr = "".join(gr)
         if gr not in mesh_groups:
             mesh_groups[gr] = []
         mesh_groups[gr].append(tr)
 
     traces = []
@@ -458,7 +463,101 @@
 
 def triangles_area(triangles):
     """Return area of triangles of shape (n,3,3) into an array of shape n"""
     norm = np.cross(
         triangles[:, 1] - triangles[:, 0], triangles[:, 2] - triangles[:, 0], axis=1
     )
     return np.linalg.norm(norm, axis=1) / 2
+
+
+def slice_mesh_with_plane(
+    verts, tris, plane_orig=(0.0, 0.0, 0.0), plane_axis=(1.0, 0.0, 0.0)
+):
+    """Slice a mesh obj defined by vertices an triangles by a plane defined by its
+    origin and axis. Returns two (verts, tris) tuples for left and right side."""
+    dists = np.dot(verts - plane_orig, plane_axis)
+
+    if np.any(dists == 0):
+        # if planes passes some vertices shift vertices slightly
+        # IMPROVE-> make special case without a hack like this
+        verts += np.array([129682, -986394, 123495]) * 1e-16
+        dists = np.dot(verts - plane_orig, plane_axis)
+    all_dists = dists[tris]
+
+    mask_left = np.all(all_dists < 0, axis=1)
+    mask_right = np.all(all_dists > 0, axis=1)
+    mask_cut = np.any(all_dists < 0, axis=1) & np.any(all_dists > 0, axis=1)
+    tri_cut = mask_cut.nonzero()[0]
+
+    d = all_dists.copy()[mask_cut]
+    t = tris.copy()[tri_cut]
+
+    s = d[:, [0, 1, 1, 2, 2, 0]].reshape(-1, 3, 2)  # pairs of distances
+
+    # make sure the first two edges are the one intersected, if not cycle it
+    im = np.prod(s, axis=2) < 0  # edge intersects if product of dist<0
+    m1 = im[:, [0, 2]].sum(axis=1) == 2
+    m2 = im[:, [1, 2]].sum(axis=1) == 2
+    if np.any(m1):
+        t[m1] = t[m1][:, [2, 0, 1]]
+        s[m1] = s[m1][:, [2, 0, 1]]
+        d[m1] = d[m1][:, [2, 0, 1]]
+    if np.any(m2):
+        t[m2] = t[m2][:, [1, 2, 0]]
+        s[m2] = s[m2][:, [1, 2, 0]]
+        d[m2] = d[m2][:, [1, 2, 0]]
+    f = verts[t]
+
+    p = np.abs(s).sum(axis=2)  # projected dists to plane
+
+    e = f[:, [0, 1, 1, 2, 2, 0]].reshape(-1, 3, 2, 3)  # edges
+    v = np.squeeze(np.diff(e, axis=2))  # edges vectors
+
+    pts = (f + v * (np.abs(d) / p).reshape(-1, 3, 1))[:, :2]
+
+    f5 = np.concatenate([f, pts], axis=1)
+    f1 = f5[:, [[3, 1, 4]]]
+    f2 = f5[:, [[0, 3, 2], [3, 4, 2]]]
+
+    fl1 = f1[d[:, 0] > 0].reshape(-1, 3, 3)
+    fr1 = f1[d[:, 0] < 0].reshape(-1, 3, 3)
+    fl2 = f2[d[:, 0] < 0].reshape(-1, 3, 3)
+    fr2 = f2[d[:, 0] > 0].reshape(-1, 3, 3)
+
+    fl0 = verts[tris[mask_left]]
+    fr0 = verts[tris[mask_right]]
+
+    fl = np.concatenate([fl0, fl1, fl2]).reshape((-1, 3))
+    fr = np.concatenate([fr0, fr1, fr2]).reshape((-1, 3))
+
+    vr, tr = np.unique(fr, axis=0, return_inverse=True)
+    tr = tr.reshape((-1, 3))
+
+    vl, tl = np.unique(fl, axis=0, return_inverse=True)
+    tl = tl.reshape((-1, 3))
+    return (vl, tl), (vr, tr)
+
+
+def slice_mesh_from_colorscale(trace, axis, colorscale):
+    """Slice mesh3d obj by axis and colorsale. Return single mesh dict with according
+    facecolor argument."""
+    cs = colorscale
+    origs = np.array(list(dict.fromkeys([v[0] for v in cs])))[1:-1]
+    colors = list(dict.fromkeys([v[1] for v in cs]))
+    vr = np.array([v for k, v in trace.items() if k in "xyz"]).T
+    tr = np.array([v for k, v in trace.items() if k in "ijk"]).T
+    axis = axis / np.linalg.norm(axis)
+    dists = np.dot(vr + np.mean(vr, axis=0), axis)
+    ptp = np.ptp(dists)
+    shift = np.mean([vr[np.argmin(dists)], vr[np.argmax(dists)]], axis=0)
+    origs = np.vstack((origs - 0.5) * ptp) * axis + shift
+
+    traces = []
+    for ind, color in enumerate(colors):
+        if ind < len(origs):
+            (vl, tl), (vr, tr) = slice_mesh_with_plane(vr, tr, origs[ind], axis)
+        else:
+            vl, tl = vr, tr
+        trace_temp = dict(zip("xyzijk", [*vl.T, *tl.T]))
+        trace_temp.update(facecolor=np.array([color] * len(tl)))
+        traces.append(trace_temp)
+    return {**trace, **merge_mesh3d(*traces)}
```

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_cuboid.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_cylinder.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_cylinder_segment.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cylinder_segment.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_dipole.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_line.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_line.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_loop.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_loop.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_sphere.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_tetrahedron.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_BH_triangle.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/field_wrap_BH.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_wrap_BH.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 level4(getB_from_sensor, getH_from_sensor): <--- USER INTERFACE
 
 level5(sens.getB, sens.getH): <--- USER INTERFACE
 """
 # pylint: disable=cyclic-import
 import numbers
+import warnings
 from itertools import product
 from typing import Callable
 
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 
 from magpylib._src.exceptions import MagpylibBadUserInput
@@ -189,14 +190,15 @@
     """
     # pylint: disable=protected-access
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     # pylint: disable=import-outside-toplevel
 
     from magpylib._src.obj_classes.class_Collection import Collection
+    from magpylib._src.obj_classes.class_magnet_TriangularMesh import TriangularMesh
 
     # CHECK AND FORMAT INPUT ---------------------------------------------------
     if isinstance(sources, str):
         return getBH_dict_level2(
             source_type=sources,
             observers=observers,
             field=field,
@@ -217,22 +219,38 @@
     #   out: src_list = ordered list of sources with flattened collections
     sources, src_list = format_src_inputs(sources)
 
     # test if all source dimensions and excitations are initialized
     check_dimensions(src_list)
     check_excitations(src_list, field)
 
+    # make sure that TriangularMesh sources have a closed mesh when getB is called - warn if not
+    if field == "B":
+        for src in src_list:
+            if isinstance(src, TriangularMesh):
+                # unchecked mesh status - may be open
+                if src.status_open is None:
+                    warnings.warn(
+                        f"Unchecked mesh status of {src} detected before B-field computation. "
+                        "An open mesh may return bad results."
+                    )
+                elif src.status_open:  # mesh is open
+                    warnings.warn(
+                        f"Open mesh of {src} detected before B-field computation. "
+                        "An open mesh may return bad results."
+                    )
+
     # format observers input:
     #   allow only bare sensor, collection, pos_vec or list thereof
     #   transform input into an ordered list of sensors (pos_vec->pixel)
     #   check if all pixel shapes are similar - or else if pixel_agg is given
     pixel_agg_func = check_format_pixel_agg(pixel_agg)
     sensors, pix_shapes = check_format_input_observers(observers, pixel_agg)
     pix_nums = [
-        int(np.product(ps[:-1])) for ps in pix_shapes
+        int(np.prod(ps[:-1])) for ps in pix_shapes
     ]  # number of pixel for each sensor
     pix_inds = np.cumsum([0] + pix_nums)  # cummulative indices of pixel for each sensor
     pix_all_same = len(set(pix_shapes)) == 1
 
     # check which sensors have unit roation
     #   so that they dont have to be rotated back later (performance issue)
     #   this check is made now when sensor paths are not yet tiled.
```

### Comparing `magpylib-4.2.0/magpylib/_src/fields/special_cel.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/special_cel.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/fields/special_el3.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/special_el3.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/input_checks.py` & `magpylib-4.3.0rc1/magpylib/_src/input_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,14 +356,40 @@
         if np.any(inp <= 0):
             raise MagpylibBadUserInput(
                 f"Input parameter `{sig_name}` cannot have values <= 0."
             )
     return inp
 
 
+def check_format_input_vector2(
+    inp,
+    shape,
+    param_name,
+):
+    """checks vector input and returns in formatted form
+    - inp must be array_like
+    - convert inp to ndarray with dtype float
+    - make sure that inp.ndim = target_ndim, None dimensions are ignored
+    """
+    is_array_like(
+        inp,
+        f"Input parameter `{param_name}` must be array_like.\n"
+        f"Instead received type {type(inp)}.",
+    )
+    inp = make_float_array(
+        inp,
+        f"Input parameter `{param_name}` must contain only float compatible entries.\n",
+    )
+    for d1, d2 in zip(inp.shape, shape):
+        if d2 is not None:
+            if d1 != d2:
+                raise ValueError(f"Input parameter `{param_name}` has bad shape.")
+    return inp
+
+
 def check_format_input_vertices(inp):
     """checks vertices input and returns in formatted form
     - vector check with dim = (n,3) but n must be >=2
     """
     inp = check_format_input_vector(
         inp,
         dims=(2,),
@@ -415,21 +441,21 @@
             f"but received {inp} instead."
         )
     return inp
 
 
 def check_format_input_backend(inp):
     """checks show-backend input and returns Non if bad input value"""
-    backends = SUPPORTED_PLOTTING_BACKENDS
+    backends = [*SUPPORTED_PLOTTING_BACKENDS, "auto"]
     if inp is None:
         inp = default_settings.display.backend
     if inp in backends:
         return inp
     raise MagpylibBadUserInput(
-        f"Input parameter `backend` must be one of `{backends+(None,)}`.\n"
+        f"Input parameter `backend` must be one of `{backends+[None]}`.\n"
         f"Instead received {inp}."
     )
 
 
 def check_format_input_observers(inp, pixel_agg=None):
     """
     checks observers input and returns a list of sensor objects
@@ -520,15 +546,14 @@
         wanted_types += (Collection,)
 
     if typechecks:
         all_types = (BaseSource, Sensor, Collection)
 
     obj_list = []
     for obj in inp:
-
         # add to list if wanted type
         if isinstance(obj, wanted_types):
             obj_list.append(obj)
 
         # recursion
         if isinstance(obj, Collection) and recursive:
             obj_list += check_format_input_obj(
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseDisplayRepr.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseDisplayRepr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """BaseGeo class code"""
 # pylint: disable=cyclic-import
+# pylint: disable=too-many-branches
 import numpy as np
 
 from magpylib._src.display.display import show
 from magpylib._src.display.traces_generic import make_DefaultTrace
 
 UNITS = {
     "parent": None,
@@ -57,18 +58,26 @@
                     val = val.as_rotvec(degrees=True)
                     if len(val) != 1:
                         k = f"{k} (last)"
                     val = f"{val[-1]}"
                 elif k == "pixel":
                     val = getattr(self, "pixel")
                     px_shape = val.shape[:-1]
-                    val_str = f"{int(np.product(px_shape))}"
+                    val_str = f"{int(np.prod(px_shape))}"
                     if val.ndim > 2:
                         val_str += f" ({'x'.join(str(p) for p in px_shape)})"
                     val = val_str
+                elif k == "status_disconnected_data":
+                    val = getattr(self, k)
+                    if val is not None:
+                        val = f"{len(val)} part{'s'[:len(val)^1]}"
+                elif isinstance(getattr(self, k), (list, tuple, np.ndarray)):
+                    val = np.array(getattr(self, k))
+                    if np.prod(val.shape) > 4:
+                        val = f"shape{val.shape}"
                 else:
                     val = getattr(self, k)
                 lines.append(f"  • {k}: {val} {unit_str}")
         return lines
 
     def describe(self, *, exclude=("style", "field_func"), return_string=False):
         """Returns a view of the object properties.
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseExcitations.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseExcitations.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseGeo.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseGeo.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,21 @@
             0.0,
             0.0,
         ),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
+        self._style_kwargs = {}
         self._parent = None
         # set _position and _orientation attributes
         self._init_position_orientation(position, orientation)
 
         if style is not None or kwargs:  # avoid style creation cost if not needed
-            self.style = self._process_style_kwargs(style=style, **kwargs)
+            self._style_kwargs = self._process_style_kwargs(style=style, **kwargs)
 
     @staticmethod
     def _process_style_kwargs(style=None, **kwargs):
         if kwargs:
             if style is None:
                 style = {}
             style_kwargs = {}
@@ -238,25 +238,25 @@
 
     @property
     def style(self):
         """
         Object style in the form of a BaseStyle object. Input must be
         in the form of a style dictionary.
         """
-        if not hasattr(self, "_style") or self._style is None:
-            self._style = self._validate_style(val=None)
+        if getattr(self, "_style", None) is None:
+            self._style = self._validate_style(self._style_kwargs)
+            self._style_kwargs = {}
         return self._style
 
     @style.setter
     def style(self, val):
         self._style = self._validate_style(val)
 
     def _validate_style(self, val=None):
-        if val is None:
-            val = {}
+        val = {} if val is None else val
         if isinstance(val, dict):
             val = self._style_class(**val)
         if not isinstance(val, self._style_class):
             raise ValueError(
                 f"Input parameter `style` must be of type {self._style_class}.\n"
                 f"Instead received type {type(val)}"
             )
@@ -337,15 +337,17 @@
             parent = self._parent
             self._parent = None
             obj_copy = deepcopy(self)
             self._parent = parent
         else:
             obj_copy = deepcopy(self)
 
-        if getattr(self, "_style", None) is not None:
+        if getattr(self, "_style", None) is not None or bool(
+            getattr(self, "_style_kwargs", False)
+        ):
             label = self.style.label
             if label is None:
                 label = f"{type(self).__name__}_01"
             else:
                 label = add_iteration_suffix(label)
             obj_copy.style.label = label
         style_kwargs = {}
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_BaseTransform.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_Collection.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_Collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
 
 class BaseCollection(BaseDisplayRepr):
     """Collection base class without BaseGeo properties"""
 
     _draw_func = None
 
     def __init__(self, *children, override_parent=False):
-
         BaseDisplayRepr.__init__(self)
 
         self._children = []
         self._sources = []
         self._sensors = []
         self._collections = []
         self.add(*children, override_parent=override_parent)
@@ -670,15 +669,15 @@
     Collections can be used as `sources` and `observers` input for magnetic field
     computation. For magnetic field computation a collection that contains sources
     functions like a single source. When the collection contains sensors
     it functions like a list of all its sensors.
 
     Parameters
     ----------
-    children: sources, `Sensor` or `Collection objects
+    children: sources, `Sensor` or `Collection` objects
         An ordered list of all children in the collection.
 
     sensors: `Sensor` objects
         An ordered list of all sensor objects in the collection.
 
     sources: source objects
         An ordered list of all source objects`(magnets, currents, misc) in the collection.
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_Sensor.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_Sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         self,
         position=(0, 0, 0),
         pixel=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.pixel = pixel
 
         # init inheritance
         BaseGeo.__init__(self, position, orientation, style=style, **kwargs)
         BaseDisplayRepr.__init__(self)
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_current_Line.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_current_Line.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
         current=None,
         vertices=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.vertices = vertices
 
         # init inheritance
         super().__init__(position, orientation, current, style, **kwargs)
 
     # property getters and setters
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_current_Loop.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_current_Loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         current=None,
         diameter=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.diameter = diameter
 
         # init inheritance
         super().__init__(position, orientation, current, style, **kwargs)
 
     # property getters and setters
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Cuboid.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Cuboid.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         magnetization=None,
         dimension=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.dimension = dimension
 
         # init inheritance
         super().__init__(position, orientation, magnetization, style, **kwargs)
 
     # property getters and setters
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Cylinder.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Cylinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         magnetization=None,
         dimension=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.dimension = dimension
 
         # init inheritance
         super().__init__(position, orientation, magnetization, style, **kwargs)
 
     # property getters and setters
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         magnetization=None,
         dimension=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.dimension = dimension
 
         # init inheritance
         super().__init__(position, orientation, magnetization, style, **kwargs)
 
     # property getters and setters
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Sphere.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Sphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         magnetization=None,
         diameter=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.diameter = diameter
 
         # init inheritance
         super().__init__(position, orientation, magnetization, style, **kwargs)
 
     # property getters and setters
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         magnetization=None,
         vertices=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         # instance attributes
         self.vertices = vertices
         self._object_type = "Tetrahedron"
 
         # init inheritance
         super().__init__(position, orientation, magnetization, style, **kwargs)
```

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_misc_CustomSource.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_misc_Dipole.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/_src/obj_classes/class_misc_Triangle.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_Triangle.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         magnetization=None,
         vertices=None,
         position=(0, 0, 0),
         orientation=None,
         style=None,
         **kwargs,
     ):
-
         self.vertices = vertices
 
         # init inheritance
         super().__init__(position, orientation, magnetization, style, **kwargs)
 
     # property getters and setters
     @property
```

### Comparing `magpylib-4.2.0/magpylib/_src/style.py` & `magpylib-4.3.0rc1/magpylib/_src/style.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,73 +10,84 @@
 from magpylib._src.defaults.defaults_utility import MagicProperties
 from magpylib._src.defaults.defaults_utility import SUPPORTED_PLOTTING_BACKENDS
 from magpylib._src.defaults.defaults_utility import SYMBOLS_MATPLOTLIB_TO_PLOTLY
 from magpylib._src.defaults.defaults_utility import validate_property_class
 from magpylib._src.defaults.defaults_utility import validate_style_keys
 
 
+def get_families(obj):
+    "get obj families"
+    # pylint: disable=import-outside-toplevel
+    # pylint: disable=possibly-unused-variable
+    # pylint: disable=redefined-outer-name
+    from magpylib._src.obj_classes.class_BaseExcitations import BaseMagnet as Magnet
+    from magpylib._src.obj_classes.class_magnet_Cuboid import Cuboid
+    from magpylib._src.obj_classes.class_magnet_Cylinder import Cylinder
+    from magpylib._src.obj_classes.class_magnet_Sphere import Sphere
+    from magpylib._src.obj_classes.class_magnet_CylinderSegment import CylinderSegment
+    from magpylib._src.obj_classes.class_magnet_Tetrahedron import Tetrahedron
+    from magpylib._src.obj_classes.class_magnet_TriangularMesh import TriangularMesh
+    from magpylib._src.obj_classes.class_BaseExcitations import BaseCurrent as Current
+    from magpylib._src.obj_classes.class_current_Loop import Loop
+    from magpylib._src.obj_classes.class_current_Line import Line
+    from magpylib._src.obj_classes.class_misc_Dipole import Dipole
+    from magpylib._src.obj_classes.class_misc_CustomSource import CustomSource
+    from magpylib._src.obj_classes.class_misc_Triangle import Triangle
+    from magpylib._src.obj_classes.class_Sensor import Sensor
+    from magpylib._src.display.traces_generic import MagpyMarkers as Markers
+
+    loc = locals()
+    obj_families = []
+    for item, val in loc.items():
+        if not item.startswith("_"):
+            try:
+                if isinstance(obj, val):
+                    obj_families.append(item.lower())
+            except TypeError:
+                pass
+    return obj_families
+
+
 def get_style(obj, default_settings, **kwargs):
     """Returns default style based on increasing priority:
     - style from defaults
     - style from object
     - style from kwargs arguments
     """
-    # pylint: disable=import-outside-toplevel
-    from magpylib._src.obj_classes.class_BaseExcitations import (
-        BaseMagnet as MagpyMagnet,
-    )
-    from magpylib._src.obj_classes.class_BaseExcitations import (
-        BaseCurrent as MagpyCurrent,
-    )
-    from magpylib._src.obj_classes.class_misc_Dipole import Dipole as MagpyDipole
-    from magpylib._src.obj_classes.class_misc_Triangle import Triangle as MagpyTriangle
-    from magpylib._src.obj_classes.class_Sensor import Sensor as MagpySensor
-    from magpylib._src.display.traces_generic import MagpyMarkers
-
-    families = {
-        "triangle": MagpyTriangle,
-        "magnet": MagpyMagnet,
-        "current": MagpyCurrent,
-        "dipole": MagpyDipole,
-        "sensor": MagpySensor,
-        "markers": MagpyMarkers,
-    }
-    obj_family = None
-    for fam, cls in families.items():
-        if isinstance(obj, cls):
-            obj_family = fam
-            break
+    obj_families = get_families(obj)
     # parse kwargs into style an non-style arguments
     style_kwargs = kwargs.get("style", {})
     style_kwargs.update(
         {k[6:]: v for k, v in kwargs.items() if k.startswith("style") and k != "style"}
     )
 
     # retrieve default style dictionary, local import to avoid circular import
     # pylint: disable=import-outside-toplevel
 
-    styles_by_family = default_settings.display.style.as_dict()
+    default_style = default_settings.display.style
+    base_style_flat = default_style.base.as_dict(flatten=True, separator="_")
 
     # construct object specific dictionary base on style family and default style
-    obj_style_default_dict = {
-        **styles_by_family["base"],
-        **dict(styles_by_family.get(obj_family, {}).items()),
-    }
+    for obj_family in obj_families:
+        family_style = getattr(default_style, obj_family, {})
+        if family_style:
+            family_dict = family_style.as_dict(flatten=True, separator="_")
+            base_style_flat.update(
+                {k: v for k, v in family_dict.items() if v is not None}
+            )
     style_kwargs = validate_style_keys(style_kwargs)
 
     # create style class instance and update based on precedence
     obj_style = getattr(obj, "style", None)
     style = obj_style.copy() if obj_style is not None else BaseStyle()
     style_kwargs_specific = {
         k: v for k, v in style_kwargs.items() if k.split("_")[0] in style.as_dict()
     }
     style.update(**style_kwargs_specific, _match_properties=True)
-    style.update(
-        **obj_style_default_dict, _match_properties=False, _replace_None_only=True
-    )
+    style.update(**base_style_flat, _match_properties=False, _replace_None_only=True)
 
     return style
 
 
 class BaseStyle(MagicProperties):
     """Base class for display styling options of `BaseGeo` objects.
 
@@ -435,15 +446,16 @@
                 f"but received {type(val).__name__} instead."
             )
         self._kwargs = val
 
     @property
     def constructor(self):
         """Model constructor function or method to be called to build a 3D-model object
-        (e.g. 'plot_trisurf', 'Mesh3d). Must be in accordance with the given plotting backend."""
+        (e.g. 'plot_trisurf', 'Mesh3d). Must be in accordance with the given plotting backend.
+        """
         return self._constructor
 
     @constructor.setter
     def constructor(self, val):
         assert val is None or isinstance(val, str), (
             f"The `constructor` property of {type(self).__name__} must be a string,"
             f"\nbut received {repr(val)} instead."
@@ -566,16 +578,16 @@
 
     mode: {"auto", "arrow", "color", "arrow+color"}, default="auto"
         Magnetization can be displayed via arrows, color or both. By default `mode='auto'` means
         that the chosen backend determines which mode is applied by its capability. If the backend
         can display both and `auto` is chosen, the priority is given to `color`.
     """
 
-    def __init__(self, show=None, size=None, color=None, **kwargs):
-        super().__init__(show=show, size=size, color=color, **kwargs)
+    def __init__(self, show=None, size=None, color=None, mode=None, **kwargs):
+        super().__init__(show=show, size=size, color=color, mode=mode, **kwargs)
 
     @property
     def show(self):
         """If True, show magnetization direction."""
         return self._show
 
     @show.setter
@@ -750,15 +762,15 @@
     @magnetization.setter
     def magnetization(self, val):
         self._magnetization = validate_property_class(
             val, "magnetization", Magnetization, self
         )
 
 
-class Magnet(MagicProperties, MagnetProperties):
+class DefaultMagnet(MagicProperties, MagnetProperties):
     """Defines styling properties of homogeneous magnet classes.
 
     Parameters
     ----------
     magnetization: dict or Magnetization, default=None
     """
 
@@ -798,14 +810,197 @@
         or a dictionary with equivalent key/value pairs.
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
+class MarkerLineProperties:
+    """Defines styling properties of Markers and Lines."""
+
+    @property
+    def show(self):
+        """Show/hide path.
+        - False: Shows object(s) at final path position and hides paths lines and markers.
+        - True: Shows object(s) shows object paths depending on `line`, `marker` and `frames`
+        parameters.
+        """
+        return self._show
+
+    @show.setter
+    def show(self, val):
+        assert val is None or isinstance(val, bool), (
+            f"The `show` property of {type(self).__name__} must be either True or False,\n"
+            f"but received {repr(val)} instead."
+        )
+        self._show = val
+
+    @property
+    def marker(self):
+        """`Markers` object with 'color', 'symbol', 'size' properties."""
+        return self._marker
+
+    @marker.setter
+    def marker(self, val):
+        self._marker = validate_property_class(val, "marker", Marker, self)
+
+    @property
+    def line(self):
+        """`Line` object with 'color', 'type', 'width' properties."""
+        return self._line
+
+    @line.setter
+    def line(self, val):
+        self._line = validate_property_class(val, "line", Line, self)
+
+
+class GridMesh(MagicProperties, MarkerLineProperties):
+    """Defines styling properties of GridMesh objects
+
+    Parameters
+    ----------
+    show: bool, default=None
+        Show/hide Lines and Markers
+
+    marker: dict or `Markers` object, default=None
+        `Markers` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
+        key/value pairs.
+
+    line: dict or `Line` object, default=None
+        `Line` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
+        key/value pairs.
+    """
+
+
+class OpenMesh(MagicProperties, MarkerLineProperties):
+    """Defines styling properties of OpenMesh objects
+
+    Parameters
+    ----------
+    show: bool, default=None
+        Show/hide Lines and Markers
+
+    marker: dict or `Markers` object, default=None
+        `Markers` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
+        key/value pairs.
+
+    line: dict or `Line` object, default=None
+        `Line` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
+        key/value pairs.
+    """
+
+
+class DisconnectedMesh(MagicProperties, MarkerLineProperties):
+    """Defines styling properties of DisconnectedMesh objects
+
+    Parameters
+    ----------
+    show: bool, default=None
+        Show/hide Lines and Markers
+
+    marker: dict or `Markers` object, default=None
+        `Markers` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
+        key/value pairs.
+
+    line: dict or `Line` object, default=None
+        `Line` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
+        key/value pairs.
+
+    colorsequence: iterable, default=["red", "blue", "green", "cyan", "magenta", "yellow"]
+        An iterable of color values used to cycle trough for every disconnected part of
+        disconnected triangular mesh object.
+        A color may be specified by
+      - a hex string (e.g. '#ff0000')
+      - an rgb/rgba string (e.g. 'rgb(255,0,0)')
+      - an hsl/hsla string (e.g. 'hsl(0,100%,50%)')
+      - an hsv/hsva string (e.g. 'hsv(0,100%,100%)')
+      - a named CSS color
+    """
+
+    @property
+    def colorsequence(self):
+        """An iterable of color values used to cycle trough for every disconnected part of
+        disconnected triangular mesh object.
+          A color may be specified by
+        - a hex string (e.g. '#ff0000')
+        - an rgb/rgba string (e.g. 'rgb(255,0,0)')
+        - an hsl/hsla string (e.g. 'hsl(0,100%,50%)')
+        - an hsv/hsva string (e.g. 'hsv(0,100%,100%)')
+        - a named CSS color"""
+        return self._colorsequence
+
+    @colorsequence.setter
+    def colorsequence(self, val):
+        if val is not None:
+            name = type(self).__name__
+            try:
+                val = tuple(
+                    color_validator(c, allow_None=False, parent_name=f"{name}")
+                    for c in val
+                )
+            except TypeError as err:
+                raise ValueError(
+                    f"The `colorsequence` property of {name} must be an "
+                    f"iterable of colors but received {val!r} instead"
+                ) from err
+
+        self._colorsequence = val
+
+
+class TriMesh(MagicProperties):
+    """Defines TriMesh mesh properties.
+
+    Parameters
+    ----------
+    grid: dict or GridMesh,  default=None
+        All mesh vertices and edges of a TriangularMesh object.
+
+    open: dict or OpenMesh,  default=None
+        Shows open mesh vertices and edges of a TriangularMesh object, if any.
+
+    disconnected: dict or DisconnectedMesh, default=None
+        Shows disconnected bodies of a TriangularMesh object, if any.
+    """
+
+    @property
+    def grid(self):
+        """GridMesh` instance with `'show'` property
+        or a dictionary with equivalent key/value pairs.
+        """
+        return self._grid
+
+    @grid.setter
+    def grid(self, val):
+        self._grid = validate_property_class(val, "grid", GridMesh, self)
+
+    @property
+    def open(self):
+        """OpenMesh` instance with `'show'` property
+        or a dictionary with equivalent key/value pairs.
+        """
+        return self._open
+
+    @open.setter
+    def open(self, val):
+        self._open = validate_property_class(val, "open", OpenMesh, self)
+
+    @property
+    def disconnected(self):
+        """`DisconnectedMesh` instance with `'show'` property
+        or a dictionary with equivalent key/value pairs.
+        """
+        return self._disconnected
+
+    @disconnected.setter
+    def disconnected(self, val):
+        self._disconnected = validate_property_class(
+            val, "disconnected", DisconnectedMesh, self
+        )
+
+
 class Orientation(MagicProperties):
     """Defines Triangle orientation properties.
 
     Parameters
     ----------
     show: bool, default=True
         Show/hide orientation symbol.
@@ -818,15 +1013,15 @@
 
     offset: float, default=0.1
         Defines the orientation symbol offset, normal to the triangle surface. Must be a number
         between [0,1], 0 resulting in the cone/arrow head to be coincident to the triangle surface
         and 1 with the base.
 
     symbol: {"cone", "arrow3d"}:
-        Orientation symbol for the triangular facets.
+        Orientation symbol for the triangular faces.
     """
 
     _allowed_symbols = ("cone", "arrow3d")
 
     @property
     def show(self):
         """Show/hide arrow."""
@@ -912,16 +1107,16 @@
     @orientation.setter
     def orientation(self, val):
         self._orientation = validate_property_class(
             val, "orientation", Orientation, self
         )
 
 
-class Triangle(MagicProperties, MagnetProperties, TriangleProperties):
-    """Defines styling properties of homogeneous magnet classes.
+class DefaultTriangle(MagicProperties, MagnetProperties, TriangleProperties):
+    """Defines styling properties of the Triangle class.
 
     Parameters
     ----------
     magnetization: dict or Magnetization, default=None
         Magnetization styling with `'show'`, `'size'`, `'color'` properties
         or a dictionary with equivalent key/value pairs.
 
@@ -969,14 +1164,96 @@
         Orientation styling of triangles.
     """
 
     def __init__(self, orientation=None, **kwargs):
         super().__init__(orientation=orientation, **kwargs)
 
 
+class TriangularMeshProperties:
+    """Defines TriangularMesh properties."""
+
+    @property
+    def mesh(self):
+        """`TriMesh` instance with `'show', 'markers', 'line'` properties
+        or a dictionary with equivalent key/value pairs.
+        """
+        return self._mesh
+
+    @mesh.setter
+    def mesh(self, val):
+        self._mesh = validate_property_class(val, "mesh", TriMesh, self)
+
+
+class DefaultTriangularMesh(
+    MagicProperties, MagnetProperties, TriangleProperties, TriangularMeshProperties
+):
+    """Defines styling properties of homogeneous TriangularMesh magnet classes.
+
+    Parameters
+    ----------
+    magnetization: dict or Magnetization, default=None
+        Magnetization styling with `'show'`, `'size'`, `'color'` properties
+        or a dictionary with equivalent key/value pairs.
+
+    orientation: dict or Orientation,  default=None
+        Orientation of triangles styling with `'show'`, `'size'`, `'color', `'pivot'`, `'symbol'``
+        properties or a dictionary with equivalent key/value pairs.
+
+    mesh: dict or TriMesh, default=None
+        TriMesh styling properties (e.g. `'grid', 'open', 'disconnected'`)
+    """
+
+    def __init__(self, magnetization=None, orientation=None, mesh=None, **kwargs):
+        super().__init__(
+            magnetization=magnetization, orientation=orientation, mesh=mesh, **kwargs
+        )
+
+
+class TriangularMeshStyle(MagnetStyle, TriangleProperties, TriangularMeshProperties):
+    """Defines styling properties of the TriangularMesh magnet class.
+
+    Parameters
+    ----------
+    label: str, default=None
+        Label of the class instance, e.g. to be displayed in the legend.
+
+    description: dict or `Description` object, default=None
+        Object description properties.
+
+    color: str, default=None
+        A valid css color. Can also be one of `['r', 'g', 'b', 'y', 'm', 'c', 'k', 'w']`.
+
+    opacity: float, default=None
+        Object opacity between 0 and 1, where 1 is fully opaque and 0 is fully transparent.
+
+    path: dict or `Path` object, default=None
+        An instance of `Path` or dictionary of equivalent key/value pairs, defining the object
+        path marker and path line properties.
+
+    model3d: list of `Trace3d` objects, default=None
+        A list of traces where each is an instance of `Trace3d` or dictionary of equivalent
+        key/value pairs. Defines properties for an additional user-defined model3d object which is
+        positioned relatively to the main object to be displayed and moved automatically with it.
+        This feature also allows the user to replace the original 3d representation of the object.
+
+    magnetization: dict or Magnetization, default=None
+        Magnetization styling with `'show'`, `'size'`, `'color'` properties
+        or a dictionary with equivalent key/value pairs.
+
+    orientation: dict or Orientation,  default=None,
+        Orientation styling of triangles.
+
+    mesh: dict or TriMesh,  default=None,
+        mesh styling of triangles.
+    """
+
+    def __init__(self, orientation=None, **kwargs):
+        super().__init__(orientation=orientation, **kwargs)
+
+
 class ArrowCS(MagicProperties):
     """Defines triple coordinate system arrow properties.
 
     Parameters
     ----------
     x: dict or `ArrowSingle` object, default=None
         x-direction `Arrowsingle` object or dict with equivalent key/value pairs
@@ -1109,15 +1386,15 @@
         return self._arrows
 
     @arrows.setter
     def arrows(self, val):
         self._arrows = validate_property_class(val, "arrows", ArrowCS, self)
 
 
-class Sensor(MagicProperties, SensorProperties):
+class DefaultSensor(MagicProperties, SensorProperties):
     """Defines styling properties of the Sensor class.
 
     Parameters
     ----------
     size: float, default=None
         Positive float for ratio of sensor to canvas size.
 
@@ -1248,15 +1525,15 @@
         return self._arrow
 
     @arrow.setter
     def arrow(self, val):
         self._arrow = validate_property_class(val, "current", Arrow, self)
 
 
-class Current(MagicProperties, CurrentProperties):
+class DefaultCurrent(MagicProperties, CurrentProperties):
     """Defines the specific styling properties of line current classes.
 
     Parameters
     ----------
     arrow: dict or `Arrow`object, default=None
         `Arrow` object or dict with 'show', 'size' properties/keys.
     """
@@ -1407,15 +1684,15 @@
             f"The `symbol` property of {type(self).__name__} must be one of"
             f"{list(SYMBOLS_MATPLOTLIB_TO_PLOTLY.keys())},\n"
             f"but received {repr(val)} instead."
         )
         self._symbol = val
 
 
-class Markers(BaseStyle):
+class DefaultMarkers(BaseStyle):
     """Defines styling properties of the markers trace.
 
     Parameters
     ----------
     marker: dict or `Markers` object, default=None
         `Markers` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
         key/value pairs.
@@ -1475,15 +1752,15 @@
             f"The `pivot` property of {type(self).__name__} must be one of "
             f"{self._allowed_pivots},\n"
             f"but received {repr(val)} instead."
         )
         self._pivot = val
 
 
-class Dipole(MagicProperties, DipoleProperties):
+class DefaultDipole(MagicProperties, DipoleProperties):
     """
     Defines styling properties of dipoles.
 
     Parameters
     ----------
     size: float, default=None
         Positive float for ratio of dipole size to canvas size.
@@ -1532,90 +1809,55 @@
         The arrow rotates about this point. Can be one of `['tail', 'middle', 'tip']`.
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
-class Path(MagicProperties):
+class Path(MagicProperties, MarkerLineProperties):
     """Defines styling properties of an object's path.
 
     Parameters
     ----------
+    show: bool, default=None
+        Show/hide path.
+        - False: Shows object(s) at final path position and hides paths lines and markers.
+        - True: Shows object(s) shows object paths depending on `line`, `marker` and `frames`
+        parameters.
+
     marker: dict or `Markers` object, default=None
         `Markers` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
         key/value pairs.
 
     line: dict or `Line` object, default=None
         `Line` object with 'color', 'symbol', 'size' properties, or dictionary with equivalent
         key/value pairs.
 
-    show: bool, default=None
-        Show/hide path.
-        - False: Shows object(s) at final path position and hides paths lines and markers.
-        - True: Shows object(s) shows object paths depending on `line`, `marker` and `frames`
-        parameters.
-
     frames: int or array_like, shape (n,), default=None
         Show copies of the 3D-model along the given path indices.
         - integer i: Displays the object(s) at every i'th path position.
         - array_like, shape (n,), dtype=int: Displays object(s) at given path indices.
 
     numbering: bool, default=False
         Show/hide numbering on path positions.
     """
 
     def __init__(
-        self, marker=None, line=None, frames=None, show=None, numbering=None, **kwargs
+        self, show=None, marker=None, line=None, frames=None, numbering=None, **kwargs
     ):
         super().__init__(
+            show=show,
             marker=marker,
             line=line,
             frames=frames,
-            show=show,
             numbering=numbering,
             **kwargs,
         )
 
     @property
-    def marker(self):
-        """`Markers` object with 'color', 'symbol', 'size' properties."""
-        return self._marker
-
-    @marker.setter
-    def marker(self, val):
-        self._marker = validate_property_class(val, "marker", Marker, self)
-
-    @property
-    def line(self):
-        """`Line` object with 'color', 'type', 'width' properties."""
-        return self._line
-
-    @line.setter
-    def line(self, val):
-        self._line = validate_property_class(val, "line", Line, self)
-
-    @property
-    def show(self):
-        """Show/hide path.
-        - False: Shows object(s) at final path position and hides paths lines and markers.
-        - True: Shows object(s) shows object paths depending on `line`, `marker` and `frames`
-        parameters.
-        """
-        return self._show
-
-    @show.setter
-    def show(self, val):
-        assert val is None or isinstance(val, bool), (
-            f"The `show` property of {type(self).__name__} must be either True or False,\n"
-            f"but received {repr(val)} instead."
-        )
-        self._show = val
-
-    @property
     def frames(self):
         """Show copies of the 3D-model along the given path indices.
         - integer i: Displays the object(s) at every i'th path position.
         - array_like shape (n,) of integers: Displays object(s) at given path indices.
         """
         return self._frames
 
@@ -1768,58 +2010,69 @@
 
     @base.setter
     def base(self, val):
         self._base = validate_property_class(val, "base", BaseStyle, self)
 
     @property
     def magnet(self):
-        """Magnet class."""
+        """Magnet default style class."""
         return self._magnet
 
     @magnet.setter
     def magnet(self, val):
-        self._magnet = validate_property_class(val, "magnet", Magnet, self)
+        self._magnet = validate_property_class(val, "magnet", DefaultMagnet, self)
+
+    @property
+    def triangularmesh(self):
+        """TriangularMesh default style class."""
+        return self._triangularmesh
+
+    @triangularmesh.setter
+    def triangularmesh(self, val):
+        self._triangularmesh = validate_property_class(
+            val, "triangularmesh", DefaultTriangularMesh, self
+        )
 
     @property
     def current(self):
-        """Current class."""
+        """Current default style class."""
         return self._current
 
     @current.setter
     def current(self, val):
-        self._current = validate_property_class(val, "current", Current, self)
+        self._current = validate_property_class(val, "current", DefaultCurrent, self)
 
     @property
     def dipole(self):
-        """Dipole class."""
+        """Dipole default style class."""
         return self._dipole
 
     @dipole.setter
     def dipole(self, val):
-        self._dipole = validate_property_class(val, "dipole", Dipole, self)
+        self._dipole = validate_property_class(val, "dipole", DefaultDipole, self)
 
     @property
     def triangle(self):
-        """Triangle class."""
+        """Triangle default style class."""
         return self._triangle
 
     @triangle.setter
     def triangle(self, val):
-        self._triangle = validate_property_class(val, "triangle", Triangle, self)
+        self._triangle = validate_property_class(val, "triangle", DefaultTriangle, self)
 
     @property
     def sensor(self):
-        """Sensor class."""
+        """Sensor default style class."""
         return self._sensor
 
     @sensor.setter
     def sensor(self, val):
-        self._sensor = validate_property_class(val, "sensor", Sensor, self)
+        self._sensor = validate_property_class(val, "sensor", DefaultSensor, self)
 
     @property
     def markers(self):
-        """Markers class."""
+        """Markers default style class."""
         return self._markers
 
     @markers.setter
     def markers(self, val):
-        self._markers = validate_property_class(val, "markers", Markers, self)
+        self._markers = validate_property_class(val, "markers", DefaultMarkers, self)
```

### Comparing `magpylib-4.2.0/magpylib/_src/utility.py` & `magpylib-4.3.0rc1/magpylib/_src/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,7 +347,23 @@
     )
 
     return {
         k: v
         for k, v in get_subclasses(BaseSource, recursive=True).items()
         if not v in (BaseCurrent, BaseMagnet, BaseSource)
     }
+
+
+def is_notebook() -> bool:  # pragma: no cover
+    """Check if execution is within a IPython environment"""
+    # pylint: disable=import-outside-toplevel
+    try:
+        from IPython import get_ipython
+
+        shell = get_ipython().__class__.__name__
+        if shell == "ZMQInteractiveShell":
+            return True  # Jupyter notebook or qtconsole
+        if shell == "TerminalInteractiveShell":
+            return False  # Terminal running IPython
+        return False  # Other type (?)
+    except NameError:
+        return False  # Probably standard Python interpreter
```

### Comparing `magpylib-4.2.0/magpylib/core/__init__.py` & `magpylib-4.3.0rc1/magpylib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/graphics/model3d/__init__.py` & `magpylib-4.3.0rc1/magpylib/graphics/model3d/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/magpylib/magnet/__init__.py` & `magpylib-4.3.0rc1/magpylib/magnet/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 __all__ = [
     "Cuboid",
     "Cylinder",
     "Sphere",
     "CylinderSegment",
     "Tetrahedron",
+    "TriangularMesh",
 ]
 
 from magpylib._src.obj_classes.class_magnet_Cuboid import Cuboid
 from magpylib._src.obj_classes.class_magnet_Cylinder import Cylinder
 from magpylib._src.obj_classes.class_magnet_Sphere import Sphere
 from magpylib._src.obj_classes.class_magnet_CylinderSegment import CylinderSegment
 from magpylib._src.obj_classes.class_magnet_Tetrahedron import Tetrahedron
+from magpylib._src.obj_classes.class_magnet_TriangularMesh import TriangularMesh
```

### Comparing `magpylib-4.2.0/magpylib.egg-info/PKG-INFO` & `magpylib-4.3.0rc1/magpylib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: magpylib
-Version: 4.2.0
+Version: 4.3.0rc1
 Summary: Free Python3 package to compute magnetic fields.
 Home-page: https://github.com/magpylib/magpylib
 Author: Michael Ortner
 Author-email: magpylib@gmail.com
 License: 2-Clause BSD License, Simplified BSD License, FreeBSD License
 Keywords: magnetism physics analytical parallel electromagnetic fields b-field
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 <p align="center"><img align="center" src=docs/_static/images/magpylib_flag.png ><p>
 
@@ -42,28 +42,24 @@
 <a href="https://opensource.org/licenses/BSD-2-Clause"> <img align='center' src="https://img.shields.io/badge/License-BSD_2--Clause-orange.svg"> </a>
 </p>
 
 <p align="center"> Test Coverage:
 <a href="https://codecov.io/gh/magpylib/magpylib">
   <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg" />
 
-</a>
-<a href="https://lgtm.com/projects/g/magpylib/magpylib/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/magpylib/magpylib.svg?logo=lgtm&logoWidth=18"/></a>
-</p>
 
 <p align="center"> Downloads:
 <a href="https://pypi.org/project/magpylib/">
 <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/downloads.svg" alt="Conda Cloud" height="18"></a>
- <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/installer/conda.svg" alt="Conda Cloud" height="18"></a>
-</p>
+
 
 <p align="center"> Try it online:
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.0.0?filepath=docs%2Fexamples">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0rc1?filepath=docs%2Fexamples">
 <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18"></a>
 </p>
 
 </div>
 
 ---
 
@@ -73,15 +69,15 @@
 <p align="center">
     <img align='center' src=docs/_static/images/index/source_fundamentals.png>
 </p>
 
 ---
 
 ### Dependencies:
-_Python3.7+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_
+_Python3.8+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_
 
 ---
 
 ### Documentation & Install:
 
 **Please check out our [documentation](https://magpylib.readthedocs.io/en/latest) for installation, examples and detailed information!**
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: magpylib Version: 4.2.0 Summary: Free Python3
+Metadata-Version: 2.1 Name: magpylib Version: 4.3.0rc1 Summary: Free Python3
 package to compute magnetic fields. Home-page: https://github.com/magpylib/
 magpylib Author: Michael Ortner Author-email: magpylib@gmail.com License: 2-
 Clause BSD License, Simplified BSD License, FreeBSD License Keywords: magnetism
 physics analytical parallel electromagnetic fields b-field Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Intended Audience :: Education Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.7 Description-Content-Type: text/markdown Provides-Extra:
+Requires-Python: ~=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                     [docs/_static/images/magpylib_flag.png]
 ---
    Builds: [https://anaconda.org/conda-forge/magpylib/badges/platforms.svg]
          [https://dev.azure.com/magpylib/magpylib/_apis/build/status/
      magpylib.magpylib?branchName=main] [https://circleci.com/gh/magpylib/
                             magpylib.svg?style=svg]
        Documentation: [https://readthedocs.org/projects/magpylib/badge/
      ?version=latest] [https://img.shields.io/badge/License-BSD_2--Clause-
                                   orange.svg]
-  Test Coverage: [https://codecov.io/gh/magpylib/magpylib/branch/main/graph/
-                      badge.svg] [Language_grade:_Python]
-      Downloads: [PyPI_version] [Conda_Cloud] [Conda_Cloud] [Conda_Cloud]
-                        Try it online: [MyBinder_link]
+                                Test Coverage:
+     [https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg]
+             Downloads:_[PyPI_version]_[Conda_Cloud]_[Conda_Cloud]
+                        Try_it_online:_[MyBinder_link]
 --- ### What is magpylib ? Magpylib is a Python package for calculating **3D
 static magnetic fields** of magnets, line currents and other sources. The
 computation is based on analytical expressions and therefore **extremely
 fast**. A **user friendly geometry interface** enables convenient relative
 positioning between sources and observers.
               [docs/_static/images/index/source_fundamentals.png]
---- ### Dependencies: _Python3.7+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_ --
+--- ### Dependencies: _Python3.8+_, _Numpy_, _Scipy_, _Matplotlib_, _Plotly_ --
 - ### Documentation & Install: **Please check out our [documentation](https://
 magpylib.readthedocs.io/en/latest) for installation, examples and detailed
 information!** Magpylib is on PyPI and conda-forge. **Install using pip** (`pip
 install magpylib`) or **conda** (`conda install magpylib`) package managers.
```

### Comparing `magpylib-4.2.0/magpylib.egg-info/SOURCES.txt` & `magpylib-4.3.0rc1/magpylib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 magpylib/_src/fields/field_BH_cylinder_segment.py
 magpylib/_src/fields/field_BH_dipole.py
 magpylib/_src/fields/field_BH_line.py
 magpylib/_src/fields/field_BH_loop.py
 magpylib/_src/fields/field_BH_sphere.py
 magpylib/_src/fields/field_BH_tetrahedron.py
 magpylib/_src/fields/field_BH_triangle.py
+magpylib/_src/fields/field_BH_triangularmesh.py
 magpylib/_src/fields/field_wrap_BH.py
 magpylib/_src/fields/special_cel.py
 magpylib/_src/fields/special_el3.py
 magpylib/_src/obj_classes/__init__.py
 magpylib/_src/obj_classes/class_BaseDisplayRepr.py
 magpylib/_src/obj_classes/class_BaseExcitations.py
 magpylib/_src/obj_classes/class_BaseGeo.py
@@ -51,14 +52,15 @@
 magpylib/_src/obj_classes/class_current_Line.py
 magpylib/_src/obj_classes/class_current_Loop.py
 magpylib/_src/obj_classes/class_magnet_Cuboid.py
 magpylib/_src/obj_classes/class_magnet_Cylinder.py
 magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
 magpylib/_src/obj_classes/class_magnet_Sphere.py
 magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
+magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
 magpylib/_src/obj_classes/class_misc_CustomSource.py
 magpylib/_src/obj_classes/class_misc_Dipole.py
 magpylib/_src/obj_classes/class_misc_Triangle.py
 magpylib/core/__init__.py
 magpylib/current/__init__.py
 magpylib/graphics/__init__.py
 magpylib/graphics/model3d/__init__.py
@@ -91,18 +93,19 @@
 tests/test_obj_Collection.py
 tests/test_obj_Collection_child_parent.py
 tests/test_obj_Collection_v4motion.py
 tests/test_obj_Cuboid.py
 tests/test_obj_Cylinder.py
 tests/test_obj_CylinderSegment.py
 tests/test_obj_Dipole.py
-tests/test_obj_Facet.py
 tests/test_obj_Line.py
 tests/test_obj_Loop.py
 tests/test_obj_Sensor.py
 tests/test_obj_Sphere.py
 tests/test_obj_Tetrahedron.py
+tests/test_obj_Triangle.py
+tests/test_obj_TriangularMesh.py
 tests/test_path.py
 tests/test_physics_consistency.py
 tests/test_scaling.py
 tests/test_utility.py
 tests/test_vs_mag2.py
```

### Comparing `magpylib-4.2.0/setup.py` & `magpylib-4.3.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 # This is a basic setup.py structure so we can generate
 # distributable package information with setuptools.
 # More information: https://packaging.python.org/tutorials/packaging-projects/
 ###
 ###
 # Local install:
 #   Create virtual environment:
-#   $ conda create -n packCondaTest python=3.7.1 anaconda
+#   $ conda create -n packCondaTest python=3.8.1 anaconda
 #   Activate:
 #   $ conda activate packCondaTest
 #   Generate distribution files (untracked by git):
 #   $ (packCondaTest) python3 setup.py sdist bdist_wheel
 #   Install the generated library for the environment:
 #   $ (packCondaTest) pip install .
 # The library is now in the packCondaTest environment.
 ##
 import os
 import sys
 
 import setuptools
 from setuptools.command.install import install
 
-_magPyVersion = "4.2.0"
+_magPyVersion = "4.3.0rc1"
 _SphinxVersion = "4.4.0"
 _name = "magpylib"
 _description = "Free Python3 package to compute magnetic fields."
 _author_email = "magpylib@gmail.com"
 _author = "Michael Ortner"
 _projectUrl = "https://github.com/magpylib/magpylib"
 _release = "release"
@@ -71,34 +71,35 @@
     extras_require={
         "dev": [
             "kaleido",
             "pytest",
             "coverage",
             "pylint",
             "jupyterlab>=3.2",
+            "jupyterlab_myst",
             "sphinx==4.4.0",
             "pandas",
             "pyvista",
             "ipygany",
         ]
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
-    python_requires="~=3.7",
+    python_requires="~=3.8",
     keywords="magnetism physics analytical parallel electromagnetic fields b-field",
     command_options={
         "build_sphinx": {
             "project": ("setup.py", _name),
             "version": ("setup.py", _SphinxVersion),
             "release": ("setup.py", _release),
             "source_dir": ("setup.py", "./docs"),
```

### Comparing `magpylib-4.2.0/tests/test_BaseTransform.py` & `magpylib-4.3.0rc1/tests/test_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_Coumpound_setters.py` & `magpylib-4.3.0rc1/tests/test_Coumpound_setters.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_CustomSource.py` & `magpylib-4.3.0rc1/tests/test_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test__missing_optional_modules.py` & `magpylib-4.3.0rc1/tests/test__missing_optional_modules.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_core_field_functions.py` & `magpylib-4.3.0rc1/tests/test_core_field_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
     dim = np.array([(2, 2, 2)])
     bb = magpy.core.magnet_cuboid_field("B", obs, mag, dim)[0]
 
     np.testing.assert_allclose(b, bb)
 
 
 def test_triangle2():
-    """test core single triangle vs same surface split up into 4 triangles"""
+    """test core single triangle vs same surface split up into 4 triangular faces"""
     obs = np.array([(3, 4, 5)])
     mag = np.array([(111, 222, 333)])
     fac = np.array(
         [
             [(0, 0, 0), (10, 0, 0), (0, 10, 0)],
         ]
     )
```

### Comparing `magpylib-4.2.0/tests/test_default_utils.py` & `magpylib-4.3.0rc1/tests/test_default_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_defaults.py` & `magpylib-4.3.0rc1/tests/test_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "display_autosizefactor": (0,),  # float>0
     "display_animation_maxfps": (0,),  # int>0
     "display_animation_fps": (0,),  # int>0
     "display_animation_time": (0,),  # int>0
     "display_animation_maxframes": (0,),  # int>0
     "display_animation_slider": ("notbool"),  # bool
     "display_backend": ("plotty",),  # str typo
-    "display_colorsequence": (["#2E91E5", "wrongcolor"],),  # iterable of colors
+    "display_colorsequence": (["#2E91E5", "wrongcolor"], 123),  # iterable of colors
     "display_style_base_path_line_width": (-1,),  # float>=0
     "display_style_base_path_line_style": ("wrongstyle",),
     "display_style_base_path_line_color": ("wrongcolor",),  # color
     "display_style_base_path_marker_size": (-1,),  # float>=0
     "display_style_base_path_marker_symbol": ("wrongsymbol",),
     "display_style_base_path_marker_color": ("wrongcolor",),  # color
     "display_style_base_path_show": ("notbool", 1),  # bool
@@ -61,14 +61,15 @@
     "display_style_dipole_size": (-1,),  # float>=0
     "display_style_dipole_pivot": ("wrongpivot",),  # middle, tail, tip
     "display_style_triangle_orientation_show": ("notbool",),
     "display_style_triangle_orientation_size": (-1,),
     "display_style_triangle_orientation_color": ("wrongcolor",),
     "display_style_triangle_orientation_offset": ("-1",),  # float, int
     "display_style_triangle_orientation_symbol": ("arrow0d"),  # "cone", "arrow3d"
+    "display_style_triangularmesh_mesh_disconnected_colorsequence": (1,),
     "display_style_markers_marker_size": (-1,),  # float>=0
     "display_style_markers_marker_color": ("wrongcolor",),
     "display_style_markers_marker_symbol": ("wrongsymbol",),
 }
 
 
 def get_bad_test_data():
@@ -104,18 +105,18 @@
 good_inputs = {
     "display_autosizefactor": (1,),  # float>0
     "display_animation_maxfps": (10,),  # int>0
     "display_animation_fps": (10,),  # int>0
     "display_animation_time": (10,),  # int>0
     "display_animation_maxframes": (200,),  # int>0
     "display_animation_slider": (True, False),  # bool
-    "display_backend": tuple(SUPPORTED_PLOTTING_BACKENDS),  # str typo
+    "display_backend": ["auto", *SUPPORTED_PLOTTING_BACKENDS],  # str typo
     "display_colorsequence": (
-        ["#2E91E5", "#0D2A63"],
-        ["blue", "red"],
+        ("#2e91e5", "#0d2a63"),
+        ("blue", "red"),
     ),  # ]),  # iterable of colors
     "display_style_base_path_line_width": (0, 1),  # float>=0
     "display_style_base_path_line_style": LINESTYLES_MATPLOTLIB_TO_PLOTLY.keys(),
     "display_style_base_path_line_color": ("blue", "#2E91E5"),  # color
     "display_style_base_path_marker_size": (0, 1),  # float>=0
     "display_style_base_path_marker_symbol": SYMBOLS_MATPLOTLIB_TO_PLOTLY.keys(),
     "display_style_base_path_marker_color": ("blue", "#2E91E5"),  # color
```

### Comparing `magpylib-4.2.0/tests/test_display_plotly.py` & `magpylib-4.3.0rc1/tests/test_display_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_display_pyvista.py` & `magpylib-4.3.0rc1/tests/test_display_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_elliptics.py` & `magpylib-4.3.0rc1/tests/test_elliptics.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_exceptions.py` & `magpylib-4.3.0rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_field_cylinder.py` & `magpylib-4.3.0rc1/tests/test_field_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_getBH_dict.py` & `magpylib-4.3.0rc1/tests/test_getBH_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,15 @@
     dic["sources"] = pm
     with pytest.raises(MagpylibBadUserInput):
         magpylib.getB(**dic)
 
 
 def test_subclassing():
     """Test side effects of suclasssing a source"""
+
     # pylint: disable=unused-variable
     class MyCuboid(magpylib.magnet.Cuboid):
         """Test subclass"""
 
     B1 = magpylib.getB(
         "Cuboid", (0, 0, 0), magnetization=(1, 1, 1), dimension=(1, 1, 1)
     )
```

### Comparing `magpylib-4.2.0/tests/test_getBH_interfaces.py` & `magpylib-4.3.0rc1/tests/test_getBH_interfaces.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_getBH_level2.py` & `magpylib-4.3.0rc1/tests/test_getBH_level2.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     fc2 = np.array([fc1, fc1])
 
     for poso, fb, fc in zip(
         [pos_obs, sens1, sens2, sens3, [sens1, sens2]],
         [fb1, fb1, fb1, fb1, fb2],
         [fc1, fc1, fc1, fc1, fc2],
     ):
-
         src_obs_res = [
             [pm1, poso, fb],
             [pm3, poso, fc],
             [[pm1, pm2], poso, [fb, fb]],
             [[pm1, pm2, pm3], poso, [fb, fb, fc]],
             [col1, poso, fb],
             [col2, poso, 2 * fb],
```

### Comparing `magpylib-4.2.0/tests/test_input_checks.py` & `magpylib-4.3.0rc1/tests/test_input_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,14 +475,31 @@
         if field == "H":
             return np.array([1, 2, 3])
         return observers
 
     np.testing.assert_raises(MagpylibBadUserInput, magpy.misc.CustomSource, gg)
 
 
+def test_missing_input_triangular_mesh():
+    """missing input checks for TriangularMesh"""
+
+    verts = np.array([(0, 0, 0), (1, 0, 0), (0, 1, 0), (0, 0, 1)])
+    tris = np.array([(0, 1, 2), (0, 1, 3), (1, 2, 3), (0, 2, 3)])
+
+    def trim():
+        magpy.magnet.TriangularMesh(faces=tris)
+
+    np.testing.assert_raises(MagpylibMissingInput, trim)
+
+    def trimm():
+        magpy.magnet.TriangularMesh(vertices=verts)
+
+    np.testing.assert_raises(MagpylibMissingInput, trimm)
+
+
 ###########################################################
 ###########################################################
 # DISPLAY
 
 
 def test_input_show_zoom_bad():
     """bad show zoom inputs"""
```

### Comparing `magpylib-4.2.0/tests/test_numerical_stability.py` & `magpylib-4.3.0rc1/tests/test_numerical_stability.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_BaseGeo.py` & `magpylib-4.3.0rc1/tests/test_obj_BaseGeo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 import numpy as np
 import pytest
+import pyvista as pv
 from scipy.spatial.transform import Rotation as R
 
 import magpylib as magpy
 from magpylib._src.obj_classes.class_BaseGeo import BaseGeo
 
 
 def test_BaseGeo_basics():
@@ -507,7 +508,33 @@
         + "  • parent: None \n"
         + "  • position: [0. 0. 0.] mm\n"
         + "  • orientation: [0. 0. 0.] degrees\n"
         + "  • pixel: 75 (3x5x5) "
     )
     desc = re.sub("id=*[0-9]*[0-9]", "id=REGEX", desc)
     assert desc == test
+
+    # describe tringularmesh
+    s = magpy.magnet.TriangularMesh.from_pyvista(
+        magnetization=(0, 0, 1000),
+        polydata=pv.Text3D("A"),
+    )
+    desc = s.describe(return_string=True)
+    test = (
+        "TriangularMesh(id=REGEX)\n"
+        "  • parent: None \n"
+        "  • position: [0. 0. 0.] mm\n"
+        "  • orientation: [0. 0. 0.] degrees\n"
+        "  • magnetization: [   0.    0. 1000.] mT\n"
+        "  • barycenter: [0.64466889 0.42195708 0.25      ] \n"
+        "  • faces: shape(52, 3) \n"
+        "  • mesh: shape(52, 3, 3) \n"
+        "  • status_disconnected: False \n"
+        "  • status_disconnected_data: 1 part \n"
+        "  • status_open: False \n"
+        "  • status_open_data: [] \n"
+        "  • status_reoriented: True \n"
+        "  • vertices: shape(26, 3) "
+    )
+    desc = re.sub("id=*[0-9]*[0-9]", "id=REGEX", desc)
+    # to create test: print('\\n"\n'.join(f'"{s}' for s in desc.split("\n")) + '"')
+    assert desc == test
```

### Comparing `magpylib-4.2.0/tests/test_obj_BaseGeo_v4motion.py` & `magpylib-4.3.0rc1/tests/test_obj_BaseGeo_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Collection.py` & `magpylib-4.3.0rc1/tests/test_obj_Collection.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Collection_child_parent.py` & `magpylib-4.3.0rc1/tests/test_obj_Collection_child_parent.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Collection_v4motion.py` & `magpylib-4.3.0rc1/tests/test_obj_Collection_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Cuboid.py` & `magpylib-4.3.0rc1/tests/test_obj_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Cylinder.py` & `magpylib-4.3.0rc1/tests/test_obj_Cylinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         (-12, -13, -14),
     ]
 
     dim2 = [(1, 2), (2, 3), (3, 4)]
     dim5 = [(0, 0.5, 2, 0, 360), (0, 1, 3, 0, 360), (0.0000001, 1.5, 4, 0, 360)]
 
     for d2, d5 in zip(dim2, dim5):
-
         src1 = magpy.magnet.Cylinder(mag, d2)
         src2 = magpy.magnet.CylinderSegment(mag, d5)
         B0 = src1.getB(poso)
         H0 = src1.getH(poso)
 
         B1 = src2.getB(poso)
         H1 = src2.getH(poso)
```

### Comparing `magpylib-4.2.0/tests/test_obj_CylinderSegment.py` & `magpylib-4.3.0rc1/tests/test_obj_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Dipole.py` & `magpylib-4.3.0rc1/tests/test_obj_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Facet.py` & `magpylib-4.3.0rc1/tests/test_obj_Triangle.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,14 @@
     def call_getB():
         """dummy function call getB"""
         fac.getB()
 
     np.testing.assert_raises(MagpylibMissingInput, call_getB)
 
 
-def test_barycenter():
-    """call barycenter"""
+def test_Triangle_barycenter():
+    """test Triangle barycenter"""
     mag = (0, 0, 333)
     vert = ((-1, -1, 0), (1, -1, 0), (0, 2, 0))
     face = magpy.misc.Triangle(mag, vert)
     bary = np.array([0, 0, 0])
     np.testing.assert_allclose(face.barycenter, bary)
```

### Comparing `magpylib-4.2.0/tests/test_obj_Line.py` & `magpylib-4.3.0rc1/tests/test_obj_Line.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Loop.py` & `magpylib-4.3.0rc1/tests/test_obj_Loop.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Sensor.py` & `magpylib-4.3.0rc1/tests/test_obj_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Sphere.py` & `magpylib-4.3.0rc1/tests/test_obj_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_obj_Tetrahedron.py` & `magpylib-4.3.0rc1/tests/test_obj_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_path.py` & `magpylib-4.3.0rc1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_physics_consistency.py` & `magpylib-4.3.0rc1/tests/test_physics_consistency.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_scaling.py` & `magpylib-4.3.0rc1/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_utility.py` & `magpylib-4.3.0rc1/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.2.0/tests/test_vs_mag2.py` & `magpylib-4.3.0rc1/tests/test_vs_mag2.py`

 * *Files identical despite different names*

