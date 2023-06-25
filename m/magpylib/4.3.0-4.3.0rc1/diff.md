# Comparing `tmp/magpylib-4.3.0.tar.gz` & `tmp/magpylib-4.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib-4.3.0.tar", last modified: Sun Jun 25 10:17:54 2023, max compression
+gzip compressed data, was "magpylib-4.3.0rc1.tar", last modified: Sun Jun 25 09:59:26 2023, max compression
```

## Comparing `magpylib-4.3.0.tar` & `magpylib-4.3.0rc1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.266779 magpylib-4.3.0/
--rw-r--r--   0 root         (0) root         (0)    28503 2023-06-25 10:17:22.000000 magpylib-4.3.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-25 10:17:22.000000 magpylib-4.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-25 10:17:22.000000 magpylib-4.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3709 2023-06-25 10:17:54.266779 magpylib-4.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2698 2023-06-25 10:17:22.000000 magpylib-4.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.254778 magpylib-4.3.0/magpylib/
--rw-r--r--   0 root         (0) root         (0)     1582 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.254778 magpylib-4.3.0/magpylib/_src/
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.254778 magpylib-4.3.0/magpylib/_src/defaults/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/defaults/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8636 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/defaults/defaults_classes.py
--rw-r--r--   0 root         (0) root         (0)    13988 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/defaults/defaults_utility.py
--rw-r--r--   0 root         (0) root         (0)     4511 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/defaults/defaults_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.258779 magpylib-4.3.0/magpylib/_src/display/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6552 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/backend_matplotlib.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/backend_plotly.py
--rw-r--r--   0 root         (0) root         (0)     5485 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/backend_pyvista.py
--rw-r--r--   0 root         (0) root         (0)     6764 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/display.py
--rw-r--r--   0 root         (0) root         (0)    10671 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/sensor_mesh.py
--rw-r--r--   0 root         (0) root         (0)    21826 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/traces_base.py
--rw-r--r--   0 root         (0) root         (0)    46592 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/traces_generic.py
--rw-r--r--   0 root         (0) root         (0)    19803 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/display/traces_utility.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.258779 magpylib-4.3.0/magpylib/_src/fields/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9322 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_cuboid.py
--rw-r--r--   0 root         (0) root         (0)    15908 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_cylinder.py
--rw-r--r--   0 root         (0) root         (0)    78106 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_cylinder_segment.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_dipole.py
--rw-r--r--   0 root         (0) root         (0)     6896 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_line.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_loop.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_sphere.py
--rw-r--r--   0 root         (0) root         (0)     4524 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_triangle.py
--rw-r--r--   0 root         (0) root         (0)    16435 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_BH_triangularmesh.py
--rw-r--r--   0 root         (0) root         (0)    33890 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/field_wrap_BH.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/special_cel.py
--rw-r--r--   0 root         (0) root         (0)    17660 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/fields/special_el3.py
--rw-r--r--   0 root         (0) root         (0)    22737 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/input_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/_src/obj_classes/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3990 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseExcitations.py
--rw-r--r--   0 root         (0) root         (0)    12264 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseGeo.py
--rw-r--r--   0 root         (0) root         (0)    34373 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseTransform.py
--rw-r--r--   0 root         (0) root         (0)    26941 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_Collection.py
--rw-r--r--   0 root         (0) root         (0)     9838 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_Sensor.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_current_Line.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_current_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4199 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Cuboid.py
--rw-r--r--   0 root         (0) root         (0)     4301 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Cylinder.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
--rw-r--r--   0 root         (0) root         (0)     4008 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Sphere.py
--rw-r--r--   0 root         (0) root         (0)     5406 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)    29813 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_misc_CustomSource.py
--rw-r--r--   0 root         (0) root         (0)     4022 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_misc_Dipole.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/obj_classes/class_misc_Triangle.py
--rw-r--r--   0 root         (0) root         (0)    69917 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/style.py
--rw-r--r--   0 root         (0) root         (0)    11184 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/_src/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/core/
--rw-r--r--   0 root         (0) root         (0)      980 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/current/
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/current/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/graphics/
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/graphics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/graphics/model3d/
--rw-r--r--   0 root         (0) root         (0)      557 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/graphics/model3d/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/graphics/style/
--rw-r--r--   0 root         (0) root         (0)      280 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/graphics/style/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/magnet/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/magnet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.262779 magpylib-4.3.0/magpylib/misc/
--rw-r--r--   0 root         (0) root         (0)      335 2023-06-25 10:17:22.000000 magpylib-4.3.0/magpylib/misc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.254778 magpylib-4.3.0/magpylib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3709 2023-06-25 10:17:54.000000 magpylib-4.3.0/magpylib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3745 2023-06-25 10:17:54.000000 magpylib-4.3.0/magpylib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 10:17:54.000000 magpylib-4.3.0/magpylib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 10:17:33.000000 magpylib-4.3.0/magpylib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-25 10:17:54.000000 magpylib-4.3.0/magpylib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-25 10:17:54.000000 magpylib-4.3.0/magpylib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 10:17:54.266779 magpylib-4.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-25 10:17:22.000000 magpylib-4.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:17:54.266779 magpylib-4.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13101 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_BaseTransform.py
--rw-r--r--   0 root         (0) root         (0)     5458 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_Coumpound_setters.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_CustomSource.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test__missing_optional_modules.py
--rw-r--r--   0 root         (0) root         (0)    16997 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_core_field_functions.py
--rw-r--r--   0 root         (0) root         (0)     7074 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_default_utils.py
--rw-r--r--   0 root         (0) root         (0)    10767 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_defaults.py
--rw-r--r--   0 root         (0) root         (0)    13681 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_display_matplotlib.py
--rw-r--r--   0 root         (0) root         (0)    10505 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_display_plotly.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_display_pyvista.py
--rw-r--r--   0 root         (0) root         (0)     2802 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_display_utility.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_elliptics.py
--rw-r--r--   0 root         (0) root         (0)     8671 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14085 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_field_cylinder.py
--rw-r--r--   0 root         (0) root         (0)    12137 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_getBH_dict.py
--rw-r--r--   0 root         (0) root         (0)     7627 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_getBH_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    17329 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_getBH_level2.py
--rw-r--r--   0 root         (0) root         (0)    25228 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_input_checks.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_misc.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_numerical_stability.py
--rw-r--r--   0 root         (0) root         (0)    18735 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_BaseGeo.py
--rw-r--r--   0 root         (0) root         (0)    12060 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_BaseGeo_v4motion.py
--rw-r--r--   0 root         (0) root         (0)    15492 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Collection.py
--rw-r--r--   0 root         (0) root         (0)    10144 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Collection_child_parent.py
--rw-r--r--   0 root         (0) root         (0)    23139 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Collection_v4motion.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Cuboid.py
--rw-r--r--   0 root         (0) root         (0)     2839 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Cylinder.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_CylinderSegment.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Dipole.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Line.py
--rw-r--r--   0 root         (0) root         (0)     1726 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Loop.py
--rw-r--r--   0 root         (0) root         (0)     3754 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Sensor.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Sphere.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_Triangle.py
--rw-r--r--   0 root         (0) root         (0)    14087 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_obj_TriangularMesh.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_path.py
--rw-r--r--   0 root         (0) root         (0)    10074 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_physics_consistency.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_utility.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-06-25 10:17:22.000000 magpylib-4.3.0/tests/test_vs_mag2.py
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

