# Comparing `tmp/fstrider-0.1.19.tar.gz` & `tmp/fstrider-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstrider-0.1.19.tar", last modified: Fri Mar 29 11:42:19 2024, max compression
+gzip compressed data, was "fstrider-0.1.20.tar", last modified: Thu Apr  4 13:32:05 2024, max compression
```

## Comparing `fstrider-0.1.19.tar` & `fstrider-0.1.20.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:42:19.595535 fstrider-0.1.19/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-29 11:42:15.000000 fstrider-0.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-03-29 11:42:19.595535 fstrider-0.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-03-29 11:42:15.000000 fstrider-0.1.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:42:19.595535 fstrider-0.1.19/fstrider/
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/fs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/fstrider
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/fstrider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/os.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-29 11:42:15.000000 fstrider-0.1.19/fstrider/ptk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:42:19.595535 fstrider-0.1.19/fstrider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-03-29 11:42:19.000000 fstrider-0.1.19/fstrider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-29 11:42:19.000000 fstrider-0.1.19/fstrider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 11:42:19.000000 fstrider-0.1.19/fstrider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-29 11:42:19.000000 fstrider-0.1.19/fstrider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-29 11:42:19.000000 fstrider-0.1.19/fstrider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-29 11:42:15.000000 fstrider-0.1.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 11:42:19.595535 fstrider-0.1.19/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:42:19.595535 fstrider-0.1.19/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-29 11:42:15.000000 fstrider-0.1.19/tests/test_fstrider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:42:19.595535 fstrider-0.1.19/xontrib/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-29 11:42:15.000000 fstrider-0.1.19/xontrib/fstrider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 13:32:00.000000 fstrider-0.1.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-04 13:32:05.049124 fstrider-0.1.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-04 13:32:00.000000 fstrider-0.1.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/fstrider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/fs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/fstrider
+-rw-r--r--   0 runner    (1001) docker     (127)    23859 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/fstrider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/ptk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/fstrider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 13:32:00.000000 fstrider-0.1.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:32:05.049124 fstrider-0.1.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-04 13:32:00.000000 fstrider-0.1.20/tests/test_fstrider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-04 13:32:00.000000 fstrider-0.1.20/xontrib/fstrider.py
```

### Comparing `fstrider-0.1.19/LICENSE` & `fstrider-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.19/PKG-INFO` & `fstrider-0.1.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstrider
-Version: 0.1.19
+Version: 0.1.20
 Summary: Library of the useful macroses for the xonsh shell.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,21 +88,21 @@
 
 Basic:
 
 * <kbd>Left</kbd> - move to parent directory.
 * <kbd>Right</kbd> - move to the selected directory.
 * <kbd>Space</kbd> - open menu for the current file or directory.
 * <kbd>Enter</kbd> - open file or directory using OS associations.
-* <kbd>Esc</kbd> - quit.
+* <kbd>Control q</kbd> - quit.
 
 Additional:
 
-* <kbd>Shift ~</kbd> - jump to the home directoy.
-* <kbd>Control j</kbd> - jump to path. You can jump into new path and then create it.
+* <kbd>Shift ~</kbd> - jump to the home directory.
 * <kbd>Control h</kbd> - jump to directory from history.
+* <kbd>Control j</kbd> - jump to path. You can jump into new path and then create it.
 * <kbd>Control +</kbd> - copy path to the current directory.
 
 Midnight Commander bindings: <kbd>F5</kbd> copy, <kbd>F6</kbd> move, <kbd>F7</kbd> rename, <kbd>F8</kbd> delete, <kbd>F10</kbd> quit, <kbd>F12</kbd> open with.
 
 ### Using `/` when copying or moving.
 
 fstrider was created to reduce keystrokes. So remember two things:
@@ -145,46 +145,51 @@
 Xonsh xontrib
     ++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18)
     ++ Run fstrider as fast as possible. (0.1.18)
     ++ Keeps history between running fstrider. (0.1.18)
 
 List
     ++ Async monitoring of the list and update if new files created. (0.1.19)
+    ++Add `/` to the end of directory in title and in history.
     
 Configuration
     ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
 
 Integration
     "=" to move object from path to the current dir.
 
 Tech
+    ++ Add list and menu mode.
     Errors processing
         Show errors like in case of exception.
         Process `File exists` error.
     ++ Resolve `/tmp/../../`. (0.1.17)
     Symlinks: copying, moving   
     
+    
 Style
     Grey style for copy/move and red style for delete dialogue. 
     
 Navigation
+    Move coursor to the next file after deletion.
     ++ Up key at first option moves cursor to end. (0.1.19)
-    Fix left key when go from history.    
-    Fix right key when go to file from history.
+    ++ Fix left key when go from history.    
+    ++ Fix right key when go to file from history.
 ```
 
 ### v0.3.0
 
 ```
 Navigation
     Go back to previous directory after moving or copying.
     
 List
     Sorting by size/date `sorted(glob.glob('*.png'), key=os.path.getsize)`.
     Modes: short, full (chmod/chown/date). 
+    Keep file msg after `invalidate_list`.
 
 Jump
     Use path from clipboard e.g. `text_area.buffer.paste_clipboard_data`.
     Use directories from xonsh history i.e. `__xonsh__.history[-1].cwd`
 ```
 
 ### v0.4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fstrider Version: 0.1.19 Summary: Library of the
+Metadata-Version: 2.1 Name: fstrider Version: 0.1.20 Summary: Library of the
 useful macroses for the xonsh shell. Author-email: anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -35,69 +35,72 @@
 and directories. Install or update: ```xsh pip install fstrider # OR: pip
 install -U git+https://github.com/anki-code/fstrider ``` ## Usage Run fstrider
 and start striding: ```xsh fstrider ``` In the xonsh shell you can load xontrib
 with `s` alias that works fast and allows to change directory using fstrider:
 ```xsh xontrib load fstrider fs # or fstrider ``` ### Key bindings Basic: *
 Left - move to parent directory. * Right - move to the selected directory. *
 Space - open menu for the current file or directory. * Enter - open file or
