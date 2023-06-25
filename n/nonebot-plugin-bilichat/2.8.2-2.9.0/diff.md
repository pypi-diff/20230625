# Comparing `tmp/nonebot_plugin_bilichat-2.8.2.tar.gz` & `tmp/nonebot_plugin_bilichat-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.8.2.tar", last modified: Sat Jun 24 11:10:42 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.9.0.tar", last modified: Sun Jun 25 07:30:29 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.8.2.tar` & `nonebot_plugin_bilichat-2.9.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0    34523 2023-06-24 11:10:33.094688 nonebot_plugin_bilichat-2.8.2/LICENSE
--rw-r--r--   0        0        0    12397 2023-06-24 11:10:33.094688 nonebot_plugin_bilichat-2.8.2/README.md
--rw-r--r--   0        0        0     9690 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5767 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      844 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      871 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    16355 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     2773 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7534 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     2098 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    27644 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/newbing.png
--rw-r--r--   0        0        0    59199 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     1363 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4932 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2200 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     3133 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-24 11:10:42.206816 nonebot_plugin_bilichat-2.8.2/pyproject.toml
--rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-25 07:30:21.054542 nonebot_plugin_bilichat-2.9.0/LICENSE
+-rw-r--r--   0        0        0    12710 2023-06-25 07:30:21.054542 nonebot_plugin_bilichat-2.9.0/README.md
+-rw-r--r--   0        0        0     9690 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     6614 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      844 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      871 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16355 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     2773 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0     3638 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7534 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     2098 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    27644 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/newbing.png
+-rw-r--r--   0        0        0    59199 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     1403 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0    24930 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/newbing.py
+-rw-r--r--   0        0        0     6711 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4932 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2200 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     3110 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1419 2023-06-25 07:30:29.750815 nonebot_plugin_bilichat-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14096 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.9.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.8.2/LICENSE` & `nonebot_plugin_bilichat-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/README.md` & `nonebot_plugin_bilichat-2.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -142,41 +142,42 @@
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr       | bool      | True  | 是否在**没有字幕时**调用必剪接口生成字幕 |
 | bilichat_show_error_msg     | bool      | True  | 是否在解析失败时发送错误信息 |
+| bilichat_use_browser        | bool      | Auto  | 是否使用浏览器，`Auto` 会根据是否含有相应的依赖进行选择 |
 
 注:
 
 1. 由于 OneBot 协议未规定是否应上报自身事件，因此在不同的场景下能否获取自身事件并不一定，`bilichat_enable_self` 实际能否生效也与之相关
 2. 当 `bilichat_whitelist` 存在时，`bilichat_blacklist` 将会被禁用
 3. `bilichat_dynamic_font` 可填写自定义的字体url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成AI字幕时，根据视频时长和网络情况有可能会识别失败，Bot会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
 
 ### 基础信息配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_basic_info          | bool | True         | 是否开启视频基本信息 |
-| bilichat_basic_info_style    | str  | bbot_default | 视频详情的图片样式，可用样式见下方备注 |
-| bilichat_basic_info_url      | bool | True         | 开启视频进本信息的情况下，是否一同回复一个链接 |
-| bilichat_reply_to_basic_info | bool | True         | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
+| bilichat_basic_info          | bool | True    | 是否开启视频基本信息 |
+| bilichat_basic_info_style    | str  | default | 视频详情的图片样式，可用样式见下方备注 |
+| bilichat_basic_info_url      | bool | True    | 开启视频进本信息的情况下，是否一同回复一个链接 |
+| bilichat_reply_to_basic_info | bool | True    | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
 
-注：bilichat_basic_info_style 除默认的 bbot_default 使用 PIL 绘图，其他均依赖于 `nonebot-plugin-htmlrender`，其可用的样式如下所示
+注：bilichat_basic_info_style 除默认的 bbot_default 使用 PIL 绘图（未开启浏览器时默认选择），其他均依赖于浏览器进行渲染（需要设置 bilichat_use_browser 为 True 或 Auto），其可用的样式如下所示
 
 <details>
