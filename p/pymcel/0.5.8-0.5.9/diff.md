# Comparing `tmp/pymcel-0.5.8.tar.gz` & `tmp/pymcel-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcel-0.5.8.tar", last modified: Wed Mar  6 23:30:10 2024, max compression
+gzip compressed data, was "pymcel-0.5.9.tar", last modified: Mon Mar 11 05:19:11 2024, max compression
```

## Comparing `pymcel-0.5.8.tar` & `pymcel-0.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-06 23:30:10.239939 pymcel-0.5.8/
--rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     1073 2024-02-06 17:35:22.000000 pymcel-0.5.8/LICENSE
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     2583 2024-03-06 23:30:10.239939 pymcel-0.5.8/PKG-INFO
--rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     1988 2024-02-06 18:11:02.000000 pymcel-0.5.8/README.md
--rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     1269 2024-02-06 17:35:22.000000 pymcel-0.5.8/pyproject.toml
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       38 2024-03-06 23:30:10.239939 pymcel-0.5.8/setup.cfg
--rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     3361 2024-03-06 23:29:17.000000 pymcel-0.5.8/setup.py
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-06 23:30:10.219939 pymcel-0.5.8/src/
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-06 23:30:10.229939 pymcel-0.5.8/src/pymcel/
--rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)    34857 2024-03-06 23:26:39.000000 pymcel-0.5.8/src/pymcel/__init__.py
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-02-08 15:14:51.000000 pymcel-0.5.8/src/pymcel/attic.py
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      808 2024-02-08 16:47:57.000000 pymcel-0.5.8/src/pymcel/constantes.py
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-06 23:30:10.239939 pymcel-0.5.8/src/pymcel/data/
--rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)      594 2024-02-08 14:27:42.000000 pymcel-0.5.8/src/pymcel/data/kernels
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       21 2024-02-08 14:37:34.000000 pymcel-0.5.8/src/pymcel/export.py
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     1193 2024-02-26 16:03:49.000000 pymcel-0.5.8/src/pymcel/plot.py
--rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)       16 2024-03-06 23:29:17.000000 pymcel-0.5.8/src/pymcel/version.py
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-06 23:30:10.239939 pymcel-0.5.8/src/pymcel.egg-info/
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     2583 2024-03-06 23:30:10.000000 pymcel-0.5.8/src/pymcel.egg-info/PKG-INFO
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      401 2024-03-06 23:30:10.000000 pymcel-0.5.8/src/pymcel.egg-info/SOURCES.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        1 2024-03-06 23:30:10.000000 pymcel-0.5.8/src/pymcel.egg-info/dependency_links.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       48 2024-03-06 23:30:10.000000 pymcel-0.5.8/src/pymcel.egg-info/entry_points.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       50 2024-03-06 23:30:10.000000 pymcel-0.5.8/src/pymcel.egg-info/requires.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        7 2024-03-06 23:30:10.000000 pymcel-0.5.8/src/pymcel.egg-info/top_level.txt
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-11 05:19:11.441875 pymcel-0.5.9/
+-rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     1073 2024-02-06 17:35:22.000000 pymcel-0.5.9/LICENSE
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     2583 2024-03-11 05:19:11.441875 pymcel-0.5.9/PKG-INFO
+-rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     1988 2024-02-06 18:11:02.000000 pymcel-0.5.9/README.md
+-rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     1269 2024-02-06 17:35:22.000000 pymcel-0.5.9/pyproject.toml
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       38 2024-03-11 05:19:11.441875 pymcel-0.5.9/setup.cfg
+-rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)     3361 2024-03-11 05:18:18.000000 pymcel-0.5.9/setup.py
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-11 05:19:11.431875 pymcel-0.5.9/src/
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-11 05:19:11.441875 pymcel-0.5.9/src/pymcel/
+-rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)    37716 2024-03-11 05:11:30.000000 pymcel-0.5.9/src/pymcel/__init__.py
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-02-08 15:14:51.000000 pymcel-0.5.9/src/pymcel/attic.py
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      808 2024-02-08 16:47:57.000000 pymcel-0.5.9/src/pymcel/constantes.py
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-11 05:19:11.441875 pymcel-0.5.9/src/pymcel/data/
+-rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)      594 2024-02-08 14:27:42.000000 pymcel-0.5.9/src/pymcel/data/kernels
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       21 2024-02-08 14:37:34.000000 pymcel-0.5.9/src/pymcel/export.py
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     1193 2024-02-26 16:03:49.000000 pymcel-0.5.9/src/pymcel/plot.py
+-rwxrwxrwx   0 jzuluaga  (1000) jzuluaga  (1000)       16 2024-03-11 05:18:18.000000 pymcel-0.5.9/src/pymcel/version.py
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-03-11 05:19:11.441875 pymcel-0.5.9/src/pymcel.egg-info/
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     2583 2024-03-11 05:19:11.000000 pymcel-0.5.9/src/pymcel.egg-info/PKG-INFO
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      401 2024-03-11 05:19:11.000000 pymcel-0.5.9/src/pymcel.egg-info/SOURCES.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        1 2024-03-11 05:19:11.000000 pymcel-0.5.9/src/pymcel.egg-info/dependency_links.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       48 2024-03-11 05:19:11.000000 pymcel-0.5.9/src/pymcel.egg-info/entry_points.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       50 2024-03-11 05:19:11.000000 pymcel-0.5.9/src/pymcel.egg-info/requires.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        7 2024-03-11 05:19:11.000000 pymcel-0.5.9/src/pymcel.egg-info/top_level.txt
```

### Comparing `pymcel-0.5.8/LICENSE` & `pymcel-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcel-0.5.8/PKG-INFO` & `pymcel-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcel
-Version: 0.5.8
+Version: 0.5.9
 Summary: Utilidades de Mecánica Celeste
 Home-page: https://pypi.org/project/pymcel
 Author: Jorge I. Zuluaga
 Author-email: jorge.zuluaga@udea.edu.co
 License: MIT
 Keywords: astronomy astrodynamics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymcel-0.5.8/README.md` & `pymcel-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pymcel-0.5.8/pyproject.toml` & `pymcel-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymcel-0.5.8/setup.py` & `pymcel-0.5.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         ],
