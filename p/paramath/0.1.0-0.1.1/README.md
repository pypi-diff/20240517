# Comparing `tmp/paramath-0.1.0.tar.gz` & `tmp/paramath-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramath-0.1.0.tar", last modified: Thu May 16 04:06:00 2024, max compression
+gzip compressed data, was "paramath-0.1.1.tar", last modified: Fri May 17 03:35:50 2024, max compression
```

## Comparing `paramath-0.1.0.tar` & `paramath-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 04:06:00.961878 paramath-0.1.0/
--rw-rw-rw-   0        0        0      132 2024-05-16 04:06:00.960377 paramath-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-16 02:28:39.000000 paramath-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 04:06:00.944363 paramath-0.1.0/paramath/
--rw-rw-rw-   0        0        0       21 2024-05-16 04:04:57.000000 paramath-0.1.0/paramath/__init__.py
--rw-rw-rw-   0        0        0    19997 2024-05-16 03:57:32.000000 paramath-0.1.0/paramath/main.py
-drwxrwxrwx   0        0        0        0 2024-05-16 04:06:00.959377 paramath-0.1.0/paramath.egg-info/
--rw-rw-rw-   0        0        0      132 2024-05-16 04:06:00.000000 paramath-0.1.0/paramath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-05-16 04:06:00.000000 paramath-0.1.0/paramath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 04:06:00.000000 paramath-0.1.0/paramath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 04:06:00.000000 paramath-0.1.0/paramath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 04:06:00.961878 paramath-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      219 2024-05-16 04:05:34.000000 paramath-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:35:50.254956 paramath-0.1.1/
+-rw-rw-rw-   0        0        0      132 2024-05-17 03:35:50.253453 paramath-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2024-05-17 03:35:35.000000 paramath-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 03:35:50.241944 paramath-0.1.1/paramath/
+-rw-rw-rw-   0        0        0       21 2024-05-16 04:04:57.000000 paramath-0.1.1/paramath/__init__.py
+-rw-rw-rw-   0        0        0    21904 2024-05-17 03:34:18.000000 paramath-0.1.1/paramath/main.py
+-rw-rw-rw-   0        0        0       14 2024-05-17 03:34:40.000000 paramath-0.1.1/paramath/test.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:35:50.252452 paramath-0.1.1/paramath.egg-info/
+-rw-rw-rw-   0        0        0      132 2024-05-17 03:35:50.000000 paramath-0.1.1/paramath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-17 03:35:50.000000 paramath-0.1.1/paramath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 03:35:50.000000 paramath-0.1.1/paramath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-17 03:35:50.000000 paramath-0.1.1/paramath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 03:35:50.254956 paramath-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      242 2024-05-17 03:28:25.000000 paramath-0.1.1/setup.py
```

### Comparing `paramath-0.1.0/paramath/main.py` & `paramath-0.1.1/paramath/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         fibonacci_sequence.append(next_term)
     return fibonacci_sequence
 
 def sqrt(radical: float) -> float:
     if radical > 0:
         return radical ** (1/2)
     elif radical < 0:
-        raise ValueError("Domain Error: parameter must be greater than zero.")
+        raise ValueError("Cannot take square root of negative integer values.")
     
 def nthroot(radical: float, nthconst: float) -> float:
     return radical ** (1/nthconst)
 
 def factorial(constant: int) -> int:
     try:
         factorial = 1
@@ -125,15 +125,17 @@
     Args:
         a (float): Side length a.
         b (float): Side length b.
 
     Returns:
         float: Hypotnuse of the triangle. (returns square root of the sum of both sides.)
     """
-    return sqrt((a ** 2) + (b ** 2))
+    c = (a**2) + (b**2)
+    return round(sqrt(c), 10)
+
 
 def sin(x: float) -> float:
     """Returns the sine of an angle (x).
 
     Args:
         x (float): Angle in degrees.
 
@@ -205,31 +207,34 @@
     Args:
         x (float): Angle in degrees.
 
     Returns:
         float: Returns cosecant of angle. (calculated by 1 / sin(x))
     """
 
-    if x == 180 or x == 360:
+    if x == 180 or x == 360 or x == 0:
         return "Undefined"
     return 1 / sin(x)
 
 def cot(x: float) -> float:
     """Returns the cotangent of an angle (x).
 
     Args:
         x (float): Angle in degrees.
 
     Returns:
         float: Returns cotangent of angle. (calculated by 1 / tan(x))
     """
-    if x == 0:
+    if x == 0 or x == 180 or x == 360:
         return "Undefined"
+    if x == 90 or x == 270:
+        return 0
     return 1 / tan(x)
 
+
 def sinc(x: float) -> float:
     """Returns the sine cardinal of x.
 
     Args:
         x (float): Input.
 
     Returns:
