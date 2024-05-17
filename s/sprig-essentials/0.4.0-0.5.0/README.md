# Comparing `tmp/sprig_essentials-0.4.0.tar.gz` & `tmp/sprig_essentials-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprig_essentials-0.4.0.tar", last modified: Sun Dec 17 09:19:54 2023, max compression
+gzip compressed data, was "sprig_essentials-0.5.0.tar", last modified: Fri May 17 11:02:14 2024, max compression
```

## Comparing `sprig_essentials-0.4.0.tar` & `sprig_essentials-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 09:19:54.415788 sprig_essentials-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16294 2023-12-17 09:19:54.415788 sprig_essentials-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15700 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 09:19:54.415788 sprig_essentials-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 09:19:54.411788 sprig_essentials-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 09:19:54.415788 sprig_essentials-0.4.0/src/sprig_essentials/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/src/sprig_essentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/src/sprig_essentials/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/src/sprig_essentials/buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/src/sprig_essentials/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 09:19:54.415788 sprig_essentials-0.4.0/src/sprig_essentials/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/src/sprig_essentials/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/src/sprig_essentials/graphics/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-17 09:19:46.000000 sprig_essentials-0.4.0/src/sprig_essentials/graphics/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 09:19:54.415788 sprig_essentials-0.4.0/src/sprig_essentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16294 2023-12-17 09:19:54.000000 sprig_essentials-0.4.0/src/sprig_essentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-17 09:19:54.000000 sprig_essentials-0.4.0/src/sprig_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 09:19:54.000000 sprig_essentials-0.4.0/src/sprig_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-17 09:19:54.000000 sprig_essentials-0.4.0/src/sprig_essentials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:14.790989 sprig_essentials-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-05-17 11:02:14.790989 sprig_essentials-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:02:14.790989 sprig_essentials-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:14.786989 sprig_essentials-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:14.786989 sprig_essentials-0.5.0/src/sprig_essentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:14.786989 sprig_essentials-0.5.0/src/sprig_essentials/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/graphics/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/graphics/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/graphics/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:14.790989 sprig_essentials-0.5.0/src/sprig_essentials/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/io/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/io/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/io/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-17 11:02:09.000000 sprig_essentials-0.5.0/src/sprig_essentials/io/led.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:02:14.790989 sprig_essentials-0.5.0/src/sprig_essentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-05-17 11:02:14.000000 sprig_essentials-0.5.0/src/sprig_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-17 11:02:14.000000 sprig_essentials-0.5.0/src/sprig_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:02:14.000000 sprig_essentials-0.5.0/src/sprig_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:02:14.000000 sprig_essentials-0.5.0/src/sprig_essentials.egg-info/top_level.txt
```

### Comparing `sprig_essentials-0.4.0/LICENSE` & `sprig_essentials-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sprig_essentials-0.4.0/PKG-INFO` & `sprig_essentials-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,103 @@
 Metadata-Version: 2.1
 Name: sprig_essentials
-Version: 0.4.0
-Summary: Useful functions for creating games and apps with Sprig
+Version: 0.5.0
+Summary: Simplifying the process of creating games and apps for the Sprig.
 Author-email: Sooraj Sannabhadti <developer.soorajs@gmail.com>
 Project-URL: Homepage, https://github.com/WhenLifeHandsYouLemons/sprig_essentials
 Project-URL: Bug Tracker, https://github.com/WhenLifeHandsYouLemons/sprig_essentials/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sprig-essentials 0.4.0
+# sprig-essentials
 