-directory using OS associations. * Esc - quit. Additional: * Shift ~ - jump to
-the home directoy. * Control j - jump to path. You can jump into new path and
-then create it. * Control h - jump to directory from history. * Control + -
-copy path to the current directory. Midnight Commander bindings: F5 copy, F6
-move, F7 rename, F8 delete, F10 quit, F12 open with. ### Using `/` when copying
-or moving. fstrider was created to reduce keystrokes. So remember two things: *
-Any new path will be created automatically. When you copy the file
-`example.txt` to `/tmp/some/new/path/` the path `/tmp/some/new/path/` will be
-created automatically. * If you copy directory `/tmp/dir1` and the target path
-ends with `/` e.g. `/tmp/other/` then the `dir1` will be putted into `/tmp/
-other/dir`. * If you copy directory `/tmp/dir2` and the target path ends with
-directory name e.g. `/tmp/other` then the `dir2` will be merged with `/tmp/
-other`. Existing files will be overwritten. ## Xonsh xontrib fstrider xontrib
-features: * Creates alias `fs` (or `fstrider` if `fs` exists). * Run fstrider
-as fast as possible. * Keeps history between running fstrider. Environment
-variables for fstrider xontrib: * `$XONTRIB_FSTRIDER_ALIAS` - change the alias
-name. Recommended `s`. ## Options * `'show_symlink_paths': True` - show
-symlinks in the list. * `'keys_midnight_commander': True` - use Midnight
-Commander keys. * `'monitor_state': False` - Async monitoring of the list and
-update if new files created. * `'os_path_change': True` - change os path in
-xonsh shell. * `'app_associations_save_file': False` - save filename to apps
-associations. You can change the option state by setting environment variable
-e.g. `$FSTRIDER_MONITOR_STATE=True`. ## Known issues ### Tested only on Mac OS
-Current version of fstrider is using and testing on Mac OS. It will be good to
-test and fix for Linux and Windows. ## Roadmap Feel free to grab and implement
-or propose new feature. PR is welcome! ### v0.2.0 ``` Xonsh xontrib ++ Creates
-alias `fs` (or `fstrider` if `fs` exists). (0.1.18) ++ Run fstrider as fast as
-possible. (0.1.18) ++ Keeps history between running fstrider. (0.1.18) List ++
-Async monitoring of the list and update if new files created. (0.1.19)
+directory using OS associations. * Control q - quit. Additional: * Shift ~ -
+jump to the home directory. * Control h - jump to directory from history. *
+Control j - jump to path. You can jump into new path and then create it. *
+Control + - copy path to the current directory. Midnight Commander bindings: F5
+copy, F6 move, F7 rename, F8 delete, F10 quit, F12 open with. ### Using `/
+` when copying or moving. fstrider was created to reduce keystrokes. So
+remember two things: * Any new path will be created automatically. When you
+copy the file `example.txt` to `/tmp/some/new/path/` the path `/tmp/some/new/
+path/` will be created automatically. * If you copy directory `/tmp/dir1` and
+the target path ends with `/` e.g. `/tmp/other/` then the `dir1` will be putted
+into `/tmp/other/dir`. * If you copy directory `/tmp/dir2` and the target path
+ends with directory name e.g. `/tmp/other` then the `dir2` will be merged with
+`/tmp/other`. Existing files will be overwritten. ## Xonsh xontrib fstrider
+xontrib features: * Creates alias `fs` (or `fstrider` if `fs` exists). * Run
+fstrider as fast as possible. * Keeps history between running fstrider.
+Environment variables for fstrider xontrib: * `$XONTRIB_FSTRIDER_ALIAS` -
+change the alias name. Recommended `s`. ## Options * `'show_symlink_paths':
+True` - show symlinks in the list. * `'keys_midnight_commander': True` - use
+Midnight Commander keys. * `'monitor_state': False` - Async monitoring of the
+list and update if new files created. * `'os_path_change': True` - change os
+path in xonsh shell. * `'app_associations_save_file': False` - save filename to
+apps associations. You can change the option state by setting environment
+variable e.g. `$FSTRIDER_MONITOR_STATE=True`. ## Known issues ### Tested only
+on Mac OS Current version of fstrider is using and testing on Mac OS. It will
+be good to test and fix for Linux and Windows. ## Roadmap Feel free to grab and
+implement or propose new feature. PR is welcome! ### v0.2.0 ``` Xonsh xontrib
+++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18) ++ Run fstrider
+as fast as possible. (0.1.18) ++ Keeps history between running fstrider.
+(0.1.18) List ++ Async monitoring of the list and update if new files created.
+(0.1.19) ++Add `/` to the end of directory in title and in history.
 Configuration ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
