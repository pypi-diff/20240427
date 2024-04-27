# Comparing `tmp/pypzbattlesnake-0.0.2.tar.gz` & `tmp/pypzbattlesnake-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypzbattlesnake-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pypzbattlesnake-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pypzbattlesnake-0.0.2.tar` & `pypzbattlesnake-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2024-01-27 07:48:22.501867 pypzbattlesnake-0.0.2/LICENSE
--rw-r--r--   0        0        0      133 2024-01-29 18:53:04.611042 pypzbattlesnake-0.0.2/README.md
--rw-r--r--   0        0        0      716 2024-01-30 18:41:48.876563 pypzbattlesnake-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      139 2024-02-01 06:59:46.533649 pypzbattlesnake-0.0.2/src/pypzbattlesnake/__init__.py
--rw-r--r--   0        0        0      590 2023-11-11 13:53:49.112658 pypzbattlesnake-0.0.2/src/pypzbattlesnake/common.py
--rw-r--r--   0        0        0    12878 2024-01-29 18:38:47.819387 pypzbattlesnake-0.0.2/src/pypzbattlesnake/env.py
--rw-r--r--   0        0        0     4698 2024-01-30 18:41:22.632776 pypzbattlesnake-0.0.2/src/pypzbattlesnake/renderer.py
--rw-r--r--   0        0        0      255 2023-08-28 11:10:44.500092 pypzbattlesnake-0.0.2/src/pypzbattlesnake/resources/head.svg
--rw-r--r--   0        0        0      122 2023-08-28 11:10:49.416759 pypzbattlesnake-0.0.2/src/pypzbattlesnake/resources/tail.svg
--rw-r--r--   0        0        0    11416 2024-01-29 18:45:15.432069 pypzbattlesnake-0.0.2/tests/battlesnake_test.py
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 pypzbattlesnake-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-01-27 07:48:22.501867 pypzbattlesnake-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3201 2024-04-27 10:12:05.431529 pypzbattlesnake-0.0.3/README.md
+-rw-r--r--   0        0        0      716 2024-01-30 18:41:48.876563 pypzbattlesnake-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      139 2024-03-21 10:51:01.148779 pypzbattlesnake-0.0.3/src/pypzbattlesnake/__init__.py
+-rw-r--r--   0        0        0      590 2023-11-11 13:53:49.112658 pypzbattlesnake-0.0.3/src/pypzbattlesnake/common.py
+-rw-r--r--   0        0        0    14760 2024-04-06 07:06:33.801713 pypzbattlesnake-0.0.3/src/pypzbattlesnake/env.py
+-rw-r--r--   0        0        0     5065 2024-03-29 06:16:44.281886 pypzbattlesnake-0.0.3/src/pypzbattlesnake/renderer.py
+-rw-r--r--   0        0        0      255 2023-08-28 11:10:44.500092 pypzbattlesnake-0.0.3/src/pypzbattlesnake/resources/head.svg
+-rw-r--r--   0        0        0      122 2023-08-28 11:10:49.416759 pypzbattlesnake-0.0.3/src/pypzbattlesnake/resources/tail.svg
+-rw-r--r--   0        0        0    12575 2024-03-31 07:08:07.607082 pypzbattlesnake-0.0.3/tests/battlesnake_test.py
+-rw-r--r--   0        0        0     3952 1970-01-01 00:00:00.000000 pypzbattlesnake-0.0.3/PKG-INFO
```

### Comparing `pypzbattlesnake-0.0.2/LICENSE` & `pypzbattlesnake-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypzbattlesnake-0.0.2/pyproject.toml` & `pypzbattlesnake-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypzbattlesnake-0.0.2/src/pypzbattlesnake/common.py` & `pypzbattlesnake-0.0.3/src/pypzbattlesnake/common.py`

 * *Files identical despite different names*

### Comparing `pypzbattlesnake-0.0.2/src/pypzbattlesnake/env.py` & `pypzbattlesnake-0.0.3/src/pypzbattlesnake/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import functools
 import math
-from typing import Tuple, Dict, Set
+from typing import Tuple, Dict, Set, List
 
 import gymnasium
 import numpy as np
 import pettingzoo
 from pettingzoo.utils.env import AgentID
 
 from .common import Action, SHIFT_BY_ACTION, OPPOSITE_ACTION, BASE_COLORS_COUNT, FOOD_COLOR, EMPTY_COLOR
 from .renderer import BattleSnakeRenderer
 
 ActionSpace = gymnasium.spaces.Discrete(5)
 
 
 class Snake:
-
     _color = FOOD_COLOR
 
-    def __init__(self, init_pos, team):
+    def __init__(self, init_pos, team, head_color=True):
 
         self.body: list[tuple[int, int]] = [init_pos]
         self.team = team
 
         Snake._color += 1
         self.color = Snake._color
-        Snake._color += 1
+        if head_color:
+            Snake._color += 1
         self.head_color = Snake._color
         self.action = Action.NONE
         self.health = 100
 
     def step(self, action):
 
         if action != Action.NONE and self.action != OPPOSITE_ACTION[action]:
             self.action = action
 
         self.health -= 1
 
         shift = SHIFT_BY_ACTION[self.action]
 
-        head_block = self.body[-1]
+        head_block = self.head()
         next_block = (head_block[0] + shift[0], head_block[1] + shift[1])
 
         self.body.append(next_block)
 
     def heal(self):
         self.health = 100
 
@@ -53,21 +53,25 @@
         return self.body[0]
 
 
 class BattleSnake(pettingzoo.ParallelEnv):
 
     def __init__(self, teams_count,
                  team_snakes_count, size: Tuple[int, int] = (15, 15),
-                 min_food_count: int = 5, food_spawn_interval=5, food_reward=0.1, render_mode="human"):
+                 min_food_count: int = 5, food_spawn_interval=5, food_reward=0.1, head_color=True,
+                 render_mode="human"):
 
         super().__init__()
         self.teams_count = teams_count
         self.team_snakes_count = team_snakes_count
         self.snakes_count = teams_count * team_snakes_count
-        self.colors_count = 2 * self.snakes_count + BASE_COLORS_COUNT
+        self.colors_count = self.snakes_count + BASE_COLORS_COUNT
+        self.head_color = head_color
+        if self.head_color:
+            self.colors_count += self.snakes_count
 
         self.render_mode = render_mode
 
         self.size = size
         self.max_dist = sum(size)
         self.init_positions = self._get_init_pos()
 
@@ -124,15 +128,15 @@
         self.agents = self.possible_agents.copy()
 
         Snake._color = FOOD_COLOR
         self.snakes = {}
         snake_position = iter(self.init_positions)
         for idx, team in enumerate(self.teams):
             for agent in team:
-                self.snakes[agent] = Snake(next(snake_position), team=idx)
+                self.snakes[agent] = Snake(next(snake_position), team=idx, head_color=self.head_color)
 
         self.color_mapping = self.get_color_mapping()
         self.food = set()
         for _ in range(self.min_food_count):
             self.food.add(self.random_empty_position())
         self.food_spawn_timer = 0
 
@@ -144,33 +148,36 @@
 
         return observation, info
 
     def step(self, action: Dict[str, int]):
 
         action = {agent: Action(act + 1) for agent, act in action.items()}
 
-        before_food_distance = {agent: self.find_closest_food(self.snakes[agent].head())[1] for agent in self.snakes}
+        before_food_distance = {agent: self.find_closest_food(self.snakes[agent].head()) for agent in self.snakes}
 
         for agent, act in action.items():
             if agent in self.snakes:
                 self.snakes[agent].step(act)
 
-        after_food_distance = {agent: self.find_closest_food(self.snakes[agent].head())[1] for agent in self.snakes}
+        after_food_distance = {agent: self.find_closest_food(self.snakes[agent].head()) for agent in self.snakes}
         self.reward = {
             agent: (before_food_distance[agent] - after_food_distance[agent]) / self.max_dist * self.food_reward
             if agent in self.snakes else 0 for agent in action}
 
         self.check_health()
         self.check_border_collisions()
         self.check_food_collisions()
         self.check_self_collisions()
         self.check_head_head_collisions()
         self.check_another_collisions()
 
-        self.spawn_food()
+        try:
+            self.spawn_food()
+        except ValueError as e:
+            pass
 
         end_game = self.check_end_game()
 
         observation = {agent: self.get_observation(agent) for agent in action}
         if end_game:
             terminated = {agent: True for agent in action}
             self.eliminate(self.agents.copy())
@@ -182,57 +189,62 @@
         return observation, self.reward, terminated, truncated, info
 
     def find_closest_food(self, pos):
 
         def distance(point1, point2):
             return abs(point1[0] - point2[0]) + abs(point1[1] - point2[1])
 
