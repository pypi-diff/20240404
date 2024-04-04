# Comparing `tmp/stargazer-0.0.6.tar.gz` & `tmp/stargazer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stargazer-0.0.6.tar", last modified: Fri Jul 28 11:54:51 2023, max compression
+gzip compressed data, was "stargazer-0.0.7.tar", last modified: Thu Apr  4 13:11:43 2024, max compression
```

## Comparing `stargazer-0.0.6.tar` & `stargazer-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2023-07-28 11:54:51.036068 stargazer-0.0.6/
--rw-r--r--   0 pietro    (1000) pietro    (1000)      509 2019-10-12 15:25:47.000000 stargazer-0.0.6/LICENSE
--rw-r--r--   0 pietro    (1000) pietro    (1000)     6304 2023-07-28 11:54:51.036068 stargazer-0.0.6/PKG-INFO
--rw-r--r--   0 pietro    (1000) pietro    (1000)     5868 2023-07-24 22:39:27.000000 stargazer-0.0.6/README.md
--rw-r--r--   0 pietro    (1000) pietro    (1000)       38 2023-07-28 11:54:51.036068 stargazer-0.0.6/setup.cfg
--rw-r--r--   0 pietro    (1000) pietro    (1000)      653 2023-07-28 06:14:43.000000 stargazer-0.0.6/setup.py
-drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2023-07-28 11:54:51.036068 stargazer-0.0.6/stargazer/
--rw-r--r--   0 pietro    (1000) pietro    (1000)       19 2019-10-12 15:25:47.000000 stargazer-0.0.6/stargazer/__init__.py
--rw-r--r--   0 pietro    (1000) pietro    (1000)    31325 2023-07-22 22:42:06.000000 stargazer-0.0.6/stargazer/stargazer.py
--rw-r--r--   0 pietro    (1000) pietro    (1000)     1107 2021-10-12 16:00:48.000000 stargazer-0.0.6/stargazer/utils.py
-drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2023-07-28 11:54:51.036068 stargazer-0.0.6/stargazer.egg-info/
--rw-r--r--   0 pietro    (1000) pietro    (1000)     6304 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/PKG-INFO
--rw-r--r--   0 pietro    (1000) pietro    (1000)      222 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/SOURCES.txt
--rw-r--r--   0 pietro    (1000) pietro    (1000)        1 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/dependency_links.txt
--rw-r--r--   0 pietro    (1000) pietro    (1000)       10 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/top_level.txt
+drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2024-04-04 13:11:43.986517 stargazer-0.0.7/
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      509 2019-10-12 15:25:47.000000 stargazer-0.0.7/LICENSE
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     6304 2024-04-04 13:11:43.986517 stargazer-0.0.7/PKG-INFO
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     5868 2023-07-24 22:39:27.000000 stargazer-0.0.7/README.md
+-rw-r--r--   0 pietro    (1000) pietro    (1000)       38 2024-04-04 13:11:43.986517 stargazer-0.0.7/setup.cfg
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      653 2024-04-04 13:10:16.000000 stargazer-0.0.7/setup.py
+drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2024-04-04 13:11:43.986517 stargazer-0.0.7/stargazer/
+-rw-r--r--   0 pietro    (1000) pietro    (1000)       19 2019-10-12 15:25:47.000000 stargazer-0.0.7/stargazer/__init__.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     2076 2023-08-16 07:38:22.000000 stargazer-0.0.7/stargazer/label.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)    30952 2024-01-20 06:50:46.000000 stargazer-0.0.7/stargazer/stargazer.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      686 2024-01-20 06:51:11.000000 stargazer-0.0.7/stargazer/starlib.py
+drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2024-04-04 13:11:43.986517 stargazer-0.0.7/stargazer/translators/
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      308 2023-12-06 06:11:54.000000 stargazer-0.0.7/stargazer/translators/__init__.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     2743 2023-12-22 10:01:59.000000 stargazer-0.0.7/stargazer/translators/linearmodels.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     2271 2023-11-24 13:47:57.000000 stargazer-0.0.7/stargazer/translators/statsmodels.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     1650 2023-08-16 07:55:13.000000 stargazer-0.0.7/stargazer/utils.py
+drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2024-04-04 13:11:43.986517 stargazer-0.0.7/stargazer.egg-info/
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     6304 2024-04-04 13:11:43.000000 stargazer-0.0.7/stargazer.egg-info/PKG-INFO
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      371 2024-04-04 13:11:43.000000 stargazer-0.0.7/stargazer.egg-info/SOURCES.txt
+-rw-r--r--   0 pietro    (1000) pietro    (1000)        1 2024-04-04 13:11:43.000000 stargazer-0.0.7/stargazer.egg-info/dependency_links.txt
+-rw-r--r--   0 pietro    (1000) pietro    (1000)       10 2024-04-04 13:11:43.000000 stargazer-0.0.7/stargazer.egg-info/top_level.txt
```

### Comparing `stargazer-0.0.6/PKG-INFO` & `stargazer-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stargazer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Nicely formatted regression reporting
 Home-page: https://github.com/StatsReporting/stargazer
 Author: Pietro Battiston, Matthew Burke
 Author-email: me@pietrobattiston.it, matthew.wesley.burke@gmail.com
 License: GPLv2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `stargazer-0.0.6/README.md` & `stargazer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `stargazer-0.0.6/setup.py` & `stargazer-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stargazer",
