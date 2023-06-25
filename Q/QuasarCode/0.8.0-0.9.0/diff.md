# Comparing `tmp/QuasarCode-0.8.0.tar.gz` & `tmp/QuasarCode-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\chris\source\repos\QuasarCode\QuasarCode_Python\dist\.tmp-s3nwrp1r\QuasarCode-0.8.0.tar", last modified: Sat May 20 17:33:33 2023, max compression
+gzip compressed data, was "C:\Users\chris\source\repos\QuasarCode\QuasarCode_Python\dist\.tmp-g2yqcl96\QuasarCode-0.9.0.tar", last modified: Sun Jun 25 18:37:11 2023, max compression
```

## Comparing `QuasarCode-0.8.0.tar` & `QuasarCode-0.9.0.tar`

### file list

```diff
@@ -1,74 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/
--rw-rw-rw-   0        0        0     1077 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0      826 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/README.md
--rw-rw-rw-   0        0        0      920 2023-05-20 00:29:50.000000 QuasarCode-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/
--rw-rw-rw-   0        0        0     1549 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardGroup.py
--rw-rw-rw-   0        0        0      830 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardQueue.py
--rw-rw-rw-   0        0        0      829 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardStack.py
--rw-rw-rw-   0        0        0     4878 2023-05-20 14:44:24.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_Deck.py
--rw-rw-rw-   0        0        0      619 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_IPlayingCard.py
--rw-rw-rw-   0        0        0     2027 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_PlayingCard.py
--rw-rw-rw-   0        0        0      212 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/
--rw-rw-rw-   0        0        0      259 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_Dice12.py
--rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_Dice6.py
--rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_Dice8.py
--rw-rw-rw-   0        0        0     2636 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_DiceCup.py
--rw-rw-rw-   0        0        0      368 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_IDice.py
--rw-rw-rw-   0        0        0     1412 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_NDice.py
--rw-rw-rw-   0        0        0      139 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/
--rw-rw-rw-   0        0        0      843 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_ISpinner.py
--rw-rw-rw-   0        0        0     1202 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_Spinner.py
--rw-rw-rw-   0        0        0       66 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/__init__.py
--rw-rw-rw-   0        0        0       65 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/IO/
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/
--rw-rw-rw-   0        0        0     4933 2023-05-20 15:51:12.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_ConfigsBase.py
--rw-rw-rw-   0        0        0      144 2023-03-26 16:22:26.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/__init__.py
--rw-rw-rw-   0        0        0     1763 2023-03-28 00:44:54.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_json.py
--rw-rw-rw-   0        0        0      645 2023-03-28 00:44:22.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_properties.py
--rw-rw-rw-   0        0        0     1765 2023-05-20 15:54:55.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_yaml.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Text/
--rw-rw-rw-   0        0        0      388 2023-05-20 16:18:18.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Text/__init__.py
--rw-rw-rw-   0        0        0     3365 2023-05-20 16:23:22.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Text/_console.py
--rw-rw-rw-   0        0        0       50 2023-03-26 01:12:29.000000 QuasarCode-0.8.0/src/QuasarCode/IO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/MPI/
--rw-rw-rw-   0        0        0      980 2023-05-20 14:46:27.000000 QuasarCode-0.8.0/src/QuasarCode/MPI/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/MPI/_mpi_configs.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Science/
--rw-rw-rw-   0        0        0      364 2023-05-20 00:28:18.000000 QuasarCode-0.8.0/src/QuasarCode/Science/__init__.py
--rw-rw-rw-   0        0        0     1516 2023-05-20 00:30:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/_plotting.py
--rw-rw-rw-   0        0        0     4044 2023-05-20 17:21:42.000000 QuasarCode-0.8.0/src/QuasarCode/Science/data.py
--rw-rw-rw-   0        0        0    15789 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/figure.py
--rw-rw-rw-   0        0        0    22484 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/fitline.py
--rw-rw-rw-   0        0        0     4177 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/graph.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/
--rw-rw-rw-   0        0        0     1144 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/StringLiterals.py
--rw-rw-rw-   0        0        0     3144 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/Validators.py
--rw-rw-rw-   0        0        0      210 2023-05-20 16:14:08.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/__init__.py
--rw-rw-rw-   0        0        0      190 2023-03-26 01:55:09.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_async.py
--rw-rw-rw-   0        0        0     1393 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_directorys_and_imports.py
--rw-rw-rw-   0        0        0     1375 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_multiItterator.py
--rw-rw-rw-   0        0        0     3261 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_networking.py
--rw-rw-rw-   0        0        0    12115 2023-05-20 16:13:07.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_script_wrapper.py
--rw-rw-rw-   0        0        0      737 2023-05-20 16:10:55.000000 QuasarCode-0.8.0/src/QuasarCode/__init__.py
--rw-rw-rw-   0        0        0     1884 2023-03-26 16:18:21.000000 QuasarCode-0.8.0/src/QuasarCode/_global_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/edp/
--rw-rw-rw-   0        0        0     2028 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_Event.py
--rw-rw-rw-   0        0        0      254 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_NotEnoughArgumentsError.py
--rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_SubscriberNotPresentError.py
--rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_UndersubscribedEventError.py
--rw-rw-rw-   0        0        0      391 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/edp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/
--rw-rw-rw-   0        0        0      826 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2089 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/
+-rw-rw-rw-   0        0        0     1077 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      826 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/README.md
+-rw-rw-rw-   0        0        0      920 2023-06-25 12:39:28.000000 QuasarCode-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/Games/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/
+-rw-rw-rw-   0        0        0     1549 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_CardGroup.py
+-rw-rw-rw-   0        0        0      830 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_CardQueue.py
+-rw-rw-rw-   0        0        0      829 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_CardStack.py
+-rw-rw-rw-   0        0        0     4878 2023-05-20 14:44:24.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_Deck.py
+-rw-rw-rw-   0        0        0      619 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_IPlayingCard.py
+-rw-rw-rw-   0        0        0     2027 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_PlayingCard.py
+-rw-rw-rw-   0        0        0      212 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Cards/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/
+-rw-rw-rw-   0        0        0      259 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_Dice12.py
+-rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_Dice6.py
+-rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_Dice8.py
+-rw-rw-rw-   0        0        0     2636 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_DiceCup.py
+-rw-rw-rw-   0        0        0      368 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_IDice.py
+-rw-rw-rw-   0        0        0     1412 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_NDice.py
+-rw-rw-rw-   0        0        0      139 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Dice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Spinners/
+-rw-rw-rw-   0        0        0      843 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Spinners/_ISpinner.py
+-rw-rw-rw-   0        0        0     1202 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Spinners/_Spinner.py
+-rw-rw-rw-   0        0        0       66 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/Spinners/__init__.py
+-rw-rw-rw-   0        0        0       65 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/IO/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Checkpointing/
+-rw-rw-rw-   0        0        0     3579 2023-06-25 18:13:52.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Checkpointing/_CheckpointBase.py
+-rw-rw-rw-   0        0        0     1815 2023-06-25 17:58:13.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Checkpointing/_CheckpointController.py
+-rw-rw-rw-   0        0        0     1708 2023-06-25 17:51:08.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Checkpointing/_CheckpointState.py
+-rw-rw-rw-   0        0        0      635 2023-06-25 17:53:29.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Checkpointing/_PickleCheckpoint.py
+-rw-rw-rw-   0        0        0      200 2023-06-25 13:33:20.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Checkpointing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/
+-rw-rw-rw-   0        0        0     4933 2023-05-20 15:51:12.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_ConfigsBase.py
+-rw-rw-rw-   0        0        0      144 2023-03-26 16:22:26.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/__init__.py
+-rw-rw-rw-   0        0        0     1763 2023-03-28 00:44:54.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_json.py
+-rw-rw-rw-   0        0        0      645 2023-03-28 00:44:22.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_properties.py
+-rw-rw-rw-   0        0        0     1765 2023-05-20 15:54:55.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_yaml.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Text/
+-rw-rw-rw-   0        0        0      388 2023-05-20 16:18:18.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Text/__init__.py
+-rw-rw-rw-   0        0        0     3365 2023-05-20 16:23:22.000000 QuasarCode-0.9.0/src/QuasarCode/IO/Text/_console.py
+-rw-rw-rw-   0        0        0       79 2023-06-25 12:42:29.000000 QuasarCode-0.9.0/src/QuasarCode/IO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/MPI/
+-rw-rw-rw-   0        0        0      980 2023-05-20 14:46:27.000000 QuasarCode-0.9.0/src/QuasarCode/MPI/__init__.py
+-rw-rw-rw-   0        0        0     1476 2023-06-25 12:38:22.000000 QuasarCode-0.9.0/src/QuasarCode/MPI/_mpi_configs.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/Science/
+-rw-rw-rw-   0        0        0      364 2023-05-20 00:28:18.000000 QuasarCode-0.9.0/src/QuasarCode/Science/__init__.py
+-rw-rw-rw-   0        0        0     1516 2023-05-20 00:30:36.000000 QuasarCode-0.9.0/src/QuasarCode/Science/_plotting.py
+-rw-rw-rw-   0        0        0     4044 2023-05-20 17:21:42.000000 QuasarCode-0.9.0/src/QuasarCode/Science/data.py
+-rw-rw-rw-   0        0        0    15789 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Science/figure.py
+-rw-rw-rw-   0        0        0    22484 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Science/fitline.py
+-rw-rw-rw-   0        0        0     4177 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Science/graph.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/
+-rw-rw-rw-   0        0        0     1144 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/StringLiterals.py
+-rw-rw-rw-   0        0        0     3144 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/Validators.py
+-rw-rw-rw-   0        0        0      210 2023-05-20 16:14:08.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-03-26 01:55:09.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/_async.py
+-rw-rw-rw-   0        0        0     1393 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/_directorys_and_imports.py
+-rw-rw-rw-   0        0        0     1375 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/_multiItterator.py
+-rw-rw-rw-   0        0        0     3261 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/_networking.py
+-rw-rw-rw-   0        0        0    12115 2023-05-20 16:13:07.000000 QuasarCode-0.9.0/src/QuasarCode/Tools/_script_wrapper.py
+-rw-rw-rw-   0        0        0      737 2023-06-25 12:39:26.000000 QuasarCode-0.9.0/src/QuasarCode/__init__.py
+-rw-rw-rw-   0        0        0     1884 2023-03-26 16:18:21.000000 QuasarCode-0.9.0/src/QuasarCode/_global_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode/edp/
+-rw-rw-rw-   0        0        0     2028 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/edp/_Event.py
+-rw-rw-rw-   0        0        0      254 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/edp/_NotEnoughArgumentsError.py
+-rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/edp/_SubscriberNotPresentError.py
+-rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.9.0/src/QuasarCode/edp/_UndersubscribedEventError.py
+-rw-rw-rw-   0        0        0      391 2023-03-25 22:02:36.000000 QuasarCode-0.9.0/src/QuasarCode/edp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode.egg-info/
+-rw-rw-rw-   0        0        0      826 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2346 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 18:37:11.000000 QuasarCode-0.9.0/src/QuasarCode.egg-info/top_level.txt
```

### Comparing `QuasarCode-0.8.0/LICENSE.txt` & `QuasarCode-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/PKG-INFO` & `QuasarCode-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuasarCode
-Version: 0.8.0
+Version: 0.9.0
 Summary: A general purpose library for Python applications.
 Author-email: Christopher Rowe <thequasarx1@gmail.com>
 Project-URL: Homepage, https://github.com/QuasarX1/QuasarCode
 Project-URL: Bug Tracker, https://github.com/QuasarX1/QuasarCode/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `QuasarCode-0.8.0/pyproject.toml` & `QuasarCode-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["*"]
 
 [project]
 name = "QuasarCode"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="Christopher Rowe", email="thequasarx1@gmail.com" },
 ]
 description = "A general purpose library for Python applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardGroup.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_CardGroup.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardQueue.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_CardQueue.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardStack.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_CardStack.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_Deck.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_Deck.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_IPlayingCard.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_IPlayingCard.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_PlayingCard.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Cards/_PlayingCard.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_DiceCup.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_DiceCup.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_NDice.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Dice/_NDice.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_ISpinner.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Spinners/_ISpinner.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_Spinner.py` & `QuasarCode-0.9.0/src/QuasarCode/Games/Spinners/_Spinner.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_ConfigsBase.py` & `QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_ConfigsBase.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_json.py` & `QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_json.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_properties.py` & `QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_properties.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_yaml.py` & `QuasarCode-0.9.0/src/QuasarCode/IO/Configurations/_yaml.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/IO/Text/_console.py` & `QuasarCode-0.9.0/src/QuasarCode/IO/Text/_console.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/MPI/__init__.py` & `QuasarCode-0.9.0/src/QuasarCode/MPI/__init__.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/MPI/_mpi_configs.py` & `QuasarCode-0.9.0/src/QuasarCode/MPI/_mpi_configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from QuasarCode.MPI import _raise_mpi_error
 
 if not __settings_object.mpi_avalible:
     _raise_mpi_error()
 
 from mpi4py import MPI
 
