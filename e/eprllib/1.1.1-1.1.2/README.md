# Comparing `tmp/eprllib-1.1.1.tar.gz` & `tmp/eprllib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eprllib-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eprllib-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eprllib-1.1.1.tar` & `eprllib-1.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     6706 2024-03-22 12:29:57.414473 eprllib-1.1.1/README.md
--rw-r--r--   0        0        0      660 2024-05-15 12:23:14.428918 eprllib-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 20:01:08.588762 eprllib-1.1.1/src/eprllib/ExampleFiles/__init__.py
--rw-r--r--   0        0        0  1648753 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw
--rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/epw/__init__.py
--rw-r--r--   0        0        0   245096 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf
--rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/idf/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 13:27:42.113993 eprllib-1.1.1/src/eprllib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 10:07:03.001250 eprllib-1.1.1/src/eprllib/agents/__init__.py
--rw-r--r--   0        0        0     5449 2024-03-14 16:24:23.397736 eprllib-1.1.1/src/eprllib/agents/conventional.py
--rw-r--r--   0        0        0     1028 2024-03-21 08:40:43.671486 eprllib-1.1.1/src/eprllib/agents/holon_config.py
--rw-r--r--   0        0        0     1008 2024-02-12 10:25:28.186353 eprllib-1.1.1/src/eprllib/agents/user.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.360381 eprllib-1.1.1/src/eprllib/env/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 19:16:29.819874 eprllib-1.1.1/src/eprllib/env/multiagent/__init__.py
--rw-r--r--   0        0        0     8134 2024-05-15 12:08:56.602600 eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_gym_env.py
--rw-r--r--   0        0        0    24852 2024-05-15 12:04:18.306197 eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_runner.py
--rw-r--r--   0        0        0     7670 2024-03-21 15:31:48.407127 eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_gym_env.py
--rw-r--r--   0        0        0    20698 2024-03-21 15:31:48.407127 eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_runner.py
--rw-r--r--   0        0        0        0 2024-03-21 19:16:52.042116 eprllib-1.1.1/src/eprllib/env/simpleagent/__init__.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.369889 eprllib-1.1.1/src/eprllib/postprocess/__init__.py
--rw-r--r--   0        0        0     7929 2024-05-13 20:46:38.662264 eprllib-1.1.1/src/eprllib/postprocess/marl_init_conventional.py
--rw-r--r--   0        0        0     8313 2024-05-13 20:46:38.679148 eprllib-1.1.1/src/eprllib/postprocess/marl_init_evaluation.py
--rw-r--r--   0        0        0     7401 2024-05-13 20:46:38.693583 eprllib-1.1.1/src/eprllib/postprocess/marl_init_noventilation.py
--rw-r--r--   0        0        0   448967 2024-05-10 12:09:01.402850 eprllib-1.1.1/src/eprllib/postprocess/marl_results_evaluation.ipynb
--rw-r--r--   0        0        0     3002 2024-02-22 11:24:29.811391 eprllib-1.1.1/src/eprllib/postprocess/neural_networ_analysis.ipynb
--rw-r--r--   0        0        0     1636 2024-04-18 12:01:12.679943 eprllib-1.1.1/src/eprllib/preprocess/IDFProperties.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.372239 eprllib-1.1.1/src/eprllib/preprocess/__init__.py
--rw-r--r--   0        0        0     5797 2024-03-21 15:31:48.398206 eprllib-1.1.1/src/eprllib/preprocess/conventional_experience.py
--rw-r--r--   0        0        0        0 2024-02-12 10:39:26.603572 eprllib-1.1.1/src/eprllib/tools/__init__.py
--rw-r--r--   0        0        0      829 2024-03-28 10:22:08.162993 eprllib-1.1.1/src/eprllib/tools/action_transformers.py
--rw-r--r--   0        0        0     1402 2024-02-24 11:12:25.969964 eprllib-1.1.1/src/eprllib/tools/devices_space_action.py
--rw-r--r--   0        0        0    19846 2024-03-21 15:31:48.398206 eprllib-1.1.1/src/eprllib/tools/ep_episode_config.py
--rw-r--r--   0        0        0     7642 2024-05-04 16:21:41.949814 eprllib-1.1.1/src/eprllib/tools/rewards.py
--rw-r--r--   0        0        0     3180 2024-05-10 08:22:29.542577 eprllib-1.1.1/src/eprllib/tools/utils.py
--rw-r--r--   0        0        0     7134 2024-03-21 20:29:35.640440 eprllib-1.1.1/src/eprllib/tools/weather_utils.py
--rw-r--r--   0        0        0     7086 1970-01-01 00:00:00.000000 eprllib-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6706 2024-03-22 12:29:57.414473 eprllib-1.1.2/README.md
+-rw-r--r--   0        0        0      660 2024-05-17 19:24:22.998937 eprllib-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-28 20:01:08.588762 eprllib-1.1.2/src/eprllib/ExampleFiles/__init__.py
+-rw-r--r--   0        0        0  1648753 2024-03-28 20:01:08.599401 eprllib-1.1.2/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw
+-rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.2/src/eprllib/ExampleFiles/epw/__init__.py
+-rw-r--r--   0        0        0   245096 2024-03-28 20:01:08.599401 eprllib-1.1.2/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf
+-rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.2/src/eprllib/ExampleFiles/idf/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 13:27:42.113993 eprllib-1.1.2/src/eprllib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:07:03.001250 eprllib-1.1.2/src/eprllib/agents/__init__.py
+-rw-r--r--   0        0        0     5449 2024-03-14 16:24:23.397736 eprllib-1.1.2/src/eprllib/agents/conventional.py
+-rw-r--r--   0        0        0     1028 2024-03-21 08:40:43.671486 eprllib-1.1.2/src/eprllib/agents/holon_config.py
+-rw-r--r--   0        0        0     1008 2024-02-12 10:25:28.186353 eprllib-1.1.2/src/eprllib/agents/user.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.360381 eprllib-1.1.2/src/eprllib/env/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 19:16:29.819874 eprllib-1.1.2/src/eprllib/env/multiagent/__init__.py
+-rw-r--r--   0        0        0     8681 2024-05-17 19:07:35.119321 eprllib-1.1.2/src/eprllib/env/multiagent/marl_ep_gym_env.py
+-rw-r--r--   0        0        0    24852 2024-05-15 12:04:18.306197 eprllib-1.1.2/src/eprllib/env/multiagent/marl_ep_runner.py
+-rw-r--r--   0        0        0     7670 2024-03-21 15:31:48.407127 eprllib-1.1.2/src/eprllib/env/simpleagent/VENT_ep_gym_env.py
+-rw-r--r--   0        0        0    20698 2024-03-21 15:31:48.407127 eprllib-1.1.2/src/eprllib/env/simpleagent/VENT_ep_runner.py
+-rw-r--r--   0        0        0        0 2024-03-21 19:16:52.042116 eprllib-1.1.2/src/eprllib/env/simpleagent/__init__.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.369889 eprllib-1.1.2/src/eprllib/postprocess/__init__.py
+-rw-r--r--   0        0        0     7929 2024-05-13 20:46:38.662264 eprllib-1.1.2/src/eprllib/postprocess/marl_init_conventional.py
+-rw-r--r--   0        0        0     8313 2024-05-13 20:46:38.679148 eprllib-1.1.2/src/eprllib/postprocess/marl_init_evaluation.py
+-rw-r--r--   0        0        0     7401 2024-05-13 20:46:38.693583 eprllib-1.1.2/src/eprllib/postprocess/marl_init_noventilation.py
+-rw-r--r--   0        0        0   448967 2024-05-10 12:09:01.402850 eprllib-1.1.2/src/eprllib/postprocess/marl_results_evaluation.ipynb
+-rw-r--r--   0        0        0     3002 2024-02-22 11:24:29.811391 eprllib-1.1.2/src/eprllib/postprocess/neural_networ_analysis.ipynb
+-rw-r--r--   0        0        0     1636 2024-04-18 12:01:12.679943 eprllib-1.1.2/src/eprllib/preprocess/IDFProperties.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.372239 eprllib-1.1.2/src/eprllib/preprocess/__init__.py
+-rw-r--r--   0        0        0     5797 2024-03-21 15:31:48.398206 eprllib-1.1.2/src/eprllib/preprocess/conventional_experience.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:39:26.603572 eprllib-1.1.2/src/eprllib/tools/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-28 10:22:08.162993 eprllib-1.1.2/src/eprllib/tools/action_transformers.py
+-rw-r--r--   0        0        0     1402 2024-02-24 11:12:25.969964 eprllib-1.1.2/src/eprllib/tools/devices_space_action.py
+-rw-r--r--   0        0        0    19846 2024-03-21 15:31:48.398206 eprllib-1.1.2/src/eprllib/tools/ep_episode_config.py
+-rw-r--r--   0        0        0     9600 2024-05-17 19:23:53.661129 eprllib-1.1.2/src/eprllib/tools/rewards.py
+-rw-r--r--   0        0        0     3180 2024-05-10 08:22:29.542577 eprllib-1.1.2/src/eprllib/tools/utils.py
+-rw-r--r--   0        0        0     7134 2024-03-21 20:29:35.640440 eprllib-1.1.2/src/eprllib/tools/weather_utils.py
+-rw-r--r--   0        0        0     7086 1970-01-01 00:00:00.000000 eprllib-1.1.2/PKG-INFO
```

### Comparing `eprllib-1.1.1/README.md` & `eprllib-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/pyproject.toml` & `eprllib-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "eprllib"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Germán Rodolfo Henderson"},
 ]
 description = "Building control trought DRL."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `eprllib-1.1.1/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw` & `eprllib-1.1.2/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf` & `eprllib-1.1.2/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/agents/conventional.py` & `eprllib-1.1.2/src/eprllib/agents/conventional.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/agents/holon_config.py` & `eprllib-1.1.2/src/eprllib/agents/holon_config.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/agents/user.py` & `eprllib-1.1.2/src/eprllib/agents/user.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_gym_env.py` & `eprllib-1.1.2/src/eprllib/env/multiagent/marl_ep_gym_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         self.act_queue: Optional[Queue] = None
         self.infos_queue: Optional[Queue] = None
         
         # ===CONTROLS=== #
         # variable for the registry of the episode number.
         self.episode = -1
         self.timestep = 0
+        self.terminateds = False
+        self.truncateds = False
         # dict to save the last observation and infos in the environment.
         self.last_obs = {}
         self.last_infos = {}
         for agent in self.env_config['agent_ids']:
             self.last_obs[agent] = []
             self.last_infos[agent] = []
         # list to append, if is needed, the values of PPD and energy
@@ -69,78 +71,81 @@
         seed: Optional[int] = None,
         options: Optional[Dict[str, Any]] = None
     ):
         # Increment the counting of episodes in 1.
         self.episode += 1
         # stablish the timestep counting in zero.
         self.timestep = 0
-
-        # Condition implemented to restart a new epsiode when simulation is completed and 
-        # EnergyPlus Runner is already inicialized.
-        if self.energyplus_runner is not None and self.energyplus_runner.simulation_complete:
-            self.energyplus_runner.stop()
-        
-        # Define the queues for flow control between MDP and EnergyPlus threads in a max size 
-        # of 1 because EnergyPlus timestep will be processed at a time.
-        self.obs_queue = Queue(maxsize=1)
-        self.act_queue = Queue(maxsize=1)
-        self.infos_queue = Queue(maxsize=1)
-        
-        # Define the RunPeriod of execution
-        dynamic_episode_longitude = self.env_config['episode_len_fn']
-        if dynamic_episode_longitude != None:
-            self.env_config['epjson'] = dynamic_episode_longitude(self.env_config)
-        
-        # Start EnergyPlusRunner whith the following configuration.
-        self.energyplus_runner = EnergyPlusRunner(
-            episode=self.episode,
-            env_config=self.env_config,
-            obs_queue=self.obs_queue,
-            act_queue=self.act_queue,
-            infos_queue=self.infos_queue
-        )
+        # Condition of truncated episode
+        if not self.truncateds:
+            # Condition implemented to restart a new epsiode when simulation is completed and 
+            # EnergyPlus Runner is already inicialized.
+            if self.energyplus_runner is not None and self.energyplus_runner.simulation_complete:
+                self.energyplus_runner.stop()
+            # Define the queues for flow control between MDP and EnergyPlus threads in a max size 
+            # of 1 because EnergyPlus timestep will be processed at a time.
+            self.obs_queue = Queue(maxsize=1)
+            self.act_queue = Queue(maxsize=1)
+            self.infos_queue = Queue(maxsize=1)
+            # Define the RunPeriod of execution
+            dynamic_episode_longitude = self.env_config.get('episode_len_fn', None)
+            if dynamic_episode_longitude != None:
+                self.env_config['epjson'] = dynamic_episode_longitude(self.env_config)
+            # Start EnergyPlusRunner whith the following configuration.
+            self.energyplus_runner = EnergyPlusRunner(
+                episode=self.episode,
+                env_config=self.env_config,
+                obs_queue=self.obs_queue,
+                act_queue=self.act_queue,
+                infos_queue=self.infos_queue
+            )
+            # Divide the thread in two in this point.
+            self.energyplus_runner.start()
         
-        # Divide the thread in two in this point.
-        self.energyplus_runner.start()
         # Wait untill an observation and an infos are made, and get the values.
         self.energyplus_runner.obs_event.wait()
         obs = self.obs_queue.get()
         self.energyplus_runner.infos_event.wait()
         infos = self.infos_queue.get()
         
         # Save the observation as a last observation.
         self.last_obs = obs
         self.last_infos = infos
+        
+        self.terminateds = False
+        self.truncateds = False
             
         return obs, infos
 
     def step(self, action):
         # increment the timestep in 1.
         self.timestep += 1
         # ===CONTROLS=== #
         # terminated variable is used to determine the end of a episode. Is stablished as False until the
         # environment present a terminal state.
         terminated = {}
-        terminateds = False
         truncated = {}
-        truncateds = False
-        
+        # Cut the anual simulation into shorter episodes. Default: 7 days
+        cut_episode_len = self.env_config.get('cut_episode_len', 7)
+        cut_episode_len_timesteps = cut_episode_len * 144
+        if self.timestep % cut_episode_len_timesteps == 0:
+            self.truncateds = True
         # timeout is set to 5s to handle the time of calculation of EnergyPlus simulation.
         # timeout value can be increased if EnergyPlus timestep takes longer.
         timeout = self.env_config.get("timeout", 5)
         
         # simulation_complete is likely to happen after last env step()
         # is called, hence leading to waiting on queue for a timeout.
         if self.energyplus_runner.simulation_complete:
             # check for simulation errors.
             if self.energyplus_runner.failed():
                 raise Exception("Faulty episode")
             
             # if the simulation is complete, the episode is ended.
-            terminateds = True
+            self.terminateds = True
             # we use the last observation as a observation for the timestep.
             obs = self.last_obs
             infos = self.last_infos
 
         # if the simulation is not complete, enqueue action (received by EnergyPlus through 
         # dedicated callback) and then wait to get next observation.
         else:
@@ -155,37 +160,37 @@
                 infos = self.infos_queue.get(timeout=timeout)
                 # Upgrade last observation and infos dicts.
                 self.last_obs = obs
                 self.last_infos = infos
 
             except (Full, Empty):
                 # Set the terminated variable into True to finish the episode.
-                terminateds = True
+                self.terminateds = True
                 # We use the last observation as a observation for the timestep.
                 obs = self.last_obs
                 infos = self.last_infos
         
         # Raise an exception if the episode is faulty.
         if self.energyplus_runner.failed():
-            truncateds = True
+            self.terminateds = True
             raise Exception("Faulty episode")
         
         # Calculate the reward in the timestep
         if self.env_config.get('reward_function', False):
             reward_function = self.env_config['reward_function']
         else:
             reward_function = rewards.reward_function_T3_Energy
         reward = reward_function(self, obs, infos)
         
         reward_dict = {}
         for agent in self.env_config['agent_ids']:
             reward_dict[agent] =  reward
         
-        terminated["__all__"] = terminateds
-        truncated["__all__"] = truncateds
+        terminated["__all__"] = self.terminateds
+        truncated["__all__"] = self.truncateds
         
         return obs, reward_dict, terminated, truncated, infos
 
     def close(self):
         if self.energyplus_runner is not None:
             self.energyplus_runner.stop()
```

