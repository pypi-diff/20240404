# Comparing `tmp/ForgeHg-0.5.2.tar.gz` & `tmp/ForgeHg-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForgeHg-0.5.2.tar", last modified: Thu Jul  6 15:31:22 2023, max compression
+gzip compressed data, was "ForgeHg-0.5.3.tar", last modified: Thu Apr  4 20:55:08 2024, max compression
```

## Comparing `ForgeHg-0.5.2.tar` & `ForgeHg-0.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.066315 ForgeHg-0.5.2/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:21.991742 ForgeHg-0.5.2/ForgeHg.egg-info/
--rw-r--r--   0 brondsem   (502) staff       (20)      944 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/PKG-INFO
--rw-r--r--   0 brondsem   (502) staff       (20)      470 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/SOURCES.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/dependency_links.txt
--rw-r--r--   0 brondsem   (502) staff       (20)      130 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/entry_points.txt
--rw-r--r--   0 brondsem   (502) staff       (20)       24 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/requires.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        8 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/top_level.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2020-11-03 21:41:30.000000 ForgeHg-0.5.2/ForgeHg.egg-info/zip-safe
--rw-r--r--   0 brondsem   (502) staff       (20)    18093 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/LICENSE
--rw-r--r--   0 brondsem   (502) staff       (20)      247 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/MANIFEST.in
--rw-r--r--   0 brondsem   (502) staff       (20)      944 2023-07-06 15:31:22.065813 ForgeHg-0.5.2/PKG-INFO
--rw-r--r--   0 brondsem   (502) staff       (20)     5393 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/README.rst
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.059753 ForgeHg-0.5.2/forgehg/
--rw-r--r--   0 brondsem   (502) staff       (20)        0 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/forgehg/__init__.py
--rw-r--r--   0 brondsem   (502) staff       (20)      665 2022-04-15 20:49:21.000000 ForgeHg-0.5.2/forgehg/controllers.py
--rw-r--r--   0 brondsem   (502) staff       (20)     3774 2023-07-06 15:08:14.000000 ForgeHg-0.5.2/forgehg/hg_main.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.061305 ForgeHg-0.5.2/forgehg/model/
--rw-r--r--   0 brondsem   (502) staff       (20)       27 2022-06-28 21:31:29.000000 ForgeHg-0.5.2/forgehg/model/__init__.py
--rw-r--r--   0 brondsem   (502) staff       (20)    27843 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/forgehg/model/hg.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:21.984171 ForgeHg-0.5.2/forgehg/nf/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:21.984308 ForgeHg-0.5.2/forgehg/nf/hg/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.062961 ForgeHg-0.5.2/forgehg/nf/hg/images/
--rw-r--r--   0 brondsem   (502) staff       (20)     4688 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/forgehg/nf/hg/images/hg.png
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.064271 ForgeHg-0.5.2/forgehg/templates/
--rw-r--r--   0 brondsem   (502) staff       (20)        0 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/forgehg/templates/__init__.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.064888 ForgeHg-0.5.2/forgehg/templates/hg/
--rw-r--r--   0 brondsem   (502) staff       (20)     3102 2022-06-13 13:56:25.000000 ForgeHg-0.5.2/forgehg/templates/hg/index.html
--rw-r--r--   0 brondsem   (502) staff       (20)       80 2023-07-06 15:29:09.000000 ForgeHg-0.5.2/forgehg/version.py
--rw-r--r--   0 brondsem   (502) staff       (20)       38 2023-07-06 15:31:22.066496 ForgeHg-0.5.2/setup.cfg
--rw-r--r--   0 brondsem   (502) staff       (20)     2739 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/setup.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.363776 ForgeHg-0.5.3/
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.363336 ForgeHg-0.5.3/ForgeHg.egg-info/
+-rw-r--r--   0 brondsem   (501) staff       (20)      998 2024-04-04 20:55:08.000000 ForgeHg-0.5.3/ForgeHg.egg-info/PKG-INFO
+-rw-r--r--   0 brondsem   (501) staff       (20)      470 2024-04-04 20:55:08.000000 ForgeHg-0.5.3/ForgeHg.egg-info/SOURCES.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)        1 2024-04-04 20:55:08.000000 ForgeHg-0.5.3/ForgeHg.egg-info/dependency_links.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)      130 2024-04-04 20:55:08.000000 ForgeHg-0.5.3/ForgeHg.egg-info/entry_points.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)       24 2024-04-04 20:55:08.000000 ForgeHg-0.5.3/ForgeHg.egg-info/requires.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)        8 2024-04-04 20:55:08.000000 ForgeHg-0.5.3/ForgeHg.egg-info/top_level.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)        1 2020-11-03 21:41:30.000000 ForgeHg-0.5.3/ForgeHg.egg-info/zip-safe
+-rw-r--r--   0 brondsem   (501) staff       (20)    18093 2013-02-15 23:14:03.000000 ForgeHg-0.5.3/LICENSE
+-rw-r--r--   0 brondsem   (501) staff       (20)      247 2013-02-15 23:14:03.000000 ForgeHg-0.5.3/MANIFEST.in
+-rw-r--r--   0 brondsem   (501) staff       (20)      998 2024-04-04 20:55:08.363575 ForgeHg-0.5.3/PKG-INFO
+-rw-r--r--   0 brondsem   (501) staff       (20)     5393 2023-01-13 19:44:25.000000 ForgeHg-0.5.3/README.rst
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.361669 ForgeHg-0.5.3/forgehg/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2023-01-13 19:44:25.000000 ForgeHg-0.5.3/forgehg/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)      713 2023-12-05 18:50:11.000000 ForgeHg-0.5.3/forgehg/controllers.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     3774 2023-07-06 15:08:14.000000 ForgeHg-0.5.3/forgehg/hg_main.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.362096 ForgeHg-0.5.3/forgehg/model/
+-rw-r--r--   0 brondsem   (501) staff       (20)       27 2022-06-28 21:31:29.000000 ForgeHg-0.5.3/forgehg/model/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    27843 2023-01-13 19:44:25.000000 ForgeHg-0.5.3/forgehg/model/hg.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.358445 ForgeHg-0.5.3/forgehg/nf/
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.358495 ForgeHg-0.5.3/forgehg/nf/hg/
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.362534 ForgeHg-0.5.3/forgehg/nf/hg/images/
+-rw-r--r--   0 brondsem   (501) staff       (20)     4688 2013-02-15 23:14:03.000000 ForgeHg-0.5.3/forgehg/nf/hg/images/hg.png
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.362866 ForgeHg-0.5.3/forgehg/templates/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2013-02-15 23:14:03.000000 ForgeHg-0.5.3/forgehg/templates/__init__.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:08.362995 ForgeHg-0.5.3/forgehg/templates/hg/
+-rw-r--r--   0 brondsem   (501) staff       (20)     3098 2024-04-04 20:10:02.000000 ForgeHg-0.5.3/forgehg/templates/hg/index.html
+-rw-r--r--   0 brondsem   (501) staff       (20)       80 2024-04-04 20:10:51.000000 ForgeHg-0.5.3/forgehg/version.py
+-rw-r--r--   0 brondsem   (501) staff       (20)       38 2024-04-04 20:55:08.363820 ForgeHg-0.5.3/setup.cfg
+-rw-r--r--   0 brondsem   (501) staff       (20)     2739 2023-01-13 19:44:25.000000 ForgeHg-0.5.3/setup.py
```

### Comparing `ForgeHg-0.5.2/ForgeHg.egg-info/PKG-INFO` & `ForgeHg-0.5.3/ForgeHg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForgeHg
-Version: 0.5.2
+Version: 0.5.3
 Summary: Mercurial (Hg) SCM support for Apache Allura
 Home-page: http://sourceforge.net/p/forgehg
 Author-email: dev@allura.apache.org
 License: GPLv2
 Keywords: Allura forge Mercurial Hg scm
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,11 +13,13 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: mercurial<6.2,>=5.8
+Requires-Dist: six
 
 ForgeHg enables an Allura installation to use the Mercurial
 source code management system. Mercurial (Hg) is an open source distributed
 version control system (DVCS) similar to git and written in Python.