### Comparing `magpylib-4.3.0/CHANGELOG.md` & `magpylib-4.3.0rc1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 All notable changes to magpylib are documented here.
 
 
 # Releases
 
-## [4.3.0] - 2023-06-25
+## [4.3.0rc1] - 2023-06-25
 - New `TriangularMesh` magnet class added to conveniently work with triangular surface meshes instead of large collections of individual `Triangle` objects. The `TriangularMesh` class performs important checks (closed, connected, oriented) and can directly import pyvista objects and for convex hull bodies. ([#569](https://github.com/magpylib/magpylib/issues/569), [#598](https://github.com/magpylib/magpylib/pull/598)).
 - Added magnetization coloring for `matplotlib` backend ([#597](https://github.com/magpylib/magpylib/pull/597))
 - New automatic backend behavior, set to a dynamic default `auto` depending on the current environment and the given `canvas`, if provided. ([#617](https://github.com/magpylib/magpylib/pull/617))
 - Drop python 3.7 support, following python life cycle. ([#616](https://github.com/magpylib/magpylib/pull/616))
 
 ## [4.2.0] - 2023-01-27
 - (Re)introducing the powerful `misc.Triangle` class that can be used to compute magnetic fields of arbitrarily shaped bodies by approximating their surface with triangular faces. ([#568](https://github.com/magpylib/magpylib/issues/568))
@@ -407,16 +407,16 @@
    - Loop Current
    - Current Line
    - Dipole
 - Collection class
 
 ---
 
-[Unreleased]:https://github.com/magpylib/magpylib/compare/4.3.0...HEAD
-[4.3.0]:https://github.com/magpylib/magpylib/compare/4.2.0...4.3.0
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

### Comparing `magpylib-4.3.0/LICENSE` & `magpylib-4.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/PKG-INFO` & `magpylib-4.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib
-Version: 4.3.0
+Version: 4.3.0rc1
 Summary: Free Python3 package to compute magnetic fields.
 Home-page: https://github.com/magpylib/magpylib
 Author: Michael Ortner
 Author-email: magpylib@gmail.com
 License: 2-Clause BSD License, Simplified BSD License, FreeBSD License
 Keywords: magnetism physics analytical parallel electromagnetic fields b-field
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 <a href="https://pypi.org/project/magpylib/">
 <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/downloads.svg" alt="Conda Cloud" height="18"></a>
 
 
 <p align="center"> Try it online:
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0?filepath=docs%2Fexamples">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0rc1?filepath=docs%2Fexamples">
 <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18"></a>
 </p>
 
 </div>
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: magpylib Version: 4.3.0 Summary: Free Python3
+Metadata-Version: 2.1 Name: magpylib Version: 4.3.0rc1 Summary: Free Python3
 package to compute magnetic fields. Home-page: https://github.com/magpylib/
 magpylib Author: Michael Ortner Author-email: magpylib@gmail.com License: 2-
 Clause BSD License, Simplified BSD License, FreeBSD License Keywords: magnetism
 physics analytical parallel electromagnetic fields b-field Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `magpylib-4.3.0/README.md` & `magpylib-4.3.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 <a href="https://pypi.org/project/magpylib/">
 <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/downloads.svg" alt="Conda Cloud" height="18"></a>
 
 
 <p align="center"> Try it online:
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0?filepath=docs%2Fexamples">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0rc1?filepath=docs%2Fexamples">
 <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18"></a>
 </p>
 
 </div>
 
 ---
```

### Comparing `magpylib-4.3.0/magpylib/__init__.py` & `magpylib-4.3.0rc1/magpylib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 The original software publication (version 2):
 
 https://www.sciencedirect.com/science/article/pii/S2352711020300170
 
 """
 # module level dunders
-__version__ = "4.3.0"
+__version__ = "4.3.0rc1"
 __author__ = "Michael Ortner & Alexandre Boisselet"
 __credits__ = "The Magpylib community"
 __all__ = [
     "magnet",
     "current",
     "misc",
     "getB",
```

### Comparing `magpylib-4.3.0/magpylib/_src/defaults/defaults_classes.py` & `magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_classes.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/defaults/defaults_utility.py` & `magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/defaults/defaults_values.py` & `magpylib-4.3.0rc1/magpylib/_src/defaults/defaults_values.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/backend_matplotlib.py` & `magpylib-4.3.0rc1/magpylib/_src/display/backend_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/backend_plotly.py` & `magpylib-4.3.0rc1/magpylib/_src/display/backend_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/backend_pyvista.py` & `magpylib-4.3.0rc1/magpylib/_src/display/backend_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/display.py` & `magpylib-4.3.0rc1/magpylib/_src/display/display.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/sensor_mesh.py` & `magpylib-4.3.0rc1/magpylib/_src/display/sensor_mesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/traces_base.py` & `magpylib-4.3.0rc1/magpylib/_src/display/traces_base.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/traces_generic.py` & `magpylib-4.3.0rc1/magpylib/_src/display/traces_generic.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/display/traces_utility.py` & `magpylib-4.3.0rc1/magpylib/_src/display/traces_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_cuboid.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_cylinder.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_cylinder_segment.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_cylinder_segment.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_dipole.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_line.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_line.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_loop.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_loop.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_sphere.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_tetrahedron.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_triangle.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_BH_triangularmesh.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_BH_triangularmesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/field_wrap_BH.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/field_wrap_BH.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/special_cel.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/special_cel.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/fields/special_el3.py` & `magpylib-4.3.0rc1/magpylib/_src/fields/special_el3.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/input_checks.py` & `magpylib-4.3.0rc1/magpylib/_src/input_checks.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseDisplayRepr.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseDisplayRepr.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseExcitations.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseExcitations.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseGeo.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseGeo.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_BaseTransform.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_Collection.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_Collection.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_Sensor.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_current_Line.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_current_Line.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_current_Loop.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_current_Loop.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Cuboid.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Cylinder.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Sphere.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_misc_CustomSource.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_misc_Dipole.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/obj_classes/class_misc_Triangle.py` & `magpylib-4.3.0rc1/magpylib/_src/obj_classes/class_misc_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/style.py` & `magpylib-4.3.0rc1/magpylib/_src/style.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/_src/utility.py` & `magpylib-4.3.0rc1/magpylib/_src/utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/core/__init__.py` & `magpylib-4.3.0rc1/magpylib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/graphics/model3d/__init__.py` & `magpylib-4.3.0rc1/magpylib/graphics/model3d/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib/magnet/__init__.py` & `magpylib-4.3.0rc1/magpylib/magnet/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/magpylib.egg-info/PKG-INFO` & `magpylib-4.3.0rc1/magpylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib
-Version: 4.3.0
+Version: 4.3.0rc1
 Summary: Free Python3 package to compute magnetic fields.
 Home-page: https://github.com/magpylib/magpylib
 Author: Michael Ortner
 Author-email: magpylib@gmail.com
 License: 2-Clause BSD License, Simplified BSD License, FreeBSD License
 Keywords: magnetism physics analytical parallel electromagnetic fields b-field
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 <a href="https://pypi.org/project/magpylib/">
 <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18"></a>
 <a href="https://anaconda.org/conda-forge/magpylib"><img src="https://anaconda.org/conda-forge/magpylib/badges/downloads.svg" alt="Conda Cloud" height="18"></a>
 
 
 <p align="center"> Try it online:
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0?filepath=docs%2Fexamples">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/4.3.0rc1?filepath=docs%2Fexamples">
 <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18"></a>
 </p>
 
 </div>
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: magpylib Version: 4.3.0 Summary: Free Python3
+Metadata-Version: 2.1 Name: magpylib Version: 4.3.0rc1 Summary: Free Python3
 package to compute magnetic fields. Home-page: https://github.com/magpylib/
 magpylib Author: Michael Ortner Author-email: magpylib@gmail.com License: 2-
 Clause BSD License, Simplified BSD License, FreeBSD License Keywords: magnetism
 physics analytical parallel electromagnetic fields b-field Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `magpylib-4.3.0/magpylib.egg-info/SOURCES.txt` & `magpylib-4.3.0rc1/magpylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/setup.py` & `magpylib-4.3.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ##
 import os
 import sys
 
 import setuptools
 from setuptools.command.install import install
 
-_magPyVersion = "4.3.0"
+_magPyVersion = "4.3.0rc1"
 _SphinxVersion = "4.4.0"
 _name = "magpylib"
 _description = "Free Python3 package to compute magnetic fields."
 _author_email = "magpylib@gmail.com"
 _author = "Michael Ortner"
 _projectUrl = "https://github.com/magpylib/magpylib"
 _release = "release"
```

### Comparing `magpylib-4.3.0/tests/test_BaseTransform.py` & `magpylib-4.3.0rc1/tests/test_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_Coumpound_setters.py` & `magpylib-4.3.0rc1/tests/test_Coumpound_setters.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_CustomSource.py` & `magpylib-4.3.0rc1/tests/test_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test__missing_optional_modules.py` & `magpylib-4.3.0rc1/tests/test__missing_optional_modules.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_core_field_functions.py` & `magpylib-4.3.0rc1/tests/test_core_field_functions.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_default_utils.py` & `magpylib-4.3.0rc1/tests/test_default_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_defaults.py` & `magpylib-4.3.0rc1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_display_matplotlib.py` & `magpylib-4.3.0rc1/tests/test_display_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_display_plotly.py` & `magpylib-4.3.0rc1/tests/test_display_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_display_pyvista.py` & `magpylib-4.3.0rc1/tests/test_display_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_display_utility.py` & `magpylib-4.3.0rc1/tests/test_display_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_elliptics.py` & `magpylib-4.3.0rc1/tests/test_elliptics.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_exceptions.py` & `magpylib-4.3.0rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_field_cylinder.py` & `magpylib-4.3.0rc1/tests/test_field_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_getBH_dict.py` & `magpylib-4.3.0rc1/tests/test_getBH_dict.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_getBH_interfaces.py` & `magpylib-4.3.0rc1/tests/test_getBH_interfaces.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_getBH_level2.py` & `magpylib-4.3.0rc1/tests/test_getBH_level2.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_input_checks.py` & `magpylib-4.3.0rc1/tests/test_input_checks.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_numerical_stability.py` & `magpylib-4.3.0rc1/tests/test_numerical_stability.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_BaseGeo.py` & `magpylib-4.3.0rc1/tests/test_obj_BaseGeo.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_BaseGeo_v4motion.py` & `magpylib-4.3.0rc1/tests/test_obj_BaseGeo_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Collection.py` & `magpylib-4.3.0rc1/tests/test_obj_Collection.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Collection_child_parent.py` & `magpylib-4.3.0rc1/tests/test_obj_Collection_child_parent.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Collection_v4motion.py` & `magpylib-4.3.0rc1/tests/test_obj_Collection_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Cuboid.py` & `magpylib-4.3.0rc1/tests/test_obj_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Cylinder.py` & `magpylib-4.3.0rc1/tests/test_obj_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_CylinderSegment.py` & `magpylib-4.3.0rc1/tests/test_obj_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Dipole.py` & `magpylib-4.3.0rc1/tests/test_obj_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Line.py` & `magpylib-4.3.0rc1/tests/test_obj_Line.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Loop.py` & `magpylib-4.3.0rc1/tests/test_obj_Loop.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Sensor.py` & `magpylib-4.3.0rc1/tests/test_obj_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Sphere.py` & `magpylib-4.3.0rc1/tests/test_obj_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Tetrahedron.py` & `magpylib-4.3.0rc1/tests/test_obj_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_Triangle.py` & `magpylib-4.3.0rc1/tests/test_obj_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_obj_TriangularMesh.py` & `magpylib-4.3.0rc1/tests/test_obj_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_path.py` & `magpylib-4.3.0rc1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_physics_consistency.py` & `magpylib-4.3.0rc1/tests/test_physics_consistency.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_scaling.py` & `magpylib-4.3.0rc1/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_utility.py` & `magpylib-4.3.0rc1/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-4.3.0/tests/test_vs_mag2.py` & `magpylib-4.3.0rc1/tests/test_vs_mag2.py`

 * *Files identical despite different names*