-    version='0.5.8',
+    version='0.5.9',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `pymcel-0.5.8/src/pymcel/__init__.py` & `pymcel-0.5.9/src/pymcel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,57 +250,70 @@
         y_range = abs(rangos[1][1] - rangos[1][0])
         y_middle = (rangos[1][1] + rangos[1][0])/2
         z_range = abs(rangos[2][1] - rangos[2][0])
         z_middle = (rangos[2][1] + rangos[2][0])/2
 
     # The plot bounding box is a sphere in the sense of the infinity
     # norm, hence I call half the max range the plot radius.
-    plot_radius = 0.5*max([x_range, y_range, z_range])
+    plot_radius = 0.55*max([x_range, y_range, z_range])
     
     ax.set_xlim3d([x_middle - plot_radius, x_middle + plot_radius])
     ax.set_ylim3d([y_middle - plot_radius, y_middle + plot_radius])
     ax.set_zlim3d([z_middle - plot_radius, z_middle + plot_radius])
 
     return ax.get_xlim3d(),ax.get_ylim3d(),ax.get_zlim3d()
 
 def plot_ncuerpos_3d(rs,vs,tipo='matplotlib',**opciones):
 
     #Número de partículas
     N=rs.shape[0]
 
-    if tipo == 'matplotlib':  
+    if tipo == 'matplotlib':
+
+        opciones_defecto = dict(lw=1)
+        opciones_defecto.update(opciones)
+
         fig=plt.figure()
         ax=fig.add_subplot(111,projection='3d')
 
         for i in range(N):
-            ax.plot(rs[i,:,0],rs[i,:,1],rs[i,:,2],**opciones);
+            ax.plot(rs[i,:,0],rs[i,:,1],rs[i,:,2],**opciones_defecto);
 
         fija_ejes3d_proporcionales(ax);
         fig.tight_layout();
         plt.show();
         return fig
 
     elif tipo == 'plotly':
 
+        opciones_defecto = dict(
+            mode='lines',
+            name='Cuerpo',
+            marker=dict(),
+            line=dict(),
+        )
+        opciones_defecto.update(opciones)
+
         try:
             import plotly.graph_objects as go
         except:
             print("Debes instalar primero plotly en tu sistema: pip install -Uq plotly")
             return None
 
         fig = go.Figure()
         for i in range(N):
             xs = rs[i,:,0]
             ys = rs[i,:,1]
             zs = rs[i,:,2]
             fig.add_trace(
                 go.Scatter3d(
                     x=xs, y=ys, z=zs,
-                    mode='lines',
-                    name=f"Cuerpo {i}"
+                    mode=opciones_defecto['mode'],
+                    name=opciones_defecto['name']+f" {i}",
+                    marker=opciones_defecto['marker'],
                 )
             )
         rmin = rs.min()
         rmax = rs.max()
 
         rangos = encuentra_rangos(rs)
         fig['layout']['scene']['aspectmode'] = 'cube'
@@ -308,55 +321,73 @@
             fig['layout']['scene'][axis]['range'] = rangos[i]
         fig.show()
     else:
         raise AssertionError(f"Tipo de gráfico '{tipo}' no reconocido")
 
     return fig
 
-def plot_doscuerpos_3d(rs,vs,tipo='matplotlib',**opciones):
+from scipy.interpolate import interp1d
+def plot_doscuerpos_3d(rs,vs,tipo='matplotlib',ts=None,**opciones):
 
     #Número de partículas
     N=rs.shape[0]
-    opciones_defecto = dict(color='k',lw=1)
-    opciones_defecto.update(opciones)
 
+    if ts is not None:
+        xfun = interp1d(ts,rs[:,0],kind='cubic')
+        yfun = interp1d(ts,rs[:,1],kind='cubic')
+        zfun = interp1d(ts,rs[:,2],kind='cubic')
+        tss = np.linspace(ts[0],ts[-1],10*len(ts))
+        rs = np.array([[xfun(t),yfun(t),zfun(t)] for t in tss])
+        print(rs.shape)
+        
     if tipo == 'matplotlib':  
+    
+        opciones_defecto = dict(color='k',lw=1)
+        opciones_defecto.update(opciones)
+    
         fig=plt.figure()
         ax=fig.add_subplot(111,projection='3d')
 
-        for i in range(N):
-            ax.plot(rs[:,0],rs[:,1],rs[:,2],**opciones_defecto);
+        ax.plot(rs[:,0],rs[:,1],rs[:,2],**opciones_defecto);
 
         rangos = encuentra_rangos(rs)
         fija_ejes3d_proporcionales(ax,rangos);
 
         fig.tight_layout();
         plt.show();
         return fig
 
     elif tipo == 'plotly':
+        
+        opciones_defecto = dict(
+            mode='lines',
+            name='Vector relativo',
+            marker=dict(color='Black'),
+            line=dict(color='Black'),
+        )
+        opciones_defecto.update(opciones)
 
         try:
             import plotly.graph_objects as go
         except:
             print("Debes instalar primero plotly en tu sistema: pip install -Uq plotly")
             return None
 
         fig = go.Figure()
-        for i in range(N):
-            xs = rs[:,0]
-            ys = rs[:,1]
-            zs = rs[:,2]
-            fig.add_trace(
-                go.Scatter3d(
-                    x=xs, y=ys, z=zs,
-                    mode='lines',
-                    name=f"Cuerpo {i}"
-                )
+        xs = rs[:,0]
+        ys = rs[:,1]
+        zs = rs[:,2]
+        fig.add_trace(
+            go.Scatter3d(
+                x=xs, y=ys, z=zs,
+                mode=opciones_defecto['mode'],
+                name=opciones_defecto['name'],
+                marker=opciones_defecto['marker'],
             )
+        )
         rmin = rs.min()
         rmax = rs.max()
 
         rangos = encuentra_rangos(rs)
         fig['layout']['scene']['aspectmode'] = 'cube'
         for i,axis in enumerate(['xaxis','yaxis','zaxis']):
             fig['layout']['scene'][axis]['range'] = rangos[i]
@@ -1287,7 +1318,100 @@
         Dn=abs(dE/Emed)
         n+=1
     return En,Dn,n
 
 def serie_stumpff(t,k,N=15):
     sk=lambda n:t/((2*n+k+1)*(2*n+k+2))*(1-sk(n+1)) if n<N else 0
     return (1-sk(0))/math.factorial(k)
+
+def plot_elipse(e=0.5):
+    a=10.0
+    e=float(e)
+    b=a*sqrt(1-e**2)
+
+    #Distancia foco-centro
+    c=a*e
+
+    #Máximo valor de x
+    xcmax=a
+
+    #Valores de x en los que graficaremos
+    xcs=linspace(-a,a,100)
+
+    #Ecuaciones de las cónicas referidas al apside
+    ycs_cir=a*sqrt(1-xcs**2/a**2)
+    ycs=b*sqrt(1-xcs**2/a**2)
+
+    #Gráfica
+    import matplotlib.pyplot as plt
+    fig=plt.figure(figsize=(6,6))
+    ax=fig.gca()
+
+    ax.plot(xcs,ycs_cir,'k--')
+    ax.plot(xcs,-ycs_cir,'k--')
+    ax.plot(xcs,ycs,'r')
+    ax.plot(xcs,-ycs,'r')
+
+    #Graficar la posición del foco y el centro
+    ax.plot([-c],[0],'bx',markersize=10)
+    ax.plot([0],[0],'ko',markersize=5)
+
+    #Decoración
+    ax.grid()
+    ax.set_title(f"Elipse con $a = {a}$, $e={e}$")
+
+    #Fijamos la misma escala en los ejes
+    plt.axis("equal")
+    plt.show()
+
+#Definimos el algoritmo como una rutina
+def plot_hiperbola(e=1.5):
+
+    #Semieje mayor
+    a=-10.0
+
+    #Forma
+    e=float(e)
+
+    #Semieje menor
+    beta=abs(a)*sqrt(e**2-1)
+
+    #Semilatus rectum
+    p=a*(1-e**2)
+
+    #Posición del foco
+    q=p/(1+e)
+    F=abs(a)+q
+
+    #Máximo valor de x
+    xcmax=3*abs(a)
+
+    #Valores de x en los que graficaremos
+    xcs=linspace(abs(a),xcmax,100)
+
+    #Ecuaciones de las cónicas referidas al apside
+    ycs=beta*sqrt(xcs**2/a**2-1)
+
+    #Ecuación de las asintotas
+    xas=linspace(0,xcmax,100)
+    ycs_asi=beta*xas/abs(a)
+
+    #Gráfica
+    fig=plt.figure(figsize=(6,6))
+    ax=fig.gca()
+
+    ax.plot(xas,ycs_asi,'k--')
+    ax.plot(xas,-ycs_asi,'k--')
+    ax.plot(xcs,ycs,'r')
+    ax.plot(xcs,-ycs,'r')
+
+    #Graficar la posición del foco y el vértice
+    ax.plot([F],[0],'bx',markersize=10)
+    ax.plot([0],[0],'ko',markersize=5)
+
+    #Decoración
+    ax.grid()
+    ax.set_title(f"Hipérbola con $a = {a}$, $e={e}$")
+
+    #Fijamos la misma escala en los ejes
+    plt.axis("equal")
+    plt.show()
```

### Comparing `pymcel-0.5.8/src/pymcel/constantes.py` & `pymcel-0.5.9/src/pymcel/constantes.py`

 * *Files identical despite different names*

### Comparing `pymcel-0.5.8/src/pymcel/data/kernels` & `pymcel-0.5.9/src/pymcel/data/kernels`

 * *Files identical despite different names*

### Comparing `pymcel-0.5.8/src/pymcel/plot.py` & `pymcel-0.5.9/src/pymcel/plot.py`

 * *Files identical despite different names*

### Comparing `pymcel-0.5.8/src/pymcel.egg-info/PKG-INFO` & `pymcel-0.5.9/src/pymcel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcel
-Version: 0.5.8
+Version: 0.5.9
 Summary: Utilidades de Mecánica Celeste
 Home-page: https://pypi.org/project/pymcel
 Author: Jorge I. Zuluaga
 Author-email: jorge.zuluaga@udea.edu.co
 License: MIT
 Keywords: astronomy astrodynamics
 Classifier: Programming Language :: Python :: 3
```

