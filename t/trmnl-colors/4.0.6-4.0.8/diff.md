# Comparing `tmp/trmnl-colors-4.0.6.tar.gz` & `tmp/trmnl-colors-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trmnl-colors-4.0.6.tar", last modified: Wed Aug 23 14:54:31 2023, max compression
+gzip compressed data, was "trmnl-colors-4.0.8.tar", last modified: Thu Apr  4 10:10:02 2024, max compression
```

## Comparing `trmnl-colors-4.0.6.tar` & `trmnl-colors-4.0.8.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-23 14:54:31.206343 trmnl-colors-4.0.6/
--rw-rw-rw-   0        0        0     1090 2023-06-07 10:41:05.000000 trmnl-colors-4.0.6/LICENSE
--rw-rw-rw-   0        0        0     2381 2023-08-23 14:54:31.199334 trmnl-colors-4.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2023-08-23 14:53:06.000000 trmnl-colors-4.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-08-23 14:54:31.210335 trmnl-colors-4.0.6/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-08-23 14:50:11.000000 trmnl-colors-4.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-23 14:54:30.963335 trmnl-colors-4.0.6/test/
--rw-rw-rw-   0        0        0       61 2023-06-08 16:13:27.000000 trmnl-colors-4.0.6/test/test.py
-drwxrwxrwx   0        0        0        0 2023-08-23 14:54:31.138334 trmnl-colors-4.0.6/trmnl_colors/
--rw-rw-rw-   0        0        0     5704 2023-08-23 14:49:49.000000 trmnl-colors-4.0.6/trmnl_colors/__init__.py
--rw-rw-rw-   0        0        0     1568 2023-08-23 13:18:58.000000 trmnl-colors-4.0.6/trmnl_colors/constants.py
--rw-rw-rw-   0        0        0     5577 2023-08-23 12:50:52.000000 trmnl-colors-4.0.6/trmnl_colors/functions.py
-drwxrwxrwx   0        0        0        0 2023-08-23 14:54:31.189346 trmnl-colors-4.0.6/trmnl_colors.egg-info/
--rw-rw-rw-   0        0        0     2381 2023-08-23 14:54:30.000000 trmnl-colors-4.0.6/trmnl_colors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-08-23 14:54:30.000000 trmnl-colors-4.0.6/trmnl_colors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-23 14:54:30.000000 trmnl-colors-4.0.6/trmnl_colors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-23 14:54:30.000000 trmnl-colors-4.0.6/trmnl_colors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 10:10:02.940660 trmnl-colors-4.0.8/
+-rw-rw-rw-   0        0        0     1090 2024-04-04 08:54:00.000000 trmnl-colors-4.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2533 2024-04-04 10:10:02.938660 trmnl-colors-4.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2188 2024-04-04 09:51:36.000000 trmnl-colors-4.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:10:02.940660 trmnl-colors-4.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      556 2024-04-04 09:35:59.000000 trmnl-colors-4.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:10:02.930660 trmnl-colors-4.0.8/trmnl_colors/
+-rw-rw-rw-   0        0        0     1742 2024-04-04 09:06:14.000000 trmnl-colors-4.0.8/trmnl_colors/__init__.py
+-rw-rw-rw-   0        0        0     2538 2024-04-04 09:35:43.000000 trmnl-colors-4.0.8/trmnl_colors/constants.py
+-rw-rw-rw-   0        0        0     5210 2024-04-04 09:36:55.000000 trmnl-colors-4.0.8/trmnl_colors/functions.py
+-rw-rw-rw-   0        0        0       47 2024-04-04 09:21:08.000000 trmnl-colors-4.0.8/trmnl_colors/test.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:10:02.937660 trmnl-colors-4.0.8/trmnl_colors.egg-info/
+-rw-rw-rw-   0        0        0     2533 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/top_level.txt
```

### Comparing `trmnl-colors-4.0.6/LICENSE` & `trmnl-colors-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trmnl-colors-4.0.6/PKG-INFO` & `trmnl-colors-4.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 Metadata-Version: 2.1
 Name: trmnl-colors
-Version: 4.0.6
+Version: 4.0.8
 Summary: Colors, text formats, decorations and much more for TERMINAL
 Home-page: https://github.com/Idrisvohra9/colors
 Author: Idris-Vohra
 Author-email: idrishaider987@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
-# trmnl_colors v-4.0.6
+# trmnl_colors v-4.0.8
 ## Add colors to the static WOrLd!
 
+This module is made to colorize the output of terminal when the code runs on command line, With that there are functions for adding basic text colors (Total 10 including invisible) and or text formats such as Bold, Italics, Underline, Light or Strike-through to your code.
 
