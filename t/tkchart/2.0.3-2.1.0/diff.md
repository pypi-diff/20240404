# Comparing `tmp/tkchart-2.0.3.tar.gz` & `tmp/tkchart-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkchart-2.0.3.tar", last modified: Mon Apr  1 23:47:05 2024, max compression
+gzip compressed data, was "tkchart-2.1.0.tar", last modified: Wed Apr  3 23:29:38 2024, max compression
```

## Comparing `tkchart-2.0.3.tar` & `tkchart-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.793302 tkchart-2.0.3/
--rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 tkchart-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     3450 2024-04-01 23:47:05.792318 tkchart-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1420 2024-04-01 23:40:03.000000 tkchart-2.0.3/README.md
--rw-rw-rw-   0        0        0      857 2024-04-01 23:45:12.000000 tkchart-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 23:47:05.793302 tkchart-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.753206 tkchart-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.779063 tkchart-2.0.3/src/tkchart/
--rw-rw-rw-   0        0        0     1804 2024-03-11 17:44:06.000000 tkchart-2.0.3/src/tkchart/FontStyle.py
--rw-rw-rw-   0        0        0     8808 2024-04-01 05:24:54.000000 tkchart-2.0.3/src/tkchart/Line.py
--rw-rw-rw-   0        0        0    92978 2024-04-01 23:43:10.000000 tkchart-2.0.3/src/tkchart/LineChart.py
--rw-rw-rw-   0        0        0     1816 2024-03-22 05:38:59.000000 tkchart-2.0.3/src/tkchart/Utils.py
--rw-rw-rw-   0        0        0    10049 2024-04-01 01:19:52.000000 tkchart-2.0.3/src/tkchart/Validate.py
--rw-rw-rw-   0        0        0      277 2024-04-01 23:24:43.000000 tkchart-2.0.3/src/tkchart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.792318 tkchart-2.0.3/src/tkchart.egg-info/
--rw-rw-rw-   0        0        0     3450 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 23:29:38.819351 tkchart-2.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 tkchart-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5586 2024-04-03 23:29:38.818021 tkchart-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3197 2024-04-03 23:27:12.000000 tkchart-2.1.0/README.md
+-rw-rw-rw-   0        0        0     1259 2024-04-03 23:18:36.000000 tkchart-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 23:29:38.819351 tkchart-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 23:29:38.762090 tkchart-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:29:38.792911 tkchart-2.1.0/src/tkchart/
+-rw-rw-rw-   0        0        0     1804 2024-03-11 17:44:06.000000 tkchart-2.1.0/src/tkchart/FontStyle.py
+-rw-rw-rw-   0        0        0     8808 2024-04-01 05:24:54.000000 tkchart-2.1.0/src/tkchart/Line.py
+-rw-rw-rw-   0        0        0    92583 2024-04-03 13:46:40.000000 tkchart-2.1.0/src/tkchart/LineChart.py
+-rw-rw-rw-   0        0        0     1816 2024-03-22 05:38:59.000000 tkchart-2.1.0/src/tkchart/Utils.py
+-rw-rw-rw-   0        0        0    10049 2024-04-01 01:19:52.000000 tkchart-2.1.0/src/tkchart/Validate.py
+-rw-rw-rw-   0        0        0      277 2024-04-03 13:48:34.000000 tkchart-2.1.0/src/tkchart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:29:38.804476 tkchart-2.1.0/src/tkchart.egg-info/
+-rw-rw-rw-   0        0        0     5586 2024-04-03 23:29:38.000000 tkchart-2.1.0/src/tkchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-03 23:29:38.000000 tkchart-2.1.0/src/tkchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 23:29:38.000000 tkchart-2.1.0/src/tkchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 23:29:38.000000 tkchart-2.1.0/src/tkchart.egg-info/top_level.txt
```

### Comparing `tkchart-2.0.3/LICENSE` & `tkchart-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkchart-2.0.3/src/tkchart/FontStyle.py` & `tkchart-2.1.0/src/tkchart/FontStyle.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.0.3/src/tkchart/Line.py` & `tkchart-2.1.0/src/tkchart/Line.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.0.3/src/tkchart/LineChart.py` & `tkchart-2.1.0/src/tkchart/LineChart.py`

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
@@ -382,15 +380,15 @@
             self.__y_axis_data_label.place(x=0, y=self.__y_space+self.__y_special_height_space+self.__real_height/2,anchor="w")
             
       if self.__x_axis_data != "":
          if self.__x_axis_data_position=="top":
             self.__x_axis_data_label.place(rely=1, relx=1, x=-self.__x_axis_data_req_width, y=-self.__x_axis_data_req_height)
          else:
             self.__x_axis_data_label.place(rely=1, y=-self.__x_axis_data_req_height,relx=0, anchor="n",
-                                    x=(self.__real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space)
+                                    x=(self.__const_real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space)
          
       self.__y_axis_frame.configure(width=self.__axis_size)
       self.__x_axis_frame.configure(height=self.__axis_size)
       
       self.__y_axis_frame.place(x=self.__y_value_req_width_space+self.__y_axis_data_req_width_space_side,
                          y=float(self.__y_axis_data_req_height_space_top+(self.__y_value_req_height_space/2)+self.__y_special_height_space),
                          height=self.__const_real_height+self.__y_space+self.__axis_size)
@@ -424,15 +422,15 @@
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
      
       
    def __configure_required_widget_size(self) -> None:
       """
       Configure the required sizes of the LineChart's widgets.
@@ -704,14 +702,16 @@
       if self.__x_axis_values_handle_by == "label_indices" : 
          self.__x_axis_label_count = len(self.__x_axis_values)
       
          
       elif self.__x_axis_values_handle_by=="label_count":
          if self.__x_axis_label_count == 0:
             return
+         if self.__x_axis_label_count == None:
+            self.__x_axis_label_count = len(self.__x_axis_values)
          x_axis_real_label_count = len(self.__x_axis_values)
          if self.__x_axis_label_count > x_axis_real_label_count:
             self.__x_axis_label_count = x_axis_real_label_count
          else:
             while x_axis_real_label_count%self.__x_axis_label_count != 0:
                self.__x_axis_label_count+=1
          self.__x_labels_values_index_change = int(x_axis_real_label_count/self.__x_axis_label_count)
@@ -1129,21 +1129,22 @@
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
@@ -1157,15 +1158,15 @@
          self.__set_x_y_axis_data_texts()
          self.__set_pointer_state()
          self.__set_pointer_size()
          self.__set_widgets_fonts()
          self.__set_widgets_colors()
          self.__place_widgets()
          self.__reset_chart_info()
-         self.__call_reshow_data()
+         self.__reshow_data()
       
       if chart_x_labels_change_req:
          self.__configure_x_axis_labels_info()
          self.__destroy_x_axis_labels()
          self.__create_x_axis_labels()
          self.__set_x_axis_values()
       
@@ -1186,15 +1187,15 @@
          self.__set_widgets_colors()
       
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
          
@@ -1231,27 +1232,27 @@
          This method calls the __reset() method for each line object stored in the __lines list.
       """
       
       for line in  self.__lines:
          line._Line__reset()
    
    
-   def __call_reshow_data(self) -> None:
+   #def __call_reshow_data(self) -> None:
       """
       Call the method to re-show data on the chart.
 
          This method sets a flag to force the chart to stop data showing, waits until the data showing process is stopped,
          and then triggers the re-showing of data.
       """
 
-      self.__force_to_stop_data_showing = True
-      while  self.__is_data_showing_working:
-         pass
-      self.__force_to_stop_data_showing = False
-      self.__reshow_data()
+   #   self.__force_to_stop_data_showing = True
+   #   while  self.__is_data_showing_working:
+   #      pass
+   #   self.__force_to_stop_data_showing = False
+   #   self.__reshow_data()
       
       
    def __reshow_data(self) -> None:
       """
       Re-shows data on the chart.
 
          This method recalculates the chart info, ensures that the chart can support the maximum amount of data to be shown,
@@ -1301,147 +1302,144 @@
       re_show_data = False
       if line not in self.__lines:
          Validate._invalidLine(line)
          
       line._Line__data += data
       
       if  line._Line__visibility:
-         for d in data:
-            self.__is_data_showing_working = True
-            
-            if not self.__force_to_stop_data_showing:
-               x_start = line._Line__x_end
-               y_start = line._Line__y_end
-               
-               line._Line__x_end += self.__x_axis_point_spacing
          
-               if d >=0 :
-                  d = d - self.__y_axis_min_value
-                  line._Line__y_end = self.__const_real_height - ((d )/self.__y_axis_values_gap * self.__const_real_height)
-               else:
-                  d = abs(d) +self.__y_axis_max_value
-                  line._Line__y_end = ((d)/self.__y_axis_values_gap * self.__const_real_height)
-               line._Line__y_end += ((line._Line__size)/2)
+         for d in data:
+           
+            x_start = line._Line__x_end
+            y_start = line._Line__y_end
+            
+            line._Line__x_end += self.__x_axis_point_spacing
+      
+            if d >=0 :
+               d = d - self.__y_axis_min_value
+               line._Line__y_end = self.__const_real_height - ((d )/self.__y_axis_values_gap * self.__const_real_height)
+            else:
+               d = abs(d) +self.__y_axis_max_value
+               line._Line__y_end = ((d)/self.__y_axis_values_gap * self.__const_real_height)
+            line._Line__y_end += ((line._Line__size)/2)
 
-               if round(line._Line__x_end) > round(self.__real_width) and self.__real_width < 15000:
-                  self.__place_x -= self.__x_axis_point_spacing
-                  
-                  self.__output_canvas.place(x=self.__place_x,
-                                    width=self.__real_width+self.__x_axis_point_spacing)
-                  
-                  self.__real_width += self.__x_axis_point_spacing;
+            if round(line._Line__x_end) > round(self.__real_width) and self.__real_width < self.__width*5:
+               self.__place_x -= self.__x_axis_point_spacing
                
-               elif self.__real_width > 15000:
-                  re_show_data = True
-                  break;
+               self.__output_canvas.place(x=self.__place_x,
+                                 width=self.__real_width+self.__x_axis_point_spacing)
                
-               if line._Line__fill == "enabled":
-                  points_of_polygon = [x_start, y_start, 
-                             line._Line__x_end, line._Line__y_end,
-                             line._Line__x_end, self.__const_real_height,
-                             x_start, self.__const_real_height]
-                  self.__output_canvas.create_polygon(points_of_polygon,
-                                                      fill=line._Line__fill_color)
-                  
-               if line._Line__style  == "dashed" :
-                  dash_width = line._Line__style_type[0]
-                  space_width = line._Line__style_type[1]
-                  total_width = dash_width+space_width
-                  real_x_axis_point_spacing = ((abs(y_start - line._Line__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
-                  dash_count = real_x_axis_point_spacing /( dash_width + space_width)
-                  total_change_x = (line._Line__x_end - x_start)
-                  total_change_y = (line._Line__y_end - y_start)
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
-                  if y_start >  line._Line__y_end: line_going = "to_up"
-                  else : line_going = "to_down"
-                  while (line._Line__x_end>dashed_x_start):
-                     dashed_x_end = dashed_x_start+dash_change_x
-                     dashed_y_end = dashed_y_start+dash_change_y
-                     if dashed_x_end>line._Line__x_end:
-                           dashed_x_end = dashed_x_end - (dashed_x_end-line._Line__x_end)
-                     if dashed_y_end<=line._Line__y_end and line_going=="to_up":
-                           dashed_y_end = dashed_y_end - (dashed_y_end-line._Line__y_end)
-                     if dashed_y_end>line._Line__y_end and  line_going=="to_down":
-                           dashed_y_end = dashed_y_end - (dashed_y_end-line._Line__y_end)
-                     self.__output_canvas.create_line(dashed_x_start, dashed_y_start, dashed_x_end, dashed_y_end
-                                                      ,fill=line._Line__color ,width=line._Line__size)
-                     dashed_x_start += dash_change_x + space_change_x
-                     dashed_y_start += dash_change_y + space_change_y                        
-                        
-               elif line._Line__style == "dotted":
-                  circle_size = line._Line__style_type[0]
-                  space_width = line._Line__style_type[1]
-                  total_width = circle_size+space_width
-                  real_x_axis_point_spacing = ((abs(y_start - line._Line__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
-                  circle_count = real_x_axis_point_spacing /( circle_size + space_width)
-                  total_change_x = (line._Line__x_end - x_start)
-                  total_change_y = (line._Line__y_end - y_start)
-                  circle_change_percentage = circle_size/total_width*100
-                  space_change_percentage = space_width/total_width*100
-                  circle_change_x = (total_change_x/circle_count)/100*circle_change_percentage
-                  circle_change_y = (total_change_y/circle_count)/100*circle_change_percentage
-                  space_change_x = (total_change_x/circle_count)/100*space_change_percentage
-                  space_change_y = (total_change_y/circle_count)/100*space_change_percentage
-                  dotted_x_start = x_start
-                  dotted_y_start = y_start
-                  if y_start >  line._Line__y_end: line_going = "to_up"
-                  else : line_going = "to_down"
-                  while (line._Line__x_end>dotted_x_start):
-                        x_end = dotted_x_start+circle_change_x
-                        y_end = dotted_y_start+circle_change_y
-                        if x_end>line._Line__x_end:
-                           x_end = x_end - (x_end-line._Line__x_end)
-                        if y_end<=line._Line__y_end and line_going=="to_up":
-                           y_end = y_end - (y_end-line._Line__y_end)
-                        if y_end>line._Line__y_end and  line_going=="to_down":
-                           y_end = y_end - (y_end-line._Line__y_end)
-                        self.__output_canvas.create_oval(dotted_x_start-circle_size/2,
-                                                   dotted_y_start-circle_size/2,
-                                                   dotted_x_start+circle_size-circle_size/2,
-                                                   dotted_y_start+circle_size-circle_size/2,
-                                                   fill=line._Line__color, outline=line._Line__color )
-                        dotted_x_start += circle_change_x + space_change_x
-                        dotted_y_start += circle_change_y + space_change_y
-                        
-               elif line._Line__style=="normal":
-                  self.__output_canvas.create_line(x_start, y_start, line._Line__x_end, line._Line__y_end
-                                                      ,fill=line._Line__color ,width=line._Line__size)
+               self.__real_width += self.__x_axis_point_spacing;
+            
+            elif self.__real_width > self.__width*5:
+               re_show_data = True
+               break;
+            
+            if line._Line__fill == "enabled":
+               points_of_polygon = [x_start, y_start, 
+                           line._Line__x_end, line._Line__y_end,
+                           line._Line__x_end, self.__const_real_height,
+                           x_start, self.__const_real_height]
+               self.__output_canvas.create_polygon(points_of_polygon,
+                                                   fill=line._Line__fill_color)
                
-               if line._Line__point_highlight == "enabled" and line._Line__point_highlight_size > 0 : 
-                  highlight_size =  line._Line__point_highlight_size /2 
-                  self.__output_canvas.create_oval(line._Line__x_end - highlight_size,
-                                                   line._Line__y_end - highlight_size,
-                                                   line._Line__x_end + highlight_size,
-                                                   line._Line__y_end + highlight_size,
-                                                   fill=line._Line__point_highlight_color,
-                                                   outline=line._Line__point_highlight_color)
-                  
-                  self.__output_canvas.create_oval(x_start - highlight_size,
-                                                   y_start - highlight_size,
-                                                   x_start + highlight_size,
-                                                   y_start + highlight_size,
-                                                   fill=line._Line__point_highlight_color,
-                                                   outline=line._Line__point_highlight_color)
-            else:
-               break
+            if line._Line__style  == "dashed" :
+               dash_width = line._Line__style_type[0]
+               space_width = line._Line__style_type[1]
+               total_width = dash_width+space_width
+               real_x_axis_point_spacing = ((abs(y_start - line._Line__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
+               dash_count = real_x_axis_point_spacing /( dash_width + space_width)
+               total_change_x = (line._Line__x_end - x_start)
+               total_change_y = (line._Line__y_end - y_start)
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
+               if y_start >  line._Line__y_end: line_going = "to_up"
+               else : line_going = "to_down"
+               while (line._Line__x_end>dashed_x_start):
+                  dashed_x_end = dashed_x_start+dash_change_x
+                  dashed_y_end = dashed_y_start+dash_change_y
+                  if dashed_x_end>line._Line__x_end:
+                        dashed_x_end = dashed_x_end - (dashed_x_end-line._Line__x_end)
+                  if dashed_y_end<=line._Line__y_end and line_going=="to_up":
+                        dashed_y_end = dashed_y_end - (dashed_y_end-line._Line__y_end)
+                  if dashed_y_end>line._Line__y_end and  line_going=="to_down":
+                        dashed_y_end = dashed_y_end - (dashed_y_end-line._Line__y_end)
+                  self.__output_canvas.create_line(dashed_x_start, dashed_y_start, dashed_x_end, dashed_y_end
+                                                   ,fill=line._Line__color ,width=line._Line__size)
+                  dashed_x_start += dash_change_x + space_change_x
+                  dashed_y_start += dash_change_y + space_change_y                        
+                     
+            elif line._Line__style == "dotted":
+               circle_size = line._Line__style_type[0]
+               space_width = line._Line__style_type[1]
+               total_width = circle_size+space_width
+               real_x_axis_point_spacing = ((abs(y_start - line._Line__y_end)**2) + (self.__x_axis_point_spacing**2)) ** (1/2)
+               circle_count = real_x_axis_point_spacing /( circle_size + space_width)
+               total_change_x = (line._Line__x_end - x_start)
+               total_change_y = (line._Line__y_end - y_start)
+               circle_change_percentage = circle_size/total_width*100
+               space_change_percentage = space_width/total_width*100
+               circle_change_x = (total_change_x/circle_count)/100*circle_change_percentage
+               circle_change_y = (total_change_y/circle_count)/100*circle_change_percentage
+               space_change_x = (total_change_x/circle_count)/100*space_change_percentage
+               space_change_y = (total_change_y/circle_count)/100*space_change_percentage
+               dotted_x_start = x_start
+               dotted_y_start = y_start
+               if y_start >  line._Line__y_end: line_going = "to_up"
+               else : line_going = "to_down"
+               while (line._Line__x_end>dotted_x_start):
+                     x_end = dotted_x_start+circle_change_x
+                     y_end = dotted_y_start+circle_change_y
+                     if x_end>line._Line__x_end:
+                        x_end = x_end - (x_end-line._Line__x_end)
+                     if y_end<=line._Line__y_end and line_going=="to_up":
+                        y_end = y_end - (y_end-line._Line__y_end)
+                     if y_end>line._Line__y_end and  line_going=="to_down":
+                        y_end = y_end - (y_end-line._Line__y_end)
+                     self.__output_canvas.create_oval(dotted_x_start-circle_size/2,
+                                                dotted_y_start-circle_size/2,
+                                                dotted_x_start+circle_size-circle_size/2,
+                                                dotted_y_start+circle_size-circle_size/2,
+                                                fill=line._Line__color, outline=line._Line__color )
+                     dotted_x_start += circle_change_x + space_change_x
+                     dotted_y_start += circle_change_y + space_change_y
+                     
+            elif line._Line__style=="normal":
+               self.__output_canvas.create_line(x_start, y_start, line._Line__x_end, line._Line__y_end
+                                                   ,fill=line._Line__color ,width=line._Line__size)
+            
+            if line._Line__point_highlight == "enabled" and line._Line__point_highlight_size > 0 : 
+               highlight_size =  line._Line__point_highlight_size /2 
+               self.__output_canvas.create_oval(line._Line__x_end - highlight_size,
+                                                line._Line__y_end - highlight_size,
+                                                line._Line__x_end + highlight_size,
+                                                line._Line__y_end + highlight_size,
+                                                fill=line._Line__point_highlight_color,
+                                                outline=line._Line__point_highlight_color)
+               
+               self.__output_canvas.create_oval(x_start - highlight_size,
+                                                y_start - highlight_size,
+                                                x_start + highlight_size,
+                                                y_start + highlight_size,
+                                                fill=line._Line__point_highlight_color,
+                                                outline=line._Line__point_highlight_color)
+            
    
          if re_show_data:
             self.__reshow_data()
-         self.__is_data_showing_working = False
-   
-   
+         
+         
    def __hide_pointer(self, event: tkinter.Event) -> None:
       """
       Hides the pointer widget from the GUI canvas.
 
          Args:
             event (tkinter.Event): The event triggering the pointer hiding.
       """
@@ -1661,15 +1659,15 @@
             state (bool): The hide/show state of the line.
       """
       
       Validate._isValidLine(line, "line")
       Validate._isBool(state, "state")
       if line._Line__visibility != state or self.__visibility != state:
          line._Line__visibility = state
-         self.__call_reshow_data()
+         self.__reshow_data()
       
       
    def set_lines_visibility(self, state: bool) -> None:
       """
       Hide or show all lines.
 
          Args:
@@ -1678,15 +1676,15 @@
       
       Validate._isBool(state, "state")
       self.__visibility = state
       if state == False:
          self.__output_canvas.place_forget()
       for line in self.__lines:
          line._Line__visibility = state
-      self.__call_reshow_data()
+      self.__reshow_data()
    
    
    def reset(self) -> None:
       """
       Reset the chart and lines to their initial state.
       """
       
@@ -1695,15 +1693,15 @@
       
       
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

### Comparing `tkchart-2.0.3/src/tkchart/Utils.py` & `tkchart-2.1.0/src/tkchart/Utils.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.0.3/src/tkchart/Validate.py` & `tkchart-2.1.0/src/tkchart/Validate.py`

 * *Files identical despite different names*

