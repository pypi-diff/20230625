# Comparing `tmp/apysc-2.8.9.tar.gz` & `tmp/apysc-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apysc-2.8.9.tar", last modified: Sun Jun 18 06:11:54 2023, max compression
+gzip compressed data, was "apysc-3.0.0.tar", last modified: Sun Jun 25 03:39:46 2023, max compression
```

## Comparing `apysc-2.8.9.tar` & `apysc-3.0.0.tar`

### file list

```diff
@@ -1,687 +1,690 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.304927 apysc-2.8.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-18 06:11:28.000000 apysc-2.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 06:11:28.000000 apysc-2.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-18 06:11:54.304927 apysc-2.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-18 06:11:28.000000 apysc-2.8.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.240927 apysc-2.8.9/apysc/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.244927 apysc-2.8.9/apysc/_animation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_cy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_finish_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_height.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_height_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_height_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_parallel_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_pause_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_play_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_reset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_reverse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_x_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_x_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_time_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_width.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_width_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_width_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/animation_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_animation/easing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.244927 apysc-2.8.9/apysc/_auto_reloading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_auto_reloading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_auto_reloading/auto_reloading_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.244927 apysc-2.8.9/apysc/_branch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_branch/_elif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_branch/_else.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_branch/_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_branch/if_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.244927 apysc-2.8.9/apysc/_callable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_callable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_callable/callable_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.252927 apysc-2.8.9/apysc/_chart/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/add_background_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/add_border_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_label_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_label_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_label_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_label_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_label_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_label_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/axis_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/background_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/border_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/chart_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/chart_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/create_single_column_y_axis_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/initialize_each_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/is_display_axis_label_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/overall_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_background_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_background_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_border_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_border_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_border_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_horizontal_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_matrix_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_vertical_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/set_initial_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/tick_max_num_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/tick_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/tick_text_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/tick_text_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/tick_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/tick_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/tick_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/vertical_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/x_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/x_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/x_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/x_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/x_axis_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/y_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/y_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/y_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/y_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/y_axis_single_column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/y_max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_chart/y_min_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.252927 apysc-2.8.9/apysc/_color/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_color/color_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.252927 apysc-2.8.9/apysc/_console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_console/_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    31274 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_console/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_console/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.252927 apysc-2.8.9/apysc/_converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_converter/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_converter/to_apysc_val_from_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_converter/to_builtin_val_from_apysc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.264927 apysc-2.8.9/apysc/_display/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/any_display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_fill_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_fill_color_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_line_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_line_cap_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_line_color_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_line_joints_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_line_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_line_thickness_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_x_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/append_y_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/begin_fill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/css_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/ellipse_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/ellipse_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/flip_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/flip_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/flip_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/get_bounds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    48598 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/graphics_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/graphics_clear_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/graphics_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_cap_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_caps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_dash_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_dash_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_joints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_joints_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_round_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_style_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/points_2d_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/points_var_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_append_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_apply_current_points_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_x3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polygon_y3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/rotation_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/scale_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/set_lower_scale_limit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/set_overflow_visible_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/skew_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/skew_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_font_size_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_set_text_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_singleton_for_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/svg_text_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/visible_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/width_and_height_mixin_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/x_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/y_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_display/y_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.264927 apysc-2.8.9/apysc/_event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/custom_event_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/custom_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/document_mouse_wheel_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/double_click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/enter_frame_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/enter_frame_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/handler_circular_calling_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_down_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_event_binding_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_event_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_event_unbinding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_out_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_over_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/mouse_up_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/prevent_default_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/set_handler_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/stop_propagation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_event/wheel_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.264927 apysc-2.8.9/apysc/_expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/event_handler_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/expression_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/expression_variables_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/get_last_scope_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/indent_num.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/js_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/last_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_expression/var_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.268927 apysc-2.8.9/apysc/_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_file/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_file/module_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.268927 apysc-2.8.9/apysc/_geom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_control_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_control_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_control_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_control_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_control_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_control_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_data_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_dest_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_dest_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/path_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_bottom_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_center_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_center_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_left_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_right_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_top_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/rectangle_geom_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_geom/relative_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.268927 apysc-2.8.9/apysc/_html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_html/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_html/html_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_html/html_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.272927 apysc-2.8.9/apysc/_jslib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jslib/jquery-3.6.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jslib/jslib_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jslib/svg-3.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jslib/underscore-1.12.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.272927 apysc-2.8.9/apysc/_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_jupyter/jupyter_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.272927 apysc-2.8.9/apysc/_lint_and_doc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/conf_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/docs_keyword_link_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/docs_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/docs_toctree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/docs_translation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/docstring_to_markdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/docstring_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/document_text_split_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/document_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.272927 apysc-2.8.9/apysc/_lint_and_doc/fixed_translation_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   216705 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/lint_and_doc_hash_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_lint_and_doc/translation_mapping_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.272927 apysc-2.8.9/apysc/_loop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/for_loop_exit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/initialize_for_loop_key_or_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_loop/loop_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.272927 apysc-2.8.9/apysc/_math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_math/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_math/max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_math/min_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_math/trunc_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.276927 apysc-2.8.9/apysc/_string/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_string/indent_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_string/string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.276927 apysc-2.8.9/apysc/_testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_testing/e2e_testing_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_testing/testing_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.276927 apysc-2.8.9/apysc/_time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/datetime_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/day_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/days_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/hour_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/left_and_right_datetimes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/millisecond_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/minute_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/month_end_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/month_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/now_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/second_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/timedelta_.py
--rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/total_seconds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/weekday_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_time/year_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.276927 apysc-2.8.9/apysc/_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.300927 apysc-2.8.9/apysc/_translation/jp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/about_handler_options_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/add_child_and_remove_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/add_debug_info_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_base_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_base_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)   143972 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_method_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_pause_and_play.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_return_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_width_and_height.py
--rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/append_js_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_append_and_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_extend_and_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_index_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_insert_and_insert_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_remove_and_remove_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/array_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assert_defined_and_undefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assert_equal_and_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assert_greater_and_greater_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assert_less_and_less_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assert_true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/assertion_basic_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/bind_and_trigger_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    47227 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/contains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/continue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_day.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_hour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_millisecond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_minute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_month.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_second.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_set_month_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/datetime_year.py
--rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/dblclick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/dictionary_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/dictionary_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/dictionary_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_object_get_and_set_css.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_object_mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_object_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_object_visible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_object_x_and_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_on_colaboratory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/display_on_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/draw_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    84469 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/easing_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/elif.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/else.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/enter_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/for.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/fundamental_data_classes_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/get_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/get_child_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_flip_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_scale_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_scale_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_base_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_begin_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_dashed_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_round_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_round_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_draw_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    62521 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_line_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/graphics_move_to_and_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/if.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/import_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19236 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/int_and_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/int_and_number_arithmetic_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/int_and_number_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/int_and_number_to_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/math_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/math_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/math_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/mouse_event_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/mouse_event_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/mousedown_and_mouseup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/mousemove.py
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/mouseover_and_mouseout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/num_children.py
--rw-r--r--   0 runner    (1001) docker     (123)    60597 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    49410 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    51647 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/recommended_type_checker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/remove_children.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17192 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/save_overall_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/sequential_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/set_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    30948 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/string_addition_and_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/string_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/string_lstrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/string_rstrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/string_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/string_strip.py
--rw-r--r--   0 runner    (1001) docker     (123)    47748 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    44504 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timedelta_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timedelta_total_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timer_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timer_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timer_repeat_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timer_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/timer_start_and_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    64293 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/unset_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/variable_name_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/what_apysc_can_do.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.300927 apysc-2.8.9/apysc/_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/_return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    45933 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/attr_linking_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/blank_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/deleted_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/dictionary_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/expression_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/hashable_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/initial_substitution_exp_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/initialize_locals_and_globals_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/number.py
--rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/number_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/py_builtin_iter_disabling_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/repr_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/revert_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/revert_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27409 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/string_lstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/string_rstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/string_split_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/string_strip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/to_fixed_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/to_string_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/type_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/type_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/value_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/variable_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/variable_name_suffix_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_type/variable_name_suffix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.304927 apysc-2.8.9/apysc/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109245 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/arg_validation_decos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/bool_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/color_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/display_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/event_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/geom_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/matrix_data_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/number_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/parent_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/path_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/validation_common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-18 06:11:28.000000 apysc-2.8.9/apysc/_validation/variable_name_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:11:54.240927 apysc-2.8.9/apysc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-18 06:11:54.000000 apysc-2.8.9/apysc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-06-18 06:11:54.000000 apysc-2.8.9/apysc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 06:11:54.000000 apysc-2.8.9/apysc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 06:11:54.000000 apysc-2.8.9/apysc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 06:11:54.000000 apysc-2.8.9/apysc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 06:11:54.304927 apysc-2.8.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.809819 apysc-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 03:39:25.000000 apysc-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 03:39:25.000000 apysc-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-25 03:39:46.809819 apysc-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-25 03:39:25.000000 apysc-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.753818 apysc-3.0.0/apysc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.757818 apysc-3.0.0/apysc/_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_cy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_finish_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_height_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_height_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_parallel_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_pause_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_play_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_reset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_reverse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_x_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_x_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_time_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_width_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_width_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/animation_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_animation/easing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.757818 apysc-3.0.0/apysc/_auto_reloading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_auto_reloading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_auto_reloading/auto_reloading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.757818 apysc-3.0.0/apysc/_branch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_branch/_elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_branch/_else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_branch/_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_branch/if_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.757818 apysc-3.0.0/apysc/_callable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_callable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_callable/callable_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.761818 apysc-3.0.0/apysc/_chart/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/add_background_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/add_border_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_label_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_label_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_label_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_label_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_label_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_label_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/axis_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/background_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/border_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/chart_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/chart_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/create_single_column_y_axis_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/initialize_each_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/is_display_axis_label_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/overall_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_background_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_background_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_border_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_border_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_border_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_horizontal_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_matrix_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_vertical_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/set_initial_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/tick_max_num_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/tick_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/tick_text_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/tick_text_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/tick_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/tick_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/tick_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/vertical_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/x_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/x_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/x_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/x_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/x_axis_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/y_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/y_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/y_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/y_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/y_axis_single_column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/y_max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_chart/y_min_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.761818 apysc-3.0.0/apysc/_color/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_color/color_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.761818 apysc-3.0.0/apysc/_console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_console/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31274 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_console/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_console/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.761818 apysc-3.0.0/apysc/_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_converter/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_converter/to_apysc_val_from_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_converter/to_builtin_val_from_apysc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.773818 apysc-3.0.0/apysc/_display/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/any_display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_fill_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_fill_color_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_line_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_line_cap_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_line_color_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_line_joints_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_line_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_line_thickness_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_x_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/append_y_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/begin_fill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/css_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/ellipse_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/ellipse_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/flip_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/flip_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/flip_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/get_bounds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48598 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/graphics_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/graphics_clear_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/graphics_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_cap_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_caps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_dash_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_dash_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_joints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_joints_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_round_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_style_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/points_2d_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/points_var_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_append_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_apply_current_points_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_x3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polygon_y3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/rotation_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/scale_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/set_lower_scale_limit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/set_overflow_visible_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/skew_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/skew_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_font_size_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_set_text_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_singleton_for_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/svg_text_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/visible_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/width_and_height_mixin_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/x_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/y_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_display/y_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.777818 apysc-3.0.0/apysc/_event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/custom_event_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/custom_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/document_mouse_wheel_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/double_click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/enter_frame_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/enter_frame_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/handler_circular_calling_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_down_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_event_binding_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_event_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_event_unbinding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_out_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_over_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/mouse_up_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/prevent_default_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/set_handler_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/stop_propagation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_event/wheel_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.777818 apysc-3.0.0/apysc/_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/event_handler_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/expression_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/expression_variables_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/get_last_scope_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/indent_num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/js_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/last_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_expression/var_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.777818 apysc-3.0.0/apysc/_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_file/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_file/module_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.781818 apysc-3.0.0/apysc/_geom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_control_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_control_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_control_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_control_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_control_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_control_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_dest_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_dest_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/path_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_bottom_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_center_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_center_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_left_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_right_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_top_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/rectangle_geom_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_geom/relative_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.781818 apysc-3.0.0/apysc/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_html/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_html/html_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_html/html_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.781818 apysc-3.0.0/apysc/_jslib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jslib/jquery-3.6.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jslib/jslib_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jslib/svg-3.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jslib/underscore-1.12.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.781818 apysc-3.0.0/apysc/_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_jupyter/jupyter_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.781818 apysc-3.0.0/apysc/_lint_and_doc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/conf_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/docs_keyword_link_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/docs_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/docs_toctree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/docs_translation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/docstring_to_markdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/docstring_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/document_text_split_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/document_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.781818 apysc-3.0.0/apysc/_lint_and_doc/fixed_translation_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   218414 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/lint_and_doc_hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_lint_and_doc/translation_mapping_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.785818 apysc-3.0.0/apysc/_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/for_loop_exit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/initialize_for_loop_key_or_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_loop/loop_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.785818 apysc-3.0.0/apysc/_math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_math/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_math/max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_math/min_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_math/trunc_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.785818 apysc-3.0.0/apysc/_string/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_string/indent_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_string/string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.785818 apysc-3.0.0/apysc/_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_testing/e2e_testing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_testing/testing_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.785818 apysc-3.0.0/apysc/_time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/datetime_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/day_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/days_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/hour_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/left_and_right_datetimes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/millisecond_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/minute_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/month_end_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/month_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/now_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/second_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/timedelta_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/total_seconds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/weekday_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_time/year_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.785818 apysc-3.0.0/apysc/_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.805818 apysc-3.0.0/apysc/_translation/jp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/about_handler_options_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/add_child_and_remove_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/add_debug_info_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_base_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_base_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143972 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_method_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_pause_and_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_width_and_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/append_js_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_append_and_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_extend_and_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_index_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_insert_and_insert_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_remove_and_remove_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/array_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assert_defined_and_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assert_equal_and_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assert_greater_and_greater_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assert_less_and_less_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assert_true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/assertion_basic_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/bind_and_trigger_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47227 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/contains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_hour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_millisecond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_minute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_set_month_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/datetime_year.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/dblclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/dictionary_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/dictionary_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/dictionary_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_object_get_and_set_css.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_object_mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_object_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_object_visible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_object_x_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_on_colaboratory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/display_on_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/draw_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84469 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/easing_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/enter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/fundamental_data_classes_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/get_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/get_child_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_flip_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_scale_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_scale_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_base_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_begin_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_dashed_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_round_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_round_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_draw_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62521 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_line_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/graphics_move_to_and_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/import_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/int_and_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/int_and_number_arithmetic_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/int_and_number_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/int_and_number_to_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/math_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/math_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/math_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/mouse_event_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/mouse_event_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/mousedown_and_mouseup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/mousemove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/mouseover_and_mouseout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/num_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60597 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49410 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51647 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/recommended_type_checker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/remove_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17192 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/save_overall_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/sequential_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/set_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30948 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/string_addition_and_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/string_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/string_lstrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/string_rstrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/string_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/string_strip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47748 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44504 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timedelta_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timedelta_total_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timer_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timer_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timer_repeat_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timer_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/timer_start_and_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64293 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/unset_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/variable_name_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/what_apysc_can_do.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.809819 apysc-3.0.0/apysc/_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45933 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/attr_linking_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/blank_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/deleted_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/dictionary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/expression_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/hashable_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/initial_substitution_exp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/initialize_locals_and_globals_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/number_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/py_builtin_iter_disabling_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/repr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/revert_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/revert_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/string_lstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/string_rstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/string_split_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/string_strip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/to_fixed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/to_number_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/to_string_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/type_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/value_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/variable_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/variable_name_suffix_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_type/variable_name_suffix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.809819 apysc-3.0.0/apysc/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109245 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/arg_validation_decos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/bool_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/color_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/display_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/event_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/geom_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/matrix_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/number_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/parent_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/path_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/validation_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-25 03:39:25.000000 apysc-3.0.0/apysc/_validation/variable_name_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:39:46.753818 apysc-3.0.0/apysc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-25 03:39:46.000000 apysc-3.0.0/apysc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25885 2023-06-25 03:39:46.000000 apysc-3.0.0/apysc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 03:39:46.000000 apysc-3.0.0/apysc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 03:39:46.000000 apysc-3.0.0/apysc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 03:39:46.000000 apysc-3.0.0/apysc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 03:39:46.809819 apysc-3.0.0/setup.cfg
```

### Comparing `apysc-2.8.9/LICENSE` & `apysc-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/PKG-INFO` & `apysc-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 2.8.9
+Version: 3.0.0
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-2.8.9/README.md` & `apysc-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ## Supported Python Version
 
 Python 3.7 or later.
 
 ## Installing
 
-pip command is available:
+Pip command is available:
 
 ```
 $ pip install apysc
 ```
 
 ## What's new
 