### Comparing `eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_runner.py` & `eprllib-1.1.2/src/eprllib/env/multiagent/marl_ep_runner.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_gym_env.py` & `eprllib-1.1.2/src/eprllib/env/simpleagent/VENT_ep_gym_env.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_runner.py` & `eprllib-1.1.2/src/eprllib/env/simpleagent/VENT_ep_runner.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/postprocess/marl_init_conventional.py` & `eprllib-1.1.2/src/eprllib/postprocess/marl_init_conventional.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/postprocess/marl_init_evaluation.py` & `eprllib-1.1.2/src/eprllib/postprocess/marl_init_evaluation.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/postprocess/marl_init_noventilation.py` & `eprllib-1.1.2/src/eprllib/postprocess/marl_init_noventilation.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/postprocess/marl_results_evaluation.ipynb` & `eprllib-1.1.2/src/eprllib/postprocess/marl_results_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/postprocess/neural_networ_analysis.ipynb` & `eprllib-1.1.2/src/eprllib/postprocess/neural_networ_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/preprocess/IDFProperties.py` & `eprllib-1.1.2/src/eprllib/preprocess/IDFProperties.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/preprocess/conventional_experience.py` & `eprllib-1.1.2/src/eprllib/preprocess/conventional_experience.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/tools/action_transformers.py` & `eprllib-1.1.2/src/eprllib/tools/action_transformers.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/tools/devices_space_action.py` & `eprllib-1.1.2/src/eprllib/tools/devices_space_action.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/tools/ep_episode_config.py` & `eprllib-1.1.2/src/eprllib/tools/ep_episode_config.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/tools/rewards.py` & `eprllib-1.1.2/src/eprllib/tools/rewards.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any, Dict
-
+from eprllib.env.multiagent.marl_ep_gym_env import EnergyPlusEnv_v0
 
 def reward_function_T3(config: Dict[str, Any], obs: dict, infos: dict) -> float:
     """This function returns the reward calcualted as the absolute value of the cube in the 
     difference between set point temperatur for comfort and the temperature measured in the 
     thermal zone when there are people in the zone but zero when is not.
 
     Args:
@@ -151,8 +151,47 @@
         # InputOutput Reference p.522
         if T_zone > 29.4:
             reward = -150
         elif T_zone < 16.7:
             reward = -150
         else:
             reward = 0.
-    return reward
+    return reward
+
+def normalize_reward_function(self:EnergyPlusEnv_v0, obs: dict, infos: dict) -> float:
+    """This function returns the normalize reward calcualted as the sum of the penalty of the energy 
+    amount of one week divide per the maximun reference energy demand and the average PPD comfort metric
+    divide per the maximal PPF value that can be take (100). Also, each term is divide per the longitude
+    of the episode and multiply for a ponderation factor of beta for the energy and (1-beta) for the comfort.
+    Both terms are negatives, representing a penalti for demand energy and for generate discomfort.
+
+    Args:
+        self (Environment): RLlib environment.
+        obs (dict): Zone Mean Air Temperature for the Thermal Zone in °C.
+        infos (dict): infos dict must to provide the occupancy level and the Zone Mean Temperature.
+
+    Returns:
+        float: reward normalize value
+    """
+    # define the number of timesteps per episode
+    cut_episode_len = self.env_config.get('cut_episode_len', 7)
+    cut_episode_len_timesteps = cut_episode_len * 144
+    # define the beta reward
+    beta_reward = self.env_config.get('beta_reward', 0.5)
+    # get the values of the energy and PPD
+    agent_ids = self.env_config['agent_ids']
+    cooling_meter = infos[agent_ids[0]]['cooling']
+    heating_meter = infos[agent_ids[0]]['heating']
+    ppd = infos[agent_ids[0]]['ppd']
+    self.energy_list.append(cooling_meter+heating_meter)
+    self.ppd_list.append(ppd)
+    
+    if self.timestep % cut_episode_len_timesteps == 0:
+        reward = (-beta_reward*(sum(self.energy_list)/self.env_config['energy_ref']) \
+            -(1-beta_reward)*(sum(self.ppd_list)/100)) \
+                / cut_episode_len_timesteps
+        # emptly the lists
+        self.energy_list = []
+        self.ppd_list = []
+        return reward
+    else:
+        return 0
```

### Comparing `eprllib-1.1.1/src/eprllib/tools/utils.py` & `eprllib-1.1.2/src/eprllib/tools/utils.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/src/eprllib/tools/weather_utils.py` & `eprllib-1.1.2/src/eprllib/tools/weather_utils.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.1/PKG-INFO` & `eprllib-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eprllib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Building control trought DRL.
 Author: Germán Rodolfo Henderson
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

