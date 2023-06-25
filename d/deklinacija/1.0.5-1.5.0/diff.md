# Comparing `tmp/deklinacija-1.0.5.tar.gz` & `tmp/deklinacija-1.5.0.tar.gz`

## Comparing `deklinacija-1.0.5.tar` & `deklinacija-1.5.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/__init__.py
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/module.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/utils.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.0.5/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.5/LICENSE
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 deklinacija-1.0.5/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 deklinacija-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.5.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/__init__.py
+-rw-r--r--   0        0        0    21534 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/module.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/utils.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 deklinacija-1.5.0/tests/names_female.txt
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 deklinacija-1.5.0/tests/names_male.txt
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 deklinacija-1.5.0/tests/test_names.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.5.0/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.5.0/PKG-INFO
```

### Comparing `deklinacija-1.0.5/.github/workflows/python-package.yml` & `deklinacija-1.5.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.5/deklinacija/utils.py` & `deklinacija-1.5.0/deklinacija/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,30 +7,33 @@
     'p': 'п', 'r': 'р', 's': 'с', 'š': 'ш', 't': 'т', 'u': 'у', 'v': 'в', 'z': 'з', 'ž': 'ж', 'dž': 'џ', 'dz': 'џ'}
 
 alphabet_latin = {
     'а': 'a', 'б': 'b', 'ц': 'c', 'ч': 'č', 'ћ': 'ć', 'д': 'd', 'ђ': 'đ', 'е': 'e', 'ф': 'f', 'г': 'g',
     'х': 'h', 'и': 'i', 'ј': 'j', 'к': 'k', 'л': 'l', 'љ': 'lj', 'м': 'm', 'н': 'n', 'њ': 'nj', 'о': 'o',
     'п': 'p', 'р': 'r', 'с': 's', 'ш': 'š', 'т': 't', 'у': 'u', 'в': 'v', 'з': 'z', 'ж': 'ž', 'џ': 'dž'}
 
+ZVUCNI = ["б", "д", "г", "ђ", "ж", "з", "џ"]
+
 latExceptions = []
 
+
 def isLatin(word):
     if word[-1].lower() in alphabet:
         return True
     elif word[-1].lower() in alphabet_latin:
         return False
     else:
         raise ValueError("word contains illegal characters")
 
+
 def toCyrillic(word):
 
     wordArray = []
     word = list(word)
     wordText = "".join(word)
-    
 
     if wordText.lower() not in latExceptions:
         n = 0
         while n <= (len(word)-1):
 
             if n == len(word)-1:
                 wordArray.append(word[n])
@@ -71,52 +74,56 @@
             wordArray[n] = i
             n += 1
 
     word = "".join(wordArray)
 
     return word
 
+
 def toLatin(word):
     word = list(word)
 
     n = 0
     for i in word:
         if i.lower() in alphabet_latin:
-            if i[0].isupper() and i.lower() in ['љ','њ','џ']:
-                letter = alphabet_latin[i.lower()][0].upper() + alphabet_latin[i.lower()][1]
+            if i[0].isupper() and i.lower() in ['љ', 'њ', 'џ']:
+                letter = alphabet_latin[i.lower()][0].upper(
+                ) + alphabet_latin[i.lower()][1]
                 word[n] = letter
             elif i[0].isupper():
                 word[n] = alphabet_latin[i.lower()].upper()
             else:
                 word[n] = alphabet_latin[i]
 
         else:
             word[n] = i
         n += 1
-    
+
     return "".join(word)
 
-def check(name,gender):
+
+def check(name, gender):
     if type(name) != str or type(name) != str or type(gender) != str:
-        raise TypeError("name and gender params must be a string, param latin must be a boolean")
-    
+        raise TypeError(
+            "name and gender params must be a string, param latin must be a boolean")
+
     gender = gender.strip()
     name = name.strip()
 
-    if gender.lower() not in ["male","female"]:
+    if gender.lower() not in ["male", "female"]:
         raise ValueError('gender param must be either "male" or "female"')
 
     if len(name) < 3:
         raise ValueError("name param must be at least 3 characters long")
-    
+
+
 def separateLetters(word):
     word = list(word)
     wordText = "".join(word)
     wordArray = []
