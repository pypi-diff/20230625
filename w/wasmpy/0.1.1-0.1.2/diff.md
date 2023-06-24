# Comparing `tmp/wasmpy-0.1.1.tar.gz` & `tmp/wasmpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-0.1.1.tar", last modified: Sat Jun 24 19:03:53 2023, max compression
+gzip compressed data, was "wasmpy-0.1.2.tar", last modified: Sat Jun 24 23:33:09 2023, max compression
```

## Comparing `wasmpy-0.1.1.tar` & `wasmpy-0.1.2.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.903138 wasmpy-0.1.1/
--rw-rw-rw-   0        0        0     1068 2023-06-15 12:12:24.000000 wasmpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      143 2023-06-24 18:22:33.000000 wasmpy-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2445 2023-06-24 19:03:53.903138 wasmpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1568 2023-06-24 18:50:52.000000 wasmpy-0.1.1/README.md
--rw-rw-rw-   0        0        0     4922 2023-06-24 09:33:46.000000 wasmpy-0.1.1/opcodes.py
--rw-rw-rw-   0        0        0       42 2023-06-24 19:03:53.906562 wasmpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     5270 2023-06-24 19:03:26.000000 wasmpy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.761533 wasmpy-0.1.1/wasmpy/
--rw-rw-rw-   0        0        0      106 2023-06-23 12:23:39.000000 wasmpy-0.1.1/wasmpy/__init__.py
--rw-rw-rw-   0        0        0     1689 2023-06-23 11:11:55.000000 wasmpy-0.1.1/wasmpy/hooks.py
--rw-rw-rw-   0        0        0    14893 2023-06-24 07:42:57.000000 wasmpy-0.1.1/wasmpy/instructions.py
--rw-rw-rw-   0        0        0     3097 2023-06-23 11:13:55.000000 wasmpy-0.1.1/wasmpy/module.py
--rw-rw-rw-   0        0        0     1085 2023-06-22 15:47:07.000000 wasmpy-0.1.1/wasmpy/native.py
--rw-rw-rw-   0        0        0     5286 2023-06-23 11:12:14.000000 wasmpy-0.1.1/wasmpy/sections.py
--rw-rw-rw-   0        0        0     2421 2023-06-21 19:25:53.000000 wasmpy-0.1.1/wasmpy/types.py
--rw-rw-rw-   0        0        0     2029 2023-06-23 11:12:52.000000 wasmpy-0.1.1/wasmpy/values.py
--rw-rw-rw-   0        0        0     8283 2023-06-24 08:07:05.000000 wasmpy-0.1.1/wasmpy/win_x86.cpp
-drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.773825 wasmpy-0.1.1/wasmpy/x86/
--rw-rw-rw-   0        0        0      217 2023-06-24 06:23:55.000000 wasmpy-0.1.1/wasmpy/x86/helpers.cpp
--rw-rw-rw-   0        0        0      128 2023-06-24 07:49:47.000000 wasmpy-0.1.1/wasmpy/x86/helpers.h
-drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.893447 wasmpy-0.1.1/wasmpy/x86/instructions/
--rw-rw-rw-   0        0        0       16 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/drop
--rw-rw-rw-   0        0        0       76 2023-06-24 05:34:10.000000 wasmpy-0.1.1/wasmpy/x86/instructions/drop.asm
--rw-rw-rw-   0        0        0       15 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.const
--rw-rw-rw-   0        0        0       74 2023-06-24 09:25:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.const.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.eq
--rw-rw-rw-   0        0        0      182 2023-06-24 06:48:21.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f32.eq.asm
--rw-rw-rw-   0        0        0       27 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f64.const
--rw-rw-rw-   0        0        0      124 2023-06-24 09:31:58.000000 wasmpy-0.1.1/wasmpy/x86/instructions/f64.const.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.add
--rw-rw-rw-   0        0        0      143 2023-06-24 05:51:43.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.add.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.and
--rw-rw-rw-   0        0        0      143 2023-06-24 05:54:00.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.and.asm
--rw-rw-rw-   0        0        0       37 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.clz
--rw-rw-rw-   0        0        0      178 2023-06-24 05:50:35.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.clz.asm
--rw-rw-rw-   0        0        0       15 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.const
--rw-rw-rw-   0        0        0       74 2023-06-24 09:25:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.const.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ctz
--rw-rw-rw-   0        0        0      154 2023-06-24 05:50:56.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ctz.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_s
--rw-rw-rw-   0        0        0      177 2023-06-24 05:52:39.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_s.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_u
--rw-rw-rw-   0        0        0      176 2023-06-24 05:52:55.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.div_u.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eq
--rw-rw-rw-   0        0        0      182 2023-06-24 05:38:00.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eq.asm
--rw-rw-rw-   0        0        0       28 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eqz
--rw-rw-rw-   0        0        0      143 2023-06-24 05:37:40.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.eqz.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_s
--rw-rw-rw-   0        0        0      183 2023-06-24 05:40:32.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_s.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_u
--rw-rw-rw-   0        0        0      183 2023-06-24 05:40:50.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ge_u.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_s
--rw-rw-rw-   0        0        0      182 2023-06-24 05:39:22.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_s.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_u
--rw-rw-rw-   0        0        0      182 2023-06-24 05:39:41.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.gt_u.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_s
--rw-rw-rw-   0        0        0      183 2023-06-24 05:39:57.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_s.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_u
--rw-rw-rw-   0        0        0      183 2023-06-24 05:40:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.le_u.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_s
--rw-rw-rw-   0        0        0      182 2023-06-24 05:38:36.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_s.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_u
--rw-rw-rw-   0        0        0      182 2023-06-24 05:39:02.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.lt_u.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.mul
--rw-rw-rw-   0        0        0      144 2023-06-24 05:52:17.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.mul.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ne
--rw-rw-rw-   0        0        0      184 2023-06-24 05:38:20.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.ne.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.or
--rw-rw-rw-   0        0        0      142 2023-06-24 05:54:14.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.or.asm
--rw-rw-rw-   0        0        0       21 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.popcnt
--rw-rw-rw-   0        0        0      100 2023-06-24 05:51:20.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.popcnt.asm
--rw-rw-rw-   0        0        0       42 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_s
--rw-rw-rw-   0        0        0      191 2023-06-24 05:53:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_s.asm
--rw-rw-rw-   0        0        0       42 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_u
--rw-rw-rw-   0        0        0      190 2023-06-24 05:53:43.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rem_u.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotl
--rw-rw-rw-   0        0        0      142 2023-06-24 05:55:49.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotl.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotr
--rw-rw-rw-   0        0        0      142 2023-06-24 05:56:08.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.rotr.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shl
--rw-rw-rw-   0        0        0      162 2023-06-24 05:54:48.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shl.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_s
--rw-rw-rw-   0        0        0      162 2023-06-24 05:55:11.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_s.asm
--rw-rw-rw-   0        0        0       36 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_u
--rw-rw-rw-   0        0        0      162 2023-06-24 05:55:32.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.shr_u.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.sub
--rw-rw-rw-   0        0        0      143 2023-06-24 05:52:01.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.sub.asm
--rw-rw-rw-   0        0        0        9 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.wrap_i64
--rw-rw-rw-   0        0        0       48 2023-06-24 06:35:32.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.wrap_i64.asm
--rw-rw-rw-   0        0        0       30 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.xor
--rw-rw-rw-   0        0        0      143 2023-06-24 05:54:30.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i32.xor.asm
--rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.add
--rw-rw-rw-   0        0        0      246 2023-06-24 06:33:44.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.add.asm
--rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.and
--rw-rw-rw-   0        0        0      246 2023-06-24 06:34:24.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.and.asm
--rw-rw-rw-   0        0        0       69 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.clz
--rw-rw-rw-   0        0        0      331 2023-06-24 06:32:38.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.clz.asm
--rw-rw-rw-   0        0        0       27 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.const
--rw-rw-rw-   0        0        0      124 2023-06-24 09:31:58.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.const.asm
--rw-rw-rw-   0        0        0       59 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ctz
--rw-rw-rw-   0        0        0      295 2023-06-24 06:33:00.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ctz.asm
--rw-rw-rw-   0        0        0       54 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eq
--rw-rw-rw-   0        0        0      268 2023-06-24 05:44:08.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eq.asm
--rw-rw-rw-   0        0        0       39 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eqz
--rw-rw-rw-   0        0        0      200 2023-06-24 05:43:48.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.eqz.asm
--rw-rw-rw-   0        0        0       33 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_s
--rw-rw-rw-   0        0        0      169 2023-06-24 06:36:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_s.asm
--rw-rw-rw-   0        0        0       11 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_u
--rw-rw-rw-   0        0        0       58 2023-06-24 06:36:41.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.extend_i32_u.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_s
--rw-rw-rw-   0        0        0      282 2023-06-24 05:47:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_s.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_u
--rw-rw-rw-   0        0        0      282 2023-06-24 05:47:34.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ge_u.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_s
--rw-rw-rw-   0        0        0      281 2023-06-24 05:45:53.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_s.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_u
--rw-rw-rw-   0        0        0      281 2023-06-24 05:46:13.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.gt_u.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_s
--rw-rw-rw-   0        0        0      282 2023-06-24 05:46:31.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_s.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_u
--rw-rw-rw-   0        0        0      282 2023-06-24 05:46:52.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.le_u.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_s
--rw-rw-rw-   0        0        0      281 2023-06-24 05:44:47.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_s.asm
--rw-rw-rw-   0        0        0       56 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_u
--rw-rw-rw-   0        0        0      281 2023-06-24 05:45:20.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.lt_u.asm
--rw-rw-rw-   0        0        0       54 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ne
--rw-rw-rw-   0        0        0      265 2023-06-24 05:44:26.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.ne.asm
--rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.or
--rw-rw-rw-   0        0        0      244 2023-06-24 06:34:47.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.or.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.popcnt
--rw-rw-rw-   0        0        0      186 2023-06-24 06:33:26.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.popcnt.asm
--rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.sub
--rw-rw-rw-   0        0        0      246 2023-06-24 06:34:02.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.sub.asm
--rw-rw-rw-   0        0        0       53 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.xor
--rw-rw-rw-   0        0        0      246 2023-06-24 06:35:05.000000 wasmpy-0.1.1/wasmpy/x86/instructions/i64.xor.asm
--rw-rw-rw-   0        0        0      106 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/select
--rw-rw-rw-   0        0        0      488 2023-06-24 05:37:04.000000 wasmpy-0.1.1/wasmpy/x86/instructions/select.asm
-drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.899568 wasmpy-0.1.1/wasmpy/x86/instructions/x64/
--rw-rw-rw-   0        0        0       87 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.get
--rw-rw-rw-   0        0        0      398 2023-06-24 08:53:55.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.get.asm
--rw-rw-rw-   0        0        0      100 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.set
--rw-rw-rw-   0        0        0      453 2023-06-24 08:54:49.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.set.asm
--rw-rw-rw-   0        0        0      133 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.tee
--rw-rw-rw-   0        0        0      614 2023-06-24 08:55:03.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.tee.asm
-drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.903138 wasmpy-0.1.1/wasmpy/x86/instructions/x86/
--rw-rw-rw-   0        0        0       81 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.get
--rw-rw-rw-   0        0        0      398 2023-06-24 09:03:25.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.get.asm
--rw-rw-rw-   0        0        0       90 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.set
--rw-rw-rw-   0        0        0      453 2023-06-24 09:03:43.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.set.asm
--rw-rw-rw-   0        0        0      123 2023-06-24 19:02:19.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.tee
--rw-rw-rw-   0        0        0      614 2023-06-24 09:03:57.000000 wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.tee.asm
--rw-rw-rw-   0        0        0     1193 2023-06-24 07:47:40.000000 wasmpy-0.1.1/wasmpy/x86/opcodes.h
-drwxrwxrwx   0        0        0        0 2023-06-24 19:03:53.771318 wasmpy-0.1.1/wasmpy.egg-info/
--rw-rw-rw-   0        0        0     2445 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4933 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 19:03:53.000000 wasmpy-0.1.1/wasmpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.427096 wasmpy-0.1.2/
+-rw-rw-rw-   0        0        0     1068 2023-06-15 12:12:24.000000 wasmpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-06-24 18:22:33.000000 wasmpy-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2445 2023-06-24 23:33:09.427096 wasmpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1568 2023-06-24 18:50:52.000000 wasmpy-0.1.2/README.md
+-rw-rw-rw-   0        0        0     4975 2023-06-24 22:12:53.000000 wasmpy-0.1.2/opcodes.py
+-rw-rw-rw-   0        0        0       42 2023-06-24 23:33:09.427096 wasmpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     5360 2023-06-24 23:32:18.000000 wasmpy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.270573 wasmpy-0.1.2/wasmpy/
+-rw-rw-rw-   0        0        0      106 2023-06-23 12:23:39.000000 wasmpy-0.1.2/wasmpy/__init__.py
+-rw-rw-rw-   0        0        0     1689 2023-06-23 11:11:55.000000 wasmpy-0.1.2/wasmpy/hooks.py
+-rw-rw-rw-   0        0        0    14893 2023-06-24 07:42:57.000000 wasmpy-0.1.2/wasmpy/instructions.py
+-rw-rw-rw-   0        0        0     3097 2023-06-24 21:59:04.000000 wasmpy-0.1.2/wasmpy/module.py
+-rw-rw-rw-   0        0        0     1085 2023-06-22 15:47:07.000000 wasmpy-0.1.2/wasmpy/native.py
+-rw-rw-rw-   0        0        0     5286 2023-06-23 11:12:14.000000 wasmpy-0.1.2/wasmpy/sections.py
+-rw-rw-rw-   0        0        0     2421 2023-06-21 19:25:53.000000 wasmpy-0.1.2/wasmpy/types.py
+-rw-rw-rw-   0        0        0     2029 2023-06-23 11:12:52.000000 wasmpy-0.1.2/wasmpy/values.py
+-rw-rw-rw-   0        0        0     8283 2023-06-24 23:27:15.000000 wasmpy-0.1.2/wasmpy/win_x86.cpp
+drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.287310 wasmpy-0.1.2/wasmpy/x86/
+-rw-rw-rw-   0        0        0      217 2023-06-24 06:23:55.000000 wasmpy-0.1.2/wasmpy/x86/helpers.cpp
+-rw-rw-rw-   0        0        0      128 2023-06-24 23:03:29.000000 wasmpy-0.1.2/wasmpy/x86/helpers.h
+drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.413246 wasmpy-0.1.2/wasmpy/x86/instructions/
+-rw-rw-rw-   0        0        0       16 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/drop
+-rw-rw-rw-   0        0        0       76 2023-06-24 05:34:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/drop.asm
+-rw-rw-rw-   0        0        0       16 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.const
+-rw-rw-rw-   0        0        0       81 2023-06-24 22:35:34.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.const.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.eq
+-rw-rw-rw-   0        0        0      210 2023-06-24 22:35:42.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.eq.asm
+-rw-rw-rw-   0        0        0       28 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f64.const
+-rw-rw-rw-   0        0        0      131 2023-06-24 22:35:50.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f64.const.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.add
+-rw-rw-rw-   0        0        0      150 2023-06-24 22:29:16.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.add.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.and
+-rw-rw-rw-   0        0        0      150 2023-06-24 22:35:57.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.and.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.clz
+-rw-rw-rw-   0        0        0      199 2023-06-24 22:36:17.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.clz.asm
+-rw-rw-rw-   0        0        0       16 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.const
+-rw-rw-rw-   0        0        0       81 2023-06-24 22:36:20.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.const.asm
+-rw-rw-rw-   0        0        0       33 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ctz
+-rw-rw-rw-   0        0        0      175 2023-06-24 22:36:23.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ctz.asm
+-rw-rw-rw-   0        0        0       41 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_s
+-rw-rw-rw-   0        0        0      184 2023-06-24 22:36:28.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_s.asm
+-rw-rw-rw-   0        0        0       41 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_u
+-rw-rw-rw-   0        0        0      183 2023-06-24 22:36:32.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_u.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eq
+-rw-rw-rw-   0        0        0      210 2023-06-24 22:37:09.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eq.asm
+-rw-rw-rw-   0        0        0       32 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eqz
+-rw-rw-rw-   0        0        0      171 2023-06-24 22:37:12.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eqz.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_s
+-rw-rw-rw-   0        0        0      211 2023-06-24 22:37:16.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_s.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_u
+-rw-rw-rw-   0        0        0      211 2023-06-24 22:37:19.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_u.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_s
+-rw-rw-rw-   0        0        0      210 2023-06-24 22:39:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_s.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_u
+-rw-rw-rw-   0        0        0      210 2023-06-24 22:39:15.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_u.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_s
+-rw-rw-rw-   0        0        0      211 2023-06-24 22:39:18.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_s.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_u
+-rw-rw-rw-   0        0        0      211 2023-06-24 22:39:22.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_u.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_s
+-rw-rw-rw-   0        0        0      210 2023-06-24 22:39:26.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_s.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_u
+-rw-rw-rw-   0        0        0      210 2023-06-24 22:39:29.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_u.asm
+-rw-rw-rw-   0        0        0       32 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.mul
+-rw-rw-rw-   0        0        0      151 2023-06-24 22:39:33.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.mul.asm
+-rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ne
+-rw-rw-rw-   0        0        0      212 2023-06-24 22:39:36.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ne.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.or
+-rw-rw-rw-   0        0        0      149 2023-06-24 22:39:40.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.or.asm
+-rw-rw-rw-   0        0        0       23 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.popcnt
+-rw-rw-rw-   0        0        0      114 2023-06-24 22:39:43.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.popcnt.asm
+-rw-rw-rw-   0        0        0       43 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_s
+-rw-rw-rw-   0        0        0      198 2023-06-24 22:39:46.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_s.asm
+-rw-rw-rw-   0        0        0       43 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_u
+-rw-rw-rw-   0        0        0      197 2023-06-24 22:39:50.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_u.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotl
+-rw-rw-rw-   0        0        0      149 2023-06-24 22:39:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotl.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotr
+-rw-rw-rw-   0        0        0      149 2023-06-24 22:39:57.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotr.asm
+-rw-rw-rw-   0        0        0       37 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shl
+-rw-rw-rw-   0        0        0      169 2023-06-24 22:40:01.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shl.asm
+-rw-rw-rw-   0        0        0       37 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_s
+-rw-rw-rw-   0        0        0      169 2023-06-24 22:40:05.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_s.asm
+-rw-rw-rw-   0        0        0       37 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_u
+-rw-rw-rw-   0        0        0      169 2023-06-24 22:40:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_u.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.sub
+-rw-rw-rw-   0        0        0      150 2023-06-24 22:40:14.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.sub.asm
+-rw-rw-rw-   0        0        0       10 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.wrap_i64
+-rw-rw-rw-   0        0        0       55 2023-06-24 22:40:17.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.wrap_i64.asm
+-rw-rw-rw-   0        0        0       31 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.xor
+-rw-rw-rw-   0        0        0      150 2023-06-24 22:40:21.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.xor.asm
+-rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.add
+-rw-rw-rw-   0        0        0      253 2023-06-24 22:40:33.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.add.asm
+-rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.and
+-rw-rw-rw-   0        0        0      253 2023-06-24 22:40:36.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.and.asm
+-rw-rw-rw-   0        0        0       74 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.clz
+-rw-rw-rw-   0        0        0      366 2023-06-24 22:40:40.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.clz.asm
+-rw-rw-rw-   0        0        0       28 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.const
+-rw-rw-rw-   0        0        0      131 2023-06-24 22:40:42.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.const.asm
+-rw-rw-rw-   0        0        0       64 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ctz
+-rw-rw-rw-   0        0        0      330 2023-06-24 22:40:48.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ctz.asm
+-rw-rw-rw-   0        0        0       58 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eq
+-rw-rw-rw-   0        0        0      296 2023-06-24 22:40:51.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eq.asm
+-rw-rw-rw-   0        0        0       43 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eqz
+-rw-rw-rw-   0        0        0      228 2023-06-24 22:40:55.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eqz.asm
+-rw-rw-rw-   0        0        0       38 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_s
+-rw-rw-rw-   0        0        0      204 2023-06-24 22:40:58.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_s.asm
+-rw-rw-rw-   0        0        0       14 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_u
+-rw-rw-rw-   0        0        0       79 2023-06-24 22:41:02.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_u.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_s
+-rw-rw-rw-   0        0        0      310 2023-06-24 22:41:05.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_s.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_u
+-rw-rw-rw-   0        0        0      310 2023-06-24 22:41:09.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_u.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_s
+-rw-rw-rw-   0        0        0      309 2023-06-24 22:41:13.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_s.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_u
+-rw-rw-rw-   0        0        0      309 2023-06-24 22:41:16.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_u.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_s
+-rw-rw-rw-   0        0        0      310 2023-06-24 22:41:20.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_s.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_u
+-rw-rw-rw-   0        0        0      310 2023-06-24 22:41:23.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_u.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_s
+-rw-rw-rw-   0        0        0      309 2023-06-24 22:41:27.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_s.asm
+-rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_u
+-rw-rw-rw-   0        0        0      309 2023-06-24 22:41:31.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_u.asm
+-rw-rw-rw-   0        0        0       58 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ne
+-rw-rw-rw-   0        0        0      293 2023-06-24 22:41:34.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ne.asm
+-rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.or
+-rw-rw-rw-   0        0        0      251 2023-06-24 22:41:37.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.or.asm
+-rw-rw-rw-   0        0        0       44 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.popcnt
+-rw-rw-rw-   0        0        0      214 2023-06-24 22:41:41.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.popcnt.asm
+-rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.sub
+-rw-rw-rw-   0        0        0      253 2023-06-24 22:41:44.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.sub.asm
+-rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.xor
+-rw-rw-rw-   0        0        0      253 2023-06-24 22:41:48.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.xor.asm
+-rw-rw-rw-   0        0        0      108 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/select
+-rw-rw-rw-   0        0        0      502 2023-06-24 22:41:51.000000 wasmpy-0.1.2/wasmpy/x86/instructions/select.asm
+drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.417137 wasmpy-0.1.2/wasmpy/x86/instructions/x64/
+-rw-rw-rw-   0        0        0       89 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.get
+-rw-rw-rw-   0        0        0      412 2023-06-24 22:35:15.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.get.asm
+-rw-rw-rw-   0        0        0      102 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.set
+-rw-rw-rw-   0        0        0      467 2023-06-24 22:35:21.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.set.asm
+-rw-rw-rw-   0        0        0      137 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.tee
+-rw-rw-rw-   0        0        0      642 2023-06-24 22:35:25.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.tee.asm
+drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.427096 wasmpy-0.1.2/wasmpy/x86/instructions/x86/
+-rw-rw-rw-   0        0        0       83 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.get
+-rw-rw-rw-   0        0        0      412 2023-06-24 22:42:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.get.asm
+-rw-rw-rw-   0        0        0       92 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.set
+-rw-rw-rw-   0        0        0      467 2023-06-24 22:42:13.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.set.asm
+-rw-rw-rw-   0        0        0      127 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.tee
+-rw-rw-rw-   0        0        0      642 2023-06-24 22:42:17.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.tee.asm
+-rw-rw-rw-   0        0        0     1193 2023-06-24 07:47:40.000000 wasmpy-0.1.2/wasmpy/x86/opcodes.h
+drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.285804 wasmpy-0.1.2/wasmpy.egg-info/
+-rw-rw-rw-   0        0        0     2445 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4933 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/top_level.txt
```

### Comparing `wasmpy-0.1.1/LICENSE` & `wasmpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/PKG-INFO` & `wasmpy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactions between WebAssembly and Python
 Home-page: https://github.com/olivi-r/wasmpy
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wasmpy-0.1.1/README.md` & `wasmpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/opcodes.py` & `wasmpy-0.1.2/opcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
         "i64.reinterpret_f64",
         "f32.reinterpret_i32",
         "f64.reinterpret_i64",
         offset=0x41,
     )
 )
 