-    version="0.0.6",
+    version="0.0.7",
     author="Pietro Battiston, Matthew Burke",
     author_email="me@pietrobattiston.it, matthew.wesley.burke@gmail.com",
     description="Nicely formatted regression reporting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/StatsReporting/stargazer",
     packages=setuptools.find_packages(),
```

### Comparing `stargazer-0.0.6/stargazer/stargazer.py` & `stargazer-0.0.7/stargazer/stargazer.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,71 +9,92 @@
         me@pietrobattiston.it
         https://pietrobattiston.it
     Matthew Burke:
         matthew.wesley.burke@gmail.com
         github.com/mwburke
 """
 
-from statsmodels.base.wrapper import ResultsWrapper
-from statsmodels.regression.linear_model import RegressionResults
-from math import sqrt
 from collections import defaultdict
 from enum import Enum
 import numbers
 import pandas as pd
 
+from .label import Label
+from .starlib import _find_duplicates
+
+RESULTS_CLASSES = {}
+
+from .translators import *
+
 class LineLocation(Enum):
     HEADER_TOP = 'ht'
     HEADER_BOTTOM = 'hb'
     BODY_TOP = 'bt'
     BODY_BOTTOM = 'bb'
     FOOTER_TOP = 'ft'
     FOOTER_BOTTOM = 'fb'
 
-
 class Stargazer:
     """
