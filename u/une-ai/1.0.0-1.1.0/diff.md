# Comparing `tmp/une_ai-1.0.0.tar.gz` & `tmp/une_ai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "une_ai-1.0.0.tar", last modified: Mon Jun 12 01:38:43 2023, max compression
+gzip compressed data, was "une_ai-1.1.0.tar", last modified: Sun Jun 25 03:41:45 2023, max compression
```

## Comparing `une_ai-1.0.0.tar` & `une_ai-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.193028 une_ai-1.0.0/
--rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.0.0/LICENSE
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-12 01:38:43.192891 une_ai-1.0.0/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.0.0/README.md
--rw-r--r--   0 jonathan   (501) staff       (20)      468 2023-06-12 00:06:41.000000 une_ai-1.0.0/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-06-12 01:38:43.193073 une_ai-1.0.0/setup.cfg
--rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.0.0/setup.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.186353 une_ai-1.0.0/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.187179 une_ai-1.0.0/src/une_ai/
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.0.0/src/une_ai/__init__.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.188600 une_ai-1.0.0/src/une_ai/assignments/
--rw-r--r--   0 jonathan   (501) staff       (20)       81 2023-06-04 07:40:09.000000 une_ai-1.0.0/src/une_ai/assignments/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.0.0/src/une_ai/assignments/snake_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5982 2023-06-04 07:33:36.000000 une_ai-1.0.0/src/une_ai/assignments/snake_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.190461 une_ai-1.0.0/src/une_ai/models/
--rw-r--r--   0 jonathan   (501) staff       (20)      171 2023-05-26 01:31:10.000000 une_ai-1.0.0/src/une_ai/models/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.0.0/src/une_ai/models/agent.py
--rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.0.0/src/une_ai/models/environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)      971 2023-05-26 05:00:00.000000 une_ai-1.0.0/src/une_ai/models/game_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1311 2023-05-26 02:12:21.000000 une_ai-1.0.0/src/une_ai/models/graph_node.py
--rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.0.0/src/une_ai/models/grid_map.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.191735 une_ai-1.0.0/src/une_ai/tictactoe/
--rw-r--r--   0 jonathan   (501) staff       (20)      152 2023-05-26 03:49:00.000000 une_ai-1.0.0/src/une_ai/tictactoe/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)      990 2023-06-04 04:00:01.000000 une_ai-1.0.0/src/une_ai/tictactoe/tictactoc_player.py
--rw-r--r--   0 jonathan   (501) staff       (20)     4902 2023-06-04 04:00:39.000000 une_ai-1.0.0/src/une_ai/tictactoe/tictactoe_game.py
--rw-r--r--   0 jonathan   (501) staff       (20)     4536 2023-06-04 04:01:36.000000 une_ai-1.0.0/src/une_ai/tictactoe/tictactoe_game_environment.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.192527 une_ai-1.0.0/src/une_ai/vacuum/
--rw-r--r--   0 jonathan   (501) staff       (20)      127 2023-06-06 11:05:08.000000 une_ai-1.0.0/src/une_ai/vacuum/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.0.0/src/une_ai/vacuum/vacuum_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5411 2023-06-06 03:24:31.000000 une_ai-1.0.0/src/une_ai/vacuum/vacuum_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.187963 une_ai-1.0.0/src/une_ai.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-12 01:38:42.000000 une_ai-1.0.0/src/une_ai.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      806 2023-06-12 01:38:43.000000 une_ai-1.0.0/src/une_ai.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-06-12 01:38:42.000000 une_ai-1.0.0/src/une_ai.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       13 2023-06-12 01:38:43.000000 une_ai-1.0.0/src/une_ai.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-06-12 01:38:43.000000 une_ai-1.0.0/src/une_ai.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.356260 une_ai-1.1.0/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.1.0/LICENSE
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-25 03:41:45.356094 une_ai-1.1.0/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.1.0/README.md
+-rw-r--r--   0 jonathan   (501) staff       (20)      481 2023-06-25 03:39:31.000000 une_ai-1.1.0/pyproject.toml
+-rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-06-25 03:41:45.356299 une_ai-1.1.0/setup.cfg
+-rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.1.0/setup.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.347635 une_ai-1.1.0/src/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.348794 une_ai-1.1.0/src/une_ai/
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.1.0/src/une_ai/__init__.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.351290 une_ai-1.1.0/src/une_ai/assignments/
+-rw-r--r--   0 jonathan   (501) staff       (20)      198 2023-06-17 05:23:26.000000 une_ai-1.1.0/src/une_ai/assignments/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)    12875 2023-06-25 01:46:33.000000 une_ai-1.1.0/src/une_ai/assignments/connect_four_base_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     9682 2023-06-25 02:57:40.000000 une_ai-1.1.0/src/une_ai/assignments/connect_four_game.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.1.0/src/une_ai/assignments/snake_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5982 2023-06-04 07:33:36.000000 une_ai-1.1.0/src/une_ai/assignments/snake_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.353944 une_ai-1.1.0/src/une_ai/models/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1323 2023-06-25 00:13:50.000000 une_ai-1.1.0/src/une_ai/models/MCTS_graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      254 2023-06-24 12:38:18.000000 une_ai-1.1.0/src/une_ai/models/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.1.0/src/une_ai/models/agent.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.1.0/src/une_ai/models/environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1083 2023-06-22 07:56:49.000000 une_ai-1.1.0/src/une_ai/models/game_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1312 2023-06-12 07:15:34.000000 une_ai-1.1.0/src/une_ai/models/graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.1.0/src/une_ai/models/grid_map.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5827 2023-06-24 06:33:53.000000 une_ai-1.1.0/src/une_ai/models/transposition_table.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.354700 une_ai-1.1.0/src/une_ai/tictactoe/
+-rw-r--r--   0 jonathan   (501) staff       (20)       87 2023-06-25 01:53:59.000000 une_ai-1.1.0/src/une_ai/tictactoe/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1332 2023-06-25 02:53:44.000000 une_ai-1.1.0/src/une_ai/tictactoe/tictactoc_player.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5001 2023-06-25 02:58:21.000000 une_ai-1.1.0/src/une_ai/tictactoe/tictactoe_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.355699 une_ai-1.1.0/src/une_ai/vacuum/
+-rw-r--r--   0 jonathan   (501) staff       (20)      186 2023-06-12 02:00:34.000000 une_ai-1.1.0/src/une_ai/vacuum/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      910 2023-06-12 07:14:58.000000 une_ai-1.1.0/src/une_ai/vacuum/vacuum_dock_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.1.0/src/une_ai/vacuum/vacuum_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5938 2023-06-12 02:18:54.000000 une_ai-1.1.0/src/une_ai/vacuum/vacuum_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.349763 une_ai-1.1.0/src/une_ai.egg-info/
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)      978 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)       19 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/requires.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/top_level.txt
```

### Comparing `une_ai-1.0.0/LICENSE` & `une_ai-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `une_ai-1.0.0/PKG-INFO` & `une_ai-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une_ai
-Version: 1.0.0
+Version: 1.1.0
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.0.0/README.md` & `une_ai-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `une_ai-1.0.0/src/une_ai/assignments/snake_environment.py` & `une_ai-1.1.0/src/une_ai/assignments/snake_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.0.0/src/une_ai/assignments/snake_game.py` & `une_ai-1.1.0/src/une_ai/assignments/snake_game.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.0.0/src/une_ai/models/agent.py` & `une_ai-1.1.0/src/une_ai/models/agent.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.0.0/src/une_ai/models/game_environment.py` & `une_ai-1.1.0/src/une_ai/models/game_environment.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,38 @@
 class GameEnvironment(Environment):
 
     def __init__(self, environment_name):
         super().__init__(environment_name)
 
         self._players = {}
     