-Integration "=" to move object from path to the current dir. Tech Errors
-processing Show errors like in case of exception. Process `File exists` error.
-++ Resolve `/tmp/../../`. (0.1.17) Symlinks: copying, moving Style Grey style
-for copy/move and red style for delete dialogue. Navigation ++ Up key at first
-option moves cursor to end. (0.1.19) Fix left key when go from history. Fix
-right key when go to file from history. ``` ### v0.3.0 ``` Navigation Go back
-to previous directory after moving or copying. List Sorting by size/date
+Integration "=" to move object from path to the current dir. Tech ++ Add list
+and menu mode. Errors processing Show errors like in case of exception. Process
+`File exists` error. ++ Resolve `/tmp/../../`. (0.1.17) Symlinks: copying,
+moving Style Grey style for copy/move and red style for delete dialogue.
+Navigation Move coursor to the next file after deletion. ++ Up key at first
+option moves cursor to end. (0.1.19) ++ Fix left key when go from history. ++
+Fix right key when go to file from history. ``` ### v0.3.0 ``` Navigation Go
+back to previous directory after moving or copying. List Sorting by size/date
 `sorted(glob.glob('*.png'), key=os.path.getsize)`. Modes: short, full (chmod/
-chown/date). Jump Use path from clipboard e.g.
-`text_area.buffer.paste_clipboard_data`. Use directories from xonsh history
-i.e. `__xonsh__.history[-1].cwd` ``` ### v0.4.0 ``` Title Show chown/chmod if
-"Access denied". Show what part of path is exist and what's new. Dialog
-Autocomplete for paths in menu - the feature from prompt-toolkit. Copying
-progress bar or just the console log from `rsync`. ``` ### v0.5.0 ``` List
-Fuzzy search. Research: Draggable items i.e. `ls --hyperlink`. Associations
-`.xonshrc` case in app_assoc. Highlight known suffix from app_assoc. Using
-$LS_COLORS and `dircolors` for color files. ``` ### v0.6.0 ``` List Improve
-speed of list on big amount of items - 10k+ ``` ### Waiting for community ```
-Integration Other shells support. Key bindings The way to change key bindings.
-VI mode, Emacs mode. Style Dark style. ``` ### Ideas for future ``` List Fake
-files (items in the list) Fake deleted file to show that this file was deleted.
-Interstellar wormhole - path to another path added to this directory. Read the
-path from files in this directory. Colors and gradient: by time, by size. Show
-old files with dark color. Show small files with dark color. Integration
-Catching pasting path from clipboard and ask actions: cd-ing, copy/move from,
-open. Using fstrider for anything e.g. striding around aws s3 bucket, ssh host.
-The way to setup fstrider for special needs: colors, menus, hotkeys. Keys Free
-keys to use: `/`, `-`. Xonsh shell Using xonsh shell history to jump into
-directories. Run shell command in this directory. Crazy: use xonsh prompt as a
-prompt for ptk `TextArea` AI Predict the next choice of path based on history
-and maybe files in dir. ``` ## Good to know * Copy the current path in MacOS
-Finder: Option Command C * Jump to path in MacOS Finder: Command Shift G
+chown/date). Keep file msg after `invalidate_list`. Jump Use path from
+clipboard e.g. `text_area.buffer.paste_clipboard_data`. Use directories from
+xonsh history i.e. `__xonsh__.history[-1].cwd` ``` ### v0.4.0 ``` Title Show
+chown/chmod if "Access denied". Show what part of path is exist and what's new.
+Dialog Autocomplete for paths in menu - the feature from prompt-toolkit.
+Copying progress bar or just the console log from `rsync`. ``` ### v0.5.0 ```
+List Fuzzy search. Research: Draggable items i.e. `ls --hyperlink`.
+Associations `.xonshrc` case in app_assoc. Highlight known suffix from
+app_assoc. Using $LS_COLORS and `dircolors` for color files. ``` ### v0.6.0 ```
+List Improve speed of list on big amount of items - 10k+ ``` ### Waiting for
+community ``` Integration Other shells support. Key bindings The way to change
+key bindings. VI mode, Emacs mode. Style Dark style. ``` ### Ideas for future
+``` List Fake files (items in the list) Fake deleted file to show that this
+file was deleted. Interstellar wormhole - path to another path added to this
+directory. Read the path from files in this directory. Colors and gradient: by
+time, by size. Show old files with dark color. Show small files with dark
+color. Integration Catching pasting path from clipboard and ask actions: cd-
+ing, copy/move from, open. Using fstrider for anything e.g. striding around aws
+s3 bucket, ssh host. The way to setup fstrider for special needs: colors,
+menus, hotkeys. Keys Free keys to use: `/`, `-`. Xonsh shell Using xonsh shell
+history to jump into directories. Run shell command in this directory. Crazy:
+use xonsh prompt as a prompt for ptk `TextArea` AI Predict the next choice of
+path based on history and maybe files in dir. ``` ## Good to know * Copy the
+current path in MacOS Finder: Option Command C * Jump to path in MacOS Finder:
+Command Shift G
```

### Comparing `fstrider-0.1.19/README.md` & `fstrider-0.1.20/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,21 +44,21 @@
 
 Basic:
 
 * <kbd>Left</kbd> - move to parent directory.
 * <kbd>Right</kbd> - move to the selected directory.
 * <kbd>Space</kbd> - open menu for the current file or directory.
 * <kbd>Enter</kbd> - open file or directory using OS associations.
-* <kbd>Esc</kbd> - quit.
+* <kbd>Control q</kbd> - quit.
 
 Additional:
 
-* <kbd>Shift ~</kbd> - jump to the home directoy.
-* <kbd>Control j</kbd> - jump to path. You can jump into new path and then create it.
+* <kbd>Shift ~</kbd> - jump to the home directory.
 * <kbd>Control h</kbd> - jump to directory from history.
+* <kbd>Control j</kbd> - jump to path. You can jump into new path and then create it.
 * <kbd>Control +</kbd> - copy path to the current directory.
 
 Midnight Commander bindings: <kbd>F5</kbd> copy, <kbd>F6</kbd> move, <kbd>F7</kbd> rename, <kbd>F8</kbd> delete, <kbd>F10</kbd> quit, <kbd>F12</kbd> open with.
 
 ### Using `/` when copying or moving.
 
 fstrider was created to reduce keystrokes. So remember two things:
@@ -101,46 +101,51 @@
 Xonsh xontrib
     ++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18)
     ++ Run fstrider as fast as possible. (0.1.18)
     ++ Keeps history between running fstrider. (0.1.18)
 
 List
     ++ Async monitoring of the list and update if new files created. (0.1.19)
+    ++Add `/` to the end of directory in title and in history.
     
 Configuration
     ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
 
 Integration
     "=" to move object from path to the current dir.
 
 Tech
+    ++ Add list and menu mode.
     Errors processing
         Show errors like in case of exception.
         Process `File exists` error.
     ++ Resolve `/tmp/../../`. (0.1.17)
     Symlinks: copying, moving   
     
+    
 Style
     Grey style for copy/move and red style for delete dialogue. 
     
 Navigation
+    Move coursor to the next file after deletion.
     ++ Up key at first option moves cursor to end. (0.1.19)
-    Fix left key when go from history.    
-    Fix right key when go to file from history.
+    ++ Fix left key when go from history.    
+    ++ Fix right key when go to file from history.
 ```
 
 ### v0.3.0
 
 ```
 Navigation
     Go back to previous directory after moving or copying.
     
 List
     Sorting by size/date `sorted(glob.glob('*.png'), key=os.path.getsize)`.
     Modes: short, full (chmod/chown/date). 
+    Keep file msg after `invalidate_list`.
 
 Jump
     Use path from clipboard e.g. `text_area.buffer.paste_clipboard_data`.
     Use directories from xonsh history i.e. `__xonsh__.history[-1].cwd`
 ```
 
 ### v0.4.0
```

#### html2text {}

```diff
@@ -9,69 +9,72 @@
 and directories. Install or update: ```xsh pip install fstrider # OR: pip
 install -U git+https://github.com/anki-code/fstrider ``` ## Usage Run fstrider
 and start striding: ```xsh fstrider ``` In the xonsh shell you can load xontrib
 with `s` alias that works fast and allows to change directory using fstrider:
 ```xsh xontrib load fstrider fs # or fstrider ``` ### Key bindings Basic: *
 Left - move to parent directory. * Right - move to the selected directory. *
 Space - open menu for the current file or directory. * Enter - open file or