-    
 
     n = 0
     while n <= (len(word)-1):
 
         if n == len(word)-1:
             wordArray.append(word[n])
             break
@@ -128,41 +135,51 @@
         elif word[n] in ["d", "D"] and word[n+1] in ["ž", "Ž", "z", "Z"]:
             wordArray.append(word[n]+word[n+1])
             word.pop(n+1)
             n += 1
         else:
             wordArray.append(word[n])
             n += 1
-    
+
     return wordArray
 
+
+def isZvucni(letter):
+    if toCyrillic(letter.lower()) in ZVUCNI:
+        return True
+    else:
+        return False
+
 # For converting the csv to cyrillic
 # with open('deklinacija/vokativ_database.csv',"r+",encoding="utf-8") as f:
-    
+
 #     reader = dict(csv.reader(f, delimiter=","))
 #     converted = {}
 #     text = ""
 
 #     for (k,v) in reader.items():
 #         kConverted = toCyrillic(k)
 #         vConverted = toCyrillic(v)
 #         text = text + kConverted + "," + vConverted + "\n"
-    
+
 #     f.truncate(0)
 #     f.write(text)
+
+
 def formatName(word):
     word = list(word)
     word[0] = word[0].upper()
     n = 1
     while n < len(word):
         word[n] = word[n].lower()
         n += 1
     return "".join(word)
-        
+
+
 module_path = os.path.abspath(__file__)
 
 module_directory = os.path.dirname(module_path)
 
 csv_file_path = os.path.join(module_directory, 'vokativ_database.csv')
 
-with open(csv_file_path,"r",encoding="utf-8") as file:
+with open(csv_file_path, "r", encoding="utf-8") as file:
     vokativ_db = dict(csv.reader(file, delimiter=","))
```

### Comparing `deklinacija-1.0.5/deklinacija/vokativ_database.csv` & `deklinacija-1.5.0/deklinacija/vokativ_database.csv`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 Љуба,Љубо
 Лола,Лоло
 Лоза,Лозо
 Луча,Луча
 Лука,Лука
 Луна,Луна
 Маја,Мајо
+Мама,Мама
 Мања,Мања
 Мара,Маро
 Маша,Машо
 Миа,Миа
 Мика,Мико
 Мића,Мићо
 Мија,Мијо
@@ -118,14 +119,15 @@
 Сока,Соко
 Соња,Соња
 Срба,Србо
 Срђа,Срђо
 Тада,Тадо
 Тања,Тања
 Тара,Таро
+Тата,Тата
 Теа,Теа
 Тина,Тина
 Тода,Тодо
 Тома,Томо
 Тоша,Тошо
 Уна,Уна
 Вања,Вања
@@ -138,8 +140,9 @@
 Зага,Заго
 Жика,Жико
 Жива,Живо
 Зоја,Зоја
 Зора,Зоро
 Хана,Хана
 Дина,Дина
-Веља,Вељо
+Веља,Вељо
+Мима,Мима
```

### Comparing `deklinacija-1.0.5/.gitignore` & `deklinacija-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.5/LICENSE` & `deklinacija-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.5/README.md` & `deklinacija-1.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 # deklinacija
-A Python library for declension of personal names in Serbian, with support for both Cyrillic and Latin scripts.
+A Python library for declension of personal names in Serbian, with support for both Cyrillic and Latin scripts, and last names.
 
 ## Installation
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
 The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
 ```
-**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below).
+To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below). You can also input a full name (with a first name and a last name, multiple last names are supported too, separated with a whitespace character) and the script will change the name accordingly. 
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
 genitiv = dek.genitiv("Velja","male") #Velje
-dativ = dek.dativ("Петар","male") #Петру
-akuzativ = dek.akuzativ("Jana","female") #Janu
+genitiv2 = dek.genitiv("Velja Petrović","male") #Velje Petrovića
+dativ = dek.dativ("Jana","female") #Jani
+dativ2 = dek.dativ("Jana Paunovska","female") #Jani Paunovskoj
+akuzativ = dek.akuzativ("Петар","male") #Петра
+akuzativ2 = dek.akuzativ("Петар Петровић","male") #Петра Петровића
 vokativ = dek.vokativ("Predrag","male") #Predraže
-vokativ2 = dek.vokativ("PREDRAG","male") #PREDRAŽE
+vokativ2 = dek.vokativ("PREDRAG JANKOVIĆ","male") #PREDRAŽE JANKOVIĆU
 instrumental = dek.instrumental("Uroš","male") #Urošem
-instrumental2 = dek.instrumental("Вук","male") #Вуком
+instrumental2 = dek.instrumental("Uroš Konstantinović","male") #Urošem Konstantinovićem
 lokativ = dek.lokativ("Lana","female") #Lani
+lokativ = dek.lokativ("Lana Petrović","female") #Lani Petrović
 
-print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
-#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje.
-#Translation: Hello Predrag! You have received a friend request from Velja.
+print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv2}.") 
+#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje Petrovića.
+#Translation: Hello Predrag! You have received a friend request from Velja Petrović.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
 The `declineAll()` function returns a `dictionary`, where keys are the grammatical cases.
 
 ```python
 import deklinacija as dek
 