-class __MPI_Config(object):
+class _MPI_Config(object):
     __singleton = None
     __update = True
 
     @staticmethod
     def _is_singleton_avalible():
-        return __MPI_Config.__singleton is not None
+        return _MPI_Config.__singleton is not None
 
     @staticmethod
     def _get_singleton():
-        return __MPI_Config.__singleton
+        return _MPI_Config.__singleton
 
     def __init__(self, comm):
-        if __MPI_Config.__update:
-            __MPI_Config.__update = False
-            __MPI_Config.__singleton = self
+        if _MPI_Config.__update:
+            _MPI_Config.__update = False
+            _MPI_Config.__singleton = self
             self.__MPI_COMM = comm
             self.__MPI_COMM_SIZE = int(self.__MPI_COMM.Get_size())
             self.__MPI_RANK = self.__MPI_COMM.Get_rank()
 
         else:
             raise RuntimeError("Only one instance of the MPI_Config object may exist. Change configuration using the update method.")
 
@@ -38,18 +38,18 @@
         return self.__MPI_COMM_SIZE
 
     @property
     def rank(self):
         return self.__MPI_RANK
 
     def update(self, comm):
-        __MPI_Config.__update(comm)
+        _MPI_Config.__update(comm)
 
     @staticmethod
     def __update(comm):