+        if not len(self.food):
+            return 0
+
         closest_food = next(iter(self.food))
         min_dist = distance(closest_food, pos)
 
         for food in self.food:
             dist = distance(food, pos)
             if dist < min_dist:
-                closest_food = food
                 min_dist = dist
 
-        return closest_food, min_dist
+        return min_dist
 
     def check_health(self):
         eliminate_agents = []
         for agent in self.agents:
             if self.snakes[agent].health <= 0:
                 eliminate_agents.append(agent)
         self.eliminate(eliminate_agents)
 
+    def is_border_collision(self, position):
+        return not (0 <= position[0] < self.size[0]) or not (0 <= position[1] < self.size[1])
+
     def check_border_collisions(self):
         eliminate_agents = []
         for agent in self.agents:
-            head = self.snakes[agent].head()
-            if not (0 <= head[0] < self.size[0]) or not (0 <= head[1] < self.size[1]):
+            if self.is_border_collision(self.snakes[agent].head()):
                 eliminate_agents.append(agent)
         self.eliminate(eliminate_agents)
 
     def check_food_collisions(self):
         for agent in self.agents:
             snake = self.snakes[agent]
             snake_head = snake.body[-1]
             if snake_head in self.food:
                 snake.heal()
                 self.food.remove(snake_head)
                 self.reward[agent] = self.food_reward
             else:
                 snake.body.pop(0)
 
+    def is_body_collision(self, snake, position):
+        return position in snake.body[:-1]
+
     def check_self_collisions(self):
         eliminate_agents = []
         for agent in self.agents:
-            snake = self.snakes[agent]
-            snake_head = snake.head()
-            if snake_head in snake.body[:-1]:
+            if self.is_body_collision(self.snakes[agent], self.snakes[agent].head()):
                 eliminate_agents.append(agent)
         self.eliminate(eliminate_agents)
 
     def check_head_head_collisions(self):
         eliminate_agents = []
         all_heads = [self.snakes[agent].head() for agent in self.agents]
         for agent in self.agents:
@@ -249,42 +261,42 @@
                     eliminate_agents.append(agent)
                     self.reward[other_agent] = -1.0 if self.snakes[agent].team == self.snakes[other_agent].team else 1.0
         self.eliminate(eliminate_agents)
 
     def eliminate(self, eliminate_agent):
         for agent in eliminate_agent:
             self.reward[agent] = -1.0
-            self.agents.remove(agent)
             snake = self.snakes[agent]
             for teammate in self.teams[snake.team]:
                 if teammate in self.reward:
                     self.reward[teammate] = -1.0
+            self.agents.remove(agent)
             self.snakes.pop(agent)
             self.eliminated_agents.add(agent)
 
     def get_color_mapping(self):
 
         def agent_color_mapping(snake_id):
             snake = self.snakes[snake_id]
             snake_color_mapping = [0, ] * self.colors_count
             snake_color_mapping[1] = 1
             current_agent_color = BASE_COLORS_COUNT
             snake_color_mapping[snake.color] = current_agent_color
-            snake_color_mapping[snake.head_color] = current_agent_color + 1
+            snake_color_mapping[snake.head_color] = current_agent_color + self.head_color
             for teammate in self.teams[snake.team]:
                 if teammate != snake_id:
-                    current_agent_color += 2
+                    current_agent_color += 1 + self.head_color
                     snake_color_mapping[self.snakes[teammate].color] = current_agent_color
-                    snake_color_mapping[self.snakes[teammate].head_color] = current_agent_color + 1
+                    snake_color_mapping[self.snakes[teammate].head_color] = current_agent_color + self.head_color
             for opponent_team in range(len(self.teams)):
                 if opponent_team != snake.team:
                     for opponent in self.teams[opponent_team]:
-                        current_agent_color += 2
+                        current_agent_color += 1 + self.head_color
                         snake_color_mapping[self.snakes[opponent].color] = current_agent_color
-                        snake_color_mapping[self.snakes[opponent].head_color] = current_agent_color + 1
+                        snake_color_mapping[self.snakes[opponent].head_color] = current_agent_color + self.head_color
             return snake_color_mapping
 
         return {snake_id: agent_color_mapping(snake_id) for snake_id in self.possible_agents}
 
     def as_array(self):
 
         field = np.zeros(self.size, dtype=np.int64)
