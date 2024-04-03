# Comparing `tmp/ctkchart-2.0.3.tar.gz` & `tmp/ctkchart-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctkchart-2.0.3.tar", last modified: Mon Apr  1 23:36:59 2024, max compression
+gzip compressed data, was "ctkchart-2.1.0.tar", last modified: Wed Apr  3 22:23:33 2024, max compression
```

## Comparing `ctkchart-2.0.3.tar` & `ctkchart-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.516157 ctkchart-2.0.3/
--rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 ctkchart-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     3638 2024-04-01 23:36:59.500905 ctkchart-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2024-04-01 23:35:38.000000 ctkchart-2.0.3/README.md
--rw-rw-rw-   0        0        0     1011 2024-04-01 11:03:36.000000 ctkchart-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 23:36:59.517134 ctkchart-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.127618 ctkchart-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.488140 ctkchart-2.0.3/src/ctkchart/
--rw-rw-rw-   0        0        0     9191 2024-04-01 05:35:12.000000 ctkchart-2.0.3/src/ctkchart/CTkLine.py
--rw-rw-rw-   0        0        0    98481 2024-04-01 23:20:48.000000 ctkchart-2.0.3/src/ctkchart/CTkLineChart.py
--rw-rw-rw-   0        0        0     1804 2024-03-31 14:08:39.000000 ctkchart-2.0.3/src/ctkchart/FontStyle.py
--rw-rw-rw-   0        0        0     1916 2024-03-22 05:40:12.000000 ctkchart-2.0.3/src/ctkchart/Utils.py
--rw-rw-rw-   0        0        0    10886 2024-04-01 18:33:10.000000 ctkchart-2.0.3/src/ctkchart/Validate.py
--rw-rw-rw-   0        0        0      289 2024-04-01 23:24:49.000000 ctkchart-2.0.3/src/ctkchart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.499930 ctkchart-2.0.3/src/ctkchart.egg-info/
--rw-rw-rw-   0        0        0     3638 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 22:23:33.895429 ctkchart-2.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 ctkchart-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5674 2024-04-03 22:23:33.875020 ctkchart-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3271 2024-04-03 15:48:23.000000 ctkchart-2.1.0/README.md
+-rw-rw-rw-   0        0        0     1272 2024-04-03 22:23:19.000000 ctkchart-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 22:23:33.896406 ctkchart-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 22:23:33.696355 ctkchart-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 22:23:33.828951 ctkchart-2.1.0/src/ctkchart/
+-rw-rw-rw-   0        0        0     9191 2024-04-01 05:35:12.000000 ctkchart-2.1.0/src/ctkchart/CTkLine.py
+-rw-rw-rw-   0        0        0    98084 2024-04-03 13:40:34.000000 ctkchart-2.1.0/src/ctkchart/CTkLineChart.py
+-rw-rw-rw-   0        0        0     1804 2024-03-31 14:08:39.000000 ctkchart-2.1.0/src/ctkchart/FontStyle.py
+-rw-rw-rw-   0        0        0     1916 2024-03-22 05:40:12.000000 ctkchart-2.1.0/src/ctkchart/Utils.py
+-rw-rw-rw-   0        0        0    10886 2024-04-01 18:33:10.000000 ctkchart-2.1.0/src/ctkchart/Validate.py
+-rw-rw-rw-   0        0        0      289 2024-04-03 13:49:00.000000 ctkchart-2.1.0/src/ctkchart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:23:33.844288 ctkchart-2.1.0/src/ctkchart.egg-info/
+-rw-rw-rw-   0        0        0     5674 2024-04-03 22:23:33.000000 ctkchart-2.1.0/src/ctkchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-04-03 22:23:33.000000 ctkchart-2.1.0/src/ctkchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 22:23:33.000000 ctkchart-2.1.0/src/ctkchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-03 22:23:33.000000 ctkchart-2.1.0/src/ctkchart.egg-info/top_level.txt
```

### Comparing `ctkchart-2.0.3/LICENSE` & `ctkchart-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctkchart-2.0.3/src/ctkchart/CTkLine.py` & `ctkchart-2.1.0/src/ctkchart/CTkLine.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.0.3/src/ctkchart/CTkLineChart.py` & `ctkchart-2.1.0/src/ctkchart/CTkLineChart.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,14 @@
       self.__x_axis_display_values_indices = x_axis_display_values_indices
       self.__x_labels_values_index_change = 1
       self.__x_axis_data = str(x_axis_data)
       self.__x_axis_data_position = x_axis_data_position
       self.__x_axis_values = x_axis_values
       self.__x_axis_values_handle_by = "label_count"
       self.__x_space = x_space
