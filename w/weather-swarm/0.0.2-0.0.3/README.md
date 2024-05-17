# Comparing `tmp/weather_swarm-0.0.2.tar.gz` & `tmp/weather_swarm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_swarm-0.0.2.tar", max compression
+gzip compressed data, was "weather_swarm-0.0.3.tar", max compression
```

## Comparing `weather_swarm-0.0.2.tar` & `weather_swarm-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     2359 2024-05-10 18:12:01.051225 weather_swarm-0.0.2/README.md
--rw-r--r--   0        0        0     1419 2024-05-17 16:38:43.695093 weather_swarm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       73 2024-05-17 16:38:42.911943 weather_swarm-0.0.2/weather_swarm/__init__.py
--rw-r--r--   0        0        0     7890 2024-05-09 18:51:04.425595 weather_swarm-0.0.2/weather_swarm/baron_tools_schema.py
--rw-r--r--   0        0        0     2529 2024-05-17 16:32:42.620789 weather_swarm-0.0.2/weather_swarm/llama.py
--rw-r--r--   0        0        0    10182 2024-05-09 18:48:47.262272 weather_swarm-0.0.2/weather_swarm/prompts.py
--rw-r--r--   0        0        0    29729 2024-05-09 18:51:04.766079 weather_swarm-0.0.2/weather_swarm/tools.py
--rw-r--r--   0        0        0        0 2024-05-17 16:31:04.902341 weather_swarm-0.0.2/weather_swarm/worker_agents.py
--rw-r--r--   0        0        0     3125 1970-01-01 00:00:00.000000 weather_swarm-0.0.2/setup.py
--rw-r--r--   0        0        0     3392 1970-01-01 00:00:00.000000 weather_swarm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2791 2024-05-17 18:11:53.166879 weather_swarm-0.0.3/README.md
+-rw-r--r--   0        0        0     1419 2024-05-17 18:27:16.890717 weather_swarm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-05-17 16:39:57.227269 weather_swarm-0.0.3/weather_swarm/__init__.py
+-rw-r--r--   0        0        0     2529 2024-05-17 16:32:42.620789 weather_swarm-0.0.3/weather_swarm/llama.py
+-rw-r--r--   0        0        0    10182 2024-05-09 18:48:47.262272 weather_swarm-0.0.3/weather_swarm/prompts.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:02:48.214105 weather_swarm-0.0.3/weather_swarm/tools/__init__.py
+-rw-r--r--   0        0        0     7890 2024-05-09 18:51:04.425595 weather_swarm-0.0.3/weather_swarm/tools/baron_tools_schema.py
+-rw-r--r--   0        0        0     2070 2024-05-17 17:04:26.838814 weather_swarm-0.0.3/weather_swarm/tools/find_lon_lat_tool.py
+-rw-r--r--   0        0        0    29914 2024-05-17 18:05:30.452504 weather_swarm-0.0.3/weather_swarm/tools/tools.py
+-rw-r--r--   0        0        0     5829 2024-05-17 18:18:22.746776 weather_swarm-0.0.3/weather_swarm/worker_agents.py
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 weather_swarm-0.0.3/setup.py
+-rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 weather_swarm-0.0.3/PKG-INFO
```

### Comparing `weather_swarm-0.0.2/README.md` & `weather_swarm-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 
 ## Features
 Baron Weather includes the following key features:
 - **Real-time Weather Data Access**: Instantly fetch and analyze weather conditions using the Baron API.
 - **Autonomous Agents**: A swarm system for handling multiple concurrent API queries efficiently.
 - **Data Visualization**: Tools for visualizing complex meteorological data for easier interpretation.
 
+
 ## Prerequisites
 Before you begin, ensure you have met the following requirements:
-- Python 3.9 or newer
+- Python 3.10 or newer
 - git installed on your machine
 
 ## Installation
 
+There are 2 methods, git cloning which allows you to modify the codebase or pip install for simple usage:
+
+### Pip 
+`pip3 install -U weather-swarm`
+
 ### Cloning the Repository
 To get started with Baron Weather, clone the repository to your local machine using:
 
 ```bash
 git clone https://github.com/baronservices/weatherman_agent.git
 cd weatherman_agent
 ```