@@ -318,15 +330,15 @@
         empty_indices = np.argwhere(field == EMPTY_COLOR)
         index = rng.choice(empty_indices, axis=0)
         return tuple(index)
 
     @functools.lru_cache(maxsize=None)
     def observation_space(self, agent: AgentID):
         dim = math.prod(self.size)
-        dim = np.full((dim,), BASE_COLORS_COUNT + 2*self.snakes_count)
+        dim = np.full((dim,), self.colors_count)
         return gymnasium.spaces.MultiDiscrete(dim)
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent: AgentID):
         return ActionSpace
 
     def render(self) -> None:
@@ -342,22 +354,58 @@
 
     def init_template(self):
         return {"colors_count": self.snakes_count + BASE_COLORS_COUNT,
                 "field_x": self.size[0],
                 "field_y": self.size[1]}
 
     def check_end_game(self):
-        teams_left = set()
-        for name, snake in self.snakes.items():
-            teams_left.add(snake.team)
+        if self.teams_count > 1:
+            teams_left = set()
+            for name, snake in self.snakes.items():
+                teams_left.add(snake.team)
 
-        return len(teams_left) <= 1
+            return len(teams_left) <= 1
+        else:
+            return len(self.snakes) == 0
 
     def spawn_food(self):
 
         while len(self.food) < self.min_food_count:
             self.food.add(self.random_empty_position())
 
         self.food_spawn_timer += 1
         if self.food_spawn_timer >= self.food_spawn_interval:
             self.food.add(self.random_empty_position())
             self.food_spawn_timer = 0
+
+    def action_masks(self, agent: AgentID) -> List[bool]:
+
+        def check_action_validity(snake: Snake, action) -> bool:
+            if snake is None:
+                return action == Action.NONE
+            if snake.action != Action.NONE and action == OPPOSITE_ACTION[snake.action]:
+                return False
+            if action == Action.NONE:
+                action = snake.action
+            head = snake.head()
+            next_position = (head[0] + SHIFT_BY_ACTION[action][0], head[1] + SHIFT_BY_ACTION[action][1])
+            if self.is_border_collision(next_position):
+                return False
+            for s_agent, s in self.snakes.items():
+                if s_agent == agent and s.head() == next_position:
+                    continue
+                if s.tail() == next_position:
+                    continue
+                if self.is_body_collision(s, next_position):
+                    return False
+                if s.head() == next_position:
+                    return False
+            return True
+
+        snake = self.snakes.get(agent, None)
+        mask = [check_action_validity(snake, action) for action in Action]
+        if not np.any(mask):
+            mask[-1] = True
+        return mask
+
+    def get_head(self, agent):
+        return self.snakes[agent].head()
```

### Comparing `pypzbattlesnake-0.0.2/src/pypzbattlesnake/renderer.py` & `pypzbattlesnake-0.0.3/src/pypzbattlesnake/renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 def random_color():
     h = np.random.default_rng().random()
     return tuple(map(lambda x: int(255 * x), colorsys.hls_to_rgb(h, 0.4, 0.8)))
 
 
 PALITE = [(0, 104, 139), (0, 104, 139), (159, 0, 255), (159, 0, 255), (212, 137, 28), (212, 137, 28), (0, 155, 92),
           (0, 155, 92)]
+HEADLESS_PALITE = [(0, 104, 139), (159, 0, 255), (212, 137, 28), (0, 155, 92)]
 
 
 def get_shift(cell_a, cell_b):
     return cell_a[0] - cell_b[0], cell_a[1] - cell_b[1]
 
 
 class BattleSnakeRenderer:
@@ -51,16 +52,21 @@
         file_path = pathlib.Path(__file__).parent.resolve()
 
         size_x = self.env.size[0] * (RECT_SIZE + RECT_PADDING) + GRID_PADDING * 2 - RECT_PADDING
         size_y = self.env.size[1] * (RECT_SIZE + RECT_PADDING) + GRID_PADDING * 2 - RECT_PADDING
         self.screen = pygame.display.set_mode((size_x, size_y))
 
         self.field: list[list[pygame.Rect]] = []