-    Class that is constructed with one or more trained
-    OLS models from the statsmodels package.
+    Class that is constructed with one or more trained statistical models, for
+    instance from the statsmodels package.
 
     The user then can change the rendering options by
     chaining different methods to the Stargazer object
     and then render the results in either HTML or LaTeX.
     """
 
-    # This is a mapping from 'show_*' attribute to name of generating method
-    # "_generate_{LABEL}" (if present) and to name of stat in data store
-    # otherwise.
+    # The following tuple represents a mapping from 'show_*' attribute to
+    # - name of generating method "_generate_{LABEL}" (if present) and
+    #   name of stat in data store otherwise.
+    # - label, in the form of a str or a Label
     # Stats will be automatically formatted. Order matters!
-    _auto_stats = [('n', 'nobs'),
-                   ('r2', 'r2'),
-                   ('adj_r2', 'r2_adj'),
-                   ('residual_std_err', 'resid_std_err'),
-                   ('f_statistic', 'f_statistic')]
+    # Note that a stat is automatically hidden if none of the models displayed
+    # has it.
+
+    _auto_stats = [('n', 'nobs', 'Observations'),
+
+                   ('ngroups', 'ngroups', 'N. of groups'),
+
+                   ('r2', 'r2',
+                    Label({'LaTeX' : '$R^2$',
+                           'html' : 'R<sup>2</sup>'})),
+
+                   ('within_r2', 'within_r2',
+                    Label({'LaTeX' : 'Within $R^2$',
+                           'html' : 'Within R<sup>2</sup>'})),
+
+                   ('adj_r2', 'r2_adj',
+                    Label({'LaTeX' : 'Adjusted $R^2$',
+                           'html' : 'Adjusted R<sup>2</sup>'})),
+
+                   ('pseudo_r2', 'pseudo_r2',
+                    Label({'LaTeX' : 'Pseudo $R^2$',
+                           'html' : 'Pseudo R<sup>2</sup>'})),
+
+                   ('residual_std_err', 'resid_std_err',
+                    'Residual Std. Error'),
+
+                   ('f_statistic', 'f_statistic', 'F Statistic')]
 
     def __init__(self, models):
         self.models = models
         self.num_models = len(models)
         self.reset_params()
         self.extract_data()
 
     def validate_input(self):
         """
         Check inputs to see if they are going to
         cause any problems further down the line.
 
         Any future checking will be added here.
         """
-        targets = []
 
-        for m in self.models:
-            if not isinstance(m, (ResultsWrapper,
-                                  RegressionResults)):
-                raise ValueError('Please use trained OLS models as inputs')
-            targets.append(m.model.endog_names)
+        targets = [mod['dependent_variable'] for mod in self.model_data]
 
         if targets.count(targets[0]) != len(targets):
             self.dependent_variable = ''
             self.dep_var_name = None
         else:
             self.dependent_variable = targets[0]
 
@@ -88,26 +109,30 @@
         self.title_text = None
         self.show_header = True
         self.dep_var_name = 'Dependent variable: '
         self.column_labels = None
         self.column_separators = None
         self.show_model_nums = True
         self.original_cov_names = None
-        self.cov_map = None
+        self.cov_map = lambda x : x
         self.cov_spacing = None
         self.show_precision = True
         self.show_sig = True
         self.sig_levels = [0.1, 0.05, 0.01]
         self.sig_digits = 3
         self.confidence_intervals = False
         self.show_footer = True
         self.custom_lines = defaultdict(list)
         self.show_n = True
+        self.show_ngroups = True
         self.show_r2 = True
+        # Off by default, as discussed in GH #98:
+        self.show_within_r2 = False
         self.show_adj_r2 = True
+        self.show_pseudo_r2 = True
         self.show_residual_std_err = True
         self.show_f_statistic = True
         self.show_dof = True
         self.show_notes = True
         self.notes_label = 'Note:'
         self.notes_append = True
         self.custom_notes = []
@@ -116,76 +141,37 @@
 
     def extract_data(self):
         """
         Extract the values we need from the models and store
         for use or modification. They should not be able to
         be modified by any rendering parameters.
         """
-        self.validate_input()
         self.model_data = []
         for m in self.models:
             self.model_data.append(self.extract_model_data(m))
 
         covs = []
         for md in self.model_data:
             covs = covs + list(md['cov_names'])
         self.cov_names = sorted(set(covs))
 
-    def _extract_feature(self, obj, feature):
+        self.validate_input()
+
+    def extract_model_data(self, model):
         """
