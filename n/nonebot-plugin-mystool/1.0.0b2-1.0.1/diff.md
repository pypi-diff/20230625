# Comparing `tmp/nonebot_plugin_mystool-1.0.0b2.tar.gz` & `tmp/nonebot_plugin_mystool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-1.0.0b2.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-1.0.1.tar", max compression
```

## Comparing `nonebot_plugin_mystool-1.0.0b2.tar` & `nonebot_plugin_mystool-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     4110 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/README.md
--rw-r--r--   0        0        0     1324 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     1997 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     4494 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    12132 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/data_model.py
--rw-r--r--   0        0        0    21315 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    11767 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/game_sign_api.py
--rw-r--r--   0        0        0     5467 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/good_image.py
--rw-r--r--   0        0        0     1959 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0     9562 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    21993 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/myb_missions_api.py
--rw-r--r--   0        0        0    23357 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0    10775 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plugin_data.py
--rw-r--r--   0        0        0     8912 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    63231 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/simple_api.py
--rw-r--r--   0        0        0     2244 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_check.py
--rw-r--r--   0        0        0    11313 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_data.py
--rw-r--r--   0        0        0    10283 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-25 11:38:30.508511 nonebot_plugin_mystool-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4016 2023-06-25 11:38:30.508511 nonebot_plugin_mystool-1.0.1/README.md
+-rw-r--r--   0        0        0     1317 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2056 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     4438 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    12132 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/data_model.py
+-rw-r--r--   0        0        0    21256 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    11767 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/game_sign_api.py
+-rw-r--r--   0        0        0     5467 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/good_image.py
+-rw-r--r--   0        0        0     1959 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0     9516 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    21993 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/myb_missions_api.py
+-rw-r--r--   0        0        0    23451 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0    10768 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/plugin_data.py
+-rw-r--r--   0        0        0     8858 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    62920 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/simple_api.py
+-rw-r--r--   0        0        0     2244 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/user_check.py
+-rw-r--r--   0        0        0    11313 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/user_data.py
+-rw-r--r--   0        0        0    10283 2023-06-25 11:38:30.512511 nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.0.1/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/LICENSE` & `nonebot_plugin_mystool-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/README.md` & `nonebot_plugin_mystool-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,212 +46,206 @@
 000002d0: 6c61 7374 2d63 6f6d 6d69 742f 4c6a 7a64  last-commit/Ljzd
 000002e0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
 000002f0: 6769 6e2d 6d79 7354 6f6f 6c3f 7374 796c  gin-mysTool?styl
 00000300: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
 00000310: 3e0a 3c2f 6469 763e 0a0a 2320 6d79 7354  >.</div>..# mysT
 00000320: 6f6f 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8  ool - ..........
 00000330: be85 e58a a9e5 b7a5 e585 b7e6 8f92 e4bb  ................