-        self.snake_colors = {snake.color: random_color() if snake.color - BASE_COLORS_COUNT > len(PALITE)
-                             else PALITE[snake.color - BASE_COLORS_COUNT] for _, snake in self.env.snakes.items()}
+        if env.head_color:
+            self.snake_colors = {snake.color: random_color() if snake.color - BASE_COLORS_COUNT > len(PALITE)
+                                 else PALITE[snake.color - BASE_COLORS_COUNT] for _, snake in self.env.snakes.items()}
+        else:
+            self.snake_colors = {snake.color: random_color() if snake.color - BASE_COLORS_COUNT > len(PALITE)
+                                 else HEADLESS_PALITE[snake.color - BASE_COLORS_COUNT] for _, snake in self.env.snakes.items()}
+
 
         rect_x = GRID_PADDING
         for x in range(self.env.size[0]):
             rect_y = GRID_PADDING
             self.field.append([])
             for y in range(self.env.size[1]):
                 self.field[-1].append(pygame.Rect(rect_x, rect_y, RECT_SIZE, RECT_SIZE))
```

### Comparing `pypzbattlesnake-0.0.2/tests/battlesnake_test.py` & `pypzbattlesnake-0.0.3/tests/battlesnake_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import multiset
 from pettingzoo.test import parallel_api_test
 
-from pypzbattlesnake import Action
+from pypzbattlesnake.common import Action
 from pypzbattlesnake import BattleSnake
 
 REWARD_STEP = 1 / 18
 FLOAT_EPS = 0.00001
 
 
 def count_cell_colors(obs):
@@ -66,14 +66,19 @@
     assert env.snakes["snake_0_1"].color == 4
     assert env.snakes["snake_0_1"].head_color == 5
     assert env.snakes["snake_1_0"].color == 6
     assert env.snakes["snake_1_0"].head_color == 7
     assert env.snakes["snake_1_1"].color == 8
     assert env.snakes["snake_1_1"].head_color == 9
 
+    assert env.action_masks("snake_0_0") == [True, True, True, True, True]
+    assert env.action_masks("snake_0_1") == [True, True, True, True, True]
+    assert env.action_masks("snake_1_0") == [True, True, True, True, True]
+    assert env.action_masks("snake_1_1") == [True, True, True, True, True]
+
 
 def test_step():
     env = BattleSnake(2, 2, (9, 9), 3, 5, 1.0)
     observation, _, = env.reset()
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
     assert env.snakes["snake_0_0"].head() == (1, 1)
     assert field[1][1] == 3
@@ -84,34 +89,37 @@
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
 
     assert env.snakes["snake_0_0"].head() == (1, 0)
     assert field[1][0] == 3
     assert abs(reward["snake_0_0"] - -REWARD_STEP) < FLOAT_EPS
     assert not terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
+    assert env.action_masks("snake_0_0") == [False, False, True, True, True]
 
     observation, reward, terminated, truncated, _ = env.step(
         {"snake_0_0": 2, "snake_0_1": 4,
          "snake_1_0": 4, "snake_1_1": 4})
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
 
     assert env.snakes["snake_0_0"].head() == (0, 0)
     assert field[0][0] == 3
+    assert env.action_masks("snake_0_0") == [False, True, False, False, True]
 
     assert abs(reward["snake_0_0"] - -REWARD_STEP) < FLOAT_EPS
     assert not terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
 
     observation, reward, terminated, truncated, _ = env.step(
         {"snake_0_0": 1, "snake_0_1": 4,
          "snake_1_0": 4, "snake_1_1": 4})
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
 
     assert env.snakes["snake_0_0"].head() == (0, 1)
     assert field[0][1] == 3