-        __MPI_Config.__update = True
-        __MPI_Config(comm)
+        _MPI_Config.__update = True
+        _MPI_Config(comm)
 
-if not __MPI_Config._is_singleton_avalible():
-    __MPI_Config(MPI.COMM_WORLD)
+if not _MPI_Config._is_singleton_avalible():
+    _MPI_Config(MPI.COMM_WORLD)
 
-mpi_config = __MPI_Config._get_singleton()
+mpi_config = _MPI_Config._get_singleton()
```

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Science/_plotting.py` & `QuasarCode-0.9.0/src/QuasarCode/Science/_plotting.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Science/data.py` & `QuasarCode-0.9.0/src/QuasarCode/Science/data.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Science/figure.py` & `QuasarCode-0.9.0/src/QuasarCode/Science/figure.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Science/fitline.py` & `QuasarCode-0.9.0/src/QuasarCode/Science/fitline.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Science/graph.py` & `QuasarCode-0.9.0/src/QuasarCode/Science/graph.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Tools/StringLiterals.py` & `QuasarCode-0.9.0/src/QuasarCode/Tools/StringLiterals.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Tools/Validators.py` & `QuasarCode-0.9.0/src/QuasarCode/Tools/Validators.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Tools/_directorys_and_imports.py` & `QuasarCode-0.9.0/src/QuasarCode/Tools/_directorys_and_imports.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Tools/_multiItterator.py` & `QuasarCode-0.9.0/src/QuasarCode/Tools/_multiItterator.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Tools/_networking.py` & `QuasarCode-0.9.0/src/QuasarCode/Tools/_networking.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/Tools/_script_wrapper.py` & `QuasarCode-0.9.0/src/QuasarCode/Tools/_script_wrapper.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/__init__.py` & `QuasarCode-0.9.0/src/QuasarCode/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Adds functionality to Python along with wrapers for existing modules for ease of use
 
 Credits:
     Written by Christopher Rowe
     Notable contribusions taken from code written by Tim Greenshaw 10/2018
 
-Version: 0.8.0
+Version: 0.9.0
 """
 
 from ._global_settings import settings_object as Settings
 
 from . import edp
 
 from . import Games
```