-00000340: b60a 0a2a 2ae7 8988 e69c ac20 2d20 7631  ...**...... - v1
-00000350: 2e30 2e30 2d62 6574 612e 322a 2a0a 0a23  .0.0-beta.2**..#
-00000360: 2323 20f0 9f93 a320 e69b b4e6 96b0 e586  ## .... ........
-00000370: 85e5 aeb9 0a0a 2323 2323 2032 3032 332e  ......#### 2023.
-00000380: 362e 3232 202d 2076 312e 302e 302d 6265  6.22 - v1.0.0-be
-00000390: 7461 2e32 0ae6 94b9 e58a a8e8 be83 e5a4  ta.2............
-000003a0: a7ef bc8c e79b aee5 898d e698 af20 4265  ............. Be
-000003b0: 7461 20e7 8988 efbc 8ce5 8faf e883 bde4  ta .............
-000003c0: b88d e7a8 b3e5 ae9a 0a0a 5769 6e64 6f77  ..........Window
-000003d0: 73e3 8081 6d61 634f 5320 e4b8 8be6 97a0  s...macOS ......
-000003e0: e6b3 95e5 a49a e8bf 9be7 a88b e794 9fe6  ................
-000003f0: 8890 e595 86e5 9381 e59b bee7 8987 e79a  ................
-00000400: 84e9 97ae e9a2 98e6 9a82 e697 b6e6 b2a1  ................
-00000410: e69c 89e4 bfae e5a4 8d0a 0a2d 20e6 94af  ...........- ...
-00000420: e68c 81e4 bdbf e794 a8e4 baba e69c bae9  ................
-00000430: aa8c e8af 81e6 8993 e7a0 81e5 b9b3 e58f  ................
-00000440: b0e5 a484 e790 86e4 baba e69c bae9 aa8c  ................
-00000450: e8af 81e4 bbbb e58a a120 5b23 3131 395d  ......... [#119]
-00000460: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000470: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
-00000480: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-00000490: 6f6f 6c2f 7075 6c6c 2f31 3139 2920 6279  ool/pull/119) by
-000004a0: 2040 4e69 6768 742d 7374 6172 732d 310a   @Night-stars-1.
-000004b0: 2d20 e58e 9fe7 a59e e4be bfe7 acba e88e  - ..............
-000004c0: b7e5 8f96 e5a4 b1e8 b4a5 e697 b6e6 9bb4  ................
-000004d0: e68d a2e4 b8ba e4bd bfe7 94a8 e7b1 b3e6  ................
-000004e0: b8b8 e7a4 be69 4f53 e5b0 8fe7 bb84 e4bb  .....iOS........
-000004f0: b641 5049 e88e b7e5 8f96 205b 2331 3139  .API...... [#119
-00000500: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000510: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
-00000520: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00000530: 746f 6f6c 2f70 756c 6c2f 3131 3929 2062  tool/pull/119) b
-00000540: 7920 404e 6967 6874 2d73 7461 7273 2d31  y @Night-stars-1
-00000550: 0a2d 20e4 bfae e5a4 8de5 8e9f e7a5 9ee4  .- .............
-00000560: bebf e7ac bae5 928c e8ae a8e8 aeba e58c  ................
-00000570: bae7 adbe e588 b0e5 8faf e883 bde5 9ba0  ................
-00000580: e4b8 ba44 53e6 97a0 e695 88e8 808c e5a4  ...DS...........
-00000590: b1e8 b4a5 e79a 84e9 97ae e9a2 980a 0a23  ...............#
-000005a0: 2323 2320 3230 3233 2e36 2e31 3020 2d20  ### 2023.6.10 - 
-000005b0: 7631 2e30 2e30 2d62 6574 612e 310a e694  v1.0.0-beta.1...
-000005c0: b9e5 8aa8 e8be 83e5 a4a7 efbc 8ce7 9bae  ................
-000005d0: e589 8de6 98af 2042 6574 6120 e789 88ef  ...... Beta ....
-000005e0: bc8c e58f afe8 83bd e4b8 8de7 a8b3 e5ae  ................
-000005f0: 9a0a 0a2d 20e5 a4a7 e987 8fe7 9a84 e4bb  ...- ...........
-00000600: a3e7 a081 e987 8de6 9e84 efbc 8ce5 8c85  ................
-00000610: e68b ace7 b1b3 e6b8 b8e7 a4be 4150 49e7  ............API.
-00000620: 9a84 e5ae a2e6 88b7 e7ab afe5 ae9e e78e  ................
-00000630: b0e3 8081 e794 a8e6 88b7 e695 b0e6 8dae  ................
-00000640: e79b b8e5 85b3 e380 81e6 8f92 e4bb b6e9  ................
-00000650: 858d e7bd aee7 9bb8 e585 b3e3 8081 4150  ..............AP
-00000660: 49e7 9bb8 e585 b3e6 95b0 e68d aee6 a8a1  I...............
-00000670: e59e 8b0a 2d20 7e7e e4bf aee5 a48d e59c  ....- ~~........
-00000680: a820 5769 6e64 6f77 7320 e4b8 8be6 97a0  . Windows ......
-00000690: e6b3 95e5 a49a e8bf 9be7 a88b e794 9fe6  ................
-000006a0: 8890 e595 86e5 9381 e59b bee7 8987 e79a  ................
-000006b0: 84e9 97ae e9a2 987e 7e0a 2d20 e4bb 8ee6  .......~~.- ....
-000006c0: 98be e7a4 bae7 94a8 e688 b7e8 b4a6 e58f  ................
-000006d0: b7e7 bb91 e5ae 9ae7 9a84 e689 8be6 9cba  ................
-000006e0: e58f b7e6 94b9 e4b8 bae6 98be e7a4 bae8  ................
-000006f0: b4a6 e58f b7e7 9a84 e7b1 b3e6 b8b8 e7a4  ................
-00000700: be49 440a 2d20 e8ae bee7 bdae e380 81e5  .ID.- ..........
-00000710: 8591 e68d a2e8 aea1 e588 92e5 8a9f e883  ................
-00000720: bde6 94af e68c 81e7 bea4 e881 8ae4 bdbf  ................
-00000730: e794 a80a 2d20 e799 bbe9 9986 e7bb 91e5  ....- ..........
-00000740: ae9a e58f aae9 9c80 e8a6 81e8 bf9b e8a1  ................
-00000750: 8ce4 b880 e6ac a1e7 9fad e4bf a1e9 aa8c  ................
-00000760: e8af 810a 2d20 e794 a8e6 88b7 e695 b0e6  ....- ..........
-00000770: 8dae e696 87e4 bbb6 e380 81e6 8f92 e4bb  ................
-00000780: b6e9 858d e7bd aee6 9687 e4bb b620 2a2a  ............. **
-00000790: e6a0 bce5 bc8f e69b b4e6 96b0 efbc 8ce4  ................
-000007a0: b88e 2076 312e 302e 3020 e4b9 8be5 898d  .. v1.0.0 ......
-000007b0: e79a 84e7 8988 e69c ace4 b88d e585 bce5  ................
-000007c0: aeb9 2a2a 0a2d 20e4 bfae e5a4 8de6 b7bb  ..**.- .........
-000007d0: e58a a0e5 8591 e68d a2e4 bbbb e58a a1e6  ................
-000007e0: 97b6 e587 bae7 8eb0 e79a 8455 4944 e4b8  ...........UID..
-000007f0: 8de5 ad98 e59c a8e9 9499 e8af af0a 2d20  ..............- 
-00000800: e4bf aee5 a48d e595 86e5 9381 e59b bee7  ................
-00000810: 8987 e794 9fe6 8890 e5ae 8ce6 898d e58f  ................
-00000820: 91e5 87ba e590 8ee5 8fb0 e6ad a3e5 9ca8  ................
-00000830: e794 9fe6 8890 e68f 90e7 a4ba e79a 84e9  ................
-00000840: 97ae e9a2 980a 2d20 e5bc 82e5 b8b8 e68d  ......- ........
-00000850: 95e8 8eb7 e69b b4e5 8aa0 e587 86e7 a1ae  ................
-00000860: 0a2d 20e6 94b9 e8bf 9be4 ba86 e4b8 80e4  .- .............
-00000870: ba9b e696 87e6 9cac 0a0a 2323 2323 2032  ..........#### 2
-00000880: 3032 332e 352e 3138 0a2d 20e5 a49a e8bf  023.5.18.- .....
-00000890: 9be7 a88b e794 9fe6 8890 e595 86e5 9381  ................
-000008a0: e59b bee7 8987 efbc 88e5 a49a e6a0 b8ef  ................
-000008b0: bc89 efbc 8ce5 8aa0 e5bf abe5 9bbe e789  ................
-000008c0: 87e7 949f e688 90e9 809f e5ba a60a 2d20  ..............- 
-000008d0: e4bf aee5 a48d e983 a8e5 8886 e595 86e5  ................
-000008e0: 9381 e585 91e6 8da2 e697 b6e9 97b4 e994  ................
-000008f0: 99e8 afaf e79a 84e9 97ae e9a2 98ef bc88  ................
-00000900: e5a6 82e7 b1b3 e6b8 b8e7 a4be e595 86e5  ................
-00000910: 9381 e699 9ae4 ba86 e4b8 80e5 91a8 efbc  ................
-00000920: 890a 0a23 2323 2320 3230 3233 2e35 2e34  ...#### 2023.5.4
-00000930: 0a2d 20e5 a29e e58a a0e5 afb9 e698 9fe7  .- .............
-00000940: a9b9 e993 81e9 8193 e79a 84e7 adbe e588  ................
-00000950: b0e5 8a9f e883 bde7 9a84 e694 afe6 8c81  ................
-00000960: 202d 205b 2338 395d 2868 7474 7073 3a2f   - [#89](https:/
-00000970: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-00000980: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-00000990: 6769 6e2d 6d79 7374 6f6f 6c2f 7075 6c6c  gin-mystool/pull
-000009a0: 2f38 3929 2062 7920 4061 7961 6b61 7375  /89) by @ayakasu
-000009b0: 6b69 0a2d 20e4 bfae e5a4 8de6 8f92 e4bb  ki.- ...........
-000009c0: b6e5 91bd e4bb a4e4 bc98 e585 88e5 baa6  ................
-000009d0: e997 aee9 a298 202d 205b 2338 385d 2868  ...... - [#88](h
-000009e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000009f0: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
-00000a00: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000a10: 6c2f 7075 6c6c 2f38 3829 2062 7920 4061  l/pull/88) by @a
-00000a20: 7961 6b61 7375 6b69 0a2d 20e9 83a8 e588  yakasuki.- .....
-00000a30: 86e6 9687 e69c ace9 9499 e8af afe4 bfae  ................
-00000a40: e6ad a320 2d20 5b23 3930 5d28 6874 7470  ... - [#90](http
-00000a50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
-00000a60: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
-00000a70: 706c 7567 696e 2d6d 7973 746f 6f6c 2f70  plugin-mystool/p
-00000a80: 756c 6c2f 3930 2920 6279 2040 626c 6163  ull/90) by @blac
-00000a90: 6b2d 7a65 726f 3335 380a 0a2e 2e2e 0a0a  k-zero358.......
-00000aa0: 2323 2323 2032 3032 332e 332e 3330 0a2d  #### 2023.3.30.-
-00000ab0: 20e4 bfae e5a4 8d20 602f e585 91e6 8da2   ...... `/......
-00000ac0: 6020 e591 bde4 bba4 e58f afe8 83bd e4b8  ` ..............
-00000ad0: 8ee5 85b6 e4bb 96e6 8f92 e4bb b6e5 91bd  ................
-00000ae0: e4bb a4e5 86b2 e7aa 81e7 9a84 e997 aee9  ................
-00000af0: a298 efbc 8ce5 908c e697 b620 5bf0 9f94  ........... [...
-00000b00: 97e7 94a8 e6b3 95e5 8f98 e69b b45d 2868  .............](h
-00000b10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b20: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
-00000b30: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000b40: 6c2f 7769 6b69 2f49 6e66 6f72 6d61 7469  l/wiki/Informati
-00000b50: 6f6e 2d45 7863 6861 6e67 6523 e5a2 9ee5  on-Exchange#....
-00000b60: 8aa0 e588 a0e9 99a4 e585 91e6 8da2 e8ae  ................
-00000b70: a1e5 8892 290a 2d20 2e2e 2e0a 0a23 2320  ....).- .....## 
-00000b80: e58a 9fe8 83bd e592 8ce7 89b9 e680 a70a  ................
-00000b90: 0a2d 20e7 9fad e4bf a1e9 aa8c e8af 81e7  .- .............
-00000ba0: 99bb e5bd 95ef bc8c e585 8de6 8a93 e58c  ................
-00000bb0: 85e8 8eb7 e58f 9620 436f 6f6b 6965 0a2d  ....... Cookie.-
-00000bc0: 20e8 87aa e58a a8e5 ae8c e688 90e6 af8f   ...............
-00000bd0: e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb bbe5  ................
-00000be0: 8aa1 0a2d 20e8 87aa e58a a8e8 bf9b e8a1  ...- ...........
-00000bf0: 8ce6 b8b8 e688 8fe7 adbe e588 b00a 2d20  ..............- 
-00000c00: e58f afe5 88b6 e5ae 9ae7 b1b3 e6b8 b8e5  ................
-00000c10: b881 e595 86e5 9381 e585 91e6 8da2 e8ae  ................
-00000c20: a1e5 8892 efbc 8ce5 88b0 e782 b9e5 8591  ................
-00000c30: e68d a20a 2d20 e58f afe6 94af e68c 81e5  ....- ..........
-00000c40: a49a e4b8 aa20 5151 20e8 b4a6 e58f b7ef  ..... QQ .......
-00000c50: bc8c e6af 8fe4 b8aa 2051 5120 e8b4 a6e5  ........ QQ ....
-00000c60: 8fb7 e58f afe7 bb91 e5ae 9ae5 a49a e4b8  ................
-00000c70: aae7 b1b3 e593 88e6 b8b8 e8b4 a6e6 88b7  ................
-00000c80: 0a2d 2051 5120 e68e a8e9 8081 e689 a7e8  .- QQ ..........
-00000c90: a18c e7bb 93e6 9e9c e980 9ae7 9fa5 0a2d  ...............-
-00000ca0: 20e5 8e9f e7a5 9ee6 a091 e884 82e3 8081   ...............
-00000cb0: e6b4 9ee5 a4a9 e5ae 9de9 92b1 e380 81e8  ................
-00000cc0: b4a8 e987 8fe5 8f82 e58f 98e4 bbaa e5b7  ................
-00000cd0: b2e6 bba1 e697 b6e6 8ea8 e980 81e9 809a  ................
-00000ce0: e79f a50a 0a23 2320 e4bd bfe7 94a8 e8af  .....## ........
-00000cf0: b4e6 988e 0a0a 2323 2320 f09f 9ba0 efb8  ......### ......
-00000d00: 8f20 4e6f 6e65 426f 7432 20e6 9cba e599  . NoneBot2 .....
-00000d10: a8e4 baba e983 a8e7 bdb2 e592 8ce6 8f92  ................
-00000d20: e4bb b6e5 ae89 e8a3 850a 0ae8 afb7 e69f  ................
-00000d30: a5e7 9c8b 202d 3e20 5bf0 9f94 9749 6e73  .... -> [....Ins
-00000d40: 7461 6c6c 6174 696f 6e5d 2868 7474 7073  tallation](https
-00000d50: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
-00000d60: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
-00000d70: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
-00000d80: 6b69 2f49 6e73 7461 6c6c 6174 696f 6e29  ki/Installation)
-00000d90: 0a0a 2323 2320 f09f 9396 20e6 8f92 e4bb  ..### .... .....
-00000da0: b6e5 85b7 e4bd 93e4 bdbf e794 a8e8 afb4  ................
-00000db0: e698 8e0a 0ae8 afb7 e69f a5e7 9c8b 202d  .............. -
-00000dc0: 3e20 5bf0 9f94 9757 696b 6920 e696 87e6  > [....Wiki ....
-00000dd0: a1a3 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
-00000de0: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-00000df0: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00000e00: 7973 746f 6f6c 2f77 696b 6929 0a0a 2323  ystool/wiki)..##
-00000e10: 2320 e29d 9320 e88e b7e5 8f96 e68f 92e4  # ... ..........
-00000e20: bbb6 e5b8 aee5 8aa9 e4bf a1e6 81af 0a0a  ................
-00000e30: 2323 2323 20e6 8f92 e4bb b6e5 91bd e4bb  #### ...........
-00000e40: a40a 0a60 6060 0a2f e5b8 aee5 8aa9 0a60  ...```./.......`
-00000e50: 6060 0a0a 3e20 e29a a0ef b88f 20e6 b3a8  ``..> ...... ...
-00000e60: e684 8f20 e6ad a4e5 a484 e6b2 a1e6 9c89  ... ............
-00000e70: e4bd bfe7 94a8 205b f09f 9497 20e6 8f92  ...... [.... ...
-00000e80: e4bb b6e5 91bd e4bb a4e5 a4b4 5d28 6874  ............](ht
-00000e90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ea0: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
-00000eb0: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
-00000ec0: 2f77 696b 692f 436f 6e66 6967 7572 6174  /wiki/Configurat
-00000ed0: 696f 6e2d 436f 6e66 6967 2363 6f6d 6d61  ion-Config#comma
-00000ee0: 6e64 7374 6172 7429 0a0a 2323 20e5 85b6  ndstart)..## ...
-00000ef0: e4bb 960a 0a23 2323 205b f09f 9383 e6ba  .....### [......
-00000f00: 90e7 a081 e8af b4e6 988e 5d28 6874 7470  ..........](http
-00000f10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
-00000f20: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
-00000f30: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
-00000f40: 696b 692f 536f 7572 6365 2d53 7472 7563  iki/Source-Struc
-00000f50: 7475 7265 290a 2323 2320 e980 82e9 858d  ture).### ......
-00000f60: 205b e7bb aae5 b1b1 e79c 9fe5 afbb 426f   [............Bo
-00000f70: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00000f80: 622e 636f 6d2f 4869 6269 4b69 6572 2f7a  b.com/HibiKier/z
-00000f90: 6865 6e78 756e 5f62 6f74 2920 e79a 84e5  henxun_bot) ....
-00000fa0: 8886 e694 af0a 2d20 6874 7470 733a 2f2f  ......- https://
-00000fb0: 6769 7468 7562 2e63 6f6d 2f4d 5754 4a43  github.com/MWTJC
-00000fc0: 2f7a 6865 6e78 756e 2d70 6c75 6769 6e2d  /zhenxun-plugin-
-00000fd0: 6d79 7374 6f6f 6c0a 2d20 6874 7470 733a  mystool.- https:
-00000fe0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7961  //github.com/aya
-00000ff0: 6b61 7375 6b69 2f6e 6f6e 6562 6f74 2d70  kasuki/nonebot-p
-00001000: 6c75 6769 6e2d 6d79 7374 6f6f 6c0a       lugin-mystool.
+00000340: b60a 0a23 2320 f09f 93a3 20e6 9bb4 e696  ...## .... .....
+00000350: b0e5 8685 e5ae b90a 0a23 2323 2032 3032  .........### 202
+00000360: 332e 362e 3233 202d 2076 312e 302e 310a  3.6.23 - v1.0.1.
+00000370: 2d20 e4bf aee5 a48d e697 a0e6 b395 e5af  - ..............
+00000380: bce5 87ba 436f 6f6b 6965 73e7 9a84 e997  ....Cookies.....
+00000390: aee9 a298 0a2d 20e4 bfae e5a4 8de5 9ba0  .....- .........
+000003a0: e7bc bae5 b091 e58f 82e9 878f e8b4 a8e5  ................
+000003b0: 8f98 e4bb aae6 95b0 e68d aee8 808c e5af  ................
+000003c0: bce8 87b4 e4b8 8de6 96ad e68f 90e9 8692  ................
+000003d0: e79a 8442 7567 0a2d 20e4 bfae e5a4 8de8  ...Bug.- .......
+000003e0: b4a6 e58f b7e8 aebe e7bd aee4 b8ad e6b8  ................
+000003f0: b8e6 888f e7ad bee5 88b0 e5bc 80e5 90af  ................
+00000400: 2fe5 85b3 e997 ade7 8ab6 e680 81e5 ae9e  /...............
+00000410: e999 85e5 afb9 e5ba 94e7 9a84 e698 afe7  ................
+00000420: b1b3 e6b8 b8e5 b881 e4bb bbe5 8aa1 e79a  ................
+00000430: 8442 7567 2023 3132 3120 6279 2040 7878  .Bug #121 by @xx
+00000440: 7467 3636 360a 0a0a 2323 2320 3230 3233  tg666...### 2023
+00000450: 2e36 2e32 3320 2d20 7631 2e30 2e30 0a23  .6.23 - v1.0.0.#
+00000460: 2323 2320 7631 2e30 2e30 0a2d 20e4 bfae  ### v1.0.0.- ...
+00000470: e5a4 8d57 696e 646f 7773 2c20 6d61 634f  ...Windows, macO
+00000480: 53e5 a49a e8bf 9be7 a88b e794 9fe6 8890  S...............
+00000490: e595 86e5 9381 e59b bee7 8987 e5a4 b1e8  ................
+000004a0: b4a5 e79a 84e9 97ae e9a2 9820 5b23 3132  ........... [#12
+000004b0: 305d 2868 7474 7073 3a2f 2f67 6974 6875  0](https://githu
+000004c0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+000004d0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+000004e0: 7374 6f6f 6c2f 7075 6c6c 2f31 3230 2920  stool/pull/120) 
+000004f0: 6279 2040 4e69 6768 742d 7374 6172 732d  by @Night-stars-
+00000500: 310a 0a23 2323 2320 7631 2e30 2e30 2d62  1..#### v1.0.0-b
+00000510: 6574 612e 320a 2d20 e694 afe6 8c81 e4bd  eta.2.- ........
+00000520: bfe7 94a8 e4ba bae6 9cba e9aa 8ce8 af81  ................
+00000530: e689 93e7 a081 e5b9 b3e5 8fb0 e5a4 84e7  ................
+00000540: 9086 e4ba bae6 9cba e9aa 8ce8 af81 e4bb  ................
+00000550: bbe5 8aa1 205b 2331 3139 5d28 6874 7470  .... [#119](http
+00000560: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00000570: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+00000580: 706c 7567 696e 2d6d 7973 746f 6f6c 2f70  plugin-mystool/p
+00000590: 756c 6c2f 3131 3929 2062 7920 404e 6967  ull/119) by @Nig
+000005a0: 6874 2d73 7461 7273 2d31 0a2d 20e5 8e9f  ht-stars-1.- ...
+000005b0: e7a5 9ee4 bebf e7ac bae8 8eb7 e58f 96e5  ................
+000005c0: a4b1 e8b4 a5e6 97b6 e69b b4e6 8da2 e4b8  ................
+000005d0: bae4 bdbf e794 a8e7 b1b3 e6b8 b8e7 a4be  ................
+000005e0: 694f 53e5 b08f e7bb 84e4 bbb6 4150 49e8  iOS.........API.
+000005f0: 8eb7 e58f 9620 5b23 3131 395d 2868 7474  ..... [#119](htt
+00000600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000610: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
+00000620: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
+00000630: 7075 6c6c 2f31 3139 2920 6279 2040 4e69  pull/119) by @Ni
+00000640: 6768 742d 7374 6172 732d 310a 2d20 e4bf  ght-stars-1.- ..
+00000650: aee5 a48d e58e 9fe7 a59e e4be bfe7 acba  ................
+00000660: e592 8ce8 aea8 e8ae bae5 8cba e7ad bee5  ................
+00000670: 88b0 e58f afe8 83bd e59b a0e4 b8ba 4453  ..............DS
+00000680: e697 a0e6 9588 e880 8ce5 a4b1 e8b4 a5e7  ................
+00000690: 9a84 e997 aee9 a298 0a0a 2323 2323 2076  ..........#### v
+000006a0: 312e 302e 302d 6265 7461 2e31 0a2d 20e5  1.0.0-beta.1.- .
+000006b0: a4a7 e987 8fe7 9a84 e4bb a3e7 a081 e987  ................
+000006c0: 8de6 9e84 efbc 8ce5 8c85 e68b ace7 b1b3  ................
+000006d0: e6b8 b8e7 a4be 4150 49e7 9a84 e5ae a2e6  ......API.......
+000006e0: 88b7 e7ab afe5 ae9e e78e b0e3 8081 e794  ................
+000006f0: a8e6 88b7 e695 b0e6 8dae e79b b8e5 85b3  ................
+00000700: e380 81e6 8f92 e4bb b6e9 858d e7bd aee7  ................
+00000710: 9bb8 e585 b3e3 8081 4150 49e7 9bb8 e585  ........API.....
+00000720: b3e6 95b0 e68d aee6 a8a1 e59e 8b0a 2d20  ..............- 
+00000730: e4bb 8ee6 98be e7a4 bae7 94a8 e688 b7e8  ................
+00000740: b4a6 e58f b7e7 bb91 e5ae 9ae7 9a84 e689  ................
+00000750: 8be6 9cba e58f b7e6 94b9 e4b8 bae6 98be  ................
+00000760: e7a4 bae8 b4a6 e58f b7e7 9a84 e7b1 b3e6  ................
+00000770: b8b8 e7a4 be49 440a 2d20 e8ae bee7 bdae  .....ID.- ......
+00000780: e380 81e5 8591 e68d a2e8 aea1 e588 92e5  ................
+00000790: 8a9f e883 bde6 94af e68c 81e7 bea4 e881  ................
+000007a0: 8ae4 bdbf e794 a80a 2d20 e799 bbe9 9986  ........- ......
+000007b0: e7bb 91e5 ae9a e58f aae9 9c80 e8a6 81e8  ................
+000007c0: bf9b e8a1 8ce4 b880 e6ac a1e7 9fad e4bf  ................
+000007d0: a1e9 aa8c e8af 810a 2d20 e794 a8e6 88b7  ........- ......
+000007e0: e695 b0e6 8dae e696 87e4 bbb6 e380 81e6  ................
+000007f0: 8f92 e4bb b6e9 858d e7bd aee6 9687 e4bb  ................
+00000800: b620 2a2a e6a0 bce5 bc8f e69b b4e6 96b0  . **............
+00000810: efbc 8ce4 b88e 2076 312e 302e 3020 e4b9  ...... v1.0.0 ..
+00000820: 8be5 898d e79a 84e7 8988 e69c ace4 b88d  ................
+00000830: e585 bce5 aeb9 2a2a 0a2d 20e4 bfae e5a4  ......**.- .....
+00000840: 8de6 b7bb e58a a0e5 8591 e68d a2e4 bbbb  ................
+00000850: e58a a1e6 97b6 e587 bae7 8eb0 e79a 8455  ...............U
+00000860: 4944 e4b8 8de5 ad98 e59c a8e9 9499 e8af  ID..............
+00000870: af0a 2d20 e4bf aee5 a48d e595 86e5 9381  ..- ............
+00000880: e59b bee7 8987 e794 9fe6 8890 e5ae 8ce6  ................
+00000890: 898d e58f 91e5 87ba e590 8ee5 8fb0 e6ad  ................
+000008a0: a3e5 9ca8 e794 9fe6 8890 e68f 90e7 a4ba  ................
+000008b0: e79a 84e9 97ae e9a2 980a 2d20 e5bc 82e5  ..........- ....
+000008c0: b8b8 e68d 95e8 8eb7 e69b b4e5 8aa0 e587  ................
+000008d0: 86e7 a1ae 0a2d 20e6 94b9 e8bf 9be4 ba86  .....- .........
+000008e0: e4b8 80e4 ba9b e696 87e6 9cac 0a0a 2323  ..............##
+000008f0: 2320 3230 3233 2e35 2e31 3820 2d20 7630  # 2023.5.18 - v0
+00000900: 2e32 2e39 0a2d 20e5 a49a e8bf 9be7 a88b  .2.9.- .........
+00000910: e794 9fe6 8890 e595 86e5 9381 e59b bee7  ................
+00000920: 8987 efbc 88e5 a49a e6a0 b8ef bc89 efbc  ................
+00000930: 8ce5 8aa0 e5bf abe5 9bbe e789 87e7 949f  ................
+00000940: e688 90e9 809f e5ba a60a 2d20 e4bf aee5  ..........- ....
+00000950: a48d e983 a8e5 8886 e595 86e5 9381 e585  ................
+00000960: 91e6 8da2 e697 b6e9 97b4 e994 99e8 afaf  ................
+00000970: e79a 84e9 97ae e9a2 98ef bc88 e5a6 82e7  ................
+00000980: b1b3 e6b8 b8e7 a4be e595 86e5 9381 e699  ................
+00000990: 9ae4 ba86 e4b8 80e5 91a8 efbc 890a 0a23  ...............#
+000009a0: 2323 2032 3032 332e 352e 3420 2d20 7630  ## 2023.5.4 - v0
+000009b0: 2e32 2e38 0a2d 20e5 a29e e58a a0e5 afb9  .2.8.- .........
+000009c0: e698 9fe7 a9b9 e993 81e9 8193 e79a 84e7  ................
+000009d0: adbe e588 b0e5 8a9f e883 bde7 9a84 e694  ................
+000009e0: afe6 8c81 202d 205b 2338 395d 2868 7474  .... - [#89](htt
+000009f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000a00: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
+00000a10: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
+00000a20: 7075 6c6c 2f38 3929 2062 7920 4061 7961  pull/89) by @aya
+00000a30: 6b61 7375 6b69 0a2d 20e4 bfae e5a4 8de6  kasuki.- .......
+00000a40: 8f92 e4bb b6e5 91bd e4bb a4e4 bc98 e585  ................
+00000a50: 88e5 baa6 e997 aee9 a298 202d 205b 2338  .......... - [#8
+00000a60: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+00000a70: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+00000a80: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000a90: 7374 6f6f 6c2f 7075 6c6c 2f38 3829 2062  stool/pull/88) b
+00000aa0: 7920 4061 7961 6b61 7375 6b69 0a2d 20e9  y @ayakasuki.- .
+00000ab0: 83a8 e588 86e6 9687 e69c ace9 9499 e8af  ................
+00000ac0: afe4 bfae e6ad a320 2d20 5b23 3930 5d28  ....... - [#90](
+00000ad0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000ae0: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000af0: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000b00: 6f6c 2f70 756c 6c2f 3930 2920 6279 2040  ol/pull/90) by @
+00000b10: 626c 6163 6b2d 7a65 726f 3335 380a 0a23  black-zero358..#
+00000b20: 2320 e58a 9fe8 83bd e592 8ce7 89b9 e680  # ..............
+00000b30: a70a 0a2d 20e7 9fad e4bf a1e9 aa8c e8af  ...- ...........
+00000b40: 81e7 99bb e5bd 95ef bc8c e585 8de6 8a93  ................
+00000b50: e58c 85e8 8eb7 e58f 9620 436f 6f6b 6965  ......... Cookie
+00000b60: 0a2d 20e8 87aa e58a a8e5 ae8c e688 90e6  .- .............
+00000b70: af8f e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb  ................
+00000b80: bbe5 8aa1 0a2d 20e8 87aa e58a a8e8 bf9b  .....- .........
+00000b90: e8a1 8ce6 b8b8 e688 8fe7 adbe e588 b00a  ................
+00000ba0: 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3 e6b8  - ..............
+00000bb0: b8e5 b881 e595 86e5 9381 e585 91e6 8da2  ................
+00000bc0: e8ae a1e5 8892 efbc 8ce5 88b0 e782 b9e5  ................
+00000bd0: 8591 e68d a20a 2d20 e58f afe6 94af e68c  ......- ........
+00000be0: 81e5 a49a e4b8 aa20 5151 20e8 b4a6 e58f  ....... QQ .....
+00000bf0: b7ef bc8c e6af 8fe4 b8aa 2051 5120 e8b4  .......... QQ ..
+00000c00: a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5 a49a  ................
+00000c10: e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4 a6e6  ................
+00000c20: 88b7 0a2d 2051 5120 e68e a8e9 8081 e689  ...- QQ ........
+00000c30: a7e8 a18c e7bb 93e6 9e9c e980 9ae7 9fa5  ................
+00000c40: 0a2d 20e5 8e9f e7a5 9ee6 a091 e884 82e3  .- .............
+00000c50: 8081 e6b4 9ee5 a4a9 e5ae 9de9 92b1 e380  ................
+00000c60: 81e8 b4a8 e987 8fe5 8f82 e58f 98e4 bbaa  ................
+00000c70: e5b7 b2e6 bba1 e697 b6e6 8ea8 e980 81e9  ................
+00000c80: 809a e79f a50a 0a23 2320 e4bd bfe7 94a8  .......## ......
+00000c90: e8af b4e6 988e 0a0a 2323 2320 f09f 9ba0  ........### ....
+00000ca0: efb8 8f20 4e6f 6e65 426f 7432 20e6 9cba  ... NoneBot2 ...
+00000cb0: e599 a8e4 baba e983 a8e7 bdb2 e592 8ce6  ................
+00000cc0: 8f92 e4bb b6e5 ae89 e8a3 850a 0ae8 afb7  ................
+00000cd0: e69f a5e7 9c8b 202d 3e20 5bf0 9f94 9749  ...... -> [....I
+00000ce0: 6e73 7461 6c6c 6174 696f 6e5d 2868 7474  nstallation](htt
+00000cf0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000d00: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
+00000d10: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
+00000d20: 7769 6b69 2f49 6e73 7461 6c6c 6174 696f  wiki/Installatio
+00000d30: 6e29 0a0a 2323 2320 f09f 9396 20e6 8f92  n)..### .... ...
+00000d40: e4bb b6e5 85b7 e4bd 93e4 bdbf e794 a8e8  ................
+00000d50: afb4 e698 8e0a 0ae8 afb7 e69f a5e7 9c8b  ................
+00000d60: 202d 3e20 5bf0 9f94 9757 696b 6920 e696   -> [....Wiki ..
+00000d70: 87e6 a1a3 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
+00000d80: 7468 7562 2e63 6f6d 2f4c 6a7a 642d 5052  thub.com/Ljzd-PR
+00000d90: 4f2f 6e6f 6e65 626f 742d 706c 7567 696e  O/nonebot-plugin
+00000da0: 2d6d 7973 746f 6f6c 2f77 696b 6929 0a0a  -mystool/wiki)..
+00000db0: 2323 2320 e29d 9320 e88e b7e5 8f96 e68f  ### ... ........
+00000dc0: 92e4 bbb6 e5b8 aee5 8aa9 e4bf a1e6 81af  ................
+00000dd0: 0a0a 2323 2323 20e6 8f92 e4bb b6e5 91bd  ..#### .........
+00000de0: e4bb a40a 0a60 6060 0a2f e5b8 aee5 8aa9  .....```./......
+00000df0: 0a60 6060 0a0a 3e20 e29a a0ef b88f 20e6  .```..> ...... .
+00000e00: b3a8 e684 8f20 e6ad a4e5 a484 e6b2 a1e6  ..... ..........
+00000e10: 9c89 e4bd bfe7 94a8 205b f09f 9497 20e6  ........ [.... .
+00000e20: 8f92 e4bb b6e5 91bd e4bb a4e5 a4b4 5d28  ..............](
+00000e30: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000e40: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000e50: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000e60: 6f6c 2f77 696b 692f 436f 6e66 6967 7572  ol/wiki/Configur
+00000e70: 6174 696f 6e2d 436f 6e66 6967 2363 6f6d  ation-Config#com
+00000e80: 6d61 6e64 7374 6172 7429 0a0a 2323 20e5  mandstart)..## .
+00000e90: 85b6 e4bb 960a 0a23 2323 205b f09f 9383  .......### [....
+00000ea0: e6ba 90e7 a081 e8af b4e6 988e 5d28 6874  ............](ht
+00000eb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000ec0: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
+00000ed0: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
+00000ee0: 2f77 696b 692f 536f 7572 6365 2d53 7472  /wiki/Source-Str
+00000ef0: 7563 7475 7265 290a 2323 2320 e980 82e9  ucture).### ....
+00000f00: 858d 205b e7bb aae5 b1b1 e79c 9fe5 afbb  .. [............
+00000f10: 426f 745d 2868 7474 7073 3a2f 2f67 6974  Bot](https://git
+00000f20: 6875 622e 636f 6d2f 4869 6269 4b69 6572  hub.com/HibiKier
+00000f30: 2f7a 6865 6e78 756e 5f62 6f74 2920 e79a  /zhenxun_bot) ..
+00000f40: 84e5 8886 e694 af0a 2d20 6874 7470 733a  ........- https:
+00000f50: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 5754  //github.com/MWT
+00000f60: 4a43 2f7a 6865 6e78 756e 2d70 6c75 6769  JC/zhenxun-plugi
+00000f70: 6e2d 6d79 7374 6f6f 6c0a 2d20 6874 7470  n-mystool.- http
+00000f80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00000f90: 7961 6b61 7375 6b69 2f6e 6f6e 6562 6f74  yakasuki/nonebot
+00000fa0: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c0a  -plugin-mystool.
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/pyproject.toml` & `nonebot_plugin_mystool-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v1.0.0-beta.2"
+version = "v1.0.1"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,18 @@
     """.strip(),
     extra={"version": VERSION}
 )
 
 # 在此处使用 get_driver() 防止多进程生成图片时反复调用
 
 from .utils import CommandBegin
+from nonebot import init
 from nonebot import get_driver
 
+init()  # 初始化Driver对象
 get_driver().on_startup(CommandBegin.set_command_begin)
 
 # 加载其它代码
 
 FILE_PATH = Path(__file__).parent.absolute()
 
 for _, file, _ in pkgutil.iter_modules([str(FILE_PATH)]):
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,16 @@
     else:
         await address_matcher.send(
             "请跟随指引设置收货地址ID，如果你还没有设置米游社收获地址，请前往官网或App设置。\n🚪过程中发送“退出”即可退出")
     if len(user_account) == 1:
         account = next(iter(user_account.values()))
         matcher.set_arg('bbs_uid', Message(account.bbs_uid))
     else:
-        uids = map(lambda x: x.bbs_uid, user_account.values())
         msg = "您有多个账号，您要设置以下哪个账号的收货地址？\n"
-        msg += "\n".join(map(lambda x: f"🆔{x}", uids))
+        msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
         await matcher.send(msg)
 
 
 @address_matcher.got('bbs_uid')
 async def _(event: PrivateMessageEvent, state: T_State, uid=Arg("bbs_uid")):
     if isinstance(uid, Message):
         uid = uid.extract_plain_text().strip()
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/data_model.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,9 +484,9 @@
 class GeetestResultV4(BaseModel):
     """
     GEETEST GT4 人机验证结果数据
     """
     captcha_id: str
     lot_number: str
     pass_token: str
-    gen_time: int
+    gen_time: str
     captcha_output: str
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,16 @@
     if len(command) > 1:
         state['command_2'] = command[1]
         matcher.set_arg("good_id", command_arg)
         if len(user_account) == 1:
             uid = next(iter(user_account.values())).bbs_uid
             matcher.set_arg('bbs_uid', Message(uid))
         else:
-            uids = map(lambda x: x.bbs_uid, user_account.values())
             msg = "您有多个账号，您要配置以下哪个账号的兑换计划？\n"
-            msg += "\n".join(map(lambda x: f"🆔{x}", uids))
+            msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
             msg += "\n🚪发送“退出”即可退出"
             await matcher.send(msg)
     # 如果未使用二级命令，则进行查询操作，并结束交互
     else:
         msg = ""
         for plan in user.exchange_plans:
             good_detail_status, good = await get_good_detail(plan.good)
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/game_sign_api.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/game_sign_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/good_image.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/good_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,16 @@
     user_account = _conf.users[event.user_id].accounts
     if not user_account:
         await output_cookies.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     elif len(user_account) == 1:
         account = next(iter(user_account.values()))
         matcher.set_arg('bbs_uid', Message(account.bbs_uid))
     else:
-        uids = map(lambda x: x.bbs_uid, user_account)
         msg = "您有多个账号，您要导出哪个账号的Cookies数据？\n"
-        msg += "\n".join(map(lambda x: f"🆔{x}", uids))
+        msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
         msg += "\n🚪发送“退出”即可退出"
         await output_cookies.send(msg)
 
 
 @output_cookies.got('bbs_uid')
 async def _(event: PrivateMessageEvent, matcher: Matcher, uid=Arg("bbs_uid")):
     """
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/myb_missions_api.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/myb_missions_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,14 +398,16 @@
                             return
                         else:
                             has_checked[account.bbs_uid]['transformer'] = True
                             msg += '❕您的参量质变仪已准备就绪\n\n'
                     else:
                         has_checked[account.bbs_uid]['transformer'] = False
                         return