-colors module is made to colorize the output of terminal when the code runs on command line, With that there are functions for adding basic text colors (Total 10 including invsisble) and or text formats such as Bold, Italics, Underline, Light or Strikethrough to your code.
+But wait there is more! use background colors, filled Variants which can be accessed by calling their specific name and 'Bg' postfix as in background. Here is an example describing with  use case:
 
-But wait there is more! use background colors, filled Variants which can be accessed by calling thier specific name and 'bg' postfix as in background. Here is an example describing with  use case:
+```python
+from trmnl_colors import *
+blueBg()
+print("Hello")
+reset()
+```
 
 ## Latest Updates:
 
 ### Introducing constants to make your life more easier:
 
 >### Use case for constants
 
 ```python
 from trmnl_colors.constants import *
 
-print(RedB + "Hello" + GreenB + " World!", end="")
+print(RedBold + "Hello" + GreenBold + " World!", end="")
 
 print(RESET,end="")
 
 ```
 >### Use case for functions
 
 ```python
 from trmnl_colors.functions import *
-bluebg()
+blueBg()
 print("Hello")
-reset()
+white()
 ```
 
-* Each color can be accessed by calling thier particular name and the first letter of the format at the postfix.
 ```python
 from trmnl_colors.functions import *
-yellowB()
+yellowBold()
 print("Hello") # After every color call remember to call the reset function.
 # Outputs Hello in yellow color in Bold text
-reset()
+white()
 ```
-* For example:Call clr.redB() for red color with text format Bold, S for strikethrough D for Default U for Underline I for Italics L is for special lighter color substitute for each color.
-
 
 * There are also filled color variants in which the font color and the background color match each other making them viable for specific type of color operations. 
 
-* There is a special function called reset() which is basically the default white so that the color function gets reset it is recommended to use this function after every usage of a color to mantain the color of the terminal.
-* 
-* PS if you want to create blocks of colors for decoration purposes use filled variants e.g. clr.whitefilled() 
+* There is a special function called white() which is basically the default white so that the color function gets reset it is recommended to use this function at the end to maintain the color of the terminal.
+* PS. if you want to create blocks of colors for decoration purposes use filled variants e.g. whiteFilled() 
 
 ## Terminal Application Screenshots with trmnl_colors:
+### Create Terminal programs such as the below examples. Only your imagination and python skills are a limit!
 
+![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20171908.png?raw=true)
+![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20172610.png?raw=true)
 > Explore & stay Creative
->## by: Idris-Vohra
+
+>## by: [Idris Vohra]("https://github.com/Idrisvohra9")
```

### Comparing `trmnl-colors-4.0.6/README.md` & `trmnl-colors-4.0.8/trmnl_colors/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,38 @@
-
-# trmnl_colors v-4.0.6
+"""trmnl_colors v-4.0.8
 ## Add colors to the static WOrLd!
 
 
-colors module is made to colorize the output of terminal when the code runs on command line, With that there are functions for adding basic text colors (Total 10 including invsisble) and or text formats such as Bold, Italics, Underline, Light or Strikethrough to your code.
-
-But wait there is more! use background colors, filled Variants which can be accessed by calling thier specific name and 'bg' postfix as in background. Here is an example describing with  use case:
-
-## Latest Updates:
-
-### Introducing constants to make your life more easier:
-
->### Use case for constants
-
-```python
-from trmnl_colors.constants import *
-
-print(RedB + "Hello" + GreenB + " World!", end="")
-
-print(RESET,end="")
-
-```
->### Use case for functions
+colors module is made to colorize the output of terminal when the code runs on command line, With that there are functions for adding basic text colors (Total 10 including invisible) and or text formats such as Bold, Italics, Underline, Light or Strike-through to your code.
 
+But wait there is more! use background colors, filled Variants which can be accessed by calling their specific name and 'bg' postfix as in background. Here is an example describing with  use case:
 ```python
-from trmnl_colors.functions import *
+from trmnl_colors import *
 bluebg()
 print("Hello")
 reset()
 ```
 
-* Each color can be accessed by calling thier particular name and the first letter of the format at the postfix.
+* Each color can be accessed by calling their particular name and the first letter of the format at the postfix.
 ```python
-from trmnl_colors.functions import *
+from trmnl_colors import *
 yellowB()
 print("Hello") # After every color call remember to call the reset function.
 # Outputs Hello in yellow color in Bold text
 reset()
 ```
 * For example:Call clr.redB() for red color with text format Bold, S for strikethrough D for Default U for Underline I for Italics L is for special lighter color substitute for each color.
 
 
 * There are also filled color variants in which the font color and the background color match each other making them viable for specific type of color operations. 
 
-* There is a special function called reset() which is basically the default white so that the color function gets reset it is recommended to use this function after every usage of a color to mantain the color of the terminal.
+* There is a special function called reset() which is basically the default white so that the color function gets reset it is recommended to use this function after every usage of a color to maintain the color of the terminal.
 * 
 * PS if you want to create blocks of colors for decoration purposes use filled variants e.g. clr.whitefilled() 
 
-## Terminal Application Screenshots with trmnl_colors:
+Explore & stay Creative
+### by: Idris-Vohra :O
+
+"""
 