-        Just return obj.feature if present and None otherwise.
+        Call appropriate (library-specific) data extractor.
         """
-        try:
-            return getattr(obj, feature)
-        except AttributeError:
-            return None
 
-    def extract_model_data(self, model):
-        # For features that are simple attributes of "model", establish the
-        # mapping with internal name (TODO: adopt same names?):
-        statsmodels_map = {'p_values' : 'pvalues',
-                           'cov_values' : 'params',
-                           'cov_std_err' : 'bse',
-                           'r2' : 'rsquared',
-                           'r2_adj' : 'rsquared_adj',
-                           'f_p_value' : 'f_pvalue',
-                           'degree_freedom' : 'df_model',
-                           'degree_freedom_resid' : 'df_resid',
-                           'nobs' : 'nobs',
-                           'f_statistic' : 'fvalue'
-                           }
-
-        data = {}
-        for key, val in statsmodels_map.items():
-            data[key] = self._extract_feature(model, val)
+        for klass in model.__class__.__mro__:
+            if klass in RESULTS_CLASSES:
+                extractor = RESULTS_CLASSES[klass]
 
-        if isinstance(model, ResultsWrapper):
-            data['cov_names'] = model.params.index.values
-        else:
-            # Simple RegressionResults, for instance as a result of
-            # get_robustcov_results():
-            data['cov_names'] = model.model.data.orig_exog.columns
-
-            # These are simple arrays, not Series:
-            for what in 'cov_values', 'p_values', 'cov_std_err':
-                data[what] = pd.Series(data[what],
-                                       index=data['cov_names'])
-
-        data['conf_int_low_values'] = model.conf_int()[0]
-        data['conf_int_high_values'] = model.conf_int()[1]
-        data['resid_std_err'] = (sqrt(sum(model.resid**2) / model.df_resid)
-                                 if hasattr(model, 'resid') else None)
-
-        # Workaround for
-        # https://github.com/statsmodels/statsmodels/issues/6778:
-        if 'f_statistic' in data:
-            data['f_statistic'] = (lambda x : x[0, 0] if getattr(x, 'ndim', 0)
-                                   else x)(data['f_statistic'])
+                return extractor(model)
 
-        return data
+        raise NotImplementedError(model.__class__)
 
     # Begin render option functions
     def title(self, title):
         self.title_text = title
 
     def show_header(self, show):
         assert type(show) == bool, 'Please input True/False'
@@ -237,24 +223,53 @@
         assert type(show) == bool, 'Please input True/False'
         self.confidence_intervals = show
 
     def dependent_variable_name(self, name):
         assert type(name) == str, 'Please input a string to use as the depedent variable name'
         self.dependent_variable = name
 
-    def covariate_order(self, cov_names):
+    def covariate_order(self, cov_names, restrict=True):
+        """
+        Specify order and subset of covariates.
+
+        Paramters
+        ---------
+        cov_names : list of str
+            Covariate names, or a subset of them, in the desired order.
+        restrict : bool, default True
+            Whether covariates not included in "cov_names" should be dropped;
+            otherwise, they are just appended, in their default order.
+        """
+
+        duplicates = _find_duplicates(cov_names)
+        assert not duplicates, ('Covariates must not be repeated, the '
+                                f'following are: {duplicates}')
+
+
         missing = set(cov_names).difference(set(self.cov_names))
         assert not missing, ('Covariate order must contain subset of existing '
                              'covariates: {} are not.'.format(missing))
+
+        if not restrict:
+            others = [name for name in self.cov_names if name not in cov_names]
+            cov_names += others
+
         self.original_cov_names = self.cov_names
         self.cov_names = cov_names
 
     def rename_covariates(self, cov_map):
-        assert isinstance(cov_map, dict), 'Please input a dictionary with covariate names as keys'
-        self.cov_map = cov_map
+        if hasattr(cov_map, "get"):
+            self.cov_map = lambda k : cov_map.get(k, k)
+        elif callable(cov_map):
+            self.cov_map = cov_map
+        else:
+            msg = ('"rename_covariates" must receive either a dictionary with '
+                   'covariate names as keys, or a function accepting any '
+                   'covariate name as input and returning the new name.')
+            raise ValueError(msg)
 
     def reset_covariate_order(self):
         if self.original_cov_names is not None:
             self.cov_names = self.original_cov_names
 
     def add_line(self, label, values, location=LineLocation.BODY_BOTTOM):
         """
@@ -291,34 +306,41 @@
         self.custom_notes = notes
 
     def append_notes(self, append):
         assert type(append) == bool, 'Please input True/False'
         self.notes_append = append
 
     def render_html(self, *args, **kwargs):
-        return HTMLRenderer(self).render(*args, **kwargs)
+        with Label.context('html'):
+            return HTMLRenderer(self).render(*args, **kwargs)
 
     def _repr_html_(self):
         return self.render_html()
 
     def render_latex(self, *args, escape=False, **kwargs):
         """
         Render as LaTeX code.
 
         Parameters
         ----------
         escape : bool
             Escape special characters.
+            To prevent a specific string from being escaped, just pass it as
+
+                Label({'LaTeX' : 'the_string'})
+
+            ... it will be left unchanged.
 
         Returns
         -------
         str
             The LaTeX code.
         """