-<summary>bbot_default</summary>
+<summary>bbot_default（无浏览器时默认）</summary>
 
 ![](docs/bbot_default.png)
 </details>
 
 <details>
-<summary>style_blue</summary>
+<summary>style_blue（有浏览器时默认）</summary>
 
 ![](docs/style_blue.png)
 </details>
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
@@ -185,19 +186,19 @@
 |:-----:|:----:|:----:|:----:|
 | bilichat_word_cloud  | bool | False | 是否开启词云功能 |
 
 注：词云功能在 python3.11 中由于 `wordcloud` 包安装失败暂时无法启用，请不要在 3.11 中开启此功能
 
 ### AI视频总结配置项
 
-开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[openai,newbing]`
+开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[summary]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径, 填写 `no_login` 则不进行登录（可能有次数限制）, 若留空则禁用newbing总结 |
+| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径, 填写 `no_login` 则不进行登录（有限制）, 若留空则禁用newbing总结 |
 | bilichat_newbing_token_limit | int       | 0                  | newbing请求的文本量上限, 0为无上限 |
 | bilichat_newbing_preprocess  | bool      | True               | 是否对newbing的返回值进行预处理, 以去除其中不想要的内容 |
 | bilichat_openai_token        | str       | None               | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None               | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301 | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500               | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
@@ -247,11 +248,12 @@
 - [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
 - [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 - [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 - [nonebot-plugin-bing-chat](https://github.com/Harry-Jing/nonebot-plugin-bing-chat): newbing解析的代码参考
 - [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项BUG修复和代码参考
+- [hamo-reid](https://github.com/hamo-reid) 为 style_blue 绘制了界面
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -34,46 +34,49 @@
 | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
 True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_show_error_msg | bool | True |
-æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | æ³¨: 1. ç±äº OneBot
+æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | | bilichat_use_browser | bool |
+Auto | æ¯å¦ä½¿ç¨æµè§å¨ï¼`Auto`
+ä¼æ ¹æ®æ¯å¦å«æç¸åºçä¾èµè¿è¡éæ© | æ³¨: 1. ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
 å®éè½å¦çæä¹ä¸ä¹ç¸å³ 2. å½ `bilichat_whitelist`
 å­å¨æ¶ï¼`bilichat_blacklist` å°ä¼è¢«ç¦ç¨ 3. `bilichat_dynamic_font`
 å¯å¡«åèªå®ä¹çå­ä½urlï¼ä½å¹¶ä¸æ¨èä¿®æ¹ 4. å½ä½¿ç¨ `bcut_asr`
 æ¥å£æ¥çæAIå­å¹æ¶ï¼æ ¹æ®è§é¢æ¶é¿åç½ç»æåµæå¯è½ä¼è¯å«å¤±è´¥ï¼Botä¼æç¤º
 `BCut-ASR conversion failed due to network error`ãå¯ä»¥éè¿è°é«
 `bilichat_neterror_retry`
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ ###
 åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_basic_info | bool | True |
-æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str |
-bbot_default | è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
+æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str | default |
+è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
 bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
 bilichat_reply_to_basic_info | bool | True |
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) |
 æ³¨ï¼bilichat_basic_info_style é¤é»è®¤ç bbot_default ä½¿ç¨ PIL
-ç»å¾ï¼å¶ä»åä¾èµäº `nonebot-plugin-
-htmlrender`ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º  bbot_default ![](docs/
-bbot_default.png)   style_blue ![](docs/style_blue.png)  ### è¯äºéç½®é¡¹
-å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bilichat_word_cloud | bool | False | æ¯å¦å¼å¯è¯äºåè½ |
-æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº `wordcloud`
-åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11 ä¸­å¼å¯æ­¤åè½ ###
-AIè§é¢æ»ç»éç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-
-plugin-bilichat[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:
------:|:----:|:----:|:----:| | bilichat_newbing_cookie | str | None |
-newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
-åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
-| | bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
+ç»å¾ï¼æªå¼å¯æµè§å¨æ¶é»è®¤éæ©ï¼ï¼å¶ä»åä¾èµäºæµè§å¨è¿è¡æ¸²æï¼éè¦è®¾ç½®
+bilichat_use_browser ä¸º True æ Autoï¼ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º
+bbot_defaultï¼æ æµè§å¨æ¶é»è®¤ï¼ ![](docs/bbot_default.png)
+style_blueï¼ææµè§å¨æ¶é»è®¤ï¼ ![](docs/style_blue.png)  ###
+è¯äºéç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-
+bilichat[wordcloud]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
+-:|:----:|:----:| | bilichat_word_cloud | bool | False |
+æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
+`wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
+ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
+å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[summary]` |
+éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾, å¡«å
+`no_login` åä¸è¿è¡ç»å½ï¼æéå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç» |
+| bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess | bool | True |
 æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç, ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹
 | | bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str | None |
 è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
 gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
 bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
@@ -120,10 +123,11 @@
 åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
 BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
 github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [nonebot-plugin-bing-chat](https://github.com/Harry-
 Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè - [Misaka-Mikoto-
 Tech](https://github.com/Misaka-Mikoto-Tech)
-ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹BUGä¿®å¤åä»£ç åè ## â³ Star è¶å¿ [!
+ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹BUGä¿®å¤åä»£ç åè - [hamo-reid](https://
+github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ ## â³ Star è¶å¿ [!
 [Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
 bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import sys
 from pathlib import Path
 from typing import List, Literal, Optional, Union
 
 from nonebot import get_driver, require
 from nonebot.log import logger
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, Field, validator
 
 # get package version
 if sys.version_info < (3, 10):
     from importlib_metadata import version
 else:
     from importlib.metadata import version
 
@@ -29,18 +29,19 @@
     bilichat_enable_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
     bilichat_cd_time: int = 120
     bilichat_neterror_retry: int = 3
     bilichat_show_error_msg: bool = True
+    bilichat_use_browser: bool = Field(default="Auto")
 
     # basic info
     bilichat_basic_info: bool = True
-    bilichat_basic_info_style: Literal["bbot_default", "style_blue"] = "bbot_default"
+    bilichat_basic_info_style: Literal["bbot_default", "style_blue"] = Field(default="default")
     bilichat_basic_info_url: bool = True
     bilichat_reply_to_basic_info: bool = True
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
@@ -61,14 +62,45 @@
         "gpt-4",
         "gpt-4-0314",
         "gpt-4-0613",
         "gpt-4-32k-0314",
     ] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
 
+    @validator("bilichat_use_browser", always=True, pre=True)
+    def check_htmlrender(cls, v):
+        if not v:
+            return v
+        try:
+            require("nonebot_plugin_htmlrender")
+            if v == "Auto":
+                logger.info("bilichat_use_browser dependencies have been satisfied, enable bilichat_use_browser")
+            return True
+        except Exception as e:
+            if v == "Auto":
+                logger.info("bilichat_use_browser's dependency is not satisfied, disable bilichat_use_browser")
+                return False
+            raise RuntimeError(
+                "Package(s) of fuction styles not installed, use **pip install nonebot-plugin-bilichat[extra]** to install required dependencies"
+            ) from e
+
+    @validator("bilichat_basic_info_style", always=True,pre=True)
+    def check_use_browser(cls, v, values):
+        if v == "bbot_default":
+            return v
+        # 不包含浏览器
+        if values["bilichat_use_browser"] != True:
+            if v == "default":
+                return "bbot_default"
+            raise RuntimeError(
+                f"style {v} require browser to work, please enable **bilichat_use_browser** or set style to default"
+            )
+        # 包含浏览器
+        return "style_blue" if v == "default" else v
+
     @validator("bilichat_openai_proxy", always=True, pre=True)
     def check_openai_proxy(cls, v, values):
         if not (values["bilichat_openai_token"] or values["bilichat_newbing_cookie"]):
             return v
         if v is None:
             logger.warning(
                 "you have enabled openai or newbing summary without a proxy, this may cause request failure."
@@ -97,24 +129,24 @@
 
     @validator("bilichat_openai_token", always=True)
     def check_pypackage_openai(cls, v):
         if (importlib.util.find_spec("tiktoken_async") and importlib.util.find_spec("minidynamicrender")) or not v:
             return v
         else:
             raise RuntimeError(
-                "Package(s) of fuction openai summary not installed, use **pip install nonebot-plugin-bilichat[openai]** to install required dependencies"
+                "Package(s) of fuction openai summary not installed, use **pip install nonebot-plugin-bilichat[summary]** to install required dependencies"
             )
 
     @validator("bilichat_newbing_cookie", always=True)
     def check_pypackage_newbing_and_cookie(cls, v):
         if not v:
             return v
-        if not importlib.util.find_spec("EdgeGPT") or not importlib.util.find_spec("minidynamicrender"):
+        if not importlib.util.find_spec("minidynamicrender"):
             raise RuntimeError(
-                "Package(s) of fuction newbing summary not installed, use **pip install nonebot-plugin-bilichat[newbing]** to install required dependencies"
+                "Package(s) of fuction newbing summary not installed, use **pip install nonebot-plugin-bilichat[summary]** to install required dependencies"
             )
 
         # verify cookie file
         if Path(v).is_file():
             try:
                 json.loads(Path(v).read_text("utf-8"))
             except Exception as e:
@@ -136,27 +168,14 @@
         if (importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")) or not v:
             return v
         else:
             raise RuntimeError(
                 "Package(s) of fuction wordcloud not installed, use **pip install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
             )
 
-    @validator("bilichat_basic_info_style", always=True)
-    def check_htmlrender(cls, v):
-        if v == "bbot_default":
-            return v
-        else:
-            try:
-                require("nonebot_plugin_htmlrender")
-                return v
-            except Exception as e:
-                raise RuntimeError(
-                    "Package(s) of fuction styles not installed, use **pip install nonebot-plugin-bilichat[extra]** to install required dependencies"
-                ) from e
-
     def verify_permission(self, uid: Union[str, int]):
         if self.bilichat_whitelist:
             return str(uid) in self.bilichat_whitelist
         elif self.bilichat_blacklist:
             return str(uid) not in self.bilichat_blacklist
         else:
             return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/newbing.png` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/newbing.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     # openai cache -> newbing cache -> newbing new sum -> openai new sum
     logger.info(f"Generation summary of Video(Column) {cache.id}")
     if not cache.episodes[cid] or not cache.episodes[cid].content:
         return "视频无有效字幕"
 
     # try using openai cache
     # this will not cause new summarization