+                else:
+                    has_checked[account.bbs_uid]['transformer'] = False
             msg += "❖实时便笺❖" \
                    f"\n⏳树脂数量：{board.current_resin} / 160" \
                    f"\n🕰️探索派遣：{board.current_expedition_num} / {board.max_expedition_num}" \
                    f"\n📅每日委托：{4 - board.finished_task_num} 个任务未完成" \
                    f"\n💰洞天财瓮：{board.current_home_coin} / {board.max_home_coin}" \
                    f"\n🎰参量质变仪：{board.transformer_text if board.transformer else 'N/A'}"
             if group_event:
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plugin_data.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/plugin_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Mapping
 
 from loguru import logger
 from pydantic import BaseModel, ValidationError, BaseSettings, validator
 
 from .user_data import UserData, UserAccount
 
-VERSION = "v1.0.0-beta.2"
+VERSION = "v1.0.1"
 """程序当前版本"""
 
 ROOT_PATH = Path(__name__).parent.absolute()
 '''NoneBot2 机器人根目录'''
 
 DATA_PATH = ROOT_PATH / "data" / "nonebot-plugin-mystool"
 '''插件数据保存目录'''
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,16 @@
     if not user_account:
         await account_setting.finish(
             f"⚠️你尚未绑定米游社账户，请先使用『{_conf.preference.command_start}登录』进行登录")
     if len(user_account) == 1:
         uid = next(iter(user_account.values())).bbs_uid
         matcher.set_arg('bbs_uid', Message(uid))
     else:
-        uids = map(lambda x: x.bbs_uid, user_account.values())
         msg = "您有多个账号，您要更改以下哪个账号的设置？\n"
-        msg += "\n".join(map(lambda x: f"🆔{x}", uids))
+        msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
         msg += "\n🚪发送“退出”即可退出"
         await matcher.send(msg)
 
 
 @account_setting.got('bbs_uid')
 async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State, uid=Arg('bbs_uid')):
     """
@@ -70,15 +69,15 @@
         await account_setting.reject('⚠️您发送的账号不在以上账号内，请重新发送')
     account = user_account[uid]
     state['account'] = account
     state["prepare_to_delete"] = False
 
     user_setting = ""
     user_setting += f"1️⃣ 米游币任务自动执行：{'开' if account.enable_mission else '关'}"
-    user_setting += f"\n2️⃣ 游戏自动签到：{'开' if account.enable_mission else '关'}"
+    user_setting += f"\n2️⃣ 游戏自动签到：{'开' if account.enable_game_sign else '关'}"
     platform_show = "iOS" if account.platform == "ios" else "安卓"
     user_setting += f"\n3️⃣ 设备平台：{platform_show}"
 
     # 筛选出用户数据中的missionGame对应的游戏全称
     user_setting += "\n\n4️⃣ 执行米游币任务的频道：" + \
                     "\n- " + "、".join(map(lambda x: f"『{x.NAME}』", account.mission_games))
     user_setting += f"\n\n5️⃣ 原神树脂恢复提醒：{'开' if account.enable_resin else '关'}"
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/simple_api.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/simple_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -756,67 +756,62 @@
 
 
 async def create_mobile_captcha(phone_number: int,
                                 mmt_data: MmtData,
                                 geetest_result: Union[GeetestResult, GeetestResultV4],
                                 client: Optional[httpx.AsyncClient] = None,
                                 use_v4: bool = True,
-                                device_id: str = generate_device_id(),
+                                device_id: str = None,
                                 retry: bool = True
                                 ) -> Tuple[CreateMobileCaptchaStatus, Optional[httpx.AsyncClient]]:
     """
     发送短信验证码
 
     :param phone_number: 手机号
     :param mmt_data: 人机验证任务数据
     :param geetest_result: 人机验证结果数据
     :param client: httpx.AsyncClient 连接
     :param use_v4: 是否使用极验第四代人机验证