-directory using OS associations. * Esc - quit. Additional: * Shift ~ - jump to
-the home directoy. * Control j - jump to path. You can jump into new path and
-then create it. * Control h - jump to directory from history. * Control + -
-copy path to the current directory. Midnight Commander bindings: F5 copy, F6
-move, F7 rename, F8 delete, F10 quit, F12 open with. ### Using `/` when copying
-or moving. fstrider was created to reduce keystrokes. So remember two things: *
-Any new path will be created automatically. When you copy the file
-`example.txt` to `/tmp/some/new/path/` the path `/tmp/some/new/path/` will be
-created automatically. * If you copy directory `/tmp/dir1` and the target path
-ends with `/` e.g. `/tmp/other/` then the `dir1` will be putted into `/tmp/
-other/dir`. * If you copy directory `/tmp/dir2` and the target path ends with
-directory name e.g. `/tmp/other` then the `dir2` will be merged with `/tmp/
-other`. Existing files will be overwritten. ## Xonsh xontrib fstrider xontrib
-features: * Creates alias `fs` (or `fstrider` if `fs` exists). * Run fstrider
-as fast as possible. * Keeps history between running fstrider. Environment
-variables for fstrider xontrib: * `$XONTRIB_FSTRIDER_ALIAS` - change the alias
-name. Recommended `s`. ## Options * `'show_symlink_paths': True` - show
-symlinks in the list. * `'keys_midnight_commander': True` - use Midnight
-Commander keys. * `'monitor_state': False` - Async monitoring of the list and
-update if new files created. * `'os_path_change': True` - change os path in
-xonsh shell. * `'app_associations_save_file': False` - save filename to apps
-associations. You can change the option state by setting environment variable
-e.g. `$FSTRIDER_MONITOR_STATE=True`. ## Known issues ### Tested only on Mac OS
-Current version of fstrider is using and testing on Mac OS. It will be good to
-test and fix for Linux and Windows. ## Roadmap Feel free to grab and implement
-or propose new feature. PR is welcome! ### v0.2.0 ``` Xonsh xontrib ++ Creates
-alias `fs` (or `fstrider` if `fs` exists). (0.1.18) ++ Run fstrider as fast as
-possible. (0.1.18) ++ Keeps history between running fstrider. (0.1.18) List ++
-Async monitoring of the list and update if new files created. (0.1.19)
+directory using OS associations. * Control q - quit. Additional: * Shift ~ -
+jump to the home directory. * Control h - jump to directory from history. *
+Control j - jump to path. You can jump into new path and then create it. *
+Control + - copy path to the current directory. Midnight Commander bindings: F5
+copy, F6 move, F7 rename, F8 delete, F10 quit, F12 open with. ### Using `/
+` when copying or moving. fstrider was created to reduce keystrokes. So
+remember two things: * Any new path will be created automatically. When you
+copy the file `example.txt` to `/tmp/some/new/path/` the path `/tmp/some/new/
+path/` will be created automatically. * If you copy directory `/tmp/dir1` and
+the target path ends with `/` e.g. `/tmp/other/` then the `dir1` will be putted
+into `/tmp/other/dir`. * If you copy directory `/tmp/dir2` and the target path
+ends with directory name e.g. `/tmp/other` then the `dir2` will be merged with
+`/tmp/other`. Existing files will be overwritten. ## Xonsh xontrib fstrider
+xontrib features: * Creates alias `fs` (or `fstrider` if `fs` exists). * Run
+fstrider as fast as possible. * Keeps history between running fstrider.
+Environment variables for fstrider xontrib: * `$XONTRIB_FSTRIDER_ALIAS` -
+change the alias name. Recommended `s`. ## Options * `'show_symlink_paths':
+True` - show symlinks in the list. * `'keys_midnight_commander': True` - use
+Midnight Commander keys. * `'monitor_state': False` - Async monitoring of the
+list and update if new files created. * `'os_path_change': True` - change os
+path in xonsh shell. * `'app_associations_save_file': False` - save filename to
+apps associations. You can change the option state by setting environment
+variable e.g. `$FSTRIDER_MONITOR_STATE=True`. ## Known issues ### Tested only
+on Mac OS Current version of fstrider is using and testing on Mac OS. It will
+be good to test and fix for Linux and Windows. ## Roadmap Feel free to grab and
+implement or propose new feature. PR is welcome! ### v0.2.0 ``` Xonsh xontrib
+++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18) ++ Run fstrider
+as fast as possible. (0.1.18) ++ Keeps history between running fstrider.
+(0.1.18) List ++ Async monitoring of the list and update if new files created.
+(0.1.19) ++Add `/` to the end of directory in title and in history.
 Configuration ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