-    if cache.episodes[cid].openai:
+    if cache.episodes[cid].openai and plugin_config.bilichat_openai_token:
         return await openai_summarization(cache, cid)
     
     # try newbing
     if plugin_config.bilichat_newbing_cookie:
         summary, newbing_meaning = await newbing_summarization(cache, cid)
         if newbing_meaning or not plugin_config.bilichat_openai_token:
             return summary
```

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import json
 import random
 import re
 from collections import OrderedDict
 from pathlib import Path
 from typing import List, Literal
 
-from EdgeGPT import Chatbot, ConversationStyle
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..lib.store import BING_APOLOGY
 from ..model.cache import Cache
 from ..model.exception import AbortError, BingChatResponseException
 from ..model.newbing import BingChatResponse
 from ..optional import capture_exception  # type: ignore
+from .newbing import Chatbot, ConversationStyle
 from .text_to_image import t2i
 
 cookies = (
     {}
     if plugin_config.bilichat_newbing_cookie == "no_login"
     else json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
 )
```

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,13 +77,13 @@
     return img_raw
 
 
 async def t2i(data: str, src: str):
     try:
         if len(data) < 30:
             return data
-        if plugin_config.bilichat_basic_info_style != "bbot_default":
+        if plugin_config.bilichat_use_browser:
             return await pw_text2image(data, src)
         return await rich_text2image(data, src)
     except Exception as e:
         logger.exception(e)
         return f"总结图片生成失败 {e}\n {data}"