@@ -41,15 +41,15 @@
 
 Please see [apysc documentation](https://simon-ritchie.github.io/apysc/en/index.html) and [quick start guide](https://simon-ritchie.github.io/apysc/en/quick_start.html) page.
 
 <a href="https://simon-ritchie.github.io/apysc/en/index.html"><img src="https://github.com/simon-ritchie/apysc/blob/main/assets/document_index_screenshot.png"></a>
 
 ## What apysc can do in its current implementation
 
-- **Save HTML or use it on the Jupyter notebook, JupyterLab, and Google Colaboratory!**
+- **Save HTML or use it on the Jupyter Notebook, JupyterLab, and Google Colaboratory!**
 
 ![](https://github.com/simon-ritchie/apysc/blob/main/assets/jupyterlab_interface.png)
 
 Documents:
 
 - [save_overall_html interface](https://simon-ritchie.github.io/apysc/en/save_overall_html.html)
 - [display_on_jupyter interface](https://simon-ritchie.github.io/apysc/en/display_on_jupyter.html)
@@ -149,27 +149,31 @@
 - **Basic control, like the for loop, if branch instruction, and so on**
 
 Documents:
 
 - [If](https://simon-ritchie.github.io/apysc/en/if.html)
 - [Elif](https://simon-ritchie.github.io/apysc/en/elif.html)
 - [Else](https://simon-ritchie.github.io/apysc/en/else.html)
-- [For](https://simon-ritchie.github.io/apysc/en/for.html)
+- [ForArrayIndices](https://simon-ritchie.github.io/apysc/en/for_array_indices.html)
+- [ForArrayValues](https://simon-ritchie.github.io/apysc/en/for_array_values.html)
+- [ForDictKeys](https://simon-ritchie.github.io/apysc/en/for_dict_keys.html)
+- [ForDictValues](https://simon-ritchie.github.io/apysc/en/for_dict_values.html)
+- [ForDictKeysAndValues](https://simon-ritchie.github.io/apysc/en/for_dict_keys_and_values.html)
 
 ---
 
 For more details, please see the following document:
 
 [What apysc can do in its current implementation](https://simon-ritchie.github.io/apysc/en/what_apysc_can_do.html)
 
 ## License
 
 The apysc library is under the MIT License.
 
-The logo image is using followed Creative Commons license font:
+The logo image uses the following Creative Commons license font:
 
 - [Pauline Font - by Marcos Boric (2020)](https://www.behance.net/gallery/94972757/Pauline-Font)
 - [Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.en)
 
 Also, the apysc library depends on the following libraries:
 
 - [jQuery, MIT License](https://github.com/jquery/jquery/blob/main/LICENSE.txt)
```

#### html2text {}

```diff
@@ -14,25 +14,25 @@
 byob.yarr.is/simon-ritchie/apysc/passing_doctests_num) ![](https://
 byob.yarr.is/simon-ritchie/apysc/passing_lints) ![logo](https://github.com/
 simon-ritchie/apysc/blob/main/assets/logo_v1/logo_small_v1.png) Language: |
 English | [æ¥æ¬èª (Japanese)](https://github.com/simon-ritchie/apysc/blob/
 main/README_JP.md) | apysc (pronounced `Ã¦pisk`) is a Python frontend library
 to create HTML and js files with ActionScript 3 (as3)-like interface. Notes:
 Currently developing and only works partially. ## Supported Python Version
-Python 3.7 or later. ## Installing pip command is available: ``` $ pip install
+Python 3.7 or later. ## Installing Pip command is available: ``` $ pip install
 apysc ``` ## What's new To check the major features updating and destructive
 changes, please see the Discussions' [Announcements](https://github.com/simon-
 ritchie/apysc/discussions/categories/announcements) and [Destructive changes]
 (https://github.com/simon-ritchie/apysc/discussions/categories/destructive-
 changes). ## How to start Please see [apysc documentation](https://simon-
 ritchie.github.io/apysc/en/index.html) and [quick start guide](https://simon-
 ritchie.github.io/apysc/en/quick_start.html) page. [https://github.com/simon-
 ritchie/apysc/blob/main/assets/document_index_screenshot.png] ## What apysc can
 do in its current implementation - **Save HTML or use it on the Jupyter
-notebook, JupyterLab, and Google Colaboratory!** ![](https://github.com/simon-
+Notebook, JupyterLab, and Google Colaboratory!** ![](https://github.com/simon-
 ritchie/apysc/blob/main/assets/jupyterlab_interface.png) Documents: -
 [save_overall_html interface](https://simon-ritchie.github.io/apysc/en/
 save_overall_html.html) - [display_on_jupyter interface](https://simon-
 ritchie.github.io/apysc/en/display_on_jupyter.html) - [display_on_colaboratory
 interface](https://simon-ritchie.github.io/apysc/en/
 display_on_colaboratory.html) --- - **Draw the many types of vector graphics**
 ![](https://github.com/simon-ritchie/apysc/blob/main/assets/
@@ -63,21 +63,26 @@
 fragments: ```py ... rectangle.animation_x( x=100, duration=1000,
 easing=ap.Easing.EASE_IN_QUART, ).start() ... ``` Abstract document: [Animation
 interfaces abstract (each animation attribute)](https://simon-
 ritchie.github.io/apysc/en/animation_interfaces_abstract.html) --- - **Basic
 control, like the for loop, if branch instruction, and so on** Documents: -
 [If](https://simon-ritchie.github.io/apysc/en/if.html) - [Elif](https://simon-
 ritchie.github.io/apysc/en/elif.html) - [Else](https://simon-ritchie.github.io/
-apysc/en/else.html) - [For](https://simon-ritchie.github.io/apysc/en/for.html)
---- For more details, please see the following document: [What apysc can do in
+apysc/en/else.html) - [ForArrayIndices](https://simon-ritchie.github.io/apysc/
+en/for_array_indices.html) - [ForArrayValues](https://simon-ritchie.github.io/
+apysc/en/for_array_values.html) - [ForDictKeys](https://simon-
+ritchie.github.io/apysc/en/for_dict_keys.html) - [ForDictValues](https://simon-
+ritchie.github.io/apysc/en/for_dict_values.html) - [ForDictKeysAndValues]
+(https://simon-ritchie.github.io/apysc/en/for_dict_keys_and_values.html) --
+- For more details, please see the following document: [What apysc can do in
 its current implementation](https://simon-ritchie.github.io/apysc/en/
 what_apysc_can_do.html) ## License The apysc library is under the MIT License.
-The logo image is using followed Creative Commons license font: - [Pauline Font
-- by Marcos Boric (2020)](https://www.behance.net/gallery/94972757/Pauline-
-Font) - [Attribution 4.0 International (CC BY 4.0)](https://
+The logo image uses the following Creative Commons license font: - [Pauline
+Font - by Marcos Boric (2020)](https://www.behance.net/gallery/94972757/
+Pauline-Font) - [Attribution 4.0 International (CC BY 4.0)](https://
 creativecommons.org/licenses/by/4.0/deed.en) Also, the apysc library depends on
 the following libraries: - [jQuery, MIT License](https://github.com/jquery/
 jquery/blob/main/LICENSE.txt) - [jQuery Mousewheel](https://github.com/jquery/
 jquery-mousewheel/blob/main/LICENSE.txt) - [SVG.js, MIT License](https://
 github.com/svgdotjs/svg.js/blob/master/LICENSE.txt) - [Underscore.js, MIT
 License](https://github.com/jashkenas/underscore/blob/master/LICENSE) - [Static
 Typing for Python (Python official backport package)](https://github.com/
```

### Comparing `apysc-2.8.9/apysc/__init__.py` & `apysc-3.0.0/apysc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 from apysc._type.string import String as Str
 from apysc._type.array import Array
 from apysc._type.dictionary import Dictionary
 from apysc._type.any_value import AnyValue
 from apysc._branch._if import If
 from apysc._branch._elif import Elif
 from apysc._branch._else import Else
-from apysc._loop._for import For
 from apysc._loop.for_array_indices import ForArrayIndices
 from apysc._loop.for_array_values import ForArrayValues
 from apysc._loop.for_array_indices_and_values import ForArrayIndicesAndValues
 from apysc._loop.for_dict_keys import ForDictKeys
+from apysc._loop.for_dict_values import ForDictValues
+from apysc._loop.for_dict_keys_and_values import ForDictKeysAndValues
 from apysc._loop._continue import Continue
 from apysc._loop._range import range
 from apysc._display.display_object import DisplayObject
 from apysc._display._document import document
 from apysc._display.sprite import Sprite
 from apysc._display.graphics import Graphics
 from apysc._display.stage import Stage
@@ -126,8 +127,8 @@
 from apysc._math.math import Math
 from apysc._auto_reloading.auto_reloading_decorator import set_auto_reloading
 from apysc._chart.x_axis_settings import XAxisSettings
 from apysc._chart.y_axis_single_column_settings import YAxisSingleColumnSettings
 from apysc._chart.x_axis_label_position import XAxisLabelPosition
 from apysc._chart.y_axis_label_position import YAxisLabelPosition
 
-__version__: str = "2.8.9"
+__version__: str = "3.0.0"
```

### Comparing `apysc-2.8.9/apysc/_animation/animation_base.py` & `apysc-3.0.0/apysc/_animation/animation_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_cx.py` & `apysc-3.0.0/apysc/_animation/animation_cx.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_cx_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_cy.py` & `apysc-3.0.0/apysc/_animation/animation_cy.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_cy_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_fill_alpha.py` & `apysc-3.0.0/apysc/_animation/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_fill_alpha_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_fill_color.py` & `apysc-3.0.0/apysc/_animation/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_fill_color_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_finish_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_finish_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_height.py` & `apysc-3.0.0/apysc/_animation/animation_height.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_height_for_ellipse.py` & `apysc-3.0.0/apysc/_animation/animation_height_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_height_for_ellipse_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_height_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_height_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_line_alpha.py` & `apysc-3.0.0/apysc/_animation/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_line_alpha_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_line_color.py` & `apysc-3.0.0/apysc/_animation/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_line_color_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_line_thickness.py` & `apysc-3.0.0/apysc/_animation/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_line_thickness_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_mixins.py` & `apysc-3.0.0/apysc/_animation/animation_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_move.py` & `apysc-3.0.0/apysc/_animation/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_move_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_parallel.py` & `apysc-3.0.0/apysc/_animation/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_parallel_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_parallel_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_pause_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_pause_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_play_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_play_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_radius.py` & `apysc-3.0.0/apysc/_animation/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_radius_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_reset_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_reset_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_reverse_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_reverse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_rotation_around_center.py` & `apysc-3.0.0/apysc/_animation/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_rotation_around_center_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_rotation_around_point.py` & `apysc-3.0.0/apysc/_animation/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_rotation_around_point_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_x_from_center.py` & `apysc-3.0.0/apysc/_animation/animation_scale_x_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_x_from_center_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_x_from_point.py` & `apysc-3.0.0/apysc/_animation/animation_scale_x_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_x_from_point_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_y_from_center.py` & `apysc-3.0.0/apysc/_animation/animation_scale_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_y_from_center_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_y_from_point.py` & `apysc-3.0.0/apysc/_animation/animation_scale_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_scale_y_from_point_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_time_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_time_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_width.py` & `apysc-3.0.0/apysc/_animation/animation_width.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_width_for_ellipse.py` & `apysc-3.0.0/apysc/_animation/animation_width_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_width_for_ellipse_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_width_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_width_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_x.py` & `apysc-3.0.0/apysc/_animation/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_x_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_y.py` & `apysc-3.0.0/apysc/_animation/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/animation_y_mixin.py` & `apysc-3.0.0/apysc/_animation/animation_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_animation/easing.py` & `apysc-3.0.0/apysc/_animation/easing.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_auto_reloading/auto_reloading_decorator.py` & `apysc-3.0.0/apysc/_auto_reloading/auto_reloading_decorator.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_branch/_elif.py` & `apysc-3.0.0/apysc/_branch/_elif.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_branch/_else.py` & `apysc-3.0.0/apysc/_branch/_else.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_branch/_if.py` & `apysc-3.0.0/apysc/_branch/_if.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_branch/if_base.py` & `apysc-3.0.0/apysc/_branch/if_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_callable/callable_util.py` & `apysc-3.0.0/apysc/_callable/callable_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/add_background_mixin.py` & `apysc-3.0.0/apysc/_chart/add_background_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/add_border_mixin.py` & `apysc-3.0.0/apysc/_chart/add_border_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_label_bold_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_label_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_label_fill_alpha_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_label_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_label_fill_color_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_label_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_label_font_family_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_label_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_label_font_size_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_label_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_label_italic_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_label_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_line_alpha_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_line_color_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/axis_line_thickness_mixin.py` & `apysc-3.0.0/apysc/_chart/axis_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/background_container_mixin.py` & `apysc-3.0.0/apysc/_chart/background_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/border_container_mixin.py` & `apysc-3.0.0/apysc/_chart/border_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/chart_container_mixin.py` & `apysc-3.0.0/apysc/_chart/chart_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/create_single_column_y_axis_mixin.py` & `apysc-3.0.0/apysc/_chart/create_single_column_y_axis_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,15 @@
 
     diff: Number = y_axis_max - y_axis_min
     interval: Number = diff / (ticks_num - 1)
     y_axis_text_values: Array[String] = Array(
         [], variable_name_suffix=variable_name_suffix
     )
     range_arr: Array[Int] = ap.range(ticks_num)
-    i: Int
-    with ap.For(range_arr) as i:
+    with ap.ForArrayIndices(arr=range_arr) as i:
         tick_value: Union[Int, Number] = y_axis_min + i * interval
         value_text: String = cast(Union[Int, Number], tick_value).to_string()
         y_axis_text_values.append(value_text)
     return y_axis_text_values
 
 
 def _calculate_y_axis_min(
@@ -276,15 +275,15 @@
     -------
     y_axis_ticks_texts : Array[SVGText]
         Created y-axis ticks texts.
     """
     import apysc as ap
 
     y_axis_ticks_texts: Array[SVGText] = Array([])
-    with ap.For(y_axis_ticks_y_coordinates) as i:
+    with ap.ForArrayIndices(arr=y_axis_ticks_y_coordinates) as i:
         y_coordinate: Number = y_axis_ticks_y_coordinates[i]
         data_dict: Dictionary[str, Union[Int, Number, String]] = data[i]
         text_value: String = _extract_text_value_from_data_dict(
             data_dict=data_dict,
             y_axis_column_name=y_axis_column_name,
         )
         txt: SVGText = ap.SVGText(
@@ -328,24 +327,23 @@
     variable_name_suffix : str
         A JavaScript variable name suffix string.
         This setting is sometimes useful for JavaScript debugging.
     """
     import apysc as ap
 
     x: Number = horizontal_padding._copy()
-    i: Int
-    with ap.For(y_axis_ticks_texts) as i:
+    with ap.ForArrayIndices(arr=y_axis_ticks_texts) as i:
         txt: ap.SVGText = y_axis_ticks_texts[i]
         bounding_box: ap.RectangleGeom = txt.get_bounds()
         max_arr: ap.Array[Union[Int, Number]] = ap.Array(
             [x, bounding_box.width + horizontal_padding],
             variable_name_suffix=variable_name_suffix,
         )
         x = ap.Math.max(max_arr)
-    with ap.For(y_axis_ticks_texts) as i:
+    with ap.ForArrayIndices(arr=y_axis_ticks_texts) as i:
         txt = y_axis_ticks_texts[i]
         txt.x = x
 
 
 def _extract_text_value_from_data_dict(
     *,
     data_dict: Dictionary[str, Union[Int, Number, String]],
@@ -413,17 +411,16 @@
         [], variable_name_suffix=variable_name_suffix
     )
     y_start_coordinate: Int = Int(
         vertical_padding,
         variable_name_suffix=variable_name_suffix,
     )
     range_arr: Array[Int] = ap.range(y_axis_ticks_num)
-    i: Int
     interval: Number = y_axis_height / (y_axis_ticks_num - 1)
-    with ap.For(range_arr) as i:
+    with ap.ForArrayIndices(range_arr) as i:
         y_coordinate: Number = interval * i + y_start_coordinate
         y_axis_ticks_y_coordinates.append(y_coordinate)
     y_axis_ticks_y_coordinates.reverse()
     return y_axis_ticks_y_coordinates
 
 
 def _calculate_y_axis_ticks_num(
@@ -610,14 +607,13 @@
         A values array.
     """
     import apysc as ap
 
     values: Array[Union[Int, Number]] = Array(
         [], variable_name_suffix=variable_name_suffix
     )
-    i: Int
-    with ap.For(data) as i:
+    with ap.ForArrayIndices(data) as i:
         dict_value: Dictionary[str, Union[Int, Number]] = cast(
             Dictionary[str, Union[Int, Number]], data[i]
         )
         values.append(dict_value[column_name])
     return values
```

### Comparing `apysc-2.8.9/apysc/_chart/initialize_each_container_mixin.py` & `apysc-3.0.0/apysc/_chart/initialize_each_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/is_display_axis_label_mixin.py` & `apysc-3.0.0/apysc/_chart/is_display_axis_label_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/overall_container_mixin.py` & `apysc-3.0.0/apysc/_chart/overall_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_background_fill_alpha_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_background_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_background_fill_color_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_background_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_border_alpha_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_border_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_border_color_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_border_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_border_thickness_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_border_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_height_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_horizontal_padding_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_horizontal_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_matrix_data_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_matrix_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_overall_container_coordinates_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_overall_container_coordinates_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_vertical_padding_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_vertical_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_width_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_x_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/set_initial_y_mixin.py` & `apysc-3.0.0/apysc/_chart/set_initial_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/tick_max_num_mixin.py` & `apysc-3.0.0/apysc/_chart/tick_max_num_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/tick_text_bold_mixin.py` & `apysc-3.0.0/apysc/_chart/tick_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/tick_text_fill_alpha_mixin.py` & `apysc-3.0.0/apysc/_chart/tick_text_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/tick_text_fill_color_mixin.py` & `apysc-3.0.0/apysc/_chart/tick_text_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/tick_text_font_family_mixin.py` & `apysc-3.0.0/apysc/_chart/tick_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/tick_text_font_size_mixin.py` & `apysc-3.0.0/apysc/_chart/tick_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/tick_text_italic_mixin.py` & `apysc-3.0.0/apysc/_chart/tick_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/vertical_bar_chart.py` & `apysc-3.0.0/apysc/_chart/vertical_bar_chart.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/x_axis_column_name_mixin.py` & `apysc-3.0.0/apysc/_chart/x_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/x_axis_container_mixin.py` & `apysc-3.0.0/apysc/_chart/x_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/x_axis_label_position_mixin.py` & `apysc-3.0.0/apysc/_chart/x_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/x_axis_settings.py` & `apysc-3.0.0/apysc/_chart/x_axis_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/y_axis_column_name_mixin.py` & `apysc-3.0.0/apysc/_chart/y_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/y_axis_container_mixin.py` & `apysc-3.0.0/apysc/_chart/y_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/y_axis_label_position_mixin.py` & `apysc-3.0.0/apysc/_chart/y_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/y_axis_single_column_settings.py` & `apysc-3.0.0/apysc/_chart/y_axis_single_column_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/y_max_mixin.py` & `apysc-3.0.0/apysc/_chart/y_max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_chart/y_min_mixin.py` & `apysc-3.0.0/apysc/_chart/y_min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_color/color_util.py` & `apysc-3.0.0/apysc/_color/color_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_console/_trace.py` & `apysc-3.0.0/apysc/_console/_trace.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_console/assertion.py` & `apysc-3.0.0/apysc/_console/assertion.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_console/loggers.py` & `apysc-3.0.0/apysc/_console/loggers.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_converter/cast.py` & `apysc-3.0.0/apysc/_converter/cast.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_converter/to_apysc_val_from_builtin.py` & `apysc-3.0.0/apysc/_converter/to_apysc_val_from_builtin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_converter/to_builtin_val_from_apysc.py` & `apysc-3.0.0/apysc/_converter/to_builtin_val_from_apysc.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/_document.py` & `apysc-3.0.0/apysc/_display/_document.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/any_display_object.py` & `apysc-3.0.0/apysc/_display/any_display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_fill_alpha_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_fill_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_fill_color_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_fill_color_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_line_alpha_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_line_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_line_cap_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_line_cap_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_line_color_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_line_color_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_line_joints_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_line_joints_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_line_point_mixin.py` & `apysc-3.0.0/apysc/_display/append_line_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_line_thickness_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_line_thickness_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_x_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_x_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/append_y_attr_expression_mixin.py` & `apysc-3.0.0/apysc/_display/append_y_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/begin_fill_mixin.py` & `apysc-3.0.0/apysc/_display/begin_fill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/child_mixin.py` & `apysc-3.0.0/apysc/_display/child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/circle.py` & `apysc-3.0.0/apysc/_display/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/css_interface.py` & `apysc-3.0.0/apysc/_display/css_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/css_mixin.py` & `apysc-3.0.0/apysc/_display/css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/cx_mixin.py` & `apysc-3.0.0/apysc/_display/cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/cy_mixin.py` & `apysc-3.0.0/apysc/_display/cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/display_object.py` & `apysc-3.0.0/apysc/_display/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/ellipse.py` & `apysc-3.0.0/apysc/_display/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/ellipse_height_mixin.py` & `apysc-3.0.0/apysc/_display/ellipse_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/ellipse_width_mixin.py` & `apysc-3.0.0/apysc/_display/ellipse_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/fill_alpha_mixin.py` & `apysc-3.0.0/apysc/_display/fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/fill_color_mixin.py` & `apysc-3.0.0/apysc/_display/fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/flip_interface_helper.py` & `apysc-3.0.0/apysc/_display/flip_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/flip_x_mixin.py` & `apysc-3.0.0/apysc/_display/flip_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/flip_y_mixin.py` & `apysc-3.0.0/apysc/_display/flip_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/get_bounds_mixin.py` & `apysc-3.0.0/apysc/_display/get_bounds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/graphics.py` & `apysc-3.0.0/apysc/_display/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/graphics_base.py` & `apysc-3.0.0/apysc/_display/graphics_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/graphics_clear_mixin.py` & `apysc-3.0.0/apysc/_display/graphics_clear_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/graphics_expression.py` & `apysc-3.0.0/apysc/_display/graphics_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/height_mixin.py` & `apysc-3.0.0/apysc/_display/height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line.py` & `apysc-3.0.0/apysc/_display/line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_alpha_mixin.py` & `apysc-3.0.0/apysc/_display/line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_cap_mixin.py` & `apysc-3.0.0/apysc/_display/line_cap_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_caps.py` & `apysc-3.0.0/apysc/_display/line_caps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_color_mixin.py` & `apysc-3.0.0/apysc/_display/line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_dash_dot_setting.py` & `apysc-3.0.0/apysc/_display/line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_dash_dot_setting_mixin.py` & `apysc-3.0.0/apysc/_display/line_dash_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_dash_setting.py` & `apysc-3.0.0/apysc/_display/line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_dash_setting_mixin.py` & `apysc-3.0.0/apysc/_display/line_dash_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_dot_setting.py` & `apysc-3.0.0/apysc/_display/line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_dot_setting_mixin.py` & `apysc-3.0.0/apysc/_display/line_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_joints.py` & `apysc-3.0.0/apysc/_display/line_joints.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_joints_mixin.py` & `apysc-3.0.0/apysc/_display/line_joints_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_round_dot_setting.py` & `apysc-3.0.0/apysc/_display/line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_round_dot_setting_mixin.py` & `apysc-3.0.0/apysc/_display/line_round_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_style_mixin.py` & `apysc-3.0.0/apysc/_display/line_style_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/line_thickness_mixin.py` & `apysc-3.0.0/apysc/_display/line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/parent_mixin.py` & `apysc-3.0.0/apysc/_display/parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/path.py` & `apysc-3.0.0/apysc/_display/path.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/points_2d_mixin.py` & `apysc-3.0.0/apysc/_display/points_2d_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon.py` & `apysc-3.0.0/apysc/_display/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_append_constructor_expression_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_append_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_apply_current_points_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_apply_current_points_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_x1_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_x2_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_x3_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_x3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_y1_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_y2_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polygon_y3_mixin.py` & `apysc-3.0.0/apysc/_display/polygon_y3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/polyline.py` & `apysc-3.0.0/apysc/_display/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/radius_mixin.py` & `apysc-3.0.0/apysc/_display/radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/rectangle.py` & `apysc-3.0.0/apysc/_display/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/rotation_around_center_mixin.py` & `apysc-3.0.0/apysc/_display/rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/rotation_around_point_mixin.py` & `apysc-3.0.0/apysc/_display/rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/rotation_interface_helper.py` & `apysc-3.0.0/apysc/_display/rotation_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/scale_interface_helper.py` & `apysc-3.0.0/apysc/_display/scale_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/scale_x_from_center_mixin.py` & `apysc-3.0.0/apysc/_display/scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/scale_x_from_point_mixin.py` & `apysc-3.0.0/apysc/_display/scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/scale_y_from_center_mixin.py` & `apysc-3.0.0/apysc/_display/scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/scale_y_from_point_mixin.py` & `apysc-3.0.0/apysc/_display/scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/set_lower_scale_limit_mixin.py` & `apysc-3.0.0/apysc/_display/set_lower_scale_limit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/set_overflow_visible_setting_mixin.py` & `apysc-3.0.0/apysc/_display/set_overflow_visible_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/skew_x_mixin.py` & `apysc-3.0.0/apysc/_display/skew_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/skew_y_mixin.py` & `apysc-3.0.0/apysc/_display/skew_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/sprite.py` & `apysc-3.0.0/apysc/_display/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/stage.py` & `apysc-3.0.0/apysc/_display/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text.py` & `apysc-3.0.0/apysc/_display/svg_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,15 +515,19 @@
             parent=parent,
             variable_name_suffix=variable_name_suffix,
         )
         text_spans_: Array[SVGTextSpan] = svg_text._convert_text_spans_list_to_array(
             text_spans=text_spans
         )
         i: Int
-        with ap.For(arr_or_dict=text_spans_, locals_=locals(), globals_=globals()) as i:
+        with ap.ForArrayIndices(
+            arr=text_spans_,
+            locals_=locals(),
+            globals_=globals(),
+        ) as i:
             text_span: SVGTextSpan = text_spans_[i]
             expression: str = (
                 f"{svg_text.variable_name}.add({text_span.variable_name});"
             )
             ap.append_js_expression(expression=expression)
         return svg_text
```

### Comparing `apysc-2.8.9/apysc/_display/svg_text_align_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_bold_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_delta_x_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_delta_y_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_font_family_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_font_size_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_italic_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_leading_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_align_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_bold_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_delta_x_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_delta_y_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_font_family_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_font_size_value_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_font_size_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_italic_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_leading_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_set_text_value_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_set_text_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_singleton_for_text_span.py` & `apysc-3.0.0/apysc/_display/svg_text_singleton_for_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_span.py` & `apysc-3.0.0/apysc/_display/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/svg_text_text_mixin.py` & `apysc-3.0.0/apysc/_display/svg_text_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/triangle.py` & `apysc-3.0.0/apysc/_display/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/visible_mixin.py` & `apysc-3.0.0/apysc/_display/visible_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/width_and_height_mixin_for_ellipse.py` & `apysc-3.0.0/apysc/_display/width_and_height_mixin_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/width_mixin.py` & `apysc-3.0.0/apysc/_display/width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/x_interface.py` & `apysc-3.0.0/apysc/_display/x_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/x_mixin.py` & `apysc-3.0.0/apysc/_display/x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/y_interface.py` & `apysc-3.0.0/apysc/_display/y_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_display/y_mixin.py` & `apysc-3.0.0/apysc/_display/y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/animation_event.py` & `apysc-3.0.0/apysc/_event/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/click_mixin.py` & `apysc-3.0.0/apysc/_event/click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/custom_event_mixin.py` & `apysc-3.0.0/apysc/_event/custom_event_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/document_mouse_wheel_func.py` & `apysc-3.0.0/apysc/_event/document_mouse_wheel_func.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/double_click_mixin.py` & `apysc-3.0.0/apysc/_event/double_click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/enter_frame_event.py` & `apysc-3.0.0/apysc/_event/enter_frame_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/enter_frame_mixin.py` & `apysc-3.0.0/apysc/_event/enter_frame_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/event.py` & `apysc-3.0.0/apysc/_event/event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/handler.py` & `apysc-3.0.0/apysc/_event/handler.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/handler_circular_calling_util.py` & `apysc-3.0.0/apysc/_event/handler_circular_calling_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_down_mixin.py` & `apysc-3.0.0/apysc/_event/mouse_down_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_event.py` & `apysc-3.0.0/apysc/_event/mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_event_binding_expression_mixin.py` & `apysc-3.0.0/apysc/_event/mouse_event_binding_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_event_mixins.py` & `apysc-3.0.0/apysc/_event/mouse_event_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_event_unbinding_mixin.py` & `apysc-3.0.0/apysc/_event/mouse_event_unbinding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_move_mixin.py` & `apysc-3.0.0/apysc/_event/mouse_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_out_mixin.py` & `apysc-3.0.0/apysc/_event/mouse_out_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_over_mixin.py` & `apysc-3.0.0/apysc/_event/mouse_over_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/mouse_up_mixin.py` & `apysc-3.0.0/apysc/_event/mouse_up_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/prevent_default_mixin.py` & `apysc-3.0.0/apysc/_event/prevent_default_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/set_handler_data_mixin.py` & `apysc-3.0.0/apysc/_event/set_handler_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/stop_propagation_mixin.py` & `apysc-3.0.0/apysc/_event/stop_propagation_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/timer_event.py` & `apysc-3.0.0/apysc/_event/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_event/wheel_event.py` & `apysc-3.0.0/apysc/_event/wheel_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_expression/event_handler_scope.py` & `apysc-3.0.0/apysc/_expression/event_handler_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_expression/expression_data_util.py` & `apysc-3.0.0/apysc/_expression/expression_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_expression/expression_variables_util.py` & `apysc-3.0.0/apysc/_expression/expression_variables_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_expression/indent_num.py` & `apysc-3.0.0/apysc/_expression/indent_num.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_expression/js_functions.py` & `apysc-3.0.0/apysc/_expression/js_functions.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_expression/last_scope.py` & `apysc-3.0.0/apysc/_expression/last_scope.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     ELSE = 4
     FOR = 5
     EVENT_HANDLER = 6
     FOR_ARRAY_INDICES = 7
     FOR_ARRAY_VALUES = 8
     FOR_ARRAY_INDICES_AND_VALUES = 9
     FOR_DICT_KEYS = 10
+    FOR_DICT_VALUES = 11
+    FOR_DICT_KEYS_AND_VALUES = 12
 
 
 def reset() -> None:
     """
     Reset last expression's scope information.
     """
     from apysc._expression import expression_data_util
```

### Comparing `apysc-2.8.9/apysc/_expression/var_names.py` & `apysc-3.0.0/apysc/_expression/var_names.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_file/file_util.py` & `apysc-3.0.0/apysc/_file/file_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_file/module_util.py` & `apysc-3.0.0/apysc/_file/module_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_bezier_2d.py` & `apysc-3.0.0/apysc/_geom/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_bezier_2d_continual.py` & `apysc-3.0.0/apysc/_geom/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_bezier_3d.py` & `apysc-3.0.0/apysc/_geom/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_bezier_3d_continual.py` & `apysc-3.0.0/apysc/_geom/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_close.py` & `apysc-3.0.0/apysc/_geom/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_control_x1_mixin.py` & `apysc-3.0.0/apysc/_geom/path_control_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_control_x2_mixin.py` & `apysc-3.0.0/apysc/_geom/path_control_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_control_x_mixin.py` & `apysc-3.0.0/apysc/_geom/path_control_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_control_y1_mixin.py` & `apysc-3.0.0/apysc/_geom/path_control_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_control_y2_mixin.py` & `apysc-3.0.0/apysc/_geom/path_control_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_control_y_mixin.py` & `apysc-3.0.0/apysc/_geom/path_control_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_data.py` & `apysc-3.0.0/apysc/_geom/path_data.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_data_base.py` & `apysc-3.0.0/apysc/_geom/path_data_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_data_util.py` & `apysc-3.0.0/apysc/_geom/path_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_dest_x_mixin.py` & `apysc-3.0.0/apysc/_geom/path_dest_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_dest_y_mixin.py` & `apysc-3.0.0/apysc/_geom/path_dest_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_horizontal.py` & `apysc-3.0.0/apysc/_geom/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_line_to.py` & `apysc-3.0.0/apysc/_geom/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_move_to.py` & `apysc-3.0.0/apysc/_geom/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_vertical.py` & `apysc-3.0.0/apysc/_geom/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_x_mixin.py` & `apysc-3.0.0/apysc/_geom/path_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/path_y_mixin.py` & `apysc-3.0.0/apysc/_geom/path_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/point2d.py` & `apysc-3.0.0/apysc/_geom/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_bottom_y_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_bottom_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_center_x_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_center_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_center_y_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_center_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_height_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_left_x_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_left_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_right_x_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_right_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_top_y_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_top_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/rectangle_geom_width_mixin.py` & `apysc-3.0.0/apysc/_geom/rectangle_geom_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_geom/relative_mixin.py` & `apysc-3.0.0/apysc/_geom/relative_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_html/debug_mode.py` & `apysc-3.0.0/apysc/_html/debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_html/exporter.py` & `apysc-3.0.0/apysc/_html/exporter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_html/html_util.py` & `apysc-3.0.0/apysc/_html/html_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_jslib/jquery-3.6.3.min.js` & `apysc-3.0.0/apysc/_jslib/jquery-3.6.3.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_jslib/jquery.mousewheel-3.1.13.min.js` & `apysc-3.0.0/apysc/_jslib/jquery.mousewheel-3.1.13.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_jslib/jslib_util.py` & `apysc-3.0.0/apysc/_jslib/jslib_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_jslib/svg-3.1.2.min.js` & `apysc-3.0.0/apysc/_jslib/svg-3.1.2.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_jslib/underscore-1.12.0.min.js` & `apysc-3.0.0/apysc/_jslib/underscore-1.12.0.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_jupyter/jupyter_util.py` & `apysc-3.0.0/apysc/_jupyter/jupyter_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py` & `apysc-3.0.0/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/conf_common.py` & `apysc-3.0.0/apysc/_lint_and_doc/conf_common.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/docs_keyword_link_mapping.py` & `apysc-3.0.0/apysc/_lint_and_doc/docs_keyword_link_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     "mousemove": "mousemove",
     "unbind_mousemove": "mousemove",
     "unbind_mousemove_all": "mousemove",
     "If": "if",
     "Elif": "elif",
     "Else": "else",
     "Return": "return",
-    "For": "for",
     "Continue": "continue",
     "Timer": "timer",
     "TimerEvent": "timer_event",
     "FPS": "fps",
     "fps": "fps",
     "timer_complete": "timer_complete",
     "AnimationEvent": "animation_event",
@@ -202,8 +201,10 @@
     "lstrip": "string_lstrip",
     "strip": "string_strip",
     "rstrip": "string_rstrip",
     "ForArrayIndices": "for_array_indices",
     "ForArrayValues": "for_array_values",
     "ForArrayIndicesAndValues": "for_array_indices_and_values",
     "ForDictKeys": "for_dict_keys",
+    "ForDictValues": "for_dict_values",
+    "ForDictKeysAndValues": "for_dict_keys_and_values",
 }
```

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/docs_lang.py` & `apysc-3.0.0/apysc/_lint_and_doc/docs_lang.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/docs_toctree_util.py` & `apysc-3.0.0/apysc/_lint_and_doc/docs_toctree_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,16 @@
     """
     if adjacent_doc_file_name == expected_md_file_name:
         return False
     if adjacent_doc_file_name.strip() == "":
         return False
     now_unix_time: float = datetime.now().timestamp()
     file_path: str = f"./docs_src/source/{adjacent_doc_file_name}"
+    if not os.path.exists(file_path):
+        return False
     os.utime(file_path, (now_unix_time, now_unix_time))
     logger.info(msg=f"Document's modified time is updated: {adjacent_doc_file_name}")
     for lang in Lang:
         if lang == Lang.EN:
             continue
         other_lang_doc_file_path: str = (
             f"./docs_src/source/{lang.value}_{adjacent_doc_file_name}"
```

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/docs_translation_converter.py` & `apysc-3.0.0/apysc/_lint_and_doc/docs_translation_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/docstring_to_markdown_converter.py` & `apysc-3.0.0/apysc/_lint_and_doc/docstring_to_markdown_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/docstring_util.py` & `apysc-3.0.0/apysc/_lint_and_doc/docstring_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/document_text_split_util.py` & `apysc-3.0.0/apysc/_lint_and_doc/document_text_split_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/document_util.py` & `apysc-3.0.0/apysc/_lint_and_doc/document_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py` & `apysc-3.0.0/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/fixed_translation_mapping/jp.py` & `apysc-3.0.0/apysc/_lint_and_doc/fixed_translation_mapping/jp.py`

 * *Files 0% similar despite different names*

```diff
@@ -4028,12 +4028,44 @@
             val="`ap.Dictionary`の各キーのためのループ用のクラスです。<hr>",
         ),
         Mapping(
             key="  - A dictionary to iterate.",
             val="  - イテレーションで扱うための辞書。",
         ),
         Mapping(
-            key="  - A dictionary key type. This interface accepsts hashable types, such as the `String`, `Int`, or `Boolean`.",
-            val="  - 辞書のキーの型。このインターフェイスはハッシュ化可能な`String`、`Int`、`Boolean`といった型のみ受け付けます。",
+            key="  - A dictionary key type. This interface accepsts hashable types, such as the `String`, `Int`, `Number`, or `Boolean`.",
+            val="  - 辞書のキーの型。このインターフェイスはハッシュ化可能な`String`、`Int`、`Number`、`Boolean`といった型のみ受け付けます。",
+        ),
+        Mapping(
+            key="## ForDictValues API",
+            val="## ForDictValues API",
+        ),
+        Mapping(
+            key="The loop implementation class for the `ap.Dictionary` values.<hr>",
+            val="`ap.Dictionary`の値のためのループ制御のためのクラスです。<hr>",
+        ),
+        Mapping(
+            key="  - A dictionary value type. This interface accepts `InitializeForLoopKeyOrValueInterface` subclasses, such as the `Int`, `String`, or `Rectangle`.",
+            val="  - 辞書の値の型。ごのインターフェイスは`Int`、`String`、`Rectangle`などの`InitializeForLoopKeyOrValueInterface`のサブクラスの型のみ受け付けます。",
+        ),
+        Mapping(
+            key="ForDictValues class",
+            val="ForDictValues クラス",
+        ),
+        Mapping(
+            key="## ForDictKeysAndValues API",
+            val="## ForDictKeysAndValues API",
+        ),
+        Mapping(
+            key="ForDictKeysAndValues class",
+            val="ForDictKeysAndValues クラス",
+        ),
+        Mapping(
+            key="The loop implementation class for the `ap.Dictionary` keys and values.<hr>",
+            val="`ap.Dictionary`のキーと値のためのループのクラスの実装です。<hr>",
+        ),
+        Mapping(
+            key="  - A dictionary key type. This interface accepts hashable types, such as the `String`, `Int`, `Number`, or `Boolean`.",
+            val="  - 辞書のキーの型。このインターフェイスは`String`、`Int`、`Number`、`Boolean`といったハッシュ化可能な型を受け付けます。",
         ),
     ]
 )
```

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/lint_and_doc_hash_util.py` & `apysc-3.0.0/apysc/_lint_and_doc/lint_and_doc_hash_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_lint_and_doc/translation_mapping_utils.py` & `apysc-3.0.0/apysc/_lint_and_doc/translation_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_loop/_continue.py` & `apysc-3.0.0/apysc/_loop/_continue.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,61 +9,61 @@
 class Continue:
     """
     The loop continue expression class.
 
     Notes
     -----
     This class can be instantiated in the with loop statement,
-    for example, after the `with ap.For(...):` statement.
+    for example, after the `with ap.ForArrayIndices(...):` statement.
 
     References
     ----------
     - Continue
         - https://simon-ritchie.github.io/apysc/en/continue.html
 
     Examples
     --------
     >>> import apysc as ap
     >>> arr: ap.Array = ap.Array(range(3))
-    >>> with ap.For(arr) as i:
+    >>> with ap.ForArrayIndices(arr) as i:
     ...     with ap.If(i == 1):
     ...         _ = ap.Continue()
     ...
     """
 
     @final
     @add_debug_info_setting(module_name=__name__)
     def __init__(self) -> None:
         """
         The loop continue expression class.
 
         Notes
         -----
         This class can be instantiated in the with loop statement,
-        for example, after the `with ap.For(...):` statement.
+        for example, after the `with ap.ForArrayIndices(...):` statement.
 
         References
         ----------
         - Continue
             - https://simon-ritchie.github.io/apysc/en/continue.html
 
         Examples
         --------
         >>> import apysc as ap
         >>> arr: ap.Array = ap.Array(range(3))
-        >>> with ap.For(arr) as i:
+        >>> with ap.ForArrayIndices(arr) as i:
         ...     with ap.If(i == 1):
         ...         _ = ap.Continue()
         ...
         """
         import apysc as ap
         from apysc._loop import loop_count
 
         current_loop_count: int = loop_count.get_current_loop_count()
         if current_loop_count == 0:
             err_msg: str = (
                 "The `Continue` class can be instantiated in the with "
                 "loop statement, for example, after the "
-                "`with ap.For(...):` statement."
+                "`with ap.ForArrayIndices(...):` statement."
             )
             raise Exception(err_msg)
         ap.append_js_expression(expression="continue;")
```

### Comparing `apysc-2.8.9/apysc/_loop/_for.py` & `apysc-3.0.0/apysc/_type/int.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,215 +1,230 @@
-"""This module is for the `For` loop class implementation.
+"""Class implementation of integer.
 """
 
-from typing import Any
-from typing import Dict
-from typing import Generic
-from typing import Optional
-from typing import TypeVar
 from typing import Union
 
 from typing_extensions import final
 
-from apysc._expression.indent_num import Indent
 from apysc._html.debug_mode import add_debug_info_setting
-from apysc._type.array import Array
-from apysc._type.dictionary import Dictionary
-from apysc._type.int import Int
-from apysc._type.number import Number
-from apysc._type.string import String
-
-_Target = TypeVar("_Target", Int, String, Number)
-
-
-class For(Generic[_Target]):
+from apysc._loop.initialize_for_loop_key_or_value_interface import (
+    InitializeForLoopKeyOrValueInterface,
+)
+from apysc._type.hashable_interface import HashableInterface
+from apysc._type.number_value_mixin import NumberValueMixIn
+from apysc._type.to_fixed_mixin import ToFixedMixIn
+from apysc._type.to_number_mixin import ToNumberMixIn
+from apysc._type.to_string_mixin import ToStringMixIn
+from apysc._validation import arg_validation_decos
+
+
+class Int(
+    NumberValueMixIn[int, "Int"],
+    InitializeForLoopKeyOrValueInterface,
+    ToStringMixIn,
+    ToFixedMixIn,
+    HashableInterface,
+    ToNumberMixIn,
+):
     """
-    The class to append for the (loop) expression.
+    Integer class for the apysc library.
 
     References
     ----------
-    - For
-        - https://simon-ritchie.github.io/apysc/en/for.html
+    - Int and Number
+        - https://simon-ritchie.github.io/apysc/en/int_and_number.html
+    - Int and Number common arithmetic operations
+        - https://simon-ritchie.github.io/apysc/en/int_and_number_arithmetic_operations.html  # noqa
+    - Int and Number common comparison operations
+        - https://simon-ritchie.github.io/apysc/en/int_and_number_comparison_operations.html  # noqa
 
     Examples
     --------
     >>> import apysc as ap
-    >>> arr: ap.Array = ap.Array(range(3))
-    >>> with ap.For(arr) as i:
-    ...     ap.trace("Loop index is:", i)
-    ...
+    >>> int_val: ap.Int = ap.Int(10)
+    >>> int_val
+    Int(10)
+
+    >>> int_val == 10
+    Boolean(True)
+
+    >>> int_val == ap.Int(10)
+    Boolean(True)
+
+    >>> int_val >= 10
+    Boolean(True)
+
+    >>> int_val += 10
+    >>> int_val
+    Int(20)
+
+    >>> int_val = ap.Int(10.5)
+    >>> int_val
+    Int(10)
     """
 
-    _arr_or_dict: Union[Array, Dictionary]
-    _locals: Dict[str, Any]
-    _globals: Dict[str, Any]
-    _snapshot_name: str
-    _indent: Indent
-
-    @final
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_builtin_string(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
-        arr_or_dict: Union[Array, Dictionary],
+        value: Union[int, float, NumberValueMixIn],
         *,
-        locals_: Optional[Dict[str, Any]] = None,
-        globals_: Optional[Dict[str, Any]] = None,
+        variable_name_suffix: str = "",
+        skip_init_substitution_expression_appending: bool = False,
     ) -> None:
         """
-        The class to append for the (loop) expression.
+        Integer class for apysc library.
 
         Parameters
         ----------
-        arr_or_dict : Array or Dictionary
-            Array or Dictionary instance to iterate.
-        locals_ : dict or None, default None
-            Current scope's local variables. Set locals()
-            value to this argument. If specified, this interface
-            reverts all local scope VariableNameMixIn
-            variables (like Int, Sprite) at the end of a `For`
-            scope. This setting is useful when you don't want to
-            update each variable by implementing the `For` scope.
-        globals_ : dict or None, default None
-            Current scope's global variables. Set globals()
-            value to this argument. This setting works
-            the same way as the locals_ argument.
+        value : int or float or Int or Number
+            Initial integer value. If the `float` or `Number`
+            value is specified, this class casts it to an integer.
+        variable_name_suffix : str, default ''
+            A JavaScript variable name suffix string.
+            This setting is sometimes useful for JavaScript debugging.
+        skip_init_substitution_expression_appending : bool, default False
+            A boolean indicates whether to skip an initial substitution
+            expression or not. This class uses this option internally.
 
         References
         ----------
-        - For
-            - https://simon-ritchie.github.io/apysc/en/for.html
+        - Int and Number
+            - https://simon-ritchie.github.io/apysc/en/int_and_number.html
+        - Int and Number common arithmetic operations
+            - https://simon-ritchie.github.io/apysc/en/int_and_number_arithmetic_operations.html  # noqa
+        - Int and Number common comparison operations
+            - https://simon-ritchie.github.io/apysc/en/int_and_number_comparison_operations.html  # noqa
 
         Examples
         --------
         >>> import apysc as ap
-        >>> arr: ap.Array = ap.Array(range(3))
-        >>> with ap.For(arr) as i:
-        ...     ap.trace("Loop index is:", i)
-        ...
-        """
-        self._validate_arr_or_dict_val_type(arr_or_dict=arr_or_dict)
-        if locals_ is None:
-            locals_ = {}
-        if globals_ is None:
-            globals_ = {}
-        self._arr_or_dict = arr_or_dict
-        self._locals = locals_
-        self._globals = globals_
-        self._indent = Indent()
+        >>> int_val: ap.Int = ap.Int(10)
+        >>> int_val
+        Int(10)
+
+        >>> int_val == 10
+        Boolean(True)
+
+        >>> int_val == ap.Int(10)
+        Boolean(True)
+
+        >>> int_val >= 10
+        Boolean(True)
+
+        >>> int_val += 10
+        >>> int_val
+        Int(20)
+
+        >>> int_val = ap.Int(10.5)
+        >>> int_val
+        Int(10)
+        """
+        from apysc._converter import cast
+        from apysc._expression import expression_variables_util
+        from apysc._expression import var_names
+        from apysc._expression.event_handler_scope import TemporaryNotHandlerScope
+        from apysc._type import type_util
+
+        with TemporaryNotHandlerScope():
+            is_number_specified: bool = type_util.is_number(value=value)
+            TYPE_NAME: str = var_names.INT
+            self.variable_name = expression_variables_util.get_next_variable_name(
+                type_name=TYPE_NAME
+            )
+            super(Int, self).__init__(
+                value=value,
+                type_name=TYPE_NAME,
+                variable_name_suffix=variable_name_suffix,
+            )
+            self._value = cast.to_int_from_float(int_or_float=self.value)
+            self._append_constructor_expression()
+            self._append_cast_expression(is_number_specified=is_number_specified)
+
+        self._append_initial_substitution_expression_if_in_handler_scope(
+            skip_appending=skip_init_substitution_expression_appending,
+        )
 
     @final
-    def _validate_arr_or_dict_val_type(
-        self, *, arr_or_dict: Union[Array, Dictionary]
-    ) -> None:
+    @add_debug_info_setting(module_name=__name__)
+    def _append_cast_expression(self, *, is_number_specified: bool) -> None:
         """
-        Validate loop value type is Array of Dictionary.
+        Append integer cast (Math.trunc) expression.
 
         Parameters
         ----------
-        arr_or_dict : Array or Dictionary
-            Value to be checked.
-
-        Raises
-        ------
-        TypeError
-            If a value type is neither Array nor Dictionary.
+        is_number_specified : bool
+            Boolean value whether a specified value is Number
+            instance or not.
         """
-        if isinstance(arr_or_dict, (Array, Dictionary)):
+        import apysc as ap
+
+        if not is_number_specified:
             return
-        raise TypeError(
-            "Specified value type is neither Array nor Dictionary: "
-            f"{type(arr_or_dict)}"
+        expression: str = (
+            f"{self.variable_name} = Math.trunc({self.variable_name}, 10);"
         )
+        ap.append_js_expression(expression=expression)
 
     @final
-    @add_debug_info_setting(module_name=__name__)
-    def __enter__(self) -> _Target:
+    def _set_value_and_skip_expression_appending(
+        self, *, value: Union[int, float, NumberValueMixIn]
+    ) -> None:
         """
-        This class calls this method at the with-statement.
+        Update value attribute and skip expression appending.
 
-        Returns
-        -------
-        i_or_key : Int or String
-            Loop index or dictionary key.
-        """
-        import apysc as ap
-        from apysc._loop import loop_count
-        from apysc._type import revert_mixin
-
-        loop_count.increment_current_loop_count()
-        self._snapshot_name = revert_mixin.make_snapshots_of_each_scope_vars(
-            locals_=self._locals, globals_=self._globals
-        )
-        i_or_key: Union[ap.Int, ap.String]
-        if isinstance(self._arr_or_dict, ap.Array):
-            i_or_key = ap.Int(0)
-            self._append_arr_enter_expression(i=i_or_key)
-        elif isinstance(self._arr_or_dict, ap.Dictionary):
-            if self._arr_or_dict._value:
-                key: str = str(list(self._arr_or_dict._value.keys())[0])
-            else:
-                key = ""
-            i_or_key = ap.String(key)
-            self._append_dict_enter_expression(key=i_or_key)
-        self._indent.__enter__()
-        return i_or_key  # type: ignore
+        Parameters
+        ----------
+        value : int or float or Int or Number
+            Any number value to set. This interface casts that
+            value to an integer if float or number value is specified.
+        """
+        from apysc._converter import cast
+
+        if isinstance(value, NumberValueMixIn):
+            value._value = cast.to_int_from_float(int_or_float=value._value)
+            value_: Union[int, float, NumberValueMixIn] = value._value
+        else:
+            value = cast.to_int_from_float(int_or_float=value)
+            value_ = value
+        self._value = value_  # type: ignore
 
-    @final
-    @add_debug_info_setting(module_name=__name__)
-    def __exit__(self, *args: Any) -> None:
+    def __repr__(self) -> str:
         """
-        This class calls this method at the with-statement.
+        Get a representation string of this instance.
+
+        Returns
+        -------
+        repr_str : str
+            Representation string of this instance.
         """
-        import apysc as ap
-        from apysc._expression import last_scope
-        from apysc._expression.last_scope import LastScope
-        from apysc._loop import loop_count
-        from apysc._type import revert_mixin
-
-        loop_count.decrement_current_loop_count()
-        revert_mixin.revert_each_scope_vars(
-            snapshot_name=self._snapshot_name,
-            locals_=self._locals,
-            globals_=self._globals,
-        )
-        self._indent.__exit__()
-        ap.append_js_expression(expression="}")
-        last_scope.set_last_scope(value=LastScope.FOR)
+        if not hasattr(self, "_value"):
+            repr_str: str = "Int(0)"
+        else:
+            repr_str = f"Int({self._value})"
+        return repr_str
 
+    @classmethod
     @final
-    @add_debug_info_setting(module_name=__name__)
-    def _append_arr_enter_expression(self, *, i: Int) -> None:
+    def _initialize_for_loop_key_or_value(cls) -> "Int":
         """
-        Append for loop start expression (for Array value).
+        Initialize this instance for a loop key or value.
 
-        Parameters
-        ----------
-        i : Int
-            Loop index value.
+        Returns
+        -------
+        int_value : Int
+            An initialized integer value.
         """
-        import apysc as ap
-
-        i_name: str = i.variable_name
-        expression: str = (
-            f"var length = {self._arr_or_dict.variable_name}.length;\n"
-            f"for ({i_name} = 0; {i_name} < length; {i_name}++) {{"
-        )
-        ap.append_js_expression(expression=expression)
+        return Int(0)
 
     @final
-    @add_debug_info_setting(module_name=__name__)
-    def _append_dict_enter_expression(self, *, key: String) -> None:
+    def __hash__(self) -> int:
         """
-        Append for loop start expression (for Dictionary value).
+        Get a hashed value.
 
-        Parameters
-        ----------
-        key : String
-            Loop (dictionary) key value.
+        Returns
+        -------
+        hashed_value : int
+            A hashed value.
         """
-        import apysc as ap
-
-        key_name: str = key.variable_name
-        expression: str = (
-            f"for (var {key_name} in " f"{self._arr_or_dict.variable_name}) {{"
-        )
-        ap.append_js_expression(expression=expression)
+        return int(self._value)
```

### Comparing `apysc-2.8.9/apysc/_loop/_range.py` & `apysc-3.0.0/apysc/_loop/_range.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_loop/for_array_indices.py` & `apysc-3.0.0/apysc/_loop/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_loop/for_array_indices_and_values.py` & `apysc-3.0.0/apysc/_loop/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_loop/for_array_values.py` & `apysc-3.0.0/apysc/_loop/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_loop/for_dict_keys.py` & `apysc-3.0.0/apysc/_loop/for_dict_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 from apysc._loop.for_loop_exit_mixin import ForLoopExitMixIn
 from apysc._type.boolean import Boolean
 from apysc._type.dictionary import Dictionary
 from apysc._type.initialize_locals_and_globals_mixin import (
     InitializeLocalsAndGlobalsMixIn,
 )
 from apysc._type.int import Int
+from apysc._type.number import Number
 from apysc._type.string import String
 from apysc._validation import arg_validation_decos
 
-_DictKey = TypeVar("_DictKey", String, Int, Boolean)
+_DictKey = TypeVar("_DictKey", String, Int, Number, Boolean)
 
 
 class ForDictKeys(
     ForLoopExitMixIn,
     GetLastScopeInterface,
     InitializeLocalsAndGlobalsMixIn,
     Generic[_DictKey],
@@ -87,15 +88,15 @@
 
         Parameters
         ----------
         dict_ : Dictionary[_DictKey, Any]
             A dictionary to iterate.
         dict_key_type : Type[_DictKey]
             A dictionary key type. This interface accepts hashable types,
-            such as the `String`, `Int`, or `Boolean`.
+            such as the `String`, `Int`, `Number`, or `Boolean`.
         locals_ : Optional[Dict[str, Any]], optional
             Current scope's local variables. Set locals()
             value to this argument. If specified, this interface
             reverts all local scope VariableNameMixIn
             variables (like Int, Sprite) at the end of a with-statement
             scope. This setting is useful when you don't want to
             update each variable.
```

### Comparing `apysc-2.8.9/apysc/_loop/for_loop_exit_mixin.py` & `apysc-3.0.0/apysc/_loop/for_loop_exit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_loop/initialize_for_loop_key_or_value_interface.py` & `apysc-3.0.0/apysc/_loop/initialize_for_loop_key_or_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_loop/loop_count.py` & `apysc-3.0.0/apysc/_loop/loop_count.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_math/max_mixin.py` & `apysc-3.0.0/apysc/_math/max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_math/min_mixin.py` & `apysc-3.0.0/apysc/_math/min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_math/trunc_mixin.py` & `apysc-3.0.0/apysc/_math/trunc_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_string/indent_util.py` & `apysc-3.0.0/apysc/_string/indent_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_string/string_util.py` & `apysc-3.0.0/apysc/_string/string_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_testing/e2e_testing_helper.py` & `apysc-3.0.0/apysc/_testing/e2e_testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_testing/testing_helper.py` & `apysc-3.0.0/apysc/_testing/testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/datetime_.py` & `apysc-3.0.0/apysc/_time/datetime_.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/day_mixin.py` & `apysc-3.0.0/apysc/_time/day_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/days_mixin.py` & `apysc-3.0.0/apysc/_time/days_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/fps.py` & `apysc-3.0.0/apysc/_time/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/hour_mixin.py` & `apysc-3.0.0/apysc/_time/hour_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/left_and_right_datetimes_mixin.py` & `apysc-3.0.0/apysc/_time/left_and_right_datetimes_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/millisecond_mixin.py` & `apysc-3.0.0/apysc/_time/millisecond_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/minute_mixin.py` & `apysc-3.0.0/apysc/_time/minute_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/month_end_mixin.py` & `apysc-3.0.0/apysc/_time/month_end_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/month_mixin.py` & `apysc-3.0.0/apysc/_time/month_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/now_mixin.py` & `apysc-3.0.0/apysc/_time/now_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/second_mixin.py` & `apysc-3.0.0/apysc/_time/second_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/timedelta_.py` & `apysc-3.0.0/apysc/_time/timedelta_.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/timer.py` & `apysc-3.0.0/apysc/_time/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/total_seconds_mixin.py` & `apysc-3.0.0/apysc/_time/total_seconds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/weekday_mixin.py` & `apysc-3.0.0/apysc/_time/weekday_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_time/year_mixin.py` & `apysc-3.0.0/apysc/_time/year_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/about_handler_options_type.py` & `apysc-3.0.0/apysc/_translation/jp/about_handler_options_type.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/add_child_and_remove_child.py` & `apysc-3.0.0/apysc/_translation/jp/add_child_and_remove_child.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/add_debug_info_setting.py` & `apysc-3.0.0/apysc/_translation/jp/add_debug_info_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_base_start.py` & `apysc-3.0.0/apysc/_translation/jp/animation_base_start.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_base_target.py` & `apysc-3.0.0/apysc/_translation/jp/animation_base_target.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_complete.py` & `apysc-3.0.0/apysc/_translation/jp/animation_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_delay.py` & `apysc-3.0.0/apysc/_translation/jp/animation_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_duration.py` & `apysc-3.0.0/apysc/_translation/jp/animation_duration.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_event.py` & `apysc-3.0.0/apysc/_translation/jp/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_fill_alpha.py` & `apysc-3.0.0/apysc/_translation/jp/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_fill_color.py` & `apysc-3.0.0/apysc/_translation/jp/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_finish.py` & `apysc-3.0.0/apysc/_translation/jp/animation_finish.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_interfaces_abstract.py` & `apysc-3.0.0/apysc/_translation/jp/animation_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_line_alpha.py` & `apysc-3.0.0/apysc/_translation/jp/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_line_color.py` & `apysc-3.0.0/apysc/_translation/jp/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_line_thickness.py` & `apysc-3.0.0/apysc/_translation/jp/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_method_chaining.py` & `apysc-3.0.0/apysc/_translation/jp/animation_method_chaining.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_move.py` & `apysc-3.0.0/apysc/_translation/jp/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_parallel.py` & `apysc-3.0.0/apysc/_translation/jp/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_pause_and_play.py` & `apysc-3.0.0/apysc/_translation/jp/animation_pause_and_play.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_radius.py` & `apysc-3.0.0/apysc/_translation/jp/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_reset.py` & `apysc-3.0.0/apysc/_translation/jp/animation_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_return_value.py` & `apysc-3.0.0/apysc/_translation/jp/animation_return_value.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_reverse.py` & `apysc-3.0.0/apysc/_translation/jp/animation_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_rotation_around_center.py` & `apysc-3.0.0/apysc/_translation/jp/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_rotation_around_point.py` & `apysc-3.0.0/apysc/_translation/jp/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_scale_x_and_y_from_center.py` & `apysc-3.0.0/apysc/_translation/jp/animation_scale_x_and_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_scale_x_and_y_from_point.py` & `apysc-3.0.0/apysc/_translation/jp/animation_scale_x_and_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_time.py` & `apysc-3.0.0/apysc/_translation/jp/animation_time.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_width_and_height.py` & `apysc-3.0.0/apysc/_translation/jp/animation_width_and_height.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_x.py` & `apysc-3.0.0/apysc/_translation/jp/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/animation_y.py` & `apysc-3.0.0/apysc/_translation/jp/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/append_js_expression.py` & `apysc-3.0.0/apysc/_translation/jp/append_js_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array.py` & `apysc-3.0.0/apysc/_translation/jp/array.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_append_and_push.py` & `apysc-3.0.0/apysc/_translation/jp/array_append_and_push.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_clear.py` & `apysc-3.0.0/apysc/_translation/jp/array_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_comparison.py` & `apysc-3.0.0/apysc/_translation/jp/array_comparison.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_extend_and_concat.py` & `apysc-3.0.0/apysc/_translation/jp/array_extend_and_concat.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_index_of.py` & `apysc-3.0.0/apysc/_translation/jp/array_index_of.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_insert_and_insert_at.py` & `apysc-3.0.0/apysc/_translation/jp/array_insert_and_insert_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_join.py` & `apysc-3.0.0/apysc/_translation/jp/array_join.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_length.py` & `apysc-3.0.0/apysc/_translation/jp/array_length.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_pop.py` & `apysc-3.0.0/apysc/_translation/jp/array_pop.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_remove_and_remove_at.py` & `apysc-3.0.0/apysc/_translation/jp/array_remove_and_remove_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_reverse.py` & `apysc-3.0.0/apysc/_translation/jp/array_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_slice.py` & `apysc-3.0.0/apysc/_translation/jp/array_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/array_sort.py` & `apysc-3.0.0/apysc/_translation/jp/array_sort.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py` & `apysc-3.0.0/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assert_defined_and_undefined.py` & `apysc-3.0.0/apysc/_translation/jp/assert_defined_and_undefined.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py` & `apysc-3.0.0/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assert_equal_and_not_equal.py` & `apysc-3.0.0/apysc/_translation/jp/assert_equal_and_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assert_greater_and_greater_equal.py` & `apysc-3.0.0/apysc/_translation/jp/assert_greater_and_greater_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assert_less_and_less_equal.py` & `apysc-3.0.0/apysc/_translation/jp/assert_less_and_less_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assert_true_and_false.py` & `apysc-3.0.0/apysc/_translation/jp/assert_true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/assertion_basic_behavior.py` & `apysc-3.0.0/apysc/_translation/jp/assertion_basic_behavior.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/bind_and_trigger_custom_event.py` & `apysc-3.0.0/apysc/_translation/jp/bind_and_trigger_custom_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/boolean.py` & `apysc-3.0.0/apysc/_translation/jp/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py` & `apysc-3.0.0/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/circle.py` & `apysc-3.0.0/apysc/_translation/jp/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/click.py` & `apysc-3.0.0/apysc/_translation/jp/click.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/contains.py` & `apysc-3.0.0/apysc/_translation/jp/contains.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/continue.py` & `apysc-3.0.0/apysc/_translation/jp/continue.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,37 +15,37 @@
     ##################################################
     "Before reading on, maybe it is helpful to read the following page (apysc uses the `Continue` class for the same reason):": "このページを読み進める前に以下のページを確認しておくと役に立つかもしれません（apyscでは`Continue`クラスを同様の利用で使用しています）。",  # noqa
     ##################################################
     "- [Why the apysc library doesn't use the Python built-in data type](why_apysc_doesnt_use_python_builtin_data_type.md)": "- [なぜapyscではPythonのビルトインのデータの型を使用していないのか](jp_why_apysc_doesnt_use_python_builtin_data_type.md)",  # noqa
     ##################################################
     "## What is the Continue class?": "## Continue クラスの概要",
     ##################################################
-    "The `with For` block uses the `Continue` class to skip a current loop iteration (in JavaScript). It behaves like the Python built-in `continue` keyword.": "`with For`のブロックではJavaScript上での特定のループをスキップするために`Continue`クラスが使用されます。このインターフェイスはPythonビルトインの`continue`キーワードのように動作します。",  # noqa
+    "The `with ap.ForArrayIndices` block uses the `Continue` class to skip a current loop iteration (in JavaScript). It behaves like the Python built-in `continue` keyword.": "`with For`のブロックではJavaScript上での特定のループをスキップするために`Continue`クラスが使用されます。このインターフェイスはPythonビルトインの`continue`キーワードのように動作します。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
-    "The `Continue` class can only be used in the `with For` (or other loop class) block, as follows:": "`Continue`クラスは以下のコード例のように`with For`（もしくは他のループクラス）のブロックでのみ使用することができます:",  # noqa
+    "The `Continue` class can only be used in the `with ap.ForArrayIndices` (or other loop class) block, as follows:": "`Continue`クラスは以下のコード例のように`with For`（もしくは他のループクラス）のブロックでのみ使用することができます:",  # noqa
     ##################################################
-    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=250, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\n\narr: ap.Array = ap.Array(range(2))\ni: ap.Int\nwith ap.For(arr) as i:\n    condition: ap.Boolean = i == 0\n    with ap.If(condition):\n        sprite.graphics.begin_fill(color="#0af")\n        sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\n        ap.Continue()\n\n    sprite.graphics.begin_fill(color="#f0a")\n    sprite.graphics.draw_rect(x=150, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="continue_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=250, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\n\narr: ap.Array = ap.Array(range(2))\ni: ap.Int\nwith ap.For(arr) as i:\n    condition: ap.Boolean = i == 0\n    with ap.If(condition):\n        sprite.graphics.begin_fill(color="#0af")\n        sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\n        ap.Continue()\n\n    sprite.graphics.begin_fill(color="#f0a")\n    sprite.graphics.draw_rect(x=150, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="continue_basic_usage/")\n```',  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=250, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\n\narr: ap.Array = ap.Array(range(2))\nwith ap.ForArrayIndices(arr) as i:\n    condition: ap.Boolean = i == 0\n    with ap.If(condition):\n        sprite.graphics.begin_fill(color="#0af")\n        sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\n        ap.Continue()\n\n    sprite.graphics.begin_fill(color="#f0a")\n    sprite.graphics.draw_rect(x=150, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="continue_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=250, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\n\narr: ap.Array = ap.Array(range(2))\nwith ap.ForArrayIndices(arr) as i:\n    condition: ap.Boolean = i == 0\n    with ap.If(condition):\n        sprite.graphics.begin_fill(color="#0af")\n        sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\n        ap.Continue()\n\n    sprite.graphics.begin_fill(color="#f0a")\n    sprite.graphics.draw_rect(x=150, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="continue_basic_usage/")\n```',  # noqa
     ##################################################
-    "If you use the `Continue` class in the out of the `with For` block, then an exception is raised:": "もし`Continue`クラスを`with For`ブロック外で使用した場合はエラーになります:",  # noqa
+    "If you use the `Continue` class in the out of the `with ap.ForArrayIndices` block, then an exception is raised:": "もし`Continue`クラスを`with For`ブロック外で使用した場合はエラーになります:",  # noqa
     ##################################################
     "```py\nimport apysc as ap\n\nap.Continue()\n```": "```py\nimport apysc as ap\n\nap.Continue()\n```",  # noqa
     ##################################################
-    "```\nException: The `Continue` class can be instantiated in the with loop statement, for example, after the `with ap.For(...):` statement.\n```": "```\nException: The `Continue` class can be instantiated in the with loop statement, for example, after the `with ap.For(...):` statement.\n```",  # noqa
+    "```\nException: The `Continue` class can be instantiated in the with loop statement, for example, after the `with ap.ForArrayIndices(...):` statement.\n```": "```\nException: The `Continue` class can be instantiated in the with loop statement, for example, after the `with ap.ForArrayIndices(...):` statement.\n```",  # noqa
     ##################################################
     "## Continue API": "## Continue API",
     ##################################################
     '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "The loop continue expression class.<hr>": "ループのcontinueの表現を扱うためのクラスです。<hr>",
     ##################################################
     "**[Notes]**": "**[特記事項]**",
     ##################################################
-    "This class can be instantiated in the with loop statement, for example, after the `with ap.For(...):` statement.<hr>": "このクラスはwithステートメントのループ内でのみインスタンス化することができます。例えば`with ap.For(...)ステート内が該当します。`<hr>",  # noqa
+    "This class can be instantiated in the with loop statement, for example, after the `with ap.ForArrayIndices(...):` statement.<hr>": "このクラスはwithステートメントのループ内でのみインスタンス化することができます。例えば`with ap.ForArrayIndices(...)ステート内が該当します。`<hr>",  # noqa
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    "```py\n>>> import apysc as ap\n>>> arr: ap.Array = ap.Array(range(3))\n>>> with ap.For(arr) as i:\n...     with ap.If(i == 1):\n...         _ = ap.Continue()\n...\n```": "```py\n>>> import apysc as ap\n>>> arr: ap.Array = ap.Array(range(3))\n>>> with ap.For(arr) as i:\n...     with ap.If(i == 1):\n...         _ = ap.Continue()\n...\n```",  # noqa
+    "```py\n>>> import apysc as ap\n>>> arr: ap.Array = ap.Array(range(3))\n>>> with ap.ForArrayIndices(arr) as i:\n...     with ap.If(i == 1):\n...         _ = ap.Continue()\n...\n```": "```py\n>>> import apysc as ap\n>>> arr: ap.Array = ap.Array(range(3))\n>>> with ap.ForArrayIndices(arr) as i:\n...     with ap.If(i == 1):\n...         _ = ap.Continue()\n...\n```",  # noqa
 }
```

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime.py` & `apysc-3.0.0/apysc/_translation/jp/datetime.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_day.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_day.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_hour.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_hour.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_millisecond.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_millisecond.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_minute.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_minute.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_month.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_month.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_now.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_now.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_second.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_second.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_set_month_end.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_set_month_end.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/datetime_year.py` & `apysc-3.0.0/apysc/_translation/jp/datetime_year.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/dblclick.py` & `apysc-3.0.0/apysc/_translation/jp/dblclick.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/delete.py` & `apysc-3.0.0/apysc/_translation/jp/delete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/dictionary.py` & `apysc-3.0.0/apysc/_translation/jp/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/dictionary_generic.py` & `apysc-3.0.0/apysc/_translation/jp/dictionary_generic.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/dictionary_get.py` & `apysc-3.0.0/apysc/_translation/jp/dictionary_get.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/dictionary_length.py` & `apysc-3.0.0/apysc/_translation/jp/dictionary_length.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_object.py` & `apysc-3.0.0/apysc/_translation/jp/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py` & `apysc-3.0.0/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_object_get_and_set_css.py` & `apysc-3.0.0/apysc/_translation/jp/display_object_get_and_set_css.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_object_mouse_event.py` & `apysc-3.0.0/apysc/_translation/jp/display_object_mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_object_parent.py` & `apysc-3.0.0/apysc/_translation/jp/display_object_parent.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_object_visible.py` & `apysc-3.0.0/apysc/_translation/jp/display_object_visible.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_object_x_and_y.py` & `apysc-3.0.0/apysc/_translation/jp/display_object_x_and_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_on_colaboratory.py` & `apysc-3.0.0/apysc/_translation/jp/display_on_colaboratory.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/display_on_jupyter.py` & `apysc-3.0.0/apysc/_translation/jp/display_on_jupyter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/draw_interfaces_abstract.py` & `apysc-3.0.0/apysc/_translation/jp/draw_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/easing_enum.py` & `apysc-3.0.0/apysc/_translation/jp/easing_enum.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/elif.py` & `apysc-3.0.0/apysc/_translation/jp/elif.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/ellipse.py` & `apysc-3.0.0/apysc/_translation/jp/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/else.py` & `apysc-3.0.0/apysc/_translation/jp/else.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/enter_frame.py` & `apysc-3.0.0/apysc/_translation/jp/enter_frame.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py` & `apysc-3.0.0/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/for.py` & `apysc-3.0.0/apysc/_translation/jp/path_line_to.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,83 @@
 """This module is for the translation mapping data of the
 following document:
 
-Document file: for.md
+Document file: path_line_to.md
 Language: jp
 """
 
 from typing import Dict
 
 MAPPING: Dict[str, str] = {
     ##################################################
-    "# For class": "# For クラス",
+    "# PathLineTo class": "# PathLineTo クラス",
     ##################################################
-    "This page explains the `For` class.": "このページでは`For`クラスについて説明します。",
+    "This page explains the `PathLineTo` class.": "このページでは`PathLineTo`クラスについて説明します。",
     ##################################################
-    "Before reading on, maybe it is helpful to read the following page (the apysc uses the `For` class for the same reason for each data type):": "このページを読み進める前に以下のページを事前に確認しておくと役に立つかもしれません（apyscでは`For`クラスを各データ型のクラスと同じ理由で使用しています）。",  # noqa
+    "## What class is this?": "## クラス概要",
     ##################################################
-    "- [Why the apysc library doesn't use the Python built-in data type](why_apysc_doesnt_use_python_builtin_data_type.md)": "- [なぜapyscではPythonのビルトインのデータの型を使用していないのか](jp_why_apysc_doesnt_use_python_builtin_data_type.md)",  # noqa
+    "The `PathLineTo` class is the class to set a new line from the current position on a path.": "`PathLineTo`クラスは現在設定されている座標位置から新たな線のパスを描画します。",  # noqa
     ##################################################
-    "## What is the For class?": "## For クラスの概要",
-    ##################################################
-    "The `For` class is the apysc for loop class. It behaves like the Python built-in `for` keyword.": "`For`クラスはapyscのループ制御用のクラスです。このクラスはPythonのビルトインの`for`のキーワードのように動作します。",  # noqa
+    "Mainly, the `Path` class constructor or `draw_path` interfaces use this setting.": "主にこの設定は`Path`クラスのコンストラクタと`draw_path`メソッドのインターフェイスで使用されます。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
-    "The `For` class requires using the `with` statement. The `as` keyword value becomes the `Int` type index (an `i` variable)  or `String` type key.": "`For`クラスは`with`ステートメントと一緒に使用する必要があります。`as`のキーワードの値は`Int`型のインデックス（`i`の変数）もしくは`String`型のキーになります。",  # noqa
+    "The `PathLineTo` class constructor requires the `x` and `y` arguments.": "`PathLineTo`クラスのコンストラクタでは`x`と`y`の引数指定が必要となります。",  # noqa
+    ##################################################
+    "The `Path` class constructor or `draw_path` interfaces' `path_data_list` argument requires its instance.": "`Path`クラスのコンストラクタもしくは`draw_path`メソッドのインターフェイスの`path_data_list`引数でそのインスタンスが必要とされます。",  # noqa
+    ##################################################
+    "The following example sets the line drawing from x=50 and y=50 to x=150 and y=50 with the `PathLineTo` instance:": "以下のコード例ではx=50, y=50の位置からx=150, y=50の位置に向けて`PathLineTo`のインスタンスを設定して線の描画設定を行っています:",  # noqa
     ##################################################
-    "The following example draws the three rectangles in the `with For` block:": "以下のコード例では3つの四角を`with For`のブロック内で描画しています:",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=100, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=150, y=50),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=100, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=150, y=50),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_basic_usage/")\n```',  # noqa
     ##################################################
-    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=350, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\n\narr: ap.Array[int] = ap.Array(range(3))\ni: ap.Int\nwith ap.For(arr) as i:\n    sprite.graphics.draw_rect(x=i * 100 + 50, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="for_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=350, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\n\narr: ap.Array[int] = ap.Array(range(3))\ni: ap.Int\nwith ap.For(arr) as i:\n    sprite.graphics.draw_rect(x=i * 100 + 50, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="for_basic_usage/")\n```',  # noqa
+    "## Relative position setting": "## 相対座標設定",
     ##################################################
-    "The `For` class constructor's first argument accepts an `Array` or `Dictionary` value. If you pass a `Dictionary` value, the `as` keyword value becomes a `String` value, not `Int`\\.": "`For`クラスの第一引数は`Array`もしくは`Dictionary`クラスの値を受け付けます。もしも`Dictionary`の値を指定した場合、`as`のキーワードの値は`Int`の代わりに`String`の値になります。",  # noqa
+    "The constructor's `relative` optional argument changes its behavior.": "コンストラクタの`relative`のオプション引数はその挙動を変更します。",  # noqa
     ##################################################
-    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=250, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\n\ndict_val: ap.Dictionary = ap.Dictionary(\n    {"magenta": ap.String("#f0a"), "cyan": ap.String("#0af")}\n)\nkey: ap.String\nwith ap.For(dict_val) as key:\n    color: ap.String = dict_val[key]\n    sprite.graphics.begin_fill(color=color)\n    condition_1: ap.Boolean = key == "magenta"\n    condition_2: ap.Boolean = key == "cyan"\n    with ap.If(condition_1):\n        sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\n    with ap.Elif(condition_2):\n        sprite.graphics.draw_rect(x=150, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="for_basic_usage_with_dict/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=250, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\n\ndict_val: ap.Dictionary = ap.Dictionary(\n    {"magenta": ap.String("#f0a"), "cyan": ap.String("#0af")}\n)\nkey: ap.String\nwith ap.For(dict_val) as key:\n    color: ap.String = dict_val[key]\n    sprite.graphics.begin_fill(color=color)\n    condition_1: ap.Boolean = key == "magenta"\n    condition_2: ap.Boolean = key == "cyan"\n    with ap.If(condition_1):\n        sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\n    with ap.Elif(condition_2):\n        sprite.graphics.draw_rect(x=150, y=50, width=50, height=50)\n\nap.save_overall_html(dest_dir_path="for_basic_usage_with_dict/")\n```',  # noqa
+    "For example, if you set True to its argument, coordinates become relative.": "例として、もしその引数にTrueを指定した場合座標は相対座標として設定されます。",  # noqa
     ##################################################
-    "## See also": "## 関連資料",
+    "The default setting is False, and it becomes absolute.": "デフォルト値はFalseとなっており、この設定では絶対座標として扱われます。",  # noqa
     ##################################################
-    "- [Each branch instruction class's scope variables reverting setting](branch_instruction_variables_reverting_setting.md)": "- [分岐条件の各クラスのスコープ内変数の復元設定](jp_branch_instruction_variables_reverting_setting.md)",  # noqa
+    "The following example sets the relative setting and draws the line to the 50px under position from the current position:": "以下のコード例ではrelativeの設定を行い、現在の位置から50px下の位置に向けて線の描画を行っています:",  # noqa
     ##################################################
-    "  - Notes: the `For` class also has the same arguments and behaves in the same way.": "  - 特記事項: `For`クラスは同じ各引数を持っており、同じように動作します。",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=150, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=0, y=50, relative=True),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_relative/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=150, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=0, y=50, relative=True),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_relative/")\n```',  # noqa
     ##################################################
-    "## For API": "## For API",
+    "## PathLineTo class constructor API": "## PathLineTo クラスのコンストラクタのAPI",
     ##################################################
     '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
-    "The class to append for the (loop) expression.<hr>": "for（ループ）表現を追加するためのクラス。<hr>",
+    "Path data class for the SVG `line to` (L).<hr>": "SVGの特定座標に対する線（L）の描画のためのパスデータのクラスです。<hr>",  # noqa
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
-    "- `arr_or_dict`: Array or Dictionary": "- `arr_or_dict`: Array or Dictionary",
+    "- `x`: float or Number": "- `x`: float or Number",
+    ##################################################
+    "  - X-coordinate of the destination point.": "  - 終点のX座標。",
+    ##################################################
+    "- `y`: float or Number": "- `y`: float or Number",
     ##################################################
-    "  - Array or Dictionary instance to iterate.": "  - ループで使用するためのArray もしくは Dictionary クラスのインスタンス。",  # noqa
+    "  - Y-coordinate of the destination point.": "  - 終点のY座標。",
     ##################################################
-    "- `locals_`: dict or None, default None": "- `locals_`: dict or None, default None",  # noqa
+    "- `relative`: bool or Boolean, default False": "- `relative`: bool or Boolean, default False",  # noqa
     ##################################################
-    "  - Current scope's local variables. Set locals() value to this argument. If specified, this interface reverts all local scope VariableNameMixIn variables (like Int, Sprite) at the end of a `For` scope. This setting is useful when you don't want to update each variable by implementing the `For` scope.": "  - 現在のスコープのローカル変数。設定する場合にはlocals()関数の値をこの引数に指定してください。もし設定された場合にはこのいんたーふぇいろは`For`クラスによるスコープの終わりにVariableNameMixInを継承した各変数（IntやSpriteなど）の値を元の状態に復元します。この設定はもしも変数の値を`For`のスコープ内で更新したくない場合などに便利な時があります。",  # noqa
+    "  - A boolean value indicates whether the path coordinates are relative or not (absolute).": "  - パスの座標が相対座標として扱うかもしくは絶対座標として扱うかどうかの真偽値。",  # noqa
     ##################################################
-    "- `globals_`: dict or None, default None": "- `globals_`: dict or None, default None",  # noqa
+    "- `variable_name_suffix`: str, default ''": "- `variable_name_suffix`: str, default ''",  # noqa
     ##################################################
-    "  - Current scope's global variables. Set globals() value to this argument. This setting works the same way as the locals_ argument.": "  - 現在のスコープの各グローバル変数。設定する場合にはglobal()関数の値をこの引数に指定してください。この設定はlocals_引数と同じように動作します。",  # noqa
+    "  - A JavaScript variable name suffix string. This setting is sometimes useful for JavaScript debugging.": "  - JavaScript上の変数のサフィックスの設定です。この設定はJavaScriptのデバッグ時に役立つことがあります。",  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    '```py\n>>> import apysc as ap\n>>> arr: ap.Array = ap.Array(range(3))\n>>> with ap.For(arr) as i:\n...     ap.trace("Loop index is:", i)\n...\n```': '```py\n>>> import apysc as ap\n>>> arr: ap.Array = ap.Array(range(3))\n>>> with ap.For(arr) as i:\n...     ap.trace("Loop index is:", i)\n...\n```',  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage()\n>>> sprite: ap.Sprite = ap.Sprite()\n>>> sprite.graphics.line_style(color="#fff", thickness=3)\n>>> path: ap.Path = sprite.graphics.draw_path(\n...     path_data_list=[\n...         ap.PathMoveTo(x=0, y=50),\n...         ap.PathLineTo(x=50, y=50),\n...     ]\n... )\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage()\n>>> sprite: ap.Sprite = ap.Sprite()\n>>> sprite.graphics.line_style(color="#fff", thickness=3)\n>>> path: ap.Path = sprite.graphics.draw_path(\n...     path_data_list=[\n...         ap.PathMoveTo(x=0, y=50),\n...         ap.PathLineTo(x=50, y=50),\n...     ]\n... )\n```',  # noqa
+    ##################################################
+    "<hr>": "<hr>",
+    ##################################################
+    "**[References]**": "**[関連資料]**",
+    ##################################################
+    "- [Path class](https://simon-ritchie.github.io/apysc/en/path.html)": "- [Path クラス](https://simon-ritchie.github.io/apysc/jp/jp_path.html)",  # noqa
+    ##################################################
+    "- [Graphics draw_path interface](https://simon-ritchie.github.io/apysc/en/graphics_draw_path.html)": "- [Graphics クラスの draw_path インターフェイス](https://simon-ritchie.github.io/apysc/jp/jp_graphics_draw_path.html)",  # noqa
 }
```

### Comparing `apysc-2.8.9/apysc/_translation/jp/for_array_indices.py` & `apysc-3.0.0/apysc/_translation/jp/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/for_array_indices_and_values.py` & `apysc-3.0.0/apysc/_translation/jp/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/for_array_values.py` & `apysc-3.0.0/apysc/_translation/jp/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/for_dict_keys.py` & `apysc-3.0.0/apysc/_translation/jp/for_dict_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ##################################################
     "This class requires using the `with`-statement.": "このクラスは`with`ステートメントと共に使う必要があります。",  # noqa
     ##################################################
     "The `as`-keyword value becomes a `Dictionary`'s key.": "`as`キーワードの値は`Dictionary`のキーとなります。",  # noqa
     ##################################################
     "Also, this class requires the `dict_key_type` to specify a type of `Dictionary`'s key type.": "また、このクラスは`Dictionary`のキーの型を指定するための`dict_key_type`引数の指定が必要になります。",  # noqa
     ##################################################
-    "This type only accepts an apysc type, such as the `String`, `Int`, or `Boolean`.": "この型の指定は`String`や`Int`、`Boolean`といったapyscの型のみ受け付けます。",  # noqa
+    "This type only accepts an apysc type, such as the `String`, `Int`, `Number`, or `Boolean`.": "この型の指定は`String`や`Int`、`Number`、`Boolean`といったapyscの型のみ受け付けます。",  # noqa
     ##################################################
     '```py\n# runnable\nimport apysc as ap\n\nap.Stage(stage_width=0, stage_height=0, background_color="#333", stage_elem_id="stage")\n\ndict_: ap.Dictionary[ap.String, int] = ap.Dictionary(\n    {\n        ap.String("apple"): 120,\n        ap.String("orange"): 200,\n    }\n)\nkeys: ap.Array[ap.String] = ap.Array([])\nwith ap.ForDictKeys(dict_=dict_, dict_key_type=ap.String) as key:\n    keys.append(key)\nap.assert_arrays_equal(\n    keys,\n    ["apple", "orange"],\n)\n\nap.save_overall_html(dest_dir_path="for_dict_keys_basic_usage_1/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(stage_width=0, stage_height=0, background_color="#333", stage_elem_id="stage")\n\ndict_: ap.Dictionary[ap.String, int] = ap.Dictionary(\n    {\n        ap.String("apple"): 120,\n        ap.String("orange"): 200,\n    }\n)\nkeys: ap.Array[ap.String] = ap.Array([])\nwith ap.ForDictKeys(dict_=dict_, dict_key_type=ap.String) as key:\n    keys.append(key)\nap.assert_arrays_equal(\n    keys,\n    ["apple", "orange"],\n)\n\nap.save_overall_html(dest_dir_path="for_dict_keys_basic_usage_1/")\n```',  # noqa
     ##################################################
     "## See also": "## 関連資料",
     ##################################################
     "- [Each branch instruction class's scope variables reverting setting](branch_instruction_variables_reverting_setting.md)": "- [分岐条件の各クラスのスコープ内変数の復元設定](jp_branch_instruction_variables_reverting_setting.md)",  # noqa
     ##################################################
@@ -53,15 +53,15 @@
     ##################################################
     "- `dict_`: Dictionary[_DictKey, Any]": "- `dict_`: Dictionary[_DictKey, Any]",
     ##################################################
     "  - A dictionary to iterate.": "  - イテレーションで扱うための辞書。",
     ##################################################
     "- `dict_key_type`: Type[_DictKey]": "- `dict_key_type`: Type[_DictKey]",
     ##################################################
-    "  - A dictionary key type. This interface accepts hashable types, such as the `String`, `Int`, or `Boolean`.": "  - 辞書のキーの型。このインターフェイスはハッシュ化可能な`String`、`Int`、`Boolean`といった型のみ受け付けます。",  # noqa
+    "  - A dictionary key type. This interface accepts hashable types, such as the `String`, `Int`, `Number`, or `Boolean`.": "  - 辞書のキーの型。このインターフェイスは`String`、`Int`、`Number`、`Boolean`といったハッシュ化可能な型を受け付けます。",  # noqa
     ##################################################
     "- `locals_`: Optional[Dict[str, Any]], optional": "- `locals_`: Optional[Dict[str, Any]], optional",  # noqa
     ##################################################
     "  - Current scope's local variables. Set locals() value to this argument. If specified, this interface reverts all local scope VariableNameMixIn variables (like Int, Sprite) at the end of a with-statement scope. This setting is useful when you don't want to update each variable.": "  - 現在のスコープの各ローカル変数。この引数にはlocals()関数の返却値を設定してください。もしこの引数が指定された場合、このインターフェイスはローカルスコープのVariableNameMixInの各変数（例 : IntやSpriteなど）の値をwithステートメントの最後で復元します。この設定は各変数を更新したくない場合等に役立ちます。",  # noqa
     ##################################################
     "- `globals_`: Optional[Dict[str, Any]], optional": "- `globals_`: Optional[Dict[str, Any]], optional",  # noqa
     ##################################################
```

### Comparing `apysc-2.8.9/apysc/_translation/jp/fps.py` & `apysc-3.0.0/apysc/_translation/jp/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/fundamental_data_classes_value_interface.py` & `apysc-3.0.0/apysc/_translation/jp/fundamental_data_classes_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/get_bounds.py` & `apysc-3.0.0/apysc/_translation/jp/get_bounds.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/get_child_at.py` & `apysc-3.0.0/apysc/_translation/jp/get_child_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics.py` & `apysc-3.0.0/apysc/_translation/jp/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_fill_alpha.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_fill_color.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_flip_interfaces.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_flip_interfaces.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_line_alpha.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_line_color.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_line_dash_setting.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_line_dot_setting.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_line_round_dot_setting.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_line_thickness.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_rotation_around_center.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_rotation_around_point.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_scale_from_center.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_scale_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_scale_from_point.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_scale_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_base_skew.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_base_skew.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_begin_fill.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_begin_fill.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_clear.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_circle.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_circle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_dash_dotted_line.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_dash_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_dashed_line.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_dashed_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_dotted_line.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_ellipse.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_line.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_path.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_path.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_polygon.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_rect.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_round_dotted_line.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_round_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_round_rect.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_round_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_draw_triangle.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_draw_triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_line_style.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_line_style.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/graphics_move_to_and_line_to.py` & `apysc-3.0.0/apysc/_translation/jp/graphics_move_to_and_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/if.py` & `apysc-3.0.0/apysc/_translation/jp/if.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/import_conventions.py` & `apysc-3.0.0/apysc/_translation/jp/import_conventions.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/index.py` & `apysc-3.0.0/apysc/_translation/jp/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     ##################################################
     "## Branch instruction": "## 条件分岐の制御",
     ##################################################
     "```{toctree}\n:maxdepth: 1\nif\nelif\nelse\nbranch_instruction_variables_reverting_setting\nreturn\n```": "```{toctree}\n:maxdepth: 1\njp_if\njp_elif\njp_else\njp_branch_instruction_variables_reverting_setting\njp_return\n```",  # noqa
     ##################################################
     "## Loop": "## ループ",
     ##################################################
-    "```{toctree}\n:maxdepth: 1\nfor\nfor_array_indices\nfor_array_values\nfor_array_indices_and_values\nfor_dict_keys\ncontinue\nrange\n```": "```{toctree}\n:maxdepth: 1\njp_for\njp_for_array_indices\njp_for_array_values\njp_for_array_indices_and_values\njp_for_dict_keys\njp_continue\njp_range\n```",  # noqa
+    "```{toctree}\n:maxdepth: 1\nfor_array_indices\nfor_array_values\nfor_array_indices_and_values\nfor_dict_keys\nfor_dict_values\nfor_dict_keys_and_values\ncontinue\nrange\n```": "```{toctree}\n:maxdepth: 1\njp_for_array_indices\njp_for_array_values\njp_for_array_indices_and_values\njp_for_dict_keys\njp_for_dict_values\njp_for_dict_keys_and_values\njp_continue\njp_range\n```",  # noqa
     ##################################################
     "## Timer and enter-frame": "## タイマーとenter-frame",
     ##################################################
     "```{toctree}\n:maxdepth: 1\ntimer\ntimer_event\ntimer_delay\nfps\ntimer_repeat_count\ntimer_start_and_stop\ntimer_complete\ntimer_reset\nenter_frame\nunbind_enter_frame_and_unbind_enter_frame_all\n```": "```{toctree}\n:maxdepth: 1\njp_timer\njp_timer_event\njp_timer_delay\njp_fps\njp_timer_repeat_count\njp_timer_start_and_stop\njp_timer_complete\njp_timer_reset\njp_enter_frame\njp_unbind_enter_frame_and_unbind_enter_frame_all\n```",  # noqa
     ##################################################
     "## DateTime class": "## DateTime クラス",
     ##################################################
```

### Comparing `apysc-2.8.9/apysc/_translation/jp/int_and_number.py` & `apysc-3.0.0/apysc/_translation/jp/int_and_number.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/int_and_number_arithmetic_operations.py` & `apysc-3.0.0/apysc/_translation/jp/int_and_number_arithmetic_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/int_and_number_comparison_operations.py` & `apysc-3.0.0/apysc/_translation/jp/int_and_number_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/int_and_number_to_fixed.py` & `apysc-3.0.0/apysc/_translation/jp/int_and_number_to_fixed.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/line.py` & `apysc-3.0.0/apysc/_translation/jp/line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/math_max.py` & `apysc-3.0.0/apysc/_translation/jp/math_max.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/math_min.py` & `apysc-3.0.0/apysc/_translation/jp/math_min.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/math_trunc.py` & `apysc-3.0.0/apysc/_translation/jp/math_trunc.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/mouse_event_abstract.py` & `apysc-3.0.0/apysc/_translation/jp/mouse_event_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/mouse_event_basic.py` & `apysc-3.0.0/apysc/_translation/jp/mouse_event_basic.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/mousedown_and_mouseup.py` & `apysc-3.0.0/apysc/_translation/jp/mousedown_and_mouseup.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/mousemove.py` & `apysc-3.0.0/apysc/_translation/jp/mousemove.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/mouseover_and_mouseout.py` & `apysc-3.0.0/apysc/_translation/jp/mouseover_and_mouseout.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/num_children.py` & `apysc-3.0.0/apysc/_translation/jp/num_children.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path.py` & `apysc-3.0.0/apysc/_translation/jp/path.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_bezier_2d.py` & `apysc-3.0.0/apysc/_translation/jp/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_bezier_2d_continual.py` & `apysc-3.0.0/apysc/_translation/jp/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_bezier_3d.py` & `apysc-3.0.0/apysc/_translation/jp/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_bezier_3d_continual.py` & `apysc-3.0.0/apysc/_translation/jp/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_close.py` & `apysc-3.0.0/apysc/_translation/jp/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_horizontal.py` & `apysc-3.0.0/apysc/_translation/jp/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_line_to.py` & `apysc-3.0.0/apysc/_translation/jp/path_vertical.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 """This module is for the translation mapping data of the
 following document:
 
-Document file: path_line_to.md
+Document file: path_vertical.md
 Language: jp
 """
 
 from typing import Dict
 
 MAPPING: Dict[str, str] = {
     ##################################################
-    "# PathLineTo class": "# PathLineTo クラス",
+    "# PathVertical class": "# PathVertical クラス",
     ##################################################
-    "This page explains the `PathLineTo` class.": "このページでは`PathLineTo`クラスについて説明します。",
+    "This page explains the `PathVertical` class.": "このページでは`PathVertical`クラスについて説明します。",  # noqa
     ##################################################
     "## What class is this?": "## クラス概要",
     ##################################################
-    "The `PathLineTo` class is the class to set a new line from the current position on a path.": "`PathLineTo`クラスは現在設定されている座標位置から新たな線のパスを描画します。",  # noqa
+    "The `PathVertical` class is the class to set a new vertical line on a path.": "`PathVertical`クラスはパス上に新しい垂直の直線の設定を追加するためのクラスです。",  # noqa
+    ##################################################
+    "It simplifies an implementation if you need to draw a vertical line and not change a horizontal coordinate.": "この設定はもし垂直方向の線の描画のみが必要で水平方向の座標設定が不要な場合にコードの記述をシンプルにします。",  # noqa
     ##################################################
     "Mainly, the `Path` class constructor or `draw_path` interfaces use this setting.": "主にこの設定は`Path`クラスのコンストラクタと`draw_path`メソッドのインターフェイスで使用されます。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
-    "The `PathLineTo` class constructor requires the `x` and `y` arguments.": "`PathLineTo`クラスのコンストラクタでは`x`と`y`の引数指定が必要となります。",  # noqa
+    "The `PathVertical` class constructor requires only one argument, `y`.": "`PathVertical`クラスのコンストラクタでは`y`の引数指定のみ必要とします。",  # noqa
     ##################################################
     "The `Path` class constructor or `draw_path` interfaces' `path_data_list` argument requires its instance.": "`Path`クラスのコンストラクタもしくは`draw_path`メソッドのインターフェイスの`path_data_list`引数でそのインスタンスが必要とされます。",  # noqa
     ##################################################
-    "The following example sets the line drawing from x=50 and y=50 to x=150 and y=50 with the `PathLineTo` instance:": "以下のコード例ではx=50, y=50の位置からx=150, y=50の位置に向けて`PathLineTo`のインスタンスを設定して線の描画設定を行っています:",  # noqa
+    "The following example sets the y=150 coordinates and draws the vertical line from the y=50 coordinate:": "以下のコード例ではy=50の座標からy=150の座標に向けて垂直の直線を描画しています:",  # noqa
     ##################################################
-    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=100, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=150, y=50),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=100, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=150, y=50),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_basic_usage/")\n```',  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=200, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathVertical(y=150),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_vertical_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=200, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathVertical(y=150),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_vertical_basic_usage/")\n```',  # noqa
     ##################################################
     "## Relative position setting": "## 相対座標設定",
     ##################################################
     "The constructor's `relative` optional argument changes its behavior.": "コンストラクタの`relative`のオプション引数はその挙動を変更します。",  # noqa
     ##################################################
     "For example, if you set True to its argument, coordinates become relative.": "例として、もしその引数にTrueを指定した場合座標は相対座標として設定されます。",  # noqa
     ##################################################
     "The default setting is False, and it becomes absolute.": "デフォルト値はFalseとなっており、この設定では絶対座標として扱われます。",  # noqa
     ##################################################
-    "The following example sets the relative setting and draws the line to the 50px under position from the current position:": "以下のコード例ではrelativeの設定を行い、現在の位置から50px下の位置に向けて線の描画を行っています:",  # noqa
+    "The following example sets the relative setting and draws the line to the 50px under position from the current position:": "以下のコード例ではrelativeの設定をして現在の座標から垂直方向に50px下の位置に直線を描画しています:",  # noqa
     ##################################################
-    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=150, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=0, y=50, relative=True),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_relative/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=150, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathLineTo(x=0, y=50, relative=True),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_line_to_relative/")\n```',  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=150, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathVertical(y=50, relative=True),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_vertical_relative/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=100, stage_height=150, stage_elem_id="stage"\n)\npath: ap.Path = ap.Path(\n    path_data_list=[\n        ap.PathMoveTo(x=50, y=50),\n        ap.PathVertical(y=50, relative=True),\n    ],\n    line_color="#0af",\n    line_thickness=5,\n)\n\nap.save_overall_html(dest_dir_path="path_vertical_relative/")\n```',  # noqa
     ##################################################
-    "## PathLineTo class constructor API": "## PathLineTo クラスのコンストラクタのAPI",
+    "## PathVertical class constructor API": "## PathVertical クラスのコンストラクタのAPI",
     ##################################################
     '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
-    "Path data class for the SVG `line to` (L).<hr>": "SVGの特定座標に対する線（L）の描画のためのパスデータのクラスです。<hr>",  # noqa
+    "Path data class for the SVG `vertical line' (V).<hr>": "SVGの垂直方向への線（V）の描画のためのパスデータのクラスです。<hr>",  # noqa
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
-    "- `x`: float or Number": "- `x`: float or Number",
-    ##################################################
-    "  - X-coordinate of the destination point.": "  - 終点のX座標。",
-    ##################################################
     "- `y`: float or Number": "- `y`: float or Number",
     ##################################################
     "  - Y-coordinate of the destination point.": "  - 終点のY座標。",
     ##################################################
     "- `relative`: bool or Boolean, default False": "- `relative`: bool or Boolean, default False",  # noqa
     ##################################################
     "  - A boolean value indicates whether the path coordinates are relative or not (absolute).": "  - パスの座標が相対座標として扱うかもしくは絶対座標として扱うかどうかの真偽値。",  # noqa
@@ -67,15 +65,15 @@
     ##################################################
     "  - A JavaScript variable name suffix string. This setting is sometimes useful for JavaScript debugging.": "  - JavaScript上の変数のサフィックスの設定です。この設定はJavaScriptのデバッグ時に役立つことがあります。",  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage()\n>>> sprite: ap.Sprite = ap.Sprite()\n>>> sprite.graphics.line_style(color="#fff", thickness=3)\n>>> path: ap.Path = sprite.graphics.draw_path(\n...     path_data_list=[\n...         ap.PathMoveTo(x=0, y=50),\n...         ap.PathLineTo(x=50, y=50),\n...     ]\n... )\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage()\n>>> sprite: ap.Sprite = ap.Sprite()\n>>> sprite.graphics.line_style(color="#fff", thickness=3)\n>>> path: ap.Path = sprite.graphics.draw_path(\n...     path_data_list=[\n...         ap.PathMoveTo(x=0, y=50),\n...         ap.PathLineTo(x=50, y=50),\n...     ]\n... )\n```',  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage()\n>>> sprite: ap.Sprite = ap.Sprite()\n>>> sprite.graphics.line_style(color="#fff", thickness=3)\n>>> path: ap.Path = sprite.graphics.draw_path(\n...     path_data_list=[\n...         ap.PathMoveTo(x=0, y=50),\n...         ap.PathVertical(y=100),\n...     ]\n... )\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage()\n>>> sprite: ap.Sprite = ap.Sprite()\n>>> sprite.graphics.line_style(color="#fff", thickness=3)\n>>> path: ap.Path = sprite.graphics.draw_path(\n...     path_data_list=[\n...         ap.PathMoveTo(x=0, y=50),\n...         ap.PathVertical(y=100),\n...     ]\n... )\n```',  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[References]**": "**[関連資料]**",
     ##################################################
     "- [Path class](https://simon-ritchie.github.io/apysc/en/path.html)": "- [Path クラス](https://simon-ritchie.github.io/apysc/jp/jp_path.html)",  # noqa
     ##################################################
```

### Comparing `apysc-2.8.9/apysc/_translation/jp/path_move_to.py` & `apysc-3.0.0/apysc/_translation/jp/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/point2d.py` & `apysc-3.0.0/apysc/_translation/jp/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/polygon.py` & `apysc-3.0.0/apysc/_translation/jp/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/polyline.py` & `apysc-3.0.0/apysc/_translation/jp/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/quick_start.py` & `apysc-3.0.0/apysc/_translation/jp/quick_start.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/range.py` & `apysc-3.0.0/apysc/_translation/jp/range.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/recommended_type_checker_settings.py` & `apysc-3.0.0/apysc/_translation/jp/recommended_type_checker_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/rectangle.py` & `apysc-3.0.0/apysc/_translation/jp/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/rectangle_geom.py` & `apysc-3.0.0/apysc/_translation/jp/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/remove_children.py` & `apysc-3.0.0/apysc/_translation/jp/remove_children.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/return.py` & `apysc-3.0.0/apysc/_translation/jp/return.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/save_overall_html.py` & `apysc-3.0.0/apysc/_translation/jp/save_overall_html.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/sequential_animation.py` & `apysc-3.0.0/apysc/_translation/jp/sequential_animation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/set_debug_mode.py` & `apysc-3.0.0/apysc/_translation/jp/set_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/sprite.py` & `apysc-3.0.0/apysc/_translation/jp/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/stage.py` & `apysc-3.0.0/apysc/_translation/jp/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/string.py` & `apysc-3.0.0/apysc/_translation/jp/string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/string_addition_and_multiplication.py` & `apysc-3.0.0/apysc/_translation/jp/string_addition_and_multiplication.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/string_comparison_operations.py` & `apysc-3.0.0/apysc/_translation/jp/string_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/string_lstrip.py` & `apysc-3.0.0/apysc/_translation/jp/string_lstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/string_rstrip.py` & `apysc-3.0.0/apysc/_translation/jp/string_rstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/string_split.py` & `apysc-3.0.0/apysc/_translation/jp/string_split.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/string_strip.py` & `apysc-3.0.0/apysc/_translation/jp/string_strip.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/svg_text.py` & `apysc-3.0.0/apysc/_translation/jp/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/svg_text_span.py` & `apysc-3.0.0/apysc/_translation/jp/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timedelta.py` & `apysc-3.0.0/apysc/_translation/jp/timedelta.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timedelta_days.py` & `apysc-3.0.0/apysc/_translation/jp/timedelta_days.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timedelta_total_seconds.py` & `apysc-3.0.0/apysc/_translation/jp/timedelta_total_seconds.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timer.py` & `apysc-3.0.0/apysc/_translation/jp/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timer_complete.py` & `apysc-3.0.0/apysc/_translation/jp/timer_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timer_delay.py` & `apysc-3.0.0/apysc/_translation/jp/timer_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timer_event.py` & `apysc-3.0.0/apysc/_translation/jp/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timer_repeat_count.py` & `apysc-3.0.0/apysc/_translation/jp/timer_repeat_count.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timer_reset.py` & `apysc-3.0.0/apysc/_translation/jp/timer_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/timer_start_and_stop.py` & `apysc-3.0.0/apysc/_translation/jp/timer_start_and_stop.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/to_string.py` & `apysc-3.0.0/apysc/_translation/jp/to_string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/trace.py` & `apysc-3.0.0/apysc/_translation/jp/trace.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/triangle.py` & `apysc-3.0.0/apysc/_translation/jp/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py` & `apysc-3.0.0/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/unset_debug_mode.py` & `apysc-3.0.0/apysc/_translation/jp/unset_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/variable_name_suffix.py` & `apysc-3.0.0/apysc/_translation/jp/variable_name_suffix.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/what_apysc_can_do.py` & `apysc-3.0.0/apysc/_translation/jp/what_apysc_can_do.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py` & `apysc-3.0.0/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/_delete.py` & `apysc-3.0.0/apysc/_type/_delete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/_return.py` & `apysc-3.0.0/apysc/_type/_return.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/any_value.py` & `apysc-3.0.0/apysc/_type/any_value.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/array.py` & `apysc-3.0.0/apysc/_type/array.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/attr_linking_mixin.py` & `apysc-3.0.0/apysc/_type/attr_linking_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py` & `apysc-3.0.0/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/blank_object_mixin.py` & `apysc-3.0.0/apysc/_type/blank_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/boolean.py` & `apysc-3.0.0/apysc/_type/boolean.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     InitializeForLoopKeyOrValueInterface,
 )
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.hashable_interface import HashableInterface
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.int import Int
 from apysc._type.revert_mixin import RevertMixIn
+from apysc._type.to_number_mixin import ToNumberMixIn
 from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._type.variable_name_mixin import VariableNameMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Boolean(
@@ -30,16 +31,16 @@
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
     InitializeForLoopKeyOrValueInterface,
     HashableInterface,
+    ToNumberMixIn,
 ):
-
     """
     Boolean class for the apysc library.
 
     Notes
     -----
     The Bool class is the alias of the Boolean, and it behaves
     the same as the Boolean class.
```

### Comparing `apysc-2.8.9/apysc/_type/copy_mixin.py` & `apysc-3.0.0/apysc/_type/copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/deleted_object_mixin.py` & `apysc-3.0.0/apysc/_type/deleted_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/dictionary.py` & `apysc-3.0.0/apysc/_type/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/expression_string.py` & `apysc-3.0.0/apysc/_type/expression_string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/initial_substitution_exp_mixin.py` & `apysc-3.0.0/apysc/_type/initial_substitution_exp_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/initialize_locals_and_globals_mixin.py` & `apysc-3.0.0/apysc/_type/initialize_locals_and_globals_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/int.py` & `apysc-3.0.0/apysc/_type/number.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-"""Class implementation of integer.
+"""Class implementation of the floating-point number value.
 """
 
+from typing import Any
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._loop.initialize_for_loop_key_or_value_interface import (
     InitializeForLoopKeyOrValueInterface,
@@ -12,217 +13,197 @@
 from apysc._type.hashable_interface import HashableInterface
 from apysc._type.number_value_mixin import NumberValueMixIn
 from apysc._type.to_fixed_mixin import ToFixedMixIn
 from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._validation import arg_validation_decos
 
 
-class Int(
-    NumberValueMixIn[int, "Int"],
+class Number(
+    NumberValueMixIn[float, "Number"],
     InitializeForLoopKeyOrValueInterface,
     ToStringMixIn,
     ToFixedMixIn,
     HashableInterface,
 ):
     """
-    Integer class for the apysc library.
+    Floating point number class for the apysc library.
+
+    Notes
+    -----
+    The `Float` class is the alias of the Number,
+    and it behaves the same as the Number class.
 
     References
     ----------
     - Int and Number
         - https://simon-ritchie.github.io/apysc/en/int_and_number.html
     - Int and Number common arithmetic operations
         - https://simon-ritchie.github.io/apysc/en/int_and_number_arithmetic_operations.html  # noqa
     - Int and Number common comparison operations
         - https://simon-ritchie.github.io/apysc/en/int_and_number_comparison_operations.html  # noqa
 
     Examples
     --------
     >>> import apysc as ap
-    >>> int_val: ap.Int = ap.Int(10)
-    >>> int_val
-    Int(10)
+    >>> number: ap.Number = ap.Number(10.5)
+    >>> number
+    Number(10.5)
 
-    >>> int_val == 10
+    >>> number == 10.5
     Boolean(True)
 
-    >>> int_val == ap.Int(10)
+    >>> number == ap.Number(10.5)
     Boolean(True)
 
-    >>> int_val >= 10
+    >>> number >= 10.5
     Boolean(True)
 
-    >>> int_val += 10
-    >>> int_val
-    Int(20)
-
-    >>> int_val = ap.Int(10.5)
-    >>> int_val
-    Int(10)
+    >>> number += 10.3
+    >>> number
+    Number(20.8)
     """
 
     @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         value: Union[int, float, NumberValueMixIn],
         *,
         variable_name_suffix: str = "",
         skip_init_substitution_expression_appending: bool = False,
     ) -> None:
         """
-        Integer class for apysc library.
+        Floating point number class for apysc library.
 
         Parameters
         ----------
         value : int or float or Int or Number
-            Initial integer value. If the `float` or `Number`
-            value is specified, this class casts it to an integer.
+            Initial floating point number value. This class
+            casts it to float if you specify int or Int value.
         variable_name_suffix : str, default ''
             A JavaScript variable name suffix string.
             This setting is sometimes useful for JavaScript debugging.
         skip_init_substitution_expression_appending : bool, default False
             A boolean indicates whether to skip an initial substitution
             expression or not. This class uses this option internally.
 
+        Notes
+        -----
+        The `Float` class is the alias of the Number, and it behaves
+        the same as the Number class.
+
         References
         ----------
         - Int and Number
             - https://simon-ritchie.github.io/apysc/en/int_and_number.html
         - Int and Number common arithmetic operations
             - https://simon-ritchie.github.io/apysc/en/int_and_number_arithmetic_operations.html  # noqa
         - Int and Number common comparison operations
             - https://simon-ritchie.github.io/apysc/en/int_and_number_comparison_operations.html  # noqa
 
         Examples
         --------
         >>> import apysc as ap
-        >>> int_val: ap.Int = ap.Int(10)
-        >>> int_val
-        Int(10)
+        >>> number: ap.Number = ap.Number(10.5)
+        >>> number
+        Number(10.5)
 
-        >>> int_val == 10
+        >>> number == 10.5
         Boolean(True)
 
-        >>> int_val == ap.Int(10)
+        >>> number == ap.Number(10.5)
         Boolean(True)
 
-        >>> int_val >= 10
+        >>> number >= 10.5
         Boolean(True)
 
-        >>> int_val += 10
-        >>> int_val
-        Int(20)
-
-        >>> int_val = ap.Int(10.5)
-        >>> int_val
-        Int(10)
+        >>> number += 10.3
+        >>> number
+        Number(20.8)
         """
         from apysc._converter import cast
         from apysc._expression import expression_variables_util
         from apysc._expression import var_names
         from apysc._expression.event_handler_scope import TemporaryNotHandlerScope
-        from apysc._type import type_util
 
         with TemporaryNotHandlerScope():
-            is_number_specified: bool = type_util.is_number(value=value)
-            TYPE_NAME: str = var_names.INT
+            TYPE_NAME: str = var_names.NUMBER
             self.variable_name = expression_variables_util.get_next_variable_name(
                 type_name=TYPE_NAME
             )
-            super(Int, self).__init__(
+            super(Number, self).__init__(
                 value=value,
                 type_name=TYPE_NAME,
                 variable_name_suffix=variable_name_suffix,
             )
-            self._value = cast.to_int_from_float(int_or_float=self.value)
+            self._value = cast.to_float_from_int(int_or_float=self.value)
             self._append_constructor_expression()
-            self._append_cast_expression(is_number_specified=is_number_specified)
 
         self._append_initial_substitution_expression_if_in_handler_scope(
             skip_appending=skip_init_substitution_expression_appending,
         )
 
     @final
-    @add_debug_info_setting(module_name=__name__)
-    def _append_cast_expression(self, *, is_number_specified: bool) -> None:
-        """
-        Append integer cast (Math.trunc) expression.
-
-        Parameters
-        ----------
-        is_number_specified : bool
-            Boolean value whether a specified value is Number
-            instance or not.
-        """
-        import apysc as ap
-
-        if not is_number_specified:
-            return
-        expression: str = (
-            f"{self.variable_name} = Math.trunc({self.variable_name}, 10);"
-        )
-        ap.append_js_expression(expression=expression)
-
-    @final
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     def _set_value_and_skip_expression_appending(
-        self, *, value: Union[int, float, NumberValueMixIn]
+        self, *, value: Union[int, float, Any]
     ) -> None:
         """
         Update value attribute and skip expression appending.
 
         Parameters
         ----------
         value : int or float or Int or Number
-            Any number value to set. This interface casts that
-            value to an integer if float or number value is specified.
+            Any number value to set. If a float or Number
+            value is specified, this interface casts its
+            value to an integer.
         """
         from apysc._converter import cast
 
         if isinstance(value, NumberValueMixIn):
-            value._value = cast.to_int_from_float(int_or_float=value._value)
-            value_: Union[int, float, NumberValueMixIn] = value._value
+            value._value = cast.to_float_from_int(int_or_float=value._value)
+            value_ = value._value
         else:
-            value = cast.to_int_from_float(int_or_float=value)
+            value = cast.to_float_from_int(int_or_float=value)
             value_ = value
-        self._value = value_  # type: ignore
+        self._value = value_
 
     def __repr__(self) -> str:
         """
         Get a representation string of this instance.
 
         Returns
         -------
         repr_str : str
             Representation string of this instance.
         """
         if not hasattr(self, "_value"):
-            repr_str: str = "Int(0)"
+            repr_str: str = "Number(0)"
         else:
-            repr_str = f"Int({self._value})"
+            repr_str = f"Number({self._value})"
         return repr_str
 
     @classmethod
     @final
-    def _initialize_for_loop_key_or_value(cls) -> "Int":
+    def _initialize_for_loop_key_or_value(cls) -> "Number":
         """
         Initialize this instance for a loop key or value.
 
         Returns
         -------
-        int_value : Int
-            An initialized integer value.
+        num_value : Number
+            An initialized number value.
         """
-        return Int(0)
+        return Number(0)
 
     @final
     def __hash__(self) -> int:
         """
         Get a hashed value.
 
         Returns
         -------
         hashed_value : int
             A hashed value.
         """
-        return int(self._value)
+        return hash(self._value)
```

### Comparing `apysc-2.8.9/apysc/_type/number.py` & `apysc-3.0.0/apysc/_loop/for_dict_values.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,195 +1,187 @@
-"""Class implementation of the floating-point number value.
+"""The loop implementation class for the `ap.Dictionary` values.
 """
 
 from typing import Any
-from typing import Union
+from typing import Dict
+from typing import Generic
+from typing import Optional
+from typing import Type
+from typing import TypeVar
 
 from typing_extensions import final
 
+from apysc._expression.get_last_scope_interface import GetLastScopeInterface
+from apysc._expression.indent_num import Indent
+from apysc._expression.last_scope import LastScope
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.for_loop_exit_mixin import ForLoopExitMixIn
 from apysc._loop.initialize_for_loop_key_or_value_interface import (
     InitializeForLoopKeyOrValueInterface,
 )
-from apysc._type.number_value_mixin import NumberValueMixIn
-from apysc._type.to_fixed_mixin import ToFixedMixIn
-from apysc._type.to_string_mixin import ToStringMixIn
+from apysc._type.dictionary import Dictionary
+from apysc._type.initialize_locals_and_globals_mixin import (
+    InitializeLocalsAndGlobalsMixIn,
+)
+from apysc._type.string import String
 from apysc._validation import arg_validation_decos
 
+_DictValue = TypeVar("_DictValue", bound=InitializeForLoopKeyOrValueInterface)
 
-class Number(
-    NumberValueMixIn[float, "Number"],
-    InitializeForLoopKeyOrValueInterface,
-    ToStringMixIn,
-    ToFixedMixIn,
+
+class ForDictValues(
+    ForLoopExitMixIn,
+    GetLastScopeInterface,
+    InitializeLocalsAndGlobalsMixIn,
+    Generic[_DictValue],
 ):
     """
-    Floating point number class for the apysc library.
-
-    Notes
-    -----
-    The `Float` class is the alias of the Number,
-    and it behaves the same as the Number class.
+    The loop implementation class for the `ap.Dictionary` values.
 
     References
     ----------
-    - Int and Number
-        - https://simon-ritchie.github.io/apysc/en/int_and_number.html
-    - Int and Number common arithmetic operations
-        - https://simon-ritchie.github.io/apysc/en/int_and_number_arithmetic_operations.html  # noqa
-    - Int and Number common comparison operations
-        - https://simon-ritchie.github.io/apysc/en/int_and_number_comparison_operations.html  # noqa
+    - ForDictValues class
+        - https://simon-ritchie.github.io/apysc/en/for_dict_values.html
 
-    Examples
-    --------
+    References
+    ----------
     >>> import apysc as ap
-    >>> number: ap.Number = ap.Number(10.5)
-    >>> number
-    Number(10.5)
-
-    >>> number == 10.5
-    Boolean(True)
-
-    >>> number == ap.Number(10.5)
-    Boolean(True)
-
-    >>> number >= 10.5
-    Boolean(True)
-
-    >>> number += 10.3
-    >>> number
-    Number(20.8)
+
+    >>> _ = ap.Stage(
+    ...     stage_width=250,
+    ...     stage_height=150,
+    ...     background_color="#333",
+    ...     stage_elem_id="stage",
+    ... )
+    >>> dict_: ap.Dictionary[str, ap.Number] = ap.Dictionary(
+    ...     {"a": ap.Number(50), "b": ap.Number(150)},
+    ... )
+    >>> with ap.ForDictValues(dict_=dict_, dict_value_type=ap.Number) as value:
+    ...     _ = ap.Rectangle(x=value, y=50, width=50, height=50, fill_color="#0af")
+    ...
     """
 
-    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
-    @arg_validation_decos.is_builtin_string(arg_position_index=2, optional=False)
+    _dict: Dictionary[Any, _DictValue]
+    _dict_value_type: Type[_DictValue]
+    _variable_name_suffix: str
+
+    @final
+    @arg_validation_decos.is_apysc_dict(arg_position_index=1)
+    @arg_validation_decos.is_initialize_for_loop_key_or_value_interface_subclass(
+        arg_position_index=2,
+    )
+    @arg_validation_decos.is_builtin_string(arg_position_index=5, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
-        value: Union[int, float, NumberValueMixIn],
+        dict_: Dictionary[Any, _DictValue],
+        dict_value_type: Type[_DictValue],
         *,
+        locals_: Optional[Dict[str, Any]] = None,
+        globals_: Optional[Dict[str, Any]] = None,
         variable_name_suffix: str = "",
-        skip_init_substitution_expression_appending: bool = False,
     ) -> None:
         """
-        Floating point number class for apysc library.
+        The loop implementation class for the `ap.Dictionary` values.
 
         Parameters
         ----------
-        value : int or float or Int or Number
-            Initial floating point number value. This class
-            casts it to float if you specify int or Int value.
-        variable_name_suffix : str, default ''
+        dict_ : Dictionary[Any, _DictValue]
+            A dictionary to iterate.
+        dict_value_type : Type[_DictValue]
+            A dictionary value type. This interface accepts
+            `InitializeForLoopKeyOrValueInterface` subclasses,
+            such as the `Int`, `String`, or `Rectangle`.
+        locals_ : Optional[Dict[str, Any]], optional
+            Current scope's local variables. Set locals()
+            value to this argument. If specified, this interface
+            reverts all local scope VariableNameMixIn
+            variables (like Int, Sprite) at the end of a with-statement
+            scope. This setting is useful when you don't want to
+            update each variable.
+        globals_ : Optional[Dict[str, Any]], optional
+            Current scope's global variables. Set globals()
+            value to this argument. This setting works
+            the same way as the locals_ argument.
+        variable_name_suffix : str, optional
             A JavaScript variable name suffix string.
             This setting is sometimes useful for JavaScript debugging.
-        skip_init_substitution_expression_appending : bool, default False
-            A boolean indicates whether to skip an initial substitution
-            expression or not. This class uses this option internally.
-
-        Notes
-        -----
-        The `Float` class is the alias of the Number, and it behaves
-        the same as the Number class.
 
         References
         ----------
-        - Int and Number
-            - https://simon-ritchie.github.io/apysc/en/int_and_number.html
-        - Int and Number common arithmetic operations
-            - https://simon-ritchie.github.io/apysc/en/int_and_number_arithmetic_operations.html  # noqa
-        - Int and Number common comparison operations
-            - https://simon-ritchie.github.io/apysc/en/int_and_number_comparison_operations.html  # noqa
+        - ForDictValues class
+            - https://simon-ritchie.github.io/apysc/en/for_dict_values.html
 
-        Examples
-        --------
+        References
+        ----------
         >>> import apysc as ap
-        >>> number: ap.Number = ap.Number(10.5)
-        >>> number
-        Number(10.5)
-
-        >>> number == 10.5
-        Boolean(True)
-
-        >>> number == ap.Number(10.5)
-        Boolean(True)
-
-        >>> number >= 10.5
-        Boolean(True)
-
-        >>> number += 10.3
-        >>> number
-        Number(20.8)
-        """
-        from apysc._converter import cast
-        from apysc._expression import expression_variables_util
-        from apysc._expression import var_names
-        from apysc._expression.event_handler_scope import TemporaryNotHandlerScope
-
-        with TemporaryNotHandlerScope():
-            TYPE_NAME: str = var_names.NUMBER
-            self.variable_name = expression_variables_util.get_next_variable_name(
-                type_name=TYPE_NAME
-            )
-            super(Number, self).__init__(
-                value=value,
-                type_name=TYPE_NAME,
-                variable_name_suffix=variable_name_suffix,
-            )
-            self._value = cast.to_float_from_int(int_or_float=self.value)
-            self._append_constructor_expression()
 
-        self._append_initial_substitution_expression_if_in_handler_scope(
-            skip_appending=skip_init_substitution_expression_appending,
-        )
+        >>> _ = ap.Stage(
+        ...     stage_width=250,
+        ...     stage_height=150,
+        ...     background_color="#333",
+        ...     stage_elem_id="stage",
+        ... )
+        >>> dict_: ap.Dictionary[str, ap.Number] = ap.Dictionary(
+        ...     {"a": ap.Number(50), "b": ap.Number(150)},
+        ... )
+        >>> with ap.ForDictValues(dict_=dict_, dict_value_type=ap.Number) as value:
+        ...     _ = ap.Rectangle(x=value, y=50, width=50, height=50, fill_color="#0af")
+        ...
+        """
+        self._initialize_locals_and_globals(locals_, globals_=globals_)
+        self._dict = dict_
+        self._dict_value_type = dict_value_type
+        self._variable_name_suffix = variable_name_suffix
+        self._indent = Indent()
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
-    def _set_value_and_skip_expression_appending(
-        self, *, value: Union[int, float, Any]
-    ) -> None:
+    def _get_last_scope(self) -> LastScope:
         """
-        Update value attribute and skip expression appending.
-
-        Parameters
-        ----------
-        value : int or float or Int or Number
-            Any number value to set. If a float or Number
-            value is specified, this interface casts its
-            value to an integer.
-        """
-        from apysc._converter import cast
-
-        if isinstance(value, NumberValueMixIn):
-            value._value = cast.to_float_from_int(int_or_float=value._value)
-            value_ = value._value
-        else:
-            value = cast.to_float_from_int(int_or_float=value)
-            value_ = value
-        self._value = value_
-
-    def __repr__(self) -> str:
-        """
-        Get a representation string of this instance.
+        Get a target last scope value.
 
         Returns
         -------
-        repr_str : str
-            Representation string of this instance.
+        last_scope : LastScope
+            A target last scope.
         """
-        if not hasattr(self, "_value"):
-            repr_str: str = "Number(0)"
-        else:
-            repr_str = f"Number({self._value})"
-        return repr_str
+        return LastScope.FOR_DICT_VALUES
 
-    @classmethod
     @final
-    def _initialize_for_loop_key_or_value(cls) -> "Number":
+    @add_debug_info_setting(module_name=__name__)
+    def __enter__(self) -> _DictValue:
         """
-        Initialize this instance for a loop key or value.
+        The entering method for the beginning of with-statement.
 
         Returns
         -------
-        num_value : Number
-            An initialized number value.
+        dict_value : _DictValue
+            A dictionary value of iteration.
         """
-        return Number(0)
+        import apysc as ap
+        from apysc._loop import loop_count
+        from apysc._type import revert_mixin
+        from apysc._validation.variable_name_validation import (
+            validate_variable_name_interface_type,
+        )
+
+        loop_count.increment_current_loop_count()
+        self._snapshot_name = revert_mixin.make_snapshots_of_each_scope_vars(
+            locals_=self._locals, globals_=self._globals
+        )
+        dict_value: _DictValue = (
+            self._dict_value_type._initialize_for_loop_key_or_value()
+        )
+        dict_value_variable_name: str = validate_variable_name_interface_type(
+            instance=dict_value,
+        ).variable_name
+
+        dict_key: String = String("", variable_name_suffix=self._variable_name_suffix)
+        expression: str = (
+            f"for ({dict_key.variable_name} in {self._dict.variable_name}) {{"
+            f"\n  {dict_value_variable_name} = {self._dict.variable_name}"
+            f"[{dict_key.variable_name}];"
+        )
+        ap.append_js_expression(expression=expression)
+
+        self._indent.__enter__()
+        return dict_value
```

### Comparing `apysc-2.8.9/apysc/_type/number_value_mixin.py` & `apysc-3.0.0/apysc/_type/number_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/py_builtin_iter_disabling_mixin.py` & `apysc-3.0.0/apysc/_type/py_builtin_iter_disabling_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/revert_interface.py` & `apysc-3.0.0/apysc/_type/revert_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/revert_mixin.py` & `apysc-3.0.0/apysc/_type/revert_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/string.py` & `apysc-3.0.0/apysc/_type/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from apysc._type.hashable_interface import HashableInterface
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.revert_mixin import RevertMixIn
 from apysc._type.string_lstrip_mixin import StringLStripMixIn
 from apysc._type.string_rstrip_mixin import StringRStripMixIn
 from apysc._type.string_split_mixin import StringSplitMixIn
 from apysc._type.string_strip_mixin import StringStripMixIn
+from apysc._type.to_number_mixin import ToNumberMixIn
 from apysc._type.variable_name_mixin import VariableNameMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class String(
     StringSplitMixIn,
@@ -34,14 +35,15 @@
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
     InitializeForLoopKeyOrValueInterface,
     HashableInterface,
+    ToNumberMixIn,
 ):
     """
     String class for apysc library.
 
     Notes
     -----
     The `Str` class is the alias of `String`.
```

### Comparing `apysc-2.8.9/apysc/_type/string_lstrip_mixin.py` & `apysc-3.0.0/apysc/_type/string_lstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/string_rstrip_mixin.py` & `apysc-3.0.0/apysc/_type/string_rstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/string_split_mixin.py` & `apysc-3.0.0/apysc/_type/string_split_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/string_strip_mixin.py` & `apysc-3.0.0/apysc/_type/string_strip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/to_fixed_mixin.py` & `apysc-3.0.0/apysc/_type/to_fixed_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/to_string_mixin.py` & `apysc-3.0.0/apysc/_type/to_string_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/type_util.py` & `apysc-3.0.0/apysc/_type/type_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/value_util.py` & `apysc-3.0.0/apysc/_type/value_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,30 +86,33 @@
     value_str += "}"
     return value_str
 
 
 def _validate_dict_key_type(*, key: Any) -> None:
     """
     Validate whether a dictionary key type is the `int`, `str`, `float`,
-    `bool`, `ap.Int`, `ap.String`, or `ap.Boolean`.
+    `bool`, `ap.Int`, `ap.Number`, `ap.String`, or `ap.Boolean`.
 
     Parameters
     ----------
     key : *
         Dictionary key to validate.
 
     Raises
     ------
     TypeError
         If a key-type isn't the `int`, `str`, `float`, `bool`, `ap.Int`,
-        `ap.String`, or `ap.Boolean`.
+        `ap.Number`, `ap.String`, or `ap.Boolean`.
     """
     import apysc as ap
 
-    if isinstance(key, (str, int, float, bool, ap.String, ap.Int, ap.Boolean)):
+    if isinstance(
+        key,
+        (str, int, float, bool, ap.String, ap.Int, ap.Number, ap.Boolean),
+    ):
         return
     raise TypeError(
         "Dictionary key type only supports `int`, `str`, `float`,"
         f"`bool`, `ap.Int`, `ap.String`, or `ap.Boolean`: {type(key)}"
     )
```

### Comparing `apysc-2.8.9/apysc/_type/variable_name_mixin.py` & `apysc-3.0.0/apysc/_type/variable_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/variable_name_suffix_attr_or_var_mixin.py` & `apysc-3.0.0/apysc/_type/variable_name_suffix_attr_or_var_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/variable_name_suffix_mixin.py` & `apysc-3.0.0/apysc/_type/variable_name_suffix_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_type/variable_name_suffix_utils.py` & `apysc-3.0.0/apysc/_type/variable_name_suffix_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/arg_validation_decos.py` & `apysc-3.0.0/apysc/_validation/arg_validation_decos.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/bool_validation.py` & `apysc-3.0.0/apysc/_validation/bool_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/color_validation.py` & `apysc-3.0.0/apysc/_validation/color_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/display_validation.py` & `apysc-3.0.0/apysc/_validation/display_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/event_validation.py` & `apysc-3.0.0/apysc/_validation/event_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/geom_validation.py` & `apysc-3.0.0/apysc/_validation/geom_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/handler_validation.py` & `apysc-3.0.0/apysc/_validation/handler_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/matrix_data_validation.py` & `apysc-3.0.0/apysc/_validation/matrix_data_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/number_validation.py` & `apysc-3.0.0/apysc/_validation/number_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/parent_validation.py` & `apysc-3.0.0/apysc/_validation/parent_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/path_validation.py` & `apysc-3.0.0/apysc/_validation/path_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/string_validation.py` & `apysc-3.0.0/apysc/_validation/string_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/validation_common_utils.py` & `apysc-3.0.0/apysc/_validation/validation_common_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc/_validation/variable_name_validation.py` & `apysc-3.0.0/apysc/_validation/variable_name_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.9/apysc.egg-info/PKG-INFO` & `apysc-3.0.0/apysc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 2.8.9
+Version: 3.0.0
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-2.8.9/apysc.egg-info/SOURCES.txt` & `apysc-3.0.0/apysc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -351,20 +351,21 @@
 apysc/_lint_and_doc/lint_and_doc_hash_util.py
 apysc/_lint_and_doc/translation_mapping_utils.py
 apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
 apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
 apysc/_lint_and_doc/fixed_translation_mapping/jp.py
 apysc/_loop/__init__.py
 apysc/_loop/_continue.py
-apysc/_loop/_for.py
 apysc/_loop/_range.py
 apysc/_loop/for_array_indices.py
 apysc/_loop/for_array_indices_and_values.py
 apysc/_loop/for_array_values.py
 apysc/_loop/for_dict_keys.py
+apysc/_loop/for_dict_keys_and_values.py
+apysc/_loop/for_dict_values.py
 apysc/_loop/for_loop_exit_mixin.py
 apysc/_loop/initialize_for_loop_key_or_value_interface.py
 apysc/_loop/loop_count.py
 apysc/_math/__init__.py
 apysc/_math/math.py
 apysc/_math/max_mixin.py
 apysc/_math/min_mixin.py
@@ -486,19 +487,20 @@
 apysc/_translation/jp/draw_interfaces_abstract.py
 apysc/_translation/jp/easing_enum.py
 apysc/_translation/jp/elif.py
 apysc/_translation/jp/ellipse.py
 apysc/_translation/jp/else.py
 apysc/_translation/jp/enter_frame.py
 apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
-apysc/_translation/jp/for.py
 apysc/_translation/jp/for_array_indices.py
 apysc/_translation/jp/for_array_indices_and_values.py
 apysc/_translation/jp/for_array_values.py
 apysc/_translation/jp/for_dict_keys.py
+apysc/_translation/jp/for_dict_keys_and_values.py
+apysc/_translation/jp/for_dict_values.py
 apysc/_translation/jp/fps.py
 apysc/_translation/jp/fundamental_data_classes_value_interface.py
 apysc/_translation/jp/get_bounds.py
 apysc/_translation/jp/get_child_at.py
 apysc/_translation/jp/graphics.py
 apysc/_translation/jp/graphics_base_fill_alpha.py
 apysc/_translation/jp/graphics_base_fill_color.py
@@ -626,14 +628,15 @@
 apysc/_type/revert_mixin.py
 apysc/_type/string.py
 apysc/_type/string_lstrip_mixin.py
 apysc/_type/string_rstrip_mixin.py
 apysc/_type/string_split_mixin.py
 apysc/_type/string_strip_mixin.py
 apysc/_type/to_fixed_mixin.py
+apysc/_type/to_number_mixin.py
 apysc/_type/to_string_mixin.py
 apysc/_type/type_name_mixin.py
 apysc/_type/type_util.py
 apysc/_type/value_util.py
 apysc/_type/variable_name_mixin.py
 apysc/_type/variable_name_suffix_attr_or_var_mixin.py
 apysc/_type/variable_name_suffix_mixin.py
```