-    :param device_id: 设备 ID
+    :param device_id: 设备ID
     :param retry: 是否允许重试
     """
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = device_id
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     if use_v4 and isinstance(geetest_result, GeetestResultV4):
-        params = {
+        geetest_v4_data = geetest_result.dict(skip_defaults=True)
+        content = {
             "action_type": "login",
             "mmt_key": mmt_data.mmt_key,
-            "geetest_v4_data": geetest_result.dict(skip_defaults=True),
-            "mobile": phone_number,
-            "t": round(NtpTime.time() * 1000)
+            "geetest_v4_data": str(geetest_v4_data).replace("'", '"'),
+            "mobile": str(phone_number),
+            "t": str(round(NtpTime.time() * 1000))
         }
     else:
-        params = {
+        content = {
             "action_type": "login",
             "mmt_key": mmt_data.mmt_key,
             "geetest_challenge": mmt_data.challenge,
             "geetest_validate": geetest_result.validate,
             "geetest_seccode": geetest_result.seccode,
             "mobile": phone_number,
             "t": round(NtpTime.time() * 1000)
         }
-    encoded_params = urlencode(params)
 
     async def request():
         """
         发送请求的闭包函数
         """
         return await client.post(URL_CREATE_MOBILE_CAPTCHA,
-                                 content=encoded_params,
+                                 data=content,
                                  headers=headers,
                                  timeout=_conf.preference.timeout)
 
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
-                # FIXME 2023/4/13: 似乎会导致卡在连接状态，暂时弃用
-                #   res = await client.options(URL_CREATE_MOBILE_CAPTCHA,
-                #                            headers=headers,
-                #                            timeout=conf.preference.timeout)
-                #   cookies.update(res.cookies)
                 if client and not client.is_closed:
                     res = await request()
                 else:
                     async with httpx.AsyncClient() as client:
                         res = await request()
                 api_result = ApiResultHandler(res.json())
                 if api_result.success:
```

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_check.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/user_check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_data.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/user_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-1.0.1/src/nonebot_plugin_mystool/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b2/PKG-INFO` & `nonebot_plugin_mystool-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 1.0.0b2
+Version: 1.0.1
 Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
@@ -39,56 +39,51 @@
   <img alt="CodeFactor" src="https://www.codefactor.io/repository/github/ljzd-pro/nonebot-plugin-mystool/badge?style=for-the-badge">
   <img alt="最新发行版" src="https://img.shields.io/github/v/release/Ljzd-PRO/nonebot-plugin-mysTool?logo=python&style=for-the-badge">
   <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
 </div>
 
 # mysTool - 米游社辅助工具插件
 
-**版本 - v1.0.0-beta.2**
+## 📣 更新内容
 
-### 📣 更新内容
+### 2023.6.23 - v1.0.1
+- 修复无法导出Cookies的问题
+- 修复因缺少参量质变仪数据而导致不断提醒的Bug
+- 修复账号设置中游戏签到开启/关闭状态实际对应的是米游币任务的Bug #121 by @xxtg666
 
-#### 2023.6.22 - v1.0.0-beta.2
-改动较大，目前是 Beta 版，可能不稳定
 
-Windows、macOS 下无法多进程生成商品图片的问题暂时没有修复
+### 2023.6.23 - v1.0.0
+#### v1.0.0
+- 修复Windows, macOS多进程生成商品图片失败的问题 [#120](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/120) by @Night-stars-1
 
+#### v1.0.0-beta.2
 - 支持使用人机验证打码平台处理人机验证任务 [#119](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/119) by @Night-stars-1
 - 原神便笺获取失败时更换为使用米游社iOS小组件API获取 [#119](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/119) by @Night-stars-1
 - 修复原神便笺和讨论区签到可能因为DS无效而失败的问题
 
-#### 2023.6.10 - v1.0.0-beta.1
-改动较大，目前是 Beta 版，可能不稳定
-
+#### v1.0.0-beta.1
 - 大量的代码重构，包括米游社API的客户端实现、用户数据相关、插件配置相关、API相关数据模型
-- ~~修复在 Windows 下无法多进程生成商品图片的问题~~
 - 从显示用户账号绑定的手机号改为显示账号的米游社ID
 - 设置、兑换计划功能支持群聊使用
 - 登陆绑定只需要进行一次短信验证
 - 用户数据文件、插件配置文件 **格式更新，与 v1.0.0 之前的版本不兼容**
 - 修复添加兑换任务时出现的UID不存在错误
 - 修复商品图片生成完才发出后台正在生成提示的问题
 - 异常捕获更加准确
 - 改进了一些文本
 
-#### 2023.5.18
+### 2023.5.18 - v0.2.9
 - 多进程生成商品图片（多核），加快图片生成速度
 - 修复部分商品兑换时间错误的问题（如米游社商品晚了一周）
 
-#### 2023.5.4
+### 2023.5.4 - v0.2.8
 - 增加对星穹铁道的签到功能的支持 - [#89](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/89) by @ayakasuki
 - 修复插件命令优先度问题 - [#88](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/88) by @ayakasuki
 - 部分文本错误修正 - [#90](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/90) by @black-zero358
 
-...
-
-#### 2023.3.30
-- 修复 `/兑换` 命令可能与其他插件命令冲突的问题，同时 [🔗用法变更](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-Exchange#增加删除兑换计划)
-- ...
-
 ## 功能和特性
 
 - 短信验证登录，免抓包获取 Cookie
 - 自动完成每日米游币任务
 - 自动进行游戏签到
 - 可制定米游币商品兑换计划，到点兑换
 - 可支持多个 QQ 账号，每个 QQ 账号可绑定多个米哈游账户
```