+prefixed = {"local.get": "localidx += 10;\n\t\t\t"}
 
 consumes = {
     "local.get": 4,
     "local.set": 4,
     "local.tee": 4,
     "i32.const": 4,
     "i64.const": 8,
```

### Comparing `wasmpy-0.1.1/setup.py` & `wasmpy-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,17 +61,19 @@
             out.writelines(
                 (
                     "// auto-generated\n\n",
                     '#include "opcodes.h"\n',
                     '#include "helpers.h"\n\n',
                     "bytes decodeFunc(bytes buf, char plat)\n{\n\t",
                     "std::vector<bytes> insts = {};\n\t",
+                    "int localidx;\n\t",
                     "for (size_t i = 0; i < buf.size(); i++)\n\t{\n\t\t",
-                    "int localidx = buf.at(i + 4) << 24 | buf.at(i + 3) << 16 | buf.at(i + 2) << 8 | buf.at(i + 1);\n\t\t",
-                    "localidx *= 10;\n\t\t",
+                    "if (i < buf.size() - 4)\n\t\t{\n\t\t\t"
+                    "localidx = buf.at(i + 4) << 24 | buf.at(i + 3) << 16 | buf.at(i + 2) << 8 | buf.at(i + 1);\n\t\t\t",
+                    "localidx *= 10;\n\t\t}\n\t\t",
                     "switch (buf.at(i))\n\t\t{\n\t\t",
                 )
             )
 
             if bits == 8:
                 extra = listdir("wasmpy/x86/instructions/x64")
 
@@ -80,29 +82,28 @@
 
             for file in listdir("wasmpy/x86/instructions") + extra:
                 if os.path.isdir(file):
                     continue
 
                 inst = os.path.basename(file)
 
-                if os.path.splitext(file)[1].lower() != ".asm":
+                if inst in opcodes.opcodes:
                     with open(file, "rb") as fp:
                         data = ", ".join(str(i) for i in fp.read())
 
                     # alter binary data of instructions that take arguments
                     if inst in opcodes.replacements:
                         for replacement in opcodes.replacements[inst]:
                             data = data.replace(*replacement)
 
-                    out.writelines(
-                        (
-                            f"case {opcodes.opcodes[inst]}:\n\t\t\t",
-                            f"insts.push_back({{{data}}});\n\t\t\t",
-                        )
-                    )
+                    out.write(f"case {opcodes.opcodes[inst]}:\n\t\t\t")
+                    if inst in opcodes.prefixed:
+                        out.write(opcodes.prefixed[inst])
+
+                    out.write(f"insts.push_back({{{data}}});\n\t\t\t")
 
                     if inst in opcodes.consumes:
                         out.write(f"i += {opcodes.consumes[inst]};\n\t\t\t")
 
                     out.write("break;\n\n\t\t")
 
             out.writelines(
@@ -123,15 +124,15 @@
 
 
 with open("README.md", "r") as fp:
     description = fp.read()
 
 setuptools.setup(
     name="wasmpy",
-    version="0.1.1",
+    version="0.1.2",
     author="Olivia Ryan",
     author_email="olivia.r.dev@gmail.com",
     description="Interactions between WebAssembly and Python",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/olivi-r/wasmpy",
     packages=["wasmpy"],
@@ -146,15 +147,15 @@
             py_limited_api=True,
         )
     ],
     options={"bdist_wheel": {"py_limited_api": "cp36"}},
     cmdclass={
         "assemble": assemble,
         "build_ext": build_ext,
-        "genopcodes": gen_opcodes,
+        "gen_opcodes": gen_opcodes,
     },
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Assembly",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

### Comparing `wasmpy-0.1.1/wasmpy/hooks.py` & `wasmpy-0.1.2/wasmpy/hooks.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/instructions.py` & `wasmpy-0.1.2/wasmpy/instructions.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/module.py` & `wasmpy-0.1.2/wasmpy/module.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/native.py` & `wasmpy-0.1.2/wasmpy/native.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/sections.py` & `wasmpy-0.1.2/wasmpy/sections.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/types.py` & `wasmpy-0.1.2/wasmpy/types.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/values.py` & `wasmpy-0.1.2/wasmpy/values.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/win_x86.cpp` & `wasmpy-0.1.2/wasmpy/win_x86.cpp`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy/x86/instructions/x64/local.tee.asm` & `wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.tee.asm`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 pop ax
 shl eax, 16
 pop ax
 mov ecx, eax
 push cx
 shr ecx, 16
 push cx
-push word 2
+push strict word 2
 push rbp
 mov rcx, rsp
 mov rsp, rbp
 mov rbp, rcx
 sub rsp, 0xff00ff
 push ax
 shr eax, 16
 push ax
-push word 2
+push strict word 2
 mov rsp, rbp
 pop rbp
 jmp end
 v64:
 pop ax
 shl eax, 16
 pop ax
@@ -33,23 +33,23 @@
 mov ebx, ecx
 push bx
 shr ebx, 16
 push bx
 push dx
 shr edx, 16
 push dx
-push word 4
+push strict word 4
 push rbp
 mov rdx, rsp
 mov rsp, rbp
 mov rbp, rdx
 sub rsp, 0xff00ff
 push cx
 shr ecx, 16
 push cx
 push ax
 shr eax, 16
 push ax
-push word 4
+push strict word 4
 mov rsp, rbp
 pop rbp
 end:
```

### Comparing `wasmpy-0.1.1/wasmpy/x86/instructions/x86/local.tee.asm` & `wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.tee.asm`

 * *Files 17% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 pop ax
 shl eax, 16
 pop ax
 mov ecx, eax
 push cx
 shr ecx, 16
 push cx
-push word 2
+push strict word 2
 push ebp
 mov ecx, esp
 mov esp, ebp
 mov ebp, ecx
 sub esp, 0xff00ff
 push ax
 shr eax, 16
 push ax
-push word 2
+push strict word 2
 mov esp, ebp
 pop ebp
 jmp end
 v64:
 pop ax
 shl eax, 16
 pop ax
@@ -33,23 +33,23 @@
 mov ebx, ecx
 push bx
 shr ebx, 16
 push bx
 push dx
 shr edx, 16
 push dx
-push word 4
+push strict word 4
 push ebp
 mov edx, esp
 mov esp, ebp
 mov ebp, edx
 sub esp, 0xff00ff
 push cx
 shr ecx, 16
 push cx
 push ax
 shr eax, 16
 push ax
-push word 4
+push strict word 4
 mov esp, ebp
 pop ebp
 end:
```

### Comparing `wasmpy-0.1.1/wasmpy/x86/opcodes.h` & `wasmpy-0.1.2/wasmpy/x86/opcodes.h`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.1/wasmpy.egg-info/PKG-INFO` & `wasmpy-0.1.2/wasmpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactions between WebAssembly and Python
 Home-page: https://github.com/olivi-r/wasmpy
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wasmpy-0.1.1/wasmpy.egg-info/SOURCES.txt` & `wasmpy-0.1.2/wasmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

