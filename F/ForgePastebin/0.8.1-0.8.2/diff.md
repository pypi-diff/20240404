# Comparing `tmp/ForgePastebin-0.8.1.tar.gz` & `tmp/ForgePastebin-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForgePastebin-0.8.1.tar", last modified: Fri Aug 18 21:10:18 2023, max compression
+gzip compressed data, was "ForgePastebin-0.8.2.tar", last modified: Thu Apr  4 20:55:02 2024, max compression
```

## Comparing `ForgePastebin-0.8.1.tar` & `ForgePastebin-0.8.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.959287 ForgePastebin-0.8.1/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.945218 ForgePastebin-0.8.1/ForgePastebin.egg-info/
--rw-r--r--   0 brondsem   (502) staff       (20)      262 2023-08-18 21:10:18.000000 ForgePastebin-0.8.1/ForgePastebin.egg-info/PKG-INFO
--rw-r--r--   0 brondsem   (502) staff       (20)      894 2023-08-18 21:10:18.000000 ForgePastebin-0.8.1/ForgePastebin.egg-info/SOURCES.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2023-08-18 21:10:18.000000 ForgePastebin-0.8.1/ForgePastebin.egg-info/dependency_links.txt
--rw-r--r--   0 brondsem   (502) staff       (20)       52 2023-08-18 21:10:18.000000 ForgePastebin-0.8.1/ForgePastebin.egg-info/entry_points.txt
--rw-r--r--   0 brondsem   (502) staff       (20)       14 2023-08-18 21:10:18.000000 ForgePastebin-0.8.1/ForgePastebin.egg-info/top_level.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2020-12-31 17:47:17.000000 ForgePastebin-0.8.1/ForgePastebin.egg-info/zip-safe
--rw-r--r--   0 brondsem   (502) staff       (20)       81 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/MANIFEST.in
--rw-r--r--   0 brondsem   (502) staff       (20)      262 2023-08-18 21:10:18.958812 ForgePastebin-0.8.1/PKG-INFO
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.947826 ForgePastebin-0.8.1/forgepastebin/
--rw-r--r--   0 brondsem   (502) staff       (20)        0 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/forgepastebin/__init__.py
--rw-r--r--   0 brondsem   (502) staff       (20)     8207 2023-01-13 19:08:09.000000 ForgePastebin-0.8.1/forgepastebin/app.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.949248 ForgePastebin-0.8.1/forgepastebin/controllers/
--rw-r--r--   0 brondsem   (502) staff       (20)        0 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/forgepastebin/controllers/__init__.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.950294 ForgePastebin-0.8.1/forgepastebin/model/
--rw-r--r--   0 brondsem   (502) staff       (20)       25 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/forgepastebin/model/__init__.py
--rw-r--r--   0 brondsem   (502) staff       (20)     1832 2023-08-18 20:32:29.000000 ForgePastebin-0.8.1/forgepastebin/model/paste.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.940044 ForgePastebin-0.8.1/forgepastebin/nf/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.940532 ForgePastebin-0.8.1/forgepastebin/nf/pastebin/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.951004 ForgePastebin-0.8.1/forgepastebin/nf/pastebin/css/
--rw-r--r--   0 brondsem   (502) staff       (20)     4236 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/forgepastebin/nf/pastebin/css/pygments.css
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.953273 ForgePastebin-0.8.1/forgepastebin/nf/pastebin/images/
--rw-r--r--   0 brondsem   (502) staff       (20)     3626 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/forgepastebin/nf/pastebin/images/pastebin_24.png
--rw-r--r--   0 brondsem   (502) staff       (20)     3966 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/forgepastebin/nf/pastebin/images/pastebin_32.png
--rw-r--r--   0 brondsem   (502) staff       (20)     4705 2013-02-19 19:30:18.000000 ForgePastebin-0.8.1/forgepastebin/nf/pastebin/images/pastebin_48.png
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.954858 ForgePastebin-0.8.1/forgepastebin/templates/
--rw-r--r--   0 brondsem   (502) staff       (20)      319 2019-03-21 17:56:43.000000 ForgePastebin-0.8.1/forgepastebin/templates/new.html
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.956068 ForgePastebin-0.8.1/forgepastebin/templates/paste/
--rw-r--r--   0 brondsem   (502) staff       (20)     1183 2019-03-21 17:56:43.000000 ForgePastebin-0.8.1/forgepastebin/templates/paste/paste.html
--rw-r--r--   0 brondsem   (502) staff       (20)      143 2019-03-21 17:56:43.000000 ForgePastebin-0.8.1/forgepastebin/templates/paste/paste.js
--rw-r--r--   0 brondsem   (502) staff       (20)      898 2019-03-21 17:56:43.000000 ForgePastebin-0.8.1/forgepastebin/templates/pastes.html
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.956725 ForgePastebin-0.8.1/forgepastebin/templates/widgets/
--rw-r--r--   0 brondsem   (502) staff       (20)      551 2019-03-21 17:56:43.000000 ForgePastebin-0.8.1/forgepastebin/templates/widgets/paste_form.html
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-08-18 21:10:18.957899 ForgePastebin-0.8.1/forgepastebin/tests/
--rw-r--r--   0 brondsem   (502) staff       (20)        0 2019-03-21 17:56:43.000000 ForgePastebin-0.8.1/forgepastebin/tests/__init__.py
--rw-r--r--   0 brondsem   (502) staff       (20)     1627 2023-01-13 19:08:09.000000 ForgePastebin-0.8.1/forgepastebin/tests/test_functional.py
--rw-r--r--   0 brondsem   (502) staff       (20)       80 2023-08-18 21:06:47.000000 ForgePastebin-0.8.1/forgepastebin/version.py
--rw-r--r--   0 brondsem   (502) staff       (20)     1489 2023-01-13 19:08:09.000000 ForgePastebin-0.8.1/forgepastebin/widgets.py
--rw-r--r--   0 brondsem   (502) staff       (20)       38 2023-08-18 21:10:18.959388 ForgePastebin-0.8.1/setup.cfg
--rw-r--r--   0 brondsem   (502) staff       (20)      895 2023-01-13 19:08:09.000000 ForgePastebin-0.8.1/setup.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.609991 ForgePastebin-0.8.2/
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.609541 ForgePastebin-0.8.2/ForgePastebin.egg-info/
+-rw-r--r--   0 brondsem   (501) staff       (20)      262 2024-04-04 20:55:02.000000 ForgePastebin-0.8.2/ForgePastebin.egg-info/PKG-INFO
+-rw-r--r--   0 brondsem   (501) staff       (20)      894 2024-04-04 20:55:02.000000 ForgePastebin-0.8.2/ForgePastebin.egg-info/SOURCES.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)        1 2024-04-04 20:55:02.000000 ForgePastebin-0.8.2/ForgePastebin.egg-info/dependency_links.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)       52 2024-04-04 20:55:02.000000 ForgePastebin-0.8.2/ForgePastebin.egg-info/entry_points.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)       14 2024-04-04 20:55:02.000000 ForgePastebin-0.8.2/ForgePastebin.egg-info/top_level.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)        1 2020-12-31 17:47:17.000000 ForgePastebin-0.8.2/ForgePastebin.egg-info/zip-safe
+-rw-r--r--   0 brondsem   (501) staff       (20)       81 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/MANIFEST.in
+-rw-r--r--   0 brondsem   (501) staff       (20)      262 2024-04-04 20:55:02.609769 ForgePastebin-0.8.2/PKG-INFO
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.606282 ForgePastebin-0.8.2/forgepastebin/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/forgepastebin/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     8193 2024-04-04 20:09:58.000000 ForgePastebin-0.8.2/forgepastebin/app.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.606588 ForgePastebin-0.8.2/forgepastebin/controllers/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/forgepastebin/controllers/__init__.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.607012 ForgePastebin-0.8.2/forgepastebin/model/
+-rw-r--r--   0 brondsem   (501) staff       (20)       25 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/forgepastebin/model/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1832 2023-08-18 20:32:29.000000 ForgePastebin-0.8.2/forgepastebin/model/paste.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.603734 ForgePastebin-0.8.2/forgepastebin/nf/
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.603841 ForgePastebin-0.8.2/forgepastebin/nf/pastebin/
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.607314 ForgePastebin-0.8.2/forgepastebin/nf/pastebin/css/
+-rw-r--r--   0 brondsem   (501) staff       (20)     4236 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/forgepastebin/nf/pastebin/css/pygments.css
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.608010 ForgePastebin-0.8.2/forgepastebin/nf/pastebin/images/
+-rw-r--r--   0 brondsem   (501) staff       (20)     3626 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/forgepastebin/nf/pastebin/images/pastebin_24.png
+-rw-r--r--   0 brondsem   (501) staff       (20)     3966 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/forgepastebin/nf/pastebin/images/pastebin_32.png
+-rw-r--r--   0 brondsem   (501) staff       (20)     4705 2013-02-19 19:30:18.000000 ForgePastebin-0.8.2/forgepastebin/nf/pastebin/images/pastebin_48.png
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.608420 ForgePastebin-0.8.2/forgepastebin/templates/
+-rw-r--r--   0 brondsem   (501) staff       (20)      319 2019-03-21 17:56:43.000000 ForgePastebin-0.8.2/forgepastebin/templates/new.html
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.608849 ForgePastebin-0.8.2/forgepastebin/templates/paste/
+-rw-r--r--   0 brondsem   (501) staff       (20)     1183 2019-03-21 17:56:43.000000 ForgePastebin-0.8.2/forgepastebin/templates/paste/paste.html
+-rw-r--r--   0 brondsem   (501) staff       (20)      143 2019-03-21 17:56:43.000000 ForgePastebin-0.8.2/forgepastebin/templates/paste/paste.js
+-rw-r--r--   0 brondsem   (501) staff       (20)      898 2019-03-21 17:56:43.000000 ForgePastebin-0.8.2/forgepastebin/templates/pastes.html
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.609047 ForgePastebin-0.8.2/forgepastebin/templates/widgets/
+-rw-r--r--   0 brondsem   (501) staff       (20)      551 2019-03-21 17:56:43.000000 ForgePastebin-0.8.2/forgepastebin/templates/widgets/paste_form.html
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-04-04 20:55:02.609327 ForgePastebin-0.8.2/forgepastebin/tests/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2019-03-21 17:56:43.000000 ForgePastebin-0.8.2/forgepastebin/tests/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1627 2023-01-13 19:08:09.000000 ForgePastebin-0.8.2/forgepastebin/tests/test_functional.py
+-rw-r--r--   0 brondsem   (501) staff       (20)       80 2024-04-04 20:11:30.000000 ForgePastebin-0.8.2/forgepastebin/version.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1489 2023-01-13 19:08:09.000000 ForgePastebin-0.8.2/forgepastebin/widgets.py
+-rw-r--r--   0 brondsem   (501) staff       (20)       38 2024-04-04 20:55:02.610045 ForgePastebin-0.8.2/setup.cfg
+-rw-r--r--   0 brondsem   (501) staff       (20)      895 2023-01-13 19:08:09.000000 ForgePastebin-0.8.2/setup.py
```

### Comparing `ForgePastebin-0.8.1/ForgePastebin.egg-info/SOURCES.txt` & `ForgePastebin-0.8.2/ForgePastebin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/app.py` & `ForgePastebin-0.8.2/forgepastebin/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     @h.exceptionless([], log)
     def sitemap(self):
         menu_id = self.config.options.mount_label.title()
         return [SitemapEntry(menu_id, '.')[self.sidebar_menu()] ]
 
     def sidebar_menu(self):
         links = []