+    @abstractmethod
     def add_player(self, player):
-        assert isinstance(player, Agent), "A player must be an instance of an Agent subclass."
+        pass
 
-        player_name = player.who_am_I()
-        self._players[player_name] = player
+    def get_player(self, player_name):
+        assert player_name in self._players.keys(), "The player with name '{0}' was not added to the game.".format(player_name)
 
-        return player_name
+        return self._players[player_name]
     
     @abstractmethod
     def get_game_state(self):
         pass
 
     @abstractstaticmethod
     def get_legal_actions(game_state):
         pass
 
     @abstractstaticmethod
     def is_terminal(game_state):
         pass
+    
+    @abstractstaticmethod
+    def get_winner(game_state):
+        pass
 
     @abstractstaticmethod
     def transition_result(game_state, action):
         pass
 
     @abstractstaticmethod
     def turn(game_state):
```

### Comparing `une_ai-1.0.0/src/une_ai/models/graph_node.py` & `une_ai-1.1.0/src/une_ai/models/graph_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,9 @@
             path_cost += path_cost_parent
             path = path_parent + path
 
         self._path = path
         self._path_cost = path_cost
         
         return path, path_cost
+
```

### Comparing `une_ai-1.0.0/src/une_ai/models/grid_map.py` & `une_ai-1.1.0/src/une_ai/models/grid_map.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.0.0/src/une_ai/tictactoe/tictactoe_game.py` & `une_ai-1.1.0/src/une_ai/tictactoe/tictactoe_game.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,141 +1,134 @@
-from une_ai.tictactoe import TicTacToeGameEnvironment
-from une_ai.tictactoe import TicTacToePlayer
-
 import pygame