-        return LaTeXRenderer(self, escape=escape).render(*args, **kwargs)
+        with Label.context('LaTeX'):
+            return LaTeXRenderer(self, escape=escape).render(*args, **kwargs)
 
 
 class Renderer:
     """
     Base class for renderers to specific formats. Only meant to be subclassed.
     """
 
@@ -404,26 +426,19 @@
         return f_text
 
     def _generate_stat_values(self, stat):
         if hasattr(self, f'_generate_{stat}'):
             generator = getattr(self, f'_generate_{stat}')
             return [generator(md) for md in self.model_data]
         else:
-            return [md[stat] for md in self.model_data]
+            return [md.get(stat, None) for md in self.model_data]
 
 class HTMLRenderer(Renderer):
     fmt = 'html'
 
-    # Labels for stats in Stargazer._auto_stats:
-    _stats_labels = {'n' : 'Observations',
-                     'r2' : 'R<sup>2</sup>',
-                     'adj_r2' : 'Adjusted R<sup>2</sup>',
-                     'residual_std_err' : 'Residual Std. Error',
-                     'f_statistic' : 'F Statistic'}
-
     def render(self):
         html = self.generate_header()
         html += self.generate_body()
         html += self.generate_footer()
         return html
 
     def generate_header(self):
@@ -501,17 +516,16 @@
             cov_text += self.generate_cov_precision(cov_name, spacing=spacing)
         else:
             cov_text += '<tr></tr>'
 
         return cov_text
 
     def generate_cov_main(self, cov_name, spacing):
-        cov_print_name = cov_name
-        if self.cov_map is not None:
-            cov_print_name = self.cov_map.get(cov_print_name, cov_name)
+        cov_print_name = self.cov_map(cov_name)
+
         cov_text = (f'<tr><td style="text-align:left">'
                     f'{cov_print_name}</td>')
         for md in self.model_data:
             if cov_name in md['cov_names']:
                 cov_text += f'<td{spacing}>'
                 cov_text += self._float_format(md['cov_values'][cov_name])
                 if self.show_sig:
