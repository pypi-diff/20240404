# Comparing `tmp/pygame-popup-0.9.0.tar.gz` & `tmp/pygame-popup-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame-popup-0.9.0.tar", last modified: Mon Aug 14 15:54:52 2023, max compression
+gzip compressed data, was "pygame-popup-0.9.1.tar", last modified: Mon Aug 14 18:37:33 2023, max compression
```

## Comparing `pygame-popup-0.9.0.tar` & `pygame-popup-0.9.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:52.355820 pygame-popup-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/src/pygame_popup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-14 15:54:52.000000 pygame-popup-0.9.0/src/pygame_popup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-14 15:54:52.000000 pygame-popup-0.9.0/src/pygame_popup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 15:54:52.000000 pygame-popup-0.9.0/src/pygame_popup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-14 15:54:52.000000 pygame-popup-0.9.0/src/pygame_popup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-14 15:54:52.000000 pygame-popup-0.9.0/src/pygame_popup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/src/pygamepopup/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/src/pygamepopup/_exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/_exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/_exceptions/wrong_initialization_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/src/pygamepopup/components/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/components/box_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/components/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/components/dynamic_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/components/image_button.py
--rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/components/info_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/components/text_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:54:52.359820 pygame-popup-0.9.0/src/pygamepopup/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/images/default_box.png
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/images/default_box_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/menu_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-14 15:54:48.000000 pygame-popup-0.9.0/src/pygamepopup/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:33.895582 pygame-popup-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-14 18:37:33.895582 pygame-popup-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-14 18:37:33.895582 pygame-popup-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:33.891582 pygame-popup-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:33.891582 pygame-popup-0.9.1/src/pygame_popup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-14 18:37:33.000000 pygame-popup-0.9.1/src/pygame_popup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-14 18:37:33.000000 pygame-popup-0.9.1/src/pygame_popup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 18:37:33.000000 pygame-popup-0.9.1/src/pygame_popup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-14 18:37:33.000000 pygame-popup-0.9.1/src/pygame_popup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-14 18:37:33.000000 pygame-popup-0.9.1/src/pygame_popup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:33.895582 pygame-popup-0.9.1/src/pygamepopup/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:33.895582 pygame-popup-0.9.1/src/pygamepopup/_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/_exceptions/wrong_initialization_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:33.895582 pygame-popup-0.9.1/src/pygamepopup/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/components/box_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/components/dynamic_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/components/image_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/components/info_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/components/text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 18:37:33.895582 pygame-popup-0.9.1/src/pygamepopup/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/images/default_box.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/images/default_box_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/menu_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-14 18:37:26.000000 pygame-popup-0.9.1/src/pygamepopup/types.py
```

### Comparing `pygame-popup-0.9.0/LICENSE` & `pygame-popup-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/PKG-INFO` & `pygame-popup-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-popup
-Version: 0.9.0
+Version: 0.9.1
 Summary: A popup manager for pygame
 Home-page: https://github.com/Grimmys/pygame_popup_manager
 Author: Grimmys
 Author-email: grimmys.programming@gmail.com
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/Grimmys/pygame_popup_manager/issues
 Platform: UNKNOWN
```

### Comparing `pygame-popup-0.9.0/README.md` & `pygame-popup-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/setup.py` & `pygame-popup-0.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pygame-popup",
-    version="0.9.0",
+    version="0.9.1",
     author="Grimmys",
     author_email="grimmys.programming@gmail.com",
     description="A popup manager for pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Grimmys/pygame_popup_manager",
     project_urls={
```

### Comparing `pygame-popup-0.9.0/src/pygame_popup.egg-info/PKG-INFO` & `pygame-popup-0.9.1/src/pygame_popup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-popup
-Version: 0.9.0
+Version: 0.9.1
 Summary: A popup manager for pygame
 Home-page: https://github.com/Grimmys/pygame_popup_manager
 Author: Grimmys
 Author-email: grimmys.programming@gmail.com
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/Grimmys/pygame_popup_manager/issues
 Platform: UNKNOWN
```

### Comparing `pygame-popup-0.9.0/src/pygame_popup.egg-info/SOURCES.txt` & `pygame-popup-0.9.1/src/pygame_popup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/components/box_element.py` & `pygame-popup-0.9.1/src/pygamepopup/components/box_element.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/components/button.py` & `pygame-popup-0.9.1/src/pygamepopup/components/button.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/components/dynamic_button.py` & `pygame-popup-0.9.1/src/pygamepopup/components/dynamic_button.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/components/image_button.py` & `pygame-popup-0.9.1/src/pygamepopup/components/image_button.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/components/info_box.py` & `pygame-popup-0.9.1/src/pygamepopup/components/info_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         element_grid: list[list[BoxElement]],
         width: int = DEFAULT_POPUP_WIDTH,
         element_linked: Optional[pygame.Rect] = None,
         position: Optional[Position] = None,
         has_close_button: bool = True,
         title_color: pygame.Color = WHITE,
         background_path: str = None,
-        close_button_text: str = _default_texts["close_button"],
+        close_button_text: Optional[str] = None,
         close_button_background_path: str = None,
         close_button_background_hover_path: str = None,
         visible_on_background: bool = True,
         has_vertical_separator: bool = False,
         identifier: str = "",
     ) -> None:
         self.title: str = title
@@ -102,15 +102,16 @@
         }
         background_path = (
             os.path.abspath(background_path)
             if background_path
             else _default_sprites["info_box_background"]
         )
         self.sprite: pygame.Surface = pygame.image.load(background_path)
-        self.close_button_text: str = close_button_text
+        self.close_button_text: str = close_button_text if close_button_text is not None \
+            else _default_texts["close_button"]
         self.__close_button_background_path: str = close_button_background_path
         self.__close_button_background_hover_path: str = (
             close_button_background_hover_path
         )
         self.__elements: list[_Row] = self.init_elements()
         self.buttons: Sequence[Button] = []
         self.__size: tuple[int, int] = (width, 0)
```

### Comparing `pygame-popup-0.9.0/src/pygamepopup/components/text_element.py` & `pygame-popup-0.9.1/src/pygamepopup/components/text_element.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/configuration.py` & `pygame-popup-0.9.1/src/pygamepopup/configuration.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/fonts.py` & `pygame-popup-0.9.1/src/pygamepopup/fonts.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/images/default_box.png` & `pygame-popup-0.9.1/src/pygamepopup/images/default_box.png`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/images/default_box_hover.png` & `pygame-popup-0.9.1/src/pygamepopup/images/default_box_hover.png`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/initialization.py` & `pygame-popup-0.9.1/src/pygamepopup/initialization.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.9.0/src/pygamepopup/menu_manager.py` & `pygame-popup-0.9.1/src/pygamepopup/menu_manager.py`

 * *Files identical despite different names*