-import math
-import random
 
 BLACK = (0, 0, 0)
 WHITE = (255, 255, 255)
 RED = (255, 0, 0)
 BLUE = (0, 0, 255)
 
-pygame.init()
 DISPLAY_WIDTH = 320
 DISPLAY_HEIGHT = 240
 SCORE_BAR_HEIGHT = 40
 BOX_SIZE = 50
 
-window = pygame.display.set_mode((DISPLAY_WIDTH, DISPLAY_HEIGHT+SCORE_BAR_HEIGHT))
-pygame.display.set_caption('Tic Tac Toe')
-window_clock = pygame.time.Clock()
-
 class TicTacToeGame:
 
-    def __init__(self, agent_program_MAX, agent_program_MIN, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, box_size=BOX_SIZE):
+    def __init__(self, agent_X, agent_O, environment, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, box_size=BOX_SIZE):
+        assert type(agent_X).__name__ == 'TicTacToePlayer', "agent_X must be an instance of a the class TicTacToePlayer"
+        assert type(agent_O).__name__ == 'TicTacToePlayer', "agent_O must be an instance of the class TicTacToePlayer"
+        assert type(environment).__name__ == 'TicTacToeGameEnvironment', "The parameter environment must be an instance of the class TicTacToeGameEnvironment"
+        
+        pygame.init()
+        window = pygame.display.set_mode((DISPLAY_WIDTH, DISPLAY_HEIGHT+SCORE_BAR_HEIGHT))
+        pygame.display.set_caption('Tic Tac Toe')
+        self._window_clock = pygame.time.Clock()
+
         self._box_size = box_size
         self._display = window
         self._display_size = (display_w, display_h)
         self._agents = {}
-        self._agents['MAX'] = TicTacToePlayer('MAX', agent_program_MAX)
-        self._agents['MIN'] = TicTacToePlayer('MIN', agent_program_MIN)
-        self._environment = TicTacToeGameEnvironment(
-            self._agents['MAX'],
-            self._agents['MIN'],
-        )
+        self._agents['X'] = agent_X
+        self._agents['O'] = agent_O
+        self._environment = environment
         
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
         # try to look among the most common fonts
         test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica']
         for font in test_fonts:
             if font in fonts:
                 self._font = font
                 break
 
         self.main()
         
     def _play_step(self):
         game_state = self._environment.get_game_state()
-        if TicTacToeGameEnvironment.is_terminal(game_state):
+        if type(self._environment).is_terminal(game_state):
             return
         
-        cur_marker = TicTacToeGameEnvironment.turn(game_state)
-        cur_player = self._environment.get_player_name(cur_marker)
+        cur_marker = type(self._environment).turn(game_state)
         
         # SENSE
-        self._agents[cur_player].sense(self._environment)
+        self._agents[cur_marker].sense(self._environment)
         # THINK
-        actions = self._agents[cur_player].think()
+        actions = self._agents[cur_marker].think()
         # ACT
-        self._agents[cur_player].act(actions, self._environment)
+        self._agents[cur_marker].act(actions, self._environment)
     
     def _reset_bg(self):
         self._display.fill(BLACK)
     
     def _draw_box(self, x, y, color, alpha = 255):
         font = pygame.font.SysFont(self._font, 30)
         game_state = self._environment.get_game_state()
