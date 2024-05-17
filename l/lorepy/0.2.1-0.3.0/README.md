# Comparing `tmp/lorepy-0.2.1.tar.gz` & `tmp/lorepy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lorepy-0.2.1.tar", last modified: Mon May 13 12:41:49 2024, max compression
+gzip compressed data, was "lorepy-0.3.0.tar", last modified: Fri May 17 14:18:01 2024, max compression
```

## Comparing `lorepy-0.2.1.tar` & `lorepy-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 12:41:49.768399 lorepy-0.2.1/
--rw-rw-rw-   0        0        0    21284 2024-02-07 13:25:48.000000 lorepy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     7418 2024-05-13 12:41:49.766384 lorepy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6693 2024-02-07 14:28:01.000000 lorepy-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 12:41:49.768399 lorepy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1057 2024-05-13 08:51:41.000000 lorepy-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:41:49.701384 lorepy-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 12:41:49.730383 lorepy-0.2.1/src/lorepy/
--rw-rw-rw-   0        0        0       30 2024-05-13 08:51:41.000000 lorepy-0.2.1/src/lorepy/__init__.py
--rw-rw-rw-   0        0        0     3038 2024-05-13 08:51:41.000000 lorepy-0.2.1/src/lorepy/lorepy.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:41:49.765384 lorepy-0.2.1/src/lorepy.egg-info/
--rw-rw-rw-   0        0        0     7418 2024-05-13 12:41:49.000000 lorepy-0.2.1/src/lorepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-13 12:41:49.000000 lorepy-0.2.1/src/lorepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 12:41:49.000000 lorepy-0.2.1/src/lorepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-13 12:41:49.000000 lorepy-0.2.1/src/lorepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 12:41:49.000000 lorepy-0.2.1/src/lorepy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 12:41:49.763383 lorepy-0.2.1/tests/
--rw-rw-rw-   0        0        0     3086 2024-05-13 07:49:13.000000 lorepy-0.2.1/tests/test_plot.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.746631 lorepy-0.3.0/
+-rw-rw-rw-   0        0        0    21284 2024-02-07 13:25:48.000000 lorepy-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     8080 2024-05-17 14:18:01.744631 lorepy-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7355 2024-05-17 13:56:54.000000 lorepy-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:18:01.746631 lorepy-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2024-05-17 13:56:54.000000 lorepy-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.661728 lorepy-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.693632 lorepy-0.3.0/src/lorepy/
+-rw-rw-rw-   0        0        0       30 2024-05-13 08:51:41.000000 lorepy-0.3.0/src/lorepy/__init__.py
+-rw-rw-rw-   0        0        0     3453 2024-05-17 13:56:54.000000 lorepy-0.3.0/src/lorepy/lorepy.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.743631 lorepy-0.3.0/src/lorepy.egg-info/
+-rw-rw-rw-   0        0        0     8080 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.741630 lorepy-0.3.0/tests/
+-rw-rw-rw-   0        0        0     3032 2024-05-17 14:04:53.000000 lorepy-0.3.0/tests/test_plot.py
```

### Comparing `lorepy-0.2.1/LICENSE` & `lorepy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lorepy-0.2.1/PKG-INFO` & `lorepy-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: lorepy
-Version: 0.2.1
-Summary: Draw Logistic Regression Plots in Python
-Home-page: https://github.com/raeslab/lorepy/
-Author: Sebastian Proost
-Author-email: sebastian.proost@gmail.com
-License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
-Project-URL: Bug Tracker, https://github.com/raeslab/lorepy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib>=3.4.1
-Requires-Dist: numpy>=1.20.2
-Requires-Dist: pandas>=1.2.4
-Requires-Dist: scikit-learn>=0.24.1
-
 [![Run Pytest](https://github.com/raeslab/lorepy/actions/workflows/autopytest.yml/badge.svg)](https://github.com/raeslab/lorepy/actions/workflows/autopytest.yml) [![Coverage](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/coverage-badge.svg)](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/coverage-badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/686018963.svg)](https://zenodo.org/badge/latestdoi/686018963) [![PyPI version](https://badge.fury.io/py/lorepy.svg)](https://badge.fury.io/py/lorepy) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
 
 # lorepy: Logistic Regression Plots for Python
 
 Logistic Regression plots are used to plot the distribution of a categorical dependent variable in function of a 
 continuous independent variable.
 
@@ -150,14 +131,32 @@
 
 plt.savefig("./docs/img/loreplot_other_clf.png", dpi=150)
 plt.show()
 ```
 
 ![Lorepy with different types of classifiers](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/loreplot_other_clf.png)
 
+
+In case there are confounders, these can be taken into account using the ```confounders``` argument. This requires a
+list of tuples, with the feature and the reference value for that feature to use in plots. E.g. if you wish to deconfound
+for Body Mass Index (BMI) and use a BMI of 25 in plots, set this to [("BMI", 25)].
+
+```python
+loreplot(
+    data=iris_df,
+    x="sepal width (cm)",
+    y="species",
+    confounders=[("petal width (cm)", 1)],
+)
+plt.savefig("./docs/img/loreplot_confounder.png", dpi=150)
+plt.show()
+```
+
+![Loreplot with a confounder](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/loreplot_confounder.png)
+
 ## Development
 
 Additional [documentation for developers](./docs/dev_docs.md) is included with details on running tests, building and deploying to PyPi.
 
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
```

### Comparing `lorepy-0.2.1/setup.py` & `lorepy-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="lorepy",
-    version="0.2.1",
+    version="0.3.0",
     author="Sebastian Proost",
     author_email="sebastian.proost@gmail.com",
     description="Draw Logistic Regression Plots in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raeslab/lorepy/",
     project_urls={
```

### Comparing `lorepy-0.2.1/src/lorepy/lorepy.py` & `lorepy-0.3.0/src/lorepy/lorepy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import pandas as pd
 from sklearn.linear_model import LogisticRegression
 from pandas import DataFrame
 import numpy as np
 import matplotlib.pyplot as plt
 from typing import Optional, Tuple
 
 
-def _get_area_df(X, lg, x_feature, x_range=None) -> DataFrame:
-    values = (
-        np.linspace(X.min(), X.max(), num=200)
-        if x_range is None
-        else np.linspace(x_range[0], x_range[1], num=200)
-    )
-    proba = lg.predict_proba(values.reshape(-1, 1))
+def _get_area_df(lg, x_feature, x_range, deconfound=[]) -> DataFrame:
+    values = np.linspace(x_range[0], x_range[1], num=200)
+
+    predict_df = pd.DataFrame({"values": values})
+
+    for k, v in deconfound:
+        predict_df[k] = v
+
+    proba = lg.predict_proba(predict_df.values)
     proba_df = DataFrame(proba, columns=lg.classes_)
     proba_df[x_feature] = values
     proba_df.set_index(x_feature, inplace=True)
 
     return proba_df
 
 
-def _get_dots_df(X, y, lg, y_feature) -> DataFrame:
+def _get_dots_df(X, y, lg, y_feature, confounders=[]) -> DataFrame:
     output = []
 
     for v, s in zip(X, y):
-        proba = lg.predict_proba([v])
+        proba = lg.predict_proba([v] + [i[1] for i in confounders])
         i = list(lg.classes_).index(s)
         min_value = sum(proba[0][:i])
         max_value = sum(proba[0][: i + 1])
         margin = (max_value - min_value) / 10
         ypos = np.random.uniform(low=min_value + margin, high=max_value - margin)
         output.append({y_feature: s, "x": v[0], "y": ypos})
 
@@ -39,51 +42,56 @@
     x: str,
     y: str,
     add_dots: bool = True,
     x_range: Optional[Tuple[float, float]] = None,
     scatter_kws: dict = dict({}),
     ax=None,
     clf=None,
+    confounders=[],
     **kwargs
 ):
     """
     Code to create a loreplot with a numerical feature on the x-axis and categorical y from a pandas dataset
 
     :param data: Pandas dataframe with data
     :param x: Needs to be a numerical feature
     :param y: Categorical feature
-    :param add_dots: Shows where true samples are in the plot
+    :param add_dots: Shows where true samples are in the plot (cannot be enabled when deconfounding for additional variables)
     :param x_range: Either None (range will be selected automatically) or a tuple with min and max value for the x-axis
     :param scatter_kws: Dictionary with keyword arguments to pass to the scatter function
     :param ax: subplot to draw on, in case lorepy is used in a subplot
     :param clf: provide a different scikit-learn classifier for the function. Should implement the predict_proba() and fit()
+    :param confounders: list of tuples with the feature and reference value e.g. [("BMI", 25)] will confounders BMI and use a reference of 25 for plots
     :param kwargs: Additional arguments to pass to pandas' plot.area function
     """
     if ax is None:
         ax = plt.gca()
-    tmp_df = data[[x, y]].dropna()
-    X_reg = np.array(tmp_df[x]).reshape(-1, 1)
+
+    x_features = [x] + [i[0] for i in confounders]
+
+    tmp_df = data[x_features + [y]].dropna()
+    X_reg = np.array(tmp_df[x_features])
     y_reg = np.array(tmp_df[y])
 
+    if x_range is None:
+        x_range = (X_reg[:, 0].min(), X_reg[:, 0].max())
+
     lg = LogisticRegression(multi_class="multinomial") if clf is None else clf
     lg.fit(X_reg, y_reg)
 
     if "linestyle" not in kwargs.keys():
         kwargs["linestyle"] = "None"
 
-    area_df = _get_area_df(X_reg, lg, x, x_range=x_range)
+    area_df = _get_area_df(lg, x, x_range, deconfound=confounders)
     area_df.plot.area(ax=ax, **kwargs)
 
-    if add_dots:
+    if add_dots and len(confounders) == 0:
         dot_df = _get_dots_df(X_reg, y_reg, lg, y)
         if "color" not in scatter_kws.keys():
             scatter_kws["color"] = "w"
         if "alpha" not in scatter_kws.keys():
             scatter_kws["alpha"] = 0.3
         ax.scatter(dot_df["x"], dot_df["y"], **scatter_kws)
 
-    if x_range is None:
-        ax.set_xlim(X_reg.min(), X_reg.max())
-    else:
-        ax.set_xlim(*x_range)
+    ax.set_xlim(*x_range)
 
     ax.set_ylim(0, 1)
```

### Comparing `lorepy-0.2.1/src/lorepy.egg-info/PKG-INFO` & `lorepy-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lorepy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Draw Logistic Regression Plots in Python
 Home-page: https://github.com/raeslab/lorepy/
 Author: Sebastian Proost
 Author-email: sebastian.proost@gmail.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: Bug Tracker, https://github.com/raeslab/lorepy/issues
 Classifier: Programming Language :: Python :: 3
@@ -150,14 +150,32 @@
 
 plt.savefig("./docs/img/loreplot_other_clf.png", dpi=150)
 plt.show()
 ```
 
 ![Lorepy with different types of classifiers](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/loreplot_other_clf.png)
 
+
+In case there are confounders, these can be taken into account using the ```confounders``` argument. This requires a
+list of tuples, with the feature and the reference value for that feature to use in plots. E.g. if you wish to deconfound
+for Body Mass Index (BMI) and use a BMI of 25 in plots, set this to [("BMI", 25)].
+
+```python
+loreplot(
+    data=iris_df,
+    x="sepal width (cm)",
+    y="species",
+    confounders=[("petal width (cm)", 1)],
+)
+plt.savefig("./docs/img/loreplot_confounder.png", dpi=150)
+plt.show()
+```
+
+![Loreplot with a confounder](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/loreplot_confounder.png)
+
 ## Development
 
 Additional [documentation for developers](./docs/dev_docs.md) is included with details on running tests, building and deploying to PyPi.
 
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
```

### Comparing `lorepy-0.2.1/tests/test_plot.py` & `lorepy-0.3.0/tests/test_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,43 @@
 import matplotlib.pyplot as plt
 
 from lorepy.lorepy import loreplot, _get_dots_df, _get_area_df
 
 # Generate a sample dataset for testing
 X = np.concatenate([np.random.randint(0, 10, 50), np.random.randint(2, 12, 50)])
 y = [0] * 50 + [1] * 50
+z = X
 
-df = pd.DataFrame({"x": X, "y": y})
+df = pd.DataFrame({"x": X, "y": y, "z": z})
 
 
 # Test case for loreplot with default parameters
 def test_loreplot_default():
     loreplot(df, "x", "y")  ## first test without specifying the axis
 
     fig, ax = plt.subplots()
     loreplot(df, "x", "y", ax=ax)
     assert ax.get_title() == ""
     assert ax.get_xlabel() == "x"
     assert ax.get_ylabel() == ""
 
 
+# Test case for loreplot with confounder
+def test_loreplot_default():
+    loreplot(
+        df, "x", "y", confounders=[("z", 1)]
+    )  ## first test without specifying the axis
+
+    fig, ax = plt.subplots()
+    loreplot(df, "x", "y", ax=ax)
+    assert ax.get_title() == ""
+    assert ax.get_xlabel() == "x"
+    assert ax.get_ylabel() == ""
+
+
 # Test case for loreplot with custom clf
 def test_loreplot_custom_clf():
     svc = SVC(probability=True)
     loreplot(df, "x", "y", clf=svc)
 
     fig, ax = plt.subplots()
     loreplot(df, "x", "y", ax=ax)
@@ -79,28 +93,15 @@
     assert "y" in dots_df.columns
     assert "y_feature" not in dots_df.columns
     assert len(dots_df) == len(X_reg)
 
 
 # Test case for _get_area_df
 def test_get_area_df():
-    area_df = _get_area_df(X_reg, lg, "x")
+    area_df = _get_area_df(lg, "x", (X_reg.min(), X_reg.max()))
     assert isinstance(area_df, DataFrame)
     assert "x" not in area_df.columns
     assert 0 in area_df.columns
     assert 1 in area_df.columns
     assert len(area_df) == 200
     assert area_df.index[0] == X_reg.min()
     assert area_df.index[-1] == X_reg.max()
-
-
-# Test case for _get_area_df with custom x_range
-def test_get_area_df_custom_range():
-    x_range = (2.0, 4.0)
-    area_df = _get_area_df(X_reg, lg, "x", x_range=x_range)
-    assert isinstance(area_df, DataFrame)
-    assert "x" not in area_df.columns
-    assert 0 in area_df.columns
-    assert 1 in area_df.columns
-    assert len(area_df) == 200
-    assert area_df.index[0] == x_range[0]
-    assert area_df.index[-1] == x_range[1]
```