-Nikola = dek.declineAll("Nikola","male") 
+name = dek.declineAll("Nikola","male") 
 #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
 #'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
 
-print("Dali ste poklon",Nikola['dativ']) 
+print("Dali ste poklon",name['dativ']) 
 #Dali ste poklon Nikoli
 #Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
-- Declension of last names
 - Possessive forms
 
 
 ## Attribution
 [Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
```

### Comparing `deklinacija-1.0.5/pyproject.toml` & `deklinacija-1.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.0.5"
+version = "1.5.0"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.0.5/PKG-INFO` & `deklinacija-1.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.0.5
+Version: 1.5.0
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # deklinacija
-A Python library for declension of personal names in Serbian, with support for both Cyrillic and Latin scripts.
+A Python library for declension of personal names in Serbian, with support for both Cyrillic and Latin scripts, and last names.
 
 ## Installation
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
 The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
 ```
-**As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below).
+To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below). You can also input a full name (with a first name and a last name, multiple last names are supported too, separated with a whitespace character) and the script will change the name accordingly. 
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
 genitiv = dek.genitiv("Velja","male") #Velje
-dativ = dek.dativ("Петар","male") #Петру
-akuzativ = dek.akuzativ("Jana","female") #Janu
+genitiv2 = dek.genitiv("Velja Petrović","male") #Velje Petrovića
+dativ = dek.dativ("Jana","female") #Jani
+dativ2 = dek.dativ("Jana Paunovska","female") #Jani Paunovskoj
+akuzativ = dek.akuzativ("Петар","male") #Петра
+akuzativ2 = dek.akuzativ("Петар Петровић","male") #Петра Петровића
 vokativ = dek.vokativ("Predrag","male") #Predraže
-vokativ2 = dek.vokativ("PREDRAG","male") #PREDRAŽE
+vokativ2 = dek.vokativ("PREDRAG JANKOVIĆ","male") #PREDRAŽE JANKOVIĆU
 instrumental = dek.instrumental("Uroš","male") #Urošem
-instrumental2 = dek.instrumental("Вук","male") #Вуком
+instrumental2 = dek.instrumental("Uroš Konstantinović","male") #Urošem Konstantinovićem
 lokativ = dek.lokativ("Lana","female") #Lani
+lokativ = dek.lokativ("Lana Petrović","female") #Lani Petrović
 
-print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
-#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje.
-#Translation: Hello Predrag! You have received a friend request from Velja.
+print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv2}.") 
+#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje Petrovića.
+#Translation: Hello Predrag! You have received a friend request from Velja Petrović.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
 The `declineAll()` function returns a `dictionary`, where keys are the grammatical cases.
 
 ```python
 import deklinacija as dek
 
-Nikola = dek.declineAll("Nikola","male") 
+name = dek.declineAll("Nikola","male") 
 #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
 #'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
 
-print("Dali ste poklon",Nikola['dativ']) 
+print("Dali ste poklon",name['dativ']) 
 #Dali ste poklon Nikoli
 #Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
-- Declension of last names
 - Possessive forms
 
 
 ## Attribution
 [Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
```

