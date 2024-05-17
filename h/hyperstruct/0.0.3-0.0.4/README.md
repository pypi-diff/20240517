# Comparing `tmp/hyperstruct-0.0.3.tar.gz` & `tmp/hyperstruct-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperstruct-0.0.3.tar", max compression
+gzip compressed data, was "hyperstruct-0.0.4.tar", max compression
```

## Comparing `hyperstruct-0.0.3.tar` & `hyperstruct-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2024-05-14 02:51:22.994386 hyperstruct-0.0.3/LICENSE
--rw-r--r--   0        0        0     3330 2024-05-14 02:51:22.994386 hyperstruct-0.0.3/README.md
--rw-r--r--   0        0        0     1830 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1425 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/src/hyperstruct/__init__.py
--rw-r--r--   0        0        0      292 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/src/hyperstruct/__main__.py
--rw-r--r--   0        0        0    12738 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/src/hyperstruct/fuselage.py
--rw-r--r--   0        0        0        0 2024-05-14 02:51:22.994386 hyperstruct-0.0.3/src/hyperstruct/py.typed
--rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 hyperstruct-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-17 02:13:14.146999 hyperstruct-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3330 2024-05-17 02:13:14.146999 hyperstruct-0.0.4/README.md
+-rw-r--r--   0        0        0     1830 2024-05-17 02:13:27.250902 hyperstruct-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1568 2024-05-17 02:13:27.250902 hyperstruct-0.0.4/src/hyperstruct/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-17 02:13:14.146999 hyperstruct-0.0.4/src/hyperstruct/__main__.py
+-rw-r--r--   0        0        0    17510 2024-05-17 02:13:27.250902 hyperstruct-0.0.4/src/hyperstruct/fuselage.py
+-rw-r--r--   0        0        0        0 2024-05-17 02:13:14.146999 hyperstruct-0.0.4/src/hyperstruct/py.typed
+-rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 hyperstruct-0.0.4/PKG-INFO
```

### Comparing `hyperstruct-0.0.3/LICENSE` & `hyperstruct-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperstruct-0.0.3/README.md` & `hyperstruct-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperstruct-0.0.3/pyproject.toml` & `hyperstruct-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperstruct"
-version = "0.0.3"
+version = "0.0.4"
 description = "Hyperstruct"
 authors = ["Benjamin Crews <aceF22@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/czarified/hyperstruct"
 repository = "https://github.com/czarified/hyperstruct"
 documentation = "https://hyperstruct.readthedocs.io"
```

### Comparing `hyperstruct-0.0.3/src/hyperstruct/__init__.py` & `hyperstruct-0.0.4/src/hyperstruct/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """Hyperstruct."""
 
 from dataclasses import dataclass
+from importlib.metadata import version
+
+
+__version__ = version("hyperstruct")
 
 
 @dataclass
 class Material:
     """The HyperStruct material model.
 
     The material object contains the basic material allowables.
@@ -50,14 +54,17 @@
     """The basic foundation for sizing.
 
     An Aircraft is composed of different Assemblies, which contain various Components.
     Components have several base methods and attributes that enable sizing and
     weights estimation.
     """
 
+    material: Material
+    """material the cover is made of."""
+
     def synthesis(self) -> None:
         """The sizing method.
 
         The sizing method collects all sizing routines and executes them
         in the order of the `routines` list.
         """
         # This doesn't work. It's just a placeholder.
```

### Comparing `hyperstruct-0.0.3/src/hyperstruct/fuselage.py` & `hyperstruct-0.0.4/src/hyperstruct/fuselage.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,32 +8,28 @@
 from dataclasses import dataclass
 from typing import Any
 from typing import Tuple
 
 import numpy as np
 
 from hyperstruct import Component
-from hyperstruct import Material
 
 
 @dataclass
 class Cover(Component):
     """Fuselage Cover component.
 
     The Fuselage Cover components (aka Skins) are evalutated
     for sufficient thickness to satisfy strength, flutter,
     acoustic fatigue, and minimum thickness. Should the shell section
     be pressurized or contain fuel, they are evaluated for pressure requirements.
     The cover sizing procedure starts at minimum thicknesses and proceeds
     through a systematic check for the different criteria.
     """
 
-    material: Material
-    """material the cover is made of."""
-
     milled: bool
     """if panel is to be milled for different field vs land thicknesses."""
 
     L: float
     """frame spacing."""
 
     D: float
@@ -126,14 +122,20 @@
     def field_thickness_postbuckled(self, alpha: float = 45) -> float:
         """Field thickness based on critical shear flow.
 
         Evaluate the min thickness required to satisfy post-buckled strength.
         Postbuckled strength assumes sizing covers with diagonal tension. The
         diagonal tension angle is unknown because intermediate frame and
         stringer sizing is not known. An initial estimate of 45 degrees is used.
+
+        Args:
+            alpha: Diagonal tension angle (assumed 45 degrees)
+
+        Returns:
+            A float of field thickness.
         """
         F_scr = (
             self.k_s
             * np.pi**2
             * self.material.E
             / (12 * (1 - self.material.nu**2))
             * (self.t_c / min(self.D, self.L)) ** 2
@@ -191,15 +193,19 @@
         Cabin pressurization is a cyclic occurrence that subjects the cover
         to possible fatigue failure. The maximum allowable stress to prevent
         fatigue is represented as a fraction of the material ultimate
         tensile strength. The pre=programmed allowable represents a change
         from zero to peak pressure 20,000 times during the vehicle's useful
         life, with a stress concentration factor of 4.0.
 
-        Returns: (t_l, t_c)
+        Args:
+            F_allow: Allowable stress (25% yield, if not provided)
+
+        Returns:
+            A tuple of (Land thickness, Field thickness).
         """
         b = min(self.D, self.L)
         if not F_allow:
             F_allow = self.material.F_ty / 4.0
 
         # TODO: Lookup the vehicle-level load factors for the CG
         Nz_plus = 6
@@ -251,30 +257,40 @@
         is a function of dynamic pressure, Mach number, geometry, and material.
         Curve-fits for each variable are utilized, with a baseline thickness
         value returned.
 
         To find the final required thickness, this method must be looped
         over for all Mach and altitudes corresponding to the flight
         envelope conditions of the aircraft.
+
+        Args:
+            mach: Mach Number
+            altitude: Altitude (in thousands of feet)
+
+        Returns:
+            A float of Field Thickness.
         """
         # Dynamic pressures based on standard day atmosphere.
         # Dynamic Pressure, q, in [psf]
         # Altitudes must be measured in [ft]
-        if altitude <= 20000:
+        if altitude <= 20:
             q = mach**2 * (1479.757 - 52.187 * altitude + 0.619868 * altitude**2)
-        elif 20000 < altitude <= 70000:
+        elif 20 < altitude <= 70:
             q = mach**2 * (
                 1465.175
                 - 50.76695 * altitude
                 + 0.6434412 * altitude**2
                 - 0.002907194 * altitude**3
             )
-        elif altitude > 70000:
+        elif altitude > 70:
             q = mach**2 * (199.659 / altitude) ** 4
 
+        # Dynamic pressure is in [psf] convert to [psi]
+        q = q / 144
+
         # Calculate the Mach Number Effect
         # The Mach Number Effect, FM, is a 3 piece function from SWEEP.
         # This function is more conservative than the AFRL baseline curve,
         # but less conservative than the NACA curve. ADA002867, pg. 100.
         if 1.0 <= mach < 1.4:
             FM = 0.4851674 + 1.66456 * (mach - 1) ** 3
         elif 1.4 <= mach <= 2.0:
@@ -316,15 +332,16 @@
                 conservative when aspect ratios approach 1.
 
         The sound pressure level used is based on a material property. This value
         provides the fatigue life of 10^9 cycles for the material. The overall
         decibel level is then increased by 30, which represents jet noise instead
         of a purely random spectrum.
 
-        Returns: (t_l, t_c)
+        Returns:
+            A tuple of Land thickness, Field thickness (t_l, t_c).
         """
         # Random distribution acoustic level, that provides a material fatigue
         # life of 10^9 cycles.
         db_r = self.material.db_r
         db_oa = db_r + 30
         P = 2.9e-9 * 10 ** (db_oa / 20)
         # Note: K_c is directly hardcoded to 2.62, per Fig. 20 of ADA002867
@@ -339,7 +356,135 @@
         x_l = self.D**2 / (t_l * self.RC)
         x_c = self.D**2 / (t_c * self.RC)
         # Ratio of curved panel thickness over flat panel
         f_l = 1.0794 + 0.000143 * x_l - 0.076475 * (1 / x_l) - 0.29969 * np.log(x_l)
         f_c = 1.0794 + 0.000143 * x_c - 0.076475 * (1 / x_c) - 0.29969 * np.log(x_c)
 
         return (float(f_l * t_l), float(f_c * t_c))
+
+
+@dataclass
+class MinorFrame(Component):
+    """Fuselage Minor Frame Component.
+
+    Minor Frames form part of the basic structural grid work that resists
+    vehicle shear and bending loads. As opposed to Major Frames, Minor
+    Frames do not redistribute concentrated loads. Minor Frames are sized
+    for general shell stability, acoustic fatigue, and forced crippling
+    due to postbuckled cover (skin) design.
+
+    Minor Frames have an assumed construction, shown here? The geometry
+    variables, frame depth (c), and cap flange width (b), are user input
+    parameters. Thickness is the only parameter determined by sizing.
+
+    For simplicity, the flanges are assumed to have a thickness twice
+    that of the web.
+    """
+
+    c: float
+    """frame depth."""
+
+    b: float
+    """cap flange width."""
+
+    t_r: float = 0.0
+    """cap flange thickness."""
+
+    @property
+    def t_w(self) -> float:
+        """Web thickness."""
+        return self.t_r / 2
+
+    @property
+    def area(self) -> float:
+        """Cross-sectional area."""
+        return 4 * self.b * self.t_r + self.c * self.t_w
+
+    @property
+    def i_xx(self) -> float:
+        """Second moment of area (bending moment of inertia).
+
+        Assumes the simplified case that t_r = 2*t_w.
+        """
+        return self.t_r * (
+            self.b * self.c**2 + 2 * self.b**3 / 3 - self.b**2 * self.c + self.c**3 / 24
+        )
+
+    @property
+    def rho(self) -> float:
+        """Radius of gyration."""
+        return float(
+            (
+                (
+                    self.b * self.c**2
+                    + 2 * self.b**3 / 3
+                    - self.b**2 * self.c
+                    + self.c**3 / 24
+                )
+                / (4 * self.b + self.c / 2)
+            )
+            ** 0.5
+        )
+
+    def general_stability(self, L: float, D: float, M: float) -> float:
+        """Thickness to avoid general instability.
+
+        The thickness that provides frame stiffness sufficient to prevent
+        general instability failure is solved via the Shanley equation.
+
+        Args:
+            L: Frame Spacing
+            D: Fuselage Diameter
+            M: Bending moment at the cut
+
+        Returns:
+            A float of Flange thickness.
+        """
+        c_f = 1 / 16000
+        numerator = c_f * M * D**2
+        denominator = (
+            self.material.E_c
+            * L
+            * (self.b * self.c**2 + 2 * self.b**3 * self.c / 3 + self.c**3 / 24)
+        )
+
+        return float(numerator / denominator)
+
+    def acoustic_fatigue(self, b: float) -> float:
+        """Thickness requirements based on acoustic fatigue.
+
+        Assumptions are:
+            1.) The overall pressure level from jet engine noise is approximately
+                30db higher than the random spectrum pressure level.
+            2.) The accuracy of noise intensity prediction is on the order of +/-3db.
+            3.) Beam theory is sufficient for modelign the shell elements.
+            4.) The design to repetitive pressure intensity from jet engine noise
+                can be correlated tot he material endurance limit. Polished specimen
+                s-n data, K_t=1, is a sufficiently representative strength index.
+            5.) The method is based on a limited amount of testing.
+            6.) The method does not consider panel aspect ratio, and is, therefore,
+                conservative when aspect ratios approach 1.
+
+        The sound pressure level used is based on a material property. This value
+        provides the fatigue life of 10^9 cycles for the material. The overall
+        decibel level is then increased by 30, which represents jet noise instead
+        of a purely random spectrum.
+
+        Args:
+            b: Support spacing (frame spacing)
+
+        Returns:
+            A float of Flange thickness.
+        """
+        # Random distribution acoustic level, that provides a material fatigue
+        # life of 10^9 cycles.
+        db_r = self.material.db_r
+        db_oa = db_r + 30
+        P = 2.9e-9 * 10 ** (db_oa / 20)
+        # Note: K_c is directly hardcoded to 7.025, per Fig. 20 of ADA002867
+        t_r = 7.025 * b**0.5 * P**2 / self.material.F_en
+
+        return float(t_r)
+
+    def forced_crippling(self) -> float:
+        """Thickness from force crippling."""
+        return 0.0
```

### Comparing `hyperstruct-0.0.3/PKG-INFO` & `hyperstruct-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperstruct
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hyperstruct
 Home-page: https://github.com/czarified/hyperstruct
 License: MIT
 Author: Benjamin Crews
 Author-email: aceF22@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 1 - Planning
```

