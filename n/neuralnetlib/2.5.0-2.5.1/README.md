# Comparing `tmp/neuralnetlib-2.5.0.tar.gz` & `tmp/neuralnetlib-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.5.0.tar", last modified: Wed Apr 24 18:04:19 2024, max compression
+gzip compressed data, was "neuralnetlib-2.5.1.tar", last modified: Fri May 17 20:38:08 2024, max compression
```

## Comparing `neuralnetlib-2.5.0.tar` & `neuralnetlib-2.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:04:19.166271 neuralnetlib-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-24 18:04:19.166271 neuralnetlib-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:04:19.166271 neuralnetlib-2.5.0/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    45621 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:04:19.166271 neuralnetlib-2.5.0/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-24 18:04:19.000000 neuralnetlib-2.5.0/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 18:04:19.000000 neuralnetlib-2.5.0/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:04:19.000000 neuralnetlib-2.5.0/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 18:04:19.000000 neuralnetlib-2.5.0/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 18:04:19.000000 neuralnetlib-2.5.0/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 18:04:19.166271 neuralnetlib-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 18:04:10.000000 neuralnetlib-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45924 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/setup.py
```

### Comparing `neuralnetlib-2.5.0/LICENSE` & `neuralnetlib-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/PKG-INFO` & `neuralnetlib-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -77,15 +77,15 @@
 # ... Preprocess x_train, y_train, x_test, y_test if necessary (you can use neuralnetlib.preprocess and neuralnetlib.utils)
 
 # Create a model
 model = Model()
 model.add(Input(10))  # 10 features
 model.add(Dense(8))
 model.add(Dense(1))
-model.add(Activation(Sigmoid()))  # many way to tell the model which Activation Function you'd like, see the next example
+model.add(Activation(Sigmoid()))  # many ways to tell the model which Activation Function you'd like, see the next example
 
 # Compile the model
 model.compile(loss_function='bce', optimizer='sgd')
 
 # Train the model
 model.fit(X_train, y_train, epochs=10, batch_size=32, metrics=[accuracy_score])
 ```
@@ -99,16 +99,15 @@
 from neuralnetlib.metrics import accuracy_score
 
 # ... Preprocess x_train, y_train, x_test, y_test if necessary (you can use neuralnetlib.preprocess and neuralnetlib.utils)
 
 # Create and compile a model
 model = Model()
 model.add(Input(28, 28, 1)) # For example, MNIST images
-model.add(Conv2D(32, kernel_size=3, padding='same'))
-model.add(Activation('relu'))  # activation supports both str...
+model.add(Conv2D(32, kernel_size=3, padding='same'), activation='relu')  # activation supports both str...
 model.add(BatchNormalization())
 model.add(MaxPooling2D(pool_size=2))
 model.add(Dense(64, activation='relu'))
 model.add(Dense(10, activation=Softmax()))  # ... and ActivationFunction objects
 model.compile(loss_function='categorical_crossentropy', optimizer=Adam())
```

### Comparing `neuralnetlib-2.5.0/README.md` & `neuralnetlib-2.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 # ... Preprocess x_train, y_train, x_test, y_test if necessary (you can use neuralnetlib.preprocess and neuralnetlib.utils)
 
 # Create a model
 model = Model()
 model.add(Input(10))  # 10 features
 model.add(Dense(8))
 model.add(Dense(1))
-model.add(Activation(Sigmoid()))  # many way to tell the model which Activation Function you'd like, see the next example
+model.add(Activation(Sigmoid()))  # many ways to tell the model which Activation Function you'd like, see the next example
 
 # Compile the model
 model.compile(loss_function='bce', optimizer='sgd')
 
 # Train the model
 model.fit(X_train, y_train, epochs=10, batch_size=32, metrics=[accuracy_score])
 ```
@@ -78,16 +78,15 @@
 from neuralnetlib.metrics import accuracy_score
 
 # ... Preprocess x_train, y_train, x_test, y_test if necessary (you can use neuralnetlib.preprocess and neuralnetlib.utils)
 
 # Create and compile a model
 model = Model()
 model.add(Input(28, 28, 1)) # For example, MNIST images
-model.add(Conv2D(32, kernel_size=3, padding='same'))
-model.add(Activation('relu'))  # activation supports both str...
+model.add(Conv2D(32, kernel_size=3, padding='same'), activation='relu')  # activation supports both str...
 model.add(BatchNormalization())
 model.add(MaxPooling2D(pool_size=2))
 model.add(Dense(64, activation='relu'))
 model.add(Dense(10, activation=Softmax()))  # ... and ActivationFunction objects
 model.compile(loss_function='categorical_crossentropy', optimizer=Adam())
```