-        padding_left = int((self._display_size[0] - 3*self._box_size)/2)
-        padding_top = int((self._display_size[1] - 3*self._box_size)/2)
+        n_cells = self._environment.get_board_size()
+        padding_left = int((self._display_size[0] - n_cells*self._box_size)/2)
+        padding_top = int((self._display_size[1] - n_cells*self._box_size)/2)
         x_coord = padding_left + x*self._box_size
         y_coord = padding_top + y*self._box_size
 
         surface = pygame.Surface((self._box_size-2,self._box_size-2))
         surface.set_alpha(alpha) # alpha level
         pygame.draw.rect(surface, color, surface.get_rect())
-        self._display.blit(surface, (x_coord, y_coord,self._box_size,self._box_size) )
+        self._display.blit(surface, (x_coord, y_coord) )
 
-        cur_mark = game_state.get_item_value(x, y)
+        game_board = game_state['game-board']
+        cur_mark = game_board.get_item_value(x, y)
         if cur_mark != None:
             color = RED if cur_mark == 'X' else BLUE
             text_size = font.size(cur_mark)
             mark_text = font.render(cur_mark, True, color)
             top = y_coord + int((BOX_SIZE - text_size[1])/2)
             left = x_coord + int((BOX_SIZE - text_size[0])/2)
-            self._display.blit(mark_text, (left, top, text_size[0], text_size[1]))
+            self._display.blit(mark_text, (left, top))
     
     def _draw_board(self):
-        for i in range(0, 3):
-            for j in range(0, 3):
+        n_cells = self._environment.get_board_size()
+        for i in range(0, n_cells):
+            for j in range(0, n_cells):
                 self._draw_box(j, i, WHITE)
     
     def _draw_game_over(self):
-        mark = TicTacToeGameEnvironment.get_winner(self._environment.get_game_state())
-        if mark == 'X':
-            winner = 'MAX'
-        elif mark == 'O':
-            winner = 'MIN'
-        else:
-            winner = None
+        winner = type(self._environment).get_winner(self._environment.get_game_state())
         
         if winner is not None:
-            text = "Player {1} ({0}) won!".format(mark, winner)
+            text = "Player {0} won!".format(winner)
         else:
             text = "Tie!"
         
+        n_cells = self._environment.get_board_size()
         font = pygame.font.SysFont(self._font, 20)
         text_size = font.size(text)
         game_over_text = font.render(text, True, WHITE)
-        padding_top = int((self._display_size[1] - 3*self._box_size)/2)
+        padding_top = int((self._display_size[1] - n_cells*self._box_size)/2)
         x_coord = int((self._display_size[0] - text_size[0])/2)
-        y_coord = padding_top + 3*self._box_size + 30
-        self._display.blit(game_over_text, (x_coord, y_coord, text_size[0], text_size[1]))
+        y_coord = padding_top + n_cells*self._box_size + 30
+        self._display.blit(game_over_text, (x_coord, y_coord))
                 
     def _draw_frame(self):
         self._reset_bg()
         self._draw_board()
-        if TicTacToeGameEnvironment.is_terminal(self._environment.get_game_state()):
+        if type(self._environment).is_terminal(self._environment.get_game_state()):
             self._draw_game_over()
 
     def main(self):
         running = True
 
         while running:
             # update frame
             self._draw_frame()
+            # Update the clock and display
+            pygame.display.update()
 
             #Event Tasking
             for event in pygame.event.get():
                 if event.type == pygame.QUIT:
                     pygame.quit()
                     running = False
                     quit()
             
             # updating game with one step
             # sense - think - act
             self._play_step()
-
-            # Update the clock and display
-            pygame.display.update()
-            window_clock.tick(1)
+            
+            self._window_clock.tick(1)
```

### Comparing `une_ai-1.0.0/src/une_ai/vacuum/vacuum_environment.py` & `une_ai-1.1.0/src/une_ai/vacuum/vacuum_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.0.0/src/une_ai/vacuum/vacuum_game.py` & `une_ai-1.1.0/src/une_ai/vacuum/vacuum_game.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-from une_ai.vacuum import VacuumEnvironment
 from une_ai.models import Agent
 
 import pygame
 import math
 
 BLACK = (0, 0, 0)
 WHITE = (255, 255, 255)
 RED = (255, 0, 0)
 GREEN = (0, 255, 0)
 BLUE = (0, 0, 255)
 YELLOW = (255, 255, 0)