-      self.__force_to_stop_data_showing = False
-      self.__is_data_showing_working = False
       self.__pointer_state = pointer_state
       self.__pointing_callback_function = pointing_callback_function
       self.__pointing_values_precision = pointing_values_precision
       self.__pointer_lock = pointer_lock
       self.__pointer_size = pointer_size
       self.__pointer_color = pointer_color
       self.__x_values_frame_place_req = True
@@ -237,15 +235,15 @@
       if  self.__x_axis_display_values_indices != None :
          self.__x_axis_display_values_indices = Utils._sort_tuple(self.__x_axis_display_values_indices)
          self.__x_axis_values_handle_by = "label_indices"
       else:
          self.__x_axis_values_handle_by = "label_count"
 
       
-      self.__theme = "unknown"
+      self.__theme = customtkinter.get_appearance_mode()
       self.__margin = 10
 
       self.__create_widgets()
       self.__configure_required_widget_size()
       self.__configure_x_axis_labels_info()
       self.__configure_x_axis_point_spacing()
       self.__create_x_axis_labels()
@@ -277,15 +275,15 @@
          """
          Internal loop to track theme changes and update the widget appearance.
          """
          
          if self.__theme !=  customtkinter.get_appearance_mode():
             self.__theme = customtkinter.get_appearance_mode()
             self.__configure_widget_for_theme_changes()
-            self.__call_reshow_data()
+            self.__reshow_data()
          try:
             self.master.after(1000,__track_theme_changes_loop)
          except AttributeError:
             Validate._invalidMaster(self.master)
       __track_theme_changes_loop()
       
       
