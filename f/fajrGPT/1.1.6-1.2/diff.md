# Comparing `tmp/fajrGPT-1.1.6.tar.gz` & `tmp/fajrGPT-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.1.6.tar", last modified: Mon Jun 12 01:18:23 2023, max compression
+gzip compressed data, was "fajrGPT-1.2.tar", last modified: Sun Jun 25 17:36:04 2023, max compression
```

## Comparing `fajrGPT-1.1.6.tar` & `fajrGPT-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:18:23.893493 fajrGPT-1.1.6/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.6/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:18:23.893287 fajrGPT-1.1.6/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.1.6/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:18:23.889788 fajrGPT-1.1.6/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.1.6/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.6/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     8176 2023-06-12 01:17:52.000000 fajrGPT-1.1.6/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:18:23.892795 fajrGPT-1.1.6/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-12 01:18:23.893542 fajrGPT-1.1.6/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-06-12 01:18:04.000000 fajrGPT-1.1.6/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-25 17:36:04.499924 fajrGPT-1.2/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.2/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-06-25 17:36:04.499758 fajrGPT-1.2/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.2/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-25 17:36:04.497516 fajrGPT-1.2/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.2/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.2/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     8697 2023-06-25 17:34:53.000000 fajrGPT-1.2/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-25 17:36:04.499565 fajrGPT-1.2/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-25 17:36:04.499962 fajrGPT-1.2/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1127 2023-06-25 17:35:52.000000 fajrGPT-1.2/setup.py
```

### Comparing `fajrGPT-1.1.6/LICENSE` & `fajrGPT-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.6/PKG-INFO` & `fajrGPT-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.6
+Version: 1.2
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.1.6/README.md` & `fajrGPT-1.2/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.6/fajrGPT/quran_metadata.py` & `fajrGPT-1.2/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.6/fajrGPT/wake.py` & `fajrGPT-1.2/fajrGPT/wake.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,40 +14,58 @@
 from Quran_Module import Project_Quran
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 COMPLETIONS_MODEL = "gpt-3.5-turbo"
 
 @click.command()
 @click.option('--url', required=True, help='YouTube video URL.')
-@click.option('--hours', required=True, help='Countdown hours.')
+@click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
 @click.option('--output', required=True, help='Name of the output file.')
 
-def main(url, hours, output):
+def main(url, time, output):
     # Download video
     flag = download_video(url,output)
 
     # test audio
     test_audio(f'{output}.mp3',output,flag)
 
+    # convert time to seconds
+    countdown_seconds = convert_to_seconds(time)
+
     # Start countdown
-    countdown(hours)
+    countdown(countdown_seconds)
 
     # Play audio with fade-in effect on a separate thread
     play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',))
     play_audio_thread.start()
 
     # display the quran verses
     get_verses_and_explanations()
 
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
     # return back to the main thread
     play_audio_thread.join()
 
+def convert_to_seconds(time_str):
+    # Get the number and the time unit (h/m/s)
+    number = int(time_str[:-1])
+    unit = time_str[-1].lower()
+
+    # Convert to seconds
+    if unit == "h":
+        return number * 60 * 60
+    elif unit == "m":
+        return number * 60
+    elif unit == "s":
+        return number
+    else:
+        raise ValueError("Invalid time format. Use [number][h/m/s] format.")
+
 
 def download_video(url,output):
     ydl_opts = {
         'format': 'bestaudio/best',
         'postprocessors': [{
             'key': 'FFmpegExtractAudio',
             'preferredcodec': 'mp3',
@@ -76,16 +94,15 @@
         try:
             audio = AudioSegment.from_file(file_path, format="mp3")
         except:
             print("Error: Audio file could not be loaded.")
     else:
         print(f'{output}.mp3 has already been downloaded and converted.')
 
-def countdown(hours):
-    countdown_seconds = float(hours) * 60 * 60
+def countdown(countdown_seconds):
     # use tqdm to display the countdown progress
     print('\n\n\n\n ---------------- BEGINNING COUNTDOWN ---------------- \n\n\n\n')
     # print the current time in HH:MM format
     print(f'\n\nSTART TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
     for i in tqdm(range(int(countdown_seconds))):
         time.sleep(1)
     print('\n\n\n\n ---------------- COUNTDOWN COMPLETE ----------------')
```

### Comparing `fajrGPT-1.1.6/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.2/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.6
+Version: 1.2
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.1.6/setup.py` & `fajrGPT-1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.1.6",
+    version="1.2",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