```

### Comparing `ForgeHg-0.5.2/LICENSE` & `ForgeHg-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.2/PKG-INFO` & `ForgeHg-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForgeHg
-Version: 0.5.2
+Version: 0.5.3
 Summary: Mercurial (Hg) SCM support for Apache Allura
 Home-page: http://sourceforge.net/p/forgehg
 Author-email: dev@allura.apache.org
 License: GPLv2
 Keywords: Allura forge Mercurial Hg scm
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,11 +13,13 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: mercurial<6.2,>=5.8
+Requires-Dist: six
 
 ForgeHg enables an Allura installation to use the Mercurial
 source code management system. Mercurial (Hg) is an open source distributed
 version control system (DVCS) similar to git and written in Python.
```

### Comparing `ForgeHg-0.5.2/README.rst` & `ForgeHg-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.2/forgehg/controllers.py` & `ForgeHg-0.5.3/forgehg/controllers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from allura.lib.utils import permanent_redirect
 from tg import expose, redirect
 from tg.decorators import with_trailing_slash
 from tg import tmpl_context as c
 
+from allura.lib import helpers as h
 from allura.controllers import repository
 
 
 class BranchBrowser(repository.BranchBrowser):
 
     @expose('jinja:forgehg:templates/hg/index.html')
     @with_trailing_slash
     def index(self, limit=None, page=0, count=0, **kw):
         is_empty = c.app.repo.is_empty()
         latest = c.app.repo.latest(branch=self._branch)
         if is_empty or not latest:
             return dict(allow_fork=False, log=[], is_empty=is_empty)
