# Comparing `tmp/chomp64-2.1.2.tar.gz` & `tmp/chomp64-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chomp64-2.1.2.tar", last modified: Sun Jun 25 10:57:52 2023, max compression
+gzip compressed data, was "chomp64-2.2.2.tar", last modified: Sun Jun 25 11:22:46 2023, max compression
```

## Comparing `chomp64-2.1.2.tar` & `chomp64-2.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 10:57:52.441630 chomp64-2.1.2/
--rw-rw-rw-   0        0        0     1094 2023-06-25 08:49:13.000000 chomp64-2.1.2/LICENSE
--rw-rw-rw-   0        0        0      429 2023-06-25 10:57:52.440625 chomp64-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-06-25 08:49:13.000000 chomp64-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 10:57:52.425156 chomp64-2.1.2/chomp64/
--rw-rw-rw-   0        0        0        0 2023-06-25 09:38:56.000000 chomp64-2.1.2/chomp64/__init__.py
--rw-rw-rw-   0        0        0     9717 2023-06-25 10:55:42.000000 chomp64-2.1.2/chomp64/v2BasicChomper.py
-drwxrwxrwx   0        0        0        0 2023-06-25 10:57:52.438382 chomp64-2.1.2/chomp64.egg-info/
--rw-rw-rw-   0        0        0      429 2023-06-25 10:57:52.000000 chomp64-2.1.2/chomp64.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-06-25 10:57:52.000000 chomp64-2.1.2/chomp64.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 10:57:52.000000 chomp64-2.1.2/chomp64.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 10:57:52.000000 chomp64-2.1.2/chomp64.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 10:57:52.441630 chomp64-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-06-25 10:38:46.000000 chomp64-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:22:46.590826 chomp64-2.2.2/
+-rw-rw-rw-   0        0        0     1094 2023-06-25 08:49:13.000000 chomp64-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0      429 2023-06-25 11:22:46.588815 chomp64-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-06-25 08:49:13.000000 chomp64-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 11:22:46.568451 chomp64-2.2.2/chomp64/
+-rw-rw-rw-   0        0        0        0 2023-06-25 09:38:56.000000 chomp64-2.2.2/chomp64/__init__.py
+-rw-rw-rw-   0        0        0     9657 2023-06-25 11:20:20.000000 chomp64-2.2.2/chomp64/v2BasicChomper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:22:46.587809 chomp64-2.2.2/chomp64.egg-info/
+-rw-rw-rw-   0        0        0      429 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 11:22:46.593829 chomp64-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-06-25 11:20:34.000000 chomp64-2.2.2/setup.py
```

### Comparing `chomp64-2.1.2/LICENSE` & `chomp64-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chomp64-2.1.2/chomp64/v2BasicChomper.py` & `chomp64-2.2.2/chomp64/v2BasicChomper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import argparse,os,struct
 class tokenizer():
-    def __init__(self, infile:str, outfile:str, flags:dict=None):
-        if (flags is None):
-            self.flags = {'v':False,'o':False}
-        else:
-            self.flags = flags
+    def __init__(self, infile:str, outfile:str, overwrite=False, verbose=False):
+        self.overwrite = overwrite
+        self.verbose = verbose
         self.memory_entry_point, self.memory_exit_point = 0x0801, 0x0000
-
         try:
-            if (self.flags['v']):
+            if (self.verbose):
                 print("CHOMP64: Validating input filepath...")
             assert(self.__validate_in_file(infile)), "\nCHOMP64: Something went wrong. Please check your input filepath.\n"
         except Exception as e:
             print(e)
             exit()         
         
         try:
-            if (self.flags['v']):
+            if (self.verbose):
                 print("CHOMP64: Validating output filepath...")
             assert(self.__validate_out_file(outfile)), "\nCHOMP64: Something went wrong. Please check your output filepath.\n"
         except Exception as e:
             print(e)
             exit()
         
         self.infile, self.outfile = os.path.join(os.getcwd(),infile), os.path.join(os.getcwd(), outfile)
@@ -57,15 +54,15 @@
             return True
         
         return False
 
     def __validate_out_file(self,file):
         res = ""
         path = os.path.join(os.getcwd(), file)
-        if (os.path.exists(path) and not self.flags['o']):
+        if (os.path.exists(path) and not self.overwrite):
             while (res.upper() != 'Y' and res.upper() != "N"):
                 res = input("\nCHOMP64: The output file currently exists. Would you like to overwrite it? (Y/N)  ")
                 print()
             
             if (res.upper() == 'N'):
                 print("CHOMP64: Please enter a new output file.\n")
                 exit()
@@ -79,51 +76,51 @@
 
     def tokenize(self):
         for i in range(len(self.original_content)):
             line = self.original_content[i]
             if (not line.strip()):
                 continue
             
-            if (self.flags['v']):
+            if (self.verbose):
                 print("CHOMP64: Crunching line:\t" + line.strip())
             
             line_num,line_content = self.__strip_line_number(line, i)
             line_content = self.__tokenize_line(line_content)
             
-            if (self.flags['v']):
+            if (self.verbose):
                 print("CHOMP64: Tokens found:\t", self.line_tokens)
 
             self.line_tokens = []
             self.tokenized_content.append((line_num,line_content))
 
-        if (self.flags['v']):
+        if (self.verbose):
             print("CHOMP64: Tokenization successful, writing to output file...")
 
         self.__write_to_ouput_file()
 
-        if (self.flags['v']):
+        if (self.verbose):
             print("CHOMP64: Write successful")
 
 
     def __tokenize_line(self, line):
         line = line.upper()
         line_no_quoted_material = self.__remove_quoted_material(line)
         tokenized_line = []
 
         if ("REM" in line_no_quoted_material):
-            if (self.flags['v']):
+            if (self.verbose):
                 print("CHOMP64: Remarked line, continuing...")
             comment_line = self.__convert_to_list(line_no_quoted_material.replace("REM",""))
             tokenized_line.extend([0x8F])
             tokenized_line.extend(comment_line)
             self.line_tokens.append("REM")
             return tokenized_line
         
         if (':' in line_no_quoted_material):
-            if (self.flags['v']):
+            if (self.verbose):
                 print("CHOMP64: Multiple commands in line, splitting...")
             
             split = line.index(':')
             left, right = line[0:split], line[split+1:]
             split_left, split_right = self.__tokenize_line(left), self.__tokenize_line(right)
 
             tokenized_line.extend(split_left)
@@ -226,10 +223,10 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("inpath", help="Path to desired input file (*.bas)")
     parser.add_argument("outpath", help="Path to desired output file (*.prg)")
     parser.add_argument("-o","--overwrite", help="Overwrite output file, if it exists", action='store_true')
     parser.add_argument("-v","--verbose", help="Display tokenizer steps", action='store_true')
     args=parser.parse_args()
 
-    t = tokenizer(args.inpath, args.outpath, {"o":args.overwrite, 'v':args.verbose})
+    t = tokenizer(args.inpath, args.outpath, overwrite=args.overwrite, verbose=args.verbose)
     t.tokenize()
```

### Comparing `chomp64-2.1.2/setup.py` & `chomp64-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 setup(
     name='chomp64',
-    version='2.1.2',
+    version='2.2.2',
     description='v2 BASIC Tokenizer',
     url='https://github.com/gvbarker/CHOMP',
     author='Giancarlo Barker',
     author_email='jonzomb80@gmail.com',
     license='MIT',
     packages=['chomp64'],
     classifiers=[
```