### Comparing `QuasarCode-0.8.0/src/QuasarCode/_global_settings.py` & `QuasarCode-0.9.0/src/QuasarCode/_global_settings.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode/edp/_Event.py` & `QuasarCode-0.9.0/src/QuasarCode/edp/_Event.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.8.0/src/QuasarCode.egg-info/PKG-INFO` & `QuasarCode-0.9.0/src/QuasarCode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuasarCode
-Version: 0.8.0
+Version: 0.9.0
 Summary: A general purpose library for Python applications.
 Author-email: Christopher Rowe <thequasarx1@gmail.com>
 Project-URL: Homepage, https://github.com/QuasarX1/QuasarCode
 Project-URL: Bug Tracker, https://github.com/QuasarX1/QuasarCode/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `QuasarCode-0.8.0/src/QuasarCode.egg-info/SOURCES.txt` & `QuasarCode-0.9.0/src/QuasarCode.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 src/QuasarCode/Games/Dice/_IDice.py
 src/QuasarCode/Games/Dice/_NDice.py
 src/QuasarCode/Games/Dice/__init__.py
 src/QuasarCode/Games/Spinners/_ISpinner.py
 src/QuasarCode/Games/Spinners/_Spinner.py
 src/QuasarCode/Games/Spinners/__init__.py
 src/QuasarCode/IO/__init__.py
+src/QuasarCode/IO/Checkpointing/_CheckpointBase.py
+src/QuasarCode/IO/Checkpointing/_CheckpointController.py
+src/QuasarCode/IO/Checkpointing/_CheckpointState.py
+src/QuasarCode/IO/Checkpointing/_PickleCheckpoint.py
+src/QuasarCode/IO/Checkpointing/__init__.py
 src/QuasarCode/IO/Configurations/_ConfigsBase.py
 src/QuasarCode/IO/Configurations/__init__.py
 src/QuasarCode/IO/Configurations/_json.py
 src/QuasarCode/IO/Configurations/_properties.py
 src/QuasarCode/IO/Configurations/_yaml.py
 src/QuasarCode/IO/Text/__init__.py
 src/QuasarCode/IO/Text/_console.py
```