@@ -430,15 +428,15 @@
             self.__y_axis_data_label.place(x=self.__margin, y=self.__y_space+self.__y_special_height_space+self.__real_height/2,anchor="w")
       
       if self.__x_axis_data != "":
          if self.__x_axis_data_position=="top":
             self.__x_axis_data_label.place(rely=1, relx=1, x=-self.__x_axis_data_req_width+-self.__margin, y=-self.__x_axis_data_req_height)
          else:
             self.__x_axis_data_label.place(rely=1, y=-self.__x_axis_data_req_height, relx=0, anchor="n",
-                                    x=(self.__real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space+self.__margin)
+                                    x=(self.__const_real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space+self.__margin)
       
       self.__y_axis_frame.configure(width=self.__axis_size)
       self.__x_axis_frame.configure(height=self.__axis_size)
 
       self.__y_axis_frame.place(x=self.__y_value_req_width_space+self.__y_axis_data_req_width_space_side+self.__margin,
                          y=float(self.__y_axis_data_req_height_space_top+(self.__y_value_req_height_space/2)+self.__y_special_height_space),
                          )
@@ -478,18 +476,18 @@
          This method calculates and sets the spacing between points on the x-axis based on the 
          specified handle method. If the spacing is handled automatically, it calculates the spacing 
          based on the real width of the LineChart and the number of x-axis values. If handled manually, 
          it uses the specified x-axis point spacing value.
       """
    
       if self.__x_axis_point_spacing_handle_by== "auto":
-         self.__x_axis_point_spacing = (self.__real_width / len(self.__x_axis_values))
+         self.__x_axis_point_spacing = (self.__const_real_width / len(self.__x_axis_values))
       elif self.__x_axis_point_spacing_handle_by== "manual":
          self.__x_axis_point_spacing = self.__x_axis_point_spacing
-     
+         
       
    def __configure_required_widget_size(self) -> None:
       """
       Configure the required sizes of the LineChart's widgets.
 
          This method calculates and sets the required sizes for various widgets in the LineChart,
          such as axis labels, based on the provided data and styling options. It determines the
@@ -1198,21 +1196,22 @@
       if pointer_size != None:
          Validate._isInt(pointer_size, "pointer_size")
          self.__pointer_size = pointer_size
          pointer_size_change_req = True
          
       if x_axis_point_spacing != None:
          Validate._isValidXAxisPointSpacing(x_axis_point_spacing, "x_axis_point_spacing")
-         if x_axis_point_spacing != self.__x_axis_point_spacing:
-            if x_axis_point_spacing == "auto":
+         if x_axis_point_spacing == "auto" : 
+            if self.__x_axis_point_spacing_handle_by != "auto":
                self.__x_axis_point_spacing_handle_by = "auto"
-            else:
+               reshow_data_req = True
+         elif self.__x_axis_point_spacing != x_axis_point_spacing:
                self.__x_axis_point_spacing_handle_by = "manual"
-            self.__x_axis_point_spacing = x_axis_point_spacing
-            reshow_data_req = True
+               self.__x_axis_point_spacing = x_axis_point_spacing
+               reshow_data_req = True
       
       if chart_reset_req :
          self.__destroy_x_axis_labels()
          self.__destroy_y_axis_labels()
          self.__destroy_x_y_sections()
          self.__configure_required_widget_size()
          self.__configure_x_axis_point_spacing()
@@ -1227,15 +1226,15 @@
          self.__set_pointer_state()
          self.__set_pointer_size()
          self.__set_widgets_fonts()
          self.__set_customtkinter_widgets_colors()
          self.__set_tkinter_widgets_colors()
          self.__place_widgets()
          self.__reset_chart_info()
-         self.__call_reshow_data()
+         self.__reshow_data()
       
       if chart_x_labels_change_req:
          self.__configure_x_axis_labels_info()
          self.__destroy_x_axis_labels()
          self.__create_x_axis_labels()
          self.__set_x_axis_values()
       
@@ -1257,15 +1256,15 @@
          self.__set_tkinter_widgets_colors()
       
       if widget_size_change_req == True:
          self.__set_pointer_size()
          
       if reshow_data_req:
          self.__configure_x_axis_point_spacing()
-         self.__call_reshow_data()
+         self.__reshow_data()
       
       if pointer_size_change_req:
          self.__set_pointer_size()
          
       if pointer_state_change_req:
          self.__set_pointer_state()
          
@@ -1303,28 +1302,34 @@
       """
       
       for line in  self.__lines:
          line._CTkLine__reset()
    
 
    
-   def __call_reshow_data(self) -> None:
+   #def __call_reshow_data(self) -> None:
       """
       Call the method to re-show data on the chart.
 
          This method sets a flag to force the chart to stop data showing, waits until the data showing process is stopped,
          and then triggers the re-showing of data.
       """
-
-      self.__force_to_stop_data_showing = True
-      while  self.__is_data_showing_working:
-         pass
-      self.__force_to_stop_data_showing = False
-      self.__reshow_data()
+   #   import time
+   #   import threading as thead
       
+   #   def wait():
+   #      self.__force_to_stop_data_showing = True
+   #      while  self.__is_data_showing_working:
+   #         print("waitin")
+   #         time.sleep(0.1)
+   #      self.__force_to_stop_data_showing = False
+   
+   #      self.__reshow_data()
+   #   thead.Thread(target=wait).start()
+   
       
    def __reshow_data(self) -> None:
       """
       Re-shows data on the chart.
 
          This method recalculates the chart info, ensures that the chart can support the maximum amount of data to be shown,
          resets each line with the latest data, and then displays the data for each line.
@@ -1339,19 +1344,16 @@
          
          for line in  self.__lines:
             if maximum_data>max_support:
                line._CTkLine__temp_data = line._CTkLine__data[maximum_data-(max_support)::]
             else:
                line._CTkLine__temp_data = line._CTkLine__data
             line._CTkLine__reset()
-         
-         lines = self.__lines
-         self.lines =[]
-         
-         for line in lines:
+      
+         for line in self.__lines:
             self.show_data(line=line, data=line._CTkLine__temp_data)
    
    
    def __get_color_by_theme(self, color_s: Union[Tuple[str, str], str]) -> str:
       """
       Get the color based on the current theme.
 
@@ -1389,152 +1391,146 @@
       
       re_show_data = False
       if line not in self.__lines:
          Validate._invalidLine(line)
       
       line._CTkLine__data += data
       
-      if line._CTkLine__visibility:
+      if line._CTkLine__visibility :
          
          line_color = self.__get_color_by_theme(line._CTkLine__color)
          highlight_color = self.__get_color_by_theme(line._CTkLine__point_highlight_color)
          fill_color = self.__get_color_by_theme(line._CTkLine__fill_color)
          
          for d in data:
-            self.__is_data_showing_working = True
             
-            if not self.__force_to_stop_data_showing:
-               x_start = line._CTkLine__x_end
-               y_start = line._CTkLine__y_end
-               
-               line._CTkLine__x_end += self.__x_axis_point_spacing
-         
-               if d >=0 :
-                  d = d - self.__y_axis_min_value
-                  line._CTkLine__y_end = self.__const_real_height - ((d )/self.__y_axis_values_gap * self.__const_real_height)
-               else:
-                  d = abs(d) +self.__y_axis_max_value
-                  line._CTkLine__y_end = ((d)/self.__y_axis_values_gap * self.__const_real_height)
-               line._CTkLine__y_end += ((line._CTkLine__size)/2)
+            x_start = line._CTkLine__x_end
+            y_start = line._CTkLine__y_end
+            
+            line._CTkLine__x_end += self.__x_axis_point_spacing
+      
+            if d >=0 :
+               d = d - self.__y_axis_min_value
+               line._CTkLine__y_end = self.__const_real_height - ((d )/self.__y_axis_values_gap * self.__const_real_height)
+            else:
+               d = abs(d) +self.__y_axis_max_value
+               line._CTkLine__y_end = ((d)/self.__y_axis_values_gap * self.__const_real_height)
+            line._CTkLine__y_end += ((line._CTkLine__size)/2)
 
-               if round(line._CTkLine__x_end) > round(self.__real_width) and self.__real_width < 15000:
-                  self.__place_x -= self.__x_axis_point_spacing
-                  
-                  self.__output_canvas.place(x=self.__place_x,
-                                    width=self.__real_width+self.__x_axis_point_spacing)
-                  
-                  self.__real_width += self.__x_axis_point_spacing;
+            if round(line._CTkLine__x_end) > round(self.__real_width) and self.__real_width < self.__width*5:
+               self.__place_x -= self.__x_axis_point_spacing
                
-               elif self.__real_width > 15000:
-                  re_show_data = True
-                  break;
+               self.__output_canvas.place(x=self.__place_x,
+                                 width=self.__real_width+self.__x_axis_point_spacing)
                
-               if line._CTkLine__fill == "enabled":
-                  points_of_polygon = [x_start, y_start, 
-                             line._CTkLine__x_end, line._CTkLine__y_end,
-                             line._CTkLine__x_end, self.__const_real_height,
-                             x_start, self.__const_real_height]
-                  self.__output_canvas.create_polygon(points_of_polygon,
-                                                      fill=fill_color)
-                  
-               if line._CTkLine__style  == "dashed" :
-                  dash_width = line._CTkLine__style_type[0]
-                  space_width = line._CTkLine__style_type[1]
-                  total_width = dash_width+space_width
-                  real_x_axis_point_spacing = ((abs(y_start - line._CTkLine__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
-                  dash_count = real_x_axis_point_spacing /( dash_width + space_width)
-                  total_change_x = (line._CTkLine__x_end - x_start)
-                  total_change_y = (line._CTkLine__y_end - y_start)
-                  dash_change_percentage = dash_width/total_width
-                  space_change_percentage = space_width/total_width
-                  change_x = (total_change_x/dash_count)
-                  change_y = (total_change_y/dash_count)
-                  dash_change_x = change_x*dash_change_percentage
-                  dash_change_y = change_y*dash_change_percentage
-                  space_change_x = change_x*space_change_percentage
-                  space_change_y = change_y*space_change_percentage
-                  dashed_x_start = x_start
-                  dashed_y_start = y_start
-                  if y_start >  line._CTkLine__y_end: line_going = "to_up"
-                  else : line_going = "to_down"
-                  while (line._CTkLine__x_end>dashed_x_start):
-                     dashed_x_end = dashed_x_start+dash_change_x
-                     dashed_y_end = dashed_y_start+dash_change_y
-                     if dashed_x_end>line._CTkLine__x_end:
-                           dashed_x_end = dashed_x_end - (dashed_x_end-line._CTkLine__x_end)
-                     if dashed_y_end<=line._CTkLine__y_end and line_going=="to_up":
-                           dashed_y_end = dashed_y_end - (dashed_y_end-line._CTkLine__y_end)
-                     if dashed_y_end>line._CTkLine__y_end and  line_going=="to_down":
-                           dashed_y_end = dashed_y_end - (dashed_y_end-line._CTkLine__y_end)
-                     self.__output_canvas.create_line(dashed_x_start, dashed_y_start, dashed_x_end, dashed_y_end
-                                                      ,fill=line_color ,width=line._CTkLine__size)
-                     dashed_x_start += dash_change_x + space_change_x
-                     dashed_y_start += dash_change_y + space_change_y
-                        
-               elif line._CTkLine__style == "dotted":
-                  circle_size = line._CTkLine__style_type[0]
-                  space_width = line._CTkLine__style_type[1]
-                  total_width = circle_size+space_width
-                  real_x_axis_point_spacing = ((abs(y_start - line._CTkLine__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
-                  circle_count = real_x_axis_point_spacing /( circle_size + space_width)
-                  total_change_x = (line._CTkLine__x_end - x_start)
-                  total_change_y = (line._CTkLine__y_end - y_start)
-                  circle_change_percentage = circle_size/total_width*100
-                  space_change_percentage = space_width/total_width*100
-                  circle_change_x = (total_change_x/circle_count)/100*circle_change_percentage
-                  circle_change_y = (total_change_y/circle_count)/100*circle_change_percentage
-                  space_change_x = (total_change_x/circle_count)/100*space_change_percentage
-                  space_change_y = (total_change_y/circle_count)/100*space_change_percentage
-                  dotted_x_start = x_start
-                  dotted_y_start = y_start
-                  if y_start >  line._CTkLine__y_end: line_going = "to_up"
-                  else : line_going = "to_down"
-                  while (line._CTkLine__x_end>dotted_x_start):
-                        x_end = dotted_x_start+circle_change_x
-                        y_end = dotted_y_start+circle_change_y
-                        if x_end>line._CTkLine__x_end:
-                           x_end = x_end - (x_end-line._CTkLine__x_end)
-                        if y_end<=line._CTkLine__y_end and line_going=="to_up":
-                           y_end = y_end - (y_end-line._CTkLine__y_end)
-                        if y_end>line._CTkLine__y_end and  line_going=="to_down":
-                           y_end = y_end - (y_end-line._CTkLine__y_end)
-                        self.__output_canvas.create_oval(dotted_x_start-circle_size/2,
-                                                   dotted_y_start-circle_size/2,
-                                                   dotted_x_start+circle_size-circle_size/2,
-                                                   dotted_y_start+circle_size-circle_size/2,
-                                                   fill=line_color, outline=line_color )
-                        dotted_x_start += circle_change_x + space_change_x
-                        dotted_y_start += circle_change_y + space_change_y
-
-               elif line._CTkLine__style=="normal":
-                  self.__output_canvas.create_line(x_start, y_start, line._CTkLine__x_end, line._CTkLine__y_end
-                                                      ,fill=line_color ,width=line._CTkLine__size)
-                    
-               if line._CTkLine__point_highlight == "enabled" and line._CTkLine__point_highlight_size > 0 : 
-                  highlight_size =  line._CTkLine__point_highlight_size /2 
-                  self.__output_canvas.create_oval(line._CTkLine__x_end - highlight_size,
-                                                   line._CTkLine__y_end - highlight_size,
-                                                   line._CTkLine__x_end + highlight_size,
-                                                   line._CTkLine__y_end + highlight_size,
-                                                   fill=highlight_color,
-                                                   outline=highlight_color)
+               self.__real_width += self.__x_axis_point_spacing;
+            
+            elif self.__real_width > self.__width*5:
+               re_show_data = True
+               break;
+            
+            if line._CTkLine__fill == "enabled":
+               points_of_polygon = [x_start, y_start, 
+                           line._CTkLine__x_end, line._CTkLine__y_end,
+                           line._CTkLine__x_end, self.__const_real_height,
+                           x_start, self.__const_real_height]
+               self.__output_canvas.create_polygon(points_of_polygon,
+                                                   fill=fill_color)
+               
+            if line._CTkLine__style  == "dashed" :
+               dash_width = line._CTkLine__style_type[0]
+               space_width = line._CTkLine__style_type[1]
+               total_width = dash_width+space_width
+               real_x_axis_point_spacing = ((abs(y_start - line._CTkLine__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
+               dash_count = real_x_axis_point_spacing /( dash_width + space_width)
+               total_change_x = (line._CTkLine__x_end - x_start)
+               total_change_y = (line._CTkLine__y_end - y_start)
+               dash_change_percentage = dash_width/total_width
+               space_change_percentage = space_width/total_width
+               change_x = (total_change_x/dash_count)
+               change_y = (total_change_y/dash_count)
+               dash_change_x = change_x*dash_change_percentage
+               dash_change_y = change_y*dash_change_percentage
+               space_change_x = change_x*space_change_percentage
+               space_change_y = change_y*space_change_percentage
+               dashed_x_start = x_start
+               dashed_y_start = y_start
+               if y_start >  line._CTkLine__y_end: line_going = "to_up"
+               else : line_going = "to_down"
+               while (line._CTkLine__x_end>dashed_x_start):
+                  dashed_x_end = dashed_x_start+dash_change_x
+                  dashed_y_end = dashed_y_start+dash_change_y
+                  if dashed_x_end>line._CTkLine__x_end:
+                        dashed_x_end = dashed_x_end - (dashed_x_end-line._CTkLine__x_end)
+                  if dashed_y_end<=line._CTkLine__y_end and line_going=="to_up":
+                        dashed_y_end = dashed_y_end - (dashed_y_end-line._CTkLine__y_end)
+                  if dashed_y_end>line._CTkLine__y_end and  line_going=="to_down":
+                        dashed_y_end = dashed_y_end - (dashed_y_end-line._CTkLine__y_end)
+                  self.__output_canvas.create_line(dashed_x_start, dashed_y_start, dashed_x_end, dashed_y_end
+                                                   ,fill=line_color ,width=line._CTkLine__size)
+                  dashed_x_start += dash_change_x + space_change_x
+                  dashed_y_start += dash_change_y + space_change_y
+                     
+            elif line._CTkLine__style == "dotted":
+               circle_size = line._CTkLine__style_type[0]
+               space_width = line._CTkLine__style_type[1]
+               total_width = circle_size+space_width
+               real_x_axis_point_spacing = ((abs(y_start - line._CTkLine__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
+               circle_count = real_x_axis_point_spacing /( circle_size + space_width)
+               total_change_x = (line._CTkLine__x_end - x_start)
+               total_change_y = (line._CTkLine__y_end - y_start)
+               circle_change_percentage = circle_size/total_width*100
+               space_change_percentage = space_width/total_width*100
+               circle_change_x = (total_change_x/circle_count)/100*circle_change_percentage
+               circle_change_y = (total_change_y/circle_count)/100*circle_change_percentage
+               space_change_x = (total_change_x/circle_count)/100*space_change_percentage
+               space_change_y = (total_change_y/circle_count)/100*space_change_percentage
+               dotted_x_start = x_start
+               dotted_y_start = y_start
+               if y_start >  line._CTkLine__y_end: line_going = "to_up"
+               else : line_going = "to_down"
+               while (line._CTkLine__x_end>dotted_x_start):
+                     x_end = dotted_x_start+circle_change_x
+                     y_end = dotted_y_start+circle_change_y
+                     if x_end>line._CTkLine__x_end:
+                        x_end = x_end - (x_end-line._CTkLine__x_end)
+                     if y_end<=line._CTkLine__y_end and line_going=="to_up":
+                        y_end = y_end - (y_end-line._CTkLine__y_end)
+                     if y_end>line._CTkLine__y_end and  line_going=="to_down":
+                        y_end = y_end - (y_end-line._CTkLine__y_end)
+                     self.__output_canvas.create_oval(dotted_x_start-circle_size/2,
+                                                dotted_y_start-circle_size/2,
+                                                dotted_x_start+circle_size-circle_size/2,
+                                                dotted_y_start+circle_size-circle_size/2,
+                                                fill=line_color, outline=line_color )
+                     dotted_x_start += circle_change_x + space_change_x
+                     dotted_y_start += circle_change_y + space_change_y
+
+            elif line._CTkLine__style=="normal":
+               self.__output_canvas.create_line(x_start, y_start, line._CTkLine__x_end, line._CTkLine__y_end
+                                                   ,fill=line_color ,width=line._CTkLine__size)
                   
-                  self.__output_canvas.create_oval(x_start - highlight_size,
-                                                   y_start - highlight_size,
-                                                   x_start + highlight_size,
-                                                   y_start + highlight_size,
-                                                   fill=highlight_color,
-                                                   outline=highlight_color)
-            else:
-               break
-         
+            if line._CTkLine__point_highlight == "enabled" and line._CTkLine__point_highlight_size > 0 : 
+               highlight_size =  line._CTkLine__point_highlight_size /2 
+               self.__output_canvas.create_oval(line._CTkLine__x_end - highlight_size,
+                                                line._CTkLine__y_end - highlight_size,
+                                                line._CTkLine__x_end + highlight_size,
+                                                line._CTkLine__y_end + highlight_size,
+                                                fill=highlight_color,
+                                                outline=highlight_color)
+               
+               self.__output_canvas.create_oval(x_start - highlight_size,
+                                                y_start - highlight_size,
+                                                x_start + highlight_size,
+                                                y_start + highlight_size,
+                                                fill=highlight_color,
+                                                outline=highlight_color)
+            
          if re_show_data:
-            self.__reshow_data()
-         self.__is_data_showing_working = False
-   
+            self.__reshow_data()   
    
    def __hide_pointer(self, event: tkinter.Event) -> None:
       """
       Hides the pointer widget from the GUI canvas.
 
          Args:
             event (tkinter.Event): The event triggering the pointer hiding.
@@ -1755,15 +1751,15 @@
             state (bool): The hide/show state of the line.
       """
       
       Validate._isValidCTkLine(line, "line")
       Validate._isBool(state, "state")
       if line._CTkLine__visibility != state or self.__visibility != state:
          line._CTkLine__visibility = state
-         self.__call_reshow_data()
+         self.__reshow_date()
 
       
    def set_lines_visibility(self, state: bool) -> None:
       """
       Hide or show all lines.
 
          Args:
@@ -1772,15 +1768,15 @@
       
       Validate._isBool(state, "state")
       self.__visibility = state
       if state == False:
          self.__output_canvas.place_forget()
       for line in self.__lines:
          line._CTkLine__visibility = state
-      self.__call_reshow_data()
+      self.__reshow_data()
    
       
    def reset(self) -> None:
       """
       Reset the chart and lines to their initial state.
       """
       
@@ -1789,15 +1785,15 @@
    
    
    def __apply_line_configuration(self) -> None :
       """
       Apply changes to the lines and redraw the chart. 
       """
       
-      self.__call_reshow_data()
+      self.__reshow_data()
       
       
    def cget(self, attribute_name: Literal[
          "width", "height", "axis_color", "bg_color", "fg_color",
          "data_font_style", "axis_font_style", "y_axis_precision", 
          "y_axis_data", "y_axis_label_count", "y_axis_values", 
          "y_axis_font_color", "y_axis_data_font_color",
```

### Comparing `ctkchart-2.0.3/src/ctkchart/FontStyle.py` & `ctkchart-2.1.0/src/ctkchart/FontStyle.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.0.3/src/ctkchart/Utils.py` & `ctkchart-2.1.0/src/ctkchart/Utils.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.0.3/src/ctkchart/Validate.py` & `ctkchart-2.1.0/src/ctkchart/Validate.py`

 * *Files identical despite different names*

