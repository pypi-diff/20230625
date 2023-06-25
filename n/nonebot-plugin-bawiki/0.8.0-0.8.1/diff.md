# Comparing `tmp/nonebot_plugin_bawiki-0.8.0.tar.gz` & `tmp/nonebot_plugin_bawiki-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.8.0.tar", last modified: Fri Jun 23 17:01:03 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.8.1.tar", last modified: Sun Jun 25 16:16:03 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.8.0.tar` & `nonebot_plugin_bawiki-0.8.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1068 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/LICENSE
--rw-r--r--   0        0        0     9028 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/README.md
--rw-r--r--   0        0        0      734 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0      947 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/__init__.py
--rw-r--r--   0        0        0     3739 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/arona.py
--rw-r--r--   0        0        0     2320 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/calender.py
--rw-r--r--   0        0        0     1265 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/clear_cache.py
--rw-r--r--   0        0        0     1218 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/craft.py
--rw-r--r--   0        0        0     1003 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/emoji.py
--rw-r--r--   0        0        0     2580 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/event.py
--rw-r--r--   0        0        0      976 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/furniture.py
--rw-r--r--   0        0        0     6327 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/gacha.py
--rw-r--r--   0        0        0     3555 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/global_future.py
--rw-r--r--   0        0        0     1775 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/level_guide.py
--rw-r--r--   0        0        0     1428 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/manga.py
--rw-r--r--   0        0        0     4356 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/raid.py
--rw-r--r--   0        0        0     3597 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_fav.py
--rw-r--r--   0        0        0     1868 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_rank.py
--rw-r--r--   0        0        0     1625 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
--rw-r--r--   0        0        0     2011 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_wiki_schale.py
--rw-r--r--   0        0        0     3375 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/time_atk.py
--rw-r--r--   0        0        0     3255 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/voice.py
--rw-r--r--   0        0        0     1152 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0        0 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/arona.py
--rw-r--r--   0        0        0     5814 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/bawiki.py
--rw-r--r--   0        0        0     9814 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/gamekee.py
--rw-r--r--   0        0        0    18830 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/schaledb.py
--rw-r--r--   0        0        0     7390 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0     1358 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/__init__.py
--rw-r--r--   0        0        0     1784 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/manual.py
--rw-r--r--   0        0        0     2216 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/pic_menu.py
--rw-r--r--   0        0        0      919 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/__init__.py
--rw-r--r--   0        0        0    21514 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-06-23 17:00:11.628459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gradient.png
--rw-r--r--   0        0        0     4596 2023-06-23 17:00:11.628459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1481 2023-06-23 17:01:03.804653 nonebot_plugin_bawiki-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10479 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/LICENSE
+-rw-r--r--   0        0        0     9414 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/README.md
+-rw-r--r--   0        0        0      734 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/__init__.py
+-rw-r--r--   0        0        0     3827 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/arona.py
+-rw-r--r--   0        0        0     2320 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/calender.py
+-rw-r--r--   0        0        0     1265 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/clear_cache.py
+-rw-r--r--   0        0        0     1218 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/craft.py
+-rw-r--r--   0        0        0     1003 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/emoji.py
+-rw-r--r--   0        0        0     2580 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/event.py
+-rw-r--r--   0        0        0      976 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/furniture.py
+-rw-r--r--   0        0        0     6327 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/gacha.py
+-rw-r--r--   0        0        0     3555 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/global_future.py
+-rw-r--r--   0        0        0     1775 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/level_guide.py
+-rw-r--r--   0        0        0     1428 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/manga.py
+-rw-r--r--   0        0        0     4356 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/raid.py
+-rw-r--r--   0        0        0     3597 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_fav.py
+-rw-r--r--   0        0        0     1868 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_rank.py
+-rw-r--r--   0        0        0     1625 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
+-rw-r--r--   0        0        0     2011 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_schale.py
+-rw-r--r--   0        0        0     3375 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/time_atk.py
+-rw-r--r--   0        0        0     3255 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/voice.py
+-rw-r--r--   0        0        0     1152 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0        0 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/arona.py
+-rw-r--r--   0        0        0     5814 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/bawiki.py
+-rw-r--r--   0        0        0     9814 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/gamekee.py
+-rw-r--r--   0        0        0    18830 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/schaledb.py
+-rw-r--r--   0        0        0     7390 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/gacha.py
+-rw-r--r--   0        0        0     1358 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/__init__.py
+-rw-r--r--   0        0        0     1784 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/manual.py
+-rw-r--r--   0        0        0     2216 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/pic_menu.py
+-rw-r--r--   0        0        0      919 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/__init__.py
+-rw-r--r--   0        0        0    21514 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-06-25 16:15:31.678212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gradient.png
+-rw-r--r--   0        0        0     4596 2023-06-25 16:15:31.678212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1481 2023-06-25 16:16:03.258182 nonebot_plugin_bawiki-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.1/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.8.0/LICENSE` & `nonebot_plugin_bawiki-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/README.md` & `nonebot_plugin_bawiki-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,23 @@
 |    `BA_SCHALE_MIRROR_URL`     |  否  |   ...   |                  SchaleDB 网页截图的地址                  |
 |      `BA_BAWIKI_DB_URL`       |  否  |   ...   |                    bawiki-data 的地址                     |
 |      `BA_ARONA_API_URL`       |  否  |   ...   |                  Arona Bot 数据源的地址                   |
 |      `BA_ARONA_CDN_URL`       |  否  |   ...   |                  Arona Bot 图片 CDN 地址                  |
 | `BA_CLEAR_REQ_CACHE_INTERVAL` |  否  |   `3`   |             插件清理请求缓存的间隔，单位小时              |
 |  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  |   ...   | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
 