-Integration "=" to move object from path to the current dir. Tech Errors
-processing Show errors like in case of exception. Process `File exists` error.
-++ Resolve `/tmp/../../`. (0.1.17) Symlinks: copying, moving Style Grey style
-for copy/move and red style for delete dialogue. Navigation ++ Up key at first
-option moves cursor to end. (0.1.19) Fix left key when go from history. Fix
-right key when go to file from history. ``` ### v0.3.0 ``` Navigation Go back
-to previous directory after moving or copying. List Sorting by size/date
+Integration "=" to move object from path to the current dir. Tech ++ Add list
+and menu mode. Errors processing Show errors like in case of exception. Process
+`File exists` error. ++ Resolve `/tmp/../../`. (0.1.17) Symlinks: copying,
+moving Style Grey style for copy/move and red style for delete dialogue.
+Navigation Move coursor to the next file after deletion. ++ Up key at first
+option moves cursor to end. (0.1.19) ++ Fix left key when go from history. ++
+Fix right key when go to file from history. ``` ### v0.3.0 ``` Navigation Go
+back to previous directory after moving or copying. List Sorting by size/date
 `sorted(glob.glob('*.png'), key=os.path.getsize)`. Modes: short, full (chmod/
-chown/date). Jump Use path from clipboard e.g.
-`text_area.buffer.paste_clipboard_data`. Use directories from xonsh history
-i.e. `__xonsh__.history[-1].cwd` ``` ### v0.4.0 ``` Title Show chown/chmod if
-"Access denied". Show what part of path is exist and what's new. Dialog
-Autocomplete for paths in menu - the feature from prompt-toolkit. Copying
-progress bar or just the console log from `rsync`. ``` ### v0.5.0 ``` List
-Fuzzy search. Research: Draggable items i.e. `ls --hyperlink`. Associations
-`.xonshrc` case in app_assoc. Highlight known suffix from app_assoc. Using
-$LS_COLORS and `dircolors` for color files. ``` ### v0.6.0 ``` List Improve
-speed of list on big amount of items - 10k+ ``` ### Waiting for community ```
-Integration Other shells support. Key bindings The way to change key bindings.
-VI mode, Emacs mode. Style Dark style. ``` ### Ideas for future ``` List Fake
-files (items in the list) Fake deleted file to show that this file was deleted.
-Interstellar wormhole - path to another path added to this directory. Read the
-path from files in this directory. Colors and gradient: by time, by size. Show
-old files with dark color. Show small files with dark color. Integration
-Catching pasting path from clipboard and ask actions: cd-ing, copy/move from,
-open. Using fstrider for anything e.g. striding around aws s3 bucket, ssh host.
-The way to setup fstrider for special needs: colors, menus, hotkeys. Keys Free
-keys to use: `/`, `-`. Xonsh shell Using xonsh shell history to jump into
-directories. Run shell command in this directory. Crazy: use xonsh prompt as a
-prompt for ptk `TextArea` AI Predict the next choice of path based on history
-and maybe files in dir. ``` ## Good to know * Copy the current path in MacOS
-Finder: Option Command C * Jump to path in MacOS Finder: Command Shift G
+chown/date). Keep file msg after `invalidate_list`. Jump Use path from
+clipboard e.g. `text_area.buffer.paste_clipboard_data`. Use directories from
+xonsh history i.e. `__xonsh__.history[-1].cwd` ``` ### v0.4.0 ``` Title Show
+chown/chmod if "Access denied". Show what part of path is exist and what's new.
+Dialog Autocomplete for paths in menu - the feature from prompt-toolkit.
+Copying progress bar or just the console log from `rsync`. ``` ### v0.5.0 ```
+List Fuzzy search. Research: Draggable items i.e. `ls --hyperlink`.
+Associations `.xonshrc` case in app_assoc. Highlight known suffix from
+app_assoc. Using $LS_COLORS and `dircolors` for color files. ``` ### v0.6.0 ```
+List Improve speed of list on big amount of items - 10k+ ``` ### Waiting for
+community ``` Integration Other shells support. Key bindings The way to change
+key bindings. VI mode, Emacs mode. Style Dark style. ``` ### Ideas for future
+``` List Fake files (items in the list) Fake deleted file to show that this
+file was deleted. Interstellar wormhole - path to another path added to this
+directory. Read the path from files in this directory. Colors and gradient: by
+time, by size. Show old files with dark color. Show small files with dark
+color. Integration Catching pasting path from clipboard and ask actions: cd-
+ing, copy/move from, open. Using fstrider for anything e.g. striding around aws
+s3 bucket, ssh host. The way to setup fstrider for special needs: colors,
+menus, hotkeys. Keys Free keys to use: `/`, `-`. Xonsh shell Using xonsh shell
+history to jump into directories. Run shell command in this directory. Crazy:
+use xonsh prompt as a prompt for ptk `TextArea` AI Predict the next choice of
+path based on history and maybe files in dir. ``` ## Good to know * Copy the
+current path in MacOS Finder: Option Command C * Jump to path in MacOS Finder:
+Command Shift G
```

### Comparing `fstrider-0.1.19/fstrider/__init__.py` & `fstrider-0.1.20/fstrider/__init__.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.19/fstrider/fs.py` & `fstrider-0.1.20/fstrider/fs.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.19/fstrider/fstrider.py` & `fstrider-0.1.20/fstrider/fstrider.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         'app_associations_save_file': False,
         'keys_midnight_commander': True,
         'monitor_state': False,
     }
 
     def __init__(self, current_path = None):
         self.title = Label('Welcome to fstrider!')
+        self.mode = 'list'
         self.history = []
 
         current_path = '.' if current_path is None else current_path
         self.current_path = Path(current_path).absolute()
         self.list = self.create_list()
 
         self._app_associations_file = '/tmp/strider_app_associations_file.json'
@@ -124,16 +125,17 @@
         # except:
         #     pass
 
         return style
 
     @staticmethod
     def format_path_accent(p : Path, color='grey'):
+        is_root = str(p) == '/'
         return f'<style fg="{color}">' + (html.escape(str(p.parent)) if str(p.parent) != '/' else '') \
-                + '/' + f'</style><style fg="{color}"><b>' + html.escape(p.name) + '</b></style>'
+                + '/' + f'</style><style fg="{color}"><b>' + html.escape(p.name) + ('/' if p.is_dir() and not is_root else '') + '</b></style>'
 
     def set_title(self, p: Path, msg=None):
         """Set the main title."""
         at = access_type(p)
         if 'noaccess' in at:
             color = 'red'
             if not msg:
@@ -147,22 +149,27 @@
 
         if msg:
             txt += f'<style fg="grey"> - {html.escape(msg)}</style>'
 
         self.title.text = HTML(txt)
 
     async def invalidate_list(self):
+        prev_p = self.current_path
         prev_list = itertools.islice(Path(self.current_path).glob('*'), 100)
         while True:
-            curr_list = itertools.islice(Path(self.current_path).glob('*'), 100)
-            if curr_list != prev_list:
-                self.update_list(selected_by_value=self.list.get_selected_value(), file_msg={p: 'Modified' for p in curr_list if time()-p.lstat().st_mtime < 30})
-                prev_list = curr_list
+            if self.mode == 'list':
+                curr_p = self.current_path
+                curr_list = itertools.islice(Path(self.current_path).glob('*'), 100)
+
+                if curr_p == prev_p and curr_list != prev_list:
+                    self.update_list(selected_by_value=self.list.get_selected_value(), file_msg={p: 'Modified' for p in curr_list if time()-p.lstat().st_mtime < 30 and p not in prev_list})
+                    prev_list = curr_list
+                    prev_p = curr_p
 
-            self.app.invalidate()
+                self.app.invalidate()
             await asyncio.sleep(1)
 
     def create_list(self):
         """Create the main list."""
         default = None
         radio_list = StriderRadioList([('', '')], default)
         radio_list.open_character = radio_list.close_character = ''
@@ -182,44 +189,52 @@
             if radio_list._selected_index == len(radio_list.values) - 1:
                 radio_list._selected_index = 0
             else:
                 radio_list._selected_index = min(len(radio_list.values) - 1, radio_list._selected_index + 1)
 
         @radio_list.control.key_bindings.add("left")
         def _list_left(event):
-            self.stride(self.current_path.parent)
+            if self.mode in ('list', 'menu'):
+                self.stride(self.current_path.parent, selected_by_value=self.current_path)
+            elif self.mode in ('history'):
+                self.stride(self.current_path, selected_by_value=self.current_path)
 
         @radio_list.control.key_bindings.add("enter")
         def _list_enter(event):
             radio_list._handle_enter()
