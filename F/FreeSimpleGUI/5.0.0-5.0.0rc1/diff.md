# Comparing `tmp/FreeSimpleGUI-5.0.0.tar.gz` & `tmp/FreeSimpleGUI-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeSimpleGUI-5.0.0.tar", last modified: Thu Apr  4 02:50:13 2024, max compression
+gzip compressed data, was "FreeSimpleGUI-5.0.0rc1.tar", last modified: Thu Apr  4 01:23:40 2024, max compression
```

## Comparing `FreeSimpleGUI-5.0.0.tar` & `FreeSimpleGUI-5.0.0rc1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:50:13.418150 FreeSimpleGUI-5.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:50:13.418150 FreeSimpleGUI-5.0.0/FreeSimpleGUI/
--rw-r--r--   0 runner    (1001) docker     (127)  2093612 2024-04-04 02:50:09.000000 FreeSimpleGUI-5.0.0/FreeSimpleGUI/FreeSimpleGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 02:50:09.000000 FreeSimpleGUI-5.0.0/FreeSimpleGUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:50:13.418150 FreeSimpleGUI-5.0.0/FreeSimpleGUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 02:50:13.000000 FreeSimpleGUI-5.0.0/FreeSimpleGUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 02:50:13.000000 FreeSimpleGUI-5.0.0/FreeSimpleGUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 02:50:13.000000 FreeSimpleGUI-5.0.0/FreeSimpleGUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-04 02:50:13.000000 FreeSimpleGUI-5.0.0/FreeSimpleGUI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 02:50:13.000000 FreeSimpleGUI-5.0.0/FreeSimpleGUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 02:50:09.000000 FreeSimpleGUI-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 02:50:09.000000 FreeSimpleGUI-5.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 02:50:13.418150 FreeSimpleGUI-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-04 02:50:09.000000 FreeSimpleGUI-5.0.0/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36240 2024-04-04 02:50:09.000000 FreeSimpleGUI-5.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-04 02:50:13.418150 FreeSimpleGUI-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 02:50:09.000000 FreeSimpleGUI-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:23:40.666794 FreeSimpleGUI-5.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:23:40.666794 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI/
+-rw-r--r--   0 runner    (1001) docker     (127)  2094645 2024-04-04 01:23:35.000000 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI/FreeSimpleGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 01:23:35.000000 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:23:40.666794 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 01:23:40.000000 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-04 01:23:40.000000 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:23:40.000000 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-04 01:23:40.000000 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 01:23:40.000000 FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 01:23:35.000000 FreeSimpleGUI-5.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 01:23:35.000000 FreeSimpleGUI-5.0.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 01:23:40.666794 FreeSimpleGUI-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-04 01:23:40.666794 FreeSimpleGUI-5.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 01:23:35.000000 FreeSimpleGUI-5.0.0rc1/setup.py
```

### Comparing `FreeSimpleGUI-5.0.0/FreeSimpleGUI/FreeSimpleGUI.py` & `FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI/FreeSimpleGUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 
-version = __version__ = '5.0.0rc1'
+version = __version__ = "5.0.0rc1"
 
-_change_log = ''
+_change_log = ""
 
 __version__ = version.split()[0]  # For PEP 396 and PEP 345
 
 # The shortened version of version
 try:
     ver = version.split(' ')[0]
 except:
@@ -193,15 +193,15 @@
     """
     Returns a string with current date and time formatted YYYY-MM-DD HH:MM:SS for easy logging
 
     :return:    String with date and time formatted YYYY-MM-DD  HH:MM:SS
     :rtype:     (str)
     """
     now = datetime.datetime.now()
-    current_time = now.strftime('%Y-%m-%d %H:%M:%S')
+    current_time = now.strftime("%Y-%m-%d %H:%M:%S")
     return current_time
 
 
 
 def running_linux():
     """
     Determines the OS is Linux by using sys.platform
@@ -275,31 +275,31 @@
 # count = (count + 1) % MAX                   # Increment to MAX then roll over to 0
 
 """
     Welcome to the "core" PySimpleGUI code....
 
     It's a mess.... really... it's a mess internally... it's the external-facing interfaces that
     are not a mess.  The Elements and the methods for them are well-designed.
-    PEP8 - this code is far far from PEP8 compliant.
-    It was written PRIOR to learning that PEP8 existed.
+    PEP8 - this code is far far from PEP8 compliant. 
+    It was written PRIOR to learning that PEP8 existed. 
 
     I'll be honest.... started learning Python in Nov 2017, started writing PySimpleGUI in Feb 2018.
     Released PySimpleGUI in July 2018.  I knew so little about Python that my parameters were all named
     using CamelCase.  DOH!  Someone on Reddit set me straight on that.  So overnight I renamed all of the
     parameters to lower case.  Unfortunately, the internal naming conventions have been set.  Mixing them
     with PEP8 at this moment would be even MORE confusing.
 
-    Code I write now, outside PySimpleGUI, IS PEP8 compliant.
+    Code I write now, outside PySimpleGUI, IS PEP8 compliant.  
 
     The variable and function naming in particular are not compliant.  There is
     liberal use of CamelVariableAndFunctionNames, but for anything externally facing, there are aliases
     available for all functions.  If you've got a serious enough problem with 100% PEP8 compliance
     that you'll pass on this package, then that's your right and I invite you to do so.  However, if
     perhaps you're a practical thinker where it's the results that matter, then you'll have no
-    trouble with this code base.  There is consisency however.
+    trouble with this code base.  There is consisency however.  
 
     I truly hope you get a lot of enjoyment out of using PySimpleGUI.  It came from good intentions.
 """
 
 # ----====----====----==== Constants the user CAN safely change ====----====----====----#
 
 # Base64 encoded GIF file
@@ -324,51 +324,51 @@
 
 DEFAULT_ELEMENT_SIZE = (45, 1)  # In CHARACTERS
 DEFAULT_BUTTON_ELEMENT_SIZE = (10, 1)  # In CHARACTERS
 DEFAULT_MARGINS = (10, 5)  # Margins for each LEFT/RIGHT margin is first term
 DEFAULT_ELEMENT_PADDING = (5, 3)  # Padding between elements (row, col) in pixels
 DEFAULT_AUTOSIZE_TEXT = True
 DEFAULT_AUTOSIZE_BUTTONS = True
-DEFAULT_FONT = ('Helvetica', 10)
+DEFAULT_FONT = ("Helvetica", 10)
 DEFAULT_TEXT_JUSTIFICATION = 'left'
 DEFAULT_BORDER_WIDTH = 1
 DEFAULT_AUTOCLOSE_TIME = 3  # time in seconds to show an autoclose form
 DEFAULT_DEBUG_WINDOW_SIZE = (80, 20)
 DEFAULT_WINDOW_LOCATION = (None, None)
 MAX_SCROLLED_TEXT_BOX_HEIGHT = 50
 DEFAULT_TOOLTIP_TIME = 400
 DEFAULT_TOOLTIP_OFFSET = (0, -20)
 DEFAULT_KEEP_ON_TOP = None
 DEFAULT_SCALING = None
 DEFAULT_ALPHA_CHANNEL = 1.0
 DEFAULT_HIDE_WINDOW_WHEN_CREATING = True
-TOOLTIP_BACKGROUND_COLOR = '#ffffe0'
+TOOLTIP_BACKGROUND_COLOR = "#ffffe0"
 TOOLTIP_FONT = None
 DEFAULT_USE_BUTTON_SHORTCUTS = False
 #################### COLOR STUFF ####################
-BLUES = ('#082567', '#0A37A3', '#00345B')
-PURPLES = ('#480656', '#4F2398', '#380474')
-GREENS = ('#01826B', '#40A860', '#96D2AB', '#00A949', '#003532')
-YELLOWS = ('#F3FB62', '#F0F595')
-TANS = ('#FFF9D5', '#F4EFCF', '#DDD8BA')
+BLUES = ("#082567", "#0A37A3", "#00345B")
+PURPLES = ("#480656", "#4F2398", "#380474")
+GREENS = ("#01826B", "#40A860", "#96D2AB", "#00A949", "#003532")
+YELLOWS = ("#F3FB62", "#F0F595")
+TANS = ("#FFF9D5", "#F4EFCF", "#DDD8BA")
 NICE_BUTTON_COLORS = ((GREENS[3], TANS[0]),
                       ('#000000', '#FFFFFF'),
                       ('#FFFFFF', '#000000'),
                       (YELLOWS[0], PURPLES[1]),
                       (YELLOWS[0], GREENS[3]),
                       (YELLOWS[0], BLUES[2]))
 
 COLOR_SYSTEM_DEFAULT = '1234567890'  # A Magic Number kind of signal to PySimpleGUI that the color should not be set at all
 DEFAULT_BUTTON_COLOR = ('white', BLUES[0])  # Foreground, Background (None, None) == System Default
 OFFICIAL_PYSIMPLEGUI_BUTTON_COLOR = ('white', BLUES[0])
 
 # The "default PySimpleGUI theme"
 OFFICIAL_PYSIMPLEGUI_THEME = CURRENT_LOOK_AND_FEEL = 'Dark Blue 3'
 
-DEFAULT_ERROR_BUTTON_COLOR = ('#FFFFFF', '#FF0000')
+DEFAULT_ERROR_BUTTON_COLOR = ("#FFFFFF", "#FF0000")
 DEFAULT_BACKGROUND_COLOR = None
 DEFAULT_ELEMENT_BACKGROUND_COLOR = None
 DEFAULT_ELEMENT_TEXT_COLOR = COLOR_SYSTEM_DEFAULT
 DEFAULT_TEXT_ELEMENT_BACKGROUND_COLOR = None
 DEFAULT_TEXT_COLOR = COLOR_SYSTEM_DEFAULT
 DEFAULT_INPUT_ELEMENTS_COLOR = COLOR_SYSTEM_DEFAULT
 DEFAULT_INPUT_TEXT_COLOR = COLOR_SYSTEM_DEFAULT
@@ -411,17 +411,17 @@
 DEFAULT_TTK_THEME = THEME_DEFAULT
 ttk_theme_in_use = None
 # TTK_THEME_LIST = ('default', 'winnative', 'clam', 'alt', 'classic', 'vista', 'xpnative')
 
 
 USE_TTK_BUTTONS = None
 
-DEFAULT_PROGRESS_BAR_COLOR = ('#01826B', '#D0D0D0')  # a nice green progress bar
+DEFAULT_PROGRESS_BAR_COLOR = ("#01826B", '#D0D0D0')  # a nice green progress bar
 DEFAULT_PROGRESS_BAR_COMPUTE = ('#000000', '#000000')  # Means that the progress bar colors should be computed from other colors
-DEFAULT_PROGRESS_BAR_COLOR_OFFICIAL = ('#01826B', '#D0D0D0')  # a nice green progress bar
+DEFAULT_PROGRESS_BAR_COLOR_OFFICIAL = ("#01826B", '#D0D0D0')  # a nice green progress bar
 DEFAULT_PROGRESS_BAR_SIZE = (20, 20)  # Size of Progress Bar (characters for length, pixels for width)
 DEFAULT_PROGRESS_BAR_BORDER_WIDTH = 1
 DEFAULT_PROGRESS_BAR_RELIEF = RELIEF_GROOVE
 # PROGRESS_BAR_STYLES = ('default', 'winnative', 'clam', 'alt', 'classic', 'vista', 'xpnative')
 DEFAULT_PROGRESS_BAR_STYLE = DEFAULT_TTK_THEME
 DEFAULT_METER_ORIENTATION = 'Horizontal'
 DEFAULT_SLIDER_ORIENTATION = 'vertical'
@@ -624,15 +624,15 @@
 BUTTON_TYPE_REALTIME = 9
 BUTTON_TYPE_CALENDAR_CHOOSER = 30
 BUTTON_TYPE_COLOR_CHOOSER = 40
 BUTTON_TYPE_SHOW_DEBUGGER = 50
 
 BROWSE_FILES_DELIMITER = ';'  # the delimiter to be used between each file in the returned string
 
-FILE_TYPES_ALL_FILES = (('ALL Files', '*.* *'),)
+FILE_TYPES_ALL_FILES = (("ALL Files", "*.* *"),)
 
 BUTTON_DISABLED_MEANS_IGNORE = 'ignore'
 
 # -------------------------  Element types  ------------------------- #
 
 ELEM_TYPE_TEXT = 'text'
 ELEM_TYPE_INPUT_TEXT = 'input'
@@ -780,17 +780,17 @@
         self.widget = widget
         self.text = text
         self.timeout = timeout
         # self.wraplength = wraplength if wraplength else widget.winfo_screenwidth() // 2
         self.tipwindow = None
         self.id = None
         self.x = self.y = 0
-        self.widget.bind('<Enter>', self.enter)
-        self.widget.bind('<Leave>', self.leave)
-        self.widget.bind('<ButtonPress>', self.leave)
+        self.widget.bind("<Enter>", self.enter)
+        self.widget.bind("<Leave>", self.leave)
+        self.widget.bind("<ButtonPress>", self.leave)
 
     def enter(self, event=None):
         """
         Called by tkinter when mouse enters a widget
         :param event: from tkinter.  Has x,y coordinates of mouse
         :type event:
 
@@ -837,16 +837,16 @@
         try:
             self.tipwindow.wm_overrideredirect(True)
             # if running_mac() and ENABLE_MAC_NOTITLEBAR_PATCH:
             if _mac_should_apply_notitlebar_patch():
                 self.tipwindow.wm_overrideredirect(False)
         except Exception as e:
             print('* Error performing wm_overrideredirect in showtip *', e)
-        self.tipwindow.wm_geometry('+%d+%d' % (x, y))
-        self.tipwindow.wm_attributes('-topmost', 1)
+        self.tipwindow.wm_geometry("+%d+%d" % (x, y))
+        self.tipwindow.wm_attributes("-topmost", 1)
 
         label = ttk.Label(self.tipwindow, text=self.text, justify=tk.LEFT,
                           background=TOOLTIP_BACKGROUND_COLOR, relief=tk.SOLID, borderwidth=1)
         if TOOLTIP_FONT is not None:
             label.config(font=TOOLTIP_FONT)
         label.pack()
 
@@ -1129,15 +1129,15 @@
 
         """
         if self._popup_menu_location == (None, None):
             winx, winy = self.ParentForm.current_location()
         else:
             winx, winy = self._popup_menu_location
         # self.ParentForm.TKroot.update()
-        self.ParentForm.TKroot.tk.call('wm', 'geometry', menu, '+{}+{}'.format(winx, winy))
+        self.ParentForm.TKroot.tk.call('wm', 'geometry', menu, "+{}+{}".format(winx, winy))
 
     def _MenuItemChosenCallback(self, item_chosen):  # TEXT Menu item callback
         """
         Callback function called when user chooses a menu item from menubar, Button Menu or right click menu
 
         :param item_chosen: String holding the value chosen.
         :type item_chosen:  str
@@ -1634,36 +1634,36 @@
 
 
     def _grab_anywhere_on_using_control_key(self):
         """
         Turns on Grab Anywhere functionality AFTER a window has been created.  Don't try on a window that's not yet
         been Finalized or Read.
         """
-        self.Widget.bind('<Control-Button-1>', self.ParentForm._StartMove)
-        self.Widget.bind('<Control-ButtonRelease-1>', self.ParentForm._StopMove)
-        self.Widget.bind('<Control-B1-Motion>', self.ParentForm._OnMotion)
+        self.Widget.bind("<Control-Button-1>", self.ParentForm._StartMove)
+        self.Widget.bind("<Control-ButtonRelease-1>", self.ParentForm._StopMove)
+        self.Widget.bind("<Control-B1-Motion>", self.ParentForm._OnMotion)
 
 
     def _grab_anywhere_on(self):
         """
         Turns on Grab Anywhere functionality AFTER a window has been created.  Don't try on a window that's not yet
         been Finalized or Read.
         """
-        self.Widget.bind('<ButtonPress-1>', self.ParentForm._StartMove)
-        self.Widget.bind('<ButtonRelease-1>', self.ParentForm._StopMove)
-        self.Widget.bind('<B1-Motion>', self.ParentForm._OnMotion)
+        self.Widget.bind("<ButtonPress-1>", self.ParentForm._StartMove)
+        self.Widget.bind("<ButtonRelease-1>", self.ParentForm._StopMove)
+        self.Widget.bind("<B1-Motion>", self.ParentForm._OnMotion)
 
     def _grab_anywhere_off(self):
         """
         Turns off Grab Anywhere functionality AFTER a window has been created.  Don't try on a window that's not yet
         been Finalized or Read.
         """
-        self.Widget.unbind('<ButtonPress-1>')
-        self.Widget.unbind('<ButtonRelease-1>')
-        self.Widget.unbind('<B1-Motion>')
+        self.Widget.unbind("<ButtonPress-1>")
+        self.Widget.unbind("<ButtonRelease-1>")
+        self.Widget.unbind("<B1-Motion>")
 
     def grab_anywhere_exclude(self):
         """
         Excludes this element from being used by the grab_anywhere feature
         Handy for elements like a Graph element when dragging is enabled. You want the Graph element to get the drag events instead of the window dragging.
         """
         self.ParentForm._grab_anywhere_ignore_these_list.append(self.Widget)
@@ -2032,15 +2032,15 @@
                     pass
             self.DefaultText = value
             if paste is True:
                 try:
                     self.TKEntry.delete('sel.first', 'sel.last')
                 except:
                     pass
-                self.TKEntry.insert('insert', value)
+                self.TKEntry.insert("insert", value)
             if move_cursor_to == 'end':
                 self.TKEntry.icursor(tk.END)
             elif move_cursor_to is not None:
                 self.TKEntry.icursor(move_cursor_to)
         if select:
             self.TKEntry.select_range(0, 'end')
         if visible is False:
@@ -2318,15 +2318,15 @@
                 combostyle.configure(style_name, selectbackground=background_color)
 
 
         if font is not None:
             self.Font = font
             self.TKCombo.configure(font=font)
             self._dropdown_newfont = tkinter.font.Font(font=font)