-        if has_access(self, 'write')():
+        if has_access(self, 'write'):
             links.append(SitemapEntry('New Paste',
                 self.config.url() + 'new', ui_icon=g.icons['add']))
         links.append(SitemapEntry('Recent Pastes',
             self.config.url()))
         return links
 
     def admin_menu(self):
@@ -106,15 +106,15 @@
     @expose()
     def _lookup(self, paste_id, *remainder):
         return PasteController(paste_id), remainder
 
     @expose('jinja:forgepastebin:templates/new.html')
     def new(self, ref_id=None, **kw):
         require_access(c.app, 'write')
-        allow_private = has_access(c.app, 'private')()
+        allow_private = has_access(c.app, 'private')
         c.paste_form = W.paste_form()
         ctx = dict(
                 allow_private=allow_private,
                 private=c.app.config.options.get('private_by_default', False),
             )
         if ref_id is not None:
             ref_paste = PBM.Paste.query.get(_id=ObjectId(ref_id))
@@ -124,24 +124,24 @@
                 ctx['private'] = ref_paste.private
         return ctx
 
     @require_post()
     @expose()
     def create(self, text, lang, private=False, **kw):
         require_access(c.app, 'write')
-        allow_private = has_access(c.app, 'private')()
+        allow_private = has_access(c.app, 'private')
         if not allow_private:
             private = False
         p = PBM.Paste(creator_id=c.user._id, text=text, lang=lang, private=asbool(private))
         redirect(p.url())
 
     @expose('jinja:forgepastebin:templates/pastes.html')
     def index(self, **kw):
         query = dict(deleted=False)