+
+            if type(self.list.current_value) is pathlib.PosixPath:
+                self.history_append(self.list.current_value)
+
             selected_item = radio_list.current_value
+
             if type(selected_item) is pathlib.PosixPath:
                 self.stride(selected_by_value=radio_list.current_value, file_msg={radio_list.current_value: 'Open with OS'})
                 open_in_os(radio_list.current_value)
             elif callable(selected_item):
                 selected_item(self.current_path)
 
         @radio_list.control.key_bindings.add("right")
         def _list_right(event):
             radio_list._handle_enter()
-            cv = radio_list.current_value
-            if type(cv) is pathlib.PosixPath and cv.is_dir():
-                self.stride(radio_list.current_value)
+            p = radio_list.current_value
+            if type(p) is pathlib.PosixPath:
+                if p.is_dir():
+                    self.stride(p)
+                else:
+                    self.stride(p.parent, selected_by_value=p)
             else:
                 # open_in_terminal(radio_list.current_value)
                 pass
 
         @radio_list.control.key_bindings.add("space")
         def _list_space(event):
             radio_list._handle_enter()
-            if type(radio_list.current_value) is pathlib.PosixPath:
-                self.stride(radio_list.current_value, title_msg='Actions', update_list=False)
-                radio_list.values = self.list_file_actions(radio_list.current_value)
-                radio_list._selected_index = 0
-                self.history_append(radio_list.current_value)
+            if type(self.list.current_value) is pathlib.PosixPath:
+                self.show_actions_menu()
 
         @radio_list.control.key_bindings.add("c-j")
         def _key_jump(event):
             def callback(result_path, input_data):
                 if result_path:
                     p = Path(result_path).expanduser().absolute()
                     if p.is_dir():
@@ -241,23 +256,24 @@
                 self.stride(r['move']['p'], selected_by_value=r['move']['selected_by_value'],
                             file_msg=r['move']['file_msg'], title_msg='Copy')
                 return r['result']
             self.input_dialog(title='Copy from', label_text='Copy here this:', callback=callback, input_data={'target_path': self.current_path})
 
         @radio_list.control.key_bindings.add("c-h")
         def _key_jump_to_directory(event):
+            self.mode = 'history'
             radio_list._selected_index = 0
             radio_list.values = [(Path(p), HTML(self.format_path_accent(p))) for p in self.history][:100]
             self.set_title(self.current_path, msg='History')
 
         @radio_list.control.key_bindings.add("c-c")
         def _key_copy_path(event):
             self.copy_path_clp(self.current_path)
 
-        @radio_list.control.key_bindings.add("escape")
+        @radio_list.control.key_bindings.add("c-q")
         def _key_exit(event):
             event.app.exit()
 
         if self.env['keys_midnight_commander']:
             @radio_list.control.key_bindings.add("f5")
             def _key_copy_path(event):
                 radio_list._handle_enter()
@@ -285,14 +301,23 @@
             @radio_list.control.key_bindings.add("f12")
             def _key_exit(event):
                 radio_list._handle_enter()
                 self.do_open_with(radio_list.current_value)
 
         return radio_list
 
+    def show_actions_menu(self):
+        self.mode = 'menu'
+        self.set_title(self.list.current_value, msg='Actions')
+        self.set_current_path(self.list.current_value)
+
+        self.list.values = self.list_file_actions(self.list.current_value)
+        self.list._selected_index = 0
+
+        self.history_append(self.list.current_value)
 
     @staticmethod
     def sort_files_in_list(list_sets):
         """Sort files in the list of sets that represent the main list."""
         def sort_func(s):
             return str(s[0]).lower()
 