+由于 CDN 可能并不给力，如果有条件的话本人推荐使用代理直接访问原地址，下面是对应 `.env` 配置：
+
+```ini
+BA_PROXY=http://127.0.0.1:7890
+BA_SCHALE_URL=https://schale.gg/
+BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
+BA_BAWIKI_DB_URL=https://bawiki.lgc2333.top/
+```
+
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
 **现在 BAWiki 会自动帮你把 PicMenu 的字体设为系统已安装的字体，再也不需要麻烦的手动配置了，好耶~**
@@ -162,14 +171,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.1
+
+- 使用 `arona` 指令模糊搜索的时候会显示图片类别了
+
 ### 0.8.0
 
 - 整理项目结构
 - 添加内置帮助指令 `ba帮助`
 - 添加 Arona Bot 数据源指令 `arona`
 - 添加了配置项 `BA_ARONA_API_URL`、`BA_ARONA_CDN_URL`、`BA_CLEAR_REQ_CACHE_INTERVAL`、`BA_AUTO_CLEAR_ARONA_CACHE`
 - 其他小更改（更换 `aiohttp` 为 `httpx` 等）
```

#### html2text {}

```diff
@@ -31,31 +31,36 @@
 ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
 çå°å | | `BA_ARONA_API_URL` | å¦ | ... | Arona Bot æ°æ®æºçå°å | |
 `BA_ARONA_CDN_URL` | å¦ | ... | Arona Bot å¾ç CDN å°å | |
 `BA_CLEAR_REQ_CACHE_INTERVAL` | å¦ | `3` |
 æä»¶æ¸çè¯·æ±ç¼å­çé´éï¼åä½å°æ¶ | |
 `BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | ... |
 æ¯å¦å¨æä»¶æ¯æ¬¡å è½½æ¶èªå¨æ¸çä» Arona Bot
-æ°æ®æºç¼å­çå¾ç | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
-ä¼èªå¨å¸®ä½ æ PicMenu
+æ°æ®æºç¼å­çå¾ç | ç±äº CDN
+å¯è½å¹¶ä¸ç»åï¼å¦æææ¡ä»¶çè¯æ¬äººæ¨èä½¿ç¨ä»£çç´æ¥è®¿é®åå°åï¼ä¸é¢æ¯å¯¹åº
+`.env` éç½®ï¼ ```ini BA_PROXY=http://127.0.0.1:7890 BA_SCHALE_URL=https://
+schale.gg/ BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
+BA_BAWIKI_DB_URL=https://bawiki.lgc2333.top/ ``` ## ð ä½¿ç¨ ### æä»¤è¡¨
+å¼å®¹ [nonebot-plugin-PicMenu](https://github.com/hamo-reid/
+nonebot_plugin_PicMenu) **ç°å¨ BAWiki ä¼èªå¨å¸®ä½ æ PicMenu
 çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
 å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹ä½¿ç¨ `baå¸®å©` æä»¤å³å¯ï¼
 å¦æè£è½½äº PicMenuï¼`baå¸®å©` æä»¤ä¼è°ç¨ PicMenu
 æ¥çæå¸®å©å¾çå¹¶åé ## ð èç³» QQï¼3076823485 Telegramï¼
 [@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
+0.8.1 - ä½¿ç¨ `arona` æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ###
 0.8.0 - æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona
 Bot æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
 `BA_ARONA_API_URL`ã`BA_ARONA_CDN_URL`ã`BA_CLEAR_REQ_CACHE_INTERVAL`ã`BA_AUTO_CLEAR_ARONA_CACHE`
 - å¶ä»å°æ´æ¹ï¼æ´æ¢ `aiohttp` ä¸º `httpx` ç­ï¼ ### 0.7.10 -
 æ·»å æä»¤ `baå³å¡` ### 0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ###
 0.7.8 - ð NoneBot 2.0 ð ### 0.7.7 - ä¿®å¤ bug ### 0.7.6 -
 ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
```

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from .command import load_commands  # noqa: E402
 from .config import Cfg as Cfg  # noqa: E402
 from .help import extra, register_help_cmd, usage  # noqa: E402
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=usage,
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki",
     type="application",
     config=Cfg,
```

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/__init__.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/arona.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/arona.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from nonebot import logger, on_command
 from nonebot.adapters.onebot.v11 import Message, MessageEvent, MessageSegment
 from nonebot.internal.matcher import Matcher
 from nonebot.params import ArgPlainText, CommandArg
 from nonebot.typing import T_State
 
-from ..data.arona import ImageModel, get_image, search
+from ..data.arona import IMAGE_TYPE_MAP, ImageModel, get_image, search
 
 if TYPE_CHECKING:
     from . import HelpList
 
 help_list: "HelpList" = [
     {
         "func": "Arona数据源攻略",
@@ -74,18 +74,20 @@
     if not res:
         await matcher.finish("没有找到相关图片")
 
     if len(res) == 1:
         await send_image(matcher, res[0])
 
     state["res"] = res
+    list_txt = "\n".join(
+        f"{i}. {r.name} ({IMAGE_TYPE_MAP.get(r.type, '未知分类')})"
+        for i, r in enumerate(res, 1)
+    )
     await matcher.pause(
-        "Arona 查到了多个结果，请 sensei 发送序号选择~\n"
-        + "\n".join(f"{i}. {r.name}" for i, r in enumerate(res, 1))
-        + "\nTip：发送 0 取消选择",
+        f"Arona 查到了多个结果，请 sensei 发送序号选择~\n{list_txt}\nTip：发送 0 取消选择",
     )
 
 
 @cmd_arona.handle()
 async def _(event: MessageEvent, matcher: Matcher, state: T_State):
     index_str = event.get_plaintext().strip()
     res: List[ImageModel] = state["res"]
```

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/calender.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/calender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/clear_cache.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/clear_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/craft.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/craft.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/emoji.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/emoji.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/event.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/furniture.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/furniture.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/gacha.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/global_future.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/global_future.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/level_guide.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/level_guide.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/manga.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/manga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/raid.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/raid.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_fav.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_fav.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_rank.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_wiki_schale.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_schale.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/time_atk.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/time_atk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/voice.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/voice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/arona.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/arona.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/bawiki.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/gamekee.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/schaledb.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/schaledb.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/__init__.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/manual.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/manual.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/pic_menu.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/pic_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/__init__.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/calender_banner.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_new.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_star.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gradient.png` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.0/pyproject.toml` & `nonebot_plugin_bawiki-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.8.0"
+version = "0.8.1"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.1",
```

### Comparing `nonebot_plugin_bawiki-0.8.0/PKG-INFO` & `nonebot_plugin_bawiki-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.8.0
+Version: 0.8.1
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -149,14 +149,23 @@
 |    `BA_SCHALE_MIRROR_URL`     |  否  |   ...   |                  SchaleDB 网页截图的地址                  |
 |      `BA_BAWIKI_DB_URL`       |  否  |   ...   |                    bawiki-data 的地址                     |
 |      `BA_ARONA_API_URL`       |  否  |   ...   |                  Arona Bot 数据源的地址                   |
 |      `BA_ARONA_CDN_URL`       |  否  |   ...   |                  Arona Bot 图片 CDN 地址                  |
 | `BA_CLEAR_REQ_CACHE_INTERVAL` |  否  |   `3`   |             插件清理请求缓存的间隔，单位小时              |
 |  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  |   ...   | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
 
+由于 CDN 可能并不给力，如果有条件的话本人推荐使用代理直接访问原地址，下面是对应 `.env` 配置：
+
+```ini
+BA_PROXY=http://127.0.0.1:7890
+BA_SCHALE_URL=https://schale.gg/
+BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
+BA_BAWIKI_DB_URL=https://bawiki.lgc2333.top/
+```
+
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
 **现在 BAWiki 会自动帮你把 PicMenu 的字体设为系统已安装的字体，再也不需要麻烦的手动配置了，好耶~**
@@ -197,14 +206,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.1
+
+- 使用 `arona` 指令模糊搜索的时候会显示图片类别了
+
 ### 0.8.0
 
 - 整理项目结构
 - 添加内置帮助指令 `ba帮助`
 - 添加 Arona Bot 数据源指令 `arona`
 - 添加了配置项 `BA_ARONA_API_URL`、`BA_ARONA_CDN_URL`、`BA_CLEAR_REQ_CACHE_INTERVAL`、`BA_AUTO_CLEAR_ARONA_CACHE`
 - 其他小更改（更换 `aiohttp` 为 `httpx` 等）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.0 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.1 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -51,31 +51,36 @@
 ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
 çå°å | | `BA_ARONA_API_URL` | å¦ | ... | Arona Bot æ°æ®æºçå°å | |
 `BA_ARONA_CDN_URL` | å¦ | ... | Arona Bot å¾ç CDN å°å | |
 `BA_CLEAR_REQ_CACHE_INTERVAL` | å¦ | `3` |
 æä»¶æ¸çè¯·æ±ç¼å­çé´éï¼åä½å°æ¶ | |
 `BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | ... |
 æ¯å¦å¨æä»¶æ¯æ¬¡å è½½æ¶èªå¨æ¸çä» Arona Bot
-æ°æ®æºç¼å­çå¾ç | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
-ä¼èªå¨å¸®ä½ æ PicMenu
+æ°æ®æºç¼å­çå¾ç | ç±äº CDN
+å¯è½å¹¶ä¸ç»åï¼å¦æææ¡ä»¶çè¯æ¬äººæ¨èä½¿ç¨ä»£çç´æ¥è®¿é®åå°åï¼ä¸é¢æ¯å¯¹åº
+`.env` éç½®ï¼ ```ini BA_PROXY=http://127.0.0.1:7890 BA_SCHALE_URL=https://
+schale.gg/ BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
+BA_BAWIKI_DB_URL=https://bawiki.lgc2333.top/ ``` ## ð ä½¿ç¨ ### æä»¤è¡¨
+å¼å®¹ [nonebot-plugin-PicMenu](https://github.com/hamo-reid/
+nonebot_plugin_PicMenu) **ç°å¨ BAWiki ä¼èªå¨å¸®ä½ æ PicMenu
 çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
 å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹ä½¿ç¨ `baå¸®å©` æä»¤å³å¯ï¼
 å¦æè£è½½äº PicMenuï¼`baå¸®å©` æä»¤ä¼è°ç¨ PicMenu
 æ¥çæå¸®å©å¾çå¹¶åé ## ð èç³» QQï¼3076823485 Telegramï¼
 [@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
+0.8.1 - ä½¿ç¨ `arona` æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ###
 0.8.0 - æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona
 Bot æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
 `BA_ARONA_API_URL`ã`BA_ARONA_CDN_URL`ã`BA_CLEAR_REQ_CACHE_INTERVAL`ã`BA_AUTO_CLEAR_ARONA_CACHE`
 - å¶ä»å°æ´æ¹ï¼æ´æ¢ `aiohttp` ä¸º `httpx` ç­ï¼ ### 0.7.10 -
 æ·»å æä»¤ `baå³å¡` ### 0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ###
 0.7.8 - ð NoneBot 2.0 ð ### 0.7.7 - ä¿®å¤ bug ### 0.7.6 -
 ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
```