-        if not has_access(c.app, 'private')():
+        if not has_access(c.app, 'private'):
             query['private'] = {'$in': [None, False]}
         pastes = PBM.Paste.query.find(query).sort('mod_date',
                 pymongo.DESCENDING).limit(10).all()
         return dict(pastes=pastes)
 
     @with_trailing_slash
     @expose('jinja:forgepastebin:templates/pastes.html')
@@ -150,15 +150,15 @@
         results = []
         count=0
         limit, page, start = g.handle_paging(limit, page, default=25)
         if not q:
             q = ''
         else:
             try:
-                if not has_access(c.app, 'private')():
+                if not has_access(c.app, 'private'):
                     private = ['-is_private_b:true']
                 else:
                     private = []
                 results = search(
                     q, short_timeout=True, ignore_errors=False,
                     rows=limit, start=start,
                     fq=[
@@ -202,23 +202,23 @@
         if request.path.endswith('.js'):
             response.content_type = 'text/javascript'
             csslink = ew.CSSLink('tool/{}/{}'.format(c.app.config.tool_name.lower(), 'css/pygments.css'))
             g.resource_manager.register(csslink)
             css = six.moves.urllib.parse.urljoin('//%s' % request.host, csslink.url())
             return dict(paste=json.dumps(self.paste.html()), js=True, csslink=json.dumps(css))
         else:
-            is_admin = has_access(c.project, 'admin')()
+            is_admin = has_access(c.project, 'admin')
             is_anon = c.user == M.User.anonymous()
             is_owner = not is_anon and c.user._id == self.paste.creator_id
             return dict(paste=self.paste, js=False, can_delete=is_owner or is_admin)
 
     @without_trailing_slash
     @expose()
     def delete(self, **kw):
-        is_admin = has_access(c.project, 'admin')()
+        is_admin = has_access(c.project, 'admin')
         is_anon = c.user == M.User.anonymous()
         is_owner = not is_anon and c.user._id == self.paste.creator_id
         if not (is_owner or is_admin):
             raise exc.HTTPForbidden()
         self.paste.deleted = True
         redirect('..')
```

### Comparing `ForgePastebin-0.8.1/forgepastebin/model/paste.py` & `ForgePastebin-0.8.2/forgepastebin/model/paste.py`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/nf/pastebin/css/pygments.css` & `ForgePastebin-0.8.2/forgepastebin/nf/pastebin/css/pygments.css`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/nf/pastebin/images/pastebin_24.png` & `ForgePastebin-0.8.2/forgepastebin/nf/pastebin/images/pastebin_24.png`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/nf/pastebin/images/pastebin_32.png` & `ForgePastebin-0.8.2/forgepastebin/nf/pastebin/images/pastebin_32.png`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/nf/pastebin/images/pastebin_48.png` & `ForgePastebin-0.8.2/forgepastebin/nf/pastebin/images/pastebin_48.png`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/templates/paste/paste.html` & `ForgePastebin-0.8.2/forgepastebin/templates/paste/paste.html`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/templates/pastes.html` & `ForgePastebin-0.8.2/forgepastebin/templates/pastes.html`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/templates/widgets/paste_form.html` & `ForgePastebin-0.8.2/forgepastebin/templates/widgets/paste_form.html`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/tests/test_functional.py` & `ForgePastebin-0.8.2/forgepastebin/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/forgepastebin/widgets.py` & `ForgePastebin-0.8.2/forgepastebin/widgets.py`

 * *Files identical despite different names*

### Comparing `ForgePastebin-0.8.1/setup.py` & `ForgePastebin-0.8.2/setup.py`

 * *Files identical despite different names*