-            self.ParentRowFrame.option_add('*TCombobox*Listbox*Font', self._dropdown_newfont)
+            self.ParentRowFrame.option_add("*TCombobox*Listbox*Font", self._dropdown_newfont)
 
 
         # make tcl call to deal with colors for the drop-down formatting
         try:
             if self.BackgroundColor not in (None, COLOR_SYSTEM_DEFAULT) and \
                 self.TextColor not in (None, COLOR_SYSTEM_DEFAULT):
                 self.Widget.tk.eval(
@@ -3710,15 +3710,15 @@
                     self.TKText.insert(tk.END, value, (just_tag, tag))
                 else:
                     self.TKText.insert(tk.END, value)
 
                 # self.TKText.tag_add(just_tag, starting_point, starting_point)
 
             except Exception as e:
-                print('* Error setting multiline *', e)
+                print("* Error setting multiline *", e)
             if self.Disabled:
                 self.TKText.configure(state='disabled')
             self.DefaultText = value
 
         # if self.Autoscroll:
         #     self.TKText.see(tk.END)
         if self.Autoscroll:
@@ -4756,15 +4756,15 @@
         # if image_filename or image_data:
         #     self.UseTtkButtons = False              # if an image is to be displayed, then force the button to not be a TTK Button
         if key is None and k is None:
             _key = self.ButtonText
             if DEFAULT_USE_BUTTON_SHORTCUTS is True:
                 pos = _key.find(MENU_SHORTCUT_CHARACTER)
                 if pos != -1:
-                    if pos < len(MENU_SHORTCUT_CHARACTER) or _key[pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                    if pos < len(MENU_SHORTCUT_CHARACTER) or _key[pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                         _key = _key[:pos] + _key[pos + len(MENU_SHORTCUT_CHARACTER):]
                     else:
                         _key = _key.replace('\\'+MENU_SHORTCUT_CHARACTER, MENU_SHORTCUT_CHARACTER)
         else:
             _key = key if key is not None else k
         if highlight_colors is not None:
             self.HighlightColors = highlight_colors
@@ -5063,15 +5063,15 @@
             # style_name = str(self.Key) + 'custombutton.TButton'
             button_style = ttk.Style()
         if text is not None:
             btext = text
             if DEFAULT_USE_BUTTON_SHORTCUTS is True:
                 pos = btext.find(MENU_SHORTCUT_CHARACTER)
                 if pos != -1:
-                    if pos < len(MENU_SHORTCUT_CHARACTER) or btext[pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                    if pos < len(MENU_SHORTCUT_CHARACTER) or btext[pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                         btext = btext[:pos] + btext[pos + len(MENU_SHORTCUT_CHARACTER):]
                     else:
                         btext = btext.replace('\\'+MENU_SHORTCUT_CHARACTER, MENU_SHORTCUT_CHARACTER)
                         pos = -1
                 if pos != -1:
                     self.TKButton.config(underline=pos)
             self.TKButton.configure(text=btext)
@@ -6680,15 +6680,15 @@
         """
         """
         Updates the variable that's used when the values dictionary is returned from a window read.
 
         Not called by the user.  It's called from another method/function that tkinter calledback
 
         :param event: (event) event info from tkinter. Contains the x and y coordinates of a click
-        :type event:
+        :type event:  
         """
 
         self.ClickPosition = self._convert_canvas_xy_to_xy(event.x, event.y)
 
     # button callback
     def motion_call_back(self, event):
         """
@@ -7853,23 +7853,23 @@
         :param **kwargs: The keyword args
         :type **kwargs:
         """
         tk.Frame.__init__(self, master, **kwargs)
 
         self.canvas = tk.Canvas(self)
 
-        self.canvas.pack(side='left', fill='both', expand=True)
+        self.canvas.pack(side="left", fill="both", expand=True)
 
         # reset the view
         self.canvas.xview_moveto(0)
         self.canvas.yview_moveto(0)
 
         # create a frame inside the canvas which will be scrolled with it
         self.TKFrame = tk.Frame(self.canvas, **kwargs)
-        self.frame_id = self.canvas.create_window(0, 0, window=self.TKFrame, anchor='nw')
+        self.frame_id = self.canvas.create_window(0, 0, window=self.TKFrame, anchor="nw")
         self.canvas.config(borderwidth=0, highlightthickness=0)
         self.TKFrame.config(borderwidth=0, highlightthickness=0)
         self.config(borderwidth=0, highlightthickness=0)
 
 
 # ---------------------------------------------------------------------- #
 #                          TkScrollableFrame (Used by Column)            #
@@ -7893,38 +7893,38 @@
 
         self.canvas = tk.Canvas(self)
         element.Widget = self.canvas
         # Okay, we're gonna make a list. Containing the y-min, x-min, y-max, and x-max of the frame
         element.element_frame = self
         _make_ttk_scrollbar(element, 'v', window)
         # element.vsb = tk.Scrollbar(self, orient=tk.VERTICAL)
-        element.vsb.pack(side='right', fill='y', expand='false')
+        element.vsb.pack(side='right', fill="y", expand="false")
 
         if not vertical_only:
             _make_ttk_scrollbar(element, 'h', window)
             # self.hscrollbar = tk.Scrollbar(self, orient=tk.HORIZONTAL)
-            element.hsb.pack(side='bottom', fill='x', expand='false')
+            element.hsb.pack(side='bottom', fill="x", expand="false")
             self.canvas.config(xscrollcommand=element.hsb.set)
             # self.canvas = tk.Canvas(self, )
         # else:
         #     self.canvas = tk.Canvas(self)
 
         self.canvas.config(yscrollcommand=element.vsb.set)
-        self.canvas.pack(side='left', fill='both', expand=True)
+        self.canvas.pack(side="left", fill="both", expand=True)
         element.vsb.config(command=self.canvas.yview)
         if not vertical_only:
             element.hsb.config(command=self.canvas.xview)
 
         # reset the view
         self.canvas.xview_moveto(0)
         self.canvas.yview_moveto(0)
 
         # create a frame inside the canvas which will be scrolled with it
         self.TKFrame = tk.Frame(self.canvas, **kwargs)
-        self.frame_id = self.canvas.create_window(0, 0, window=self.TKFrame, anchor='nw')
+        self.frame_id = self.canvas.create_window(0, 0, window=self.TKFrame, anchor="nw")
         self.canvas.config(borderwidth=0, highlightthickness=0)
         self.TKFrame.config(borderwidth=0, highlightthickness=0)
         self.config(borderwidth=0, highlightthickness=0)
 
         # Canvas can be: master, canvas, TKFrame
 
         # Chr0nic
@@ -7932,60 +7932,60 @@
         # self.unhookMouseWheel(None)
         # self.TKFrame.bind("<Enter>", self.hookMouseWheel)
         # self.TKFrame.bind("<Leave>", self.unhookMouseWheel)
         # self.bind('<Configure>', self.set_scrollregion)
 
 
         self.unhookMouseWheel(None)
-        self.canvas.bind('<Enter>', self.hookMouseWheel)
-        self.canvas.bind('<Leave>', self.unhookMouseWheel)
+        self.canvas.bind("<Enter>", self.hookMouseWheel)
+        self.canvas.bind("<Leave>", self.unhookMouseWheel)
         self.bind('<Configure>', self.set_scrollregion)
 
 
     # Chr0nic
     def hookMouseWheel(self, e):
         # print("enter")
         VarHolder.canvas_holder = self.canvas
         self.canvas.bind_all('<4>', self.yscroll, add='+')
         self.canvas.bind_all('<5>', self.yscroll, add='+')
-        self.canvas.bind_all('<MouseWheel>', self.yscroll, add='+')
-        self.canvas.bind_all('<Shift-MouseWheel>', self.xscroll, add='+')
+        self.canvas.bind_all("<MouseWheel>", self.yscroll, add='+')
+        self.canvas.bind_all("<Shift-MouseWheel>", self.xscroll, add='+')
 
     # Chr0nic
     def unhookMouseWheel(self, e):
         # print("leave")
         VarHolder.canvas_holder = None
         self.canvas.unbind_all('<4>')
         self.canvas.unbind_all('<5>')
-        self.canvas.unbind_all('<MouseWheel>')
-        self.canvas.unbind_all('<Shift-MouseWheel>')
+        self.canvas.unbind_all("<MouseWheel>")
+        self.canvas.unbind_all("<Shift-MouseWheel>")
 
     def resize_frame(self, e):
         self.canvas.itemconfig(self.frame_id, height=e.height, width=e.width)
 
     def yscroll(self, event):
         if self.canvas.yview() == (0.0, 1.0):
             return
         if event.num == 5 or event.delta < 0:
-            self.canvas.yview_scroll(1, 'unit')
+            self.canvas.yview_scroll(1, "unit")
         elif event.num == 4 or event.delta > 0:
-            self.canvas.yview_scroll(-1, 'unit')
+            self.canvas.yview_scroll(-1, "unit")
 
     def xscroll(self, event):
         if event.num == 5 or event.delta < 0:
-            self.canvas.xview_scroll(1, 'unit')
+            self.canvas.xview_scroll(1, "unit")
         elif event.num == 4 or event.delta > 0:
-            self.canvas.xview_scroll(-1, 'unit')
+            self.canvas.xview_scroll(-1, "unit")
 
     def bind_mouse_scroll(self, parent, mode):
         # ~~ Windows only
-        parent.bind('<MouseWheel>', mode)
+        parent.bind("<MouseWheel>", mode)
         # ~~ Unix only
-        parent.bind('<Button-4>', mode)
-        parent.bind('<Button-5>', mode)
+        parent.bind("<Button-4>", mode)
+        parent.bind("<Button-5>", mode)
 
     def set_scrollregion(self, event=None):
         """ Set the scroll region on the canvas """
         self.canvas.configure(scrollregion=self.canvas.bbox('all'))
 
 
 # ---------------------------------------------------------------------- #
@@ -8706,15 +8706,15 @@
                     baritem.config(font=self.Font)
 
                 if self.Font is not None:
                     baritem.config(font=self.Font)
                 pos = menu_entry[0].find(MENU_SHORTCUT_CHARACTER)
                 # print(pos)
                 if pos != -1:
-                    if pos == 0 or menu_entry[0][pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                    if pos == 0 or menu_entry[0][pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                         menu_entry[0] = menu_entry[0][:pos] + menu_entry[0][pos + len(MENU_SHORTCUT_CHARACTER):]
                 if menu_entry[0][0] == MENU_DISABLED_CHARACTER:
                     menubar.add_cascade(label=menu_entry[0][len(MENU_DISABLED_CHARACTER):], menu=baritem, underline=pos)
                     menubar.entryconfig(menu_entry[0][len(MENU_DISABLED_CHARACTER):], state='disabled')
                 else:
                     menubar.add_cascade(label=menu_entry[0], menu=baritem, underline=pos)
 
@@ -9479,16 +9479,16 @@
             self.children.append(node)
 
     def __init__(self):
         """
         Instantiate the object, initializes the Tree Data, creates a root node for you
         """
         self.tree_dict = {}  # type: Dict[str, TreeData.Node]
-        self.root_node = self.Node('', '', 'root', [], None)  # The root node
-        self.tree_dict[''] = self.root_node  # Start the tree out with the root node
+        self.root_node = self.Node("", "", 'root', [], None)  # The root node
+        self.tree_dict[""] = self.root_node  # Start the tree out with the root node
 
     def _AddNode(self, key, node):
         """
         Adds a node to tree dictionary (not user callable)
 
         :param key:  Uniquely identifies this Node
         :type key:   (str)
@@ -10063,16 +10063,16 @@
 
         if layout is not None:
             self.Layout(layout)
             if finalize:
                 self.Finalize()
 
         if CURRENT_LOOK_AND_FEEL == 'Default':
-            print('Window will be a boring gray. Try removing the theme call entirely\n',
-                  'You will get the default theme or the one set in global settings\n'
+            print("Window will be a boring gray. Try removing the theme call entirely\n",
+                  "You will get the default theme or the one set in global settings\n"
                   "If you seriously want this gray window and no more nagging, add  theme('DefaultNoMoreNagging')  or theme('Gray Gray Gray') for completely gray/System Defaults")
 
 
     @classmethod
     def _GetAContainerNumber(cls):
         """
         Not user callable!
@@ -11092,15 +11092,15 @@
         Move the upper left corner of this window to the x,y coordinates provided
         :param x: x coordinate in pixels
         :type x:  (int)
         :param y: y coordinate in pixels
         :type y:  (int)
         """
         try:
-            self.TKroot.geometry('+%s+%s' % (x, y))
+            self.TKroot.geometry("+%s+%s" % (x, y))
             self.config_last_location = (int(x), (int(y)))
 
         except:
             pass
 
 
     def move_to_center(self):
@@ -11242,23 +11242,23 @@
             return
 
         self._OnMotion(event)
 
 
     def _OnMotion(self, event):
 
-        self.TKroot.geometry(f'+{event.x_root-self._mouse_offset_x}+{event.y_root-self._mouse_offset_y}')
+        self.TKroot.geometry(f"+{event.x_root-self._mouse_offset_x}+{event.y_root-self._mouse_offset_y}")
         # print(f"+{event.x_root}+{event.y_root}")
         # ------ Move All Windows code ------
         try:
             if Window._move_all_windows:
                 for win in Window._active_windows:
                     if win == self:
                         continue
-                    win.TKroot.geometry(f'+{event.x_root-win._mouse_offset_x}+{event.y_root-win._mouse_offset_y}')
+                    win.TKroot.geometry(f"+{event.x_root-win._mouse_offset_x}+{event.y_root-win._mouse_offset_y}")
         except Exception as e:
             print('on motion error', e)
 
     def _focus_callback(self, event):
         print('Focus event = {} window = {}'.format(event, self.Title))
 
     def _config_callback(self, event):
@@ -11597,18 +11597,18 @@
         Brings this window to the top of all other windows (perhaps may not be brought before a window made to "stay
         on top")
         """
         if not self._is_window_created('tried Window.bring_to_front'):
             return
         if running_windows():
             try:
-                self.TKroot.wm_attributes('-topmost', 0)
-                self.TKroot.wm_attributes('-topmost', 1)
+                self.TKroot.wm_attributes("-topmost", 0)
+                self.TKroot.wm_attributes("-topmost", 1)
                 if not self.KeepOnTop:
-                    self.TKroot.wm_attributes('-topmost', 0)
+                    self.TKroot.wm_attributes("-topmost", 0)
             except Exception as e:
                 warnings.warn('Problem in Window.bring_to_front' + str(e), UserWarning)
         else:
             try:
                 self.TKroot.lift()
             except:
                 pass
@@ -11632,29 +11632,29 @@
         to the front
         """
         if not self._is_window_created('tried Window.keep_on_top_set'):
             return
         self.KeepOnTop = True
         self.bring_to_front()
         try:
-            self.TKroot.wm_attributes('-topmost', 1)
+            self.TKroot.wm_attributes("-topmost", 1)
         except Exception as e:
             warnings.warn('Problem in Window.keep_on_top_set trying to set wm_attributes topmost' + str(e), UserWarning)
 
 
     def keep_on_top_clear(self):
         """
         Clears keep_on_top after a window has been created.  Effect is the same
         as if the window was created with this set.
         """
         if not self._is_window_created('tried Window.keep_on_top_clear'):
             return
         self.KeepOnTop = False
         try:
-            self.TKroot.wm_attributes('-topmost', 0)
+            self.TKroot.wm_attributes("-topmost", 0)
         except Exception as e:
             warnings.warn('Problem in Window.keep_on_top_clear trying to clear wm_attributes topmost' + str(e), UserWarning)
 
 
 
     def current_location(self, more_accurate=False, without_titlebar=False):
         """
@@ -11731,15 +11731,15 @@
         """
         Changes the size of the window, if possible
 
         :param size: (width, height) of the desired window size
         :type size:  (int, int)
         """
         try:
-            self.TKroot.geometry('%sx%s' % (size[0], size[1]))
+            self.TKroot.geometry("%sx%s" % (size[0], size[1]))
             self.TKroot.update_idletasks()
         except:
             pass
 
 
     def set_size(self, size):
         """
@@ -11748,15 +11748,15 @@
 
         :param size: (width, height) of the desired window size
         :type size:  (int, int)
         """
         if not self._is_window_created('Tried to change the size of the window prior to creation.'):
             return
         try:
-            self.TKroot.geometry('%sx%s' % (size[0], size[1]))
+            self.TKroot.geometry("%sx%s" % (size[0], size[1]))
             self.TKroot.update_idletasks()
         except:
             pass
 
 
 
     def set_min_size(self, size):
@@ -11828,28 +11828,28 @@
     def grab_any_where_on(self):
         """
         Turns on Grab Anywhere functionality AFTER a window has been created.  Don't try on a window that's not yet
         been Finalized or Read.
         """
         if not self._is_window_created('tried Window.grab_any_where_on'):
             return
-        self.TKroot.bind('<ButtonPress-1>', self._StartMoveGrabAnywhere)
-        self.TKroot.bind('<ButtonRelease-1>', self._StopMove)
-        self.TKroot.bind('<B1-Motion>', self._OnMotionGrabAnywhere)
+        self.TKroot.bind("<ButtonPress-1>", self._StartMoveGrabAnywhere)
+        self.TKroot.bind("<ButtonRelease-1>", self._StopMove)
+        self.TKroot.bind("<B1-Motion>", self._OnMotionGrabAnywhere)
 
     def grab_any_where_off(self):
         """
         Turns off Grab Anywhere functionality AFTER a window has been created.  Don't try on a window that's not yet
         been Finalized or Read.
         """
         if not self._is_window_created('tried Window.grab_any_where_off'):
             return
-        self.TKroot.unbind('<ButtonPress-1>')
-        self.TKroot.unbind('<ButtonRelease-1>')
-        self.TKroot.unbind('<B1-Motion>')
+        self.TKroot.unbind("<ButtonPress-1>")
+        self.TKroot.unbind("<ButtonRelease-1>")
+        self.TKroot.unbind("<B1-Motion>")
 
     def _user_bind_callback(self, bind_string, event, propagate=True):
         """
         Used when user binds a tkinter event directly to an element
 
         :param bind_string: The event that was bound so can lookup the key modifier
         :type bind_string:  (str)
@@ -11947,16 +11947,16 @@
 
     def disable_debugger(self):
         """
         Disable the internal debugger. By default the debugger is ENABLED
         """
         if not self._is_window_created('tried Window.disable_debugger'):
             return
-        self.TKroot.unbind('<Cancel>')
-        self.TKroot.unbind('<Pause>')
+        self.TKroot.unbind("<Cancel>")
+        self.TKroot.unbind("<Pause>")
         self.DebuggerEnabled = False
 
     def set_title(self, title):
         """
         Change the title of the window
 
         :param title: The string to set the title to
@@ -12230,15 +12230,15 @@
         Starts a thread on your behalf.
 
         This is a way for you to "ease into" threading without learning the details of threading.
         Your function will run, and when it returns 2 things will happen:
         1. The value you provide for end_key will be returned to you when you call window.read()
         2. If your function returns a value, then the value returned will also be included in your windows.read call in the values dictionary
 
-        importANT - This method uses THREADS... this means you CANNOT make any FreeSimpleGUI calls from
+        IMPORTANT - This method uses THREADS... this means you CANNOT make any PySimpleGUI calls from
         the function you provide with the exception of one function, Window.write_event_value.
 
         :param func:    A lambda or a function name with no parms
         :type func:     Any
         :param end_key: Optional key that will be generated when the function returns
         :type end_key:  (Any | None)
         :return:        The id of the thread
@@ -12302,15 +12302,15 @@
             # if self._skip_first_restore_callback:
             #     self._skip_first_restore_callback = False
             #     return
             self.TKroot.unbind('<Button-1>')
             self.TKroot.deiconify()
 
             # self.ParentForm.TKroot.wm_overrideredirect(True)
-            self.TKroot.wm_attributes('-type', 'dock')
+            self.TKroot.wm_attributes("-type", 'dock')
 
         else:
             self.TKroot.unbind('<Expose>')
             self.TKroot.wm_overrideredirect(True)
         if self.TKroot.state() == 'iconic':
             self.TKroot.deiconify()
         else:
@@ -12319,15 +12319,15 @@
             else:
                 self.TKroot.attributes('-fullscreen', False)
         self.maximized = False
 
 
     def _custom_titlebar_minimize(self):
         if running_linux():
-            self.TKroot.wm_attributes('-type', 'normal')
+            self.TKroot.wm_attributes("-type", "normal")
             # self.ParentForm.TKroot.state('icon')
             # return
             # self.ParentForm.maximize()
             self.TKroot.wm_overrideredirect(False)
             # self.ParentForm.minimize()
             # self.ParentForm.TKroot.wm_overrideredirect(False)
             self.TKroot.iconify()
@@ -12361,16 +12361,16 @@
 
     def timer_start(self, frequency_ms, key=EVENT_TIMER, repeating=True):
         """
         Starts a timer that gnerates Timer Events.  The default is to repeat the timer events until timer is stopped.
         You can provide your own key or a default key will be used.  The default key is defined
         with the constants EVENT_TIMER or TIMER_KEY.  They both equal the same value.
         The values dictionary will contain the timer ID that is returned from this function.
-
-        :param frequency_ms:    How often to generate timer events in milliseconds
+        
+        :param frequency_ms:    How often to generate timer events in milliseconds 
         :type frequency_ms:     int
         :param key:             Key to be returned as the timer event
         :type key:              str | int | tuple | object
         :param repeating:       If True then repeat timer events until timer is explicitly stopped
         :type repeating:        bool
         :return:                Timer ID for the timer
         :rtype:                 int
@@ -12706,16 +12706,16 @@
 
 
 # -------------------------------------------------------------------
 # fade in/out info and default window alpha
 SYSTEM_TRAY_WIN_MARGINS = 160, 60  # from right edge of screen, from bottom of screen
 SYSTEM_TRAY_MESSAGE_MAX_LINE_LENGTH = 50
 # colors
-SYSTEM_TRAY_MESSAGE_WIN_COLOR = '#282828'
-SYSTEM_TRAY_MESSAGE_TEXT_COLOR = '#ffffff'
+SYSTEM_TRAY_MESSAGE_WIN_COLOR = "#282828"
+SYSTEM_TRAY_MESSAGE_TEXT_COLOR = "#ffffff"
 
 SYSTEM_TRAY_MESSAGE_DISPLAY_DURATION_IN_MILLISECONDS = 3000  # how long to display the window
 SYSTEM_TRAY_MESSAGE_FADE_IN_DURATION = 1000  # how long to fade in / fade out the window
 
 EVENT_SYSTEM_TRAY_ICON_DOUBLE_CLICKED = '__DOUBLE_CLICKED__'
 EVENT_SYSTEM_TRAY_ICON_ACTIVATED = '__ACTIVATED__'
 EVENT_SYSTEM_TRAY_MESSAGE_CLICKED = '__MESSAGE_CLICKED__'
@@ -12932,39 +12932,39 @@
         messages = message.split('\n')
         full_msg = ''
         for m in messages:
             m_wrap = textwrap.fill(m, SYSTEM_TRAY_MESSAGE_MAX_LINE_LENGTH)
             full_msg += m_wrap + '\n'
         message = full_msg[:-1]
 
-        win_msg_lines = message.count('\n') + 1
+        win_msg_lines = message.count("\n") + 1
         max_line = max(message.split('\n'))
 
         screen_res_x, screen_res_y = Window.get_screen_size()
         win_margin = SYSTEM_TRAY_WIN_MARGINS  # distance from screen edges
         win_width, win_height = 364, 66 + (14.8 * win_msg_lines)
 
-        layout = [[Graph(canvas_size=(win_width, win_height), graph_bottom_left=(0, win_height), graph_top_right=(win_width, 0), key='-GRAPH-',
+        layout = [[Graph(canvas_size=(win_width, win_height), graph_bottom_left=(0, win_height), graph_top_right=(win_width, 0), key="-GRAPH-",
                          background_color=SYSTEM_TRAY_MESSAGE_WIN_COLOR, enable_events=True)]]
 
         win_location = location if location is not None else (screen_res_x - win_width - win_margin[0], screen_res_y - win_height - win_margin[1])
         window = Window(title, layout, background_color=SYSTEM_TRAY_MESSAGE_WIN_COLOR, no_titlebar=True,
                         location=win_location, keep_on_top=True, alpha_channel=0, margins=(0, 0), element_padding=(0, 0), grab_anywhere=True, finalize=True)
 
-        window['-GRAPH-'].draw_rectangle((win_width, win_height), (-win_width, -win_height), fill_color=SYSTEM_TRAY_MESSAGE_WIN_COLOR,
+        window["-GRAPH-"].draw_rectangle((win_width, win_height), (-win_width, -win_height), fill_color=SYSTEM_TRAY_MESSAGE_WIN_COLOR,
                                          line_color=SYSTEM_TRAY_MESSAGE_WIN_COLOR)
         if type(icon) is bytes:
-            window['-GRAPH-'].draw_image(data=icon, location=(20, 20))
+            window["-GRAPH-"].draw_image(data=icon, location=(20, 20))
         elif icon is not None:
-            window['-GRAPH-'].draw_image(filename=icon, location=(20, 20))
-        window['-GRAPH-'].draw_text(title, location=(64, 20), color=SYSTEM_TRAY_MESSAGE_TEXT_COLOR, font=('Helvetica', 12, 'bold'),
+            window["-GRAPH-"].draw_image(filename=icon, location=(20, 20))
+        window["-GRAPH-"].draw_text(title, location=(64, 20), color=SYSTEM_TRAY_MESSAGE_TEXT_COLOR, font=("Helvetica", 12, "bold"),
                                     text_location=TEXT_LOCATION_TOP_LEFT)
-        window['-GRAPH-'].draw_text(message, location=(64, 44), color=SYSTEM_TRAY_MESSAGE_TEXT_COLOR, font=('Helvetica', 9),
+        window["-GRAPH-"].draw_text(message, location=(64, 44), color=SYSTEM_TRAY_MESSAGE_TEXT_COLOR, font=("Helvetica", 9),
                                     text_location=TEXT_LOCATION_TOP_LEFT)
-        window['-GRAPH-'].set_cursor('hand2')
+        window["-GRAPH-"].set_cursor('hand2')
 
         if fade_in_duration:
             for i in range(1, int(alpha * 100)):  # fade in
                 window.set_alpha(i / 100)
                 event, values = window.read(timeout=fade_in_duration // 100)
                 if event != TIMEOUT_KEY:
                     window.set_alpha(1)
@@ -14703,17 +14703,17 @@
     except Exception as e:
         if not SUPPRESS_ERROR_POPUPS:
             _error_popup_with_traceback('** Badly formatted button color **', color_tuple_or_string, e)
         else:
             print('** Badly formatted button color... not a tuple nor string **', color_tuple_or_string, e)
         text_color, background_color = default
     if isinstance(text_color, int):
-        text_color = '#%06X' % text_color
+        text_color = "#%06X" % text_color
     if isinstance(background_color, int):
-        background_color = '#%06X' % background_color
+        background_color = "#%06X" % background_color
     # print('converted button color', color_tuple_or_string, 'to', (text_color, background_color))
 
     return (text_color, background_color)
 
 
 #####################################  -----  RESULTS   ------ ##################################################
 
@@ -15087,15 +15087,15 @@
 
     """
     return_val = None
     if type(sub_menu_info) is str:
         if not is_sub_menu and not skip:
             pos = sub_menu_info.find(MENU_SHORTCUT_CHARACTER)
             if pos != -1:
-                if pos < len(MENU_SHORTCUT_CHARACTER) or sub_menu_info[pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                if pos < len(MENU_SHORTCUT_CHARACTER) or sub_menu_info[pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                     sub_menu_info = sub_menu_info[:pos] + sub_menu_info[pos + len(MENU_SHORTCUT_CHARACTER):]
             if sub_menu_info == '---':
                 top_menu.add('separator')
             else:
                 try:
                     item_without_key = sub_menu_info[:sub_menu_info.index(MENU_KEY_SEPARATOR)]
                 except:
@@ -15140,15 +15140,15 @@
                         if element.DisabledTextColor not in (COLOR_SYSTEM_DEFAULT, None):
                             new_menu.config(disabledforeground=element.DisabledTextColor)
                         if element.ItemFont is not None:
                             new_menu.config(font=element.ItemFont)
                     return_val = new_menu
                     pos = sub_menu_info[i].find(MENU_SHORTCUT_CHARACTER)
                     if pos != -1:
-                        if pos < len(MENU_SHORTCUT_CHARACTER) or sub_menu_info[i][pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                        if pos < len(MENU_SHORTCUT_CHARACTER) or sub_menu_info[i][pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                             sub_menu_info[i] = sub_menu_info[i][:pos] + sub_menu_info[i][pos + len(MENU_SHORTCUT_CHARACTER):]
                     if sub_menu_info[i][0] == MENU_DISABLED_CHARACTER:
                         top_menu.add_cascade(label=sub_menu_info[i][len(MENU_DISABLED_CHARACTER):], menu=new_menu,
                                              underline=pos, state='disabled')
                     else:
                         top_menu.add_cascade(label=sub_menu_info[i], menu=new_menu, underline=pos)
                     AddMenuItem(new_menu, sub_menu_info[i + 1], element, is_sub_menu=True, right_click_menu=right_click_menu)
@@ -15197,15 +15197,15 @@
 # ========================   TK CODE STARTS HERE ========================================= #
 def _fixed_map(style, style_name, option, highlight_colors=(None, None)):
     # Fix for setting text colour for Tkinter 8.6.9
     # From: https://core.tcl.tk/tk/info/509cafafae
 
     # default_map = [elm for elm in style.map("Treeview", query_opt=option) if '!' not in elm[0]]
     # custom_map = [elm for elm in style.map(style_name, query_opt=option) if '!' not in elm[0]]
-    default_map = [elm for elm in style.map('Treeview', query_opt=option) if '!' not in elm[0] and 'selected' not in elm[0]]
+    default_map = [elm for elm in style.map("Treeview", query_opt=option) if '!' not in elm[0] and 'selected' not in elm[0]]
     custom_map = [elm for elm in style.map(style_name, query_opt=option) if '!' not in elm[0] and 'selected' not in elm[0]]
     if option == 'background':
         custom_map.append(('selected', highlight_colors[1] if highlight_colors[1] is not None else ALTERNATE_TABLE_AND_TREE_SELECTED_ROW_COLORS[1]))
     elif option == 'foreground':
         custom_map.append(('selected', highlight_colors[0] if highlight_colors[0] is not None else ALTERNATE_TABLE_AND_TREE_SELECTED_ROW_COLORS[0]))
 
     new_map = custom_map + default_map
@@ -15410,18 +15410,18 @@
     if frame_color not in (None, COLOR_SYSTEM_DEFAULT):
         style.configure(style_name, framecolor=frame_color)
     if frame_color not in (None, COLOR_SYSTEM_DEFAULT):
         style.configure(style_name, bordercolor=frame_color)
 
     if (background_color not in (None, COLOR_SYSTEM_DEFAULT)) and \
         (arrow_color not in (None, COLOR_SYSTEM_DEFAULT)):
-        style.map(style_name, background=[('selected', background_color), ('active', arrow_color), ('background', background_color), ('!focus', background_color)])
+        style.map(style_name, background=[("selected", background_color), ('active', arrow_color), ('background', background_color), ('!focus', background_color)])
     if (background_color not in (None, COLOR_SYSTEM_DEFAULT)) and \
         (arrow_color not in (None, COLOR_SYSTEM_DEFAULT)):
-        style.map(style_name, arrowcolor=[('selected', arrow_color), ('active', background_color), ('background', background_color),('!focus', arrow_color)])
+        style.map(style_name, arrowcolor=[("selected", arrow_color), ('active', background_color), ('background', background_color),('!focus', arrow_color)])
 
     if scroll_width not in (None, COLOR_SYSTEM_DEFAULT):
         style.configure(style_name, width=scroll_width)
     if arrow_width not in (None, COLOR_SYSTEM_DEFAULT):
         style.configure(style_name, arrowsize=arrow_width)
 
     if scroll_relief not in (None, COLOR_SYSTEM_DEFAULT):
@@ -15455,60 +15455,60 @@
 
     """
 
     # Old bindings
     def yscroll_old(event):
         try:
             if event.num == 5 or event.delta < 0:
-                VarHolder.canvas_holder.yview_scroll(1, 'unit')
+                VarHolder.canvas_holder.yview_scroll(1, "unit")
             elif event.num == 4 or event.delta > 0:
-                VarHolder.canvas_holder.yview_scroll(-1, 'unit')
+                VarHolder.canvas_holder.yview_scroll(-1, "unit")
         except:
             pass
 
     def xscroll_old(event):
         try:
             if event.num == 5 or event.delta < 0:
-                VarHolder.canvas_holder.xview_scroll(1, 'unit')
+                VarHolder.canvas_holder.xview_scroll(1, "unit")
             elif event.num == 4 or event.delta > 0:
-                VarHolder.canvas_holder.xview_scroll(-1, 'unit')
+                VarHolder.canvas_holder.xview_scroll(-1, "unit")
         except:
             pass
 
     # Chr0nic
     def testMouseHook2(em):
         combo = em.TKCombo
-        combo.unbind_class('TCombobox', '<MouseWheel>')
-        combo.unbind_class('TCombobox', '<ButtonPress-4>')
-        combo.unbind_class('TCombobox', '<ButtonPress-5>')
+        combo.unbind_class("TCombobox", "<MouseWheel>")
+        combo.unbind_class("TCombobox", "<ButtonPress-4>")
+        combo.unbind_class("TCombobox", "<ButtonPress-5>")
         containing_frame.unbind_all('<4>')
         containing_frame.unbind_all('<5>')
-        containing_frame.unbind_all('<MouseWheel>')
-        containing_frame.unbind_all('<Shift-MouseWheel>')
+        containing_frame.unbind_all("<MouseWheel>")
+        containing_frame.unbind_all("<Shift-MouseWheel>")
 
     # Chr0nic
     def testMouseUnhook2(em):
-        containing_frame.bind_all('<4>', yscroll_old, add='+')
-        containing_frame.bind_all('<5>', yscroll_old, add='+')
-        containing_frame.bind_all('<MouseWheel>', yscroll_old, add='+')
-        containing_frame.bind_all('<Shift-MouseWheel>', xscroll_old, add='+')
+        containing_frame.bind_all('<4>', yscroll_old, add="+")
+        containing_frame.bind_all('<5>', yscroll_old, add="+")
+        containing_frame.bind_all("<MouseWheel>", yscroll_old, add="+")
+        containing_frame.bind_all("<Shift-MouseWheel>", xscroll_old, add="+")
 
     # Chr0nic
     def testMouseHook(em):
         containing_frame.unbind_all('<4>')
         containing_frame.unbind_all('<5>')
-        containing_frame.unbind_all('<MouseWheel>')
-        containing_frame.unbind_all('<Shift-MouseWheel>')
+        containing_frame.unbind_all("<MouseWheel>")
+        containing_frame.unbind_all("<Shift-MouseWheel>")
 
     # Chr0nic
     def testMouseUnhook(em):
-        containing_frame.bind_all('<4>', yscroll_old, add='+')
-        containing_frame.bind_all('<5>', yscroll_old, add='+')
-        containing_frame.bind_all('<MouseWheel>', yscroll_old, add='+')
-        containing_frame.bind_all('<Shift-MouseWheel>', xscroll_old, add='+')
+        containing_frame.bind_all('<4>', yscroll_old, add="+")
+        containing_frame.bind_all('<5>', yscroll_old, add="+")
+        containing_frame.bind_all("<MouseWheel>", yscroll_old, add="+")
+        containing_frame.bind_all("<Shift-MouseWheel>", xscroll_old, add="+")
 
     def _char_width_in_pixels(font):
         return tkinter.font.Font(font=font).measure('A')  # single character width
 
     def _char_height_in_pixels(font):
         return tkinter.font.Font(font=font).metrics('linespace')
 
@@ -15534,24 +15534,24 @@
 
     def _add_grab(element):
 
         try:
             if form.Grab is True or element.Grab is True:
                 # if something already about to the button, then don't do the grab stuff
                 if '<Button-1>' not in element.Widget.bind():
-                    element.Widget.bind('<ButtonPress-1>', toplevel_form._StartMoveGrabAnywhere)
-                    element.Widget.bind('<ButtonRelease-1>', toplevel_form._StopMove)
-                    element.Widget.bind('<B1-Motion>', toplevel_form._OnMotionGrabAnywhere)
-                element.ParentRowFrame.bind('<ButtonPress-1>', toplevel_form._StartMoveGrabAnywhere)
-                element.ParentRowFrame.bind('<ButtonRelease-1>', toplevel_form._StopMove)
-                element.ParentRowFrame.bind('<B1-Motion>', toplevel_form._OnMotionGrabAnywhere)
+                    element.Widget.bind("<ButtonPress-1>", toplevel_form._StartMoveGrabAnywhere)
+                    element.Widget.bind("<ButtonRelease-1>", toplevel_form._StopMove)
+                    element.Widget.bind("<B1-Motion>", toplevel_form._OnMotionGrabAnywhere)
+                element.ParentRowFrame.bind("<ButtonPress-1>", toplevel_form._StartMoveGrabAnywhere)
+                element.ParentRowFrame.bind("<ButtonRelease-1>", toplevel_form._StopMove)
+                element.ParentRowFrame.bind("<B1-Motion>", toplevel_form._OnMotionGrabAnywhere)
                 if element.Type == ELEM_TYPE_COLUMN:
-                    element.TKColFrame.canvas.bind('<ButtonPress-1>', toplevel_form._StartMoveGrabAnywhere)
-                    element.TKColFrame.canvas.bind('<ButtonRelease-1>', toplevel_form._StopMove)
-                    element.TKColFrame.canvas.bind('<B1-Motion>', toplevel_form._OnMotionGrabAnywhere)
+                    element.TKColFrame.canvas.bind("<ButtonPress-1>", toplevel_form._StartMoveGrabAnywhere)
+                    element.TKColFrame.canvas.bind("<ButtonRelease-1>", toplevel_form._StopMove)
+                    element.TKColFrame.canvas.bind("<B1-Motion>", toplevel_form._OnMotionGrabAnywhere)
         except Exception as e:
             pass
             # print(e)
 
     def _add_right_click_menu_and_grab(element):
         if element.RightClickMenu == MENU_RIGHT_CLICK_DISABLED:
             return
@@ -15899,15 +15899,15 @@
                     bc = DEFAULT_BUTTON_COLOR
 
                 bd = element.BorderWidth
                 pos = -1
                 if DEFAULT_USE_BUTTON_SHORTCUTS is True:
                     pos = btext.find(MENU_SHORTCUT_CHARACTER)
                     if pos != -1:
-                        if pos < len(MENU_SHORTCUT_CHARACTER) or btext[pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                        if pos < len(MENU_SHORTCUT_CHARACTER) or btext[pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                             btext = btext[:pos] + btext[pos + len(MENU_SHORTCUT_CHARACTER):]
                         else:
                             btext = btext.replace('\\'+MENU_SHORTCUT_CHARACTER, MENU_SHORTCUT_CHARACTER)
                             pos = -1
                 tkbutton = element.Widget = tk.Button(tk_row_frame, text=btext, width=width, height=height, justify=tk.CENTER, bd=bd, font=font)
                 if pos != -1:
                     tkbutton.config(underline=pos)
@@ -16032,15 +16032,15 @@
                 element.TKStringVar = stringvar
                 element.Location = (row_num, col_num)
                 btext = element.ButtonText
                 pos = -1
                 if DEFAULT_USE_BUTTON_SHORTCUTS is True:
                     pos = btext.find(MENU_SHORTCUT_CHARACTER)
                     if pos != -1:
-                        if pos < len(MENU_SHORTCUT_CHARACTER) or btext[pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                        if pos < len(MENU_SHORTCUT_CHARACTER) or btext[pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                             btext = btext[:pos] + btext[pos + len(MENU_SHORTCUT_CHARACTER):]
                         else:
                             btext = btext.replace('\\'+MENU_SHORTCUT_CHARACTER, MENU_SHORTCUT_CHARACTER)
                             pos = -1
                 btype = element.BType
                 if element.AutoSizeButton is not None:
                     auto_size = element.AutoSizeButton
@@ -16254,15 +16254,15 @@
 
             # -------------------------  INPUT placement element  ------------------------- #
             elif element_type == ELEM_TYPE_INPUT_TEXT:
                 element = element  # type: InputText
                 default_text = element.DefaultText
                 element.TKStringVar = tk.StringVar()
                 element.TKStringVar.set(default_text)
-                show = element.PasswordCharacter if element.PasswordCharacter else ''
+                show = element.PasswordCharacter if element.PasswordCharacter else ""
                 bd = border_depth
                 if element.Justification is not None:
                     justification = element.Justification
                 else:
                     justification = DEFAULT_TEXT_JUSTIFICATION
                 justify = tk.LEFT if justification.startswith('l') else tk.CENTER if justification.startswith('c') else tk.RIGHT
                 # anchor = tk.NW if justification == 'left' else tk.N if justification == 'center' else tk.NE
@@ -16356,30 +16356,30 @@
                     _error_popup_with_traceback('Combo Element error {}'.format(e),
                                                 'Combo element key: {}'.format(element.Key),
                                                 'One of your colors is bad. Check the text, background, button background and button arrow colors',
                                                 "Parent Window's Title: {}".format(toplevel_form.Title))
 
                 # Strange code that is needed to set the font for the drop-down list
                 element._dropdown_newfont = tkinter.font.Font(font=font)
-                tk_row_frame.option_add('*TCombobox*Listbox*Font', element._dropdown_newfont)
+                tk_row_frame.option_add("*TCombobox*Listbox*Font", element._dropdown_newfont)
 
                 element.TKCombo = element.Widget = ttk.Combobox(tk_row_frame, width=width, textvariable=element.TKStringVar, font=font, style=style_name)
 
                 # make tcl call to deal with colors for the drop-down formatting
                 try:
                     if element.BackgroundColor not in (None, COLOR_SYSTEM_DEFAULT) and \
                         element.TextColor not in (None, COLOR_SYSTEM_DEFAULT):
                         element.Widget.tk.eval(
                     '[ttk::combobox::PopdownWindow {}].f.l configure -foreground {} -background {} -selectforeground {} -selectbackground {}'.format(element.Widget, element.TextColor, element.BackgroundColor, element.BackgroundColor, element.TextColor))
                 except Exception as e:
                     pass    # going to let this one slide
 
                 # Chr0nic
-                element.TKCombo.bind('<Enter>', lambda event, em=element: testMouseHook2(em))
-                element.TKCombo.bind('<Leave>', lambda event, em=element: testMouseUnhook2(em))
+                element.TKCombo.bind("<Enter>", lambda event, em=element: testMouseHook2(em))
+                element.TKCombo.bind("<Leave>", lambda event, em=element: testMouseUnhook2(em))
 
                 if toplevel_form.UseDefaultFocus and not toplevel_form.FocusSet:
                     toplevel_form.FocusSet = True
                     element.TKCombo.focus_set()
 
                 if element.Size[1] != 1 and element.Size[1] is not None:
                     element.TKCombo.configure(height=element.Size[1])
@@ -16495,16 +16495,16 @@
                 if element.HorizontalScroll:
                     _make_ttk_scrollbar(element, 'h', toplevel_form)
                     element.hsb.pack(side=tk.BOTTOM, fill='x')
                     element.Widget.configure(xscrollcommand=element.hsb.set)
 
                 if not element.NoScrollbar or element.HorizontalScroll:
                     # Chr0nic
-                    element.Widget.bind('<Enter>', lambda event, em=element: testMouseHook(em))
-                    element.Widget.bind('<Leave>', lambda event, em=element: testMouseUnhook(em))
+                    element.Widget.bind("<Enter>", lambda event, em=element: testMouseHook(em))
+                    element.Widget.bind("<Leave>", lambda event, em=element: testMouseUnhook(em))
 
                 # else:
                 #     element.TKText.config(wrap='word')
 
                 # if not element.NoScrollbar:
                 #     # Vertical scrollbar
                 #     element.vsb = tk.Scrollbar(element_frame, orient="vertical", command=element.TKListbox.yview)
@@ -16572,56 +16572,56 @@
                 if element.wrap_lines is True:
                     element.TKText.config(wrap='word')
                 elif element.wrap_lines is False:
                     element.TKText.config(wrap='none')
 
                 if not element.no_scrollbar or element.HorizontalScroll:
                     # Chr0nic
-                    element.TKText.bind('<Enter>', lambda event, em=element: testMouseHook(em))
-                    element.TKText.bind('<Leave>', lambda event, em=element: testMouseUnhook(em))
+                    element.TKText.bind("<Enter>", lambda event, em=element: testMouseHook(em))
+                    element.TKText.bind("<Leave>", lambda event, em=element: testMouseUnhook(em))
 
                 if element.DefaultText:
                     element.TKText.insert(1.0, element.DefaultText)  # set the default text
                 element.TKText.config(highlightthickness=0)
                 if text_color is not None and text_color != COLOR_SYSTEM_DEFAULT:
                     element.TKText.configure(fg=text_color, selectbackground=text_color)
                     element.TKText.config(insertbackground=text_color)
                 if element.BackgroundColor is not None and element.BackgroundColor != COLOR_SYSTEM_DEFAULT:
                     element.TKText.configure(background=element.BackgroundColor, selectforeground=element.BackgroundColor)
                 if element.selected_background_color not in (None, COLOR_SYSTEM_DEFAULT):
                     element.TKText.configure(selectbackground=element.selected_background_color)
                 if element.selected_text_color not in (None, COLOR_SYSTEM_DEFAULT):
                     element.TKText.configure(selectforeground=element.selected_text_color)
-                element.TKText.tag_configure('center', justify='center')
-                element.TKText.tag_configure('left', justify='left')
-                element.TKText.tag_configure('right', justify='right')
+                element.TKText.tag_configure("center", justify='center')
+                element.TKText.tag_configure("left", justify='left')
+                element.TKText.tag_configure("right", justify='right')
 
                 if element.Justification.startswith('l'):
-                    element.TKText.tag_add('left', 1.0, 'end')
+                    element.TKText.tag_add("left", 1.0, "end")
                     element.justification_tag = 'left'
                 elif element.Justification.startswith('r'):
-                    element.TKText.tag_add('right', 1.0, 'end')
+                    element.TKText.tag_add("right", 1.0, "end")
                     element.justification_tag = 'right'
                 elif element.Justification.startswith('c'):
-                    element.TKText.tag_add('center', 1.0, 'end')
+                    element.TKText.tag_add("center", 1.0, "end")
                     element.justification_tag = 'center'
                 # if DEFAULT_SCROLLBAR_COLOR not in (None, COLOR_SYSTEM_DEFAULT):               # only works on Linux so not including it
                 #     element.TKText.vbar.config(troughcolor=DEFAULT_SCROLLBAR_COLOR)
                 expand, fill, row_should_expand, row_fill_direction = _add_expansion(element, row_should_expand, row_fill_direction)
 
                 element.element_frame.pack(side=tk.LEFT, padx=elementpad[0], pady=elementpad[1], fill=fill, expand=expand)
                 element.Widget.pack(side=tk.LEFT, fill=fill, expand=expand)
 
                 if element.visible is False:
                     element._pack_forget_save_settings(alternate_widget=element_frame)
                     # element.element_frame.pack_forget()
                 else:
                     # Chr0nic
-                    element.TKText.bind('<Enter>', lambda event, em=element: testMouseHook(em))
-                    element.TKText.bind('<Leave>', lambda event, em=element: testMouseUnhook(em))
+                    element.TKText.bind("<Enter>", lambda event, em=element: testMouseHook(em))
+                    element.TKText.bind("<Leave>", lambda event, em=element: testMouseUnhook(em))
                 if element.ChangeSubmits:
                     element.TKText.bind('<Key>', element._KeyboardHandler)
                 if element.EnterSubmits:
                     element.TKText.bind('<Return>', element._ReturnKeyHandler)
                 if element.Focus is True or (toplevel_form.UseDefaultFocus and not toplevel_form.FocusSet):
                     toplevel_form.FocusSet = True
                     element.TKText.focus_set()
@@ -16695,17 +16695,17 @@
                     progress_width = element_size[1]
                 direction = element.Orientation
                 if element.BarColor != (None, None):  # if element has a bar color, use it
                     bar_color = element.BarColor
                 else:
                     bar_color = DEFAULT_PROGRESS_BAR_COLOR
                 if element.Orientation.lower().startswith('h'):
-                    base_style_name = '.Horizontal.TProgressbar'
+                    base_style_name = ".Horizontal.TProgressbar"
                 else:
-                    base_style_name = '.Vertical.TProgressbar'
+                    base_style_name = ".Vertical.TProgressbar"
                 style_name = _make_ttk_style_name(base_style_name, element, primary_style=True)
                 element.TKProgressBar = TKProgressBar(tk_row_frame, element.MaxValue, progress_length, progress_width,
                                                       orientation=direction, BarColor=bar_color,
                                                       border_width=element.BorderWidth, relief=element.Relief,
                                                       ttk_theme=toplevel_form.TtkTheme, key=element.Key, style_name=style_name)
                 element.Widget = element.TKProgressBar.TKProgressBarForReal
                 expand, fill, row_should_expand, row_fill_direction = _add_expansion(element, row_should_expand, row_fill_direction)
@@ -16926,15 +16926,15 @@
                     if element.DisabledTextColor not in (COLOR_SYSTEM_DEFAULT, None):
                         baritem.config(disabledforeground=element.DisabledTextColor)
                     if font is not None:
                         baritem.config(font=font)
                     pos = menu_entry[0].find(MENU_SHORTCUT_CHARACTER)
                     # print(pos)
                     if pos != -1:
-                        if pos == 0 or menu_entry[0][pos - len(MENU_SHORTCUT_CHARACTER)] != '\\':
+                        if pos == 0 or menu_entry[0][pos - len(MENU_SHORTCUT_CHARACTER)] != "\\":
                             menu_entry[0] = menu_entry[0][:pos] + menu_entry[0][pos + 1:]
                     if menu_entry[0][0] == MENU_DISABLED_CHARACTER:
                         menubar.add_cascade(label=menu_entry[0][len(MENU_DISABLED_CHARACTER):], menu=baritem,
                                             underline=pos - 1)
                         menubar.entryconfig(menu_entry[0][len(MENU_DISABLED_CHARACTER):], state='disabled')
                     else:
                         menubar.add_cascade(label=menu_entry[0], menu=baritem, underline=pos)
@@ -17068,17 +17068,17 @@
                     style.configure(custom_style, tabposition=tab_position)
 
                 if element.BackgroundColor is not None and element.BackgroundColor != COLOR_SYSTEM_DEFAULT:
                     style.configure(custom_style, background=element.BackgroundColor)
 
                 # FINALLY the proper styling to get tab colors!
                 if element.SelectedTitleColor is not None and element.SelectedTitleColor != COLOR_SYSTEM_DEFAULT:
-                    style.map(custom_style + '.Tab', foreground=[('selected', element.SelectedTitleColor)])
+                    style.map(custom_style + '.Tab', foreground=[("selected", element.SelectedTitleColor)])
                 if element.SelectedBackgroundColor is not None and element.SelectedBackgroundColor != COLOR_SYSTEM_DEFAULT:
-                    style.map(custom_style + '.Tab', background=[('selected', element.SelectedBackgroundColor)])
+                    style.map(custom_style + '.Tab', background=[("selected", element.SelectedBackgroundColor)])
                 if element.TabBackgroundColor is not None and element.TabBackgroundColor != COLOR_SYSTEM_DEFAULT:
                     style.configure(custom_style + '.Tab', background=element.TabBackgroundColor)
                 if element.TextColor is not None and element.TextColor != COLOR_SYSTEM_DEFAULT:
                     style.configure(custom_style + '.Tab', foreground=element.TextColor)
                 if element.BorderWidth is not None:
                     style.configure(custom_style, borderwidth=element.BorderWidth)
                 if element.TabBorderWidth is not None:
@@ -17280,29 +17280,29 @@
                 if element.HeaderRelief is not None:
                     table_style.configure(style_name + '.Heading', relief=element.HeaderRelief)
                 table_style.configure(style_name, font=font)
                 if element.BorderWidth is not None:
                     table_style.configure(style_name, borderwidth=element.BorderWidth)
 
                 if element.HeaderBackgroundColor not in  (None, COLOR_SYSTEM_DEFAULT) and  element.HeaderTextColor not in  (None, COLOR_SYSTEM_DEFAULT):
-                    table_style.map(style_name + '.Heading', background=[('pressed', '!focus', element.HeaderBackgroundColor),
+                    table_style.map(style_name + ".Heading", background=[('pressed', '!focus', element.HeaderBackgroundColor),
                                                                          ('active', element.HeaderTextColor),])
-                    table_style.map(style_name + '.Heading', foreground=[('pressed', '!focus', element.HeaderTextColor),
+                    table_style.map(style_name + ".Heading", foreground=[('pressed', '!focus', element.HeaderTextColor),
                                                                          ('active', element.HeaderBackgroundColor),])
 
                 treeview.configure(style=style_name)
                 # scrollable_frame.pack(side=tk.LEFT,  padx=elementpad[0], pady=elementpad[1], expand=True, fill='both')
                 if element.enable_click_events is True:
                     treeview.bind('<ButtonRelease-1>', element._table_clicked)
                 if element.right_click_selects:
                     if running_mac():
                         treeview.bind('<Button-2>', element._table_clicked)
                     else:
                         treeview.bind('<Button-3>', element._table_clicked)
-                treeview.bind('<<TreeviewSelect>>', element._treeview_selected)
+                treeview.bind("<<TreeviewSelect>>", element._treeview_selected)
                 if element.BindReturnKey:
                     treeview.bind('<Return>', element._treeview_double_click)
                     treeview.bind('<Double-Button-1>', element._treeview_double_click)
 
 
 
 
@@ -17317,16 +17317,16 @@
                     # element.Widget.config(wrap='none')
                     _make_ttk_scrollbar(element, 'h', toplevel_form)
                     element.hsb.pack(side=tk.BOTTOM, fill='x')
                     element.Widget.configure(xscrollcommand=element.hsb.set)
 
                 if not element.HideVerticalScroll or not element.VerticalScrollOnly:
                     # Chr0nic
-                    element.Widget.bind('<Enter>', lambda event, em=element: testMouseHook(em))
-                    element.Widget.bind('<Leave>', lambda event, em=element: testMouseUnhook(em))
+                    element.Widget.bind("<Enter>", lambda event, em=element: testMouseHook(em))
+                    element.Widget.bind("<Leave>", lambda event, em=element: testMouseUnhook(em))
 
 
 
                 # if not element.HideVerticalScroll:
                 #     scrollbar = tk.Scrollbar(frame)
                 #     scrollbar.pack(side=tk.RIGHT, fill='y')
                 #     scrollbar.config(command=treeview.yview)
@@ -17494,16 +17494,16 @@
                     # element.Widget.config(wrap='none')
                     _make_ttk_scrollbar(element, 'h', toplevel_form)
                     element.hsb.pack(side=tk.BOTTOM, fill='x')
                     element.Widget.configure(xscrollcommand=element.hsb.set)
 
                 if not element.HideVerticalScroll or not element.VerticalScrollOnly:
                     # Chr0nic
-                    element.Widget.bind('<Enter>', lambda event, em=element: testMouseHook(em))
-                    element.Widget.bind('<Leave>', lambda event, em=element: testMouseUnhook(em))
+                    element.Widget.bind("<Enter>", lambda event, em=element: testMouseHook(em))
+                    element.Widget.bind("<Leave>", lambda event, em=element: testMouseUnhook(em))
 
 
                 # Horizontal scrollbar
                 # if not element.VerticalScrollOnly:
                 #     element.TKText.config(wrap='none')
                 #     _make_ttk_scrollbar(element, 'h')
                 #     element.hsb.pack(side=tk.BOTTOM, fill='x')
@@ -17526,15 +17526,15 @@
 
                 expand, fill, row_should_expand, row_fill_direction = _add_expansion(element, row_should_expand, row_fill_direction)
                 element.TKTreeview.pack(side=tk.LEFT, padx=0, pady=0, expand=expand, fill=fill)
                 element_frame.pack(side=tk.LEFT, padx=elementpad[0], pady=elementpad[1], expand=expand, fill=fill)
                 if element.visible is False:
                     element._pack_forget_save_settings(alternate_widget=element.element_frame)       # seems like it should be the frame if following other elements conventions
                     # element.TKTreeview.pack_forget()
-                treeview.bind('<<TreeviewSelect>>', element._treeview_selected)
+                treeview.bind("<<TreeviewSelect>>", element._treeview_selected)
                 if element.Tooltip is not None:  # tooltip
                     element.TooltipObject = ToolTip(element.TKTreeview, text=element.Tooltip,
                                                     timeout=DEFAULT_TOOLTIP_TIME)
                 _add_right_click_menu_and_grab(element)
 
                 if tclversion_detailed == '8.6.9' and ENABLE_TREEVIEW_869_PATCH:
                     # print('*** tk version 8.6.9 detected.... patching ttk treeview code ***')
@@ -17542,15 +17542,15 @@
                                    foreground=_fixed_map(tree_style, style_name, 'foreground', element.SelectedRowColors),
                                    background=_fixed_map(tree_style, style_name, 'background', element.SelectedRowColors))
 
             # -------------------------  Separator placement element  ------------------------- #
             elif element_type == ELEM_TYPE_SEPARATOR:
                 element = element  # type: VerticalSeparator
                 # style_name = str(element.Key) + "Line.TSeparator"
-                style_name = _make_ttk_style_name('.Line.TSeparator', element, primary_style=True)
+                style_name = _make_ttk_style_name(".Line.TSeparator", element, primary_style=True)
                 style = ttk.Style()
 
                 _change_ttk_theme(style, toplevel_form.TtkTheme)
 
                 if element.color not in (None, COLOR_SYSTEM_DEFAULT):
                     style.configure(style_name, background=element.color)
                 separator = element.Widget = ttk.Separator(tk_row_frame, orient=element.Orientation, )
@@ -17561,15 +17561,15 @@
                     separator.pack(side=tk.LEFT, padx=elementpad[0], pady=elementpad[1], fill=tk.X, expand=True)
                 else:
                     separator.pack(side=tk.LEFT, padx=elementpad[0], pady=elementpad[1], fill=tk.Y, expand=False)
                 element.Widget.configure(style=style_name)  # IMPORTANT!  Apply the style
             # -------------------------  SizeGrip placement element  ------------------------- #
             elif element_type == ELEM_TYPE_SIZEGRIP:
                 element = element  # type: Sizegrip
-                style_name = 'Sizegrip.TSizegrip'
+                style_name = "Sizegrip.TSizegrip"
                 style = ttk.Style()
 
                 _change_ttk_theme(style, toplevel_form.TtkTheme)
 
                 size_grip = element.Widget = ttk.Sizegrip(tk_row_frame)
                 toplevel_form.sizegrip_widget = size_grip
                 # if no size is specified, then use the background color for the window
@@ -17711,15 +17711,15 @@
     :param window:          window to turn off the titlebar if indicated in the settings
     :type window:           Window
     """
     try:
         if window.NoTitleBar:
             if running_linux():
                 # window.TKroot.wm_attributes("-type", 'splash')
-                window.TKroot.wm_attributes('-type', 'dock')
+                window.TKroot.wm_attributes("-type", 'dock')
             else:
                 window.TKroot.wm_overrideredirect(True)
                 # Special case for Mac. Need to clear flag again if not tkinter version 8.6.10+
                 # Previously restricted patch to only certain tkinter versions. Now use the patch setting exclusively regardless of tk ver
                 # if running_mac() and ENABLE_MAC_NOTITLEBAR_PATCH and (sum([int(i) for i in tclversion_detailed.split('.')]) < 24):
                 # if running_mac() and ENABLE_MAC_NOTITLEBAR_PATCH:
                 if _mac_should_apply_notitlebar_patch():
@@ -17743,15 +17743,15 @@
     PackFormIntoFrame(window, master, window)
 
     window.TKroot.configure(padx=window.Margins[0], pady=window.Margins[1])
 
 
     # ....................................... DONE creating and laying out window ..........................#
     if window._Size != (None, None):
-        master.geometry('%sx%s' % (window._Size[0], window._Size[1]))
+        master.geometry("%sx%s" % (window._Size[0], window._Size[1]))
     screen_width = master.winfo_screenwidth()  # get window info to move to middle of screen
     screen_height = master.winfo_screenheight()
     if window.Location is not None:
         if window.Location != (None, None):
             x, y = window.Location
         elif DEFAULT_WINDOW_LOCATION != (None, None):
             x, y = DEFAULT_WINDOW_LOCATION
@@ -17848,18 +17848,18 @@
     if not running_mac():
         _no_titlebar_setup(window)
 
     if not window.Resizable:
         root.resizable(False, False)
 
     if window.DisableMinimize:
-        root.attributes('-toolwindow', 1)
+        root.attributes("-toolwindow", 1)
 
     if window.KeepOnTop:
-        root.wm_attributes('-topmost', 1)
+        root.wm_attributes("-topmost", 1)
 
     if window.TransparentColor is not None:
         window.SetTransparentColor(window.TransparentColor)
 
     if window.scaling is not None:
         root.tk.call('tk', 'scaling', window.scaling)
 
@@ -17868,46 +17868,46 @@
     # root.bind('<Destroy>', MyFlexForm.DestroyedCallback())
     _convert_window_to_tk(window)
 
     # Make moveable window
     if (window.GrabAnywhere is not False and not (
             window.NonBlocking and window.GrabAnywhere is not True)):
         if not (ENABLE_MAC_DISABLE_GRAB_ANYWHERE_WITH_TITLEBAR and running_mac() and not window.NoTitleBar):
-            root.bind('<ButtonPress-1>', window._StartMoveGrabAnywhere)
-            root.bind('<ButtonRelease-1>', window._StopMove)
-            root.bind('<B1-Motion>', window._OnMotionGrabAnywhere)
+            root.bind("<ButtonPress-1>", window._StartMoveGrabAnywhere)
+            root.bind("<ButtonRelease-1>", window._StopMove)
+            root.bind("<B1-Motion>", window._OnMotionGrabAnywhere)
     if (window.GrabAnywhereUsingControlKey is not False and not (
             window.NonBlocking and window.GrabAnywhereUsingControlKey is not True)):
-        root.bind('<Control-Button-1>', window._StartMoveUsingControlKey)
-        root.bind('<Control-ButtonRelease-1>', window._StopMove)
-        root.bind('<Control-B1-Motion>', window._OnMotionUsingControlKey)
+        root.bind("<Control-Button-1>", window._StartMoveUsingControlKey)
+        root.bind("<Control-ButtonRelease-1>", window._StopMove)
+        root.bind("<Control-B1-Motion>", window._OnMotionUsingControlKey)
         # also enable movement using Control + Arrow key
-        root.bind('<Control-Left>', window._move_callback)
-        root.bind('<Control-Right>', window._move_callback)
-        root.bind('<Control-Up>', window._move_callback)
-        root.bind('<Control-Down>', window._move_callback)
+        root.bind("<Control-Left>", window._move_callback)
+        root.bind("<Control-Right>", window._move_callback)
+        root.bind("<Control-Up>", window._move_callback)
+        root.bind("<Control-Down>", window._move_callback)
 
     window.set_icon(window.WindowIcon)
     try:
         alpha_channel = 1 if window.AlphaChannel is None else window.AlphaChannel
         root.attributes('-alpha', alpha_channel)  # Make window visible again
     except Exception as e:
         print('**** Error setting Alpha Channel to {} after window was created ****'.format(alpha_channel), e)
         # pass
 
     if window.ReturnKeyboardEvents and not window.NonBlocking:
-        root.bind('<KeyRelease>', window._KeyboardCallback)
-        root.bind('<MouseWheel>', window._MouseWheelCallback)
-        root.bind('<Button-4>', window._MouseWheelCallback)
-        root.bind('<Button-5>', window._MouseWheelCallback)
+        root.bind("<KeyRelease>", window._KeyboardCallback)
+        root.bind("<MouseWheel>", window._MouseWheelCallback)
+        root.bind("<Button-4>", window._MouseWheelCallback)
+        root.bind("<Button-5>", window._MouseWheelCallback)
     elif window.ReturnKeyboardEvents:
-        root.bind('<Key>', window._KeyboardCallback)
-        root.bind('<MouseWheel>', window._MouseWheelCallback)
-        root.bind('<Button-4>', window._MouseWheelCallback)
-        root.bind('<Button-5>', window._MouseWheelCallback)
+        root.bind("<Key>", window._KeyboardCallback)
+        root.bind("<MouseWheel>", window._MouseWheelCallback)
+        root.bind("<Button-4>", window._MouseWheelCallback)
+        root.bind("<Button-5>", window._MouseWheelCallback)
 
     DEFAULT_WINDOW_SNAPSHOT_KEY_CODE = main_global_get_screen_snapshot_symcode()
 
     if DEFAULT_WINDOW_SNAPSHOT_KEY_CODE:
         # print('**** BINDING THE SNAPSHOT!', DEFAULT_WINDOW_SNAPSHOT_KEY_CODE, DEFAULT_WINDOW_SNAPSHOT_KEY)
         window.bind(DEFAULT_WINDOW_SNAPSHOT_KEY_CODE, DEFAULT_WINDOW_SNAPSHOT_KEY, propagate=False)
         # window.bind('<Win_L><F12>', DEFAULT_WINDOW_SNAPSHOT_KEY, )
@@ -17921,28 +17921,28 @@
             window._start_autoclose_timer()
             # duration = DEFAULT_AUTOCLOSE_TIME if window.AutoCloseDuration is None else window.AutoCloseDuration
             # window.TKAfterID = root.after(int(duration * 1000), window._AutoCloseAlarmCallback)
 
     if window.Timeout != None:
         window.TKAfterID = root.after(int(window.Timeout), window._TimeoutAlarmCallback)
     if window.NonBlocking:
-        window.TKroot.protocol('WM_DESTROY_WINDOW', window._OnClosingCallback)
-        window.TKroot.protocol('WM_DELETE_WINDOW', window._OnClosingCallback)
+        window.TKroot.protocol("WM_DESTROY_WINDOW", window._OnClosingCallback)
+        window.TKroot.protocol("WM_DELETE_WINDOW", window._OnClosingCallback)
 
     else:  # it's a blocking form
         # print('..... CALLING MainLoop')
         window.CurrentlyRunningMainloop = True
-        window.TKroot.protocol('WM_DESTROY_WINDOW', window._OnClosingCallback)
-        window.TKroot.protocol('WM_DELETE_WINDOW', window._OnClosingCallback)
+        window.TKroot.protocol("WM_DESTROY_WINDOW", window._OnClosingCallback)
+        window.TKroot.protocol("WM_DELETE_WINDOW", window._OnClosingCallback)
 
         if window.modal or DEFAULT_MODAL_WINDOWS_FORCED:
             window.make_modal()
 
         if window.enable_window_config_events:
-            window.TKroot.bind('<Configure>', window._config_callback)
+            window.TKroot.bind("<Configure>", window._config_callback)
 
         # ----------------------------------- tkinter mainloop call -----------------------------------
         Window._window_running_mainloop = window
         Window._root_running_mainloop = window.TKroot
         window.TKroot.mainloop()
         window.CurrentlyRunningMainloop = False
         window.TimerCancelled = True
@@ -18165,18 +18165,18 @@
             total_seconds = 1
         try:
             time_per_item = total_seconds / self.current_value
         except:
             time_per_item = 1
         seconds_remaining = (self.max_value - self.current_value) * time_per_item
         time_remaining = str(datetime.timedelta(seconds=seconds_remaining))
-        time_remaining_short = (time_remaining).split('.')[0]
-        time_delta_short = str(time_delta).split('.')[0]
+        time_remaining_short = (time_remaining).split(".")[0]
+        time_delta_short = str(time_delta).split(".")[0]
         total_time = time_delta + datetime.timedelta(seconds=seconds_remaining)
-        total_time_short = str(total_time).split('.')[0]
+        total_time_short = str(total_time).split(".")[0]
         self.stat_messages = [
             '{} of {}'.format(self.current_value, self.max_value),
             '{} %'.format(100 * self.current_value // self.max_value),
             '',
             ' {:6.2f} Iterations per Second'.format(self.current_value / total_seconds),
             ' {:6.2f} Seconds per Iteration'.format(total_seconds / (self.current_value if self.current_value else 1)),
             '',
@@ -18263,15 +18263,15 @@
     color = color[1:]
     # convert the string into hex
     color = int(color, 16)
     # invert the three bytes
     # as good as substracting each of RGB component by 255(FF)
     comp_color = 0xFFFFFF ^ color
     # convert the color back to hex by prefixing a #
-    comp_color = '#%06X' % comp_color
+    comp_color = "#%06X" % comp_color
     return comp_color
 
 
 # ========================  EasyPrint           =====#
 # ===================================================#
 class _DebugWin():
     debug_window = None
@@ -19125,17 +19125,17 @@
                                                   path=DEFAULT_USER_SETTINGS_PYSIMPLEGUI_PATH)
 
     if keep_on_top is not None:
         DEFAULT_KEEP_ON_TOP = keep_on_top
 
     if dpi_awareness is True:
         if running_windows():
-            if platform.release() == '7':
+            if platform.release() == "7":
                 ctypes.windll.user32.SetProcessDPIAware()
-            elif platform.release() == '8' or platform.release() == '10':
+            elif platform.release() == "8" or platform.release() == "10":
                 ctypes.windll.shcore.SetProcessDpiAwareness(1)
 
     if scaling is not None:
         DEFAULT_SCALING = scaling
 
     if disable_modal_windows is not None:
         DEFAULT_MODAL_WINDOWS_ENABLED = not disable_modal_windows
@@ -19199,433 +19199,433 @@
 # The official Theme code
 
 #################### ChangeLookAndFeel #######################
 # Predefined settings that will change the colors and styles #
 # of the elements.                                           #
 ##############################################################
 LOOK_AND_FEEL_TABLE = {
-    'SystemDefault': {'BACKGROUND': COLOR_SYSTEM_DEFAULT, 'TEXT': COLOR_SYSTEM_DEFAULT, 'INPUT': COLOR_SYSTEM_DEFAULT, 'TEXT_INPUT': COLOR_SYSTEM_DEFAULT,
-                      'SCROLL': COLOR_SYSTEM_DEFAULT, 'BUTTON': OFFICIAL_PYSIMPLEGUI_BUTTON_COLOR, 'PROGRESS': COLOR_SYSTEM_DEFAULT, 'BORDER': 1,
-                      'SLIDER_DEPTH': 1, 'PROGRESS_DEPTH': 0, },
-    'SystemDefaultForReal': {'BACKGROUND': COLOR_SYSTEM_DEFAULT, 'TEXT': COLOR_SYSTEM_DEFAULT, 'INPUT': COLOR_SYSTEM_DEFAULT,
-                             'TEXT_INPUT': COLOR_SYSTEM_DEFAULT, 'SCROLL': COLOR_SYSTEM_DEFAULT, 'BUTTON': COLOR_SYSTEM_DEFAULT,
-                             'PROGRESS': COLOR_SYSTEM_DEFAULT, 'BORDER': 1, 'SLIDER_DEPTH': 1, 'PROGRESS_DEPTH': 0, },
-    'SystemDefault1': {'BACKGROUND': COLOR_SYSTEM_DEFAULT, 'TEXT': COLOR_SYSTEM_DEFAULT, 'INPUT': COLOR_SYSTEM_DEFAULT, 'TEXT_INPUT': COLOR_SYSTEM_DEFAULT,
-                       'SCROLL': COLOR_SYSTEM_DEFAULT, 'BUTTON': COLOR_SYSTEM_DEFAULT, 'PROGRESS': COLOR_SYSTEM_DEFAULT, 'BORDER': 1, 'SLIDER_DEPTH': 1,
-                       'PROGRESS_DEPTH': 0, },
-    'Material1': {'BACKGROUND': '#E3F2FD', 'TEXT': '#000000', 'INPUT': '#86A8FF', 'TEXT_INPUT': '#000000', 'SCROLL': '#86A8FF',
-                  'BUTTON': ('#FFFFFF', '#5079D3'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 0, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'ACCENT1': '#FF0266', 'ACCENT2': '#FF5C93', 'ACCENT3': '#C5003C', },
-    'Material2': {'BACKGROUND': '#FAFAFA', 'TEXT': '#000000', 'INPUT': '#004EA1', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#5EA7FF',
-                  'BUTTON': ('#FFFFFF', '#0079D3'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 0, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'ACCENT1': '#FF0266', 'ACCENT2': '#FF5C93', 'ACCENT3': '#C5003C', },
-    'Reddit': {'BACKGROUND': '#ffffff', 'TEXT': '#1a1a1b', 'INPUT': '#dae0e6', 'TEXT_INPUT': '#222222', 'SCROLL': '#a5a4a4', 'BUTTON': ('#FFFFFF', '#0079d3'),
-               'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, 'ACCENT1': '#ff5414', 'ACCENT2': '#33a8ff',
-               'ACCENT3': '#dbf0ff', },
-    'Topanga': {'BACKGROUND': '#282923', 'TEXT': '#E7DB74', 'INPUT': '#393a32', 'TEXT_INPUT': '#E7C855', 'SCROLL': '#E7C855', 'BUTTON': ('#E7C855', '#284B5A'),
-                'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, 'ACCENT1': '#c15226', 'ACCENT2': '#7a4d5f',
-                'ACCENT3': '#889743', },
-    'GreenTan': {'BACKGROUND': '#9FB8AD', 'TEXT': '#000000', 'INPUT': '#F7F3EC', 'TEXT_INPUT': '#000000', 'SCROLL': '#F7F3EC', 'BUTTON': ('#FFFFFF', '#475841'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Dark': {'BACKGROUND': '#404040', 'TEXT': '#FFFFFF', 'INPUT': '#4D4D4D', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#707070', 'BUTTON': ('#FFFFFF', '#004F00'),
-             'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightGreen': {'BACKGROUND': '#B7CECE', 'TEXT': '#000000', 'INPUT': '#FDFFF7', 'TEXT_INPUT': '#000000', 'SCROLL': '#FDFFF7',
-                   'BUTTON': ('#FFFFFF', '#658268'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'ACCENT1': '#76506d',
-                   'ACCENT2': '#5148f1', 'ACCENT3': '#0a1c84', 'PROGRESS_DEPTH': 0, },
-    'Dark2': {'BACKGROUND': '#404040', 'TEXT': '#FFFFFF', 'INPUT': '#FFFFFF', 'TEXT_INPUT': '#000000', 'SCROLL': '#707070', 'BUTTON': ('#FFFFFF', '#004F00'),
-              'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Black': {'BACKGROUND': '#000000', 'TEXT': '#FFFFFF', 'INPUT': '#4D4D4D', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#707070', 'BUTTON': ('#000000', '#FFFFFF'),
-              'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Black2': {'BACKGROUND': '#000000', 'TEXT': '#FFFFFF', 'INPUT': '#000000', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#FFFFFF', 'BUTTON': ('#000000', '#FFFFFF'),
-               'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Tan': {'BACKGROUND': '#fdf6e3', 'TEXT': '#268bd1', 'INPUT': '#eee8d5', 'TEXT_INPUT': '#6c71c3', 'SCROLL': '#eee8d5', 'BUTTON': ('#FFFFFF', '#063542'),
-            'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'TanBlue': {'BACKGROUND': '#e5dece', 'TEXT': '#063289', 'INPUT': '#f9f8f4', 'TEXT_INPUT': '#242834', 'SCROLL': '#eee8d5', 'BUTTON': ('#FFFFFF', '#063289'),
-                'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkTanBlue': {'BACKGROUND': '#242834', 'TEXT': '#dfe6f8', 'INPUT': '#97755c', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#a9afbb',
-                    'BUTTON': ('#FFFFFF', '#063289'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkAmber': {'BACKGROUND': '#2c2825', 'TEXT': '#fdcb52', 'INPUT': '#705e52', 'TEXT_INPUT': '#fdcb52', 'SCROLL': '#705e52',
-                  'BUTTON': ('#000000', '#fdcb52'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBlue': {'BACKGROUND': '#1a2835', 'TEXT': '#d1ecff', 'INPUT': '#335267', 'TEXT_INPUT': '#acc2d0', 'SCROLL': '#1b6497', 'BUTTON': ('#000000', '#fafaf8'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Reds': {'BACKGROUND': '#280001', 'TEXT': '#FFFFFF', 'INPUT': '#d8d584', 'TEXT_INPUT': '#000000', 'SCROLL': '#763e00', 'BUTTON': ('#000000', '#daad28'),
-             'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Green': {'BACKGROUND': '#82a459', 'TEXT': '#000000', 'INPUT': '#d8d584', 'TEXT_INPUT': '#000000', 'SCROLL': '#e3ecf3', 'BUTTON': ('#FFFFFF', '#517239'),
-              'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'BluePurple': {'BACKGROUND': '#A5CADD', 'TEXT': '#6E266E', 'INPUT': '#E0F5FF', 'TEXT_INPUT': '#000000', 'SCROLL': '#E0F5FF',
-                   'BUTTON': ('#FFFFFF', '#303952'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Purple': {'BACKGROUND': '#B0AAC2', 'TEXT': '#000000', 'INPUT': '#F2EFE8', 'SCROLL': '#F2EFE8', 'TEXT_INPUT': '#000000', 'BUTTON': ('#000000', '#C2D4D8'),
-               'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'BlueMono': {'BACKGROUND': '#AAB6D3', 'TEXT': '#000000', 'INPUT': '#F1F4FC', 'SCROLL': '#F1F4FC', 'TEXT_INPUT': '#000000', 'BUTTON': ('#FFFFFF', '#7186C7'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'GreenMono': {'BACKGROUND': '#A8C1B4', 'TEXT': '#000000', 'INPUT': '#DDE0DE', 'SCROLL': '#E3E3E3', 'TEXT_INPUT': '#000000',
-                  'BUTTON': ('#FFFFFF', '#6D9F85'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'BrownBlue': {'BACKGROUND': '#64778d', 'TEXT': '#FFFFFF', 'INPUT': '#f0f3f7', 'SCROLL': '#A6B2BE', 'TEXT_INPUT': '#000000',
-                  'BUTTON': ('#FFFFFF', '#283b5b'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'BrightColors': {'BACKGROUND': '#b4ffb4', 'TEXT': '#000000', 'INPUT': '#ffff64', 'SCROLL': '#ffb482', 'TEXT_INPUT': '#000000',
-                     'BUTTON': ('#000000', '#ffa0dc'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'NeutralBlue': {'BACKGROUND': '#92aa9d', 'TEXT': '#000000', 'INPUT': '#fcfff6', 'SCROLL': '#fcfff6', 'TEXT_INPUT': '#000000',
-                    'BUTTON': ('#000000', '#d0dbbd'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Kayak': {'BACKGROUND': '#a7ad7f', 'TEXT': '#000000', 'INPUT': '#e6d3a8', 'SCROLL': '#e6d3a8', 'TEXT_INPUT': '#000000', 'BUTTON': ('#FFFFFF', '#5d907d'),
-              'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'SandyBeach': {'BACKGROUND': '#efeccb', 'TEXT': '#012f2f', 'INPUT': '#e6d3a8', 'SCROLL': '#e6d3a8', 'TEXT_INPUT': '#012f2f',
-                   'BUTTON': ('#FFFFFF', '#046380'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'TealMono': {'BACKGROUND': '#a8cfdd', 'TEXT': '#000000', 'INPUT': '#dfedf2', 'SCROLL': '#dfedf2', 'TEXT_INPUT': '#000000', 'BUTTON': ('#FFFFFF', '#183440'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'Default': {'BACKGROUND': COLOR_SYSTEM_DEFAULT, 'TEXT': COLOR_SYSTEM_DEFAULT, 'INPUT': COLOR_SYSTEM_DEFAULT, 'TEXT_INPUT': COLOR_SYSTEM_DEFAULT,
-                'SCROLL': COLOR_SYSTEM_DEFAULT, 'BUTTON': OFFICIAL_PYSIMPLEGUI_BUTTON_COLOR, 'PROGRESS': COLOR_SYSTEM_DEFAULT, 'BORDER': 1, 'SLIDER_DEPTH': 1,
-                'PROGRESS_DEPTH': 0, },
-    'Default1': {'BACKGROUND': COLOR_SYSTEM_DEFAULT, 'TEXT': COLOR_SYSTEM_DEFAULT, 'INPUT': COLOR_SYSTEM_DEFAULT, 'TEXT_INPUT': COLOR_SYSTEM_DEFAULT,
-                 'SCROLL': COLOR_SYSTEM_DEFAULT, 'BUTTON': COLOR_SYSTEM_DEFAULT, 'PROGRESS': COLOR_SYSTEM_DEFAULT, 'BORDER': 1, 'SLIDER_DEPTH': 1,
-                 'PROGRESS_DEPTH': 0, },
-    'DefaultNoMoreNagging': {'BACKGROUND': COLOR_SYSTEM_DEFAULT, 'TEXT': COLOR_SYSTEM_DEFAULT, 'INPUT': COLOR_SYSTEM_DEFAULT,
-                             'TEXT_INPUT': COLOR_SYSTEM_DEFAULT, 'SCROLL': COLOR_SYSTEM_DEFAULT, 'BUTTON': OFFICIAL_PYSIMPLEGUI_BUTTON_COLOR,
-                             'PROGRESS': COLOR_SYSTEM_DEFAULT, 'BORDER': 1, 'SLIDER_DEPTH': 1, 'PROGRESS_DEPTH': 0, },
-    'GrayGrayGray': {'BACKGROUND': COLOR_SYSTEM_DEFAULT, 'TEXT': COLOR_SYSTEM_DEFAULT, 'INPUT': COLOR_SYSTEM_DEFAULT, 'TEXT_INPUT': COLOR_SYSTEM_DEFAULT,
-                     'SCROLL': COLOR_SYSTEM_DEFAULT, 'BUTTON': COLOR_SYSTEM_DEFAULT, 'PROGRESS': COLOR_SYSTEM_DEFAULT, 'BORDER': 1, 'SLIDER_DEPTH': 1,
-                     'PROGRESS_DEPTH': 0, },
-    'LightBlue': {'BACKGROUND': '#E3F2FD', 'TEXT': '#000000', 'INPUT': '#86A8FF', 'TEXT_INPUT': '#000000', 'SCROLL': '#86A8FF',
-                  'BUTTON': ('#FFFFFF', '#5079D3'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 0, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'ACCENT1': '#FF0266', 'ACCENT2': '#FF5C93', 'ACCENT3': '#C5003C', },
-    'LightGrey': {'BACKGROUND': '#FAFAFA', 'TEXT': '#000000', 'INPUT': '#004EA1', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#5EA7FF',
-                  'BUTTON': ('#FFFFFF', '#0079D3'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 0, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'ACCENT1': '#FF0266', 'ACCENT2': '#FF5C93', 'ACCENT3': '#C5003C', },
-    'LightGrey1': {'BACKGROUND': '#ffffff', 'TEXT': '#1a1a1b', 'INPUT': '#dae0e6', 'TEXT_INPUT': '#222222', 'SCROLL': '#a5a4a4',
-                   'BUTTON': ('#FFFFFF', '#0079d3'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'ACCENT1': '#ff5414', 'ACCENT2': '#33a8ff', 'ACCENT3': '#dbf0ff', },
-    'DarkBrown': {'BACKGROUND': '#282923', 'TEXT': '#E7DB74', 'INPUT': '#393a32', 'TEXT_INPUT': '#E7C855', 'SCROLL': '#E7C855',
-                  'BUTTON': ('#E7C855', '#284B5A'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'ACCENT1': '#c15226', 'ACCENT2': '#7a4d5f', 'ACCENT3': '#889743', },
-    'LightGreen1': {'BACKGROUND': '#9FB8AD', 'TEXT': '#000000', 'INPUT': '#F7F3EC', 'TEXT_INPUT': '#000000', 'SCROLL': '#F7F3EC',
-                    'BUTTON': ('#FFFFFF', '#475841'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey': {'BACKGROUND': '#404040', 'TEXT': '#FFFFFF', 'INPUT': '#4D4D4D', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#707070', 'BUTTON': ('#FFFFFF', '#004F00'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightGreen2': {'BACKGROUND': '#B7CECE', 'TEXT': '#000000', 'INPUT': '#FDFFF7', 'TEXT_INPUT': '#000000', 'SCROLL': '#FDFFF7',
-                    'BUTTON': ('#FFFFFF', '#658268'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'ACCENT1': '#76506d',
-                    'ACCENT2': '#5148f1', 'ACCENT3': '#0a1c84', 'PROGRESS_DEPTH': 0, },
-    'DarkGrey1': {'BACKGROUND': '#404040', 'TEXT': '#FFFFFF', 'INPUT': '#FFFFFF', 'TEXT_INPUT': '#000000', 'SCROLL': '#707070',
-                  'BUTTON': ('#FFFFFF', '#004F00'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBlack': {'BACKGROUND': '#000000', 'TEXT': '#FFFFFF', 'INPUT': '#4D4D4D', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#707070',
-                  'BUTTON': ('#000000', '#FFFFFF'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBrown': {'BACKGROUND': '#fdf6e3', 'TEXT': '#268bd1', 'INPUT': '#eee8d5', 'TEXT_INPUT': '#6c71c3', 'SCROLL': '#eee8d5',
-                   'BUTTON': ('#FFFFFF', '#063542'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBrown1': {'BACKGROUND': '#e5dece', 'TEXT': '#063289', 'INPUT': '#f9f8f4', 'TEXT_INPUT': '#242834', 'SCROLL': '#eee8d5',
-                    'BUTTON': ('#FFFFFF', '#063289'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBlue1': {'BACKGROUND': '#242834', 'TEXT': '#dfe6f8', 'INPUT': '#97755c', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#a9afbb',
-                  'BUTTON': ('#FFFFFF', '#063289'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBrown1': {'BACKGROUND': '#2c2825', 'TEXT': '#fdcb52', 'INPUT': '#705e52', 'TEXT_INPUT': '#fdcb52', 'SCROLL': '#705e52',
-                   'BUTTON': ('#000000', '#fdcb52'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBlue2': {'BACKGROUND': '#1a2835', 'TEXT': '#d1ecff', 'INPUT': '#335267', 'TEXT_INPUT': '#acc2d0', 'SCROLL': '#1b6497',
-                  'BUTTON': ('#000000', '#fafaf8'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBrown2': {'BACKGROUND': '#280001', 'TEXT': '#FFFFFF', 'INPUT': '#d8d584', 'TEXT_INPUT': '#000000', 'SCROLL': '#763e00',
-                   'BUTTON': ('#000000', '#daad28'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGreen': {'BACKGROUND': '#82a459', 'TEXT': '#000000', 'INPUT': '#d8d584', 'TEXT_INPUT': '#000000', 'SCROLL': '#e3ecf3',
-                  'BUTTON': ('#FFFFFF', '#517239'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBlue1': {'BACKGROUND': '#A5CADD', 'TEXT': '#6E266E', 'INPUT': '#E0F5FF', 'TEXT_INPUT': '#000000', 'SCROLL': '#E0F5FF',
-                   'BUTTON': ('#FFFFFF', '#303952'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightPurple': {'BACKGROUND': '#B0AAC2', 'TEXT': '#000000', 'INPUT': '#F2EFE8', 'SCROLL': '#F2EFE8', 'TEXT_INPUT': '#000000',
-                    'BUTTON': ('#000000', '#C2D4D8'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBlue2': {'BACKGROUND': '#AAB6D3', 'TEXT': '#000000', 'INPUT': '#F1F4FC', 'SCROLL': '#F1F4FC', 'TEXT_INPUT': '#000000',
-                   'BUTTON': ('#FFFFFF', '#7186C7'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightGreen3': {'BACKGROUND': '#A8C1B4', 'TEXT': '#000000', 'INPUT': '#DDE0DE', 'SCROLL': '#E3E3E3', 'TEXT_INPUT': '#000000',
-                    'BUTTON': ('#FFFFFF', '#6D9F85'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBlue3': {'BACKGROUND': '#64778d', 'TEXT': '#FFFFFF', 'INPUT': '#f0f3f7', 'SCROLL': '#A6B2BE', 'TEXT_INPUT': '#000000',
-                  'BUTTON': ('#FFFFFF', '#283b5b'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightGreen4': {'BACKGROUND': '#b4ffb4', 'TEXT': '#000000', 'INPUT': '#ffff64', 'SCROLL': '#ffb482', 'TEXT_INPUT': '#000000',
-                    'BUTTON': ('#000000', '#ffa0dc'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightGreen5': {'BACKGROUND': '#92aa9d', 'TEXT': '#000000', 'INPUT': '#fcfff6', 'SCROLL': '#fcfff6', 'TEXT_INPUT': '#000000',
-                    'BUTTON': ('#000000', '#d0dbbd'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBrown2': {'BACKGROUND': '#a7ad7f', 'TEXT': '#000000', 'INPUT': '#e6d3a8', 'SCROLL': '#e6d3a8', 'TEXT_INPUT': '#000000',
-                    'BUTTON': ('#FFFFFF', '#5d907d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBrown3': {'BACKGROUND': '#efeccb', 'TEXT': '#012f2f', 'INPUT': '#e6d3a8', 'SCROLL': '#e6d3a8', 'TEXT_INPUT': '#012f2f',
-                    'BUTTON': ('#FFFFFF', '#046380'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBlue3': {'BACKGROUND': '#a8cfdd', 'TEXT': '#000000', 'INPUT': '#dfedf2', 'SCROLL': '#dfedf2', 'TEXT_INPUT': '#000000',
-                   'BUTTON': ('#FFFFFF', '#183440'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'LightBrown4': {'BACKGROUND': '#d7c79e', 'TEXT': '#a35638', 'INPUT': '#9dab86', 'TEXT_INPUT': '#000000', 'SCROLL': '#a35638',
-                    'BUTTON': ('#FFFFFF', '#a35638'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#a35638', '#9dab86', '#e08f62', '#d7c79e'], },
-    'DarkTeal': {'BACKGROUND': '#003f5c', 'TEXT': '#fb5b5a', 'INPUT': '#bc4873', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#bc4873', 'BUTTON': ('#FFFFFF', '#fb5b5a'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                 'COLOR_LIST': ['#003f5c', '#472b62', '#bc4873', '#fb5b5a'], },
-    'DarkPurple': {'BACKGROUND': '#472b62', 'TEXT': '#fb5b5a', 'INPUT': '#bc4873', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#bc4873',
-                   'BUTTON': ('#FFFFFF', '#472b62'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#003f5c', '#472b62', '#bc4873', '#fb5b5a'], },
-    'LightGreen6': {'BACKGROUND': '#eafbea', 'TEXT': '#1f6650', 'INPUT': '#6f9a8d', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#1f6650',
-                    'BUTTON': ('#FFFFFF', '#1f6650'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#1f6650', '#6f9a8d', '#ea5e5e', '#eafbea'], },
-    'DarkGrey2': {'BACKGROUND': '#2b2b28', 'TEXT': '#f8f8f8', 'INPUT': '#f1d6ab', 'TEXT_INPUT': '#000000', 'SCROLL': '#f1d6ab',
-                  'BUTTON': ('#2b2b28', '#e3b04b'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#2b2b28', '#e3b04b', '#f1d6ab', '#f8f8f8'], },
-    'LightBrown6': {'BACKGROUND': '#f9b282', 'TEXT': '#8f4426', 'INPUT': '#de6b35', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#8f4426',
-                    'BUTTON': ('#FFFFFF', '#8f4426'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#8f4426', '#de6b35', '#64ccda', '#f9b282'], },
-    'DarkTeal1': {'BACKGROUND': '#396362', 'TEXT': '#ffe7d1', 'INPUT': '#f6c89f', 'TEXT_INPUT': '#000000', 'SCROLL': '#f6c89f',
-                  'BUTTON': ('#ffe7d1', '#4b8e8d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#396362', '#4b8e8d', '#f6c89f', '#ffe7d1'], },
-    'LightBrown7': {'BACKGROUND': '#f6c89f', 'TEXT': '#396362', 'INPUT': '#4b8e8d', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#396362',
-                    'BUTTON': ('#FFFFFF', '#396362'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#396362', '#4b8e8d', '#f6c89f', '#ffe7d1'], },
-    'DarkPurple1': {'BACKGROUND': '#0c093c', 'TEXT': '#fad6d6', 'INPUT': '#eea5f6', 'TEXT_INPUT': '#000000', 'SCROLL': '#eea5f6',
-                    'BUTTON': ('#FFFFFF', '#df42d1'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#0c093c', '#df42d1', '#eea5f6', '#fad6d6'], },
-    'DarkGrey3': {'BACKGROUND': '#211717', 'TEXT': '#dfddc7', 'INPUT': '#f58b54', 'TEXT_INPUT': '#000000', 'SCROLL': '#f58b54',
-                  'BUTTON': ('#dfddc7', '#a34a28'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#211717', '#a34a28', '#f58b54', '#dfddc7'], },
-    'LightBrown8': {'BACKGROUND': '#dfddc7', 'TEXT': '#211717', 'INPUT': '#a34a28', 'TEXT_INPUT': '#dfddc7', 'SCROLL': '#211717',
-                    'BUTTON': ('#dfddc7', '#a34a28'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#211717', '#a34a28', '#f58b54', '#dfddc7'], },
-    'DarkBlue4': {'BACKGROUND': '#494ca2', 'TEXT': '#e3e7f1', 'INPUT': '#c6cbef', 'TEXT_INPUT': '#000000', 'SCROLL': '#c6cbef',
-                  'BUTTON': ('#FFFFFF', '#8186d5'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#494ca2', '#8186d5', '#c6cbef', '#e3e7f1'], },
-    'LightBlue4': {'BACKGROUND': '#5c94bd', 'TEXT': '#470938', 'INPUT': '#1a3e59', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#470938',
-                   'BUTTON': ('#FFFFFF', '#470938'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#470938', '#1a3e59', '#5c94bd', '#f2d6eb'], },
-    'DarkTeal2': {'BACKGROUND': '#394a6d', 'TEXT': '#c0ffb3', 'INPUT': '#52de97', 'TEXT_INPUT': '#000000', 'SCROLL': '#52de97',
-                  'BUTTON': ('#c0ffb3', '#394a6d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#394a6d', '#3c9d9b', '#52de97', '#c0ffb3'], },
-    'DarkTeal3': {'BACKGROUND': '#3c9d9b', 'TEXT': '#c0ffb3', 'INPUT': '#52de97', 'TEXT_INPUT': '#000000', 'SCROLL': '#52de97',
-                  'BUTTON': ('#c0ffb3', '#394a6d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#394a6d', '#3c9d9b', '#52de97', '#c0ffb3'], },
-    'DarkPurple5': {'BACKGROUND': '#730068', 'TEXT': '#f6f078', 'INPUT': '#01d28e', 'TEXT_INPUT': '#000000', 'SCROLL': '#01d28e',
-                    'BUTTON': ('#f6f078', '#730068'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#730068', '#434982', '#01d28e', '#f6f078'], },
-    'DarkPurple2': {'BACKGROUND': '#202060', 'TEXT': '#b030b0', 'INPUT': '#602080', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#602080',
-                    'BUTTON': ('#FFFFFF', '#202040'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#202040', '#202060', '#602080', '#b030b0'], },
-    'DarkBlue5': {'BACKGROUND': '#000272', 'TEXT': '#ff6363', 'INPUT': '#a32f80', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#a32f80',
-                  'BUTTON': ('#FFFFFF', '#341677'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#000272', '#341677', '#a32f80', '#ff6363'], },
-    'LightGrey2': {'BACKGROUND': '#f6f6f6', 'TEXT': '#420000', 'INPUT': '#d4d7dd', 'TEXT_INPUT': '#420000', 'SCROLL': '#420000',
-                   'BUTTON': ('#420000', '#d4d7dd'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#420000', '#d4d7dd', '#eae9e9', '#f6f6f6'], },
-    'LightGrey3': {'BACKGROUND': '#eae9e9', 'TEXT': '#420000', 'INPUT': '#d4d7dd', 'TEXT_INPUT': '#420000', 'SCROLL': '#420000',
-                   'BUTTON': ('#420000', '#d4d7dd'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#420000', '#d4d7dd', '#eae9e9', '#f6f6f6'], },
-    'DarkBlue6': {'BACKGROUND': '#01024e', 'TEXT': '#ff6464', 'INPUT': '#8b4367', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#8b4367',
-                  'BUTTON': ('#FFFFFF', '#543864'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#01024e', '#543864', '#8b4367', '#ff6464'], },
-    'DarkBlue7': {'BACKGROUND': '#241663', 'TEXT': '#eae7af', 'INPUT': '#a72693', 'TEXT_INPUT': '#eae7af', 'SCROLL': '#a72693',
-                  'BUTTON': ('#eae7af', '#160f30'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#160f30', '#241663', '#a72693', '#eae7af'], },
-    'LightBrown9': {'BACKGROUND': '#f6d365', 'TEXT': '#3a1f5d', 'INPUT': '#c83660', 'TEXT_INPUT': '#f6d365', 'SCROLL': '#3a1f5d',
-                    'BUTTON': ('#f6d365', '#c83660'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#3a1f5d', '#c83660', '#e15249', '#f6d365'], },
-    'DarkPurple3': {'BACKGROUND': '#6e2142', 'TEXT': '#ffd692', 'INPUT': '#e16363', 'TEXT_INPUT': '#ffd692', 'SCROLL': '#e16363',
-                    'BUTTON': ('#ffd692', '#943855'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#6e2142', '#943855', '#e16363', '#ffd692'], },
-    'LightBrown10': {'BACKGROUND': '#ffd692', 'TEXT': '#6e2142', 'INPUT': '#943855', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#6e2142',
-                     'BUTTON': ('#FFFFFF', '#6e2142'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                     'COLOR_LIST': ['#6e2142', '#943855', '#e16363', '#ffd692'], },
-    'DarkPurple4': {'BACKGROUND': '#200f21', 'TEXT': '#f638dc', 'INPUT': '#5a3d5c', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#5a3d5c',
-                    'BUTTON': ('#FFFFFF', '#382039'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#200f21', '#382039', '#5a3d5c', '#f638dc'], },
-    'LightBlue5': {'BACKGROUND': '#b2fcff', 'TEXT': '#3e64ff', 'INPUT': '#5edfff', 'TEXT_INPUT': '#000000', 'SCROLL': '#3e64ff',
-                   'BUTTON': ('#FFFFFF', '#3e64ff'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#3e64ff', '#5edfff', '#b2fcff', '#ecfcff'], },
-    'DarkTeal4': {'BACKGROUND': '#464159', 'TEXT': '#c7f0db', 'INPUT': '#8bbabb', 'TEXT_INPUT': '#000000', 'SCROLL': '#8bbabb',
-                  'BUTTON': ('#FFFFFF', '#6c7b95'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#464159', '#6c7b95', '#8bbabb', '#c7f0db'], },
-    'LightTeal': {'BACKGROUND': '#c7f0db', 'TEXT': '#464159', 'INPUT': '#6c7b95', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#464159',
-                  'BUTTON': ('#FFFFFF', '#464159'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#464159', '#6c7b95', '#8bbabb', '#c7f0db'], },
-    'DarkTeal5': {'BACKGROUND': '#8bbabb', 'TEXT': '#464159', 'INPUT': '#6c7b95', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#464159',
-                  'BUTTON': ('#c7f0db', '#6c7b95'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#464159', '#6c7b95', '#8bbabb', '#c7f0db'], },
-    'LightGrey4': {'BACKGROUND': '#faf5ef', 'TEXT': '#672f2f', 'INPUT': '#99b19c', 'TEXT_INPUT': '#672f2f', 'SCROLL': '#672f2f',
-                   'BUTTON': ('#672f2f', '#99b19c'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#672f2f', '#99b19c', '#d7d1c9', '#faf5ef'], },
-    'LightGreen7': {'BACKGROUND': '#99b19c', 'TEXT': '#faf5ef', 'INPUT': '#d7d1c9', 'TEXT_INPUT': '#000000', 'SCROLL': '#d7d1c9',
-                    'BUTTON': ('#FFFFFF', '#99b19c'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#672f2f', '#99b19c', '#d7d1c9', '#faf5ef'], },
-    'LightGrey5': {'BACKGROUND': '#d7d1c9', 'TEXT': '#672f2f', 'INPUT': '#99b19c', 'TEXT_INPUT': '#672f2f', 'SCROLL': '#672f2f',
-                   'BUTTON': ('#FFFFFF', '#672f2f'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#672f2f', '#99b19c', '#d7d1c9', '#faf5ef'], },
-    'DarkBrown3': {'BACKGROUND': '#a0855b', 'TEXT': '#f9f6f2', 'INPUT': '#f1d6ab', 'TEXT_INPUT': '#000000', 'SCROLL': '#f1d6ab',
-                   'BUTTON': ('#FFFFFF', '#38470b'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#38470b', '#a0855b', '#f1d6ab', '#f9f6f2'], },
-    'LightBrown11': {'BACKGROUND': '#f1d6ab', 'TEXT': '#38470b', 'INPUT': '#a0855b', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#38470b',
-                     'BUTTON': ('#f9f6f2', '#a0855b'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                     'COLOR_LIST': ['#38470b', '#a0855b', '#f1d6ab', '#f9f6f2'], },
-    'DarkRed': {'BACKGROUND': '#83142c', 'TEXT': '#f9d276', 'INPUT': '#ad1d45', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#ad1d45', 'BUTTON': ('#f9d276', '#ad1d45'),
-                'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                'COLOR_LIST': ['#44000d', '#83142c', '#ad1d45', '#f9d276'], },
-    'DarkTeal6': {'BACKGROUND': '#204969', 'TEXT': '#fff7f7', 'INPUT': '#dadada', 'TEXT_INPUT': '#000000', 'SCROLL': '#dadada',
-                  'BUTTON': ('#000000', '#fff7f7'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#204969', '#08ffc8', '#dadada', '#fff7f7'], },
-    'DarkBrown4': {'BACKGROUND': '#252525', 'TEXT': '#ff0000', 'INPUT': '#af0404', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#af0404',
-                   'BUTTON': ('#FFFFFF', '#252525'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#252525', '#414141', '#af0404', '#ff0000'], },
-    'LightYellow': {'BACKGROUND': '#f4ff61', 'TEXT': '#27aa80', 'INPUT': '#32ff6a', 'TEXT_INPUT': '#000000', 'SCROLL': '#27aa80',
-                    'BUTTON': ('#f4ff61', '#27aa80'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#27aa80', '#32ff6a', '#a8ff3e', '#f4ff61'], },
-    'DarkGreen1': {'BACKGROUND': '#2b580c', 'TEXT': '#fdef96', 'INPUT': '#f7b71d', 'TEXT_INPUT': '#000000', 'SCROLL': '#f7b71d',
-                   'BUTTON': ('#fdef96', '#2b580c'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#2b580c', '#afa939', '#f7b71d', '#fdef96'], },
-    'LightGreen8': {'BACKGROUND': '#c8dad3', 'TEXT': '#63707e', 'INPUT': '#93b5b3', 'TEXT_INPUT': '#000000', 'SCROLL': '#63707e',
-                    'BUTTON': ('#FFFFFF', '#63707e'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#63707e', '#93b5b3', '#c8dad3', '#f2f6f5'], },
-    'DarkTeal7': {'BACKGROUND': '#248ea9', 'TEXT': '#fafdcb', 'INPUT': '#aee7e8', 'TEXT_INPUT': '#000000', 'SCROLL': '#aee7e8',
-                  'BUTTON': ('#000000', '#fafdcb'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#248ea9', '#28c3d4', '#aee7e8', '#fafdcb'], },
-    'DarkBlue8': {'BACKGROUND': '#454d66', 'TEXT': '#d9d872', 'INPUT': '#58b368', 'TEXT_INPUT': '#000000', 'SCROLL': '#58b368',
-                  'BUTTON': ('#000000', '#009975'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#009975', '#454d66', '#58b368', '#d9d872'], },
-    'DarkBlue9': {'BACKGROUND': '#263859', 'TEXT': '#ff6768', 'INPUT': '#6b778d', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#6b778d',
-                  'BUTTON': ('#ff6768', '#263859'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#17223b', '#263859', '#6b778d', '#ff6768'], },
-    'DarkBlue10': {'BACKGROUND': '#0028ff', 'TEXT': '#f1f4df', 'INPUT': '#10eaf0', 'TEXT_INPUT': '#000000', 'SCROLL': '#10eaf0',
-                   'BUTTON': ('#f1f4df', '#24009c'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#24009c', '#0028ff', '#10eaf0', '#f1f4df'], },
-    'DarkBlue11': {'BACKGROUND': '#6384b3', 'TEXT': '#e6f0b6', 'INPUT': '#b8e9c0', 'TEXT_INPUT': '#000000', 'SCROLL': '#b8e9c0',
-                   'BUTTON': ('#e6f0b6', '#684949'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#684949', '#6384b3', '#b8e9c0', '#e6f0b6'], },
-    'DarkTeal8': {'BACKGROUND': '#71a0a5', 'TEXT': '#212121', 'INPUT': '#665c84', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#212121',
-                  'BUTTON': ('#fab95b', '#665c84'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#212121', '#665c84', '#71a0a5', '#fab95b'], },
-    'DarkRed1': {'BACKGROUND': '#c10000', 'TEXT': '#eeeeee', 'INPUT': '#dedede', 'TEXT_INPUT': '#000000', 'SCROLL': '#dedede', 'BUTTON': ('#c10000', '#eeeeee'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                 'COLOR_LIST': ['#c10000', '#ff4949', '#dedede', '#eeeeee'], },
-    'LightBrown5': {'BACKGROUND': '#fff591', 'TEXT': '#e41749', 'INPUT': '#f5587b', 'TEXT_INPUT': '#000000', 'SCROLL': '#e41749',
-                    'BUTTON': ('#fff591', '#e41749'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#e41749', '#f5587b', '#ff8a5c', '#fff591'], },
-    'LightGreen9': {'BACKGROUND': '#f1edb3', 'TEXT': '#3b503d', 'INPUT': '#4a746e', 'TEXT_INPUT': '#f1edb3', 'SCROLL': '#3b503d',
-                    'BUTTON': ('#f1edb3', '#3b503d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#3b503d', '#4a746e', '#c8cf94', '#f1edb3'], 'DESCRIPTION': ['Green', 'Turquoise', 'Yellow'], },
-    'DarkGreen2': {'BACKGROUND': '#3b503d', 'TEXT': '#f1edb3', 'INPUT': '#c8cf94', 'TEXT_INPUT': '#000000', 'SCROLL': '#c8cf94',
-                   'BUTTON': ('#f1edb3', '#3b503d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#3b503d', '#4a746e', '#c8cf94', '#f1edb3'], 'DESCRIPTION': ['Green', 'Turquoise', 'Yellow'], },
-    'LightGray1': {'BACKGROUND': '#f2f2f2', 'TEXT': '#222831', 'INPUT': '#393e46', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#222831',
-                   'BUTTON': ('#f2f2f2', '#222831'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#222831', '#393e46', '#f96d00', '#f2f2f2'], 'DESCRIPTION': ['#000000', 'Grey', 'Orange', 'Grey', 'Autumn'], },
-    'DarkGrey4': {'BACKGROUND': '#52524e', 'TEXT': '#e9e9e5', 'INPUT': '#d4d6c8', 'TEXT_INPUT': '#000000', 'SCROLL': '#d4d6c8',
-                  'BUTTON': ('#FFFFFF', '#9a9b94'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#52524e', '#9a9b94', '#d4d6c8', '#e9e9e5'], 'DESCRIPTION': ['Grey', 'Pastel', 'Winter'], },
-    'DarkBlue12': {'BACKGROUND': '#324e7b', 'TEXT': '#f8f8f8', 'INPUT': '#86a6df', 'TEXT_INPUT': '#000000', 'SCROLL': '#86a6df',
-                   'BUTTON': ('#FFFFFF', '#5068a9'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#324e7b', '#5068a9', '#86a6df', '#f8f8f8'], 'DESCRIPTION': ['Blue', 'Grey', 'Cold', 'Winter'], },
-    'DarkPurple6': {'BACKGROUND': '#070739', 'TEXT': '#e1e099', 'INPUT': '#c327ab', 'TEXT_INPUT': '#e1e099', 'SCROLL': '#c327ab',
-                    'BUTTON': ('#e1e099', '#521477'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                    'COLOR_LIST': ['#070739', '#521477', '#c327ab', '#e1e099'], 'DESCRIPTION': ['#000000', 'Purple', 'Yellow', 'Dark'], },
-    'DarkPurple7': {'BACKGROUND': '#191930', 'TEXT': '#B1B7C5', 'INPUT': '#232B5C', 'TEXT_INPUT': '#D0E3E7', 'SCROLL': '#B1B7C5',
-                    'BUTTON': ('#272D38', '#B1B7C5'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkBlue13': {'BACKGROUND': '#203562', 'TEXT': '#e3e8f8', 'INPUT': '#c0c5cd', 'TEXT_INPUT': '#000000', 'SCROLL': '#c0c5cd',
-                   'BUTTON': ('#FFFFFF', '#3e588f'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#203562', '#3e588f', '#c0c5cd', '#e3e8f8'], 'DESCRIPTION': ['Blue', 'Grey', 'Wedding', 'Cold'], },
-    'DarkBrown5': {'BACKGROUND': '#3c1b1f', 'TEXT': '#f6e1b5', 'INPUT': '#e2bf81', 'TEXT_INPUT': '#000000', 'SCROLL': '#e2bf81',
-                   'BUTTON': ('#3c1b1f', '#f6e1b5'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#3c1b1f', '#b21e4b', '#e2bf81', '#f6e1b5'], 'DESCRIPTION': ['Brown', 'Red', 'Yellow', 'Warm'], },
-    'DarkGreen3': {'BACKGROUND': '#062121', 'TEXT': '#eeeeee', 'INPUT': '#e4dcad', 'TEXT_INPUT': '#000000', 'SCROLL': '#e4dcad',
-                   'BUTTON': ('#eeeeee', '#181810'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#062121', '#181810', '#e4dcad', '#eeeeee'], 'DESCRIPTION': ['#000000', '#000000', 'Brown', 'Grey'], },
-    'DarkBlack1': {'BACKGROUND': '#181810', 'TEXT': '#eeeeee', 'INPUT': '#e4dcad', 'TEXT_INPUT': '#000000', 'SCROLL': '#e4dcad',
-                   'BUTTON': ('#FFFFFF', '#062121'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#062121', '#181810', '#e4dcad', '#eeeeee'], 'DESCRIPTION': ['#000000', '#000000', 'Brown', 'Grey'], },
-    'DarkGrey5': {'BACKGROUND': '#343434', 'TEXT': '#f3f3f3', 'INPUT': '#e9dcbe', 'TEXT_INPUT': '#000000', 'SCROLL': '#e9dcbe',
-                  'BUTTON': ('#FFFFFF', '#8e8b82'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#343434', '#8e8b82', '#e9dcbe', '#f3f3f3'], 'DESCRIPTION': ['Grey', 'Brown'], },
-    'LightBrown12': {'BACKGROUND': '#8e8b82', 'TEXT': '#f3f3f3', 'INPUT': '#e9dcbe', 'TEXT_INPUT': '#000000', 'SCROLL': '#e9dcbe',
-                     'BUTTON': ('#f3f3f3', '#8e8b82'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                     'COLOR_LIST': ['#343434', '#8e8b82', '#e9dcbe', '#f3f3f3'], 'DESCRIPTION': ['Grey', 'Brown'], },
-    'DarkTeal9': {'BACKGROUND': '#13445a', 'TEXT': '#fef4e8', 'INPUT': '#446878', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#446878',
-                  'BUTTON': ('#fef4e8', '#446878'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#13445a', '#970747', '#446878', '#fef4e8'], 'DESCRIPTION': ['Red', 'Grey', 'Blue', 'Wedding', 'Retro'], },
-    'DarkBlue14': {'BACKGROUND': '#21273d', 'TEXT': '#f1f6f8', 'INPUT': '#b9d4f1', 'TEXT_INPUT': '#000000', 'SCROLL': '#b9d4f1',
-                   'BUTTON': ('#FFFFFF', '#6a759b'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#21273d', '#6a759b', '#b9d4f1', '#f1f6f8'], 'DESCRIPTION': ['Blue', '#000000', 'Grey', 'Cold', 'Winter'], },
-    'LightBlue6': {'BACKGROUND': '#f1f6f8', 'TEXT': '#21273d', 'INPUT': '#6a759b', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#21273d',
-                   'BUTTON': ('#f1f6f8', '#6a759b'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#21273d', '#6a759b', '#b9d4f1', '#f1f6f8'], 'DESCRIPTION': ['Blue', '#000000', 'Grey', 'Cold', 'Winter'], },
-    'DarkGreen4': {'BACKGROUND': '#044343', 'TEXT': '#e4e4e4', 'INPUT': '#045757', 'TEXT_INPUT': '#e4e4e4', 'SCROLL': '#045757',
-                   'BUTTON': ('#e4e4e4', '#045757'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#222222', '#044343', '#045757', '#e4e4e4'], 'DESCRIPTION': ['#000000', 'Turquoise', 'Grey', 'Dark'], },
-    'DarkGreen5': {'BACKGROUND': '#1b4b36', 'TEXT': '#e0e7f1', 'INPUT': '#aebd77', 'TEXT_INPUT': '#000000', 'SCROLL': '#aebd77',
-                   'BUTTON': ('#FFFFFF', '#538f6a'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#1b4b36', '#538f6a', '#aebd77', '#e0e7f1'], 'DESCRIPTION': ['Green', 'Grey'], },
-    'DarkTeal10': {'BACKGROUND': '#0d3446', 'TEXT': '#d8dfe2', 'INPUT': '#71adb5', 'TEXT_INPUT': '#000000', 'SCROLL': '#71adb5',
-                   'BUTTON': ('#FFFFFF', '#176d81'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#0d3446', '#176d81', '#71adb5', '#d8dfe2'], 'DESCRIPTION': ['Grey', 'Turquoise', 'Winter', 'Cold'], },
-    'DarkGrey6': {'BACKGROUND': '#3e3e3e', 'TEXT': '#ededed', 'INPUT': '#68868c', 'TEXT_INPUT': '#ededed', 'SCROLL': '#68868c',
-                  'BUTTON': ('#FFFFFF', '#405559'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#3e3e3e', '#405559', '#68868c', '#ededed'], 'DESCRIPTION': ['Grey', 'Turquoise', 'Winter'], },
-    'DarkTeal11': {'BACKGROUND': '#405559', 'TEXT': '#ededed', 'INPUT': '#68868c', 'TEXT_INPUT': '#ededed', 'SCROLL': '#68868c',
-                   'BUTTON': ('#ededed', '#68868c'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#3e3e3e', '#405559', '#68868c', '#ededed'], 'DESCRIPTION': ['Grey', 'Turquoise', 'Winter'], },
-    'LightBlue7': {'BACKGROUND': '#9ed0e0', 'TEXT': '#19483f', 'INPUT': '#5c868e', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#19483f',
-                   'BUTTON': ('#FFFFFF', '#19483f'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#19483f', '#5c868e', '#ff6a38', '#9ed0e0'], 'DESCRIPTION': ['Orange', 'Blue', 'Turquoise'], },
-    'LightGreen10': {'BACKGROUND': '#d8ebb5', 'TEXT': '#205d67', 'INPUT': '#639a67', 'TEXT_INPUT': '#FFFFFF', 'SCROLL': '#205d67',
-                     'BUTTON': ('#d8ebb5', '#205d67'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                     'COLOR_LIST': ['#205d67', '#639a67', '#d9bf77', '#d8ebb5'], 'DESCRIPTION': ['Blue', 'Green', 'Brown', 'Vintage'], },
-    'DarkBlue15': {'BACKGROUND': '#151680', 'TEXT': '#f1fea4', 'INPUT': '#375fc0', 'TEXT_INPUT': '#f1fea4', 'SCROLL': '#375fc0',
-                   'BUTTON': ('#f1fea4', '#1c44ac'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#151680', '#1c44ac', '#375fc0', '#f1fea4'], 'DESCRIPTION': ['Blue', 'Yellow', 'Cold'], },
-    'DarkBlue16': {'BACKGROUND': '#1c44ac', 'TEXT': '#f1fea4', 'INPUT': '#375fc0', 'TEXT_INPUT': '#f1fea4', 'SCROLL': '#375fc0',
-                   'BUTTON': ('#f1fea4', '#151680'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#151680', '#1c44ac', '#375fc0', '#f1fea4'], 'DESCRIPTION': ['Blue', 'Yellow', 'Cold'], },
-    'DarkTeal12': {'BACKGROUND': '#004a7c', 'TEXT': '#fafafa', 'INPUT': '#e8f1f5', 'TEXT_INPUT': '#000000', 'SCROLL': '#e8f1f5',
-                   'BUTTON': ('#fafafa', '#005691'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#004a7c', '#005691', '#e8f1f5', '#fafafa'], 'DESCRIPTION': ['Grey', 'Blue', 'Cold', 'Winter'], },
-    'LightBrown13': {'BACKGROUND': '#ebf5ee', 'TEXT': '#921224', 'INPUT': '#bdc6b8', 'TEXT_INPUT': '#921224', 'SCROLL': '#921224',
-                     'BUTTON': ('#FFFFFF', '#921224'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                     'COLOR_LIST': ['#921224', '#bdc6b8', '#bce0da', '#ebf5ee'], 'DESCRIPTION': ['Red', 'Blue', 'Grey', 'Vintage', 'Wedding'], },
-    'DarkBlue17': {'BACKGROUND': '#21294c', 'TEXT': '#f9f2d7', 'INPUT': '#f2dea8', 'TEXT_INPUT': '#000000', 'SCROLL': '#f2dea8',
-                   'BUTTON': ('#f9f2d7', '#141829'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#141829', '#21294c', '#f2dea8', '#f9f2d7'], 'DESCRIPTION': ['#000000', 'Blue', 'Yellow'], },
-    'DarkBlue18': {'BACKGROUND': '#0c1825', 'TEXT': '#d1d7dd', 'INPUT': '#001c35', 'TEXT_INPUT': '#d1d7dd', 'SCROLL': '#00438e',
-                   'BUTTON': ('#75b7ff', '#001c35'), 'PROGRESS': ('#0074ff', '#75b7ff'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#141829', '#21294c', '#f2dea8', '#f9f2d7'], 'DESCRIPTION': ['#000000', 'Blue', 'Yellow'], },
-    'DarkBrown6': {'BACKGROUND': '#785e4d', 'TEXT': '#f2eee3', 'INPUT': '#baaf92', 'TEXT_INPUT': '#000000', 'SCROLL': '#baaf92',
-                   'BUTTON': ('#FFFFFF', '#785e4d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#785e4d', '#ff8426', '#baaf92', '#f2eee3'], 'DESCRIPTION': ['Grey', 'Brown', 'Orange', 'Autumn'], },
-    'DarkGreen6': {'BACKGROUND': '#5c715e', 'TEXT': '#f2f9f1', 'INPUT': '#ddeedf', 'TEXT_INPUT': '#000000', 'SCROLL': '#ddeedf',
-                   'BUTTON': ('#f2f9f1', '#5c715e'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#5c715e', '#b6cdbd', '#ddeedf', '#f2f9f1'], 'DESCRIPTION': ['Grey', 'Green', 'Vintage'], },
-    'DarkGreen7': {'BACKGROUND': '#0C231E', 'TEXT': '#efbe1c', 'INPUT': '#153C33', 'TEXT_INPUT': '#efbe1c', 'SCROLL': '#153C33',
-                   'BUTTON': ('#efbe1c', '#153C33'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey7': {'BACKGROUND': '#4b586e', 'TEXT': '#dddddd', 'INPUT': '#574e6d', 'TEXT_INPUT': '#dddddd', 'SCROLL': '#574e6d',
-                  'BUTTON': ('#dddddd', '#43405d'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                  'COLOR_LIST': ['#43405d', '#4b586e', '#574e6d', '#dddddd'], 'DESCRIPTION': ['Grey', 'Winter', 'Cold'], },
-    'DarkRed2': {'BACKGROUND': '#ab1212', 'TEXT': '#f6e4b5', 'INPUT': '#cd3131', 'TEXT_INPUT': '#f6e4b5', 'SCROLL': '#cd3131', 'BUTTON': ('#f6e4b5', '#ab1212'),
-                 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                 'COLOR_LIST': ['#ab1212', '#1fad9f', '#cd3131', '#f6e4b5'], 'DESCRIPTION': ['Turquoise', 'Red', 'Yellow'], },
-    'LightGrey6': {'BACKGROUND': '#e3e3e3', 'TEXT': '#233142', 'INPUT': '#455d7a', 'TEXT_INPUT': '#e3e3e3', 'SCROLL': '#233142',
-                   'BUTTON': ('#e3e3e3', '#455d7a'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,
-                   'COLOR_LIST': ['#233142', '#455d7a', '#f95959', '#e3e3e3'], 'DESCRIPTION': ['#000000', 'Blue', 'Red', 'Grey'], },
-    'HotDogStand': {'BACKGROUND': 'red', 'TEXT': 'yellow', 'INPUT': 'yellow', 'TEXT_INPUT': '#000000', 'SCROLL': 'yellow', 'BUTTON': ('red', 'yellow'),
-                    'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey8': {'BACKGROUND': '#19232D', 'TEXT': '#ffffff', 'INPUT': '#32414B', 'TEXT_INPUT': '#ffffff', 'SCROLL': '#505F69',
-                  'BUTTON': ('#ffffff', '#32414B'), 'PROGRESS': ('#505F69', '#32414B'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey9': {'BACKGROUND': '#36393F', 'TEXT': '#DCDDDE', 'INPUT': '#40444B', 'TEXT_INPUT': '#ffffff', 'SCROLL': '#202225',
-                  'BUTTON': ('#202225', '#B9BBBE'), 'PROGRESS': ('#202225', '#40444B'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey10': {'BACKGROUND': '#1c1e23', 'TEXT': '#cccdcf', 'INPUT': '#272a31', 'TEXT_INPUT': '#8b9fde', 'SCROLL': '#313641',
-                   'BUTTON': ('#f5f5f6', '#2e3d5a'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey11': {'BACKGROUND': '#1c1e23', 'TEXT': '#cccdcf', 'INPUT': '#313641', 'TEXT_INPUT': '#cccdcf', 'SCROLL': '#313641',
-                   'BUTTON': ('#f5f5f6', '#313641'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey12': {'BACKGROUND': '#1c1e23', 'TEXT': '#8b9fde', 'INPUT': '#313641', 'TEXT_INPUT': '#8b9fde', 'SCROLL': '#313641',
-                   'BUTTON': ('#cccdcf', '#2e3d5a'), 'PROGRESS': DEFAULT_PROGRESS_BAR_COMPUTE, 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey13': {'BACKGROUND': '#1c1e23', 'TEXT': '#cccdcf', 'INPUT': '#272a31', 'TEXT_INPUT': '#cccdcf', 'SCROLL': '#313641',
-                   'BUTTON': ('#8b9fde', '#313641'), 'PROGRESS': ('#cccdcf', '#272a31'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey14': {'BACKGROUND': '#24292e', 'TEXT': '#fafbfc', 'INPUT': '#1d2125', 'TEXT_INPUT': '#fafbfc', 'SCROLL': '#1d2125',
-                   'BUTTON': ('#fafbfc', '#155398'), 'PROGRESS': ('#155398', '#1d2125'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'DarkGrey15': {'BACKGROUND': '#121212', 'TEXT': '#dddddd', 'INPUT': '#1e1e1e', 'TEXT_INPUT': '#69b1ef', 'SCROLL': '#272727',
+    "SystemDefault": {"BACKGROUND": COLOR_SYSTEM_DEFAULT, "TEXT": COLOR_SYSTEM_DEFAULT, "INPUT": COLOR_SYSTEM_DEFAULT, "TEXT_INPUT": COLOR_SYSTEM_DEFAULT,
+                      "SCROLL": COLOR_SYSTEM_DEFAULT, "BUTTON": OFFICIAL_PYSIMPLEGUI_BUTTON_COLOR, "PROGRESS": COLOR_SYSTEM_DEFAULT, "BORDER": 1,
+                      "SLIDER_DEPTH": 1, "PROGRESS_DEPTH": 0, },
+    "SystemDefaultForReal": {"BACKGROUND": COLOR_SYSTEM_DEFAULT, "TEXT": COLOR_SYSTEM_DEFAULT, "INPUT": COLOR_SYSTEM_DEFAULT,
+                             "TEXT_INPUT": COLOR_SYSTEM_DEFAULT, "SCROLL": COLOR_SYSTEM_DEFAULT, "BUTTON": COLOR_SYSTEM_DEFAULT,
+                             "PROGRESS": COLOR_SYSTEM_DEFAULT, "BORDER": 1, "SLIDER_DEPTH": 1, "PROGRESS_DEPTH": 0, },
+    "SystemDefault1": {"BACKGROUND": COLOR_SYSTEM_DEFAULT, "TEXT": COLOR_SYSTEM_DEFAULT, "INPUT": COLOR_SYSTEM_DEFAULT, "TEXT_INPUT": COLOR_SYSTEM_DEFAULT,
+                       "SCROLL": COLOR_SYSTEM_DEFAULT, "BUTTON": COLOR_SYSTEM_DEFAULT, "PROGRESS": COLOR_SYSTEM_DEFAULT, "BORDER": 1, "SLIDER_DEPTH": 1,
+                       "PROGRESS_DEPTH": 0, },
+    "Material1": {"BACKGROUND": "#E3F2FD", "TEXT": "#000000", "INPUT": "#86A8FF", "TEXT_INPUT": "#000000", "SCROLL": "#86A8FF",
+                  "BUTTON": ("#FFFFFF", "#5079D3"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 0, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "ACCENT1": "#FF0266", "ACCENT2": "#FF5C93", "ACCENT3": "#C5003C", },
+    "Material2": {"BACKGROUND": "#FAFAFA", "TEXT": "#000000", "INPUT": "#004EA1", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#5EA7FF",
+                  "BUTTON": ("#FFFFFF", "#0079D3"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 0, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "ACCENT1": "#FF0266", "ACCENT2": "#FF5C93", "ACCENT3": "#C5003C", },
+    "Reddit": {"BACKGROUND": "#ffffff", "TEXT": "#1a1a1b", "INPUT": "#dae0e6", "TEXT_INPUT": "#222222", "SCROLL": "#a5a4a4", "BUTTON": ("#FFFFFF", "#0079d3"),
+               "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, "ACCENT1": "#ff5414", "ACCENT2": "#33a8ff",
+               "ACCENT3": "#dbf0ff", },
+    "Topanga": {"BACKGROUND": "#282923", "TEXT": "#E7DB74", "INPUT": "#393a32", "TEXT_INPUT": "#E7C855", "SCROLL": "#E7C855", "BUTTON": ("#E7C855", "#284B5A"),
+                "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, "ACCENT1": "#c15226", "ACCENT2": "#7a4d5f",
+                "ACCENT3": "#889743", },
+    "GreenTan": {"BACKGROUND": "#9FB8AD", "TEXT": '#000000', "INPUT": "#F7F3EC", "TEXT_INPUT": "#000000", "SCROLL": "#F7F3EC", "BUTTON": ("#FFFFFF", "#475841"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Dark": {"BACKGROUND": "#404040", "TEXT": "#FFFFFF", "INPUT": "#4D4D4D", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#707070", "BUTTON": ("#FFFFFF", "#004F00"),
+             "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightGreen": {"BACKGROUND": "#B7CECE", "TEXT": "#000000", "INPUT": "#FDFFF7", "TEXT_INPUT": "#000000", "SCROLL": "#FDFFF7",
+                   "BUTTON": ("#FFFFFF", "#658268"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "ACCENT1": "#76506d",
+                   "ACCENT2": "#5148f1", "ACCENT3": "#0a1c84", "PROGRESS_DEPTH": 0, },
+    "Dark2": {"BACKGROUND": "#404040", "TEXT": "#FFFFFF", "INPUT": "#FFFFFF", "TEXT_INPUT": "#000000", "SCROLL": "#707070", "BUTTON": ("#FFFFFF", "#004F00"),
+              "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Black": {"BACKGROUND": "#000000", "TEXT": "#FFFFFF", "INPUT": "#4D4D4D", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#707070", "BUTTON": ("#000000", "#FFFFFF"),
+              "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Black2": {"BACKGROUND": "#000000", "TEXT": "#FFFFFF", "INPUT": "#000000", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#FFFFFF", "BUTTON": ("#000000", "#FFFFFF"),
+               "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Tan": {"BACKGROUND": "#fdf6e3", "TEXT": "#268bd1", "INPUT": "#eee8d5", "TEXT_INPUT": "#6c71c3", "SCROLL": "#eee8d5", "BUTTON": ("#FFFFFF", "#063542"),
+            "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "TanBlue": {"BACKGROUND": "#e5dece", "TEXT": "#063289", "INPUT": "#f9f8f4", "TEXT_INPUT": "#242834", "SCROLL": "#eee8d5", "BUTTON": ("#FFFFFF", "#063289"),
+                "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkTanBlue": {"BACKGROUND": "#242834", "TEXT": "#dfe6f8", "INPUT": "#97755c", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#a9afbb",
+                    "BUTTON": ("#FFFFFF", "#063289"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkAmber": {"BACKGROUND": "#2c2825", "TEXT": "#fdcb52", "INPUT": "#705e52", "TEXT_INPUT": "#fdcb52", "SCROLL": "#705e52",
+                  "BUTTON": ("#000000", "#fdcb52"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBlue": {"BACKGROUND": "#1a2835", "TEXT": "#d1ecff", "INPUT": "#335267", "TEXT_INPUT": "#acc2d0", "SCROLL": "#1b6497", "BUTTON": ("#000000", "#fafaf8"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Reds": {"BACKGROUND": "#280001", "TEXT": "#FFFFFF", "INPUT": "#d8d584", "TEXT_INPUT": "#000000", "SCROLL": "#763e00", "BUTTON": ("#000000", "#daad28"),
+             "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Green": {"BACKGROUND": "#82a459", "TEXT": "#000000", "INPUT": "#d8d584", "TEXT_INPUT": "#000000", "SCROLL": "#e3ecf3", "BUTTON": ("#FFFFFF", "#517239"),
+              "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "BluePurple": {"BACKGROUND": "#A5CADD", "TEXT": "#6E266E", "INPUT": "#E0F5FF", "TEXT_INPUT": "#000000", "SCROLL": "#E0F5FF",
+                   "BUTTON": ("#FFFFFF", "#303952"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Purple": {"BACKGROUND": "#B0AAC2", "TEXT": "#000000", "INPUT": "#F2EFE8", "SCROLL": "#F2EFE8", "TEXT_INPUT": "#000000", "BUTTON": ("#000000", "#C2D4D8"),
+               "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "BlueMono": {"BACKGROUND": "#AAB6D3", "TEXT": "#000000", "INPUT": "#F1F4FC", "SCROLL": "#F1F4FC", "TEXT_INPUT": "#000000", "BUTTON": ("#FFFFFF", "#7186C7"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "GreenMono": {"BACKGROUND": "#A8C1B4", "TEXT": "#000000", "INPUT": "#DDE0DE", "SCROLL": "#E3E3E3", "TEXT_INPUT": "#000000",
+                  "BUTTON": ("#FFFFFF", "#6D9F85"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "BrownBlue": {"BACKGROUND": "#64778d", "TEXT": "#FFFFFF", "INPUT": "#f0f3f7", "SCROLL": "#A6B2BE", "TEXT_INPUT": "#000000",
+                  "BUTTON": ("#FFFFFF", "#283b5b"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "BrightColors": {"BACKGROUND": "#b4ffb4", "TEXT": "#000000", "INPUT": "#ffff64", "SCROLL": "#ffb482", "TEXT_INPUT": "#000000",
+                     "BUTTON": ("#000000", "#ffa0dc"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "NeutralBlue": {"BACKGROUND": "#92aa9d", "TEXT": "#000000", "INPUT": "#fcfff6", "SCROLL": "#fcfff6", "TEXT_INPUT": "#000000",
+                    "BUTTON": ("#000000", "#d0dbbd"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Kayak": {"BACKGROUND": "#a7ad7f", "TEXT": "#000000", "INPUT": "#e6d3a8", "SCROLL": "#e6d3a8", "TEXT_INPUT": "#000000", "BUTTON": ("#FFFFFF", "#5d907d"),
+              "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "SandyBeach": {"BACKGROUND": "#efeccb", "TEXT": "#012f2f", "INPUT": "#e6d3a8", "SCROLL": "#e6d3a8", "TEXT_INPUT": "#012f2f",
+                   "BUTTON": ("#FFFFFF", "#046380"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "TealMono": {"BACKGROUND": "#a8cfdd", "TEXT": "#000000", "INPUT": "#dfedf2", "SCROLL": "#dfedf2", "TEXT_INPUT": "#000000", "BUTTON": ("#FFFFFF", "#183440"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "Default": {"BACKGROUND": COLOR_SYSTEM_DEFAULT, "TEXT": COLOR_SYSTEM_DEFAULT, "INPUT": COLOR_SYSTEM_DEFAULT, "TEXT_INPUT": COLOR_SYSTEM_DEFAULT,
+                "SCROLL": COLOR_SYSTEM_DEFAULT, "BUTTON": OFFICIAL_PYSIMPLEGUI_BUTTON_COLOR, "PROGRESS": COLOR_SYSTEM_DEFAULT, "BORDER": 1, "SLIDER_DEPTH": 1,
+                "PROGRESS_DEPTH": 0, },
+    "Default1": {"BACKGROUND": COLOR_SYSTEM_DEFAULT, "TEXT": COLOR_SYSTEM_DEFAULT, "INPUT": COLOR_SYSTEM_DEFAULT, "TEXT_INPUT": COLOR_SYSTEM_DEFAULT,
+                 "SCROLL": COLOR_SYSTEM_DEFAULT, "BUTTON": COLOR_SYSTEM_DEFAULT, "PROGRESS": COLOR_SYSTEM_DEFAULT, "BORDER": 1, "SLIDER_DEPTH": 1,
+                 "PROGRESS_DEPTH": 0, },
+    "DefaultNoMoreNagging": {"BACKGROUND": COLOR_SYSTEM_DEFAULT, "TEXT": COLOR_SYSTEM_DEFAULT, "INPUT": COLOR_SYSTEM_DEFAULT,
+                             "TEXT_INPUT": COLOR_SYSTEM_DEFAULT, "SCROLL": COLOR_SYSTEM_DEFAULT, "BUTTON": OFFICIAL_PYSIMPLEGUI_BUTTON_COLOR,
+                             "PROGRESS": COLOR_SYSTEM_DEFAULT, "BORDER": 1, "SLIDER_DEPTH": 1, "PROGRESS_DEPTH": 0, },
+    "GrayGrayGray": {"BACKGROUND": COLOR_SYSTEM_DEFAULT, "TEXT": COLOR_SYSTEM_DEFAULT, "INPUT": COLOR_SYSTEM_DEFAULT, "TEXT_INPUT": COLOR_SYSTEM_DEFAULT,
+                     "SCROLL": COLOR_SYSTEM_DEFAULT, "BUTTON": COLOR_SYSTEM_DEFAULT, "PROGRESS": COLOR_SYSTEM_DEFAULT, "BORDER": 1, "SLIDER_DEPTH": 1,
+                     "PROGRESS_DEPTH": 0, },
+    "LightBlue": {"BACKGROUND": "#E3F2FD", "TEXT": "#000000", "INPUT": "#86A8FF", "TEXT_INPUT": "#000000", "SCROLL": "#86A8FF",
+                  "BUTTON": ("#FFFFFF", "#5079D3"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 0, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "ACCENT1": "#FF0266", "ACCENT2": "#FF5C93", "ACCENT3": "#C5003C", },
+    "LightGrey": {"BACKGROUND": "#FAFAFA", "TEXT": "#000000", "INPUT": "#004EA1", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#5EA7FF",
+                  "BUTTON": ("#FFFFFF", "#0079D3"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 0, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "ACCENT1": "#FF0266", "ACCENT2": "#FF5C93", "ACCENT3": "#C5003C", },
+    "LightGrey1": {"BACKGROUND": "#ffffff", "TEXT": "#1a1a1b", "INPUT": "#dae0e6", "TEXT_INPUT": "#222222", "SCROLL": "#a5a4a4",
+                   "BUTTON": ("#FFFFFF", "#0079d3"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "ACCENT1": "#ff5414", "ACCENT2": "#33a8ff", "ACCENT3": "#dbf0ff", },
+    "DarkBrown": {"BACKGROUND": "#282923", "TEXT": "#E7DB74", "INPUT": "#393a32", "TEXT_INPUT": "#E7C855", "SCROLL": "#E7C855",
+                  "BUTTON": ("#E7C855", "#284B5A"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "ACCENT1": "#c15226", "ACCENT2": "#7a4d5f", "ACCENT3": "#889743", },
+    "LightGreen1": {"BACKGROUND": "#9FB8AD", "TEXT": "#000000", "INPUT": "#F7F3EC", "TEXT_INPUT": "#000000", "SCROLL": "#F7F3EC",
+                    "BUTTON": ("#FFFFFF", "#475841"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey": {"BACKGROUND": "#404040", "TEXT": "#FFFFFF", "INPUT": "#4D4D4D", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#707070", "BUTTON": ("#FFFFFF", "#004F00"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightGreen2": {"BACKGROUND": "#B7CECE", "TEXT": "#000000", "INPUT": "#FDFFF7", "TEXT_INPUT": "#000000", "SCROLL": "#FDFFF7",
+                    "BUTTON": ("#FFFFFF", "#658268"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "ACCENT1": "#76506d",
+                    "ACCENT2": "#5148f1", "ACCENT3": "#0a1c84", "PROGRESS_DEPTH": 0, },
+    "DarkGrey1": {"BACKGROUND": "#404040", "TEXT": "#FFFFFF", "INPUT": "#FFFFFF", "TEXT_INPUT": "#000000", "SCROLL": "#707070",
+                  "BUTTON": ("#FFFFFF", "#004F00"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBlack": {"BACKGROUND": "#000000", "TEXT": "#FFFFFF", "INPUT": "#4D4D4D", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#707070",
+                  "BUTTON": ("#000000", "#FFFFFF"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBrown": {"BACKGROUND": "#fdf6e3", "TEXT": "#268bd1", "INPUT": "#eee8d5", "TEXT_INPUT": "#6c71c3", "SCROLL": "#eee8d5",
+                   "BUTTON": ("#FFFFFF", "#063542"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBrown1": {"BACKGROUND": "#e5dece", "TEXT": "#063289", "INPUT": "#f9f8f4", "TEXT_INPUT": "#242834", "SCROLL": "#eee8d5",
+                    "BUTTON": ("#FFFFFF", "#063289"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBlue1": {"BACKGROUND": "#242834", "TEXT": "#dfe6f8", "INPUT": "#97755c", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#a9afbb",
+                  "BUTTON": ("#FFFFFF", "#063289"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBrown1": {"BACKGROUND": "#2c2825", "TEXT": "#fdcb52", "INPUT": "#705e52", "TEXT_INPUT": "#fdcb52", "SCROLL": "#705e52",
+                   "BUTTON": ("#000000", "#fdcb52"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBlue2": {"BACKGROUND": "#1a2835", "TEXT": "#d1ecff", "INPUT": "#335267", "TEXT_INPUT": "#acc2d0", "SCROLL": "#1b6497",
+                  "BUTTON": ("#000000", "#fafaf8"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBrown2": {"BACKGROUND": "#280001", "TEXT": "#FFFFFF", "INPUT": "#d8d584", "TEXT_INPUT": "#000000", "SCROLL": "#763e00",
+                   "BUTTON": ("#000000", "#daad28"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGreen": {"BACKGROUND": "#82a459", "TEXT": "#000000", "INPUT": "#d8d584", "TEXT_INPUT": "#000000", "SCROLL": "#e3ecf3",
+                  "BUTTON": ("#FFFFFF", "#517239"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBlue1": {"BACKGROUND": "#A5CADD", "TEXT": "#6E266E", "INPUT": "#E0F5FF", "TEXT_INPUT": "#000000", "SCROLL": "#E0F5FF",
+                   "BUTTON": ("#FFFFFF", "#303952"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightPurple": {"BACKGROUND": "#B0AAC2", "TEXT": "#000000", "INPUT": "#F2EFE8", "SCROLL": "#F2EFE8", "TEXT_INPUT": "#000000",
+                    "BUTTON": ("#000000", "#C2D4D8"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBlue2": {"BACKGROUND": "#AAB6D3", "TEXT": "#000000", "INPUT": "#F1F4FC", "SCROLL": "#F1F4FC", "TEXT_INPUT": "#000000",
+                   "BUTTON": ("#FFFFFF", "#7186C7"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightGreen3": {"BACKGROUND": "#A8C1B4", "TEXT": "#000000", "INPUT": "#DDE0DE", "SCROLL": "#E3E3E3", "TEXT_INPUT": "#000000",
+                    "BUTTON": ("#FFFFFF", "#6D9F85"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBlue3": {"BACKGROUND": "#64778d", "TEXT": "#FFFFFF", "INPUT": "#f0f3f7", "SCROLL": "#A6B2BE", "TEXT_INPUT": "#000000",
+                  "BUTTON": ("#FFFFFF", "#283b5b"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightGreen4": {"BACKGROUND": "#b4ffb4", "TEXT": "#000000", "INPUT": "#ffff64", "SCROLL": "#ffb482", "TEXT_INPUT": "#000000",
+                    "BUTTON": ("#000000", "#ffa0dc"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightGreen5": {"BACKGROUND": "#92aa9d", "TEXT": "#000000", "INPUT": "#fcfff6", "SCROLL": "#fcfff6", "TEXT_INPUT": "#000000",
+                    "BUTTON": ("#000000", "#d0dbbd"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBrown2": {"BACKGROUND": "#a7ad7f", "TEXT": "#000000", "INPUT": "#e6d3a8", "SCROLL": "#e6d3a8", "TEXT_INPUT": "#000000",
+                    "BUTTON": ("#FFFFFF", "#5d907d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBrown3": {"BACKGROUND": "#efeccb", "TEXT": "#012f2f", "INPUT": "#e6d3a8", "SCROLL": "#e6d3a8", "TEXT_INPUT": "#012f2f",
+                    "BUTTON": ("#FFFFFF", "#046380"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBlue3": {"BACKGROUND": "#a8cfdd", "TEXT": "#000000", "INPUT": "#dfedf2", "SCROLL": "#dfedf2", "TEXT_INPUT": "#000000",
+                   "BUTTON": ("#FFFFFF", "#183440"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "LightBrown4": {"BACKGROUND": "#d7c79e", "TEXT": "#a35638", "INPUT": "#9dab86", "TEXT_INPUT": "#000000", "SCROLL": "#a35638",
+                    "BUTTON": ("#FFFFFF", "#a35638"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#a35638", "#9dab86", "#e08f62", "#d7c79e"], },
+    "DarkTeal": {"BACKGROUND": "#003f5c", "TEXT": "#fb5b5a", "INPUT": "#bc4873", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#bc4873", "BUTTON": ("#FFFFFF", "#fb5b5a"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                 "COLOR_LIST": ["#003f5c", "#472b62", "#bc4873", "#fb5b5a"], },
+    "DarkPurple": {"BACKGROUND": "#472b62", "TEXT": "#fb5b5a", "INPUT": "#bc4873", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#bc4873",
+                   "BUTTON": ("#FFFFFF", "#472b62"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#003f5c", "#472b62", "#bc4873", "#fb5b5a"], },
+    "LightGreen6": {"BACKGROUND": "#eafbea", "TEXT": "#1f6650", "INPUT": "#6f9a8d", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#1f6650",
+                    "BUTTON": ("#FFFFFF", "#1f6650"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#1f6650", "#6f9a8d", "#ea5e5e", "#eafbea"], },
+    "DarkGrey2": {"BACKGROUND": "#2b2b28", "TEXT": "#f8f8f8", "INPUT": "#f1d6ab", "TEXT_INPUT": "#000000", "SCROLL": "#f1d6ab",
+                  "BUTTON": ("#2b2b28", "#e3b04b"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#2b2b28", "#e3b04b", "#f1d6ab", "#f8f8f8"], },
+    "LightBrown6": {"BACKGROUND": "#f9b282", "TEXT": "#8f4426", "INPUT": "#de6b35", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#8f4426",
+                    "BUTTON": ("#FFFFFF", "#8f4426"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#8f4426", "#de6b35", "#64ccda", "#f9b282"], },
+    "DarkTeal1": {"BACKGROUND": "#396362", "TEXT": "#ffe7d1", "INPUT": "#f6c89f", "TEXT_INPUT": "#000000", "SCROLL": "#f6c89f",
+                  "BUTTON": ("#ffe7d1", "#4b8e8d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#396362", "#4b8e8d", "#f6c89f", "#ffe7d1"], },
+    "LightBrown7": {"BACKGROUND": "#f6c89f", "TEXT": "#396362", "INPUT": "#4b8e8d", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#396362",
+                    "BUTTON": ("#FFFFFF", "#396362"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#396362", "#4b8e8d", "#f6c89f", "#ffe7d1"], },
+    "DarkPurple1": {"BACKGROUND": "#0c093c", "TEXT": "#fad6d6", "INPUT": "#eea5f6", "TEXT_INPUT": "#000000", "SCROLL": "#eea5f6",
+                    "BUTTON": ("#FFFFFF", "#df42d1"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#0c093c", "#df42d1", "#eea5f6", "#fad6d6"], },
+    "DarkGrey3": {"BACKGROUND": "#211717", "TEXT": "#dfddc7", "INPUT": "#f58b54", "TEXT_INPUT": "#000000", "SCROLL": "#f58b54",
+                  "BUTTON": ("#dfddc7", "#a34a28"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#211717", "#a34a28", "#f58b54", "#dfddc7"], },
+    "LightBrown8": {"BACKGROUND": "#dfddc7", "TEXT": "#211717", "INPUT": "#a34a28", "TEXT_INPUT": "#dfddc7", "SCROLL": "#211717",
+                    "BUTTON": ("#dfddc7", "#a34a28"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#211717", "#a34a28", "#f58b54", "#dfddc7"], },
+    "DarkBlue4": {"BACKGROUND": "#494ca2", "TEXT": "#e3e7f1", "INPUT": "#c6cbef", "TEXT_INPUT": "#000000", "SCROLL": "#c6cbef",
+                  "BUTTON": ("#FFFFFF", "#8186d5"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#494ca2", "#8186d5", "#c6cbef", "#e3e7f1"], },
+    "LightBlue4": {"BACKGROUND": "#5c94bd", "TEXT": "#470938", "INPUT": "#1a3e59", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#470938",
+                   "BUTTON": ("#FFFFFF", "#470938"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#470938", "#1a3e59", "#5c94bd", "#f2d6eb"], },
+    "DarkTeal2": {"BACKGROUND": "#394a6d", "TEXT": "#c0ffb3", "INPUT": "#52de97", "TEXT_INPUT": "#000000", "SCROLL": "#52de97",
+                  "BUTTON": ("#c0ffb3", "#394a6d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#394a6d", "#3c9d9b", "#52de97", "#c0ffb3"], },
+    "DarkTeal3": {"BACKGROUND": "#3c9d9b", "TEXT": "#c0ffb3", "INPUT": "#52de97", "TEXT_INPUT": "#000000", "SCROLL": "#52de97",
+                  "BUTTON": ("#c0ffb3", "#394a6d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#394a6d", "#3c9d9b", "#52de97", "#c0ffb3"], },
+    "DarkPurple5": {"BACKGROUND": "#730068", "TEXT": "#f6f078", "INPUT": "#01d28e", "TEXT_INPUT": "#000000", "SCROLL": "#01d28e",
+                    "BUTTON": ("#f6f078", "#730068"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#730068", "#434982", "#01d28e", "#f6f078"], },
+    "DarkPurple2": {"BACKGROUND": "#202060", "TEXT": "#b030b0", "INPUT": "#602080", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#602080",
+                    "BUTTON": ("#FFFFFF", "#202040"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#202040", "#202060", "#602080", "#b030b0"], },
+    "DarkBlue5": {"BACKGROUND": "#000272", "TEXT": "#ff6363", "INPUT": "#a32f80", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#a32f80",
+                  "BUTTON": ("#FFFFFF", "#341677"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#000272", "#341677", "#a32f80", "#ff6363"], },
+    "LightGrey2": {"BACKGROUND": "#f6f6f6", "TEXT": "#420000", "INPUT": "#d4d7dd", "TEXT_INPUT": "#420000", "SCROLL": "#420000",
+                   "BUTTON": ("#420000", "#d4d7dd"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#420000", "#d4d7dd", "#eae9e9", "#f6f6f6"], },
+    "LightGrey3": {"BACKGROUND": "#eae9e9", "TEXT": "#420000", "INPUT": "#d4d7dd", "TEXT_INPUT": "#420000", "SCROLL": "#420000",
+                   "BUTTON": ("#420000", "#d4d7dd"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#420000", "#d4d7dd", "#eae9e9", "#f6f6f6"], },
+    "DarkBlue6": {"BACKGROUND": "#01024e", "TEXT": "#ff6464", "INPUT": "#8b4367", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#8b4367",
+                  "BUTTON": ("#FFFFFF", "#543864"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#01024e", "#543864", "#8b4367", "#ff6464"], },
+    "DarkBlue7": {"BACKGROUND": "#241663", "TEXT": "#eae7af", "INPUT": "#a72693", "TEXT_INPUT": "#eae7af", "SCROLL": "#a72693",
+                  "BUTTON": ("#eae7af", "#160f30"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#160f30", "#241663", "#a72693", "#eae7af"], },
+    "LightBrown9": {"BACKGROUND": "#f6d365", "TEXT": "#3a1f5d", "INPUT": "#c83660", "TEXT_INPUT": "#f6d365", "SCROLL": "#3a1f5d",
+                    "BUTTON": ("#f6d365", "#c83660"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#3a1f5d", "#c83660", "#e15249", "#f6d365"], },
+    "DarkPurple3": {"BACKGROUND": "#6e2142", "TEXT": "#ffd692", "INPUT": "#e16363", "TEXT_INPUT": "#ffd692", "SCROLL": "#e16363",
+                    "BUTTON": ("#ffd692", "#943855"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#6e2142", "#943855", "#e16363", "#ffd692"], },
+    "LightBrown10": {"BACKGROUND": "#ffd692", "TEXT": "#6e2142", "INPUT": "#943855", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#6e2142",
+                     "BUTTON": ("#FFFFFF", "#6e2142"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                     "COLOR_LIST": ["#6e2142", "#943855", "#e16363", "#ffd692"], },
+    "DarkPurple4": {"BACKGROUND": "#200f21", "TEXT": "#f638dc", "INPUT": "#5a3d5c", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#5a3d5c",
+                    "BUTTON": ("#FFFFFF", "#382039"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#200f21", "#382039", "#5a3d5c", "#f638dc"], },
+    "LightBlue5": {"BACKGROUND": "#b2fcff", "TEXT": "#3e64ff", "INPUT": "#5edfff", "TEXT_INPUT": "#000000", "SCROLL": "#3e64ff",
+                   "BUTTON": ("#FFFFFF", "#3e64ff"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#3e64ff", "#5edfff", "#b2fcff", "#ecfcff"], },
+    "DarkTeal4": {"BACKGROUND": "#464159", "TEXT": "#c7f0db", "INPUT": "#8bbabb", "TEXT_INPUT": "#000000", "SCROLL": "#8bbabb",
+                  "BUTTON": ("#FFFFFF", "#6c7b95"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#464159", "#6c7b95", "#8bbabb", "#c7f0db"], },
+    "LightTeal": {"BACKGROUND": "#c7f0db", "TEXT": "#464159", "INPUT": "#6c7b95", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#464159",
+                  "BUTTON": ("#FFFFFF", "#464159"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#464159", "#6c7b95", "#8bbabb", "#c7f0db"], },
+    "DarkTeal5": {"BACKGROUND": "#8bbabb", "TEXT": "#464159", "INPUT": "#6c7b95", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#464159",
+                  "BUTTON": ("#c7f0db", "#6c7b95"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#464159", "#6c7b95", "#8bbabb", "#c7f0db"], },
+    "LightGrey4": {"BACKGROUND": "#faf5ef", "TEXT": "#672f2f", "INPUT": "#99b19c", "TEXT_INPUT": "#672f2f", "SCROLL": "#672f2f",
+                   "BUTTON": ("#672f2f", "#99b19c"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#672f2f", "#99b19c", "#d7d1c9", "#faf5ef"], },
+    "LightGreen7": {"BACKGROUND": "#99b19c", "TEXT": "#faf5ef", "INPUT": "#d7d1c9", "TEXT_INPUT": "#000000", "SCROLL": "#d7d1c9",
+                    "BUTTON": ("#FFFFFF", "#99b19c"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#672f2f", "#99b19c", "#d7d1c9", "#faf5ef"], },
+    "LightGrey5": {"BACKGROUND": "#d7d1c9", "TEXT": "#672f2f", "INPUT": "#99b19c", "TEXT_INPUT": "#672f2f", "SCROLL": "#672f2f",
+                   "BUTTON": ("#FFFFFF", "#672f2f"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#672f2f", "#99b19c", "#d7d1c9", "#faf5ef"], },
+    "DarkBrown3": {"BACKGROUND": "#a0855b", "TEXT": "#f9f6f2", "INPUT": "#f1d6ab", "TEXT_INPUT": "#000000", "SCROLL": "#f1d6ab",
+                   "BUTTON": ("#FFFFFF", "#38470b"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#38470b", "#a0855b", "#f1d6ab", "#f9f6f2"], },
+    "LightBrown11": {"BACKGROUND": "#f1d6ab", "TEXT": "#38470b", "INPUT": "#a0855b", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#38470b",
+                     "BUTTON": ("#f9f6f2", "#a0855b"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                     "COLOR_LIST": ["#38470b", "#a0855b", "#f1d6ab", "#f9f6f2"], },
+    "DarkRed": {"BACKGROUND": "#83142c", "TEXT": "#f9d276", "INPUT": "#ad1d45", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#ad1d45", "BUTTON": ("#f9d276", "#ad1d45"),
+                "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                "COLOR_LIST": ["#44000d", "#83142c", "#ad1d45", "#f9d276"], },
+    "DarkTeal6": {"BACKGROUND": "#204969", "TEXT": "#fff7f7", "INPUT": "#dadada", "TEXT_INPUT": "#000000", "SCROLL": "#dadada",
+                  "BUTTON": ("#000000", "#fff7f7"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#204969", "#08ffc8", "#dadada", "#fff7f7"], },
+    "DarkBrown4": {"BACKGROUND": "#252525", "TEXT": "#ff0000", "INPUT": "#af0404", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#af0404",
+                   "BUTTON": ("#FFFFFF", "#252525"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#252525", "#414141", "#af0404", "#ff0000"], },
+    "LightYellow": {"BACKGROUND": "#f4ff61", "TEXT": "#27aa80", "INPUT": "#32ff6a", "TEXT_INPUT": "#000000", "SCROLL": "#27aa80",
+                    "BUTTON": ("#f4ff61", "#27aa80"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#27aa80", "#32ff6a", "#a8ff3e", "#f4ff61"], },
+    "DarkGreen1": {"BACKGROUND": "#2b580c", "TEXT": "#fdef96", "INPUT": "#f7b71d", "TEXT_INPUT": "#000000", "SCROLL": "#f7b71d",
+                   "BUTTON": ("#fdef96", "#2b580c"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#2b580c", "#afa939", "#f7b71d", "#fdef96"], },
+    "LightGreen8": {"BACKGROUND": "#c8dad3", "TEXT": "#63707e", "INPUT": "#93b5b3", "TEXT_INPUT": "#000000", "SCROLL": "#63707e",
+                    "BUTTON": ("#FFFFFF", "#63707e"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#63707e", "#93b5b3", "#c8dad3", "#f2f6f5"], },
+    "DarkTeal7": {"BACKGROUND": "#248ea9", "TEXT": "#fafdcb", "INPUT": "#aee7e8", "TEXT_INPUT": "#000000", "SCROLL": "#aee7e8",
+                  "BUTTON": ("#000000", "#fafdcb"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#248ea9", "#28c3d4", "#aee7e8", "#fafdcb"], },
+    "DarkBlue8": {"BACKGROUND": "#454d66", "TEXT": "#d9d872", "INPUT": "#58b368", "TEXT_INPUT": "#000000", "SCROLL": "#58b368",
+                  "BUTTON": ("#000000", "#009975"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#009975", "#454d66", "#58b368", "#d9d872"], },
+    "DarkBlue9": {"BACKGROUND": "#263859", "TEXT": "#ff6768", "INPUT": "#6b778d", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#6b778d",
+                  "BUTTON": ("#ff6768", "#263859"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#17223b", "#263859", "#6b778d", "#ff6768"], },
+    "DarkBlue10": {"BACKGROUND": "#0028ff", "TEXT": "#f1f4df", "INPUT": "#10eaf0", "TEXT_INPUT": "#000000", "SCROLL": "#10eaf0",
+                   "BUTTON": ("#f1f4df", "#24009c"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#24009c", "#0028ff", "#10eaf0", "#f1f4df"], },
+    "DarkBlue11": {"BACKGROUND": "#6384b3", "TEXT": "#e6f0b6", "INPUT": "#b8e9c0", "TEXT_INPUT": "#000000", "SCROLL": "#b8e9c0",
+                   "BUTTON": ("#e6f0b6", "#684949"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#684949", "#6384b3", "#b8e9c0", "#e6f0b6"], },
+    "DarkTeal8": {"BACKGROUND": "#71a0a5", "TEXT": "#212121", "INPUT": "#665c84", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#212121",
+                  "BUTTON": ("#fab95b", "#665c84"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#212121", "#665c84", "#71a0a5", "#fab95b"], },
+    "DarkRed1": {"BACKGROUND": "#c10000", "TEXT": "#eeeeee", "INPUT": "#dedede", "TEXT_INPUT": "#000000", "SCROLL": "#dedede", "BUTTON": ("#c10000", "#eeeeee"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                 "COLOR_LIST": ["#c10000", "#ff4949", "#dedede", "#eeeeee"], },
+    "LightBrown5": {"BACKGROUND": "#fff591", "TEXT": "#e41749", "INPUT": "#f5587b", "TEXT_INPUT": "#000000", "SCROLL": "#e41749",
+                    "BUTTON": ("#fff591", "#e41749"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#e41749", "#f5587b", "#ff8a5c", "#fff591"], },
+    "LightGreen9": {"BACKGROUND": "#f1edb3", "TEXT": "#3b503d", "INPUT": "#4a746e", "TEXT_INPUT": "#f1edb3", "SCROLL": "#3b503d",
+                    "BUTTON": ("#f1edb3", "#3b503d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#3b503d", "#4a746e", "#c8cf94", "#f1edb3"], "DESCRIPTION": ["Green", "Turquoise", "Yellow"], },
+    "DarkGreen2": {"BACKGROUND": "#3b503d", "TEXT": "#f1edb3", "INPUT": "#c8cf94", "TEXT_INPUT": "#000000", "SCROLL": "#c8cf94",
+                   "BUTTON": ("#f1edb3", "#3b503d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#3b503d", "#4a746e", "#c8cf94", "#f1edb3"], "DESCRIPTION": ["Green", "Turquoise", "Yellow"], },
+    "LightGray1": {"BACKGROUND": "#f2f2f2", "TEXT": "#222831", "INPUT": "#393e46", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#222831",
+                   "BUTTON": ("#f2f2f2", "#222831"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#222831", "#393e46", "#f96d00", "#f2f2f2"], "DESCRIPTION": ["#000000", "Grey", "Orange", "Grey", "Autumn"], },
+    "DarkGrey4": {"BACKGROUND": "#52524e", "TEXT": "#e9e9e5", "INPUT": "#d4d6c8", "TEXT_INPUT": "#000000", "SCROLL": "#d4d6c8",
+                  "BUTTON": ("#FFFFFF", "#9a9b94"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#52524e", "#9a9b94", "#d4d6c8", "#e9e9e5"], "DESCRIPTION": ["Grey", "Pastel", "Winter"], },
+    "DarkBlue12": {"BACKGROUND": "#324e7b", "TEXT": "#f8f8f8", "INPUT": "#86a6df", "TEXT_INPUT": "#000000", "SCROLL": "#86a6df",
+                   "BUTTON": ("#FFFFFF", "#5068a9"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#324e7b", "#5068a9", "#86a6df", "#f8f8f8"], "DESCRIPTION": ["Blue", "Grey", "Cold", "Winter"], },
+    "DarkPurple6": {"BACKGROUND": "#070739", "TEXT": "#e1e099", "INPUT": "#c327ab", "TEXT_INPUT": "#e1e099", "SCROLL": "#c327ab",
+                    "BUTTON": ("#e1e099", "#521477"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                    "COLOR_LIST": ["#070739", "#521477", "#c327ab", "#e1e099"], "DESCRIPTION": ["#000000", "Purple", "Yellow", "Dark"], },
+    "DarkPurple7": {"BACKGROUND": "#191930", "TEXT": "#B1B7C5", "INPUT": "#232B5C", "TEXT_INPUT": "#D0E3E7", "SCROLL": "#B1B7C5",
+                    "BUTTON": ("#272D38", "#B1B7C5"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkBlue13": {"BACKGROUND": "#203562", "TEXT": "#e3e8f8", "INPUT": "#c0c5cd", "TEXT_INPUT": "#000000", "SCROLL": "#c0c5cd",
+                   "BUTTON": ("#FFFFFF", "#3e588f"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#203562", "#3e588f", "#c0c5cd", "#e3e8f8"], "DESCRIPTION": ["Blue", "Grey", "Wedding", "Cold"], },
+    "DarkBrown5": {"BACKGROUND": "#3c1b1f", "TEXT": "#f6e1b5", "INPUT": "#e2bf81", "TEXT_INPUT": "#000000", "SCROLL": "#e2bf81",
+                   "BUTTON": ("#3c1b1f", "#f6e1b5"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#3c1b1f", "#b21e4b", "#e2bf81", "#f6e1b5"], "DESCRIPTION": ["Brown", "Red", "Yellow", "Warm"], },
+    "DarkGreen3": {"BACKGROUND": "#062121", "TEXT": "#eeeeee", "INPUT": "#e4dcad", "TEXT_INPUT": "#000000", "SCROLL": "#e4dcad",
+                   "BUTTON": ("#eeeeee", "#181810"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#062121", "#181810", "#e4dcad", "#eeeeee"], "DESCRIPTION": ["#000000", "#000000", "Brown", "Grey"], },
+    "DarkBlack1": {"BACKGROUND": "#181810", "TEXT": "#eeeeee", "INPUT": "#e4dcad", "TEXT_INPUT": "#000000", "SCROLL": "#e4dcad",
+                   "BUTTON": ("#FFFFFF", "#062121"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#062121", "#181810", "#e4dcad", "#eeeeee"], "DESCRIPTION": ["#000000", "#000000", "Brown", "Grey"], },
+    "DarkGrey5": {"BACKGROUND": "#343434", "TEXT": "#f3f3f3", "INPUT": "#e9dcbe", "TEXT_INPUT": "#000000", "SCROLL": "#e9dcbe",
+                  "BUTTON": ("#FFFFFF", "#8e8b82"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#343434", "#8e8b82", "#e9dcbe", "#f3f3f3"], "DESCRIPTION": ["Grey", "Brown"], },
+    "LightBrown12": {"BACKGROUND": "#8e8b82", "TEXT": "#f3f3f3", "INPUT": "#e9dcbe", "TEXT_INPUT": "#000000", "SCROLL": "#e9dcbe",
+                     "BUTTON": ("#f3f3f3", "#8e8b82"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                     "COLOR_LIST": ["#343434", "#8e8b82", "#e9dcbe", "#f3f3f3"], "DESCRIPTION": ["Grey", "Brown"], },
+    "DarkTeal9": {"BACKGROUND": "#13445a", "TEXT": "#fef4e8", "INPUT": "#446878", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#446878",
+                  "BUTTON": ("#fef4e8", "#446878"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#13445a", "#970747", "#446878", "#fef4e8"], "DESCRIPTION": ["Red", "Grey", "Blue", "Wedding", "Retro"], },
+    "DarkBlue14": {"BACKGROUND": "#21273d", "TEXT": "#f1f6f8", "INPUT": "#b9d4f1", "TEXT_INPUT": "#000000", "SCROLL": "#b9d4f1",
+                   "BUTTON": ("#FFFFFF", "#6a759b"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#21273d", "#6a759b", "#b9d4f1", "#f1f6f8"], "DESCRIPTION": ["Blue", "#000000", "Grey", "Cold", "Winter"], },
+    "LightBlue6": {"BACKGROUND": "#f1f6f8", "TEXT": "#21273d", "INPUT": "#6a759b", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#21273d",
+                   "BUTTON": ("#f1f6f8", "#6a759b"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#21273d", "#6a759b", "#b9d4f1", "#f1f6f8"], "DESCRIPTION": ["Blue", "#000000", "Grey", "Cold", "Winter"], },
+    "DarkGreen4": {"BACKGROUND": "#044343", "TEXT": "#e4e4e4", "INPUT": "#045757", "TEXT_INPUT": "#e4e4e4", "SCROLL": "#045757",
+                   "BUTTON": ("#e4e4e4", "#045757"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#222222", "#044343", "#045757", "#e4e4e4"], "DESCRIPTION": ["#000000", "Turquoise", "Grey", "Dark"], },
+    "DarkGreen5": {"BACKGROUND": "#1b4b36", "TEXT": "#e0e7f1", "INPUT": "#aebd77", "TEXT_INPUT": "#000000", "SCROLL": "#aebd77",
+                   "BUTTON": ("#FFFFFF", "#538f6a"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#1b4b36", "#538f6a", "#aebd77", "#e0e7f1"], "DESCRIPTION": ["Green", "Grey"], },
+    "DarkTeal10": {"BACKGROUND": "#0d3446", "TEXT": "#d8dfe2", "INPUT": "#71adb5", "TEXT_INPUT": "#000000", "SCROLL": "#71adb5",
+                   "BUTTON": ("#FFFFFF", "#176d81"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#0d3446", "#176d81", "#71adb5", "#d8dfe2"], "DESCRIPTION": ["Grey", "Turquoise", "Winter", "Cold"], },
+    "DarkGrey6": {"BACKGROUND": "#3e3e3e", "TEXT": "#ededed", "INPUT": "#68868c", "TEXT_INPUT": "#ededed", "SCROLL": "#68868c",
+                  "BUTTON": ("#FFFFFF", "#405559"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#3e3e3e", "#405559", "#68868c", "#ededed"], "DESCRIPTION": ["Grey", "Turquoise", "Winter"], },
+    "DarkTeal11": {"BACKGROUND": "#405559", "TEXT": "#ededed", "INPUT": "#68868c", "TEXT_INPUT": "#ededed", "SCROLL": "#68868c",
+                   "BUTTON": ("#ededed", "#68868c"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#3e3e3e", "#405559", "#68868c", "#ededed"], "DESCRIPTION": ["Grey", "Turquoise", "Winter"], },
+    "LightBlue7": {"BACKGROUND": "#9ed0e0", "TEXT": "#19483f", "INPUT": "#5c868e", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#19483f",
+                   "BUTTON": ("#FFFFFF", "#19483f"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#19483f", "#5c868e", "#ff6a38", "#9ed0e0"], "DESCRIPTION": ["Orange", "Blue", "Turquoise"], },
+    "LightGreen10": {"BACKGROUND": "#d8ebb5", "TEXT": "#205d67", "INPUT": "#639a67", "TEXT_INPUT": "#FFFFFF", "SCROLL": "#205d67",
+                     "BUTTON": ("#d8ebb5", "#205d67"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                     "COLOR_LIST": ["#205d67", "#639a67", "#d9bf77", "#d8ebb5"], "DESCRIPTION": ["Blue", "Green", "Brown", "Vintage"], },
+    "DarkBlue15": {"BACKGROUND": "#151680", "TEXT": "#f1fea4", "INPUT": "#375fc0", "TEXT_INPUT": "#f1fea4", "SCROLL": "#375fc0",
+                   "BUTTON": ("#f1fea4", "#1c44ac"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#151680", "#1c44ac", "#375fc0", "#f1fea4"], "DESCRIPTION": ["Blue", "Yellow", "Cold"], },
+    "DarkBlue16": {"BACKGROUND": "#1c44ac", "TEXT": "#f1fea4", "INPUT": "#375fc0", "TEXT_INPUT": "#f1fea4", "SCROLL": "#375fc0",
+                   "BUTTON": ("#f1fea4", "#151680"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#151680", "#1c44ac", "#375fc0", "#f1fea4"], "DESCRIPTION": ["Blue", "Yellow", "Cold"], },
+    "DarkTeal12": {"BACKGROUND": "#004a7c", "TEXT": "#fafafa", "INPUT": "#e8f1f5", "TEXT_INPUT": "#000000", "SCROLL": "#e8f1f5",
+                   "BUTTON": ("#fafafa", "#005691"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#004a7c", "#005691", "#e8f1f5", "#fafafa"], "DESCRIPTION": ["Grey", "Blue", "Cold", "Winter"], },
+    "LightBrown13": {"BACKGROUND": "#ebf5ee", "TEXT": "#921224", "INPUT": "#bdc6b8", "TEXT_INPUT": "#921224", "SCROLL": "#921224",
+                     "BUTTON": ("#FFFFFF", "#921224"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                     "COLOR_LIST": ["#921224", "#bdc6b8", "#bce0da", "#ebf5ee"], "DESCRIPTION": ["Red", "Blue", "Grey", "Vintage", "Wedding"], },
+    "DarkBlue17": {"BACKGROUND": "#21294c", "TEXT": "#f9f2d7", "INPUT": "#f2dea8", "TEXT_INPUT": "#000000", "SCROLL": "#f2dea8",
+                   "BUTTON": ("#f9f2d7", "#141829"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#141829", "#21294c", "#f2dea8", "#f9f2d7"], "DESCRIPTION": ["#000000", "Blue", "Yellow"], },
+    "DarkBlue18": {"BACKGROUND": "#0c1825", "TEXT": "#d1d7dd", "INPUT": "#001c35", "TEXT_INPUT": "#d1d7dd", "SCROLL": "#00438e",
+                   "BUTTON": ("#75b7ff", "#001c35"), "PROGRESS": ('#0074ff', '#75b7ff'), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#141829", "#21294c", "#f2dea8", "#f9f2d7"], "DESCRIPTION": ["#000000", "Blue", "Yellow"], },
+    "DarkBrown6": {"BACKGROUND": "#785e4d", "TEXT": "#f2eee3", "INPUT": "#baaf92", "TEXT_INPUT": "#000000", "SCROLL": "#baaf92",
+                   "BUTTON": ("#FFFFFF", "#785e4d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#785e4d", "#ff8426", "#baaf92", "#f2eee3"], "DESCRIPTION": ["Grey", "Brown", "Orange", "Autumn"], },
+    "DarkGreen6": {"BACKGROUND": "#5c715e", "TEXT": "#f2f9f1", "INPUT": "#ddeedf", "TEXT_INPUT": "#000000", "SCROLL": "#ddeedf",
+                   "BUTTON": ("#f2f9f1", "#5c715e"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#5c715e", "#b6cdbd", "#ddeedf", "#f2f9f1"], "DESCRIPTION": ["Grey", "Green", "Vintage"], },
+    "DarkGreen7": {"BACKGROUND": "#0C231E", "TEXT": "#efbe1c", "INPUT": "#153C33", "TEXT_INPUT": "#efbe1c", "SCROLL": "#153C33",
+                   "BUTTON": ("#efbe1c", "#153C33"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey7": {"BACKGROUND": "#4b586e", "TEXT": "#dddddd", "INPUT": "#574e6d", "TEXT_INPUT": "#dddddd", "SCROLL": "#574e6d",
+                  "BUTTON": ("#dddddd", "#43405d"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                  "COLOR_LIST": ["#43405d", "#4b586e", "#574e6d", "#dddddd"], "DESCRIPTION": ["Grey", "Winter", "Cold"], },
+    "DarkRed2": {"BACKGROUND": "#ab1212", "TEXT": "#f6e4b5", "INPUT": "#cd3131", "TEXT_INPUT": "#f6e4b5", "SCROLL": "#cd3131", "BUTTON": ("#f6e4b5", "#ab1212"),
+                 "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                 "COLOR_LIST": ["#ab1212", "#1fad9f", "#cd3131", "#f6e4b5"], "DESCRIPTION": ["Turquoise", "Red", "Yellow"], },
+    "LightGrey6": {"BACKGROUND": "#e3e3e3", "TEXT": "#233142", "INPUT": "#455d7a", "TEXT_INPUT": "#e3e3e3", "SCROLL": "#233142",
+                   "BUTTON": ("#e3e3e3", "#455d7a"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0,
+                   "COLOR_LIST": ["#233142", "#455d7a", "#f95959", "#e3e3e3"], "DESCRIPTION": ["#000000", "Blue", "Red", "Grey"], },
+    "HotDogStand": {"BACKGROUND": "red", "TEXT": "yellow", "INPUT": "yellow", "TEXT_INPUT": "#000000", "SCROLL": "yellow", "BUTTON": ("red", "yellow"),
+                    "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey8": {"BACKGROUND": "#19232D", "TEXT": "#ffffff", "INPUT": "#32414B", "TEXT_INPUT": "#ffffff", "SCROLL": "#505F69",
+                  "BUTTON": ("#ffffff", "#32414B"), "PROGRESS": ("#505F69", "#32414B"), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey9": {"BACKGROUND": "#36393F", "TEXT": "#DCDDDE", "INPUT": "#40444B", "TEXT_INPUT": "#ffffff", "SCROLL": "#202225",
+                  "BUTTON": ("#202225", "#B9BBBE"), "PROGRESS": ("#202225", "#40444B"), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey10": {"BACKGROUND": "#1c1e23", "TEXT": "#cccdcf", "INPUT": "#272a31", "TEXT_INPUT": "#8b9fde", "SCROLL": "#313641",
+                   "BUTTON": ("#f5f5f6", "#2e3d5a"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey11": {"BACKGROUND": "#1c1e23", "TEXT": "#cccdcf", "INPUT": "#313641", "TEXT_INPUT": "#cccdcf", "SCROLL": "#313641",
+                   "BUTTON": ("#f5f5f6", "#313641"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey12": {"BACKGROUND": "#1c1e23", "TEXT": "#8b9fde", "INPUT": "#313641", "TEXT_INPUT": "#8b9fde", "SCROLL": "#313641",
+                   "BUTTON": ("#cccdcf", "#2e3d5a"), "PROGRESS": DEFAULT_PROGRESS_BAR_COMPUTE, "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey13": {"BACKGROUND": "#1c1e23", "TEXT": "#cccdcf", "INPUT": "#272a31", "TEXT_INPUT": "#cccdcf", "SCROLL": "#313641",
+                   "BUTTON": ("#8b9fde", "#313641"), "PROGRESS": ("#cccdcf", "#272a31"), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey14": {"BACKGROUND": "#24292e", "TEXT": "#fafbfc", "INPUT": "#1d2125", "TEXT_INPUT": "#fafbfc", "SCROLL": "#1d2125",
+                   "BUTTON": ("#fafbfc", "#155398"), "PROGRESS": ("#155398", "#1d2125"), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "DarkGrey15": {'BACKGROUND': '#121212', 'TEXT': '#dddddd', 'INPUT': '#1e1e1e', 'TEXT_INPUT': '#69b1ef', 'SCROLL': '#272727',
                   'BUTTON': ('#69b1ef', '#2e2e2e'), 'PROGRESS': ('#69b1ef', '#2e2e2e'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,},
-    'DarkGrey16':     {'BACKGROUND': '#353535', 'TEXT': '#ffffff', 'INPUT': '#191919', 'TEXT_INPUT': '#ffffff', 'SCROLL': '#454545',
+    "DarkGrey16":     {'BACKGROUND': '#353535', 'TEXT': '#ffffff', 'INPUT': '#191919', 'TEXT_INPUT': '#ffffff', 'SCROLL': '#454545',
                        'BUTTON': ('#ffffff', '#454545'), 'PROGRESS': ('#757575', '#454545'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0,},
-    'DarkBrown7': {'BACKGROUND': '#2c2417', 'TEXT': '#baa379', 'INPUT': '#baa379', 'TEXT_INPUT': '#000000', 'SCROLL': '#392e1c',
-                   'BUTTON': ('#000000', '#baa379'), 'PROGRESS': ('#baa379', '#453923'), 'BORDER': 1, 'SLIDER_DEPTH': 1, 'PROGRESS_DEPTH': 0, },
-    'Python': {'BACKGROUND': '#3d7aab', 'TEXT': '#ffde56', 'INPUT': '#295273', 'TEXT_INPUT': '#ffde56', 'SCROLL': '#295273',
-               'BUTTON': ('#ffde56', '#295273'), 'PROGRESS': ('#ffde56', '#295273'), 'BORDER': 1, 'SLIDER_DEPTH': 1, 'PROGRESS_DEPTH': 0, },
-    'PythonPlus': {'BACKGROUND': '#001d3c', 'TEXT': '#ffffff', 'INPUT': '#015bbb', 'TEXT_INPUT': '#fed500', 'SCROLL': '#015bbb',
-                   'BUTTON': ('#fed500', '#015bbb'), 'PROGRESS': ('#015bbb', '#fed500'), 'BORDER': 1, 'SLIDER_DEPTH': 1, 'PROGRESS_DEPTH': 0, },
-    'NeonBlue1': {'BACKGROUND': '#000000', 'TEXT': '#ffffff', 'INPUT': '#000000', 'TEXT_INPUT': '#33ccff', 'SCROLL': '#33ccff',
-                  'BUTTON': ('#33ccff', '#000000'), 'PROGRESS': ('#33ccff', '#ffffff'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'NeonGreen1': {'BACKGROUND': '#000000', 'TEXT': '#ffffff', 'INPUT': '#000000', 'TEXT_INPUT': '#96ff7b', 'SCROLL': '#96ff7b',
-                   'BUTTON': ('#96ff7b', '#000000'), 'PROGRESS': ('#96ff7b', '#ffffff'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
-    'NeonYellow1': {'BACKGROUND': '#000000', 'TEXT': '#ffffff', 'INPUT': '#000000', 'TEXT_INPUT': '#ffcf40', 'SCROLL': '#ffcf40',
-                    'BUTTON': ('#ffcf40', '#000000'), 'PROGRESS': ('#ffcf40', '#ffffff'), 'BORDER': 1, 'SLIDER_DEPTH': 0, 'PROGRESS_DEPTH': 0, },
+    "DarkBrown7": {"BACKGROUND": "#2c2417", "TEXT": "#baa379", "INPUT": "#baa379", "TEXT_INPUT": "#000000", "SCROLL": "#392e1c",
+                   "BUTTON": ("#000000", "#baa379"), "PROGRESS": ("#baa379", "#453923"), "BORDER": 1, "SLIDER_DEPTH": 1, "PROGRESS_DEPTH": 0, },
+    "Python": {"BACKGROUND": "#3d7aab", "TEXT": "#ffde56", "INPUT": "#295273", "TEXT_INPUT": "#ffde56", "SCROLL": "#295273",
+               "BUTTON": ("#ffde56", "#295273"), "PROGRESS": ("#ffde56", "#295273"), "BORDER": 1, "SLIDER_DEPTH": 1, "PROGRESS_DEPTH": 0, },
+    "PythonPlus": {"BACKGROUND": "#001d3c", "TEXT": "#ffffff", "INPUT": "#015bbb", "TEXT_INPUT": "#fed500", "SCROLL": "#015bbb",
+                   "BUTTON": ("#fed500", "#015bbb"), "PROGRESS": ("#015bbb", "#fed500"), "BORDER": 1, "SLIDER_DEPTH": 1, "PROGRESS_DEPTH": 0, },
+    "NeonBlue1": {"BACKGROUND": "#000000", "TEXT": "#ffffff", "INPUT": "#000000", "TEXT_INPUT": "#33ccff", "SCROLL": "#33ccff",
+                  "BUTTON": ("#33ccff", "#000000"), "PROGRESS": ("#33ccff", "#ffffff"), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "NeonGreen1": {"BACKGROUND": "#000000", "TEXT": "#ffffff", "INPUT": "#000000", "TEXT_INPUT": "#96ff7b", "SCROLL": "#96ff7b",
+                   "BUTTON": ("#96ff7b", "#000000"), "PROGRESS": ("#96ff7b", "#ffffff"), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
+    "NeonYellow1": {"BACKGROUND": "#000000", "TEXT": "#ffffff", "INPUT": "#000000", "TEXT_INPUT": "#ffcf40", "SCROLL": "#ffcf40",
+                    "BUTTON": ("#ffcf40", "#000000"), "PROGRESS": ("#ffcf40", "#ffffff"), "BORDER": 1, "SLIDER_DEPTH": 0, "PROGRESS_DEPTH": 0, },
 }
 
 
 
 def list_of_look_and_feel_values():
     """
     Get a list of the valid values to pass into your call to change_look_and_feel
@@ -19947,15 +19947,15 @@
     def sample_layout():
         return [[Text('Text element'), InputText('Input data here', size=(10, 1))],
                 [Button('Ok'), Button('Disabled', disabled=True), Slider((1, 10), orientation='h', size=(5, 15))]]
 
     names = list_of_look_and_feel_values()
     names.sort()
     if search_string not in (None, ''):
-        names = [name for name in names if search_string.lower().replace(' ', '') in name.lower().replace(' ', '')]
+        names = [name for name in names if search_string.lower().replace(" ", "") in name.lower().replace(" ", "")]
 
     if search_string not in (None, ''):
         layout = [[Text('Themes containing "{}"'.format(search_string), font='Default 18', background_color=win_bg)]]
     else:
         layout = [[Text('List of all themes', font='Default 18', background_color=win_bg)]]
 
     col_layout = []
@@ -20250,15 +20250,15 @@
 # ..##.......##.....##.##..####.##..........##.....##..##.....##.##..####.......##
 # ..##.......##.....##.##...###.##....##....##.....##..##.....##.##...###.##....##
 # ..##........#######..##....##..######.....##....####..#######..##....##..######.
 
 def clipboard_set(new_value):
     """
     Sets the clipboard to a specific value.
-    importANT NOTE - Your FreeSimpleGUI application needs to remain running until you've pasted
+    IMPORTANT NOTE - Your PySimpleGUI application needs to remain running until you've pasted
     your clipboard. This is a tkinter limitation.  A workaround was found for Windows, but you still
     need to stay running for Linux systems.
 
     :param new_value: value to set the clipboard to. Will be converted to a string
     :type new_value:  (str | bytes)
     """
     root = _get_hidden_master_root()
@@ -21528,15 +21528,15 @@
         layout = [[]]
 
     layout += [[Text(message, auto_size_text=True, text_color=text_color, background_color=background_color)]]
 
     if not history:
         layout += [[InputText(default_text=default_path, size=size, key='-INPUT-'), browse_button]]
     else:
-        file_list = history_settings.get('-PSG file list-', [])
+        file_list = history_settings.get("-PSG file list-", [])
         last_entry = file_list[0] if file_list else ''
         layout += [[Combo(file_list, default_value=last_entry, key='-INPUT-', size=size if size != (None, None) else (80, 1), bind_return_key=True),
                     browse_button, Button('Clear History', tooltip='Clears the list of files shown in the combobox')]]
 
     layout += [[Button('Ok', size=(6, 1), bind_return_key=True), Button('Cancel', size=(6, 1))]]
 
     window = Window(title=title or message, layout=layout, icon=icon, auto_size_text=True, button_color=button_color,
@@ -21647,15 +21647,15 @@
     else:
         layout = [[]]
 
     layout += [[Text(message, auto_size_text=True, text_color=text_color, background_color=background_color)]]
     if not history:
         layout += [[InputText(default_text=default_text, size=size, key='-INPUT-', password_char=password_char)]]
     else:
-        text_list = history_settings.get('-PSG text list-', [])
+        text_list = history_settings.get("-PSG text list-", [])
         last_entry = text_list[0] if text_list else default_text
         layout += [[Combo(text_list, default_value=last_entry, key='-INPUT-', size=size if size != (None, None) else (80, 1), bind_return_key=True),
                     Button('Clear History', tooltip='Clears the list of files shown in the combobox')]]
 
     layout += [[Button('Ok', size=(6, 1), bind_return_key=True), Button('Cancel', size=(6, 1))]]
 
     window = Window(title=title or message, layout=layout, icon=icon, auto_size_text=True, button_color=button_color, no_titlebar=no_titlebar,
@@ -21842,15 +21842,15 @@
                 cur_month = 12
                 cur_year -= 1
             window['-MON-YEAR-'].update('{} {}'.format(mon_names[cur_month - 1], cur_year))
             update_days(window, cur_month, cur_year, begin_at_sunday_plus)
             if prev_choice:
                 window[prev_choice].update(background_color=theme_background_color(), text_color=theme_text_color())
         elif type(event) is tuple:
-            if window[event].DisplayText != '':
+            if window[event].DisplayText != "":
                 chosen_mon_day_year = cur_month, int(window[event].DisplayText), cur_year
                 if prev_choice:
                     window[prev_choice].update(background_color=theme_background_color(), text_color=theme_text_color())
                 window[event].update(background_color=theme_text_color(), text_color=theme_background_color())
                 prev_choice = event
                 if close_when_chosen:
                     break
@@ -22057,15 +22057,15 @@
     if SUPPRESS_ERROR_POPUPS:
         return
     trace_details = traceback.format_stack()
     error_message = ''
     file_info_pysimplegui = None
     for line in reversed(trace_details):
         if __file__ not in line:
-            file_info_pysimplegui = line.split(',')[0]
+            file_info_pysimplegui = line.split(",")[0]
             error_message = line
             break
     if file_info_pysimplegui is None:
         _error_popup_with_code(title, None, None,  'Did not find your traceback info', *args,emoji=emoji)
         return
 
     error_parts = None
@@ -22246,17 +22246,17 @@
     :return: Error string to display with file, line number, and line of code
     :rtype:  str
     """
 
     called_func = inspect.stack()[1].function
     trace_details = traceback.format_stack()
     error_message = ''
-    file_info_pysimplegui = trace_details[-1].split(',')[0]
+    file_info_pysimplegui = trace_details[-1].split(",")[0]
     for line in reversed(trace_details):
-        if line.split(',')[0] != file_info_pysimplegui:
+        if line.split(",")[0] != file_info_pysimplegui:
             error_message = line
             break
     if error_message != '':
         error_parts = error_message.split(', ')
         if len(error_parts) < 4:
             error_message = error_parts[0] + '\n' + error_parts[1] + '\n' + ''.join(error_parts[2:])
     return 'The PySimpleGUI internal reporting function is ' + called_func + '\n' + \
@@ -22505,17 +22505,17 @@
             if dirname_from_filename:
                 path = dirname_from_filename
                 filename = os.path.basename(filename)
         elif self.filename is not None:
             filename = self.filename
         else:
             if not self.use_config_file:
-                filename = os.path.splitext(os.path.basename(sys.modules['__main__'].__file__))[0] + '.json'
+                filename = os.path.splitext(os.path.basename(sys.modules["__main__"].__file__))[0] + '.json'
             else:
-                filename = os.path.splitext(os.path.basename(sys.modules['__main__'].__file__))[0] + '.ini'
+                filename = os.path.splitext(os.path.basename(sys.modules["__main__"].__file__))[0] + '.ini'
 
         if path is None:
             if self.path is not None:
                 # path = self.path
                 path = os.path.expanduser(self.path)  # expand user provided path in case it has user ~ in it. Don't think it'll hurt
             elif DEFAULT_USER_SETTINGS_PATH is not None:  # if user set the path manually system-wide using set options
                 path = os.path.expanduser(DEFAULT_USER_SETTINGS_PATH)
@@ -23071,22 +23071,22 @@
  ##.....::. ##::'##:: ##.....::'##... ##: ##:::: ##:... ##..:: ##.....::
  ##::::::::. ##'##::: ##::::::: ##:::..:: ##:::: ##:::: ##:::: ##:::::::
  ######:::::. ###:::: ######::: ##::::::: ##:::: ##:::: ##:::: ######:::
  ##...:::::: ## ##::: ##...:::: ##::::::: ##:::: ##:::: ##:::: ##...::::
  ##:::::::: ##:. ##:: ##::::::: ##::: ##: ##:::: ##:::: ##:::: ##:::::::
  ########: ##:::. ##: ########:. ######::. #######::::: ##:::: ########:
 ........::..:::::..::........:::......::::.......::::::..:::::........::
-:::'###::::'########::'####::'######::
-::'## ##::: ##.... ##:. ##::'##... ##:
-:'##:. ##:: ##:::: ##:: ##:: ##:::..::
-'##:::. ##: ########::: ##::. ######::
- #########: ##.....:::: ##:::..... ##:
- ##.... ##: ##::::::::: ##::'##::: ##:
- ##:::: ##: ##::::::::'####:. ######::
-..:::::..::..:::::::::....:::......:::
+:::'###::::'########::'####::'######::                                  
+::'## ##::: ##.... ##:. ##::'##... ##:                                  
+:'##:. ##:: ##:::: ##:: ##:: ##:::..::                                  
+'##:::. ##: ########::: ##::. ######::                                  
+ #########: ##.....:::: ##:::..... ##:                                  
+ ##.... ##: ##::::::::: ##::'##::: ##:                                  
+ ##:::: ##: ##::::::::'####:. ######::                                  
+..:::::..::..:::::::::....:::......:::        
 
 
 
 These are the functions used to implement the subprocess APIs (Exec APIs) of PySimpleGUI
 
 '''
 
@@ -23133,17 +23133,17 @@
             else:
                 sp = subprocess.Popen(command + ' ' + expanded_args, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, cwd=cwd, stdin=stdin)
         else:
             sp = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=cwd, stdin=stdin)
         if wait:
             out, err = sp.communicate()
             if out:
-                print(out.decode('utf-8'))
+                print(out.decode("utf-8"))
             if err:
-                print(err.decode('utf-8'))
+                print(err.decode("utf-8"))
     except Exception as e:
         warnings.warn('Error in execute_command_subprocess {}'.format(e), UserWarning)
         _error_popup_with_traceback('Error in execute_command_subprocess', e, 'command={}'.format(command), 'args={}'.format(args), 'cwd={}'.format(cwd))
         sp = None
     return sp
 
 
@@ -23271,17 +23271,17 @@
     """
 
     out_decoded = err_decoded = None
     if subprocess_id is not None:
         try:
             out, err = subprocess_id.communicate(timeout=timeout)
             if out:
-                out_decoded = out.decode('utf-8')
+                out_decoded = out.decode("utf-8")
             if err:
-                err_decoded = err.decode('utf-8')
+                err_decoded = err.decode("utf-8")
         except ValueError:
             # will get an error if stdout and stderr are combined and attempt to read stderr
             # so ignore the error that would be generated
             pass
         except subprocess.TimeoutExpired:
             # a Timeout error is not actually an error that needs to be reported
             pass
@@ -23334,15 +23334,15 @@
     :rtype:  str
     """
     try:  # lots can go wrong so wrapping the entire thing
         trace_details = traceback.format_stack()
         file_info_pysimplegui, error_message = None, ''
         for line in reversed(trace_details):
             if __file__ not in line:
-                file_info_pysimplegui = line.split(',')[0]
+                file_info_pysimplegui = line.split(",")[0]
                 error_message = line
                 break
         if file_info_pysimplegui is None:
             return ''
         error_parts = None
         if error_message != '':
             error_parts = error_message.split(', ')
@@ -23404,15 +23404,15 @@
  ##:::: ##: ##:::: ##:. ######:::::. ######:: ##:::::::: ########:. ######::'####: ##:::::::'####:. ######::
 ..:::::..::..:::::..:::......:::::::......:::..:::::::::........:::......:::....::..::::::::....:::......:::
 '''
 
 '''
 The Mac problems have been significant enough to warrant the addition of a series of settings that allow
 users to turn specific patches and features on or off depending on their setup.  There is not enough information
-available to make this process more atuomatic.
+available to make this process more atuomatic.  
 
 '''
 
 
 # Dictionary of Mac Patches.  Used to find the key in the global settings and the default value
 MAC_PATCH_DICT = {'Enable No Titlebar Patch' : ('-mac feature enable no titlebar patch-', False),
                   'Disable Modal Windows' : ('-mac feature disable modal windows-', True),
@@ -23531,23 +23531,23 @@
 '########::'########:'########::'##::::'##::'######::::'######:::'########:'########::
  ##.... ##: ##.....:: ##.... ##: ##:::: ##:'##... ##::'##... ##:: ##.....:: ##.... ##:
  ##:::: ##: ##::::::: ##:::: ##: ##:::: ##: ##:::..::: ##:::..::: ##::::::: ##:::: ##:
  ##:::: ##: ######::: ########:: ##:::: ##: ##::'####: ##::'####: ######::: ########::
  ##:::: ##: ##...:::: ##.... ##: ##:::: ##: ##::: ##:: ##::: ##:: ##...:::: ##.. ##:::
  ##:::: ##: ##::::::: ##:::: ##: ##:::: ##: ##::: ##:: ##::: ##:: ##::::::: ##::. ##::
  ########:: ########: ########::. #######::. ######:::. ######::: ########: ##:::. ##:
-........:::........::........::::.......::::......:::::......::::........::..:::::..::
+........:::........::........::::.......::::......:::::......::::........::..:::::..::                                                                    
 '''
 
 #####################################################################################################
 # Debugger
 #####################################################################################################
 
 
-red_x = b'R0lGODlhEAAQAPeQAIsAAI0AAI4AAI8AAJIAAJUAAJQCApkAAJoAAJ4AAJkJCaAAAKYAAKcAAKcCAKcDA6cGAKgAAKsAAKsCAKwAAK0AAK8AAK4CAK8DAqUJAKULAKwLALAAALEAALIAALMAALMDALQAALUAALYAALcEALoAALsAALsCALwAAL8AALkJAL4NAL8NAKoTAKwbAbEQALMVAL0QAL0RAKsREaodHbkQELMsALg2ALk3ALs+ALE2FbgpKbA1Nbc1Nb44N8AAAMIWAMsvAMUgDMcxAKVABb9NBbVJErFYEq1iMrtoMr5kP8BKAMFLAMxKANBBANFCANJFANFEB9JKAMFcANFZANZcANpfAMJUEMZVEc5hAM5pAMluBdRsANR8AM9YOrdERMpIQs1UVMR5WNt8X8VgYMdlZcxtYtx4YNF/btp9eraNf9qXXNCCZsyLeNSLd8SSecySf82kd9qqc9uBgdyBgd+EhN6JgtSIiNuJieGHhOGLg+GKhOKamty1ste4sNO+ueenp+inp+HHrebGrefKuOPTzejWzera1O7b1vLb2/bl4vTu7fbw7ffx7vnz8f///wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACH5BAEAAJAALAAAAAAQABAAAAjUACEJHEiwYEEABniQKfNFgQCDkATQwAMokEU+PQgUFDAjjR09e/LUmUNnh8aBCcCgUeRmzBkzie6EeQBAoAAMXuA8ciRGCaJHfXzUMCAQgYooWN48anTokR8dQk4sELggBhQrU9Q8evSHiJQgLCIIfMDCSZUjhbYuQkLFCRAMAiOQGGLE0CNBcZYmaRIDLqQFGF60eTRoSxc5jwjhACFWIAgMLtgUocJFy5orL0IQRHAiQgsbRZYswbEhBIiCCH6EiJAhAwQMKU5DjHCi9gnZEHMTDAgAOw=='
+red_x = b"R0lGODlhEAAQAPeQAIsAAI0AAI4AAI8AAJIAAJUAAJQCApkAAJoAAJ4AAJkJCaAAAKYAAKcAAKcCAKcDA6cGAKgAAKsAAKsCAKwAAK0AAK8AAK4CAK8DAqUJAKULAKwLALAAALEAALIAALMAALMDALQAALUAALYAALcEALoAALsAALsCALwAAL8AALkJAL4NAL8NAKoTAKwbAbEQALMVAL0QAL0RAKsREaodHbkQELMsALg2ALk3ALs+ALE2FbgpKbA1Nbc1Nb44N8AAAMIWAMsvAMUgDMcxAKVABb9NBbVJErFYEq1iMrtoMr5kP8BKAMFLAMxKANBBANFCANJFANFEB9JKAMFcANFZANZcANpfAMJUEMZVEc5hAM5pAMluBdRsANR8AM9YOrdERMpIQs1UVMR5WNt8X8VgYMdlZcxtYtx4YNF/btp9eraNf9qXXNCCZsyLeNSLd8SSecySf82kd9qqc9uBgdyBgd+EhN6JgtSIiNuJieGHhOGLg+GKhOKamty1ste4sNO+ueenp+inp+HHrebGrefKuOPTzejWzera1O7b1vLb2/bl4vTu7fbw7ffx7vnz8f///wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACH5BAEAAJAALAAAAAAQABAAAAjUACEJHEiwYEEABniQKfNFgQCDkATQwAMokEU+PQgUFDAjjR09e/LUmUNnh8aBCcCgUeRmzBkzie6EeQBAoAAMXuA8ciRGCaJHfXzUMCAQgYooWN48anTokR8dQk4sELggBhQrU9Q8evSHiJQgLCIIfMDCSZUjhbYuQkLFCRAMAiOQGGLE0CNBcZYmaRIDLqQFGF60eTRoSxc5jwjhACFWIAgMLtgUocJFy5orL0IQRHAiQgsbRZYswbEhBIiCCH6EiJAhAwQMKU5DjHCi9gnZEHMTDAgAOw=="
 
 
 
 
 class _Debugger:
     debugger = None
     DEBUGGER_MAIN_WINDOW_THEME = 'dark grey 13'
@@ -23630,15 +23630,15 @@
         ]
 
         # Tab based layout
         layout = [[Text('Debugging: ' + self._find_users_code())],
                   [TabGroup([[Tab('Variables', col1), Tab('REPL & Watches', col2)]])]]
 
         # ------------------------------- Create main window -------------------------------
-        window = Window('PySimpleGUI Debugger', layout, icon=PSG_DEBUGGER_LOGO, margins=(0, 0), location=location, keep_on_top=True, right_click_menu=[[''], ['Exit', ]])
+        window = Window("PySimpleGUI Debugger", layout, icon=PSG_DEBUGGER_LOGO, margins=(0, 0), location=location, keep_on_top=True, right_click_menu=[[''], ['Exit', ]])
 
         Window._read_call_from_debugger = True
         window.finalize()
         Window._read_call_from_debugger = False
 
         window.Element('_VAR1_').SetFocus()
         self.watcher_window = window
@@ -23667,15 +23667,15 @@
             self.watcher_window = None
             return False
         # ------------------------------- Process events from REPL Tab -------------------------------
         cmd = values['-REPL-']  # get the REPL entered
         # BUTTON - GO (NOTE - This button is invisible!!)
         if event == 'Go':  # GO BUTTON
             self.watcher_window.Element('-REPL-').Update('')
-            self.watcher_window.Element('-OUTPUT-').Update('>>> {}\n'.format(cmd), append=True, autoscroll=True)
+            self.watcher_window.Element('-OUTPUT-').Update(">>> {}\n".format(cmd), append=True, autoscroll=True)
 
             try:
                 result = eval('{}'.format(cmd), myglobals, mylocals)
             except Exception as e:
                 if sys.version_info[0] < 3:
                     result = 'Not available in Python 2'
                 else:
@@ -23783,15 +23783,15 @@
 
     def _find_users_code(self):
         try:  # lots can go wrong so wrapping the entire thing
             trace_details = traceback.format_stack()
             file_info_pysimplegui, error_message = None, ''
             for line in reversed(trace_details):
                 if __file__ not in line:
-                    file_info_pysimplegui = line.split(',')[0]
+                    file_info_pysimplegui = line.split(",")[0]
                     error_message = line
                     break
             if file_info_pysimplegui is None:
                 return ''
             error_parts = None
             if error_message != '':
                 error_parts = error_message.split(', ')
@@ -23809,15 +23809,15 @@
         ######                                 #     #
         #     #  ####  #####  #    # #####     #  #  # # #    # #####   ####  #    #
         #     # #    # #    # #    # #    #    #  #  # # ##   # #    # #    # #    #
         ######  #    # #    # #    # #    #    #  #  # # # #  # #    # #    # #    #
         #       #    # #####  #    # #####     #  #  # # #  # # #    # #    # # ## #
         #       #    # #      #    # #         #  #  # # #   ## #    # #    # ##  ##
         #        ####  #       ####  #          ## ##  # #    # #####   ####  #    #
-
+    
         ######                                    #                     #     #
         #     # #    # #    # #####   ####       # #   #      #         #     #   ##   #####   ####
         #     # #    # ##  ## #    # #          #   #  #      #         #     #  #  #  #    # #
         #     # #    # # ## # #    #  ####     #     # #      #         #     # #    # #    #  ####
         #     # #    # #    # #####       #    ####### #      #          #   #  ###### #####       #
         #     # #    # #    # #      #    #    #     # #      #           # #   #    # #   #  #    #
         ######   ####  #    # #       ####     #     # ###### ######       #    #    # #    #  ####
@@ -23855,15 +23855,15 @@
         #####                                        #     #
        #     # #    #  ####   ####   ####  ######    #  #  #   ##   #####  ####  #    #
        #       #    # #    # #    # #      #         #  #  #  #  #    #   #    # #    #
        #       ###### #    # #    #  ####  #####     #  #  # #    #   #   #      ######
        #       #    # #    # #    #      # #         #  #  # ######   #   #      #    #
        #     # #    # #    # #    # #    # #         #  #  # #    #   #   #    # #    #
         #####  #    #  ####   ####   ####  ######     ## ##  #    #   #    ####  #    #
-
+    
         #     #                                                       #     #
         #     #   ##   #####  #   ##   #####  #      ######  ####     #  #  # # #    #
         #     #  #  #  #    # #  #  #  #    # #      #      #         #  #  # # ##   #
         #     # #    # #    # # #    # #####  #      #####   ####     #  #  # # # #  #
          #   #  ###### #####  # ###### #    # #      #           #    #  #  # # #  # #
           # #   #    # #   #  # #    # #    # #      #      #    #    #  #  # # #   ##
            #    #    # #    # # #    # #####  ###### ######  ####      ## ##  # #    #
@@ -23930,15 +23930,15 @@
         ######                            #######
         #     # #    # # #      #####     #       #       ####    ##   ##### # #    #  ####
         #     # #    # # #      #    #    #       #      #    #  #  #    #   # ##   # #    #
         ######  #    # # #      #    #    #####   #      #    # #    #   #   # # #  # #
         #     # #    # # #      #    #    #       #      #    # ######   #   # #  # # #  ###
         #     # #    # # #      #    #    #       #      #    # #    #   #   # #   ## #    #
         ######   ####  # ###### #####     #       ######  ####  #    #   #   # #    #  ####
-
+    
         #     #
         #  #  # # #    # #####   ####  #    #
         #  #  # # ##   # #    # #    # #    #
         #  #  # # # #  # #    # #    # #    #
         #  #  # # #  # # #    # #    # # ## #
         #  #  # # #   ## #    # #    # ##  ##
          ## ##  # #    # #####   ####  #    #
@@ -24003,23 +24003,23 @@
         ######
         #     # ###### ###### #####  ######  ####  #    #
         #     # #      #      #    # #      #      #    #
         ######  #####  #####  #    # #####   ####  ######
         #   #   #      #      #####  #           # #    #
         #    #  #      #      #   #  #      #    # #    #
         #     # ###### #      #    # ######  ####  #    #
-
+    
         #######
         #       #       ####    ##   ##### # #    #  ####
         #       #      #    #  #  #    #   # ##   # #    #
         #####   #      #    # #    #   #   # # #  # #
         #       #      #    # ######   #   # #  # # #  ###
         #       #      #    # #    #   #   # #   ## #    #
         #       ######  ####  #    #   #   # #    #  ####
-
+    
         #     #
         #  #  # # #    # #####   ####  #    #
         #  #  # # ##   # #    # #    # #    #
         #  #  # # # #  # #    # #    # #    #
         #  #  # # #  # # #    # #    # # ## #
         #  #  # # #   ## #    # #    # ##  ##
          ## ##  # #    # #####   ####  #    #
@@ -24177,36 +24177,36 @@
     elif running_windows():
         platform_name, platform_ver = 'Windows', platform.win32_ver()
     elif running_linux():
         platform_name, platform_ver = 'Linux', platform.libc_ver()
     else:
         platform_name, platform_ver = 'Unknown platorm', 'Unknown platform version'
 
-    versions = 'Python Interpeter: {}\nPython version: {}.{}.{}\nPlatform: {}\nPlatform version: {}\nPort: {}\ntkinter version: {}\nPySimpleGUI version: {}\nPySimpleGUI filename: {}'.format(sys.executable, sys.version_info.major,
+    versions = "Python Interpeter: {}\nPython version: {}.{}.{}\nPlatform: {}\nPlatform version: {}\nPort: {}\ntkinter version: {}\nPySimpleGUI version: {}\nPySimpleGUI filename: {}".format(sys.executable, sys.version_info.major,
                                                                                                                                    sys.version_info.minor,
                                                                                                                                    sys.version_info.micro,
                                                                                                                                     platform_name, platform_ver,
                                                                                                                                    port,
                                                                                                                                    tclversion_detailed,
                                                                                                                                    ver,
                                                                                                                                    __file__)
     return versions
 
 
 def scheck_hh():
-    with open(__file__, 'r',encoding='utf8') as file:
+    with open(__file__, "r",encoding="utf8") as file:
         lines_in_file = file.readlines()
     combined_lines = ''.join(lines_in_file[:-1])
     entire_file_bytes = bytearray(combined_lines, encoding='utf8')
     cfileh = hh(entire_file_bytes)
     return cfileh.hexdigest()
 
 
 def read_last_line():
-    with open(__file__, 'r',encoding='utf8') as file:
+    with open(__file__, "r",encoding="utf8") as file:
         last_line = file.readlines()[-1]
     return last_line
 
 # ==================================================#
 #
 # MM""""""""`M                     oo oo
 # MM  mmmmmmmM
@@ -24377,37 +24377,37 @@
 def _random_happy_emoji():
     c = random.choice(EMOJI_BASE64_HAPPY_LIST)
     return c
 
 
 
 '''
-M"""""`'"""`YM
-M  mm.  mm.  M
-M  MMM  MMM  M .d8888b. 88d888b. .d8888b.
-M  MMM  MMM  M 88'  `88 88'  `88 88ooood8
-M  MMM  MMM  M 88.  .88 88       88.  ...
-M  MMM  MMM  M `88888P' dP       `88888P'
-MMMMMMMMMMMMMM
-
-M#"""""""'M                             .d8888P dP   dP
-##  mmmm. `M                            88'     88   88
-#'        .M .d8888b. .d8888b. .d8888b. 88baaa. 88aaa88
-M#  MMMb.'YM 88'  `88 Y8ooooo. 88ooood8 88` `88      88
-M#  MMMM'  M 88.  .88       88 88.  ... 8b. .d8      88
-M#       .;M `88888P8 `88888P' `88888P' `Y888P'      dP
-M#########M
-
-M""M
-M  M
-M  M 88d8b.d8b. .d8888b. .d8888b. .d8888b. .d8888b.
-M  M 88'`88'`88 88'  `88 88'  `88 88ooood8 Y8ooooo.
-M  M 88  88  88 88.  .88 88.  .88 88.  ...       88
-M  M dP  dP  dP `88888P8 `8888P88 `88888P' `88888P'
-MMMM                          .88
+M"""""`'"""`YM                            
+M  mm.  mm.  M                            
+M  MMM  MMM  M .d8888b. 88d888b. .d8888b. 
+M  MMM  MMM  M 88'  `88 88'  `88 88ooood8 
+M  MMM  MMM  M 88.  .88 88       88.  ... 
+M  MMM  MMM  M `88888P' dP       `88888P' 
+MMMMMMMMMMMMMM                            
+                                          
+M#"""""""'M                             .d8888P dP   dP 
+##  mmmm. `M                            88'     88   88 
+#'        .M .d8888b. .d8888b. .d8888b. 88baaa. 88aaa88 
+M#  MMMb.'YM 88'  `88 Y8ooooo. 88ooood8 88` `88      88 
+M#  MMMM'  M 88.  .88       88 88.  ... 8b. .d8      88 
+M#       .;M `88888P8 `88888P' `88888P' `Y888P'      dP 
+M#########M                                             
+                                                        
+M""M                                                
+M  M                                                
+M  M 88d8b.d8b. .d8888b. .d8888b. .d8888b. .d8888b. 
+M  M 88'`88'`88 88'  `88 88'  `88 88ooood8 Y8ooooo. 
+M  M 88  88  88 88.  .88 88.  .88 88.  ...       88 
+M  M dP  dP  dP `88888P8 `8888P88 `88888P' `88888P' 
+MMMM                          .88                   
                           d8888P
 '''
 
 
 
 '''
 
@@ -24429,28 +24429,28 @@
 RED_X_BASE64 = b'iVBORw0KGgoAAAANSUhEUgAAAFoAAABaCAYAAAA4qEECAAAQ5ElEQVR4nO1ca3SV1Zl+3nefSwJ4IQaMXBJU1HIZqwSt1ULAG/VSuXm0hVTrtMvOz+n8mBln1pqU+TNrOqur7ZrlrMrMWJ22dGoUQscbFKtAaylNtK0IbRHIDYlKQTEhOef79vvMj5yPppRLzvlOElzrPGt9a0GSs/ezn+/93r33s9/zAWWUUUYZZZRRRhlllFFGGWWUUXIQEDY16VjzKBRsalICMtY8hoWhAn9UiJ8cGCMRJCMiwtHGz1yaloqa/QNom9vcnCMgAnAk+oqLiNuuTCZ1WQXqRXOHKp/c2F7qfkpy56KoZSZT2bdq5dfP08pWgb14eQXbjjeuvFEAnouphE1NKgCPN6688fIKtgnsxSTTbX2rVn6dmUwl8MexxUXsRqKI4OpPnz8g4x6tSCQbA/MQCARAYP4InNxX+eQzL51LkR1x6X9w5S3wfCqprooASCLpHLI+/K80j/21fO/HfaXgHSvKCKgAPLx69flZGfdohXON/UFgoTcG3jPnPR2kCgGf/rBx+c0C8FzI2ZFwHzYuvxkBn3aQqpz3DLxnaMb+ILC0ui9led43DjU2jheATTG1KnrQEdnDqz99/nirfLQimWjsCwJTET3p76iAGPiBQZeft279y3EIlwofrlqxWGEbFHKBAZSTtDDSxqeS2h8EayuPhV+RZ589HieyixL6jyKvPr/Seh8dl0g09gbhn4k85O+pgJD4QB2XVX5/4ytjkUZOpIvVSxeZlxYRnFLkCGZmE9Ip7c/ZY5W9ub+JI3ZRj4MAPLp06YUVYe9/jHOusS8IvAIKEqe6hBRPUgQXmOeGD1fds3i0J8ho4ju66p7F9Fgvggs8SSHldLxVRPtyOV+ZkC/3TtBvvJPJTBitiBYCQCYzvg8D3x6fTK7u86EHxA3nwySpIgLgSC7EyonPbHyFmYyT5mZfKPFCEPVxLHN3g1O3HkCVkZRBLsNpwY9PJF1vGH57QsX7X8GTW7OFCl5QRDU15ScRDKypcInVfWHgYXAwYjiXEOLNKGRVSm3dkfvvWiDNzb714YeThfAoBK0PP5yU5mZ/7HN3f8pBfiBk1SAHyHB5w+COB0E4TuSvjvWe/4/5Sb0g7YYd0WxqUqxZw6Mr7qxNiLyRcm5c4M0Vk+YJMqUqAe3tQLCqqvnZrXz44aSsXRsU3NiZ+sm3eWTFPQtTjusSkKk5MwqGG8l/yjrp1Oe8HQ8Sbk7V/27sBggRGVZkF3pXqE6qYUIahYPzHAq/IDnvLQmZkvTy/aMr7lwsa9cGzGRShfA5E5jJpGTt2uDoijsXJ4XrEsTUnPeWH0bBnAmQRgFB5cAkERBf/eqwb1hBd5ZNTYrdu9PHwt5XK5y7ZsCbSbz1pU+puiyt27x+YeLGZ19iJpOS5uZcjDYRtXF06d23qLMn0qLTcmYewLDmklO2CViFU816e/288/tuxIxFOVmzxob7+cKEzi9tepcvmedN1yed1g0+irE2IT6t6gJjt1C+PGHjc8/HSSPRZ3uX3nUnhY8lVaZl44vMlKqExnYvfuXEDZteK3SZV7BAUQfv3f3p69IOzU60LmB8sSucc/2hf9fAv6z60abnWuvrk/Pb2goSO/rMkXuW3KWQxysTbvKA97FFToqKp3UY5d4Lf/RCazFr6YIf+2j9O+nZF39p4laG9J0JQIwkSRR5ueNh6FMqk5V4/INlt90xv60tYENDYtiCNDQk5re1BR8su+0OJR5PqUw+HoaepCuWl5FMABLSdw5oYsWFP3qhNVqPF6FbcWgCdA1g7y27vT7pZYMTTA/JWJFNwNKqmjX/nph+/sLnNm1iU5OeLRdGf/P+XUuWUO27aXWTshZv/iDAhIh4oitwXD6pZXNbNOZi2otl8ORNJTt695J5gLU41emhNxOJNUBLqWjg7bCAn7vwuZe2sAkqa049wOh37991y62E/CDptDpnjCcyYQmn6s26AF028dlNr0VjLbbNktmk799x63wKnkk4rQ28NzmN7zHMNi0pooHxiEDvnfj85pdPlRejnx2947abTdicUqkKGFdkWtI5Dbx1KrHywhe2FJWTT0ZJLMvobh++/ebr1aE56bQ25xk3sulExJsdEdqKqhdf2Tp0wCcm5SUNi1Tceud0oo+bukhLOac5bx30vK968092xo3kCCUxdQQwNjVp9eaf7LSE3p8NrSOtojD60xk2Z7uEFG9GB1QZdcO7dy5eOMQXFgE4+DO33gkm5rf2pzWIznoZfVpVs6HvYEI+W735JzvzE19skfMalQ6RefOHOxbdROJ7aXUzSrBRGPSziaMKv7Rq07btAHDkzgULzSdaVDDxTFbnMOHTqm7AfLsIGi964ZWfldrsKvlpBxsaErJ1a3hkycIFZvhupUvUDXjvKeKK7cwAOogQfNepu9szSND0ORVM9PkbURRXAEIOruF92KGKz1dt2rY9GkORdE+JETlWijYO79y24Hah/Gelam2W5onixSZJpyKePAgACplqBEViiAz6tKjrN+s0xZdqNm/7cTEbpeFgxM7vWF+flLa24Mitn2rwxHcqnLs06y1eZJN0eQ+5MD/5JG4YjOS0Uzfg/QEneKhqy0+3RpyLpHdGjOhBKTOzU9K8O/furTc0wBJPpFVnZM08ZHgHBaduND85xVjRgPRpVZc1OwANH5q8ZcfWiGvRbZ4FI3qUJM27c7sys1OTt+zYCtgDAyE7UqKORivKXeUJzlrs52m0lKgbCNlB5QOTt+zYumuERQZG6eg/eiTfWbDgRnW2zqnWBfktcqxdQAEQ5DdCqurNOszrqou3b391JNPFyf2PCqKZ/PCCBdeb881OtDZnVvSKoVBY3ur0tE71LlO9ffvOkVhdnA6jWswSrU0PLbjhelV52kGmBzF3c8PqF2BSRDzYZcZ7L9m+Y+doHAoPxajWw0lzs38qk3GXbN+x0weywhu7Xd5iLXpHd5bLSDpAvLHbB7Liku07dj41yiIDY1SeFdmNHTdeNz+l0uJEp8a1WE+FyOo0stuAZVN++otYVmccjFkdXGTWvL3wmusQJjc4kakeiHsGObR9c4Aa2E2Gy6e8+nprqQyiYjCmBYeRA/fugvp5YSgbVWRaKcQ+ITLZTXLp1B1tBZ/xlRrDPioaSRwPgBRgYMl1sBFftw0TY1Yc3pQv+e26ad4NSePzQtZ60kBqjLNHcHASVE+akLVJ4/NdN827oRSlt3EwJqkjeoy7r7v2k4C0OMFkH9/qPFU/HFzV4F0nWFqz87UdY5VCRl3oaELqvu7aT4LcoCIXj4TIQ/qLxH4HEiyf9stdPx+LSXFUHyVm4ASwg/Ufv0nM1qvg4rOVzsa9opJhFVws5ta313/8JgGMmeIPI4rBqAndWl+flGb4juvnLSDQLCI1oTeClLg5eRg5W0LvKSI1CaC54/p5C6QZvrW+fsSqWE/GqJpK++fPbUiZrnMiUwKzWCflRfEgLamqIfl2oLbqstZdI+pBD8WIC71r9uzU3N27c+3zZt+sXr6bVJ2SY7wT8jggYSkRDWkH4fD56W1vvhxxHMl+R1ToaADd1/zFrd7sibTq1Gzcuov8JBa3jbSI5mjdKvrQtF+9sWWkxR4xoSPiHR//2O2E++80dFqW8Utnoy8kkTTELBlOi7osrFvgv1j3699uHkmxR/RwtmvOnEVe7X/SqtOzxhJUdYqExoMAxCmmhCxFmYG4rFmnM31w+ptvvvKROZyNzPT2WbNuocN3UiLTcyyNyAG5Lwm3IlTvxNiiIrWlEDsl4nJkl3g8NGPPnpfO+XKDpwB3H+APzLlqMSnfS4tMiZuT8UeDqJNiSy/dvfdXAHBg1sxrAdfiRGr9YN6OnbOz5NsibLz0zd+9HI0lBu8/QcmEjnZb7bOuvMWAHyREJ8UuOAQsAagnO0Vs2aV73nqd+fYEsAOzZl5LaosTqQ3ju34+KeJytEOe9rkrf/vW1lLuIEtV5CgCsGvOVYtyoT2dVL0o7hEVAUsCGpAdDG3lzH372ob6FNG/37r88npJ6DNJkbogvtiWGKxi7QmV9121Z+/2UnkjsdeyEZH9H5vZkA3sGQUuylm8HZ+RliQ1MGsHJTNz3762yO2L+o3cuJn79rWBkgnM2pOEGmkxdpE6eGDMGufRsv9jMxtkcDMfOyBLEtH7Z12x0EK2uHwtXEkmJ7MDSdhna/ceOGPpbPS7/VfM+IRH4ocVKnWlmHwdIJ44qglZdtmevduKHk0ecfKnAMD+K2Ys9KG1CDgxHAyLON6FTwFuwPsDZlidF9mdKU8KYE8B7rK97b+AcdWA9wdSgCPpY3kjJAWc6ENr2X/FjIVDx1wMihI6eoz3Xl63yJu0KDkxjguXH6ClATcQ+v1qeOCKfft+/nIDEjKMmf8+wL/cgMQV+/a9ap4PDnh/ID0otjGu60dO9CYtv58xoyHO4UHBdyjKyXvr6haL02YILopdn0z6lKjL0vbTwoeuau/eFufrb7+fMa0Bmng8LXpZjvFq/YjoFRj8Q8Lz3ks7Oop6BUZB4kQd/L6u7gZR/J8TqQ544o0FRYGkT4u4LNkBJw9e+Vb71ji7sxNiz5zRAM8n0yJ1WdJLDLGNHCzAId8zymeuam//RaFiFyRQE6BfnDYt3Z/QnyVFrg1JQxyrk/SpQZG7neILM/d3vrQLSM0FYvkNURtvXVZ7izc8kRKZFpAxq1g5uPQjXksRNz3R0ZErpD5k2CJFhSc51dkgLydpKOhVDH960cwSgBswO6hOHiiVyAAwF8jtAlIz93e+pE4eCMwOJgBHMyuWLwgBaaDN7CdnrwGskHxdSEQrAb5WU1M7IZV4IylSGYBFlSuQg19v88TBQINVc9p7trUCyflASc2cqM3fzahZqJZcp4KpQQwvPAkJA2N/EPq5cw4d6srPS8OK6kI6NACo7+npEMq3EkRCPEMaUchlRiYIDb31GML7R0pkAJgPBK1A8qr2nm2e4WdDbz0JQs3IQnmLZ5gkEwQfm3voUOdXCxAZKG6lIAfq6tLHffBPE0Qf6S/gW1cEmADEgE4PuX/2wYM78uvkkX3VT76P3VOn3uDAHypQGxa2UvLjRFyv8d8tCP5h7nvv9WEkVx1D0VqP5PhDU9aMV32k18wr4M7UcySyJ7uCBFdc3dUzqrVwUV+/mV4zPxnKeicy/Wxi50PWj1d1/WbfGqf6SG13d38x/ReVqwjI/DYEfZdc0tQXhv8yXsQZT//lTZJ0g7ut7gBYfnVXT2vTKNdWSH7yurqrpzUAlnuyOzG4iz1tybCRfryIOx6G39Rx4/6utru7v9jdYRx3TfKGS+K3NTX/PE7kkd5T26L5qk50BcCKq3tGN5JPwXswsmtq5ieADQ6Ydio/m4BNENHj5DddT8/fXwlk4zh5Ra+Bow4FCPt6epqOkf86DlCSln93B400R6o36xwisoyVyHm+RkCu7ulpFWB5aNblyMj1Y567VQLaS36zJ51+5Eogi5h2aUls0vlAkJ4woamP/FYloI4UR0oqL3JO5L6re06ki9jeblxEnsWsnp7WQCTjzTpT5AnelYAeB/5t9tSpf7u4o2OAJ75rNMaI8lYnUPmb6uqv7amuPrxr0qT335g06bVdVVXXA4MbnrFl+eeIOL1ZVfWJN6qrX39j0qT391RXH/5NdfXXXgVK+lrjEcGvq6qm7brggmui/5/LZIdwkzerq6/9dVXVtDElNFxwSORycDd5zoocgYCczHss+QwbBORcTBVnQ9NHJDDKKKOMMsooo4wyyiijjDLK+Cji/wF6UgmmVAL7cgAAAABJRU5ErkJggg=='
 
 GREEN_CHECK_BASE64 = b'iVBORw0KGgoAAAANSUhEUgAAAFoAAABaCAYAAAA4qEECAAAJV0lEQVR4nO2cTWwc5RnHf8/M7Dq7ttdxIIIUcqGA1BQU6Ac9VSkp0NwoJE5PJJygKki9tIIEO7ND3ICEeqJUJYcqCYdKDoS0lWgpH21KuVShH/TjUolLkIpKguO1vWvvfDw9zOxH1l8zjnc3Xs/vFEXy7uzPz/7f93nnGUNKSkpKSkpKSkpKSkpKzyFMYDKC2e0L2TjYGN2+hN5DkXoVP1s4wdjgDwB4jEw3L6u30CguAJzCCV4YUp4bUuzC94BlZaclHx9hPwb78bELp8jJQaa1yrx65OQljhSe4DguLy8uOxUdhzAuDE5HkvvlEWbVRcgSYDKnHnn5CXbhSR5fXHYqemXCSj6Nj1M4Qb88wrR6EMkUpC47Jy8yFsm2sa58kZSlUYTTUVw4hRPkjIPMBC6ySDwoioHPJrEo65M8W3qJx8hwHBdS0UujTZVcLJwkLweY0cUlN35GEQJyYlLRJ3BKP2UEk9P4qejFWTyTibGFq1V2ViwqPMXRqRcYwUgzupXmha9YOJlIMoSZ7ROQEZBgJ6DsQNKKbmZBJsvBFeOilQCPQbGo6Ens0qNRdARpRddollwsnAwXPq0mkgwug2Ixq69glx7Fjr4ZoGlFhyzM5KSVrLgMSIZZfQWndKBWyYBCuo9erhlJIrnKgJGhrKdwSgeYwGSiIRnS7V1Dci2Tp9XDuLLZWJZaJdcyOTw6DZCGZNjIFR0eEDVJNsKFL4lkIsllPVVf+BaRDBu1olfTjCzEpX/pTG5lI1Z0Q7JdOEVeDqwik0PJtUweWZjJrWws0VfbjISv4TJghJlcLB2sL3yLxEUzGyc62tiMsEwl19gYFd2OZiRGXDSzESq67c1IHHq7ojvUjMShlyu6Y81IHHqzojvcjMSh9yq6C81IHHqtorvSjMShd0R3sRmJQ29ER5ebkTjEE21j8EWE/fhr8aZrTFhvgoaZbBxgJqgiZBO8xsJMXqNKblzkStgYOAQL/n2tUB9UKfy8W81IHJbPaBsLh4DRgS8wVvgWDkHrBE5Xscni4Bk69H2GjEeY1fluNCNxWLqid2FxDo9nCp8ny/v0yQ1U/L04M2d4mQyPhxM4XSOaAio4N391Wqbf0ECHUQzixuEaNiNxWLyi7Ujy6OBtZHkPU25gTj2yxgSjAw8vNlvWUWwsjuMOjt30tWlj5k019HoChPiL+5o2I3FYeGFhXHg8PXg7A/I2yHaq6gMGJoopwpz/MOMzZ5tnyzpGdH2FwzffM52f+Y1qsAUXH4n9iMOaNyNxuFJ0TfIPB29jSN5BZDvz6iFR9SoayTZw/YdwZs52NEai68uPfu7uSt/sO4oOJ5KsTZVcLB1sx+5iKRqiJzDZj8/TQ7eQ1z9iyk3M68IP0ZAtzLGP8akz0aJUbeuVRpKH7G1fKlmz7yoMJZdsZKgEHcnkVsKMtuuT7LeS1/eXlAy12TLBVyXHBIcH9uJQbeszHJHk3OEbvzJllkPJVYLYkgO8cOELGs3I/s5JBpDGE0XDOzD9NzBl+5KSm1ECTMACZoN9HJt5vS2ZXYuLseu/XO5z30T1uqvO5A7FRTMG1JoQ/2fkje1UtIoR40MIBj7gAXnjDKMD3+Y47ppWdiQ5Yw/dVelzf5tYsi6x8HVYMoSig7Cqze9SDi6QkyxBzFY7lB2OqW4yXmds6KHlHphJxGNkcPAyo1t3ehbvqOr1CSV3rBmJQ6Oldib/ic9ufP2EPjHR2LKlIZtXGRvYy+O49cfEVkO0T87bW+9ys/PnFN0SO5MVRZlnQLJUgsYpXAcXvsVIvutYilpmmyjzwXc4OnOmfmyZhFpcjA7d7fbxFnAdbszrCKfthYJAqfNbuOVodIb78bGxeH7qI6b1XlQvRJXtxXolwcADAkyxjBMjE3YmPIBPcObdLHkTb5JMsk8WEZVJqyRPUiwdBOhWJrdypQQHDxuLF6b/w4zeh+oFsmLFjhEDAx9fTcm99u8Xz47YI1mKaCzZtWZpdPhOt4+3UN2aSHIGUzAuDTK4xytefimKLqFLmdzK4mcD9Q89eBsZOYcl2xLFSEDAgBjGvPHruz++Ze8H2z4If1FLHbHWK3n4TjfrncOQYaoxF76G5MlBb2BPyfn4zx1poBKy8uldmNl/wkwoO9paSdX45b4P79t7esfpsLJaZdclb97pZv3fIxK/rQ4IyGJIwPRgMLS75Fw435Xzlxgs/ZU+F8XI81MfUeLrBPoxfSTZjWSYVVezwYOv3vm718SRULA2/XJr3xw7f5e7Sd9GjPiSw0w2BJnMycCuknPhfG23Euv6OkycOyxXnuaJbGdO/VhNTUhY2WX9lRZLD9ZFFzFx8Hgqv5NB6y2QrVQTZrLIpZybeaDsXPxL/TqvUeLeM2zIzsu7GHJTbCnQfGp2ln+V9rEDwcHjUP8d5M0/APE7vkgyyKWcl9tTcT45f61LhiR3weuyC7eS5z1MuXE1mY2rZxgt7cUevgPLfw9hc+yFL8pk4HK+2n9f+eh/P1gPkiHpuMHVNzUeebGoBOdAbiebYIGtVzKXM17fva7z6d/Wi2RYzVzHSjcHViIgICcGnoIbdXIr0ZTJltu323X+9+F6kgyrHaBZ7HbXfIJJzXDnIkiMRkbxyYiJcDE/n9lTPnpx3cRFM6ufVGptavpkG+UEMRKHmmT4LFPJ3O8eu/Z3F0txdSNhTU2N5PmFCvfgaxDd9r86wn2yic9UxjV2ueOX/75eJcNazN5F00uCYBS3OH7OO0I54XBhK7WFT+Qz5oxvMD75j/UsGdZqyDE8NDLEEc90ho94m3yHirooVuL3UHyyYgKfUuYBjk2tq93FUqztNKmNJQ6e6WwZ9Tb5R6moF8mOR9PCl5njAXd86q+9IBnaMbYbyRZ782iQ11B2gLXiO9UkazBJ1byXdZ7JrbRjPlqww3MMoyF7+RipLXyBTlK1dvVCJrfSvkH0aILJKBaeCXIyHi2QC2XXFz4uMufvZny25yRDOx+tiP6iYVAs/YiKHiYvGcLhhMYdj3omy6e43v29Khk68WhF7SD+SOEQ/XIsWiBNlCBqRi4xL9/stUxupf0PCx2PRnyfLT3HrH+YnFgoLhlMVC9T9nb3uuTOUptgOlI4xI+HlKOFixzqvwNoejwiZW2oCS0WnuBw4Z4r/i9ljWkePUj/ZHubsbFSySkpKSkpKSkpKSkpKSkpKW3g/3+PYisYNf7zAAAAAElFTkSuQmCC'
 
 
 
 '''
-M""MMMMM""M                                           dP
-M  MMMMM  M                                           88
-M  MMMMM  M 88d888b. .d8888b. 88d888b. .d8888b. .d888b88 .d8888b.
-M  MMMMM  M 88'  `88 88'  `88 88'  `88 88'  `88 88'  `88 88ooood8
-M  `MMM'  M 88.  .88 88.  .88 88       88.  .88 88.  .88 88.  ...
-Mb       dM 88Y888P' `8888P88 dP       `88888P8 `88888P8 `88888P'
-MMMMMMMMMMM 88            .88
-            dP        d8888P
-MP""""""`MM                            oo
-M  mmmmm..M
-M.      `YM .d8888b. 88d888b. dP   .dP dP .d8888b. .d8888b.
-MMMMMMM.  M 88ooood8 88'  `88 88   d8' 88 88'  `"" 88ooood8
-M. .MMM'  M 88.  ... 88       88 .88'  88 88.  ... 88.  ...
-Mb.     .dM `88888P' dP       8888P'   dP `88888P' `88888P'
+M""MMMMM""M                                           dP          
+M  MMMMM  M                                           88          
+M  MMMMM  M 88d888b. .d8888b. 88d888b. .d8888b. .d888b88 .d8888b. 
+M  MMMMM  M 88'  `88 88'  `88 88'  `88 88'  `88 88'  `88 88ooood8 
+M  `MMM'  M 88.  .88 88.  .88 88       88.  .88 88.  .88 88.  ... 
+Mb       dM 88Y888P' `8888P88 dP       `88888P8 `88888P8 `88888P' 
+MMMMMMMMMMM 88            .88                                     
+            dP        d8888P                                      
+MP""""""`MM                            oo                   
+M  mmmmm..M                                                 
+M.      `YM .d8888b. 88d888b. dP   .dP dP .d8888b. .d8888b. 
+MMMMMMM.  M 88ooood8 88'  `88 88   d8' 88 88'  `"" 88ooood8 
+M. .MMM'  M 88.  ... 88       88 .88'  88 88.  ... 88.  ... 
+Mb.     .dM `88888P' dP       8888P'   dP `88888P' `88888P' 
 MMMMMMMMMMM
 '''
 
 __upgrade_server_ip = ''
 __upgrade_server_port = ''
 
 
@@ -24729,15 +24729,15 @@
 """
 ## Type of Issue (Enhancement, Error, Bug, Question)
 
 {}
 
 ----------------------------------------
 
-## Environment
+## Environment 
 
 #### Operating System
 
 {}  version {}
 
 #### PySimpleGUI Port (tkinter, Qt, Wx, Web)
 
@@ -24827,20 +24827,20 @@
 ## How did you find PySimpleGUI?
 {}
 """.format(str(where_found))
     return body + body2
 
 
 def _github_issue_post_make_github_link(title, body):
-    pysimplegui_url = 'https://github.com/spyoungtech/FreeSimpleGui'
-    pysimplegui_issues = '{}/issues/new?'.format(pysimplegui_url)
+    pysimplegui_url = "https://github.com/spyoungtech/FreeSimpleGui"
+    pysimplegui_issues = "{}/issues/new?".format(pysimplegui_url)
 
     # Fix body cuz urllib can't do it smfh
     getVars = {'title': str(title), 'body': str(body)}
-    return (pysimplegui_issues + urllib.parse.urlencode(getVars).replace('%5Cn', '%0D'))
+    return (pysimplegui_issues + urllib.parse.urlencode(getVars).replace("%5Cn", "%0D"))
 
 
 #########################################################################################################
 
 def _github_issue_post_validate(values, checklist, issue_types):
     issue_type = None
     for itype in issue_types:
@@ -24876,15 +24876,15 @@
         popup_error("Title can't be blank", keep_on_top=True)
         return False
     elif title[1:len(title) - 1] == issue_type:
         popup_error("Title can't be blank (only the type of issue isn't enough)", keep_on_top=True)
         return False
 
     if len(values['-ML DETAILS-']) < 4:
-        popup_error('A little more details would be awesome', keep_on_top=True)
+        popup_error("A little more details would be awesome", keep_on_top=True)
         return False
 
     return True
 
 
 def _github_issue_help():
     heading_font = '_ 12 bold underline'
@@ -25148,41 +25148,41 @@
             else:
                 popup('Your markdown code is in the Markdown tab', keep_on_top=True)
 
     window.close()
 
 
 '''
-MM'"""""`MM oo   dP   M""MMMMM""MM          dP
-M' .mmm. `M      88   M  MMMMM  MM          88
-M  MMMMMMMM dP d8888P M         `M dP    dP 88d888b.
-M  MMM   `M 88   88   M  MMMMM  MM 88    88 88'  `88
-M. `MMM' .M 88   88   M  MMMMM  MM 88.  .88 88.  .88
-MM.     .MM dP   dP   M  MMMMM  MM `88888P' 88Y8888'
-MMMMMMMMMMM           MMMMMMMMMMMM
-
-M""MMMMM""M                                           dP
-M  MMMMM  M                                           88
-M  MMMMM  M 88d888b. .d8888b. 88d888b. .d8888b. .d888b88 .d8888b.
-M  MMMMM  M 88'  `88 88'  `88 88'  `88 88'  `88 88'  `88 88ooood8
-M  `MMM'  M 88.  .88 88.  .88 88       88.  .88 88.  .88 88.  ...
-Mb       dM 88Y888P' `8888P88 dP       `88888P8 `88888P8 `88888P'
-MMMMMMMMMMM 88            .88
+MM'"""""`MM oo   dP   M""MMMMM""MM          dP       
+M' .mmm. `M      88   M  MMMMM  MM          88       
+M  MMMMMMMM dP d8888P M         `M dP    dP 88d888b. 
+M  MMM   `M 88   88   M  MMMMM  MM 88    88 88'  `88 
+M. `MMM' .M 88   88   M  MMMMM  MM 88.  .88 88.  .88 
+MM.     .MM dP   dP   M  MMMMM  MM `88888P' 88Y8888' 
+MMMMMMMMMMM           MMMMMMMMMMMM                   
+                                                     
+M""MMMMM""M                                           dP          
+M  MMMMM  M                                           88          
+M  MMMMM  M 88d888b. .d8888b. 88d888b. .d8888b. .d888b88 .d8888b. 
+M  MMMMM  M 88'  `88 88'  `88 88'  `88 88'  `88 88'  `88 88ooood8 
+M  `MMM'  M 88.  .88 88.  .88 88       88.  .88 88.  .88 88.  ... 
+Mb       dM 88Y888P' `8888P88 dP       `88888P8 `88888P8 `88888P' 
+MMMMMMMMMMM 88            .88                                     
             dP        d8888P
 
 '''
 
 
 '''
-M""""""""M dP                                        dP
-Mmmm  mmmM 88                                        88
-MMMM  MMMM 88d888b. 88d888b. .d8888b. .d8888b. .d888b88
-MMMM  MMMM 88'  `88 88'  `88 88ooood8 88'  `88 88'  `88
-MMMM  MMMM 88    88 88       88.  ... 88.  .88 88.  .88
-MMMM  MMMM dP    dP dP       `88888P' `88888P8 `88888P8
+M""""""""M dP                                        dP 
+Mmmm  mmmM 88                                        88 
+MMMM  MMMM 88d888b. 88d888b. .d8888b. .d8888b. .d888b88 
+MMMM  MMMM 88'  `88 88'  `88 88ooood8 88'  `88 88'  `88 
+MMMM  MMMM 88    88 88       88.  ... 88.  .88 88.  .88 
+MMMM  MMMM dP    dP dP       `88888P' `88888P8 `88888P8 
 MMMMMMMMMM
 '''
 
 def _the_github_upgrade_thread(window, sp):
     """
     The thread that's used to run the subprocess so that the GUI can continue and the stdout/stderror is collected
 
@@ -25208,15 +25208,15 @@
 
 
 def _copy_files_from_github():
     """Update the local PySimpleGUI installation from Github"""
 
     github_url = 'https://raw.githubusercontent.com/spyoungtech/FreeSimpleGui/main/'
     #files = ["PySimpleGUI.py", "setup.py"]
-    files = ['PySimpleGUI.py']
+    files = ["PySimpleGUI.py"]
 
     # add a temp directory
     temp_dir = tempfile.TemporaryDirectory()
     psg_dir = os.path.join(temp_dir.name, 'PySimpleGUI')
     path = psg_dir
 
 
@@ -25231,40 +25231,40 @@
                 f.write(response.read())
                 downloaded.append(file)
 
     # get the new version number if possible
     with open(os.path.join(path, files[0]), encoding='utf-8') as f:
         text_data = f.read()
 
-    package_version = 'Unknown'
+    package_version = "Unknown"
     match = re.search(r'__version__ = \"([\d\.]+)', text_data)
     if match:
         package_version = match.group(1)
 
     # create a setup.py file from scratch
     setup_text = ''.join([
-            'import setuptools\n',
-            'setuptools.setup(',
+            "import setuptools\n",
+            "setuptools.setup(",
             "name='PySimpleGUI',",
             "author='PySimpleGUI',"
             "author_email='PySimpleGUI@PySimpleGUI.org',",
             "description='Unreleased Development Version',",
             "url='https://github.com/PySimpleGUI/PySimpleGUI',"
-            'packages=setuptools.find_packages(),',
+            "packages=setuptools.find_packages(),",
             "version='", package_version, "',",
-            'entry_points={',
+            "entry_points={",
             "'gui_scripts': [",
             "'psgissue=PySimpleGUI.PySimpleGUI:main_open_github_issue',",
             "'psgmain=PySimpleGUI.PySimpleGUI:_main_entry_point',",
             "'psgupgrade=PySimpleGUI.PySimpleGUI:_upgrade_entry_point',",
             "'psghelp=PySimpleGUI.PySimpleGUI:main_sdk_help',",
             "'psgver=PySimpleGUI.PySimpleGUI:main_get_debug_data',",
             "'psgsettings=PySimpleGUI.PySimpleGUI:main_global_pysimplegui_settings',",
-            '],',
-            '},)'
+            "],",
+            "},)"
             ])
 
     with open(os.path.join(temp_dir.name, 'setup.py'), 'w', encoding='utf-8') as f:
         f.write(setup_text)
 
     # create an __init__.py file
     with open(os.path.join(path, '__init__.py'), 'w', encoding='utf-8') as f:
@@ -25316,16 +25316,16 @@
 
     return package_version
 
 
 def _upgrade_from_github():
     mod_version = _copy_files_from_github()
 
-    popup('*** SUCCESS ***', 'PySimpleGUI.py installed version:', mod_version,
-          'For python located at:', os.path.dirname(sys.executable), keep_on_top=True, background_color='red',
+    popup("*** SUCCESS ***", "PySimpleGUI.py installed version:", mod_version,
+          "For python located at:", os.path.dirname(sys.executable), keep_on_top=True, background_color='red',
           text_color='white')
 
 
 def _upgrade_gui():
     try:
         cur_ver = version[:version.index('\n')]
     except:
@@ -25462,15 +25462,15 @@
 def _global_settings_get_watermark_info():
     if not pysimplegui_user_settings.get('-watermark-', False) and not Window._watermark_temp_forced:
         Window._watermark = None
         return
     forced =  Window._watermark_temp_forced
     prefix_text = pysimplegui_user_settings.get('-watermark text-', '')
 
-    ver_text = ' ' + version.split(' ', 1)[0] if pysimplegui_user_settings.get('-watermark ver-', False if not forced else True) or forced else ''
+    ver_text = ' ' + version.split(" ", 1)[0] if pysimplegui_user_settings.get('-watermark ver-', False if not forced else True) or forced else ''
     framework_ver_text = ' Tk ' + framework_version  if pysimplegui_user_settings.get('-watermark framework ver-', False if not forced else True) or forced else ''
     watermark_font = pysimplegui_user_settings.get('-watermark font-', '_ 9 bold')
     # background_color = pysimplegui_user_settings.get('-watermark bg color-', 'window.BackgroundColor')
     user_text = pysimplegui_user_settings.get('-watermark text-', '')
     python_text = ' Py {}.{}.{}'.format(sys.version_info.major, sys.version_info.minor, sys.version_info.micro)
     if user_text:
         text = str(user_text)
@@ -25485,15 +25485,15 @@
 
     settings = pysimplegui_user_settings.read()
 
     screenshot_keysym = ''
     for i in range(4):
         keysym = settings.get(json.dumps(('-snapshot keysym-', i)), '')
         if keysym:
-            screenshot_keysym += '<{}>'.format(keysym)
+            screenshot_keysym += "<{}>".format(keysym)
 
     screenshot_keysym_manual = settings.get('-snapshot keysym manual-', '')
 
     # print('BINDING INFO!', screenshot_keysym, screenshot_keysym_manual)
     if screenshot_keysym_manual:
         return screenshot_keysym_manual
     elif screenshot_keysym:
@@ -25668,15 +25668,15 @@
             # Snapshots portion
             screenshot_keysym_manual = values['-SNAPSHOT KEYSYM MANUAL-']
             pysimplegui_user_settings.set('-snapshot keysym manual-', values['-SNAPSHOT KEYSYM MANUAL-'])
             screenshot_keysym = ''
             for i in range(4):
                 pysimplegui_user_settings.set(json.dumps(('-snapshot keysym-',i)), values[('-SNAPSHOT KEYSYM-', i)])
                 if values[('-SNAPSHOT KEYSYM-', i)]:
-                    screenshot_keysym += '<{}>'.format(values[('-SNAPSHOT KEYSYM-', i)])
+                    screenshot_keysym += "<{}>".format(values[('-SNAPSHOT KEYSYM-', i)])
             if screenshot_keysym_manual:
                 DEFAULT_WINDOW_SNAPSHOT_KEY_CODE = screenshot_keysym_manual
             elif screenshot_keysym:
                 DEFAULT_WINDOW_SNAPSHOT_KEY_CODE = screenshot_keysym
 
             pysimplegui_user_settings.set('-screenshots folder-', values['-SCREENSHOTS FOLDER-'])
             pysimplegui_user_settings.set('-screenshots filename-', values['-SCREENSHOTS FILENAME-'])
@@ -25991,22 +25991,22 @@
                 ['!&Disabled', ['Popout', 'Launch Debugger']],
                 ['&Toolbar', ['Command &1', 'Command &2', 'Command &3', 'Command &4']],
                 ['&Help', '&About...'], ]
 
     button_menu_def = ['unused', ['&Paste', ['Special', 'Normal', '!Disabled'], 'Undo', 'Exit'], ]
     treedata = TreeData()
 
-    treedata.Insert('', '_A_', 'Tree Item 1', [1, 2, 3], )
-    treedata.Insert('', '_B_', 'B', [4, 5, 6], )
-    treedata.Insert('_A_', '_A1_', 'Sub Item 1', ['can', 'be', 'anything'], )
-    treedata.Insert('', '_C_', 'C', [], )
-    treedata.Insert('_C_', '_C1_', 'C1', ['or'], )
-    treedata.Insert('_A_', '_A2_', 'Sub Item 2', [None, None])
-    treedata.Insert('_A1_', '_A3_', 'A30', ['getting deep'])
-    treedata.Insert('_C_', '_C2_', 'C2', ['nothing', 'at', 'all'])
+    treedata.Insert("", '_A_', 'Tree Item 1', [1, 2, 3], )
+    treedata.Insert("", '_B_', 'B', [4, 5, 6], )
+    treedata.Insert("_A_", '_A1_', 'Sub Item 1', ['can', 'be', 'anything'], )
+    treedata.Insert("", '_C_', 'C', [], )
+    treedata.Insert("_C_", '_C1_', 'C1', ['or'], )
+    treedata.Insert("_A_", '_A2_', 'Sub Item 2', [None, None])
+    treedata.Insert("_A1_", '_A3_', 'A30', ['getting deep'])
+    treedata.Insert("_C_", '_C2_', 'C2', ['nothing', 'at', 'all'])
 
     for i in range(100):
         treedata.Insert('_C_', i, i, [])
 
     frame1 = [
         [Input('Input Text', size=(25, 1)), ],
         [Multiline(size=(30, 5), default_text='Multiline Input')],
@@ -26405,8 +26405,8 @@
         _upgrade_gui()
         exit(0)
     elif len(sys.argv) > 1 and sys.argv[1] == 'help':
         main_sdk_help()
         exit(0)
     main()
     exit(0)
-#25424909a31c4fa789f5aa4e210e7e07d412560195dc21abe678b68a3b4bdb2a8a78651d8613daaded730bc2a31adc02ba8b99717fff701cda8ae13c31f1dcee9da8837908626f1c5cc81e7a34d3b9cd032dba190647564bba72d248ad6b83e30c8abc057f3f1b1fb3a2ca853069de936f3f53522fd4732b743268e0fcde54577a05880f2057efe6bbd6349f77d6c002544f38e24db40ab84f3dde4a4b8b31e84480db31656fb74ae0c01a7af0b35ac66cf8a0fbb8ca85685fea075608c7862da6635511d0e5403c4a637138324ce1fb1308b765cba53863ddf7b01ca4fc988932b03c4a8403a72b8105f821913f02925218dbecf1e089bd32e78667939503f2abfd89b37fa293927e30550d441f21dc68273d2d07ed910f6a69bc8c792015eb623ada7e65347cf0389cf2a1696a7ccf88098a4fb4bfa44e88fac2a94a44e25b010355e48d483d896c58eb771ef47e01066156f9344750b487e176ca0642601951f096d4c03045aa8f912d475dbe04b82c6ddf1ac3adbf815aef4ca2c6add058c2789b66a9abd875f334752ec1bde11b9b56e334823304b6cc3fadf7daae277c982ebc7eadb726a33e2740d075ad082b9c20304c4a53228d6f05357c40903a78113aea4e6169e1a5351866f7a9ffc6666eb08a31bfb84d90cb3002f7ebf87871988b88a7b8a52d36a1a7dd826360b5c6ad922829d9f73d204f09d1b9ad9ffd8d
+#25424909a31c4fa789f5aa4e210e7e07d412560195dc21abe678b68a3b4bdb2a8a78651d8613daaded730bc2a31adc02ba8b99717fff701cda8ae13c31f1dcee9da8837908626f1c5cc81e7a34d3b9cd032dba190647564bba72d248ad6b83e30c8abc057f3f1b1fb3a2ca853069de936f3f53522fd4732b743268e0fcde54577a05880f2057efe6bbd6349f77d6c002544f38e24db40ab84f3dde4a4b8b31e84480db31656fb74ae0c01a7af0b35ac66cf8a0fbb8ca85685fea075608c7862da6635511d0e5403c4a637138324ce1fb1308b765cba53863ddf7b01ca4fc988932b03c4a8403a72b8105f821913f02925218dbecf1e089bd32e78667939503f2abfd89b37fa293927e30550d441f21dc68273d2d07ed910f6a69bc8c792015eb623ada7e65347cf0389cf2a1696a7ccf88098a4fb4bfa44e88fac2a94a44e25b010355e48d483d896c58eb771ef47e01066156f9344750b487e176ca0642601951f096d4c03045aa8f912d475dbe04b82c6ddf1ac3adbf815aef4ca2c6add058c2789b66a9abd875f334752ec1bde11b9b56e334823304b6cc3fadf7daae277c982ebc7eadb726a33e2740d075ad082b9c20304c4a53228d6f05357c40903a78113aea4e6169e1a5351866f7a9ffc6666eb08a31bfb84d90cb3002f7ebf87871988b88a7b8a52d36a1a7dd826360b5c6ad922829d9f73d204f09d1b9ad9ffd8d
```

### Comparing `FreeSimpleGUI-5.0.0/FreeSimpleGUI.egg-info/PKG-INFO` & `FreeSimpleGUI-5.0.0rc1/FreeSimpleGUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: FreeSimpleGUI
-Version: 5.0.0
+Version: 5.0.0rc1
 Summary: The free-forever Python GUI framework.
 Home-page: https://github.com/spyoungtech/FreeSimpleGui
 Maintainer: Spencer Phillip Young
 Maintainer-email: spencer.young@spyoung.com
-Keywords: PySimpleGui fork GUI UI tkinter Qt WxPython Remi wrapper simple easy beginner novice student graphics progressbar progressmeter
+Keywords: PySimpleGui GUI UI tkinter Qt WxPython Remi wrapper simple easy beginner novice student graphics progressbar progressmeter
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `FreeSimpleGUI-5.0.0/NOTICE` & `FreeSimpleGUI-5.0.0rc1/NOTICE`

 * *Files identical despite different names*

### Comparing `FreeSimpleGUI-5.0.0/PKG-INFO` & `FreeSimpleGUI-5.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: FreeSimpleGUI
-Version: 5.0.0
+Version: 5.0.0rc1
 Summary: The free-forever Python GUI framework.
 Home-page: https://github.com/spyoungtech/FreeSimpleGui
 Maintainer: Spencer Phillip Young
 Maintainer-email: spencer.young@spyoung.com
-Keywords: PySimpleGui fork GUI UI tkinter Qt WxPython Remi wrapper simple easy beginner novice student graphics progressbar progressmeter
+Keywords: PySimpleGui GUI UI tkinter Qt WxPython Remi wrapper simple easy beginner novice student graphics progressbar progressmeter
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `FreeSimpleGUI-5.0.0/setup.cfg` & `FreeSimpleGUI-5.0.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = FreeSimpleGUI
-version = 5.0.0
+version = 5.0.0rc1
 maintainer = Spencer Phillip Young
 maintainer_email = spencer.young@spyoung.com
 description = The free-forever Python GUI framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
-keywords = PySimpleGui fork GUI UI tkinter Qt WxPython Remi wrapper simple easy beginner novice student graphics progressbar progressmeter
+keywords = PySimpleGui GUI UI tkinter Qt WxPython Remi wrapper simple easy beginner novice student graphics progressbar progressmeter
 url = https://github.com/spyoungtech/FreeSimpleGui
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.4
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
```

