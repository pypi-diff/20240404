# Comparing `tmp/streamlit-navigation-bar-3.0.2.tar.gz` & `tmp/streamlit-navigation-bar-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-navigation-bar-3.0.2.tar", last modified: Sun Mar 31 21:53:54 2024, max compression
+gzip compressed data, was "streamlit-navigation-bar-3.0.3.tar", last modified: Thu Apr  4 18:55:07 2024, max compression
```

## Comparing `streamlit-navigation-bar-3.0.2.tar` & `streamlit-navigation-bar-3.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-31 21:53:54.192427 streamlit-navigation-bar-3.0.2/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.0.2/LICENSE
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.0.2/MANIFEST.in
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13806 2024-03-31 21:53:54.192047 streamlit-navigation-bar-3.0.2/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13289 2024-03-30 21:12:54.000000 streamlit-navigation-bar-3.0.2/README.md
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-03-31 21:53:54.192493 streamlit-navigation-bar-3.0.2/setup.cfg
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      989 2024-03-31 21:52:37.000000 streamlit-navigation-bar-3.0.2/setup.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-31 21:53:54.188382 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    15968 2024-03-31 21:52:11.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/__init__.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8403 2024-03-21 18:46:33.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/errors.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-03-30 14:23:08.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/example.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-31 21:53:54.185973 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-31 21:53:54.189933 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-31 21:53:54.190589 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/assets/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1147 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/assets/index-31IBmtiW.css
--rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/assets/index-K06dADTk.js
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/index.html
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/match_navbar.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-31 21:53:54.189742 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13806 2024-03-31 21:53:54.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      605 2024-03-31 21:53:54.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-03-31 21:53:54.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-03-31 21:53:54.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/requires.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-03-31 21:53:54.000000 streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/top_level.txt
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.705165 streamlit-navigation-bar-3.0.3/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.0.3/LICENSE
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.0.3/MANIFEST.in
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13156 2024-04-04 18:55:07.704875 streamlit-navigation-bar-3.0.3/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    12639 2024-04-04 18:38:25.000000 streamlit-navigation-bar-3.0.3/README.md
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-04 18:55:07.705275 streamlit-navigation-bar-3.0.3/setup.cfg
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1024 2024-04-04 18:37:38.000000 streamlit-navigation-bar-3.0.3/setup.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.701203 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    15968 2024-03-31 21:52:11.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/__init__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8403 2024-03-21 18:46:33.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/errors.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-03-30 14:23:08.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/example.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.698053 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.702850 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.703605 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1147 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-31IBmtiW.css
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-K06dADTk.js
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/index.html
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/match_navbar.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.702652 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13156 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      605 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/requires.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/top_level.txt
```

### Comparing `streamlit-navigation-bar-3.0.2/LICENSE` & `streamlit-navigation-bar-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/PKG-INFO` & `streamlit-navigation-bar-3.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: streamlit-navigation-bar
-Version: 3.0.2
+Version: 3.0.3
 Summary: A component that allows you to place a navigation bar in your Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Downloads](https://static.pepy.tech/badge/streamlit-navigation-bar/month)](https://pepy.tech/project/streamlit-navigation-bar)
+
 # Streamlit Navigation Bar
 
 A component that allows you to place a navigation bar in your
 Streamlit app.
 
 [![Overview](https://github.com/gabrieltempass/streamlit-navigation-bar/raw/main/images/overview.gif)](https://st-navbar.streamlit.app/)
 
@@ -325,87 +327,41 @@
 [**[App]**](https://st-navbar-3.streamlit.app/) 
 [**[Source]**](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/examples/st_navbar_3/streamlit_app.py)
 
 ## Requirements
 
 To use the navigation bar component in your Streamlit app, you will need:
 * **Python >= 3.8**
-* **Streamlit >= 1.29.0 and <= 1.32.1**
+* **Streamlit >= 1.29.0 and != 1.32.2**
 * The CSS adjustment depends on the
-  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility).
+  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility)
 
 ## Roadmap
 
 The current version of the Streamlit Navigation Bar still has some limitations,
 that are planned to be addressed in future updates. Those are:
-* Be responsive on smaller screens.
-* Add dropdown navigation.
-* Accept ``.png`` and ``.jpg`` image formats for the logo.
+* Be responsive on smaller screens
+* Add dropdown navigation
+* Accept ``.png`` and ``.jpg`` image formats for the logo
 * Style ``:link`` and ``:visited`` pseudo-classes and any CSS property for
-``:hover``.
-* Select predefined themes to style the navbar.
-* Set light and dark mode styles for the navbar.
-* Apply a format function to the displayed pages.
-
-You are welcome to help develop these features and others. Below is a guide on
-how to quickstart the development.
-
-## Development
-
-Ensure you have [Python 3.8+](https://www.python.org/downloads/),
-[Node.js](https://nodejs.org) and
-[npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-installed.
-
-1. Clone this repository:
-``` bash
-git clone git@github.com:gabrieltempass/streamlit-navigation-bar.git
-```
-
-2. Go to the `frontend` directory and initialize and run the component template
-frontend:
-``` bash
-cd streamlit-navigation-bar/streamlit_navigation_bar/frontend
-```
-``` bash
-npm install
-npm run dev
-```
-
-3. From a separate terminal, go to the repository root directory, create a new
-Python virtual environment, activate it and install Streamlit,
-[st-theme](https://github.com/gabrieltempass/streamlit-theme) and the directory
-as an editable package:
-``` bash
-cd streamlit-navigation-bar
-```
-``` bash
-python3 -m venv venv
-. venv/bin/activate
-pip install streamlit
-pip install st-theme
-pip install -e .
-```
-
-Still from the same separate terminal, run the example Streamlit app:
-``` bash
-streamlit run streamlit_navigation_bar/example.py
-```
-
-If all goes well, you should see something like this:
-
-![Quickstart success](https://github.com/gabrieltempass/streamlit-navigation-bar/raw/main/images/development.png)
-
-Modify the frontend code at
-`streamlit_navigation_bar/frontend/src/StNavbar.vue`.
-Modify the Python code at `streamlit_navigation_bar/__init__.py`.
+``:hover``
+* Select predefined themes to style the navbar
+* Set light and dark mode styles for the navbar
+* Apply a format function to the displayed pages
+
+## Contributing
+
+You are welcome to help develop the Streamlit Navigation Bar! There are
+multiple ways to contribute, such as [reporting a bug](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml)
+or [requesting a feature](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml).
+You can also just [ask a question](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=question&projects=&template=ask_question.yml),
+if you want. To submit code for a pull request, make sure to read the [guide on how to contribute](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/CONTRIBUTING.md).
 
 ## References
 
 This Streamlit component is based on:
 * The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-repository, that uses Vue 3 to code the frontend and Vite to serve the files
-locally during development, as well as bundle and compile them for production.
+  repository, by [@gabrieltempass](https://github.com/gabrieltempass)
 * The [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu/tree/master)
-component, by [@victoryhb](https://github.com/victoryhb).
+  component, by [@victoryhb](https://github.com/victoryhb)
```

### Comparing `streamlit-navigation-bar-3.0.2/README.md` & `streamlit-navigation-bar-3.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Downloads](https://static.pepy.tech/badge/streamlit-navigation-bar/month)](https://pepy.tech/project/streamlit-navigation-bar)
+
 # Streamlit Navigation Bar
 
 A component that allows you to place a navigation bar in your
 Streamlit app.
 
 [![Overview](https://github.com/gabrieltempass/streamlit-navigation-bar/raw/main/images/overview.gif)](https://st-navbar.streamlit.app/)
 
@@ -310,85 +312,39 @@
 [**[App]**](https://st-navbar-3.streamlit.app/) 
 [**[Source]**](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/examples/st_navbar_3/streamlit_app.py)
 
 ## Requirements
 
 To use the navigation bar component in your Streamlit app, you will need:
 * **Python >= 3.8**
-* **Streamlit >= 1.29.0 and <= 1.32.1**
+* **Streamlit >= 1.29.0 and != 1.32.2**
 * The CSS adjustment depends on the
-  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility).
+  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility)
 
 ## Roadmap
 
 The current version of the Streamlit Navigation Bar still has some limitations,
 that are planned to be addressed in future updates. Those are:
-* Be responsive on smaller screens.
-* Add dropdown navigation.
-* Accept ``.png`` and ``.jpg`` image formats for the logo.
+* Be responsive on smaller screens
+* Add dropdown navigation
+* Accept ``.png`` and ``.jpg`` image formats for the logo
 * Style ``:link`` and ``:visited`` pseudo-classes and any CSS property for
-``:hover``.
-* Select predefined themes to style the navbar.
-* Set light and dark mode styles for the navbar.
-* Apply a format function to the displayed pages.
-
-You are welcome to help develop these features and others. Below is a guide on
-how to quickstart the development.
-
-## Development
-
-Ensure you have [Python 3.8+](https://www.python.org/downloads/),
-[Node.js](https://nodejs.org) and
-[npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-installed.
-
-1. Clone this repository:
-``` bash
-git clone git@github.com:gabrieltempass/streamlit-navigation-bar.git
-```
-
-2. Go to the `frontend` directory and initialize and run the component template
-frontend:
-``` bash
-cd streamlit-navigation-bar/streamlit_navigation_bar/frontend
-```
-``` bash
-npm install
-npm run dev
-```
-
-3. From a separate terminal, go to the repository root directory, create a new
-Python virtual environment, activate it and install Streamlit,
-[st-theme](https://github.com/gabrieltempass/streamlit-theme) and the directory
-as an editable package:
-``` bash
-cd streamlit-navigation-bar
-```
-``` bash
-python3 -m venv venv
-. venv/bin/activate
-pip install streamlit
-pip install st-theme
-pip install -e .
-```
-
-Still from the same separate terminal, run the example Streamlit app:
-``` bash
-streamlit run streamlit_navigation_bar/example.py
-```
-
-If all goes well, you should see something like this:
-
-![Quickstart success](https://github.com/gabrieltempass/streamlit-navigation-bar/raw/main/images/development.png)
-
-Modify the frontend code at
-`streamlit_navigation_bar/frontend/src/StNavbar.vue`.
-Modify the Python code at `streamlit_navigation_bar/__init__.py`.
+``:hover``
+* Select predefined themes to style the navbar
+* Set light and dark mode styles for the navbar
+* Apply a format function to the displayed pages
+
+## Contributing
+
+You are welcome to help develop the Streamlit Navigation Bar! There are
+multiple ways to contribute, such as [reporting a bug](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml)
+or [requesting a feature](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml).
+You can also just [ask a question](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=question&projects=&template=ask_question.yml),
+if you want. To submit code for a pull request, make sure to read the [guide on how to contribute](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/CONTRIBUTING.md).
 
 ## References
 
 This Streamlit component is based on:
 * The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-repository, that uses Vue 3 to code the frontend and Vite to serve the files
-locally during development, as well as bundle and compile them for production.
+  repository, by [@gabrieltempass](https://github.com/gabrieltempass)
 * The [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu/tree/master)
-component, by [@victoryhb](https://github.com/victoryhb).
+  component, by [@victoryhb](https://github.com/victoryhb)
```

### Comparing `streamlit-navigation-bar-3.0.2/setup.py` & `streamlit-navigation-bar-3.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="streamlit-navigation-bar",
-    version="3.0.2",
+    version="3.0.3",
     author="Gabriel Tem Pass",
     author_email="redo_hint_0x@icloud.com",
     description="A component that allows you to place a navigation bar in your Streamlit app.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gabrieltempass/streamlit-navigation-bar",
     packages=[
@@ -24,11 +24,11 @@
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires=">=3.8",
     install_requires=[
-        "streamlit >= 1.29.0, <= 1.32.1",
+        "streamlit >= 1.29.0, != 1.32.2",  # Navbar doesn't work with 1.32.2
         "st-theme >= 1.2.2",
     ],
 )
```

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/__init__.py` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/errors.py` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/example.py` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/example.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/assets/index-31IBmtiW.css` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-31IBmtiW.css`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/assets/index-K06dADTk.js` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-K06dADTk.js`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/frontend/dist/index.html` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar/match_navbar.py` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/match_navbar.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/PKG-INFO` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: streamlit-navigation-bar
-Version: 3.0.2
+Version: 3.0.3
 Summary: A component that allows you to place a navigation bar in your Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Downloads](https://static.pepy.tech/badge/streamlit-navigation-bar/month)](https://pepy.tech/project/streamlit-navigation-bar)
+
 # Streamlit Navigation Bar
 
 A component that allows you to place a navigation bar in your
 Streamlit app.
 
 [![Overview](https://github.com/gabrieltempass/streamlit-navigation-bar/raw/main/images/overview.gif)](https://st-navbar.streamlit.app/)
 
@@ -325,87 +327,41 @@
 [**[App]**](https://st-navbar-3.streamlit.app/) 
 [**[Source]**](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/examples/st_navbar_3/streamlit_app.py)
 
 ## Requirements
 
 To use the navigation bar component in your Streamlit app, you will need:
 * **Python >= 3.8**
-* **Streamlit >= 1.29.0 and <= 1.32.1**
+* **Streamlit >= 1.29.0 and != 1.32.2**
 * The CSS adjustment depends on the
-  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility).
+  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility)
 
 ## Roadmap
 
 The current version of the Streamlit Navigation Bar still has some limitations,
 that are planned to be addressed in future updates. Those are:
-* Be responsive on smaller screens.
-* Add dropdown navigation.
-* Accept ``.png`` and ``.jpg`` image formats for the logo.
+* Be responsive on smaller screens
+* Add dropdown navigation
+* Accept ``.png`` and ``.jpg`` image formats for the logo
 * Style ``:link`` and ``:visited`` pseudo-classes and any CSS property for
-``:hover``.
-* Select predefined themes to style the navbar.
-* Set light and dark mode styles for the navbar.
-* Apply a format function to the displayed pages.
-
-You are welcome to help develop these features and others. Below is a guide on
-how to quickstart the development.
-
-## Development
-
-Ensure you have [Python 3.8+](https://www.python.org/downloads/),
-[Node.js](https://nodejs.org) and
-[npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-installed.
-
-1. Clone this repository:
-``` bash
-git clone git@github.com:gabrieltempass/streamlit-navigation-bar.git
-```
-
-2. Go to the `frontend` directory and initialize and run the component template
-frontend:
-``` bash
-cd streamlit-navigation-bar/streamlit_navigation_bar/frontend
-```
-``` bash
-npm install
-npm run dev
-```
-
-3. From a separate terminal, go to the repository root directory, create a new
-Python virtual environment, activate it and install Streamlit,
-[st-theme](https://github.com/gabrieltempass/streamlit-theme) and the directory
-as an editable package:
-``` bash
-cd streamlit-navigation-bar
-```
-``` bash
-python3 -m venv venv
-. venv/bin/activate
-pip install streamlit
-pip install st-theme
-pip install -e .
-```
-
-Still from the same separate terminal, run the example Streamlit app:
-``` bash
-streamlit run streamlit_navigation_bar/example.py
-```
-
-If all goes well, you should see something like this:
-
-![Quickstart success](https://github.com/gabrieltempass/streamlit-navigation-bar/raw/main/images/development.png)
-
-Modify the frontend code at
-`streamlit_navigation_bar/frontend/src/StNavbar.vue`.
-Modify the Python code at `streamlit_navigation_bar/__init__.py`.
+``:hover``
+* Select predefined themes to style the navbar
+* Set light and dark mode styles for the navbar
+* Apply a format function to the displayed pages
+
+## Contributing
+
+You are welcome to help develop the Streamlit Navigation Bar! There are
+multiple ways to contribute, such as [reporting a bug](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml)
+or [requesting a feature](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml).
+You can also just [ask a question](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=question&projects=&template=ask_question.yml),
+if you want. To submit code for a pull request, make sure to read the [guide on how to contribute](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/CONTRIBUTING.md).
 
 ## References
 
 This Streamlit component is based on:
 * The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-repository, that uses Vue 3 to code the frontend and Vite to serve the files
-locally during development, as well as bundle and compile them for production.
+  repository, by [@gabrieltempass](https://github.com/gabrieltempass)
 * The [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu/tree/master)
-component, by [@victoryhb](https://github.com/victoryhb).
+  component, by [@victoryhb](https://github.com/victoryhb)
```

### Comparing `streamlit-navigation-bar-3.0.2/streamlit_navigation_bar.egg-info/SOURCES.txt` & `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