@@ -42,31 +48,57 @@
 ## Usage
 To start querying the Baron Weather API using the autonomous agents, run:
 
 ```bash
 python main.py
 ```
 
+
+### Llama3
+
+```python
+from weather_swarm.llama import llama3Hosted
+
+
+# Example usage
+llama3 = llama3Hosted(
+    model="meta-llama/Meta-Llama-3-8B-Instruct",
+    temperature=0.8,
+    max_tokens=1000,
+    system_prompt="You are a helpful assistant.",
+)
+
+completion_generator = llama3.run(
+    "create an essay on how to bake chicken"
+)
+
+print(completion_generator)
+
+```
+
 ## Contributing
 Contributions to Baron Weather are welcome and appreciated. Here's how you can contribute:
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/YourAmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some YourAmazingFeature'`)
 4. Push to the Branch (`git push origin feature/YourAmazingFeature`)
 5. Open a Pull Request
 
-## License
-Baron Weather is released under the MIT License. See the `LICENSE` file for more details.
+
+## Tests
+To run tests run the following:
+
+`pytest`
 
 ## Contact
 Project Maintainer - [Kye Gomez](mailto:kye@swarms.world) - [GitHub Profile](https://github.com/baronservices)
 
-## Acknowledgements
-- Thanks to the Baron API for providing access to their weather data services.
-- Thanks to all contributors who help maintain and enhance this project.
-
 
+## Acknowledgements
 # Todo
 - Make API server functional
 - Make Dockerfile
-- Create a team of specialized agents for different types of weather tools.
+- Create a team of specialized agents for different types of weather tools.
+- Create documentation for llama3,
+- Create dockerfile
+- Create documentation for the agents and how to use them
```

### Comparing `weather_swarm-0.0.2/pyproject.toml` & `weather_swarm-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "weather-swarm"
-version = "0.0.2"
+version = "0.0.3"
 description = "Weather Swarm - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/baronservices/weatherman_agent"
 documentation = "https://github.com/baronservices/weatherman_agent"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/baronservices/weatherman_agent"
```

### Comparing `weather_swarm-0.0.2/weather_swarm/baron_tools_schema.py` & `weather_swarm-0.0.3/weather_swarm/tools/baron_tools_schema.py`

 * *Files identical despite different names*

### Comparing `weather_swarm-0.0.2/weather_swarm/llama.py` & `weather_swarm-0.0.3/weather_swarm/llama.py`

 * *Files identical despite different names*

### Comparing `weather_swarm-0.0.2/weather_swarm/prompts.py` & `weather_swarm-0.0.3/weather_swarm/prompts.py`

 * *Files identical despite different names*

### Comparing `weather_swarm-0.0.2/weather_swarm/tools.py` & `weather_swarm-0.0.3/weather_swarm/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,31 @@
 import hashlib
 import hmac
 import shutil
 import time
 from urllib.request import urlopen
 from urllib.request import Request
 from urllib.error import URLError
-
+import os
 import json
 import codecs
+from dotenv import load_dotenv
+
+load_dotenv()
 
 latin1 = codecs.lookup("latin-1")
 
-host = "http://api.velocityweather.com/v1"
-access_key = "Y5lHXZfgce7P"
-access_key_secret = "rcscpInzyLuweENUjUtFDmqLkK1N0EPeaWQRjy7er1"
+host = os.environ.get(
+    "BARON_API_HOST", "http://api.velocityweather.com/v1"
+)
+access_key = os.environ.get("BARON_ACCESS_KEY", "Y5lHXZfgce7P")
+access_key_secret = os.environ.get(
+    "BARON_ACCESS_KEY_SECRET",
+    "rcscpInzyLuweENUjUtFDmqLkK1N0EPeaWQRjy7er1",
+)
 
 
 def a2w(a):
     return latin1.decode(a)[0]
 
 
 def sig(key, secret):
```

### Comparing `weather_swarm-0.0.2/setup.py` & `weather_swarm-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['weather_swarm']
+['weather_swarm', 'weather_swarm.tools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['json', 'pydantic==2.7.1', 'swarms==4.9.9', 'transformers']
 
 setup_kwargs = {
     'name': 'weather-swarm',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Weather Swarm - Pytorch',
-    'long_description': "# Baron Weather\n\n## Overview\nBaron Weather is a sophisticated toolset designed to enable real-time querying of weather data using the Baron API. It utilizes a swarm of autonomous agents to handle concurrent data requests, optimizing for efficiency and accuracy in weather data retrieval and analysis.\n\n## Features\nBaron Weather includes the following key features:\n- **Real-time Weather Data Access**: Instantly fetch and analyze weather conditions using the Baron API.\n- **Autonomous Agents**: A swarm system for handling multiple concurrent API queries efficiently.\n- **Data Visualization**: Tools for visualizing complex meteorological data for easier interpretation.\n\n## Prerequisites\nBefore you begin, ensure you have met the following requirements:\n- Python 3.9 or newer\n- git installed on your machine\n\n## Installation\n\n### Cloning the Repository\nTo get started with Baron Weather, clone the repository to your local machine using:\n\n```bash\ngit clone https://github.com/baronservices/weatherman_agent.git\ncd weatherman_agent\n```\n\n### Setting Up the Environment\nCreate a Python virtual environment to manage dependencies:\n\n```bash\npython -m venv venv\nsource venv/bin/activate  # On Windows use `venv\\Scripts\\activate`\n```\n\n### Installing Dependencies\nInstall the necessary Python packages via pip:\n\n```bash\npip install -r requirements.txt\n```\n\n## Usage\nTo start querying the Baron Weather API using the autonomous agents, run:\n\n```bash\npython main.py\n```\n\n## Contributing\nContributions to Baron Weather are welcome and appreciated. Here's how you can contribute:\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/YourAmazingFeature`)\n3. Commit your Changes (`git commit -m 'Add some YourAmazingFeature'`)\n4. Push to the Branch (`git push origin feature/YourAmazingFeature`)\n5. Open a Pull Request\n\n## License\nBaron Weather is released under the MIT License. See the `LICENSE` file for more details.\n\n## Contact\nProject Maintainer - [Kye Gomez](mailto:kye@swarms.world) - [GitHub Profile](https://github.com/baronservices)\n\n## Acknowledgements\n- Thanks to the Baron API for providing access to their weather data services.\n- Thanks to all contributors who help maintain and enhance this project.\n\n\n# Todo\n- Make API server functional\n- Make Dockerfile\n- Create a team of specialized agents for different types of weather tools.",
+    'long_description': '# Baron Weather\n\n## Overview\nBaron Weather is a sophisticated toolset designed to enable real-time querying of weather data using the Baron API. It utilizes a swarm of autonomous agents to handle concurrent data requests, optimizing for efficiency and accuracy in weather data retrieval and analysis.\n\n## Features\nBaron Weather includes the following key features:\n- **Real-time Weather Data Access**: Instantly fetch and analyze weather conditions using the Baron API.\n- **Autonomous Agents**: A swarm system for handling multiple concurrent API queries efficiently.\n- **Data Visualization**: Tools for visualizing complex meteorological data for easier interpretation.\n\n\n## Prerequisites\nBefore you begin, ensure you have met the following requirements:\n- Python 3.10 or newer\n- git installed on your machine\n\n## Installation\n\nThere are 2 methods, git cloning which allows you to modify the codebase or pip install for simple usage:\n\n### Pip \n`pip3 install -U weather-swarm`\n\n### Cloning the Repository\nTo get started with Baron Weather, clone the repository to your local machine using:\n\n```bash\ngit clone https://github.com/baronservices/weatherman_agent.git\ncd weatherman_agent\n```\n\n### Setting Up the Environment\nCreate a Python virtual environment to manage dependencies:\n\n```bash\npython -m venv venv\nsource venv/bin/activate  # On Windows use `venv\\Scripts\\activate`\n```\n\n### Installing Dependencies\nInstall the necessary Python packages via pip:\n\n```bash\npip install -r requirements.txt\n```\n\n## Usage\nTo start querying the Baron Weather API using the autonomous agents, run:\n\n```bash\npython main.py\n```\n\n\n### Llama3\n\n```python\nfrom weather_swarm.llama import llama3Hosted\n\n\n# Example usage\nllama3 = llama3Hosted(\n    model="meta-llama/Meta-Llama-3-8B-Instruct",\n    temperature=0.8,\n    max_tokens=1000,\n    system_prompt="You are a helpful assistant.",\n)\n\ncompletion_generator = llama3.run(\n    "create an essay on how to bake chicken"\n)\n\nprint(completion_generator)\n\n```\n\n## Contributing\nContributions to Baron Weather are welcome and appreciated. Here\'s how you can contribute:\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/YourAmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some YourAmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/YourAmazingFeature`)\n5. Open a Pull Request\n\n\n## Tests\nTo run tests run the following:\n\n`pytest`\n\n## Contact\nProject Maintainer - [Kye Gomez](mailto:kye@swarms.world) - [GitHub Profile](https://github.com/baronservices)\n\n\n## Acknowledgements\n# Todo\n- Make API server functional\n- Make Dockerfile\n- Create a team of specialized agents for different types of weather tools.\n- Create documentation for llama3,\n- Create dockerfile\n- Create documentation for the agents and how to use them',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/baronservices/weatherman_agent',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `weather_swarm-0.0.2/PKG-INFO` & `weather_swarm-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-swarm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Weather Swarm - Pytorch
 Home-page: https://github.com/baronservices/weatherman_agent
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
@@ -31,21 +31,27 @@
 
 ## Features
 Baron Weather includes the following key features:
 - **Real-time Weather Data Access**: Instantly fetch and analyze weather conditions using the Baron API.
 - **Autonomous Agents**: A swarm system for handling multiple concurrent API queries efficiently.
 - **Data Visualization**: Tools for visualizing complex meteorological data for easier interpretation.
 
+
 ## Prerequisites
 Before you begin, ensure you have met the following requirements:
-- Python 3.9 or newer
+- Python 3.10 or newer
 - git installed on your machine
 
 ## Installation
 
+There are 2 methods, git cloning which allows you to modify the codebase or pip install for simple usage:
+
+### Pip 
+`pip3 install -U weather-swarm`
+
 ### Cloning the Repository
 To get started with Baron Weather, clone the repository to your local machine using:
 
 ```bash
 git clone https://github.com/baronservices/weatherman_agent.git
 cd weatherman_agent
 ```
@@ -68,31 +74,57 @@
 ## Usage
 To start querying the Baron Weather API using the autonomous agents, run:
 
 ```bash
 python main.py
 ```
 
+
+### Llama3
+
+```python
+from weather_swarm.llama import llama3Hosted
+
+
+# Example usage
+llama3 = llama3Hosted(
+    model="meta-llama/Meta-Llama-3-8B-Instruct",
+    temperature=0.8,
+    max_tokens=1000,
+    system_prompt="You are a helpful assistant.",
+)
+
+completion_generator = llama3.run(
+    "create an essay on how to bake chicken"
+)
+
+print(completion_generator)
+
+```
+
 ## Contributing
 Contributions to Baron Weather are welcome and appreciated. Here's how you can contribute:
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/YourAmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some YourAmazingFeature'`)
 4. Push to the Branch (`git push origin feature/YourAmazingFeature`)
 5. Open a Pull Request
 
-## License
-Baron Weather is released under the MIT License. See the `LICENSE` file for more details.
+
+## Tests
+To run tests run the following:
+
+`pytest`
 
 ## Contact
 Project Maintainer - [Kye Gomez](mailto:kye@swarms.world) - [GitHub Profile](https://github.com/baronservices)
 
-## Acknowledgements
-- Thanks to the Baron API for providing access to their weather data services.
-- Thanks to all contributors who help maintain and enhance this project.
-
 
+## Acknowledgements
 # Todo
 - Make API server functional
 - Make Dockerfile
 - Create a team of specialized agents for different types of weather tools.
+- Create documentation for llama3,
+- Create dockerfile
+- Create documentation for the agents and how to use them
```

