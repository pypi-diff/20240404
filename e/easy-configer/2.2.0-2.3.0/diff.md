# Comparing `tmp/easy_configer-2.2.0.tar.gz` & `tmp/easy_configer-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_configer-2.2.0.tar", last modified: Wed Oct 11 14:32:42 2023, max compression
+gzip compressed data, was "dist/easy_configer-2.3.0.tar", last modified: Thu Apr  4 09:05:37 2024, max compression
```

## Comparing `easy_configer-2.2.0.tar` & `easy_configer-2.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2023-10-11 14:32:42.252899 easy_configer-2.2.0/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    20289 2023-10-11 14:32:42.250889 easy_configer-2.2.0/PKG-INFO
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    19700 2023-10-11 14:31:37.000000 easy_configer-2.2.0/README.md
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2023-10-11 14:32:42.164977 easy_configer-2.2.0/easy_configer/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    13595 2023-10-11 14:24:49.000000 easy_configer-2.2.0/easy_configer/Configer.py
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     4614 2023-10-11 14:24:49.000000 easy_configer-2.2.0/easy_configer/IO_Converter.py
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2023-10-11 14:32:42.229485 easy_configer-2.2.0/easy_configer/utils/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)      807 2023-10-11 14:24:49.000000 easy_configer-2.2.0/easy_configer/utils/Flag.py
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     4801 2023-10-11 14:24:49.000000 easy_configer-2.2.0/easy_configer/utils/Type_Convertor.py
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2023-10-11 14:32:42.201802 easy_configer-2.2.0/easy_configer.egg-info/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    20289 2023-10-11 14:32:42.000000 easy_configer-2.2.0/easy_configer.egg-info/PKG-INFO
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)      288 2023-10-11 14:32:42.000000 easy_configer-2.2.0/easy_configer.egg-info/SOURCES.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)        1 2023-10-11 14:32:42.000000 easy_configer-2.2.0/easy_configer.egg-info/dependency_links.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)       34 2023-10-11 14:32:42.000000 easy_configer-2.2.0/easy_configer.egg-info/top_level.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)       38 2023-10-11 14:32:42.252899 easy_configer-2.2.0/setup.cfg
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     1057 2023-10-11 14:32:35.000000 easy_configer-2.2.0/setup.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:05:39.207001 easy_configer-2.3.0/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21584 2024-04-04 09:05:39.205013 easy_configer-2.3.0/PKG-INFO
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    20995 2024-04-04 09:03:21.000000 easy_configer-2.3.0/README.md
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:05:39.130000 easy_configer-2.3.0/easy_configer/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    14856 2024-04-04 09:04:41.000000 easy_configer-2.3.0/easy_configer/Configer.py
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     5021 2024-04-04 09:04:41.000000 easy_configer-2.3.0/easy_configer/IO_Converter.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:05:39.191013 easy_configer-2.3.0/easy_configer/utils/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     2059 2024-04-04 09:04:41.000000 easy_configer-2.3.0/easy_configer/utils/Container.py
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     4801 2024-04-04 09:04:41.000000 easy_configer-2.3.0/easy_configer/utils/Type_Convertor.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:05:39.169017 easy_configer-2.3.0/easy_configer.egg-info/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21584 2024-04-04 09:05:38.000000 easy_configer-2.3.0/easy_configer.egg-info/PKG-INFO
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)      293 2024-04-04 09:05:39.000000 easy_configer-2.3.0/easy_configer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)        1 2024-04-04 09:05:38.000000 easy_configer-2.3.0/easy_configer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)       34 2024-04-04 09:05:38.000000 easy_configer-2.3.0/easy_configer.egg-info/top_level.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)       38 2024-04-04 09:05:39.208000 easy_configer-2.3.0/setup.cfg
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     1057 2024-04-04 09:03:56.000000 easy_configer-2.3.0/setup.py
```

### Comparing `easy_configer-2.2.0/PKG-INFO` & `easy_configer-2.3.0/easy_configer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
-Name: easy_configer
-Version: 2.2.0
+Name: easy-configer
+Version: 2.3.0
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Keywords: configuration,commendline argument,argument
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Project description
-#### easy_configer version : 2.2.0
+#### easy_configer version : 2.3.0
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
-![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
+![easy-configer logo](assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
 I'm willing to provide a light-weight solution for configurating your python program. Hope this repository make every user control their large project more easier ~ ~ 
 
 ### Introduction 📝
@@ -46,79 +47,68 @@
     parse.add_argument("--lucky_num", type=int)
     ...
     args = parser.parse_args()
     args.lucky_num
     
 
 That leverage me to package my solution for solving this issue. The easy_config will cover the following attributes :
-
-1. **simple & customized syntax of declaration (partially support)**
+1. **Hierachical section config (nested dictionary)**
 
 2. **Accept multiple config file in dynamic loading manner**
 
-3. **Declare customized class instance in the config file**
+3. **Support customized class (initialized by keyword arguments)**
 
 4. **Commend-line update all declared-value wherever it belong, even in hierachical section**
 
-5. **Support the absl style FLAGS functionality** 
-
-6. **Omegaconf like hierachical config**
+5. **Support the absl style FLAGS functionality (declare once, use anywhere)** 
 
 And, of course the following attribute will also be supported :
 
-* dot-access of any default argument (flatten argument)
-
-* dict-access of any section argument (non-flatten argument) 
-
-* commend-line update any argument value (flatten & non-flatten argument)
-
-* add different settings while choosing to overload previous one.
+* dot-access of any arguments (even in nested dictionary)
 
 * inline comment '#', now you can write comment in everyline ~
 
 * support arguments interpolation!!
 
-* support config conversion, which bridge the easy_config into the other config file ~
+* support config conversion, which turn easy_config into the other kind of config package (omegaconf, argparse, ..., etc.)
 
 * support hierachical configurating system with dynamic override ~
+
 ---
 
 ### Newly update features 🚀
-1. Better syntax for override argument via commendline
-2. Better syntax for declare the config file
-3. Various support of config conversion, including omegaconf, dataclasses, dict, ..., etc.
-4. Support enviroment variable (os.Env) interpolation
-5. Dynamic sub-config loading..
-6. Also update document and some handy examples ~
+1. Enable all test case (automatically ci by git-action)
+2. Support dot-access of any arguments
+3. Consistent import syntax.. 
+4. New document is released ~
 
 ---
 
 ### Bug Fixed 🐛
-#### config string with extra space caused config error, and it's fixed in this version.
+#### Fix-up import syntax.. plz open an issue if you find a bug ~
 ---
 
 ### Dependencies 🏗️
 This package is written for Python 3.8. After refactor in this version, this package also support down to python 3.6!!
 Of course, light-weight solution **do not** contain any 3-rd package complex dependencies.
 The python standard package (such as pathlib, sys, .., etc) is the only source of dependencies, so you don't need to worry about that ~ ~
 > However, if you want to use the IO_Converter for converting config into omegaconf, you still need to install omegaconf for this functionality ~
 
 ---
 
 ### Installation ⚙️<br>
 1. **pypi install** <br>
     simply type the `pip install easy_configer` (due to name conflict of pypi pkg, we use different pkg name)
+
 2. **install from source code** <br>
     clone the project from github : `git clone repo-link` 
     Chage to the root directory of the cloned project, and type `pip install -e .`
+
 3. **import syntax** <br>
-    Because of the name conflict of pypi pkg, i choice the different pkg name.
-    To import the installed pkg, the syntax will be depended on the install method. For example. <br>
-    Pip install : `from easy_configer.Configer import Configer` <br>
-    git clone & pip install : `from easy_config.Configer import Configer` <br>
+    Wherever you install, pypi or source. Now, you just need a simple import : `from easy_configer.Configer import Configer`
     
 ---
 
 ### Quick start 🥂
 
 #### **1. Handy example of config file**
 #### Let's say we have an easy-config for development enviroment on jupyter notebook. we want to define several variable for configurating a simple math calculation.
@@ -207,24 +197,29 @@
 
         ... # loading llm model instance `Llama` ~
         llm_mod = Llama(
             ld_8bit=cfger.bknd_srv.load_8bit, 
             chat_mode=cfger.chat_mode, 
             model_type=cfger.model_type
         )
-        llm_mod.init_mod_param( **cfger.bknd_srv['mod_params'] )
 
+        # you can access nested-dict by dot access ~
+        llm_mod.init_mod_param( **cfger.bknd_srv.mod_params )
+
+        # or you can keep the dict fashion ~
         if cfger.bknd_srv['async_req']:
             chat_serv.chat_mod = llm_mod
             chat_serv.hist_db = mongo_serv
         else:
             ... # write sync conversation by yourself..
 
         sys.exit( chat_serv.server_forever() )
 
+> Note that the recommended way to access the argument is **still** key-string access `cfger.args['#4$%-var']`, as you may notice, dot-access doesn't support **ugly** variable name. 
+
 <br>
 
 ---
 
 ### More detail tutorial about each topic is as follows :
 
 #### **2. How to declare hierachical config**
@@ -267,16 +262,19 @@
         
         # omit cfg_from_str, hier-config also could be declared in str though ~
         cfger.cfg_from_ini("./hier_cfg.ini")
         
         print(cfger.dataset)  
         # output nested dict : { 'service_port':65536, 'path':'/data/kitti', 'loader':{'batch_size':32} }
         
-        print(cfger.dataset['loader']['batch_size'])
-        # output : 32
+        print(f"key-string access bz : {cfger.dataset['loader']['batch_size']}")
+        # output - "key-string access bz : 32"
+
+        print(f"bz : {cfger.dataset.loader.batch_size}")
+        # output - "dot-access bz : 32"
 
         # we usually conduct initialization such simple & elegant!
         ds = build_dataset(**cfger.dataset)
         mod = build_model(**cfger.model)
         ... # get torch Trainer
         Trainer(mod).fit(ds)
 
@@ -322,16 +320,42 @@
         cfger = Configer(description="sample for arguments interpolation")
         cfger.regist_cnvtor("pyPath", Path)  # regist customer class 'Path'
 
         cfg_str = get_str_cfg()
         cfger.cfg_from_str(cfg_str)
         # do whatever you want to do!
         
+#### **3. Access all arguments flexibly**
+We simple set a breakpoint to feel how flexible does `easy_configer.utils.Container.AttributeDict` support.
 
-#### **3. Commmend-line Support**
+    from easy_configer.Configer import Configer
+    
+    if __name__ == "__main__":
+        cfger = Configer()
+        cfger.cfg_from_ini("./hier_cfg.ini")
+        breakpoint()
+
+> We write a special example `hier_cfg.ini`!!
+    # nested-dict
+    [secA] # test depth ((sub^4)-section under secA)
+        lev = 1
+        [secA.secB]
+            lev = 2
+            [secA.secB.secC]
+                lev = 3
+                [secA.secB.secC.secD]
+                    lev = 4
+
+Now you can access each `lev` :
+1. `(pdb) cfger.secA.lev `, output `lev : 1`
+2. `(pdb) cfger['secA'].secB['lev'] `, output `lev : 2`, and so on..
+3. Most crazy one ~ `(pdb) cfger.secA.['secB'].secC['secD'].lev `, output `lev : 4`
+
+
+#### **4. Commmend-line Support**
 > We also take `hier_cfg.ini` as example!
 
     # hier_cfg.ini
     glb_var = 42@int
     [dataset]         
         ds_type = None
         path = {'root':'/data/kitti'}@Path
@@ -348,15 +372,15 @@
 
 Especially update **non-flatten argument**, you can access any argument at any level by dot-access in commend-line!! (with combining any argument update). Now, try to change any nested argument <br>
 `python quick_hier.py dataset.ds_type="'kitti'" dataset.path="{'path':'/root/ds'}" dataset.loader.batch_size=48`
 
 ( Note that the commendline declaration for string is tricky, but currently we only support two way for that : 
     `dataset.ds_type="'kitti'"` or `dataset.ds_type=kitti@str`, pick up one of you like ~ )
 
-#### **4. Import Sub-Config**
+#### **5. Import Sub-Config**
 Like `omegaconf`, most of user expect to seperate the config based on their type and dynamically merge it in runtime. It's a rational requirement and the previous version of easy-config provide two way to conduct it, but both have it's limit : 
 1. you can call the `cfg_from_ini` twice, for example, `cfg.cfg_from_ini('./base_cfg') ; cfg.cfg_from_ini('./override_cfg')`. But it's not explicitly load the config thus reducing readability.
 2. you can use the config merging, for example, `new_cfg = base_cfg | override_cfg`. But it's not elegant solution while you  have to merge several config..
 
 #### Now, we provide the thrid way : **sub-config**. you can import the sub-config in any depth of hierachical config by simply placing the `>` symbol at the beginning of line.
     # ./base_cfg.ini
     glb_seed = 42@int
@@ -376,15 +400,15 @@
     [model.backbone]
         mod_typ = 'resnet'
         [model.backbone.optimizer]
         # and yes, interpolation is still valid "after" the reference argument is declared!
             lay_seed = $glb_seed  
 
 
-#### **5. Config Operation**
+#### **6. Config Operation**
 Config operation is one of the core technique for dynamic configuration system!!
 In the following example, you can see that the merging config system already provided a impressive hierachical merging funtionality! 
 
 > For example, `ghyu.opop.add` in cfg_a can be replaced by the cfg_b in **same** section with the same variable name, while the different namespace keep their variable safely ~ so the value of `ghyu.opop.add` will be 67 and `ghyu.opop.tueo.inpo` refer the flatten variable `inpo` and the value will be 46.
 
     from easy_configer.Configer import Configer
 
@@ -442,15 +466,15 @@
         # `cfg_b = cfg_b | cfg_a`, operator support, warn to decrease the read-ability...
         # cfg_a will override the argument of cfg_b which share the identitical variable name in cfg_b!
         # operator support : `cfg_b |= cfg_a` == `cfg_b = cfg_b | cfg_a`
 
 ---
 
 ### **Miscellnous features**
-#### **6. IO Converter**
+#### **7. IO Converter**
     from dataclasses import dataclass
     from typing import Optional
 
     @dataclass
     class TableConfig:
         rows: int = 1
 
@@ -495,34 +519,48 @@
         ez_cfg = cnvt.cnvt_cfg_from(argp_cfg, 'omegaconf')
 
         # Especially, it support "dataclass"!
         ds_cfg = ServerConfig()
         ez_cfg = cnvt.cnvt_cfg_from(ds_cfg, 'dataclass')
 
 
-#### **7. Absl style flag**
+#### **8. Absl style flag**
 > easy_config also support that you can access the 'same' config file in different python file without re-declare the config. test_flag.py under the same work directory
 
+Suppose you have executed `main.py`:
+    from easy_configer.Configer import Configer
+    from utils import get_var_from_flag
+
+    if __name__ == "__main__":
+        cfg = Configer()
+        cfg.cfg_from_str("var = 32")
+
+        # both should output 32 ~
+        print(f"var from main : {cfg.var}")
+        print(f"var from flag : { get_var_from_flag() }")
+
+Now, when you step in `get_var_from_flag` function in different file..
     from easy_configer.Configer import Configer
 
-    def get_n_blk_from_flag():
+    def get_var_from_flag():
         new_cfger = Configer()
         flag = new_cfger.get_cfg_flag()
-        # test to get the pre-defined 'n_blk'
-        return flag.n_blk
+        # test to get the pre-defined 'var'
+        return flag.var
 
 ---
 
 #### **The documentation of easy_configer is also released in read doc** [🔗](https://easy-configer.readthedocs.io/en/latest/)
 
 ---
 
 ### Simple Unittest 🧪
 If you clone this repo and built from source, you can try to run the unittest.
-`cd test && python test_Configer.py`
+`python -m unittest discover`
+> I have placed all test file under test folder.
 
 ---
 
 ### License
 MIT License. More information of each term, please see LICENSE.md
 
 ### Author
```

### Comparing `easy_configer-2.2.0/README.md` & `easy_configer-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,28 @@
+Metadata-Version: 2.1
+Name: easy_configer
+Version: 2.3.0
+Summary: An easy way for configurating python program by the given config file or config str
+Home-page: https://github.com/HuangChiEn/easy_config
+Author: JosefHuang
+Author-email: a3285556aa@gmail.com
+License: MIT
+Keywords: configuration,commendline argument,argument
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Project description
-#### easy_configer version : 2.2.0
+#### easy_configer version : 2.3.0
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
-![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
+![easy-configer logo](assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
 I'm willing to provide a light-weight solution for configurating your python program. Hope this repository make every user control their large project more easier ~ ~ 
 
 ### Introduction 📝
@@ -30,79 +47,68 @@
     parse.add_argument("--lucky_num", type=int)
     ...
     args = parser.parse_args()
     args.lucky_num
     
 
 That leverage me to package my solution for solving this issue. The easy_config will cover the following attributes :
-
-1. **simple & customized syntax of declaration (partially support)**
+1. **Hierachical section config (nested dictionary)**
 
 2. **Accept multiple config file in dynamic loading manner**
 
-3. **Declare customized class instance in the config file**
+3. **Support customized class (initialized by keyword arguments)**
 
 4. **Commend-line update all declared-value wherever it belong, even in hierachical section**
 
-5. **Support the absl style FLAGS functionality** 
-
-6. **Omegaconf like hierachical config**
+5. **Support the absl style FLAGS functionality (declare once, use anywhere)** 
 
 And, of course the following attribute will also be supported :
 
-* dot-access of any default argument (flatten argument)
-
-* dict-access of any section argument (non-flatten argument) 
-
-* commend-line update any argument value (flatten & non-flatten argument)
-
-* add different settings while choosing to overload previous one.
+* dot-access of any arguments (even in nested dictionary)
 
 * inline comment '#', now you can write comment in everyline ~
 
 * support arguments interpolation!!
 
-* support config conversion, which bridge the easy_config into the other config file ~
+* support config conversion, which turn easy_config into the other kind of config package (omegaconf, argparse, ..., etc.)
 
 * support hierachical configurating system with dynamic override ~
+
 ---
 
 ### Newly update features 🚀
-1. Better syntax for override argument via commendline
-2. Better syntax for declare the config file
-3. Various support of config conversion, including omegaconf, dataclasses, dict, ..., etc.
-4. Support enviroment variable (os.Env) interpolation
-5. Dynamic sub-config loading..
-6. Also update document and some handy examples ~
+1. Enable all test case (automatically ci by git-action)
+2. Support dot-access of any arguments
+3. Consistent import syntax.. 
+4. New document is released ~
 
 ---
 
 ### Bug Fixed 🐛
-#### config string with extra space caused config error, and it's fixed in this version.
+#### Fix-up import syntax.. plz open an issue if you find a bug ~
 ---
 
 ### Dependencies 🏗️
 This package is written for Python 3.8. After refactor in this version, this package also support down to python 3.6!!
 Of course, light-weight solution **do not** contain any 3-rd package complex dependencies.
 The python standard package (such as pathlib, sys, .., etc) is the only source of dependencies, so you don't need to worry about that ~ ~
 > However, if you want to use the IO_Converter for converting config into omegaconf, you still need to install omegaconf for this functionality ~
 
 ---
 
 ### Installation ⚙️<br>
 1. **pypi install** <br>
     simply type the `pip install easy_configer` (due to name conflict of pypi pkg, we use different pkg name)
+
 2. **install from source code** <br>
     clone the project from github : `git clone repo-link` 
     Chage to the root directory of the cloned project, and type `pip install -e .`
+
 3. **import syntax** <br>
-    Because of the name conflict of pypi pkg, i choice the different pkg name.
-    To import the installed pkg, the syntax will be depended on the install method. For example. <br>
-    Pip install : `from easy_configer.Configer import Configer` <br>
-    git clone & pip install : `from easy_config.Configer import Configer` <br>
+    Wherever you install, pypi or source. Now, you just need a simple import : `from easy_configer.Configer import Configer`
     
 ---
 
 ### Quick start 🥂
 
 #### **1. Handy example of config file**
 #### Let's say we have an easy-config for development enviroment on jupyter notebook. we want to define several variable for configurating a simple math calculation.
@@ -191,24 +197,29 @@
 
         ... # loading llm model instance `Llama` ~
         llm_mod = Llama(
             ld_8bit=cfger.bknd_srv.load_8bit, 
             chat_mode=cfger.chat_mode, 
             model_type=cfger.model_type
         )
-        llm_mod.init_mod_param( **cfger.bknd_srv['mod_params'] )
 
+        # you can access nested-dict by dot access ~
+        llm_mod.init_mod_param( **cfger.bknd_srv.mod_params )
+
+        # or you can keep the dict fashion ~
         if cfger.bknd_srv['async_req']:
             chat_serv.chat_mod = llm_mod
             chat_serv.hist_db = mongo_serv
         else:
             ... # write sync conversation by yourself..
 
         sys.exit( chat_serv.server_forever() )
 
+> Note that the recommended way to access the argument is **still** key-string access `cfger.args['#4$%-var']`, as you may notice, dot-access doesn't support **ugly** variable name. 
+
 <br>
 
 ---
 
 ### More detail tutorial about each topic is as follows :
 
 #### **2. How to declare hierachical config**
@@ -251,16 +262,19 @@
         
         # omit cfg_from_str, hier-config also could be declared in str though ~
         cfger.cfg_from_ini("./hier_cfg.ini")
         
         print(cfger.dataset)  
         # output nested dict : { 'service_port':65536, 'path':'/data/kitti', 'loader':{'batch_size':32} }
         
-        print(cfger.dataset['loader']['batch_size'])
-        # output : 32
+        print(f"key-string access bz : {cfger.dataset['loader']['batch_size']}")
+        # output - "key-string access bz : 32"
+
+        print(f"bz : {cfger.dataset.loader.batch_size}")
+        # output - "dot-access bz : 32"
 
         # we usually conduct initialization such simple & elegant!
         ds = build_dataset(**cfger.dataset)
         mod = build_model(**cfger.model)
         ... # get torch Trainer
         Trainer(mod).fit(ds)
 
@@ -306,16 +320,42 @@
         cfger = Configer(description="sample for arguments interpolation")
         cfger.regist_cnvtor("pyPath", Path)  # regist customer class 'Path'
 
         cfg_str = get_str_cfg()
         cfger.cfg_from_str(cfg_str)
         # do whatever you want to do!
         
+#### **3. Access all arguments flexibly**
+We simple set a breakpoint to feel how flexible does `easy_configer.utils.Container.AttributeDict` support.
 
-#### **3. Commmend-line Support**
+    from easy_configer.Configer import Configer
+    
+    if __name__ == "__main__":
+        cfger = Configer()
+        cfger.cfg_from_ini("./hier_cfg.ini")
+        breakpoint()
+
+> We write a special example `hier_cfg.ini`!!
+    # nested-dict
+    [secA] # test depth ((sub^4)-section under secA)
+        lev = 1
+        [secA.secB]
+            lev = 2
+            [secA.secB.secC]
+                lev = 3
+                [secA.secB.secC.secD]
+                    lev = 4
+
+Now you can access each `lev` :
+1. `(pdb) cfger.secA.lev `, output `lev : 1`
+2. `(pdb) cfger['secA'].secB['lev'] `, output `lev : 2`, and so on..
+3. Most crazy one ~ `(pdb) cfger.secA.['secB'].secC['secD'].lev `, output `lev : 4`
+
+
+#### **4. Commmend-line Support**
 > We also take `hier_cfg.ini` as example!
 
     # hier_cfg.ini
     glb_var = 42@int
     [dataset]         
         ds_type = None
         path = {'root':'/data/kitti'}@Path
@@ -332,15 +372,15 @@
 
 Especially update **non-flatten argument**, you can access any argument at any level by dot-access in commend-line!! (with combining any argument update). Now, try to change any nested argument <br>
 `python quick_hier.py dataset.ds_type="'kitti'" dataset.path="{'path':'/root/ds'}" dataset.loader.batch_size=48`
 
 ( Note that the commendline declaration for string is tricky, but currently we only support two way for that : 
     `dataset.ds_type="'kitti'"` or `dataset.ds_type=kitti@str`, pick up one of you like ~ )
 
-#### **4. Import Sub-Config**
+#### **5. Import Sub-Config**
 Like `omegaconf`, most of user expect to seperate the config based on their type and dynamically merge it in runtime. It's a rational requirement and the previous version of easy-config provide two way to conduct it, but both have it's limit : 
 1. you can call the `cfg_from_ini` twice, for example, `cfg.cfg_from_ini('./base_cfg') ; cfg.cfg_from_ini('./override_cfg')`. But it's not explicitly load the config thus reducing readability.
 2. you can use the config merging, for example, `new_cfg = base_cfg | override_cfg`. But it's not elegant solution while you  have to merge several config..
 
 #### Now, we provide the thrid way : **sub-config**. you can import the sub-config in any depth of hierachical config by simply placing the `>` symbol at the beginning of line.
     # ./base_cfg.ini
     glb_seed = 42@int
@@ -360,15 +400,15 @@
     [model.backbone]
         mod_typ = 'resnet'
         [model.backbone.optimizer]
         # and yes, interpolation is still valid "after" the reference argument is declared!
             lay_seed = $glb_seed  
 
 
-#### **5. Config Operation**
+#### **6. Config Operation**
 Config operation is one of the core technique for dynamic configuration system!!
 In the following example, you can see that the merging config system already provided a impressive hierachical merging funtionality! 
 
 > For example, `ghyu.opop.add` in cfg_a can be replaced by the cfg_b in **same** section with the same variable name, while the different namespace keep their variable safely ~ so the value of `ghyu.opop.add` will be 67 and `ghyu.opop.tueo.inpo` refer the flatten variable `inpo` and the value will be 46.
 
     from easy_configer.Configer import Configer
 
@@ -426,15 +466,15 @@
         # `cfg_b = cfg_b | cfg_a`, operator support, warn to decrease the read-ability...
         # cfg_a will override the argument of cfg_b which share the identitical variable name in cfg_b!
         # operator support : `cfg_b |= cfg_a` == `cfg_b = cfg_b | cfg_a`
 
 ---
 
 ### **Miscellnous features**
-#### **6. IO Converter**
+#### **7. IO Converter**
     from dataclasses import dataclass
     from typing import Optional
 
     @dataclass
     class TableConfig:
         rows: int = 1
 
@@ -479,39 +519,53 @@
         ez_cfg = cnvt.cnvt_cfg_from(argp_cfg, 'omegaconf')
 
         # Especially, it support "dataclass"!
         ds_cfg = ServerConfig()
         ez_cfg = cnvt.cnvt_cfg_from(ds_cfg, 'dataclass')
 
 
-#### **7. Absl style flag**
+#### **8. Absl style flag**
 > easy_config also support that you can access the 'same' config file in different python file without re-declare the config. test_flag.py under the same work directory
 
+Suppose you have executed `main.py`:
+    from easy_configer.Configer import Configer
+    from utils import get_var_from_flag
+
+    if __name__ == "__main__":
+        cfg = Configer()
+        cfg.cfg_from_str("var = 32")
+
+        # both should output 32 ~
+        print(f"var from main : {cfg.var}")
+        print(f"var from flag : { get_var_from_flag() }")
+
+Now, when you step in `get_var_from_flag` function in different file..
     from easy_configer.Configer import Configer
 
-    def get_n_blk_from_flag():
+    def get_var_from_flag():
         new_cfger = Configer()
         flag = new_cfger.get_cfg_flag()
-        # test to get the pre-defined 'n_blk'
-        return flag.n_blk
+        # test to get the pre-defined 'var'
+        return flag.var
 
 ---
 
 #### **The documentation of easy_configer is also released in read doc** [🔗](https://easy-configer.readthedocs.io/en/latest/)
 
 ---
 
 ### Simple Unittest 🧪
 If you clone this repo and built from source, you can try to run the unittest.
-`cd test && python test_Configer.py`
+`python -m unittest discover`
+> I have placed all test file under test folder.
 
 ---
 
 ### License
 MIT License. More information of each term, please see LICENSE.md
 
 ### Author 
 Josef-Huang, a3285556aa@gmail.com 
 
 ### Footer
 ~ Hope God bless everyone in the world to know his word ~ <br>
-**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
+**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
```

### Comparing `easy_configer-2.2.0/easy_configer/Configer.py` & `easy_configer-2.3.0/easy_configer/Configer.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import warnings
 def warning_on_one_line(message, category, filename, lineno, file=None, line=None):
     return "{0}:{1}: {2}: {3}\n".format(filename, lineno, category.__name__, message)
 warnings.formatwarning = warning_on_one_line
 
 from .utils.Type_Convertor import Type_Convertor
-from .utils.Flag import Flag
+from .utils.Container import AttributeDict, Flag
 from .IO_Converter import IO_Converter
 
 class Configer(object):
     '''
         The Configer attemtp to make a light-weight solution for configurating your program, 
         which offer a simple syntax for declare the arguments in the configure file (.ini suffix).
         Moreover, I try to implement a highly customer reader, which allow the user to declare 
@@ -70,34 +70,41 @@
                 The path which locate the '*.ini' config file.
         '''
         def chk_src(cfg_path):
             if not cfg_path.exists():
                 raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), str(cfg_path))
             if not cfg_path.suffix == ".ini":
                 raise ValueError("The file extension should be 'ini', instead of '{0}'".format(cfg_path.suffix))
-            
+        
+        # take from : https://stackoverflow.com/questions/16480495/read-a-file-with-line-continuation-characters-in-python
+        def continuation_lines(fin):
+            for line in fin:
+                line = line.rstrip('\n')
+                while line.endswith('\\'):
+                    line = line[:-1] + next(fin).rstrip('\n')
+                yield line
+
         try:
             # check config path validation
             cfg_path = Path(cfg_path)
             chk_src(cfg_path)
 
             with cfg_path.open('r') as cfg_ptr: 
-                raw_cfg_text = cfg_ptr.read()
+                raw_cfg_text = "\n".join([ line for line in continuation_lines(cfg_ptr) ])
             
         except FileNotFoundError as fnf_err:
             print(fnf_err) ; raise
         except ValueError as val_err:
             print(val_err) ; raise
         except PermissionError as per_err:
             print(per_err) ; raise
         except Exception as ex:
             print(ex) ; raise
-        else:
-            self.__cfg_parser(raw_cfg_text)
         
+        self.__cfg_parser(raw_cfg_text)
         # build the flag object 
         self.__flag.__dict__ = self.__dict__
     
     ## Core implementation of config parser : 
     #  utils of config parser
     def __preproc_cfgstr(self, cfg_str:str) -> str:
         # eliminate the line full of white-space without any text
@@ -125,33 +132,35 @@
             Therefore, i wrote this function to deal with searching and return the "pointer" point to the section.
             It's sync with self.__dict__, so use it wiselly & carefully!!
         '''
         sec_name_lst = sec_keys_str.split('.')
         # Before easy_configer 1.3.4 ver, all section is builded upon this level
         if len(sec_name_lst) == 1:
             return self.__dict__, sec_keys_str
-
+            
         root_key = sec_name_lst.pop(0)
         if root_key not in self.__dict__:
             if not allow_init:
                 raise RuntimeError("The parent node of {0} is not defined yet, " \
                                         "it's invalid for directly made the child node".format(root_key))
-            self.__dict__[root_key] = {}
-
+            self.__dict__[root_key] = AttributeDict() 
+            
         ## Support toml like 'hierachical' format!!
         #  dynamically search the hierachical section begin from the 'next layer' of self.__dict__
         idx_sec = self.__dict__[root_key]
+        
         #  keep the index point to the node "parent", since the child node will be init as dict!
         for sec in sec_name_lst[:-1]:
+            # AttributeDict.get(.) will not trigger "defaultdict behavior"
             tmp = idx_sec.get(sec, '__UNDEFINE_VAL')
             if tmp == '__UNDEFINE_VAL':
                 if not allow_init:
                     raise RuntimeError("The parent node '{0}' is not defined yet, " \
                                             "it's invalid for directly made the child node".format(sec))
-                idx_sec[sec] = {}
+                idx_sec[sec] = AttributeDict() 
             idx_sec = idx_sec[sec]
 
         return idx_sec, sec_name_lst[-1]
 
     def __get_declr_dict(self, cfg_str:str) -> dict : 
         if self.__split_chr not in cfg_str:
             raise RuntimeError("Configuration Error : Split character '{0}'" \
@@ -187,30 +196,30 @@
             '''
                 sub_cfg_path :
                     The path of interpolated config. 
                     The sub-config path is parsed from the .ini file with split '>' symbol.
             '''
             sub_cfg = Configer(cmd_args=False)
             sub_cfg.cfg_from_ini(sub_cfg_path)
-            return self.__cfg_cnvt.cnvt_cfg_to(sub_cfg, 'dict')
+            return self.__cfg_cnvt.cnvt_cfg_to(sub_cfg, 'dict', return_attr_dict=True)
 
         cur_sec_keys = ''
         for lin in raw_cfg_text.splitlines():
             # strip empty space and 'skip' empty line in cfgstr
             cfg_str = self.__preproc_cfgstr(lin)
             if not cfg_str:
                 continue
 
             # get the section key of config string (if there exists)
             sec_keys_str = self.__get_sec(cfg_str)
             if sec_keys_str:
                 idx_sec, idx_sec_key = self.__idx_sec_by_dot(sec_keys_str)
                 if idx_sec_key in idx_sec.keys():
                     raise RuntimeError('Re-defined config, {0} section will be overrided!!'.format(sec_keys_str))
-                idx_sec[idx_sec_key] = {}
+                idx_sec[idx_sec_key] = AttributeDict()
                 cur_sec_keys = sec_keys_str
             
             # parse variable assignment string
             else:
                 # parse the value string into value dict
                 if cfg_str[0] == '>':
                     # import other .ini config as value dict
@@ -220,17 +229,18 @@
                     # normal value string
                     val_dict = self.__get_declr_dict(cfg_str)
 
                 # assign the val_dict into the corresponding section!
                 if cur_sec_keys != '':
                     idx_sec, idx_sec_key = self.__idx_sec_by_dot(cur_sec_keys)
                     idx_sec[idx_sec_key].update( val_dict )
-                else:
+                # assign the val_dict as 'flatten' arguments 
+                else: # Note that flatten args IS NOT AttributeDict!
                     self.__dict__.update( val_dict )
-
+                    
         # Update the namespace value via commend-line input 
         if self.__cmd_args:
             self.args_from_cmd()
 
     def args_from_cmd(self):   
         '''
             Update the arguments by commend line input string
@@ -241,15 +251,15 @@
         # print out helper document string
         if "-h" in cmd_arg_lst:
             cmd_arg_lst.remove("-h")
             print(self.__doc_str)
 
         # ' = ' -> '=', eliminate white space
         cmd_sp_chr = self.split_char.strip()
-        sec_ptr, sec_key = None, None
+        sec_ptr, sec_key = None, None 
         for item in cmd_arg_lst:
             itm_lst = [ itm for itm in item.split(cmd_sp_chr) if itm != '']
             if len(itm_lst) != 2:
                 raise RuntimeError(f"Invalid commendline input : the split char '{cmd_sp_chr}' should only present once and the value should be given!")
             
             sec_keys_str, val_str = itm_lst
             sec_ptr, sec_key = self.__idx_sec_by_dot(sec_keys_str, allow_init=True)
@@ -296,19 +306,36 @@
         # prevent checking private vars
         cfg_dict = { k:v for k, v in cfg.__dict__.copy().items() \
                                     if '_' != k[0] }
         hier_merge(self.__dict__, cfg_dict)
 
     # Display the namespace which record all of the declared arguments
     #   for the inner-node structure, iter-call __str__ wrapper !!
+    def __shadow_private_args(self):
+        return [ str(key) for key in self.__dict__.keys() if key[0] != '_' ] 
+
     def __str__(self):
-        key_str = [ str(key) for key in self.__dict__.keys() if key[0] != '_' ] 
+        key_str = self.__shadow_private_args()
         return "Namespace : \n" + ", ".join(key_str)
     # override default __repr__ to view configer in debugger
     __repr__ = __str__
+
+    ## public interface for iterate the entire config
+    def __iter__(self):
+        tmp_dct = {}
+        for key in self.__shadow_private_args():
+            tmp_dct[key] = self.__dict__[key]
+        return iter(tmp_dct)
+    
+    ## standard interface for dict-access for flatten argument (since Configer IS NOT AttributeDict)
+    def __getitem__(self, key):
+        return self.__dict__[key]
+
+    def __setitem__(self, key, value):
+        self.__dict__[key] = value
     
     ## Miscellnous functionality : 
     # return an absl style flag to store all of the args.
     def get_cfg_flag(self):
         return self.__flag
 
     def get_doc_str(self):
```

### Comparing `easy_configer-2.2.0/easy_configer/IO_Converter.py` & `easy_configer-2.3.0/easy_configer/IO_Converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from argparse import ArgumentParser
+from .utils.Container import AttributeDict
 
 class IO_Converter(object):
     def __init__(self):
         # 'o'utput to different config 
         self.output_dispatcher = {
             'argparse' : self._to_argparse,
             'omegaconf' : self._to_omegacfg,
@@ -47,44 +48,50 @@
             raise ImportError("Python version you used doesn't support native {0} pkg, " \
                             "please 'pip install {0}'.".format( pypi_name[pkg_name] ))
         return mod
 
     def __remove_private_var(self, raw_cfg):
         tmp_dict = {}
         for k, v in raw_cfg.__dict__.items():
-            if not k[0] == '_':
+            # all private attribute is presented at first level
+            if not k.startswith('_'):
                 tmp_dict[k] = v
         return tmp_dict
 
+    def __convert_to_dict(self, sec_val):
+        dct = {}
+        for k, v in sec_val.items():
+            if isinstance(v, AttributeDict):
+                v = self.__convert_to_dict(v)
+            dct[k] = v
+        return dct
+    
+    def _to_dict(self, raw_cfg, return_attr_dict=False):
+        cfg = self.__remove_private_var(raw_cfg)
+        # force to convert AttributeDict into native python dict!
+        return cfg if return_attr_dict else self.__convert_to_dict(cfg)
+
     # Convert easy_config to different config, QQ.. Byebye user..
-    def _to_argparse(self, raw_cfg, parse_arg=True, flatten_args=True):
+    def _to_argparse(self, raw_cfg, parse_arg=True):
         args_template = ArgumentParser( description=raw_cfg.get_doc_str() )
-        raw_dict = self.__remove_private_var(raw_cfg)
+        for sec_key, sec_val in self._to_dict(raw_cfg).items():         
+            args_template.add_argument("--{0}".format(sec_key), type=type(sec_val), default=sec_val)
         
-        for sec_key, sec_val in raw_dict.items():
-            if flatten_args and isinstance(sec_val, dict):
-                for key, val in sec_val.items():
-                    args_template.add_argument("--{0}".format(key), type=type(val), default=val)
-            else:
-                args_template.add_argument("--{0}".format(sec_key), type=type(sec_val), default=sec_val)
-
         return args_template.parse_args() if parse_arg else args_template
 
     def _to_yaml(self, raw_cfg):
         mod = self.__imp_pkg('yaml')
-        raw_dict = self.__remove_private_var(raw_cfg)
-        return mod.dump(raw_dict)
+        cfg_dict = self._to_dict(raw_cfg)
+
+        return mod.dump(cfg_dict)
 
     def _to_omegacfg(self, raw_cfg):
         mod = self.__imp_pkg('omegaconf.omegaconf')
-        raw_dict = self.__remove_private_var(raw_cfg)
-        return mod.OmegaConf.create(raw_dict)
-
-    def _to_dict(self, raw_cfg):
-        return self.__remove_private_var(raw_cfg)
+        cfg_dict = self._to_dict(raw_cfg)
+        return mod.OmegaConf.create(cfg_dict)
     
     # Convert different config to easy_config! welcome aboard, User ~ www
     def _from_argparse(self, arg_cfg):
         arg_cfg_dict = vars(arg_cfg)
         return self._from_dict(arg_cfg_dict)
 
     def _from_yaml(self, yaml_str):
@@ -102,9 +109,13 @@
         datacls_dict = mod.asdict(datacls_cfg)
         return self._from_dict(datacls_dict)
 
     def _from_dict(self, cfg_dict):
         from .Configer import Configer
         cfg = Configer()
         for k, v in cfg_dict.items():
+            if isinstance(v, dict):
+                # set_attr_dict is enabled in init..
+                # no need to convert the nested-dict manuelly!
+                v = AttributeDict(v)
             cfg.__dict__[k] = v
         return cfg
```

### Comparing `easy_configer-2.2.0/easy_configer/utils/Type_Convertor.py` & `easy_configer-2.3.0/easy_configer/utils/Type_Convertor.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.2.0/easy_configer.egg-info/PKG-INFO` & `easy_configer-2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-Metadata-Version: 2.1
-Name: easy-configer
-Version: 2.2.0
-Summary: An easy way for configurating python program by the given config file or config str
-Home-page: https://github.com/HuangChiEn/easy_config
-Author: JosefHuang
-Author-email: a3285556aa@gmail.com
-License: MIT
-Keywords: configuration,commendline argument,argument
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Project description
-#### easy_configer version : 2.2.0
+#### easy_configer version : 2.3.0
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
-![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
+![easy-configer logo](assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
 I'm willing to provide a light-weight solution for configurating your python program. Hope this repository make every user control their large project more easier ~ ~ 
 
 ### Introduction 📝
@@ -46,79 +31,68 @@
     parse.add_argument("--lucky_num", type=int)
     ...
     args = parser.parse_args()
     args.lucky_num
     
 
 That leverage me to package my solution for solving this issue. The easy_config will cover the following attributes :
-
-1. **simple & customized syntax of declaration (partially support)**
+1. **Hierachical section config (nested dictionary)**
 
 2. **Accept multiple config file in dynamic loading manner**
 
-3. **Declare customized class instance in the config file**
+3. **Support customized class (initialized by keyword arguments)**
 
 4. **Commend-line update all declared-value wherever it belong, even in hierachical section**
 
-5. **Support the absl style FLAGS functionality** 
-
-6. **Omegaconf like hierachical config**
+5. **Support the absl style FLAGS functionality (declare once, use anywhere)** 
 
 And, of course the following attribute will also be supported :
 
-* dot-access of any default argument (flatten argument)
-
-* dict-access of any section argument (non-flatten argument) 
-
-* commend-line update any argument value (flatten & non-flatten argument)
-
-* add different settings while choosing to overload previous one.
+* dot-access of any arguments (even in nested dictionary)
 
 * inline comment '#', now you can write comment in everyline ~
 
 * support arguments interpolation!!
 
-* support config conversion, which bridge the easy_config into the other config file ~
+* support config conversion, which turn easy_config into the other kind of config package (omegaconf, argparse, ..., etc.)
 
 * support hierachical configurating system with dynamic override ~
+
 ---
 
 ### Newly update features 🚀
-1. Better syntax for override argument via commendline
-2. Better syntax for declare the config file
-3. Various support of config conversion, including omegaconf, dataclasses, dict, ..., etc.
-4. Support enviroment variable (os.Env) interpolation
-5. Dynamic sub-config loading..
-6. Also update document and some handy examples ~
+1. Enable all test case (automatically ci by git-action)
+2. Support dot-access of any arguments
+3. Consistent import syntax.. 
+4. New document is released ~
 
 ---
 
 ### Bug Fixed 🐛
-#### config string with extra space caused config error, and it's fixed in this version.
+#### Fix-up import syntax.. plz open an issue if you find a bug ~
 ---
 
 ### Dependencies 🏗️
 This package is written for Python 3.8. After refactor in this version, this package also support down to python 3.6!!
 Of course, light-weight solution **do not** contain any 3-rd package complex dependencies.
 The python standard package (such as pathlib, sys, .., etc) is the only source of dependencies, so you don't need to worry about that ~ ~
 > However, if you want to use the IO_Converter for converting config into omegaconf, you still need to install omegaconf for this functionality ~
 
 ---
 
 ### Installation ⚙️<br>
 1. **pypi install** <br>
     simply type the `pip install easy_configer` (due to name conflict of pypi pkg, we use different pkg name)
+
 2. **install from source code** <br>
     clone the project from github : `git clone repo-link` 
     Chage to the root directory of the cloned project, and type `pip install -e .`
+
 3. **import syntax** <br>
-    Because of the name conflict of pypi pkg, i choice the different pkg name.
-    To import the installed pkg, the syntax will be depended on the install method. For example. <br>
-    Pip install : `from easy_configer.Configer import Configer` <br>
-    git clone & pip install : `from easy_config.Configer import Configer` <br>
+    Wherever you install, pypi or source. Now, you just need a simple import : `from easy_configer.Configer import Configer`
     
 ---
 
 ### Quick start 🥂
 
 #### **1. Handy example of config file**
 #### Let's say we have an easy-config for development enviroment on jupyter notebook. we want to define several variable for configurating a simple math calculation.
@@ -207,24 +181,29 @@
 
         ... # loading llm model instance `Llama` ~
         llm_mod = Llama(
             ld_8bit=cfger.bknd_srv.load_8bit, 
             chat_mode=cfger.chat_mode, 
             model_type=cfger.model_type
         )
-        llm_mod.init_mod_param( **cfger.bknd_srv['mod_params'] )
 
+        # you can access nested-dict by dot access ~
+        llm_mod.init_mod_param( **cfger.bknd_srv.mod_params )
+
+        # or you can keep the dict fashion ~
         if cfger.bknd_srv['async_req']:
             chat_serv.chat_mod = llm_mod
             chat_serv.hist_db = mongo_serv
         else:
             ... # write sync conversation by yourself..
 
         sys.exit( chat_serv.server_forever() )
 
+> Note that the recommended way to access the argument is **still** key-string access `cfger.args['#4$%-var']`, as you may notice, dot-access doesn't support **ugly** variable name. 
+
 <br>
 
 ---
 
 ### More detail tutorial about each topic is as follows :
 
 #### **2. How to declare hierachical config**
@@ -267,16 +246,19 @@
         
         # omit cfg_from_str, hier-config also could be declared in str though ~
         cfger.cfg_from_ini("./hier_cfg.ini")
         
         print(cfger.dataset)  
         # output nested dict : { 'service_port':65536, 'path':'/data/kitti', 'loader':{'batch_size':32} }
         
-        print(cfger.dataset['loader']['batch_size'])
-        # output : 32
+        print(f"key-string access bz : {cfger.dataset['loader']['batch_size']}")
+        # output - "key-string access bz : 32"
+
+        print(f"bz : {cfger.dataset.loader.batch_size}")
+        # output - "dot-access bz : 32"
 
         # we usually conduct initialization such simple & elegant!
         ds = build_dataset(**cfger.dataset)
         mod = build_model(**cfger.model)
         ... # get torch Trainer
         Trainer(mod).fit(ds)
 
@@ -322,16 +304,42 @@
         cfger = Configer(description="sample for arguments interpolation")
         cfger.regist_cnvtor("pyPath", Path)  # regist customer class 'Path'
 
         cfg_str = get_str_cfg()
         cfger.cfg_from_str(cfg_str)
         # do whatever you want to do!
         
+#### **3. Access all arguments flexibly**
+We simple set a breakpoint to feel how flexible does `easy_configer.utils.Container.AttributeDict` support.
 
-#### **3. Commmend-line Support**
+    from easy_configer.Configer import Configer
+    
+    if __name__ == "__main__":
+        cfger = Configer()
+        cfger.cfg_from_ini("./hier_cfg.ini")
+        breakpoint()
+
+> We write a special example `hier_cfg.ini`!!
+    # nested-dict
+    [secA] # test depth ((sub^4)-section under secA)
+        lev = 1
+        [secA.secB]
+            lev = 2
+            [secA.secB.secC]
+                lev = 3
+                [secA.secB.secC.secD]
+                    lev = 4
+
+Now you can access each `lev` :
+1. `(pdb) cfger.secA.lev `, output `lev : 1`
+2. `(pdb) cfger['secA'].secB['lev'] `, output `lev : 2`, and so on..
+3. Most crazy one ~ `(pdb) cfger.secA.['secB'].secC['secD'].lev `, output `lev : 4`
+
+
+#### **4. Commmend-line Support**
 > We also take `hier_cfg.ini` as example!
 
     # hier_cfg.ini
     glb_var = 42@int
     [dataset]         
         ds_type = None
         path = {'root':'/data/kitti'}@Path
@@ -348,15 +356,15 @@
 
 Especially update **non-flatten argument**, you can access any argument at any level by dot-access in commend-line!! (with combining any argument update). Now, try to change any nested argument <br>
 `python quick_hier.py dataset.ds_type="'kitti'" dataset.path="{'path':'/root/ds'}" dataset.loader.batch_size=48`
 
 ( Note that the commendline declaration for string is tricky, but currently we only support two way for that : 
     `dataset.ds_type="'kitti'"` or `dataset.ds_type=kitti@str`, pick up one of you like ~ )
 
-#### **4. Import Sub-Config**
+#### **5. Import Sub-Config**
 Like `omegaconf`, most of user expect to seperate the config based on their type and dynamically merge it in runtime. It's a rational requirement and the previous version of easy-config provide two way to conduct it, but both have it's limit : 
 1. you can call the `cfg_from_ini` twice, for example, `cfg.cfg_from_ini('./base_cfg') ; cfg.cfg_from_ini('./override_cfg')`. But it's not explicitly load the config thus reducing readability.
 2. you can use the config merging, for example, `new_cfg = base_cfg | override_cfg`. But it's not elegant solution while you  have to merge several config..
 
 #### Now, we provide the thrid way : **sub-config**. you can import the sub-config in any depth of hierachical config by simply placing the `>` symbol at the beginning of line.
     # ./base_cfg.ini
     glb_seed = 42@int
@@ -376,15 +384,15 @@
     [model.backbone]
         mod_typ = 'resnet'
         [model.backbone.optimizer]
         # and yes, interpolation is still valid "after" the reference argument is declared!
             lay_seed = $glb_seed  
 
 
-#### **5. Config Operation**
+#### **6. Config Operation**
 Config operation is one of the core technique for dynamic configuration system!!
 In the following example, you can see that the merging config system already provided a impressive hierachical merging funtionality! 
 
 > For example, `ghyu.opop.add` in cfg_a can be replaced by the cfg_b in **same** section with the same variable name, while the different namespace keep their variable safely ~ so the value of `ghyu.opop.add` will be 67 and `ghyu.opop.tueo.inpo` refer the flatten variable `inpo` and the value will be 46.
 
     from easy_configer.Configer import Configer
 
@@ -442,15 +450,15 @@
         # `cfg_b = cfg_b | cfg_a`, operator support, warn to decrease the read-ability...
         # cfg_a will override the argument of cfg_b which share the identitical variable name in cfg_b!
         # operator support : `cfg_b |= cfg_a` == `cfg_b = cfg_b | cfg_a`
 
 ---
 
 ### **Miscellnous features**
-#### **6. IO Converter**
+#### **7. IO Converter**
     from dataclasses import dataclass
     from typing import Optional
 
     @dataclass
     class TableConfig:
         rows: int = 1
 
@@ -495,39 +503,53 @@
         ez_cfg = cnvt.cnvt_cfg_from(argp_cfg, 'omegaconf')
 
         # Especially, it support "dataclass"!
         ds_cfg = ServerConfig()
         ez_cfg = cnvt.cnvt_cfg_from(ds_cfg, 'dataclass')
 
 
-#### **7. Absl style flag**
+#### **8. Absl style flag**
 > easy_config also support that you can access the 'same' config file in different python file without re-declare the config. test_flag.py under the same work directory
 
+Suppose you have executed `main.py`:
+    from easy_configer.Configer import Configer
+    from utils import get_var_from_flag
+
+    if __name__ == "__main__":
+        cfg = Configer()
+        cfg.cfg_from_str("var = 32")
+
+        # both should output 32 ~
+        print(f"var from main : {cfg.var}")
+        print(f"var from flag : { get_var_from_flag() }")
+
+Now, when you step in `get_var_from_flag` function in different file..
     from easy_configer.Configer import Configer
 
-    def get_n_blk_from_flag():
+    def get_var_from_flag():
         new_cfger = Configer()
         flag = new_cfger.get_cfg_flag()
-        # test to get the pre-defined 'n_blk'
-        return flag.n_blk
+        # test to get the pre-defined 'var'
+        return flag.var
 
 ---
 
 #### **The documentation of easy_configer is also released in read doc** [🔗](https://easy-configer.readthedocs.io/en/latest/)
 
 ---
 
 ### Simple Unittest 🧪
 If you clone this repo and built from source, you can try to run the unittest.
-`cd test && python test_Configer.py`
+`python -m unittest discover`
+> I have placed all test file under test folder.
 
 ---
 
 ### License
 MIT License. More information of each term, please see LICENSE.md
 
 ### Author 
 Josef-Huang, a3285556aa@gmail.com 
 
 ### Footer
 ~ Hope God bless everyone in the world to know his word ~ <br>
-**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
+**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
```

### Comparing `easy_configer-2.2.0/setup.py` & `easy_configer-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # read the contents of your README file
 this_directory = abspath(dirname(__file__))
 with open(join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='easy_configer',
-    version='2.2.0',
+    version='2.3.0',
     description='An easy way for configurating python program by the given config file or config str',
     author='JosefHuang',
     author_email='a3285556aa@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/HuangChiEn/easy_config',
```