+    assert env.action_masks("snake_0_0") == [False, True, False, True, True]
 
     assert abs(reward["snake_0_0"] - REWARD_STEP) < FLOAT_EPS
     assert not terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
 
     observation, reward, terminated, truncated, _ = env.step(
         {"snake_0_0": 3, "snake_0_1": 4,
@@ -120,14 +128,15 @@
 
     assert env.snakes["snake_0_0"].head() == (1, 1)
     assert field[1][1] == 3
 
     assert abs(reward["snake_0_0"] - REWARD_STEP) < FLOAT_EPS
     assert not terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
+    assert env.action_masks("snake_0_0") == [True, True, False, True, True]
 
 
 def test_border_collision():
 
     env = BattleSnake(2, 2, (9, 9), 3, 5, 1.0)
     observation, _, = env.reset()
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
@@ -144,24 +153,26 @@
     assert env.snakes["snake_0_0"].head() == (1, 0)
     assert field[1][0] == 3
 
     assert abs(reward["snake_0_0"] - -REWARD_STEP) < FLOAT_EPS
     assert not terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
     assert count_cell_colors(observation) == multiset.Multiset([3, 0, 1, 0, 1, 0, 1, 0, 1])
+    assert env.action_masks("snake_0_0") == [False, False, True, True, True]
 
     observation, reward, terminated, truncated, _ = env.step({"snake_0_0": 0, "snake_0_1": 4,
                                                               "snake_1_0": 4, "snake_1_1": 4})
 
     assert env.snakes.get("snake_0_0", None) is None
     assert count_cell_colors(observation) == multiset.Multiset([3, 0, 0, 0, 1, 0, 1, 0, 1])
 
     assert abs(reward["snake_0_0"] - -1.0) < FLOAT_EPS
     assert terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
+    assert env.action_masks("snake_0_0") == [False, False, False, False, True]
 
 
 def test_food_collision():
     env = BattleSnake(2, 2, (9, 9), 3, 5, 1.0)
     observation, _, = env.reset()
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
 
@@ -189,14 +200,15 @@
 def test_another_collision():
     env = BattleSnake(2, 2, (9, 9), 3, 5, 1.0)
     observation, _, = env.reset()
 
     env.snakes["snake_1_0"].body = [(2, 0), (2, 1), (2, 2)]
     env.snakes["snake_1_0"].action = Action.DOWN
     env.food = {(6, 1), (1, 6), (6, 6)}
+    assert env.action_masks("snake_0_0") == [True, True, True, False, True]
 
     observation, reward, terminated, truncated, _ = env.step(
         {"snake_0_0": 3, "snake_0_1": 4,
          "snake_1_0": 4, "snake_1_1": 4})
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
 
     assert env.snakes.get("snake_0_0", None) is None
@@ -206,23 +218,25 @@
     assert field[2][2] == 6
     assert field[2][3] == 7
 
     assert abs(reward["snake_0_0"] - -1.0) < FLOAT_EPS
     assert abs(reward["snake_1_0"] - 1.0) < FLOAT_EPS
     assert terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
+    assert env.action_masks("snake_0_0") == [False, False, False, False, True]
 
 
 def test_teammate_collision():
     env = BattleSnake(2, 2, (9, 9), 3, 5, 1.0)
     observation, _, = env.reset()
 
     env.snakes["snake_0_1"].body = [(2, 0), (2, 1), (2, 2)]
     env.snakes["snake_0_1"].action = Action.DOWN
     env.food = {(6, 1), (1, 6), (6, 6)}
+    assert env.action_masks("snake_0_0") == [True, True, True, False, True]
 
     observation, reward, terminated, truncated, _ = env.step(
         {"snake_0_0": 3, "snake_0_1": 4,
          "snake_1_0": 4, "snake_1_1": 4})
     field = np.reshape(observation["snake_0_0"][:81], (9, 9))
 
     assert env.snakes.get("snake_0_0", None) is None
@@ -232,14 +246,15 @@
     assert field[2][2] == 4
     assert field[2][3] == 5
 
     assert abs(reward["snake_0_0"] - -1.0) < FLOAT_EPS
     assert abs(reward["snake_0_1"] - -1.0) < FLOAT_EPS
     assert terminated["snake_0_0"]
     assert not truncated["snake_0_0"]
+    assert env.action_masks("snake_0_0") == [False, False, False, False, True]
 
 
 def test_head_collision():
     env = BattleSnake(2, 2, (9, 9), 3, 5, 1.0)
     observation, _, = env.reset()
 
     env.snakes["snake_1_0"].body = [(4, 1), (3, 1)]
@@ -272,14 +287,15 @@
 def test_self_collision():
     env = BattleSnake(2, 2, (9, 9), 3, 5, 1.0)
     observation, _, = env.reset()
 
     env.snakes["snake_0_0"].body = [(0, 1), (1, 1), (2, 1), (2, 2), (1, 2)]
     env.snakes["snake_0_0"].action = Action.LEFT
     env.food = {(6, 1), (1, 6), (6, 6)}
+    assert env.action_masks("snake_0_0") == [False, True, True, False, True]
 
     observation, reward, terminated, truncated, _ = env.step(
         {"snake_0_0": 0, "snake_0_1": 4,
          "snake_1_0": 4, "snake_1_1": 4})
 
     assert env.snakes.get("snake_0_0", None) is None
     assert count_cell_colors(observation) == multiset.Multiset([3, 0, 0, 0, 1, 0, 1, 0, 1])
```