+MAGENTA = (255, 0, 255)
 
 pygame.init()
 DISPLAY_WIDTH = 320
 DISPLAY_HEIGHT = 240
 SCORE_BAR_HEIGHT = 40
 TILE_SIZE = 10
 
 window = pygame.display.set_mode((DISPLAY_WIDTH, DISPLAY_HEIGHT+SCORE_BAR_HEIGHT))
 pygame.display.set_caption('Vacuum cleaner agent')
 window_clock = pygame.time.Clock()
 
 class VacuumGame:
 
-    def __init__(self, vacuum_agent, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, tile_size=TILE_SIZE):
+    def __init__(self, vacuum_agent, uses_charging_dock=False, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, tile_size=TILE_SIZE):
         assert isinstance(vacuum_agent, Agent), "The parameter vacuum_agent must be an instance of a subclass of the class Agent."
 
         self._tile_size = tile_size
         self._display = window
         self._display_size = (display_w, display_h)
         w_env = math.floor(display_w / self._tile_size)
         h_env = math.floor(display_h / self._tile_size)
-        self._environment = VacuumEnvironment(w_env, h_env)
+        if uses_charging_dock:
+            from une_ai.vacuum import VacuumDockEnvironment
+            self._environment = VacuumDockEnvironment(w_env, h_env)
+        else:
+            from une_ai.vacuum import VacuumEnvironment
+            self._environment = VacuumEnvironment(w_env, h_env)
         self._agent = vacuum_agent
 
         # updating the sensors based on initial environment state
         self._agent.sense(self._environment)
 
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
@@ -64,14 +69,22 @@
         y_coord = y*self._tile_size
 
         surface = pygame.Surface((self._tile_size,self._tile_size))
         surface.set_alpha(alpha) # alpha level
         pygame.draw.rect(surface, color, surface.get_rect())
         self._display.blit(surface, (x_coord, y_coord,self._tile_size,self._tile_size) )
     
+    def _draw_charging_dock(self):
+        try:
+            x, y = self._environment.get_charging_dock_location()
+            self._draw_tile(x, y, MAGENTA)
+        except:
+            # using the environment without charging dock
+            pass
+    
     def _draw_vacuum_agent(self):
         color = GREEN
         p = self._environment.get_percepts()
         pos = (p['location-sensor'][0], p['location-sensor'][1])
         agent_state = self._environment.get_agent_state()
         if agent_state['collided'] is not None:
             color = YELLOW
@@ -116,14 +129,15 @@
         self._display.blit(battery_text, (int(DISPLAY_WIDTH/2), DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2), SCORE_BAR_HEIGHT))
 
     def _draw_frame(self):
         self._reset_bg()
         self._draw_walls()
         self._draw_explored()
         self._draw_dirt()
+        self._draw_charging_dock()
         self._draw_vacuum_agent()
         self._draw_score_bar()
 
     def main(self):
         running = True
 
         while running:
```

### Comparing `une_ai-1.0.0/src/une_ai.egg-info/PKG-INFO` & `une_ai-1.1.0/src/une_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une-ai
-Version: 1.0.0
+Version: 1.1.0
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.0.0/src/une_ai.egg-info/SOURCES.txt` & `une_ai-1.1.0/src/une_ai.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 src/une_ai/__init__.py
 src/une_ai.egg-info/PKG-INFO
 src/une_ai.egg-info/SOURCES.txt
 src/une_ai.egg-info/dependency_links.txt
 src/une_ai.egg-info/requires.txt
 src/une_ai.egg-info/top_level.txt
 src/une_ai/assignments/__init__.py
+src/une_ai/assignments/connect_four_base_environment.py
+src/une_ai/assignments/connect_four_game.py
 src/une_ai/assignments/snake_environment.py
 src/une_ai/assignments/snake_game.py
+src/une_ai/models/MCTS_graph_node.py
 src/une_ai/models/__init__.py
 src/une_ai/models/agent.py
 src/une_ai/models/environment.py
 src/une_ai/models/game_environment.py
 src/une_ai/models/graph_node.py
 src/une_ai/models/grid_map.py
+src/une_ai/models/transposition_table.py
 src/une_ai/tictactoe/__init__.py
 src/une_ai/tictactoe/tictactoc_player.py
 src/une_ai/tictactoe/tictactoe_game.py
-src/une_ai/tictactoe/tictactoe_game_environment.py
 src/une_ai/vacuum/__init__.py
+src/une_ai/vacuum/vacuum_dock_environment.py
 src/une_ai/vacuum/vacuum_environment.py
 src/une_ai/vacuum/vacuum_game.py
```