@@ -551,17 +565,17 @@
         """
         footer = '<td colspan="' + str(self.num_models + 1) + '" style="border-bottom: 1px solid black"></td></tr>'
 
         if not self.show_footer:
             return footer
         footer += self.generate_custom_lines(LineLocation.FOOTER_TOP)
 
-        for attr, stat in Stargazer._auto_stats:
+        for attr, stat, label in Stargazer._auto_stats:
             if getattr(self, f'show_{attr}'):
-                footer += self.generate_stat(stat, self._stats_labels[attr])
+                footer += self.generate_stat(stat, label)
 
         footer += self.generate_custom_lines(LineLocation.FOOTER_BOTTOM)
         footer += '<tr><td colspan="' + str(self.num_models + 1) + '" style="border-bottom: 1px solid black"></td></tr>'
         if self.show_notes:
             footer += self.generate_notes()
         footer += '</table>'
 
@@ -619,21 +633,14 @@
             notes_text += '<td colspan="' + str(self.num_models+1) + '" style="text-align: right">' + note + '</td></tr>'
 
         return notes_text
 
 class LaTeXRenderer(Renderer):
     fmt = 'LaTeX'
 
-    # Labels for stats in Stargazer._auto_stats:
-    _stats_labels = {'n' : 'Observations',
-                     'r2' : '$R^2$',
-                     'adj_r2' : 'Adjusted $R^2$',
-                     'residual_std_err' : 'Residual Std. Error',
-                     'f_statistic' : 'F Statistic'}
-
     # LaTeX escape characters, borrowed from pandas.io.formats.latex
     _ESCAPE_CHARS = [
         ('\\', r'\textbackslash '),
         ('_', r'\_'),
         ('%', r'\%'),
         ('$', r'\$'),
         ('#', r'\#'),
@@ -641,15 +648,22 @@
         ('}', r'\}'),
         ('~', r'\textasciitilde '),
         ('^', r'\textasciicircum '),
         ('&', r'\&')
     ]
 
     def _escape(self, text):
-        """Escape LaTeX special characters"""
+        """
+        Escape LaTeX special characters
+        """
+
+        if isinstance(text, Label) and text.specific():
+            # Do _not_ escape characters of a LaTeX-specific string:
+            return text
+
         if self.kwargs.get('escape', False):
             for orig_char, escape_char in LaTeXRenderer._ESCAPE_CHARS:
                 text = text.replace(orig_char, escape_char)
         return text
 
     def render(self, only_tabular=False, insert_empty_rows=False):
         latex = self.generate_header(only_tabular=only_tabular)
@@ -674,17 +688,18 @@
         content_columns = 'c' * self.num_models
         header += '\\begin{tabular}{@{\\extracolsep{5pt}}l' + content_columns + '}\n'
         header += '\\\\[-1.8ex]\\hline\n'
         header += '\\hline \\\\[-1.8ex]\n'
         header += self.generate_custom_lines(LineLocation.HEADER_TOP)
 
         if self.dep_var_name is not None:
-            header += '& \\multicolumn{' + str(self.num_models) + '}{c}'
-            header += '{\\textit{' + self.dep_var_name + self.dependent_variable + '}} \\\n'
-            header += '\\cr \\cline{2-' + str(self.num_models + 1) + '}\n'
+            header += (f'& \\multicolumn{{{self.num_models}}}{{c}}'
+                       f'{{\\textit{{{self.dep_var_name}'
+                       f'{self._escape(self.dependent_variable)}}}}} \\\n'
+                       f'\\cr \\cline{{2-{self.num_models + 1}}}\n')
 
         if self.column_labels is not None:
             if type(self.column_labels) == str:
                 header += '\\\\[-1.8ex] & \\multicolumn{' + str(self.num_models) + '}{c}{' + self._escape(self.column_labels) + '} \\\\'
             else:
                 header += '\\\\[-1.8ex] '
                 for i, label in enumerate(self.column_labels):
@@ -739,21 +754,17 @@
             cov_text += self.generate_cov_precision(cov_name)
         else:
             cov_text += '& '
 
         return cov_text
 
     def generate_cov_main(self, cov_name):
-        cov_print_name = cov_name
-
-        if self.cov_map is not None:
-            if cov_name in self.cov_map:
-                cov_print_name = self.cov_map[cov_name]
+        cov_print_name = self.cov_map(cov_name)
 
-        cov_text = ' ' + self._escape(cov_print_name) + ' '
+        cov_text = f' {self._escape(cov_print_name)} '
         for md in self.model_data:
             if cov_name in md['cov_names']:
                 cov_text += '& ' + self._float_format(md['cov_values'][cov_name])
                 if self.show_sig:
                     cov_text += self._format_sig_icon(md['p_values'][cov_name])
                 cov_text += ' '
             else:
@@ -786,17 +797,17 @@
 
         footer = '\\hline \\\\[-1.8ex]\n'
 
         if not self.show_footer:
             return footer
         footer += self.generate_custom_lines(LineLocation.FOOTER_TOP)
 
-        for attr, stat in Stargazer._auto_stats:
+        for attr, stat, label in Stargazer._auto_stats:
             if getattr(self, f'show_{attr}'):
-                footer += self.generate_stat(stat, self._stats_labels[attr])
+                footer += self.generate_stat(stat, label)
 
         footer += self.generate_custom_lines(LineLocation.FOOTER_BOTTOM)
         footer += '\\hline\n\\hline \\\\[-1.8ex]\n'
         if self.show_notes:
             footer += self.generate_notes()
         footer += '\\end{tabular}'
```

### Comparing `stargazer-0.0.6/stargazer.egg-info/PKG-INFO` & `stargazer-0.0.7/stargazer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stargazer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Nicely formatted regression reporting
 Home-page: https://github.com/StatsReporting/stargazer
 Author: Pietro Battiston, Matthew Burke
 Author-email: me@pietrobattiston.it, matthew.wesley.burke@gmail.com
 License: GPLv2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