@@ -383,31 +408,34 @@
         :return:
         """
         self.set_title(self.current_path, msg=title_msg)
         self.list.values, self.list._selected_index = self.get_list_values(file_msg=file_msg).values()
         if selected_by_value:
             self.list._selected_index = self.get_index_in_values(self.list.values, payload=selected_by_value)
 
-    def stride(self, p: Path = None, selected_by_value=None, title_msg=None, file_msg=None, update_list=True):
+    def set_current_path(self, p):
+        p = p if p else self.current_path
+        self.current_path = p.absolute()
+
+    def stride(self, p: Path = None, selected_by_value=None, title_msg=None, file_msg=None):
         """
         Stride to the path.
         :param p:
         :param selected_by_value:
         :param title_msg:
         :param file_msg:
         :param update_list:
         :return:
         """
-        p = p if p else self.current_path
-        self.current_path = p.absolute()
+        self.mode = 'list'
+        self.set_current_path(p)
         self.set_title(p, msg=title_msg)
         if self.current_path.is_dir() and self.env['os_path_change']:
             os.chdir(self.current_path)
-        if update_list:
-            self.update_list(selected_by_value=selected_by_value, title_msg=title_msg, file_msg=file_msg)
+        self.update_list(selected_by_value=selected_by_value, title_msg=title_msg, file_msg=file_msg)
 
     def do_open_with(self, path: Path = None):
         """Show "Open with" menu."""
         apps = get_os_applications()
         p = path if path else self.current_path
         self.stride(p, title_msg='Open with')
         self.list.values = [(open_in_os, 'OS associated')] + [(functools.partial(self.open_in_os_app, app_name=a), a) for a in apps]
```

### Comparing `fstrider-0.1.19/fstrider/os.py` & `fstrider-0.1.20/fstrider/os.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.19/fstrider/ptk.py` & `fstrider-0.1.20/fstrider/ptk.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.19/fstrider.egg-info/PKG-INFO` & `fstrider-0.1.20/fstrider.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstrider
-Version: 0.1.19
+Version: 0.1.20
 Summary: Library of the useful macroses for the xonsh shell.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,21 +88,21 @@
 
 Basic:
 
 * <kbd>Left</kbd> - move to parent directory.
 * <kbd>Right</kbd> - move to the selected directory.
 * <kbd>Space</kbd> - open menu for the current file or directory.
 * <kbd>Enter</kbd> - open file or directory using OS associations.
-* <kbd>Esc</kbd> - quit.
+* <kbd>Control q</kbd> - quit.
 
 Additional:
 
-* <kbd>Shift ~</kbd> - jump to the home directoy.
-* <kbd>Control j</kbd> - jump to path. You can jump into new path and then create it.
+* <kbd>Shift ~</kbd> - jump to the home directory.
 * <kbd>Control h</kbd> - jump to directory from history.
+* <kbd>Control j</kbd> - jump to path. You can jump into new path and then create it.
 * <kbd>Control +</kbd> - copy path to the current directory.
 
 Midnight Commander bindings: <kbd>F5</kbd> copy, <kbd>F6</kbd> move, <kbd>F7</kbd> rename, <kbd>F8</kbd> delete, <kbd>F10</kbd> quit, <kbd>F12</kbd> open with.
 
 ### Using `/` when copying or moving.
 
 fstrider was created to reduce keystrokes. So remember two things:
@@ -145,46 +145,51 @@
 Xonsh xontrib
     ++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18)
     ++ Run fstrider as fast as possible. (0.1.18)
     ++ Keeps history between running fstrider. (0.1.18)
 
 List
     ++ Async monitoring of the list and update if new files created. (0.1.19)
+    ++Add `/` to the end of directory in title and in history.
     
 Configuration
     ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
 
 Integration
     "=" to move object from path to the current dir.
 
 Tech
+    ++ Add list and menu mode.
     Errors processing
         Show errors like in case of exception.
         Process `File exists` error.
     ++ Resolve `/tmp/../../`. (0.1.17)
     Symlinks: copying, moving   
     
+    
 Style
     Grey style for copy/move and red style for delete dialogue. 
     
 Navigation
+    Move coursor to the next file after deletion.
     ++ Up key at first option moves cursor to end. (0.1.19)
-    Fix left key when go from history.    
-    Fix right key when go to file from history.
+    ++ Fix left key when go from history.    
+    ++ Fix right key when go to file from history.
 ```
 
 ### v0.3.0
 
 ```
 Navigation
     Go back to previous directory after moving or copying.
     
 List
     Sorting by size/date `sorted(glob.glob('*.png'), key=os.path.getsize)`.
     Modes: short, full (chmod/chown/date). 
+    Keep file msg after `invalidate_list`.
 
 Jump
     Use path from clipboard e.g. `text_area.buffer.paste_clipboard_data`.
     Use directories from xonsh history i.e. `__xonsh__.history[-1].cwd`
 ```
 
 ### v0.4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fstrider Version: 0.1.19 Summary: Library of the
+Metadata-Version: 2.1 Name: fstrider Version: 0.1.20 Summary: Library of the
 useful macroses for the xonsh shell. Author-email: anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -35,69 +35,72 @@
 and directories. Install or update: ```xsh pip install fstrider # OR: pip
 install -U git+https://github.com/anki-code/fstrider ``` ## Usage Run fstrider
 and start striding: ```xsh fstrider ``` In the xonsh shell you can load xontrib
 with `s` alias that works fast and allows to change directory using fstrider:
 ```xsh xontrib load fstrider fs # or fstrider ``` ### Key bindings Basic: *
 Left - move to parent directory. * Right - move to the selected directory. *
 Space - open menu for the current file or directory. * Enter - open file or
-directory using OS associations. * Esc - quit. Additional: * Shift ~ - jump to
-the home directoy. * Control j - jump to path. You can jump into new path and
-then create it. * Control h - jump to directory from history. * Control + -
-copy path to the current directory. Midnight Commander bindings: F5 copy, F6
-move, F7 rename, F8 delete, F10 quit, F12 open with. ### Using `/` when copying
-or moving. fstrider was created to reduce keystrokes. So remember two things: *
-Any new path will be created automatically. When you copy the file
-`example.txt` to `/tmp/some/new/path/` the path `/tmp/some/new/path/` will be
-created automatically. * If you copy directory `/tmp/dir1` and the target path
-ends with `/` e.g. `/tmp/other/` then the `dir1` will be putted into `/tmp/
-other/dir`. * If you copy directory `/tmp/dir2` and the target path ends with
-directory name e.g. `/tmp/other` then the `dir2` will be merged with `/tmp/
-other`. Existing files will be overwritten. ## Xonsh xontrib fstrider xontrib
-features: * Creates alias `fs` (or `fstrider` if `fs` exists). * Run fstrider
-as fast as possible. * Keeps history between running fstrider. Environment
-variables for fstrider xontrib: * `$XONTRIB_FSTRIDER_ALIAS` - change the alias
-name. Recommended `s`. ## Options * `'show_symlink_paths': True` - show
-symlinks in the list. * `'keys_midnight_commander': True` - use Midnight
-Commander keys. * `'monitor_state': False` - Async monitoring of the list and
-update if new files created. * `'os_path_change': True` - change os path in
-xonsh shell. * `'app_associations_save_file': False` - save filename to apps
-associations. You can change the option state by setting environment variable
-e.g. `$FSTRIDER_MONITOR_STATE=True`. ## Known issues ### Tested only on Mac OS
-Current version of fstrider is using and testing on Mac OS. It will be good to
-test and fix for Linux and Windows. ## Roadmap Feel free to grab and implement
-or propose new feature. PR is welcome! ### v0.2.0 ``` Xonsh xontrib ++ Creates
-alias `fs` (or `fstrider` if `fs` exists). (0.1.18) ++ Run fstrider as fast as
-possible. (0.1.18) ++ Keeps history between running fstrider. (0.1.18) List ++
-Async monitoring of the list and update if new files created. (0.1.19)
+directory using OS associations. * Control q - quit. Additional: * Shift ~ -
+jump to the home directory. * Control h - jump to directory from history. *
+Control j - jump to path. You can jump into new path and then create it. *
+Control + - copy path to the current directory. Midnight Commander bindings: F5
+copy, F6 move, F7 rename, F8 delete, F10 quit, F12 open with. ### Using `/
+` when copying or moving. fstrider was created to reduce keystrokes. So
+remember two things: * Any new path will be created automatically. When you
+copy the file `example.txt` to `/tmp/some/new/path/` the path `/tmp/some/new/
+path/` will be created automatically. * If you copy directory `/tmp/dir1` and
+the target path ends with `/` e.g. `/tmp/other/` then the `dir1` will be putted
+into `/tmp/other/dir`. * If you copy directory `/tmp/dir2` and the target path
+ends with directory name e.g. `/tmp/other` then the `dir2` will be merged with
+`/tmp/other`. Existing files will be overwritten. ## Xonsh xontrib fstrider
+xontrib features: * Creates alias `fs` (or `fstrider` if `fs` exists). * Run
+fstrider as fast as possible. * Keeps history between running fstrider.
+Environment variables for fstrider xontrib: * `$XONTRIB_FSTRIDER_ALIAS` -
+change the alias name. Recommended `s`. ## Options * `'show_symlink_paths':
+True` - show symlinks in the list. * `'keys_midnight_commander': True` - use
+Midnight Commander keys. * `'monitor_state': False` - Async monitoring of the
+list and update if new files created. * `'os_path_change': True` - change os
+path in xonsh shell. * `'app_associations_save_file': False` - save filename to
+apps associations. You can change the option state by setting environment
+variable e.g. `$FSTRIDER_MONITOR_STATE=True`. ## Known issues ### Tested only
+on Mac OS Current version of fstrider is using and testing on Mac OS. It will
+be good to test and fix for Linux and Windows. ## Roadmap Feel free to grab and
+implement or propose new feature. PR is welcome! ### v0.2.0 ``` Xonsh xontrib
+++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18) ++ Run fstrider
+as fast as possible. (0.1.18) ++ Keeps history between running fstrider.
+(0.1.18) List ++ Async monitoring of the list and update if new files created.
+(0.1.19) ++Add `/` to the end of directory in title and in history.
 Configuration ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
-Integration "=" to move object from path to the current dir. Tech Errors
-processing Show errors like in case of exception. Process `File exists` error.
-++ Resolve `/tmp/../../`. (0.1.17) Symlinks: copying, moving Style Grey style
-for copy/move and red style for delete dialogue. Navigation ++ Up key at first
-option moves cursor to end. (0.1.19) Fix left key when go from history. Fix
-right key when go to file from history. ``` ### v0.3.0 ``` Navigation Go back
-to previous directory after moving or copying. List Sorting by size/date
+Integration "=" to move object from path to the current dir. Tech ++ Add list
+and menu mode. Errors processing Show errors like in case of exception. Process
+`File exists` error. ++ Resolve `/tmp/../../`. (0.1.17) Symlinks: copying,
+moving Style Grey style for copy/move and red style for delete dialogue.
+Navigation Move coursor to the next file after deletion. ++ Up key at first
+option moves cursor to end. (0.1.19) ++ Fix left key when go from history. ++
+Fix right key when go to file from history. ``` ### v0.3.0 ``` Navigation Go
+back to previous directory after moving or copying. List Sorting by size/date
 `sorted(glob.glob('*.png'), key=os.path.getsize)`. Modes: short, full (chmod/
-chown/date). Jump Use path from clipboard e.g.
-`text_area.buffer.paste_clipboard_data`. Use directories from xonsh history
-i.e. `__xonsh__.history[-1].cwd` ``` ### v0.4.0 ``` Title Show chown/chmod if
-"Access denied". Show what part of path is exist and what's new. Dialog
-Autocomplete for paths in menu - the feature from prompt-toolkit. Copying
-progress bar or just the console log from `rsync`. ``` ### v0.5.0 ``` List
-Fuzzy search. Research: Draggable items i.e. `ls --hyperlink`. Associations
-`.xonshrc` case in app_assoc. Highlight known suffix from app_assoc. Using
-$LS_COLORS and `dircolors` for color files. ``` ### v0.6.0 ``` List Improve
-speed of list on big amount of items - 10k+ ``` ### Waiting for community ```
-Integration Other shells support. Key bindings The way to change key bindings.
-VI mode, Emacs mode. Style Dark style. ``` ### Ideas for future ``` List Fake
-files (items in the list) Fake deleted file to show that this file was deleted.
-Interstellar wormhole - path to another path added to this directory. Read the
-path from files in this directory. Colors and gradient: by time, by size. Show
-old files with dark color. Show small files with dark color. Integration
-Catching pasting path from clipboard and ask actions: cd-ing, copy/move from,
-open. Using fstrider for anything e.g. striding around aws s3 bucket, ssh host.
-The way to setup fstrider for special needs: colors, menus, hotkeys. Keys Free
-keys to use: `/`, `-`. Xonsh shell Using xonsh shell history to jump into
-directories. Run shell command in this directory. Crazy: use xonsh prompt as a
-prompt for ptk `TextArea` AI Predict the next choice of path based on history
-and maybe files in dir. ``` ## Good to know * Copy the current path in MacOS
-Finder: Option Command C * Jump to path in MacOS Finder: Command Shift G
+chown/date). Keep file msg after `invalidate_list`. Jump Use path from
+clipboard e.g. `text_area.buffer.paste_clipboard_data`. Use directories from
+xonsh history i.e. `__xonsh__.history[-1].cwd` ``` ### v0.4.0 ``` Title Show
+chown/chmod if "Access denied". Show what part of path is exist and what's new.
+Dialog Autocomplete for paths in menu - the feature from prompt-toolkit.
+Copying progress bar or just the console log from `rsync`. ``` ### v0.5.0 ```
+List Fuzzy search. Research: Draggable items i.e. `ls --hyperlink`.
+Associations `.xonshrc` case in app_assoc. Highlight known suffix from
+app_assoc. Using $LS_COLORS and `dircolors` for color files. ``` ### v0.6.0 ```
+List Improve speed of list on big amount of items - 10k+ ``` ### Waiting for
+community ``` Integration Other shells support. Key bindings The way to change
+key bindings. VI mode, Emacs mode. Style Dark style. ``` ### Ideas for future
+``` List Fake files (items in the list) Fake deleted file to show that this
+file was deleted. Interstellar wormhole - path to another path added to this
+directory. Read the path from files in this directory. Colors and gradient: by
+time, by size. Show old files with dark color. Show small files with dark
+color. Integration Catching pasting path from clipboard and ask actions: cd-
+ing, copy/move from, open. Using fstrider for anything e.g. striding around aws
+s3 bucket, ssh host. The way to setup fstrider for special needs: colors,
+menus, hotkeys. Keys Free keys to use: `/`, `-`. Xonsh shell Using xonsh shell
+history to jump into directories. Run shell command in this directory. Crazy:
+use xonsh prompt as a prompt for ptk `TextArea` AI Predict the next choice of
+path based on history and maybe files in dir. ``` ## Good to know * Copy the
+current path in MacOS Finder: Option Command C * Jump to path in MacOS Finder:
+Command Shift G
```

### Comparing `fstrider-0.1.19/pyproject.toml` & `fstrider-0.1.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fstrider"
-version = "0.1.19"
+version = "0.1.20"
 license = {file = "LICENSE"}
 description = "Library of the useful macroses for the xonsh shell."
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: System :: Shells",
```

