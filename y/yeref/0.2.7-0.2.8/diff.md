# Comparing `tmp/yeref-0.2.7.tar.gz` & `tmp/yeref-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.7.tar", last modified: Sun Jun 25 10:02:34 2023, max compression
+gzip compressed data, was "yeref-0.2.8.tar", last modified: Sun Jun 25 10:12:02 2023, max compression
```

## Comparing `yeref-0.2.7.tar` & `yeref-0.2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:02:34.134276 yeref-0.2.7/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:02:34.134577 yeref-0.2.7/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 10:02:34.135677 yeref-0.2.7/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-25 10:02:15.000000 yeref-0.2.7/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:02:34.127257 yeref-0.2.7/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.7/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   558236 2023-06-25 10:01:51.000000 yeref-0.2.7/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   211219 2023-06-23 18:30:42.000000 yeref-0.2.7/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:02:34.133441 yeref-0.2.7/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:12:02.778665 yeref-0.2.8/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:12:02.778916 yeref-0.2.8/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 10:12:02.779823 yeref-0.2.8/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-25 10:11:22.000000 yeref-0.2.8/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:12:02.765372 yeref-0.2.8/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.8/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558219 2023-06-25 10:11:22.000000 yeref-0.2.8/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   211219 2023-06-23 18:30:42.000000 yeref-0.2.8/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:12:02.777309 yeref-0.2.8/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.7/setup.py` & `yeref-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.07',
+      version='0.2.08',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.7/yeref/l_.py` & `yeref-0.2.8/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
     'en': "❗️ <b>Number of characters</b> of text ( <i>including formatting</i> ): <u>{0}</u> more than allowed 1024",
     'es': "❗️ <b>Número de caracteres</b> de texto ( <i>incluido el formato</i> ): <u>{0}</u> más de los permitidos 1024",
     'fr': "❗️ <b>Nombre de caractères</b> de texte ( <i>y compris le formatage</i> ) : <u>{0}</u> plus que autorisé 1024",
     'zh': "❗️ 文本<b>字符数</b>（<i>包括格式</i>）： <u>{0}</u>超过允许的 1024",
     'ar': "❗️ <b>عدد أحرف</b> النص ( <i>بما في ذلك التنسيق</i> ): <u>{0}</u> أكثر من العدد المسموح به وهو 1024",
 }
 l_post_finish = {
-    'ru': "✅ <b>Пост готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку 🔗 Опубликовать</i>",
+    'ru': "✅ <b>Пост готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку 🔗 Публикация</i>",
     'en': "✅ <b>Post is ready</b>\n\n<i>Press &quot;➡️️/Next&quot; to confirm, and then press the button 🔗 Publish</i>",
     'es': "✅ <b>La publicación está lista</b>\n\n<i>Presiona &quot;➡️️/Siguiente&quot; para confirmar y luego presiona el botón 🔗 Publicar</i>",
     'fr': "✅ <b>La publication est prête</b>\n\n<i>Appuyez sur &quot;➡️️/Suivant&quot; pour confirmer, puis appuyez sur le bouton 🔗 Publier</i>",
     'zh': "✅<b>发布准备就绪</b>\n\n<i>按“➡️️/Next”确认，然后按按钮🔗发布</i>",
     'ar': "✅ <b>النشر جاهز</b>\n\n<i>اضغط على &quot;➡️️ / التالي&quot; للتأكيد ، ثم اضغط على الزر 🔗 نشر</i>",
 }
 l_switch_pm_text = {
@@ -429,15 +429,15 @@
     'es': "<b>fecha de creación</b>",
     'fr': "<b>date de création</b>",
     'zh': "<b>创建日期</b>",
     'ar': "<b>تاريخ الخلق</b>",
 }
 
 l_post_publish = {
-    'ru': "🔗 Опубликовать",
+    'ru': "🔗 Публикация",
     'en': "🔗 Post",
     'es': "🔗 Publicar",
     'fr': "🔗 Publier",
     'zh': "🔗 发布",
     'ar': "🔗 مشاركة",
 }
 l_post_pub = {
@@ -695,15 +695,15 @@
     'en': "📧 <b>Done!</b> Newsletter scheduled",
     'es': "📧 <b>Listo!</b> Boletín programado",
     'fr': "📧 <b>C&#x27;est fait !</b> Newsletter prévue",
     'zh': "📧<b>完成！</b>已安排时事通讯",
     'ar': "📧 <b>انتهى!</b> النشرة الإخبارية المجدولة",
 }
 l_broadcast_plan_bot = {
-    'ru': "📧 <b>Готово!</b> Рассылка запланирована в @{0} на {1}",
+    'ru': "📧 <b>Готово!</b> Рассылка запланирована в @{0}",
     'en': "📧 <b>Done!</b> Mailing scheduled for @{0}",
     'es': "📧 <b>Listo!</b> Envío programado para @{0}",
     'fr': "📧 <b>C&#x27;est fait !</b> Envoi prévu pour @{0}",
     'zh': "📧<b>完成！</b>邮寄安排在@{0}",
     'ar': "📧 <b>انتهى!</b> تمت جدولة الإرسال في @ {0}",
 }
 l_broadcast_start = {
```

### Comparing `yeref-0.2.7/yeref/yeref.py` & `yeref-0.2.8/yeref/yeref.py`

 * *Files identical despite different names*

