# Comparing `tmp/fremake_canopy-0.1.1.tar.gz` & `tmp/fremake_canopy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fremake_canopy-0.1.1.tar", last modified: Tue Apr  2 18:44:45 2024, max compression
+gzip compressed data, was "fremake_canopy-0.1.2.tar", last modified: Thu Apr  4 19:00:05 2024, max compression
```

## Comparing `fremake_canopy-0.1.1.tar` & `fremake_canopy-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-02 18:44:46.888392 fremake_canopy-0.1.1/
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     7642 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/LICENSE.md
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       59 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/MANIFEST.in
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      280 2024-04-02 18:44:46.881311 fremake_canopy-0.1.1/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     2382 2024-03-27 16:46:30.000000 fremake_canopy-0.1.1/README.md
-drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-02 18:44:46.866140 fremake_canopy-0.1.1/fremake_canopy.egg-info/
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      280 2024-04-02 18:44:46.000000 fremake_canopy-0.1.1/fremake_canopy.egg-info/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      469 2024-04-02 18:44:46.000000 fremake_canopy-0.1.1/fremake_canopy.egg-info/SOURCES.txt
--rw-r--r--   0 Bennett.Chang (21243) f           (70)        1 2024-04-02 18:44:46.000000 fremake_canopy-0.1.1/fremake_canopy.egg-info/dependency_links.txt
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       27 2024-04-02 18:44:46.000000 fremake_canopy-0.1.1/fremake_canopy.egg-info/requires.txt
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       13 2024-04-02 18:44:46.000000 fremake_canopy-0.1.1/fremake_canopy.egg-info/top_level.txt
-drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-02 18:44:46.849966 fremake_canopy-0.1.1/gfdl_fremake/
--rw-r--r--   0 Bennett.Chang (21243) f           (70)        0 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/gfdl_fremake/__init__.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     4463 2024-04-02 18:34:19.000000 fremake_canopy-0.1.1/gfdl_fremake/buildBaremetal.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     7919 2024-04-02 18:34:39.000000 fremake_canopy-0.1.1/gfdl_fremake/buildDocker.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     5780 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/gfdl_fremake/checkout.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     7672 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/gfdl_fremake/makefilefre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     4381 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/gfdl_fremake/platformfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     2367 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/gfdl_fremake/targetfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     2493 2024-04-02 18:02:51.000000 fremake_canopy-0.1.1/gfdl_fremake/varsfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     5798 2024-04-02 18:33:14.000000 fremake_canopy-0.1.1/gfdl_fremake/yamlfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       38 2024-04-02 18:44:46.893448 fremake_canopy-0.1.1/setup.cfg
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      400 2024-04-02 18:41:46.000000 fremake_canopy-0.1.1/setup.py
+drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-04 19:00:44.906262 fremake_canopy-0.1.2/
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     7642 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/LICENSE.md
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)       59 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/MANIFEST.in
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)      280 2024-04-04 19:00:44.899171 fremake_canopy-0.1.2/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     2382 2024-03-27 16:46:30.000000 fremake_canopy-0.1.2/README.md
+drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-04 19:00:44.879930 fremake_canopy-0.1.2/fremake_canopy.egg-info/
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)      280 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)      469 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/SOURCES.txt
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)        1 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/dependency_links.txt
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)       27 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/requires.txt
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)       13 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/top_level.txt
+drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-04 19:00:44.870793 fremake_canopy-0.1.2/gfdl_fremake/
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)      173 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/__init__.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     4475 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/buildBaremetal.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     7968 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/buildDocker.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     5780 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/checkout.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     7576 2024-04-04 18:35:05.000000 fremake_canopy-0.1.2/gfdl_fremake/makefilefre.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     4381 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/platformfre.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     2367 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/targetfre.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     2493 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/varsfre.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)     6030 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/yamlfre.py
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)       38 2024-04-04 19:00:44.907274 fremake_canopy-0.1.2/setup.cfg
+-rw-r--r--   0 Bennett.Chang (21243) f           (70)      400 2024-04-04 18:59:35.000000 fremake_canopy-0.1.2/setup.py
```

### Comparing `fremake_canopy-0.1.1/LICENSE.md` & `fremake_canopy-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.1/README.md` & `fremake_canopy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/buildBaremetal.py` & `fremake_canopy-0.1.2/gfdl_fremake/buildBaremetal.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 def fremake_parallel(fremakeBuildList):
 	fremakeBuildList.run()
 
 class buildBaremetal():
 ## \brief Creates the build script to compile the model
 ## \param self The buildScript object
 ## \param exp The experiment name