-        permanent_redirect(c.app.repo.url_for_commit(self._branch) + 'tree/')
+        permanent_redirect(h.urlquote(c.app.repo.url_for_commit(self._branch) + 'tree/'))
```

### Comparing `ForgeHg-0.5.2/forgehg/hg_main.py` & `ForgeHg-0.5.3/forgehg/hg_main.py`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.2/forgehg/model/hg.py` & `ForgeHg-0.5.3/forgehg/model/hg.py`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.2/forgehg/nf/hg/images/hg.png` & `ForgeHg-0.5.3/forgehg/nf/hg/images/hg.png`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.2/forgehg/templates/hg/index.html` & `ForgeHg-0.5.3/forgehg/templates/hg/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     <h2>Recent Commits{% if branch %} on {{branch}}{% endif %}</h2>
     {{c.log_widget.display(value=log, show_paging=False,
                            limit=limit, page=page, count=count)}}
     {% if int(count) > int(limit) %}
       <a href="log?page=1">More</a>
     {% endif %}
   {% elif is_empty %}
-    {% if h.has_access(c.app, 'write')() %}
+    {% if h.has_access(c.app, 'write') %}
     <div class="message warning scm-learn-basics">
       <div class="content">
         <img src="{{g.app_static('images/hg.png')}}" style="float:left">
         <h2>New to Mercurial?</h2>
         <a href="https://www.mercurial-scm.org/learn">Learn the basics</a>.
       </div>
     </div>
@@ -65,14 +65,14 @@
        {% else %} Did you get asked for your {{config.site_name}} password during this process? You can securely use your Hg repository and avoid having to re-enter your password by asking your server admin to enable uploading ssh keys. {% endif %}
       </div>
     </div>
     {% else %}
     <p><b>No (more) commits</b></p>
     {% endif %}
   {% elif c.app.repo.status == 'ready' %}
-    {% if h.has_access(c.app, 'write')() %}
+    {% if h.has_access(c.app, 'write') %}
     <p>Browsing this repo on the web is unavailable currently.  To fix, please try a <a href="{{c.app.url}}refresh">Repository Refresh</a>.  Committing and pulling code should still work.</p>
     {% else %}
     <p><b>No (more) commits</b></p>
     {% endif %}
   {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 {% endblock %} {% block header %}{{c.app.config.options.mount_label}}{%
 endblock %} {% block content %} {{ clone_info(c.app.repo) }}
  
 {% if log %}
 ********** RReecceenntt CCoommmmiittss{{%% iiff bbrraanncchh %%}} oonn {{{{bbrraanncchh}}}}{{%% eennddiiff %%}} **********
 {{c.log_widget.display(value=log, show_paging=False, limit=limit, page=page,
 count=count)}} {% if int(count) > int(limit) %} _M_o_r_e {% endif %} {% elif
-is_empty %} {% if h.has_access(c.app, 'write')() %}
+is_empty %} {% if h.has_access(c.app, 'write') %}
 [{{g.app_static('images/hg.png')}}]
 ********** NNeeww ttoo MMeerrccuurriiaall?? **********
 _L_e_a_r_n_ _t_h_e_ _b_a_s_i_c_s.
 ** EEmmppttyy RReeppoossiittoorryy **
 It looks like this Mercurial repository doesn't have any files in it. Let's
 commit your project code now.
 ********** FFiirrsstt ttiimmee uussiinngg MMeerrccuurriiaall **********
@@ -37,13 +37,13 @@
 _a_n_ _s_s_h_-_k_e_y. {% else %} Did you get asked for your {{config.site_name}} password
 during this process? You can securely use your Hg repository and avoid having
 to re-enter your password by asking your server admin to enable uploading ssh
 keys. {% endif %}
 {% else %}
 NNoo ((mmoorree)) ccoommmmiittss
 {% endif %} {% elif c.app.repo.status == 'ready' %} {% if h.has_access(c.app,
-'write')() %}
+'write') %}
 Browsing this repo on the web is unavailable currently. To fix, please try a
 _R_e_p_o_s_i_t_o_r_y_ _R_e_f_r_e_s_h. Committing and pulling code should still work.
 {% else %}
 NNoo ((mmoorree)) ccoommmmiittss
 {% endif %} {% endif %} {% endblock %}
```

### Comparing `ForgeHg-0.5.2/setup.py` & `ForgeHg-0.5.3/setup.py`

 * *Files identical despite different names*