@@ -245,47 +250,86 @@
 
     Returns:
         float: Hyperbolic sine of x.
     """
     return ((e ** x) - (e ** -x)) / 2
 
 def cosh(x: float) -> float: #hyperbolic cosine
-    """Returns the hyperbolic cosine."""
+    """Returns the hyperbolic cosine of x.
+
+    Args:
+        x (float): Input.
+
+    Returns:
+        float: Hyperbolic cosine of x.
+    """    
     return ((e ** x) + (e ** -x)) / 2
 
 def tanh(x: float) -> float: #hyperbolic tangent
-    """Returns the hyperbolic tangent."""
+    """Returns the hyperbolic tangent of x.
+
+    Args:
+        x (float): Input.
+
+    Returns:
+        float: Hyperbolic tangent of x.
+    """    
     return sinh(x) / cosh(x)
 
 def sech(x: float) -> float: #hyperbolic secant
-    """Returns the hyperbolic secant."""
+    """Returns the hyperbolic secant of x.
+
+    Args:
+        x (float): Input.
+
+    Returns:
+        float: Hyperbolic secant of x.
+    """    
     return 1 / cosh(x)
 
 def csch(x: float) -> float: #hyperbolic cosecant
-    """Returns the hyperbolic cosecant."""
+    """Returns the hyperbolic cosecant of x.
+
+    Args:
+        x (float): Input.
+
+    Returns:
+        float: Hyperbolic cosecant of x.
+    """
+    if x == 0:
+        return "Undefined"    
     return 1 / sinh(x)
 
 def coth(x: float) -> float: #hyperbolic cotangent
-    """Returns the hyperbolic cotangent."""
+    """Returns the hyperbolic cotangent of x.
+
+    Args:
+        x (float): Input.
+
+    Returns:
+        float: Hyperbolic cotangent of x.
+    """    
+    if x == 0:
+        return "undefined"
     return 1 / tanh(x)
 
 def polynomial_integral(polynomial: list, upperbound: float, lowerbound: float) -> float:
     """Takes in a list and interprets it as a polynomial. 
        For example, if you have [3, 5, -2] as the polynomial,
        it will be interpreted as 3x^2 + 5x - 2, then integrated
        using the power rule x^n+1/n+1"""
     
-def cis(x: float) -> str:
+def cis(x: float) -> complex:
     """Returns a complex number.
 
     Args:
         x (float): Angle in degrees.
 
     Returns:
-        str: Returns complex number using the cis method otherwise known as e^ix. The return value cannot be used in other methods.
+        str: Returns complex number using the cis method otherwise known as e^ix.
     """
     
     return complex(cos(x), sin(x))
 
 def mod(x: float, y: float) -> float:
     """Modulo
 
@@ -440,19 +484,18 @@
         for i in range(0, length):
             sum += values[i] ** 2
         return sum  
     
 #OBJECTS
 
 class DataSet:
-    """Create a DataSet object with a given list of numbers.
+    """Create a DataSet object using a list[int] or list[float] values to perform operations to find things such as the mean, median, maximum, minimum, count, etc..
 
     Args:
-
-    array: list[int] or list[float]
+        array: list[int] or list[float]
     """
     def __init__(self, array: list):
         self.array = array
         for n in self.array:
             if isinstance(n, int) or isinstance(n, float):
                 pass
             else:
@@ -599,19 +642,19 @@
         
         radical = (self.b ** 2) - (4 * self.a * self.c)
         denominator = 2 * self.a
 
         try: 
             solution_one = ((-1 * self.b) + sqrt(radical)) / denominator
         except TypeError:
-            solution_one = "i"
+            solution_one = "j"
         try:
             solution_two = ((-1 * self.b) - sqrt(radical)) / denominator
         except TypeError:
-            solution_two = "i"
+            solution_two = "j"
         
         return (solution_one, solution_two)
     
     def vertex(self) -> tuple:
         """
         Calculates the vertex by finding the x-cordinate using the x = -b/2a formula, 
         then plugs in x into the equation to find the y-cordinate.
@@ -675,14 +718,19 @@
         """
         Finds the limit (lim) of a given parabola as x approaches h.
         """
 
         return self.a * (h ** 2) + (self.b * h) + (self.c)
 
 class Table():
+    """
+    NEW!
+    Create a table object by providing two lists (list[int] or list[float]) of X and Y values to perform operations such as finding the line of best fit, and more!.
+
+    """
     def __init__(self, L1_X: list, L2_Y: list):
         self.L1_X = L1_X
         self.L2_Y = L2_Y
 
     def ordered_pairs(self) -> list[tuple]: 
         """Returns a list of tuples in which they hold each point of the plot in (x,y) pairs.
 
@@ -700,15 +748,15 @@
             points_list.append((self.L1_X[n], self.L2_Y[n]))
             n+=1
 
         return points_list
 
     def linear_regression(self) -> str:
         """Generates a rough approximation of a linear function that best represents the trend with respect to x and y values. 
-           Form: y=mx+b
+        Form: y=mx+b\n
         Returns:
             str: Rough approximated linear function of the plot.
         """
         index_count = len(self.L2_Y)
         sum_squared_x_values = count(self.L1_X, square=True)
         sum_squared_y_values = count(self.L2_Y, square=True)
         sum_x_y_values = 0
@@ -722,7 +770,29 @@
             sign = ""
         elif constant > 0:
             sign = "+"
         elif constant == 0:
             sign = "+"
 
         return f"y = {round(slope, 2)}x {sign} {round(constant, 2)}"
+
+    def coefficient_of_determination(self) -> float:
+        """Returns the coefficient of determination otherwise known as the R^2 value. \n
+
+        Note: R^2 is a rough approximation that essentially tells you how well the regression fits and predicts values. (The closer R^2 is to 1.0, the better.)
+
+        Returns:
+            float: Coefficient of determination / R^2
+        """
+        index_count = len(self.L2_Y)
+        sum_x = count(self.L1_X)
+        sum_y = count(self.L2_Y)
+        sum_squared_x_values = count(self.L1_X, square=True)
+        sum_squared_y_values = count(self.L2_Y, square=True)
+        sum_x_y_values = 0
+        for i in range(0, len(self.L1_X)):
+            sum_x_y_values += (self.L1_X[i] * self.L2_Y[i])
+
+        r = ((index_count * (sum_x_y_values)) - (sum_x * sum_y))/(sqrt((index_count * sum_squared_x_values) - sum_x ** 2) * sqrt((index_count * sum_squared_y_values) - sum_y ** 2))
+
+        return r**2
+
```