-## \param mkTemplate The template used by mkmf to compile the model
+## \param mkTemplatePath The template used by mkmf to compile the model
 ## \param srcDir The source directory
 ## \param bldDir The build directory
 ## \param modules The list of modules to load before compilation
 ## \param modulesInit A list of commands with new line characters to initialize modules
- def __init__(self,exp,mkTemplate,srcDir,bldDir,target,modules,modulesInit,jobs):
+ def __init__(self,exp,mkTemplatePath,srcDir,bldDir,target,modules,modulesInit,jobs):
      self.e = exp
      self.t = target.gettargetName()
      self.src = srcDir
      self.bld = bldDir
      self.make = "make --jobs="+str(jobs)+" "+target.getmakeline_add() #make line
      self.mkmf = True
-     self.template = mkTemplate
+     self.template = mkTemplatePath
      self.modules = ""
      for m in modules:
           self.modules = self.modules +" "+ m
 ## Set up the top portion of the compile script
      self.setup=[   "#!/bin/sh -fx \n",
                     "bld_dir="+self.bld+"/ \n",
                     "src_dir="+self.src+"/ \n",
```

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/buildDocker.py` & `fremake_canopy-0.1.2/gfdl_fremake/buildDocker.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 import os
 import targetfre
 
 class container():
 ## \brief Opens the Dockerfile for writing
 ## \param self The dockerfile object
-## \param base the docker base image to start from
+## \param base The docker base image to start from
+## \param libs Additional libraries defined by user 
 ## \param exp The experiment name
 ## \param RUNenv The commands that have to be run at the beginning of a RUN in the dockerfile
 ## to set up the environment
- def __init__(self,base,exp,addlibs,RUNenv,target):
-     self.base=base
+ def __init__(self,base,exp,libs,RUNenv,target):
+     self.base = base
      self.e = exp
-     self.l = addlibs
+     self.l = libs
      self.src = "/apps/"+self.e+"/src"
      self.bld = "/apps/"+self.e+"/exec"
      self.mkmf = True
      self.target = target
      self.template = "/apps/mkmf/templates/hpcme-intel21.mk"
      if RUNenv == "":
            self.setup = ["RUN \\ \n"]
```

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/checkout.py` & `fremake_canopy-0.1.2/gfdl_fremake/checkout.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/makefilefre.py` & `fremake_canopy-0.1.2/gfdl_fremake/makefilefre.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 import os
 import subprocess
+import textwrap
 
 ## \brief Writes the link line for bare metal and container builds 
 ## \param self The Makefile object
 def linklineBuild(self):
+    linkline=""
 #if additional libraries are defined, populate the link line with the correct information for libraries
 ## CONTAINER; write a script that will execute in the container, to fill in link line with additional libraries in Makefile
-    if "tmp" in self.filePath and self.l != None:
+    if "tmp" in self.filePath:
         with open(self.filePath+"/linkline.sh","a") as fh:
             fh.write("set -- ")
             for l in self.l:
                 fh.write(l+" ")
             fh.write("\n")
             
-        self.linklinecreate = ["line=''\n",
-                               "for l in $@; do\n",
-                               "    loc=$(spack location -i $l)\n",
-                               "    libraries=$(ls $loc/lib)\n",
-                               '    if echo "$libraries" | grep -q "_d"; then\n',
-                               "        for i in $libraries; do\n",
-                               '            if [ "$i" != "cmake" ] && echo "$i" | grep -q "_d"; then \n',
-                               "                ln1=${i%.*}\n",
-                               "                ln2=${ln1#???}\n",
-                               '                line=$line" -L$loc/lib -l$ln2"\n',
-                               "            fi\n",
-                               "        done\n",
-                               "    else\n",
-                               "        for i in $libraries; do\n",
-                               '            if [ "$i" != "cmake" ]; then\n',
-                               "                ln1=${i%.*}\n",
-                               "                ln2=${ln1#???}\n",
-                               '                line=$line" -L$loc/lib -l$ln2"\n',
-                               "            fi\n",
-                               "        done\n",
-                               "    fi\n",
-                               "done\n\n",
-                               "MF_PATH='/apps/"+self.e+"/exec/Makefile'\n",
-                               'sed -i "/MK_TEMPLATE = /a LL = $line" $MF_PATH\n',
-                               "sed -i 's|\($^\) \($(LDFLAGS)\)|\\1 $(LL) \\2|' $MF_PATH\n"]
+        self.linklinecreate = '''
+                               line=''
+                               for l in $@; do
+                                   loc=$(spack location -i $l)
+                                   libraries=$(ls $loc/lib)
+                                   if echo "$libraries" | grep -q "_d"; then
+                                       for i in $libraries; do
+                                           if [ "$i" != "cmake" ] && echo "$i" | grep -q "_d"; then
+                                               ln1=${i%.*}
+                                               ln2=${ln1#???}
+                                               line=$line" -L$loc/lib -l$ln2"
+                                           fi
+                                       done
+                                   else
+                                       for i in $libraries; do
+                                           if [ "$i" != "cmake" ]; then
+                                               ln1=${i%.*}
+                                               ln2=${ln1#???}
+                                               line=$line" -L$loc/lib -l$ln2"
+                                           fi
+                                       done
+                                   fi
+                               done
+                               '''
 
         with open(self.filePath+"/linkline.sh","a") as fh:
-            fh.writelines(self.linklinecreate)
+            fh.writelines(textwrap.dedent(self.linklinecreate))
+            fh.write("MF_PATH='/apps/"+self.e+"/exec/Makefile'\n")
+            fh.write('sed -i "/MK_TEMPLATE = /a LL = $line" $MF_PATH\n')
+            fh.write("sed -i 's|\($^\) \($(LDFLAGS)\)|\\1 $(LL) \\2|' $MF_PATH\n")
 
-#TO-DO: HAVE TO ADD SPACK LOCATION FOR SPACK INSTALLED LIBRARIES ON BARE METAL
 ## BARE METAL; if addlibs defined on bare metal, include those additional libraries in link line
-    elif "tmp" not in self.filePath and self.l != None:
-        linkline=""
-        for l in self.l:
-            # Write link line
-            linkline = linkline+' $(pkg-config --libs '+l+') '
-        
-        #Write to Makefile
-        os.system('sed -i "/MK_TEMPLATE = /a LL = '+linkline+'" '+self.filePath+'/Makefile'+'\n')
-        os.system("sed -i 's|\($^\) \($(LDFLAGS)\)|\\1 $(LL) \\2|' "+self.filePath+'/Makefile'+'\n')
+    elif "tmp" not in self.filePath:
+        for l in self.l: # baremetal_linkerflags
+            linkline = linkline + " " + l
+        os.system(f"sed -i '/MK_TEMPLATE = /a LL = {linkline}' {self.filePath}/Makefile")
+        os.system(f"sed -i 's|\($(LDFLAGS)\)|$(LL) \\1|' {self.filePath}/Makefile")
 
 class makefile():
 ## \brief Opens Makefile and sets the experiment and other common variables
 ## \param self The Makefile object
 ## \param exp Experiment name
+## \param libs Additional libraries/linker flags defined by user
 ## \param srcDir The path to the source directory
 ## \param bldDir The path to the build directory
-## \param mkTemplate The path of the template .mk file for compiling
- def __init__(self,exp,addlibs,srcDir,bldDir,mkTemplate):
+## \param mkTemplatePath The path of the template .mk file for compiling
+ def __init__(self,exp,libs,srcDir,bldDir,mkTemplatePath):
      self.e = exp
-     self.l = addlibs
+     self.l = libs
      self.src = srcDir 
      self.bld =  bldDir
-     self.template = mkTemplate
+     self.template = mkTemplatePath
      self.c =[] #components
      self.r=[] #requires
      self.o=[] #overrides
      os.system("mkdir -p "+self.bld)
      self.filePath = self.bld # Needed so that the container and bare metal builds can
                               # use the same function to create the Makefile
 
@@ -110,16 +110,17 @@
        fh.write("MK_TEMPLATE = "+self.template+"\n") 
        fh.write("include $(MK_TEMPLATE)"+"\n")
 # Write the main experiment compile 
        fh.write(self.e+".x: "+libstring+"\n")
        fh.write("\t$(LD) $^ $(LDFLAGS) -o $@ $(STATIC_LIBS)"+"\n")
 
 # Write the link line script with user-provided libraries 
-     linklineBuild(self)  
-    
+     if self.l:
+       linklineBuild(self)
+
 # Write the individual component library compiles
      with open(self.filePath+"/Makefile","a") as fh:
        for (c,r,o) in sd:
             libstring = " "
             for lib in r:
                  libstring = libstring+lib+"/lib"+lib+".a "
             cstring = c+"/lib"+c+".a: "
@@ -145,25 +146,26 @@
        fh.write("\t$(RM) -r "+self.e+"\n")
        fh.write("\t$(RM) -r Makefile \n")
 
 ### This seems incomplete? ~ ejs
 ## The makefile class for a container.  It gets built into a temporary directory so it can be copied
 ## into the container.
 ## \param exp Experiment name
+## \param libs Additional libraries/linker flags defined by user
 ## \param srcDir The path to the source directory
 ## \param bldDir The path to the build directory
-## \param mkTemplate The path of the template .mk file for compiling
+## \param mkTemplatePath The path of the template .mk file for compiling
 ## \param tmpDir A local path to temporarily store files build to be copied to the container
 class makefileContainer(makefile):
-  def __init__(self,exp,addlibs,srcDir,bldDir,mkTemplate,tmpDir):
+  def __init__(self,exp,libs,srcDir,bldDir,mkTemplatePath,tmpDir):
     self.e = exp
-    self.l = addlibs
+    self.l = libs
     self.src = srcDir 
     self.bld =  bldDir
-    self.template = mkTemplate
+    self.template = mkTemplatePath
     self.tmpDir = tmpDir
     self.c =[] #components
     self.r=[] #requires
     self.o=[] #overrides
     os.system("mkdir -p "+self.tmpDir)
     self.filePath = self.tmpDir # Needed so that the container and bare metal builds can
                                 # use the same function to create the Makefile
```

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/platformfre.py` & `fremake_canopy-0.1.2/gfdl_fremake/platformfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/targetfre.py` & `fremake_canopy-0.1.2/gfdl_fremake/targetfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/varsfre.py` & `fremake_canopy-0.1.2/gfdl_fremake/varsfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.1/gfdl_fremake/yamlfre.py` & `fremake_canopy-0.1.2/gfdl_fremake/yamlfre.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,19 +39,24 @@
      ## Check the yaml for required things
      ## Check for required experiment name
      try:
           self.yaml["experiment"]
      except:
           print("You must set an experiment name to compile \n")
           raise
-     ## Check for optional libraries and packages for linking
+     ## Check for optional libraries and packages for linking in container
      try: 
-          self.yaml["addlibs"]
+          self.yaml["container_addlibs"]
      except:
-          self.yaml["addlibs"]=""
+          self.yaml["container_addlibs"]=""
+     ## Check for optional libraries and packages for linking on bare-metal system
+     try:
+          self.yaml["baremetal_linkerflags"]
+     except:
+          self.yaml["baremetal_linkerflags"]=""
 #     ## Set up the srcDir
 #     self.src = modelRoot + "/" + self.yaml["experiment"] + "/src"
      ## Check for required src
      try:
           self.yaml["src"]
      except:
           print("You must set a src to specify the sources in "+self.yaml["experiment"]+"\n")
```