-> Explore & stay Creative
->## by: Idris-Vohra
+from .constants import *
+from .functions import *
```

### Comparing `trmnl-colors-4.0.6/setup.py` & `trmnl-colors-4.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setuptools.setup(
     name="trmnl-colors",
-    version="4.0.6",
+    version="4.0.8",
     author="Idris-Vohra",
     author_email="idrishaider987@gmail.com",
     packages=["trmnl_colors"],
     description="Colors, text formats, decorations and much more for TERMINAL",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/Idrisvohra9/colors",
```

### Comparing `trmnl-colors-4.0.6/trmnl_colors.egg-info/PKG-INFO` & `trmnl-colors-4.0.8/trmnl_colors.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 Metadata-Version: 2.1
 Name: trmnl-colors
-Version: 4.0.6
+Version: 4.0.8
 Summary: Colors, text formats, decorations and much more for TERMINAL
 Home-page: https://github.com/Idrisvohra9/colors
 Author: Idris-Vohra
 Author-email: idrishaider987@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
-# trmnl_colors v-4.0.6
+# trmnl_colors v-4.0.8
 ## Add colors to the static WOrLd!
 
+This module is made to colorize the output of terminal when the code runs on command line, With that there are functions for adding basic text colors (Total 10 including invisible) and or text formats such as Bold, Italics, Underline, Light or Strike-through to your code.
 
-colors module is made to colorize the output of terminal when the code runs on command line, With that there are functions for adding basic text colors (Total 10 including invsisble) and or text formats such as Bold, Italics, Underline, Light or Strikethrough to your code.
+But wait there is more! use background colors, filled Variants which can be accessed by calling their specific name and 'Bg' postfix as in background. Here is an example describing with  use case:
 
-But wait there is more! use background colors, filled Variants which can be accessed by calling thier specific name and 'bg' postfix as in background. Here is an example describing with  use case:
+```python
+from trmnl_colors import *
+blueBg()
+print("Hello")
+reset()
+```
 
 ## Latest Updates:
 
 ### Introducing constants to make your life more easier:
 
 >### Use case for constants
 
 ```python
 from trmnl_colors.constants import *
 
-print(RedB + "Hello" + GreenB + " World!", end="")
+print(RedBold + "Hello" + GreenBold + " World!", end="")
 
 print(RESET,end="")
 
 ```
 >### Use case for functions
 
 ```python
 from trmnl_colors.functions import *
-bluebg()
+blueBg()
 print("Hello")
-reset()
+white()
 ```
 
-* Each color can be accessed by calling thier particular name and the first letter of the format at the postfix.
 ```python
 from trmnl_colors.functions import *
-yellowB()
+yellowBold()
 print("Hello") # After every color call remember to call the reset function.
 # Outputs Hello in yellow color in Bold text
-reset()
+white()
 ```
-* For example:Call clr.redB() for red color with text format Bold, S for strikethrough D for Default U for Underline I for Italics L is for special lighter color substitute for each color.
-
 
 * There are also filled color variants in which the font color and the background color match each other making them viable for specific type of color operations. 
 
-* There is a special function called reset() which is basically the default white so that the color function gets reset it is recommended to use this function after every usage of a color to mantain the color of the terminal.
-* 
-* PS if you want to create blocks of colors for decoration purposes use filled variants e.g. clr.whitefilled() 
+* There is a special function called white() which is basically the default white so that the color function gets reset it is recommended to use this function at the end to maintain the color of the terminal.
+* PS. if you want to create blocks of colors for decoration purposes use filled variants e.g. whiteFilled() 
 
 ## Terminal Application Screenshots with trmnl_colors:
+### Create Terminal programs such as the below examples. Only your imagination and python skills are a limit!
 
+![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20171908.png?raw=true)
+![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20172610.png?raw=true)
 > Explore & stay Creative
->## by: Idris-Vohra
+
+>## by: [Idris Vohra]("https://github.com/Idrisvohra9")
```