```

### Comparing `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.2/pyproject.toml` & `nonebot_plugin_bilichat-2.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=23.3.0",
     "nonebot-plugin-all4one>=0.1.0a2",
     "nonebot2[fastapi,websockets]>=2.0.0rc4",
 ]
-test = [
-    "nonebug>=0.3.2",
-    "pytest-asyncio>=0.21.0",
-]
 
 [tool.black]
 line-length = 120
 target-version = [
     "py38",
     "py39",
     "py310",
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.8.2"
+version = "2.9.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
@@ -49,31 +45,26 @@
     "nonebot-plugin-sentry>=0.2.2",
     "nonebot-plugin-htmlrender>=0.2.0.3",
 ]
 wordcloud = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
 ]
-openai = [
+summary = [
     "tiktoken-async>=0.3.2",
     "minidynamicrender>=1.1.9",
-]
-newbing = [
-    "EdgeGPT>=0.1.22.1,<0.9.0",
-    "minidynamicrender>=1.1.9",
-    "setuptools",
+    "aiohttp>=3.8.4",
 ]
 all = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
     "tiktoken-async>=0.3.2",
-    "EdgeGPT>=0.1.22.1,<0.9.0",
     "minidynamicrender>=1.1.9",
     "nonebot-plugin-htmlrender>=0.2.0.3",
-    "setuptools",
+    "aiohttp>=3.8.4",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_bilichat-2.8.2/PKG-INFO` & `nonebot_plugin_bilichat-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.8.2
+Version: 2.9.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -13,30 +13,26 @@
 Requires-Dist: nonebot-adapter-onebot>=2.2.2
 Requires-Dist: nonebot-plugin-segbuilder>=0.2.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
-Requires-Dist: tiktoken-async>=0.3.2; extra == "openai"
-Requires-Dist: minidynamicrender>=1.1.9; extra == "openai"
-Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "newbing"
-Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
-Requires-Dist: setuptools; extra == "newbing"
+Requires-Dist: tiktoken-async>=0.3.2; extra == "summary"
+Requires-Dist: minidynamicrender>=1.1.9; extra == "summary"
+Requires-Dist: aiohttp>=3.8.4; extra == "summary"
 Requires-Dist: jieba>=0.42.1; extra == "all"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "all"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "all"
-Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "all"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "all"
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "all"
-Requires-Dist: setuptools; extra == "all"
+Requires-Dist: aiohttp>=3.8.4; extra == "all"
 Provides-Extra: extra
 Provides-Extra: wordcloud
-Provides-Extra: openai
-Provides-Extra: newbing
+Provides-Extra: summary
 Provides-Extra: all
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="docs/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="docs/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -180,41 +176,42 @@
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr       | bool      | True  | 是否在**没有字幕时**调用必剪接口生成字幕 |
 | bilichat_show_error_msg     | bool      | True  | 是否在解析失败时发送错误信息 |
+| bilichat_use_browser        | bool      | Auto  | 是否使用浏览器，`Auto` 会根据是否含有相应的依赖进行选择 |
 
 注:
 
 1. 由于 OneBot 协议未规定是否应上报自身事件，因此在不同的场景下能否获取自身事件并不一定，`bilichat_enable_self` 实际能否生效也与之相关
 2. 当 `bilichat_whitelist` 存在时，`bilichat_blacklist` 将会被禁用
 3. `bilichat_dynamic_font` 可填写自定义的字体url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成AI字幕时，根据视频时长和网络情况有可能会识别失败，Bot会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
 
 ### 基础信息配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_basic_info          | bool | True         | 是否开启视频基本信息 |
-| bilichat_basic_info_style    | str  | bbot_default | 视频详情的图片样式，可用样式见下方备注 |
-| bilichat_basic_info_url      | bool | True         | 开启视频进本信息的情况下，是否一同回复一个链接 |
-| bilichat_reply_to_basic_info | bool | True         | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
+| bilichat_basic_info          | bool | True    | 是否开启视频基本信息 |
+| bilichat_basic_info_style    | str  | default | 视频详情的图片样式，可用样式见下方备注 |
+| bilichat_basic_info_url      | bool | True    | 开启视频进本信息的情况下，是否一同回复一个链接 |
+| bilichat_reply_to_basic_info | bool | True    | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
 
-注：bilichat_basic_info_style 除默认的 bbot_default 使用 PIL 绘图，其他均依赖于 `nonebot-plugin-htmlrender`，其可用的样式如下所示
+注：bilichat_basic_info_style 除默认的 bbot_default 使用 PIL 绘图（未开启浏览器时默认选择），其他均依赖于浏览器进行渲染（需要设置 bilichat_use_browser 为 True 或 Auto），其可用的样式如下所示
 
 <details>
-<summary>bbot_default</summary>
+<summary>bbot_default（无浏览器时默认）</summary>
 
 ![](docs/bbot_default.png)
 </details>
 
 <details>
-<summary>style_blue</summary>
+<summary>style_blue（有浏览器时默认）</summary>
 
 ![](docs/style_blue.png)
 </details>
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
@@ -223,19 +220,19 @@
 |:-----:|:----:|:----:|:----:|
 | bilichat_word_cloud  | bool | False | 是否开启词云功能 |
 
 注：词云功能在 python3.11 中由于 `wordcloud` 包安装失败暂时无法启用，请不要在 3.11 中开启此功能
 
 ### AI视频总结配置项
 
-开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[openai,newbing]`
+开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[summary]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径, 填写 `no_login` 则不进行登录（可能有次数限制）, 若留空则禁用newbing总结 |
+| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径, 填写 `no_login` 则不进行登录（有限制）, 若留空则禁用newbing总结 |
 | bilichat_newbing_token_limit | int       | 0                  | newbing请求的文本量上限, 0为无上限 |
 | bilichat_newbing_preprocess  | bool      | True               | 是否对newbing的返回值进行预处理, 以去除其中不想要的内容 |
 | bilichat_openai_token        | str       | None               | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None               | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301 | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500               | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
@@ -285,11 +282,12 @@
 - [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
 - [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 - [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 - [nonebot-plugin-bing-chat](https://github.com/Harry-Jing/nonebot-plugin-bing-chat): newbing解析的代码参考
 - [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项BUG修复和代码参考
+- [hamo-reid](https://github.com/hamo-reid) 为 style_blue 绘制了界面
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -1,29 +1,26 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.8.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.9.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
 sentry>=0.2.2; extra == "extra" Requires-Dist: nonebot-plugin-
 htmlrender>=0.2.0.3; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
 "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud" Requires-
-Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-Dist:
-minidynamicrender>=1.1.9; extra == "openai" Requires-Dist:
-EdgeGPT<0.9.0,>=0.1.22.1; extra == "newbing" Requires-Dist:
-minidynamicrender>=1.1.9; extra == "newbing" Requires-Dist: setuptools; extra
-== "newbing" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
+Dist: tiktoken-async>=0.3.2; extra == "summary" Requires-Dist:
+minidynamicrender>=1.1.9; extra == "summary" Requires-Dist: aiohttp>=3.8.4;
+extra == "summary" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
 wordcloud>=1.8.2.2; extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra
-== "all" Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "all" Requires-Dist:
-minidynamicrender>=1.1.9; extra == "all" Requires-Dist: nonebot-plugin-
-htmlrender>=0.2.0.3; extra == "all" Requires-Dist: setuptools; extra == "all"
-Provides-Extra: extra Provides-Extra: wordcloud Provides-Extra: openai
-Provides-Extra: newbing Provides-Extra: all Description-Content-Type: text/
+== "all" Requires-Dist: minidynamicrender>=1.1.9; extra == "all" Requires-Dist:
+nonebot-plugin-htmlrender>=0.2.0.3; extra == "all" Requires-Dist:
+aiohttp>=3.8.4; extra == "all" Provides-Extra: extra Provides-Extra: wordcloud
+Provides-Extra: summary Provides-Extra: all Description-Content-Type: text/
 markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
                [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
 ## ð ä»ç»
@@ -57,46 +54,49 @@
 | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
 True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_show_error_msg | bool | True |
-æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | æ³¨: 1. ç±äº OneBot
+æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | | bilichat_use_browser | bool |
+Auto | æ¯å¦ä½¿ç¨æµè§å¨ï¼`Auto`
+ä¼æ ¹æ®æ¯å¦å«æç¸åºçä¾èµè¿è¡éæ© | æ³¨: 1. ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
 å®éè½å¦çæä¹ä¸ä¹ç¸å³ 2. å½ `bilichat_whitelist`
 å­å¨æ¶ï¼`bilichat_blacklist` å°ä¼è¢«ç¦ç¨ 3. `bilichat_dynamic_font`
 å¯å¡«åèªå®ä¹çå­ä½urlï¼ä½å¹¶ä¸æ¨èä¿®æ¹ 4. å½ä½¿ç¨ `bcut_asr`
 æ¥å£æ¥çæAIå­å¹æ¶ï¼æ ¹æ®è§é¢æ¶é¿åç½ç»æåµæå¯è½ä¼è¯å«å¤±è´¥ï¼Botä¼æç¤º
 `BCut-ASR conversion failed due to network error`ãå¯ä»¥éè¿è°é«
 `bilichat_neterror_retry`
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ ###
 åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_basic_info | bool | True |
-æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str |
-bbot_default | è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
+æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str | default |
+è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
 bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
 bilichat_reply_to_basic_info | bool | True |
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) |
 æ³¨ï¼bilichat_basic_info_style é¤é»è®¤ç bbot_default ä½¿ç¨ PIL
-ç»å¾ï¼å¶ä»åä¾èµäº `nonebot-plugin-
-htmlrender`ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º  bbot_default ![](docs/
-bbot_default.png)   style_blue ![](docs/style_blue.png)  ### è¯äºéç½®é¡¹
-å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bilichat_word_cloud | bool | False | æ¯å¦å¼å¯è¯äºåè½ |
-æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº `wordcloud`
-åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11 ä¸­å¼å¯æ­¤åè½ ###
-AIè§é¢æ»ç»éç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-
-plugin-bilichat[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:
------:|:----:|:----:|:----:| | bilichat_newbing_cookie | str | None |
-newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
-åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
-| | bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
+ç»å¾ï¼æªå¼å¯æµè§å¨æ¶é»è®¤éæ©ï¼ï¼å¶ä»åä¾èµäºæµè§å¨è¿è¡æ¸²æï¼éè¦è®¾ç½®
+bilichat_use_browser ä¸º True æ Autoï¼ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º
+bbot_defaultï¼æ æµè§å¨æ¶é»è®¤ï¼ ![](docs/bbot_default.png)
+style_blueï¼ææµè§å¨æ¶é»è®¤ï¼ ![](docs/style_blue.png)  ###
+è¯äºéç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-
+bilichat[wordcloud]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
+-:|:----:|:----:| | bilichat_word_cloud | bool | False |
+æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
+`wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
+ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
+å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[summary]` |
+éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾, å¡«å
+`no_login` åä¸è¿è¡ç»å½ï¼æéå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç» |
+| bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess | bool | True |
 æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç, ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹
 | | bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str | None |
 è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
 gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
 bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
@@ -143,10 +143,11 @@
 åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
 BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
 github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [nonebot-plugin-bing-chat](https://github.com/Harry-
 Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè - [Misaka-Mikoto-
 Tech](https://github.com/Misaka-Mikoto-Tech)
-ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹BUGä¿®å¤åä»£ç åè ## â³ Star è¶å¿ [!
+ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹BUGä¿®å¤åä»£ç åè - [hamo-reid](https://
+github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ ## â³ Star è¶å¿ [!
 [Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
 bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