-Useful functions to simplify the process of creating games and apps with Sprig when using [CircuitPython](https://circuitpython.org/).
+Useful functions to simplify the process of creating games and apps with Sprig when using [*CircuitPython*](https://circuitpython.org/).
 
-**This package can currently only be used when developing using a device with internet. The package is not available for download on the Raspberry Pi Pico itself yet.**
+**This package can currently only be used when developing using a device with internet. The package is not available for download on the *Raspberry Pi Pico* itself yet.**
 
 [![Upload Python Package](https://github.com/WhenLifeHandsYouLemons/sprig_essentials/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WhenLifeHandsYouLemons/sprig_essentials/actions/workflows/python-publish.yml)
 
 ---
 
 ## Installation
 
-To install the correct CircuitPython firmware and libraries for the Raspberry Pi Pico, follow these steps:
+### Basic Installation
 
-1. Download the .UF2 from the CircuitPython website [here](https://circuitpython.org/board/raspberry_pi_pico/).
-2. Press and hold the white button on the RPi Pico, then plug it into your computer while pressing the button. It should appear as a USB drive.
-3. Drag the downloaded .UF2 file into the USB drive. The RPi Pico should automatically reboot and CircuitPython should be installed.
+To install the correct *CircuitPython* firmware and libraries for the *Raspberry Pi Pico*, follow these steps:
+
+1. Download the .UF2 from the *CircuitPython* website [here](https://circuitpython.org/board/raspberry_pi_pico/).
+2. Press and hold the white button on the *RPi Pico*, then plug it into your computer while pressing the button. It should appear as a USB drive.
+3. Drag the downloaded `.UF2` file into the USB drive. The *RPi Pico* should automatically reboot and *CircuitPython* should be installed.
 4. In the USB drive, create a new folder called `lib` if it doesn't already exist.
 5. Download the necessary libraries from [this sub-folder](https://github.com/WhenLifeHandsYouLemons/sprig-essentials/tree/cbcddaf0884fbc39bbaa791aa085280db103ce35/libraries) and place them in the `lib` folder.
+6. At this point, you can now start using the `sprig_essentials` package on the *Raspberry Pi Pico*.
 
-To install `sprig_essentials` and use it on your Windows machine when developing for the Raspberry Pi Pico:
+To install `sprig_essentials` and use it on your Windows machine when developing for the *Raspberry Pi Pico*, you need to do the following:
 
-```txt
+```shell
 pip install sprig-essentials
 ```
 
-This package is intended to run on the `Raspberry Pi Pico H`.
+Then, to use it in a program you can import the entire package:
+
+```py
+import sprig_essentials as se
+```
+
+Or import specific modules (for example, the [display](#display-module) module):
+
+```py
+from sprig_essentials.io import display
+```
+
+### Manual Installation
+
+This package can be installed manually by downloading and compiling the source code. To do this, follow these steps:
+
+1. Clone the repository and nvaigate to it:
 
-This package assumes you've installed `CircuitPython` and are using the `ST7735` display.
+    ```shell
+    git clone https://github.com/WhenLifeHandsYouLemons/sprig-essentials.git
+    cd sprig-essentials
+    ```
+
+2. Compile the package:
+
+    ```shell
+    python convert_to_mpy.py
+    ```
+
+    or
+
+    ```shell
+    python3 convert_to_mpy.py
+    ```
+
+3. Copy the files inside the `output` folder to your Raspberry Pi Pico's `lib` folder.
+4. You can now start using the `sprig_essentials` package on the Raspberry Pi Pico.
+
+**This package is intended to run on the `Raspberry Pi Pico H`.**
+
+**This package assumes you've installed `CircuitPython` and are using the `ST7735` display.**
 
 ---
 
 ## Wiring Diagram
 
 The wiring diagram that this package assumes is intended for anyone using a Sprig, however, you can also wire this manually and achieve the same effect.
 
-![Image showing the pin connections from the Raspberry Pi Pico H to the various peripherals on the Sprig's board](https://camo.githubusercontent.com/d9b4afd8b99cc6befd3e04bdb8231c9fd134333ebd6a17166ca391429221ff05/68747470733a2f2f70617065722d6174746163686d656e74732e64726f70626f782e636f6d2f735f303531314241344231393135393837353345434243343935363743303632334234453646313535314241453338333243443842384232454441463236464142365f313636323537323037313339375f53637265656e2b53686f742b323032322d30392d30372b61742b312e33342e32312b504d2e706e67 "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
+![Image showing the PCB wires from the Raspberry Pi Pico H to the various peripherals on the Sprig's board](documentation/images/sprig_pcb_wiring_diagram.png "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
 
-Here's a clearer electrical wiring diagram:
+Here's a clearer pin connection diagram for GPIO pin numbers:
 
-![Image showing the electric wiring diagram for the Raspberry Pi Pico H and the Sprig](https://camo.githubusercontent.com/f0ff037c476cfa07603e9c8ec77394ee53f18701c89f509a2852b623583d1807/68747470733a2f2f70617065722d6174746163686d656e74732e64726f70626f782e636f6d2f735f303531314241344231393135393837353345434243343935363743303632334234453646313535314241453338333243443842384232454441463236464142365f313636323537313738303737365f53637265656e2b53686f742b323032322d30392d30372b61742b312e31322e35372b504d2e706e67 "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
+![Image showing the pin connection diagram for the Raspberry Pi Pico H and the Sprig](documentation/images/sprig_peripheral_pin_connection_image.png "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
 
 ---
 
 ## Documentation
 
 ### Core module
 
@@ -82,22 +123,21 @@
 
 ```py
 hex_value = core.convertRGBToHex([255, 255, 255])
 ```
 
 ---
 
-
 ### `display` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import display
+from sprig_essentials.io import display
 
 display_device = display.Display()
 ```
 
 - **Parameters:**
   - `backlight_pin`: Pin number for the backlight (default: `board.GP17`)
   - `clock_pin`: Pin number for the clock (default: `board.GP18`)
@@ -338,15 +378,15 @@
 
 ### `audio` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import audio
+from sprig_essentials.io import audio
 
 audio_device = audio.Audio()
 ```
 
 - **Parameters:**
   - `bit_clock_pin`: Pin number for the bit clock (default: `board.GP10`)
   - `word_select_pin`: Pin number for word select (default: `board.GP11`)
@@ -552,15 +592,15 @@
 
 ### `buttons` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import button
+from sprig_essentials.io import button
 
 # Initialize a button using a pin number
 button_1 = button.Button(board.GP5)
 
 # Or if using a Sprig
 buttons = button.Button(quick_start=True)
 ```
@@ -605,29 +645,35 @@
 quick_buttons = button.quickStartButtons()
 ```
 
 ---
 
 #### `getPressed`
 
-Gets the current state of the button.
+Gets the current state of the button. This automatically updates the current and previous state of the button.
 
-- **Parameters:**
-  - `button`: Optional digital input object; if provided, gets the state of this specific button
-- **Returns:** If a specific button is provided, returns `True` if pressed, `False` if released. If no button is specified, returns a list of states for all buttons.
+- **Parameters:** `None`
+- **Returns:**
+  - Returns `True` if pressed
+  - Returns `False` if released
+  - If no button is specified, returns a list of states for all buttons.
 
 Example:
 
 ```py
 button = button.Button(board.GP5)
-state = button.getPressed()    # Get state of specific button
+state = button.getPressed()
 
-# Or if using Sprig's 8 buttons
+# Or if using the Sprig's 8 buttons
 buttons = button.Button()
 states = buttons.getPressed()    # Get state of all buttons
+
+# Getting the state of a specific button
+w_button = buttons[0]
+w_state = buttons.getPressed(w_button)
 ```
 
 ---
 
 #### `updateButton`
 
 Updates the current and previous state of the button.
@@ -646,29 +692,29 @@
 buttons.updateButton()    # Update state of all buttons
 ```
 
 ---
 
 #### `getButtonStateChange`
 
-Returns the state change of the button.
+Returns the state change of the button. This automatically updates the current and previous state of the button.
 
 - **Parameters:** `None`
 - **Returns:**:
   - `"pressed"` if state changes from `False` to `True`
   - `"released"` if state changes from `True` to `False`
-  - `"no change"` if state did not change
+  - `"no change"` if state did not change.
 
 Example:
 
 ```py
 button = button.Button(board.GP5)
-state_change = button.getButtonStateChange()    # Get state change of specific button
+state_change = button.getButtonStateChange()
 
-# Or if using Sprig's 8 buttons
+# Or if using the Sprig's 8 buttons
 buttons = button.Button()
 state_changes = buttons.getButtonStateChange()    # Get state change of all buttons
 ```
 
 ---
 
 #### `resetButtonStates`
@@ -686,7 +732,98 @@
 
 # Or if using Sprig's 8 buttons
 buttons = button.Button()
 buttons.resetButtonStates()    # Reset state of all buttons
 ```
 
 ---
+
+### `led` module
+
+#### Initialisation
+
+```py
+import board
+from sprig_essentials.io import led
+
+# If you want to manually initialise the LED
+led_device = led.LED(board.GP28)
+
+# If you want to create the LED object and initialise it later
+led_device = led.LED()
+
+# If you are using this with a Sprig
+led_device = led.LED(quick_start=True)
+```
+
+- **Parameters:**
+  - `led_pin`: Pin number for the LED (default: `board.GP25`)
+- **Returns:** `LED` object.
+
+The `LED` class manages the Sprig's LED and its components. The initialisation functions in this class don't have to be called if you are using this with a Sprig.
+
+---
+
+#### `createLED`
+
+Creates a digital output object for the specified pin.
+
+- **Parameters:**
+  - `led_pin`: Pin number for the LED
+- **Returns:** `digitalio__digital_in_out` object.
+
+Example:
+
+```py
+led_object = led.LED()
+led_object.createLED(board.GP28)
+```
+
+---
+
+#### `on`
+
+Turns the LED on.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.on()
+```
+
+---
+
+#### `off`
+
+Turns the LED off.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.off()
+```
+
+---
+
+#### `toggle`
+
+Toggles the LED.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.toggle()
+```
+
+---
```

### Comparing `sprig_essentials-0.4.0/README.md` & `sprig_essentials-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,89 @@
-# sprig-essentials 0.4.0
+# sprig-essentials
 
-Useful functions to simplify the process of creating games and apps with Sprig when using [CircuitPython](https://circuitpython.org/).
+Useful functions to simplify the process of creating games and apps with Sprig when using [*CircuitPython*](https://circuitpython.org/).
 
-**This package can currently only be used when developing using a device with internet. The package is not available for download on the Raspberry Pi Pico itself yet.**
+**This package can currently only be used when developing using a device with internet. The package is not available for download on the *Raspberry Pi Pico* itself yet.**
 
 [![Upload Python Package](https://github.com/WhenLifeHandsYouLemons/sprig_essentials/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WhenLifeHandsYouLemons/sprig_essentials/actions/workflows/python-publish.yml)
 
 ---
 
 ## Installation
 
-To install the correct CircuitPython firmware and libraries for the Raspberry Pi Pico, follow these steps:
+### Basic Installation
 
-1. Download the .UF2 from the CircuitPython website [here](https://circuitpython.org/board/raspberry_pi_pico/).
-2. Press and hold the white button on the RPi Pico, then plug it into your computer while pressing the button. It should appear as a USB drive.
-3. Drag the downloaded .UF2 file into the USB drive. The RPi Pico should automatically reboot and CircuitPython should be installed.
+To install the correct *CircuitPython* firmware and libraries for the *Raspberry Pi Pico*, follow these steps:
+
+1. Download the .UF2 from the *CircuitPython* website [here](https://circuitpython.org/board/raspberry_pi_pico/).
+2. Press and hold the white button on the *RPi Pico*, then plug it into your computer while pressing the button. It should appear as a USB drive.
+3. Drag the downloaded `.UF2` file into the USB drive. The *RPi Pico* should automatically reboot and *CircuitPython* should be installed.
 4. In the USB drive, create a new folder called `lib` if it doesn't already exist.
 5. Download the necessary libraries from [this sub-folder](https://github.com/WhenLifeHandsYouLemons/sprig-essentials/tree/cbcddaf0884fbc39bbaa791aa085280db103ce35/libraries) and place them in the `lib` folder.
+6. At this point, you can now start using the `sprig_essentials` package on the *Raspberry Pi Pico*.
 
-To install `sprig_essentials` and use it on your Windows machine when developing for the Raspberry Pi Pico:
+To install `sprig_essentials` and use it on your Windows machine when developing for the *Raspberry Pi Pico*, you need to do the following:
 
-```txt
+```shell
 pip install sprig-essentials
 ```
 
-This package is intended to run on the `Raspberry Pi Pico H`.
+Then, to use it in a program you can import the entire package:
+
+```py
+import sprig_essentials as se
+```
+
+Or import specific modules (for example, the [display](#display-module) module):
+
+```py
+from sprig_essentials.io import display
+```
+
+### Manual Installation
+
+This package can be installed manually by downloading and compiling the source code. To do this, follow these steps:
+
+1. Clone the repository and nvaigate to it:
 
-This package assumes you've installed `CircuitPython` and are using the `ST7735` display.
+    ```shell
+    git clone https://github.com/WhenLifeHandsYouLemons/sprig-essentials.git
+    cd sprig-essentials
+    ```
+
+2. Compile the package:
+
+    ```shell
+    python convert_to_mpy.py
+    ```
+
+    or
+
+    ```shell
+    python3 convert_to_mpy.py
+    ```
+
+3. Copy the files inside the `output` folder to your Raspberry Pi Pico's `lib` folder.
+4. You can now start using the `sprig_essentials` package on the Raspberry Pi Pico.
+
+**This package is intended to run on the `Raspberry Pi Pico H`.**
+
+**This package assumes you've installed `CircuitPython` and are using the `ST7735` display.**
 
 ---
 
 ## Wiring Diagram
 
 The wiring diagram that this package assumes is intended for anyone using a Sprig, however, you can also wire this manually and achieve the same effect.
 
-![Image showing the pin connections from the Raspberry Pi Pico H to the various peripherals on the Sprig's board](https://camo.githubusercontent.com/d9b4afd8b99cc6befd3e04bdb8231c9fd134333ebd6a17166ca391429221ff05/68747470733a2f2f70617065722d6174746163686d656e74732e64726f70626f782e636f6d2f735f303531314241344231393135393837353345434243343935363743303632334234453646313535314241453338333243443842384232454441463236464142365f313636323537323037313339375f53637265656e2b53686f742b323032322d30392d30372b61742b312e33342e32312b504d2e706e67 "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
+![Image showing the PCB wires from the Raspberry Pi Pico H to the various peripherals on the Sprig's board](documentation/images/sprig_pcb_wiring_diagram.png "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
 
-Here's a clearer electrical wiring diagram:
+Here's a clearer pin connection diagram for GPIO pin numbers:
 
-![Image showing the electric wiring diagram for the Raspberry Pi Pico H and the Sprig](https://camo.githubusercontent.com/f0ff037c476cfa07603e9c8ec77394ee53f18701c89f509a2852b623583d1807/68747470733a2f2f70617065722d6174746163686d656e74732e64726f70626f782e636f6d2f735f303531314241344231393135393837353345434243343935363743303632334234453646313535314241453338333243443842384232454441463236464142365f313636323537313738303737365f53637265656e2b53686f742b323032322d30392d30372b61742b312e31322e35372b504d2e706e67 "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
+![Image showing the pin connection diagram for the Raspberry Pi Pico H and the Sprig](documentation/images/sprig_peripheral_pin_connection_image.png "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
 
 ---
 
 ## Documentation
 
 ### Core module
 
@@ -68,22 +109,21 @@
 
 ```py
 hex_value = core.convertRGBToHex([255, 255, 255])
 ```
 
 ---
 
-
 ### `display` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import display
+from sprig_essentials.io import display
 
 display_device = display.Display()
 ```
 
 - **Parameters:**
   - `backlight_pin`: Pin number for the backlight (default: `board.GP17`)
   - `clock_pin`: Pin number for the clock (default: `board.GP18`)
@@ -324,15 +364,15 @@
 
 ### `audio` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import audio
+from sprig_essentials.io import audio
 
 audio_device = audio.Audio()
 ```
 
 - **Parameters:**
   - `bit_clock_pin`: Pin number for the bit clock (default: `board.GP10`)
   - `word_select_pin`: Pin number for word select (default: `board.GP11`)
@@ -538,15 +578,15 @@
 
 ### `buttons` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import button
+from sprig_essentials.io import button
 
 # Initialize a button using a pin number
 button_1 = button.Button(board.GP5)
 
 # Or if using a Sprig
 buttons = button.Button(quick_start=True)
 ```
@@ -591,29 +631,35 @@
 quick_buttons = button.quickStartButtons()
 ```
 
 ---
 
 #### `getPressed`
 
-Gets the current state of the button.
+Gets the current state of the button. This automatically updates the current and previous state of the button.
 
-- **Parameters:**
-  - `button`: Optional digital input object; if provided, gets the state of this specific button
-- **Returns:** If a specific button is provided, returns `True` if pressed, `False` if released. If no button is specified, returns a list of states for all buttons.
+- **Parameters:** `None`
+- **Returns:**
+  - Returns `True` if pressed
+  - Returns `False` if released
+  - If no button is specified, returns a list of states for all buttons.
 
 Example:
 
 ```py
 button = button.Button(board.GP5)
-state = button.getPressed()    # Get state of specific button
+state = button.getPressed()
 
-# Or if using Sprig's 8 buttons
+# Or if using the Sprig's 8 buttons
 buttons = button.Button()
 states = buttons.getPressed()    # Get state of all buttons
+
+# Getting the state of a specific button
+w_button = buttons[0]
+w_state = buttons.getPressed(w_button)
 ```
 
 ---
 
 #### `updateButton`
 
 Updates the current and previous state of the button.
@@ -632,29 +678,29 @@
 buttons.updateButton()    # Update state of all buttons
 ```
 
 ---
 
 #### `getButtonStateChange`
 
-Returns the state change of the button.
+Returns the state change of the button. This automatically updates the current and previous state of the button.
 
 - **Parameters:** `None`
 - **Returns:**:
   - `"pressed"` if state changes from `False` to `True`
   - `"released"` if state changes from `True` to `False`
-  - `"no change"` if state did not change
+  - `"no change"` if state did not change.
 
 Example:
 
 ```py
 button = button.Button(board.GP5)
-state_change = button.getButtonStateChange()    # Get state change of specific button
+state_change = button.getButtonStateChange()
 
-# Or if using Sprig's 8 buttons
+# Or if using the Sprig's 8 buttons
 buttons = button.Button()
 state_changes = buttons.getButtonStateChange()    # Get state change of all buttons
 ```
 
 ---
 
 #### `resetButtonStates`
@@ -672,7 +718,98 @@
 
 # Or if using Sprig's 8 buttons
 buttons = button.Button()
 buttons.resetButtonStates()    # Reset state of all buttons
 ```
 
 ---
+
+### `led` module
+
+#### Initialisation
+
+```py
+import board
+from sprig_essentials.io import led
+
+# If you want to manually initialise the LED
+led_device = led.LED(board.GP28)
+
+# If you want to create the LED object and initialise it later
+led_device = led.LED()
+
+# If you are using this with a Sprig
+led_device = led.LED(quick_start=True)
+```
+
+- **Parameters:**
+  - `led_pin`: Pin number for the LED (default: `board.GP25`)
+- **Returns:** `LED` object.
+
+The `LED` class manages the Sprig's LED and its components. The initialisation functions in this class don't have to be called if you are using this with a Sprig.
+
+---
+
+#### `createLED`
+
+Creates a digital output object for the specified pin.
+
+- **Parameters:**
+  - `led_pin`: Pin number for the LED
+- **Returns:** `digitalio__digital_in_out` object.
+
+Example:
+
+```py
+led_object = led.LED()
+led_object.createLED(board.GP28)
+```
+
+---
+
+#### `on`
+
+Turns the LED on.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.on()
+```
+
+---
+
+#### `off`
+
+Turns the LED off.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.off()
+```
+
+---
+
+#### `toggle`
+
+Toggles the LED.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.toggle()
+```
+
+---
```

### Comparing `sprig_essentials-0.4.0/pyproject.toml` & `sprig_essentials-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprig_essentials"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Sooraj Sannabhadti", email="developer.soorajs@gmail.com" },
 ]
-description = "Useful functions for creating games and apps with Sprig"
+description = "Simplifying the process of creating games and apps for the Sprig."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sprig_essentials-0.4.0/src/sprig_essentials/__init__.py` & `sprig_essentials-0.5.0/src/sprig_essentials/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-# Useful functions to have when using any module
-
 # Convert rgb colour values to hex
 def convertRGBToHex(rgb: list):
     if len(rgb) > 3:
         raise IndexError(f"The list should have 3 value for the red, green, and blue channels! You have: {len(rgb)} values in your list.")
     elif rgb[0] > 255 or rgb[0] < 0 or rgb[1] > 255 or rgb[1] < 0 or rgb[2] > 255 or rgb[2] < 0:
         raise ValueError(f"The values should be between 0 and 255 inclusive! Your input is: {rgb}.")
     elif (type(rgb[0]) != int and type(rgb[0]) != float) or (type(rgb[1]) != int and type(rgb[1]) != float) or (type(rgb[2]) != int and type(rgb[2]) != float):
         raise TypeError("The values in the list are not of the correct type! It should either be an int or a float.")
     else:
         return int("{:02x}{:02x}{:02x}".format(rgb[0], rgb[1], rgb[2]), 16)
-
```

### Comparing `sprig_essentials-0.4.0/src/sprig_essentials/audio.py` & `sprig_essentials-0.5.0/src/sprig_essentials/io/audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import board
 import displayio
 import audiobusio, audiocore, audiomp3
 import array, math
-from typing import Any
 
 # To show return tooltips for functions
+class Any:pass
 class pin_number:pass
 class audiobusio__i2s:pass
 class audiocore__rawsample:pass
 class audiocore__wavefile:pass
 class circuitpython_typing__AudioSample:pass
 
 # Reset all pins to allow new connections
@@ -96,11 +96,14 @@
     return wave_file
 
 # Generate one period of sine wave.
 def createSineWave() -> "list[int]":
     length = 8000 // 440
     sine_wave = array.array("H", [0] * length)
 
+    amplitude = 2 ** 15
+    x_offset = 2 ** 15
+
     for i in range(length):
-        sine_wave[i] = int(math.sin(math.pi * 2 * i / length) * (2 ** 15) + 2 ** 15)
+        sine_wave[i] = int(amplitude * math.sin(math.pi * 2 * i / length) + x_offset)
 
     return sine_wave
```

### Comparing `sprig_essentials-0.4.0/src/sprig_essentials/buttons.py` & `sprig_essentials-0.5.0/src/sprig_essentials/io/buttons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import board
 import displayio, digitalio
-from typing import Any, Union
 
 # To show return tooltips for functions
+class Any:pass
 class pin_number:pass
 class digitalio__digital_in_out:pass
 
 # Reset all pins to allow new connections
 displayio.release_displays()
 
 class Button:
@@ -43,15 +43,15 @@
         button = digitalio.DigitalInOut(btn_pin)
         button.direction = digitalio.Direction.INPUT
         button.pull = digitalio.Pull.UP
 
         return button
 
     # Automates buttons creation, assuming you're using a Sprig
-    def quickStartButtons(self) -> digitalio__digital_in_out:
+    def quickStartButtons(self) -> "tuple[digitalio__digital_in_out]":
         w = digitalio.DigitalInOut(board.GP5)
         w.direction = digitalio.Direction.INPUT
         w.pull = digitalio.Pull.UP
 
         a = digitalio.DigitalInOut(board.GP6)
         a.direction = digitalio.Direction.INPUT
         a.pull = digitalio.Pull.UP
@@ -80,48 +80,51 @@
         l.direction = digitalio.Direction.INPUT
         l.pull = digitalio.Pull.UP
 
         return w, a, s, d, i, j, k, l
 
     # Gets the current state of the button
     # True is pressed, False is released
-    def getPressed(self,
-                   button: digitalio__digital_in_out = None) -> Union[bool, "list[bool]"]:
-        if button != None:
-            return not button.value
+    def getPressed(self) -> bool | "list[bool]":
+        self.updateButton()
 
         if not self.quick_start:
             return not self.button.value
         else:
             # Return a list of all the buttons that are pressed currently
             return [self.getPressed(self.w), self.getPressed(self.a), self.getPressed(self.s), self.getPressed(self.d),
                     self.getPressed(self.i), self.getPressed(self.j), self.getPressed(self.k), self.getPressed(self.l)]
 
-    # Returns "pressed" if state changes from False to True, and "released" if state changes from True to False, and "no change" if nothing changed
-    # IMPORTANT: Run updateButton immediately before running this
-    def getButtonStateChange(self) -> Union[bool, "list[bool]"]:
+    # Returns "pressed" if state changes from False to True,
+    #         "released" if state changes from True to False,
+    #         "no change" if nothing changed
+    def getButtonStateChange(self) -> bool | "list[bool]":
+        self.updateButton()
+
         if not self.quick_start:
             if self.prev_state != self.cur_state:
                 if self.cur_state:
                     return "pressed"
                 else:
                     return "released"
             else:
                 return "no change"
         else:
             # Return a list of all the buttons that are pressed currently
             output = []
+
             for p, c in zip(self.quick_btns_prev_states, self.quick_btns_cur_states):
                 if p != c:
                     if c:
                         output.append("pressed")
                     else:
                         output.append("released")
                 else:
                     output.append("no change")
+
             return output
 
     # Update the current and previous state of the button
     def updateButton(self) -> None:
         if self.quick_start:
             self.quick_btns_prev_states = self.quick_btns_cur_states.copy()
             self.quick_btns_cur_states = self.getPressed()
```

### Comparing `sprig_essentials-0.4.0/src/sprig_essentials/display.py` & `sprig_essentials-0.5.0/src/sprig_essentials/io/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import board
-import displayio, digitalio, busio, terminalio
-from adafruit_display_text import label
+import displayio, digitalio, busio
 from adafruit_st7735r import ST7735R
-from typing import Any
 
 # To show return tooltips for functions
+class Any:pass
 class pin_number:pass
 class digitalio__digital_in_out:pass
 class busio__spi:pass
 class displayio__display_bus:pass
 class st7735r:pass
 class displayio__group:pass
 class displayio__bitmap:pass
 class displayio__palette:pass
 class displayio__sprite:pass
-class terminalio__font:pass
-class label__label:pass
 
 # Reset all pins to allow new connections
 displayio.release_displays()
 
 class Display:
     def __init__(self,
                  backlight_pin: pin_number = board.GP17,
@@ -134,16 +131,7 @@
 def createSprite(bitmap: displayio__bitmap,
                  pixel_shader: displayio__palette,
                  x: int = 0,
                  y: int = 0) -> displayio__sprite:
     sprite = displayio.TileGrid(bitmap, pixel_shader=pixel_shader, x=x, y=y)
 
     return sprite
-
-def createTextSprite(text: str,
-                     colour: tuple,
-                     x: int = 0,
-                     y: int = 0,
-                     font: terminalio__font = terminalio.FONT) -> label__label:
-    text_area = label.Label(font, text=text, color=colour, x=x, y=y)
-
-    return text_area
```

### Comparing `sprig_essentials-0.4.0/src/sprig_essentials.egg-info/PKG-INFO` & `sprig_essentials-0.5.0/src/sprig_essentials.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,103 @@
 Metadata-Version: 2.1
-Name: sprig-essentials
-Version: 0.4.0
-Summary: Useful functions for creating games and apps with Sprig
+Name: sprig_essentials
+Version: 0.5.0
+Summary: Simplifying the process of creating games and apps for the Sprig.
 Author-email: Sooraj Sannabhadti <developer.soorajs@gmail.com>
 Project-URL: Homepage, https://github.com/WhenLifeHandsYouLemons/sprig_essentials
 Project-URL: Bug Tracker, https://github.com/WhenLifeHandsYouLemons/sprig_essentials/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sprig-essentials 0.4.0
+# sprig-essentials
 
-Useful functions to simplify the process of creating games and apps with Sprig when using [CircuitPython](https://circuitpython.org/).
+Useful functions to simplify the process of creating games and apps with Sprig when using [*CircuitPython*](https://circuitpython.org/).
 
-**This package can currently only be used when developing using a device with internet. The package is not available for download on the Raspberry Pi Pico itself yet.**
+**This package can currently only be used when developing using a device with internet. The package is not available for download on the *Raspberry Pi Pico* itself yet.**
 
 [![Upload Python Package](https://github.com/WhenLifeHandsYouLemons/sprig_essentials/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WhenLifeHandsYouLemons/sprig_essentials/actions/workflows/python-publish.yml)
 
 ---
 
 ## Installation
 
-To install the correct CircuitPython firmware and libraries for the Raspberry Pi Pico, follow these steps:
+### Basic Installation
 
-1. Download the .UF2 from the CircuitPython website [here](https://circuitpython.org/board/raspberry_pi_pico/).
-2. Press and hold the white button on the RPi Pico, then plug it into your computer while pressing the button. It should appear as a USB drive.
-3. Drag the downloaded .UF2 file into the USB drive. The RPi Pico should automatically reboot and CircuitPython should be installed.
+To install the correct *CircuitPython* firmware and libraries for the *Raspberry Pi Pico*, follow these steps:
+
+1. Download the .UF2 from the *CircuitPython* website [here](https://circuitpython.org/board/raspberry_pi_pico/).
+2. Press and hold the white button on the *RPi Pico*, then plug it into your computer while pressing the button. It should appear as a USB drive.
+3. Drag the downloaded `.UF2` file into the USB drive. The *RPi Pico* should automatically reboot and *CircuitPython* should be installed.
 4. In the USB drive, create a new folder called `lib` if it doesn't already exist.
 5. Download the necessary libraries from [this sub-folder](https://github.com/WhenLifeHandsYouLemons/sprig-essentials/tree/cbcddaf0884fbc39bbaa791aa085280db103ce35/libraries) and place them in the `lib` folder.
+6. At this point, you can now start using the `sprig_essentials` package on the *Raspberry Pi Pico*.
 
-To install `sprig_essentials` and use it on your Windows machine when developing for the Raspberry Pi Pico:
+To install `sprig_essentials` and use it on your Windows machine when developing for the *Raspberry Pi Pico*, you need to do the following:
 
-```txt
+```shell
 pip install sprig-essentials
 ```
 
-This package is intended to run on the `Raspberry Pi Pico H`.
+Then, to use it in a program you can import the entire package:
+
+```py
+import sprig_essentials as se
+```
+
+Or import specific modules (for example, the [display](#display-module) module):
+
+```py
+from sprig_essentials.io import display
+```
+
+### Manual Installation
+
+This package can be installed manually by downloading and compiling the source code. To do this, follow these steps:
+
+1. Clone the repository and nvaigate to it:
 
-This package assumes you've installed `CircuitPython` and are using the `ST7735` display.
+    ```shell
+    git clone https://github.com/WhenLifeHandsYouLemons/sprig-essentials.git
+    cd sprig-essentials
+    ```
+
+2. Compile the package:
+
+    ```shell
+    python convert_to_mpy.py
+    ```
+
+    or
+
+    ```shell
+    python3 convert_to_mpy.py
+    ```
+
+3. Copy the files inside the `output` folder to your Raspberry Pi Pico's `lib` folder.
+4. You can now start using the `sprig_essentials` package on the Raspberry Pi Pico.
+
+**This package is intended to run on the `Raspberry Pi Pico H`.**
+
+**This package assumes you've installed `CircuitPython` and are using the `ST7735` display.**
 
 ---
 
 ## Wiring Diagram
 
 The wiring diagram that this package assumes is intended for anyone using a Sprig, however, you can also wire this manually and achieve the same effect.
 
-![Image showing the pin connections from the Raspberry Pi Pico H to the various peripherals on the Sprig's board](https://camo.githubusercontent.com/d9b4afd8b99cc6befd3e04bdb8231c9fd134333ebd6a17166ca391429221ff05/68747470733a2f2f70617065722d6174746163686d656e74732e64726f70626f782e636f6d2f735f303531314241344231393135393837353345434243343935363743303632334234453646313535314241453338333243443842384232454441463236464142365f313636323537323037313339375f53637265656e2b53686f742b323032322d30392d30372b61742b312e33342e32312b504d2e706e67 "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
+![Image showing the PCB wires from the Raspberry Pi Pico H to the various peripherals on the Sprig's board](documentation/images/sprig_pcb_wiring_diagram.png "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
 
-Here's a clearer electrical wiring diagram:
+Here's a clearer pin connection diagram for GPIO pin numbers:
 
-![Image showing the electric wiring diagram for the Raspberry Pi Pico H and the Sprig](https://camo.githubusercontent.com/f0ff037c476cfa07603e9c8ec77394ee53f18701c89f509a2852b623583d1807/68747470733a2f2f70617065722d6174746163686d656e74732e64726f70626f782e636f6d2f735f303531314241344231393135393837353345434243343935363743303632334234453646313535314241453338333243443842384232454441463236464142365f313636323537313738303737365f53637265656e2b53686f742b323032322d30392d30372b61742b312e31322e35372b504d2e706e67 "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
+![Image showing the pin connection diagram for the Raspberry Pi Pico H and the Sprig](documentation/images/sprig_peripheral_pin_connection_image.png "Taken from 'https://github.com/hackclub/sprig/blob/main/docs/GROWING_A_SPRIG.md'")
 
 ---
 
 ## Documentation
 
 ### Core module
 
@@ -82,22 +123,21 @@
 
 ```py
 hex_value = core.convertRGBToHex([255, 255, 255])
 ```
 
 ---
 
-
 ### `display` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import display
+from sprig_essentials.io import display
 
 display_device = display.Display()
 ```
 
 - **Parameters:**
   - `backlight_pin`: Pin number for the backlight (default: `board.GP17`)
   - `clock_pin`: Pin number for the clock (default: `board.GP18`)
@@ -338,15 +378,15 @@
 
 ### `audio` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import audio
+from sprig_essentials.io import audio
 
 audio_device = audio.Audio()
 ```
 
 - **Parameters:**
   - `bit_clock_pin`: Pin number for the bit clock (default: `board.GP10`)
   - `word_select_pin`: Pin number for word select (default: `board.GP11`)
@@ -552,15 +592,15 @@
 
 ### `buttons` module
 
 #### Initialisation
 
 ```py
 import board
-from sprig_essentials import button
+from sprig_essentials.io import button
 
 # Initialize a button using a pin number
 button_1 = button.Button(board.GP5)
 
 # Or if using a Sprig
 buttons = button.Button(quick_start=True)
 ```
@@ -605,29 +645,35 @@
 quick_buttons = button.quickStartButtons()
 ```
 
 ---
 
 #### `getPressed`
 
-Gets the current state of the button.
+Gets the current state of the button. This automatically updates the current and previous state of the button.
 
-- **Parameters:**
-  - `button`: Optional digital input object; if provided, gets the state of this specific button
-- **Returns:** If a specific button is provided, returns `True` if pressed, `False` if released. If no button is specified, returns a list of states for all buttons.
+- **Parameters:** `None`
+- **Returns:**
+  - Returns `True` if pressed
+  - Returns `False` if released
+  - If no button is specified, returns a list of states for all buttons.
 
 Example:
 
 ```py
 button = button.Button(board.GP5)
-state = button.getPressed()    # Get state of specific button
+state = button.getPressed()
 
-# Or if using Sprig's 8 buttons
+# Or if using the Sprig's 8 buttons
 buttons = button.Button()
 states = buttons.getPressed()    # Get state of all buttons
+
+# Getting the state of a specific button
+w_button = buttons[0]
+w_state = buttons.getPressed(w_button)
 ```
 
 ---
 
 #### `updateButton`
 
 Updates the current and previous state of the button.
@@ -646,29 +692,29 @@
 buttons.updateButton()    # Update state of all buttons
 ```
 
 ---
 
 #### `getButtonStateChange`
 
-Returns the state change of the button.
+Returns the state change of the button. This automatically updates the current and previous state of the button.
 
 - **Parameters:** `None`
 - **Returns:**:
   - `"pressed"` if state changes from `False` to `True`
   - `"released"` if state changes from `True` to `False`
-  - `"no change"` if state did not change
+  - `"no change"` if state did not change.
 
 Example:
 
 ```py
 button = button.Button(board.GP5)
-state_change = button.getButtonStateChange()    # Get state change of specific button
+state_change = button.getButtonStateChange()
 
-# Or if using Sprig's 8 buttons
+# Or if using the Sprig's 8 buttons
 buttons = button.Button()
 state_changes = buttons.getButtonStateChange()    # Get state change of all buttons
 ```
 
 ---
 
 #### `resetButtonStates`
@@ -686,7 +732,98 @@
 
 # Or if using Sprig's 8 buttons
 buttons = button.Button()
 buttons.resetButtonStates()    # Reset state of all buttons
 ```
 
 ---
+
+### `led` module
+
+#### Initialisation
+
+```py
+import board
+from sprig_essentials.io import led
+
+# If you want to manually initialise the LED
+led_device = led.LED(board.GP28)
+
+# If you want to create the LED object and initialise it later
+led_device = led.LED()
+
+# If you are using this with a Sprig
+led_device = led.LED(quick_start=True)
+```
+
+- **Parameters:**
+  - `led_pin`: Pin number for the LED (default: `board.GP25`)
+- **Returns:** `LED` object.
+
+The `LED` class manages the Sprig's LED and its components. The initialisation functions in this class don't have to be called if you are using this with a Sprig.
+
+---
+
+#### `createLED`
+
+Creates a digital output object for the specified pin.
+
+- **Parameters:**
+  - `led_pin`: Pin number for the LED
+- **Returns:** `digitalio__digital_in_out` object.
+
+Example:
+
+```py
+led_object = led.LED()
+led_object.createLED(board.GP28)
+```
+
+---
+
+#### `on`
+
+Turns the LED on.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.on()
+```
+
+---
+
+#### `off`
+
+Turns the LED off.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.off()
+```
+
+---
+
+#### `toggle`
+
+Toggles the LED.
+
+- **Parameters:** `None`
+- **Returns:** `None`
+
+Example:
+
+```py
+led_object = led.LED(board.GP28)
+led_object.toggle()
+```
+
+---
```