### Comparing `neuralnetlib-2.5.0/neuralnetlib/activations.py` & `neuralnetlib-2.5.1/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib/callbacks.py` & `neuralnetlib-2.5.1/neuralnetlib/callbacks.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib/layers.py` & `neuralnetlib-2.5.1/neuralnetlib/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,26 +28,32 @@
             return Dense.from_config(config)
         elif config['name'] == 'Activation':
             return Activation.from_config(config)
         elif config['name'] == 'Conv2D':
             return Conv2D.from_config(config)
         elif config['name'] == 'MaxPooling2D':
             return MaxPooling2D.from_config(config)
+        elif config['name'] == 'AveragePooling2D':
+            return AveragePooling2D.from_config(config)
         elif config['name'] == 'Flatten':
             return Flatten.from_config(config)
         elif config['name'] == 'Dropout':
             return Dropout.from_config(config)
         elif config['name'] == 'Conv1D':
             return Conv1D.from_config(config)
         elif config['name'] == 'MaxPooling1D':
             return MaxPooling1D.from_config(config)
+        elif config['name'] == 'AveragePooling1D':
+            return AveragePooling1D.from_config(config)
         elif config['name'] == 'Embedding':
             return Embedding.from_config(config)
         elif config['name'] == 'BatchNormalization':
             return BatchNormalization.from_config(config)
+        elif config['name'] == 'Permute':
+            return Permute.from_config(config)
         else:
             raise ValueError(f'Invalid layer name: {config["name"]}')
 
 
 class Input(Layer):
     def __init__(self, input_shape: tuple | int):
         if isinstance(input_shape, int):
```

### Comparing `neuralnetlib-2.5.0/neuralnetlib/losses.py` & `neuralnetlib-2.5.1/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib/metrics.py` & `neuralnetlib-2.5.1/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib/model.py` & `neuralnetlib-2.5.1/neuralnetlib/model.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib/optimizers.py` & `neuralnetlib-2.5.1/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib/preprocessing.py` & `neuralnetlib-2.5.1/neuralnetlib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib/utils.py` & `neuralnetlib-2.5.1/neuralnetlib/utils.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.0/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.5.1/neuralnetlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -77,15 +77,15 @@
 # ... Preprocess x_train, y_train, x_test, y_test if necessary (you can use neuralnetlib.preprocess and neuralnetlib.utils)
 
 # Create a model
 model = Model()
 model.add(Input(10))  # 10 features
 model.add(Dense(8))
 model.add(Dense(1))
-model.add(Activation(Sigmoid()))  # many way to tell the model which Activation Function you'd like, see the next example
+model.add(Activation(Sigmoid()))  # many ways to tell the model which Activation Function you'd like, see the next example
 
 # Compile the model
 model.compile(loss_function='bce', optimizer='sgd')
 
 # Train the model
 model.fit(X_train, y_train, epochs=10, batch_size=32, metrics=[accuracy_score])
 ```
@@ -99,16 +99,15 @@
 from neuralnetlib.metrics import accuracy_score
 
 # ... Preprocess x_train, y_train, x_test, y_test if necessary (you can use neuralnetlib.preprocess and neuralnetlib.utils)
 
 # Create and compile a model
 model = Model()
 model.add(Input(28, 28, 1)) # For example, MNIST images
-model.add(Conv2D(32, kernel_size=3, padding='same'))
-model.add(Activation('relu'))  # activation supports both str...
+model.add(Conv2D(32, kernel_size=3, padding='same'), activation='relu')  # activation supports both str...
 model.add(BatchNormalization())
 model.add(MaxPooling2D(pool_size=2))
 model.add(Dense(64, activation='relu'))
 model.add(Dense(10, activation=Softmax()))  # ... and ActivationFunction objects
 model.compile(loss_function='categorical_crossentropy', optimizer=Adam())
```

### Comparing `neuralnetlib-2.5.0/setup.py` & `neuralnetlib-2.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.5.0',
+    version='2.5.1',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

