# Comparing `tmp/yeref-0.2.6.tar.gz` & `tmp/yeref-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.6.tar", last modified: Fri Jun 23 16:53:05 2023, max compression
+gzip compressed data, was "yeref-0.2.7.tar", last modified: Sun Jun 25 10:02:34 2023, max compression
```

## Comparing `yeref-0.2.6.tar` & `yeref-0.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:53:05.983103 yeref-0.2.6/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:53:05.983258 yeref-0.2.6/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-23 16:53:05.983843 yeref-0.2.6/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-23 16:52:30.000000 yeref-0.2.6/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:53:05.978439 yeref-0.2.6/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.6/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.6/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   211218 2023-06-23 16:52:30.000000 yeref-0.2.6/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:53:05.982717 yeref-0.2.6/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:02:34.134276 yeref-0.2.7/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:02:34.134577 yeref-0.2.7/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 10:02:34.135677 yeref-0.2.7/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-25 10:02:15.000000 yeref-0.2.7/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:02:34.127257 yeref-0.2.7/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.7/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558236 2023-06-25 10:01:51.000000 yeref-0.2.7/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   211219 2023-06-23 18:30:42.000000 yeref-0.2.7/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:02:34.133441 yeref-0.2.7/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-25 10:02:34.000000 yeref-0.2.7/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.6/setup.py` & `yeref-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.06',
+      version='0.2.07',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.6/yeref/l_.py` & `yeref-0.2.7/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,15 +599,15 @@
     'en': "👩🏽‍💻 You have a premium account! In the <b>[Privacy]</b> settings, add @{0} to <i>the exclusions</i> for <b>[Voice Messages]</b> to display видео-заметку / голосовое",
     'es': "👩🏽‍💻 ¡Tienes una cuenta premium! En la configuración <b>de [Privacidad]</b> , agregue @{0} a <i>las exclusiones</i> de <b>[Mensajes de voz]</b> para mostrar видео-заметку / голосовое",
     'fr': "👩🏽‍💻 Vous avez un compte premium ! Dans les paramètres <b>[Confidentialité]</b> , ajoutez @{0} aux <i>exclusions</i> pour <b>[Messages vocaux]</b> pour afficher видео-заметку / голосовое",
     'zh': "👩🏽‍💻 您拥有高级帐户！在<b>[隐私]</b>设置中，将@{0}添加到<b>[语音消息]</b>的<i>排除项</i>中以显示видео-заметку / голосовое",
     'ar': "👩🏽‍💻 لديك حساب مميز! في إعدادات <b>[الخصوصية]</b> ، أضف @ {0} إلى <i>استثناءات</i> <b>[الرسائل الصوتية]</b> لعرض видео-заметку / голосовое",
 }
 l_post_tz = {
-    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 <b>Текуще</b>е время: <u>{0}</u> ({1}{2} по Гринвичу)",
+    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 <b>Текущее</b> время: <u>{0}</u> ({1}{2} по Гринвичу)",
     'en': "📍 Location <b>time zone</b> set\n\n🕐 <b>Current</b> time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora <b>actual</b> : <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure <b>actuelle</b> : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐<b>当前</b>时间： <u>{0}</u> （{1}{2} GMT）",
     'ar': "📍 تعيين <b>المنطقة الزمنية</b> للموقع\n\n🕐 الوقت <b>الحالي</b> : <u>{0}</u> ({1} {2} GMT)",
 }
 l_post_time_future = {
@@ -695,15 +695,15 @@
     'en': "📧 <b>Done!</b> Newsletter scheduled",
     'es': "📧 <b>Listo!</b> Boletín programado",
     'fr': "📧 <b>C&#x27;est fait !</b> Newsletter prévue",
     'zh': "📧<b>完成！</b>已安排时事通讯",
     'ar': "📧 <b>انتهى!</b> النشرة الإخبارية المجدولة",
 }
 l_broadcast_plan_bot = {
-    'ru': "📧 <b>Готово!</b> Рассылка запланирована в @{0}",
+    'ru': "📧 <b>Готово!</b> Рассылка запланирована в @{0} на {1}",
     'en': "📧 <b>Done!</b> Mailing scheduled for @{0}",
     'es': "📧 <b>Listo!</b> Envío programado para @{0}",
     'fr': "📧 <b>C&#x27;est fait !</b> Envoi prévu pour @{0}",
     'zh': "📧<b>完成！</b>邮寄安排在@{0}",
     'ar': "📧 <b>انتهى!</b> تمت جدولة الإرسال في @ {0}",
 }
 l_broadcast_start = {
@@ -728,15 +728,15 @@
     'es': "🏁 <b>Boletín</b> completado\n\n📧 <b>Número</b> de usuarios que recibieron el mensaje: <u>{0}</u>",
     'fr': "🏁 <b>Newsletter</b> terminée\n\n📧 <b>Nombre</b> d&#x27;utilisateurs ayant reçu le message : <u>{0}</u>",
     'zh': "🏁<b>通讯</b>已完成\n\n📧 收到消息的用户<b>数</b>： <u>{0}</u>",
     'ar': "🏁 اكتملت <b>النشرة الإخبارية</b>\n\n📧 <b>عدد</b> المستخدمين الذين تلقوا الرسالة: <u>{0}</u>",
 }
 
 l_generate_calendar_time = {
-    'ru': "🕒 <b>Отправь время</b> поста на {0} в формате {1}. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n🔗 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
+    'ru': "🕒 <b>Отправь время</b> поста на {0} в формате {1}. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n📍 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
     'en': "🕒 <b>Send the time</b> of the post to {0} in the format {1} . Current time: <u>{2}</u> ({3} GMT)\n\n🔗 Send <b>geolocation</b> to <i>automatically</i> determine the time zone",
     'es': "🕒 <b>Envía la hora</b> de la publicación a {0} en el formato {1} . Hora actual: <u>{2}</u> ({3} GMT)\n\n🔗 Enviar <b>geolocalización</b> para determinar <i>automáticamente</i> la zona horaria",
     'fr': "🕒 <b>Envoyez l&#x27;heure</b> de la publication à {0} au format {1} . Heure actuelle : <u>{2}</u> ({3} GMT)\n\n🔗 Envoyez <b>la géolocalisation</b> pour déterminer <i>automatiquement</i> le fuseau horaire",
     'zh': "🕒 以{1}格式将帖子<b>时间发送到</b>{0}。当前时间： <u>{2}</u> ({3} GMT)\n\n🔗 发送<b>地理定位</b>以<i>自动</i>确定时区",
     'ar': "🕒 <b>أرسل وقت</b> النشر إلى {0} بالتنسيق {1} . الوقت الحالي: <u>{2}</u> ({3} GMT)\n\n🔗 أرسل <b>الموقع الجغرافي</b> لتحديد المنطقة الزمنية <i>تلقائيًا</i>",
 }
 l_month_1 = {
```

### Comparing `yeref-0.2.6/yeref/yeref.py` & `yeref-0.2.7/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 
                     con.commit()
                     return cur.lastrowid
         except Exception as e:
             logger.info(log_ % str(e))
             await asyncio.sleep(round(random.uniform(1, 2), 2))
             retry -= 1
-    return 0
+    return -1
 
 
 async def db_bot_create(db):
     con = sqlite3.connect(db, timeout=10)
     try:
         cur = con.cursor()
```

