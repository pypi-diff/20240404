# Comparing `tmp/feynamp-0.0.5.tar.gz` & `tmp/feynamp-0.0.5.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynamp-0.0.5.tar", max compression
+gzip compressed data, was "feynamp-0.0.5.12.tar", max compression
```

## Comparing `feynamp-0.0.5.tar` & `feynamp-0.0.5.12.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    35149 2024-03-31 20:19:53.021362 feynamp-0.0.5/LICENSE
--rw-r--r--   0        0        0      104 2024-03-31 20:19:53.021362 feynamp-0.0.5/README.md
--rw-r--r--   0        0        0     1358 2024-03-31 20:19:53.021362 feynamp-0.0.5/feynamp/__init__.py
--rw-r--r--   0        0        0     3135 2024-03-31 20:19:53.021362 feynamp-0.0.5/feynamp/amplitude.py
--rw-r--r--   0        0        0     3688 2024-03-31 20:19:53.021362 feynamp-0.0.5/feynamp/form/__init__.py
--rw-r--r--   0        0        0     2143 2024-03-31 20:19:53.021362 feynamp-0.0.5/feynamp/form/color.py
--rw-r--r--   0        0        0     5065 2024-03-31 20:19:53.021362 feynamp-0.0.5/feynamp/form/lorentz.py
--rw-r--r--   0        0        0     7007 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/form/momentum.py
--rw-r--r--   0        0        0     1687 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/leg.py
--rw-r--r--   0        0        0      213 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/log.py
--rw-r--r--   0        0        0      483 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/math.py
--rw-r--r--   0        0        0     2029 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/momentum.py
--rw-r--r--   0        0        0     1525 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/propagator.py
--rw-r--r--   0        0        0      577 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/sympy/__init__.py
--rw-r--r--   0        0        0     6314 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/sympy/color.py
--rw-r--r--   0        0        0     3383 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/sympy/lorentz.py
--rw-r--r--   0        0        0      465 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/util.py
--rw-r--r--   0        0        0     6275 2024-03-31 20:19:53.025362 feynamp-0.0.5/feynamp/vertex.py
--rw-r--r--   0        0        0     2118 2024-03-31 20:19:54.025359 feynamp-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 feynamp-0.0.5/setup.py
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 feynamp-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-04 09:31:27.109037 feynamp-0.0.5.12/LICENSE
+-rw-r--r--   0        0        0     1259 2024-04-04 09:31:27.109037 feynamp-0.0.5.12/README.md
+-rw-r--r--   0        0        0     1358 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/__init__.py
+-rw-r--r--   0        0        0     3373 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/amplitude.py
+-rw-r--r--   0        0        0     1651 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/__init__.py
+-rw-r--r--   0        0        0     2187 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/color.py
+-rw-r--r--   0        0        0     2191 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/form.py
+-rw-r--r--   0        0        0     8567 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/lorentz.py
+-rw-r--r--   0        0        0     7042 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/momentum.py
+-rw-r--r--   0        0        0     1687 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/leg.py
+-rw-r--r--   0        0        0      149 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/log.py
+-rw-r--r--   0        0        0      469 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/math.py
+-rw-r--r--   0        0        0     2029 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/momentum.py
+-rw-r--r--   0        0        0     1525 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/propagator.py
+-rw-r--r--   0        0        0      577 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/sympy/__init__.py
+-rw-r--r--   0        0        0     6324 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/sympy/color.py
+-rw-r--r--   0        0        0     3383 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/sympy/lorentz.py
+-rw-r--r--   0        0        0      601 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/util.py
+-rw-r--r--   0        0        0     6581 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/vertex.py
+-rw-r--r--   0        0        0     2175 2024-04-04 09:31:27.117037 feynamp-0.0.5.12/pyproject.toml
+-rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 feynamp-0.0.5.12/setup.py
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 feynamp-0.0.5.12/PKG-INFO
```

### Comparing `feynamp-0.0.5/LICENSE` & `feynamp-0.0.5.12/LICENSE`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5/feynamp/__init__.py` & `feynamp-0.0.5.12/feynamp/__init__.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5/feynamp/amplitude.py` & `feynamp-0.0.5.12/feynamp/amplitude.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from feynamp.log import debug
 from feynamp.propagator import get_propagator_math_string
 from feynamp.vertex import get_vertex_math_string
 
 
 def feynman_diagram_to_string(feynman_diagram, feyn_model):
     fd = feynman_diagram
+    # TODO use these informations from qgraf, might need to be implemented in feynml
+    # sign = fd.get_sign()
+    # symmetry = fd.get_symmetry_factor()
     vm = []
     lm = []
     pm = []
     for v in fd.vertices:
         vm.append("(" + get_vertex_math_string(fd, v, feyn_model) + ")")
     for l in fd.legs:
         lm.append("(" + get_leg_math_string(fd, l, feyn_model) + ")")
@@ -51,18 +54,20 @@
     """
     dims = lst_fd[0].get_externals_size()
     for fd in lst_fd:
         assert (
             dims == fd.get_externals_size()
         ), "All FeynmanDiagrams must have the same external legs"
     # TODO handle relative fermion sign (also majorana!) https://cds.cern.ch/record/238903/files/th-6549-92.pdf
+    # TODO also multiply by the symmetry factor from qgraf
     # return multiply(lst_fd,[l.conjugated() for l in lst_fd],feyn_model)
     s = ""
     lst_fd1 = [feynman_diagram_to_string(l, feyn_model) for l in lst_fd]
     lst_fd2 = [feynman_diagram_to_string(l.conjugated(), feyn_model) for l in lst_fd]
+    debug(f"{lst_fd1=}")
     # TODO this could also be done in multiply by comparing the diagrams
     for i in range(len(lst_fd1)):
         for j in range(i, len(lst_fd2)):
             sfd1 = lst_fd1[i]
             sfd2 = lst_fd2[j]
             if i == j:
                 ttag = ""
```

### Comparing `feynamp-0.0.5/feynamp/form/__init__.py` & `feynamp-0.0.5.12/feynamp/form/form.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 import os
 import re
-from typing import List
 
 import form
-import sympy
-from feynml.feynmandiagram import FeynmanDiagram
-from feynmodel.feyn_model import FeynModel
-
-import feynamp
-from feynamp.log import debug
 
 count = 0
 dummy = 0
 init = """
 Symbols Pi,G,ZERO,Tr,Nc,Cf,CA,MC,ee;
 AutoDeclare Index Mu,Spin,Pol,Col,Glu,Propagator;
 AutoDeclare Symbol Mass,fd,mss,mst,msu;
 AutoDeclare Vector Mom;
 Tensors f(antisymmetric),Metric(symmetric),df(symmetric),da(symmetric),Identity(symmetric);
 Function ProjM,ProjP,VF,xg,xgi,P,dg,dgi,xeg,xegi;
-CFunctions Den,T,Denom,P,Gamma,u,v,ubar,vbar,eps,epsstar,VC,VA,GammaId;
+CFunctions Den,T,Denom,P,Gamma,u,v,ubar,vbar,eps,epsstar,VC,VA,GammaId, GammaCollect, GammaIdCollect;
 Indices a,o,n,m,tm,tn,beta,b,m,betap,alphap,a,alpha,ind,delta,k,j,l,c,d,e;
 """
 
 
 def get_dummy_index():
     global dummy
     dummy = dummy + 1
@@ -44,19 +37,19 @@
 
 
 def run(s, show=False, keep_form_file=True):
     global count
     count = count + 1
     with open("form" + str(count) + ".frm", "w") as frm:
         with form.open(keep_log=1000) as f:
-            l = s.split("Local")[1].split("=")[0].strip()
-            txt = s + "print " + l + ";.sort;"
+            local = s.split("Local")[1].split("=")[0].strip()
+            txt = s + "print " + local + ";.sort;"
             f.write(txt)
             frm.write(txt)
-            r = f.read("" + l)
+            r = f.read("" + local)
             r = re.sub(r"\+factor_\^?[0-9]*", r"", r).strip("*")
             if show:
                 print(r + "\n")
             # delete frm file
             if not keep_form_file:
                 os.remove("form" + str(count) + ".frm")
             return r
@@ -73,51 +66,7 @@
             .replace("^", "**")
             .replace("mss", "s")
             .replace("msu", "u")
             .replace("mst", "t")
         )
     )
     return simplify(ret.subs("Nc", "3").subs("Cf", "4/3"))
-
-
-# TODO compute squared  functino which coutns legs!!"!!!" and picks right mandelstamm,s
-
-
-def compute_squared(fds: List[FeynmanDiagram], fm: FeynModel):
-    dims = fds[0].get_externals_size()
-    for fd in fds:
-        assert (
-            dims == fd.get_externals_size()
-        ), "All FeynmanDiagrams must have the same external legs"
-    s2 = feynamp.amplitude.square(fds, fm, tag=False)
-    debug(f"{s2=}")
-    fs = ""
-    fs += feynamp.form.lorentz.get_gammas()
-    fs += feynamp.form.color.get_color()
-    fs += feynamp.form.momentum.get_kinematics()
-    fs += feynamp.form.momentum.get_onshell(fds, fm)
-    fs += feynamp.form.momentum.get_mandelstamm(fds, fm)
-
-    rs = feynamp.form.momentum.apply(s2, fs)
-    debug(f"{rs=}")
-
-    rr = feynamp.form.momentum.apply_den(
-        rs,
-        feynamp.form.momentum.get_onshell(fds, fm)
-        + feynamp.form.momentum.get_mandelstamm(fds, fm),
-    )
-    debug(f"{rr=}")
-
-    ret = sympy.simplify(
-        sympy.parse_expr(
-            rr.replace("Mom_", "")
-            .replace(".", "_")
-            .replace("^", "**")
-            .replace("mss", "s")
-            .replace("msu", "u")
-            .replace("mst", "t")
-        ).subs({"Nc": "3", "Cf": "4/3"})
-        * sympy.parse_expr(
-            "*".join([*feynamp.get_color_average(fds), *feynamp.get_spin_average(fds)])
-        )
-    )
-    return ret
```

### Comparing `feynamp-0.0.5/feynamp/form/color.py` & `feynamp-0.0.5.12/feynamp/form/color.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from feynamp.form import *
+from feynamp.form.form import init, run, string_to_form
 
 color = """
 **********************************************************
 *                  COLOUR STRUCTURE SIMPLIFY             *
 **********************************************************
     
 repeat;
 * remove df(k,j)
    id df(k?,l?)*df(l?,j?)=df(k,j);
-   id T(a?,k?,l?)*df(k?,j?)=T(a,j,l);id T(a?,k?,l?)*df(l?,j?)=T(a,k,j);
+   id T(a?,k?,l?)*df(k?,j?)=T(a,j,l);
+   id T(a?,k?,l?)*df(l?,j?)=T(a,k,j);
 * remove da(a,b)
    id da(a?,b?)*da(b?,c?)=da(a,c);
    id T(a?,k?,l?)*da(a?,b?)=T(b,k,l);
    id f(a?,b?,c?)*da(a?,d?)=f(d,b,c);
 * length-three objects simplify:
-   id T(b?,k?,j?)*T(a?,j?,c?)*T(b?,c?,l?)=(Cf-Nc*Tr)*T(a,k,l);
-   id T(b?,j?,l?)*T(c?,l?,k?)*f(a?,b?,c?)=i_*Nc*Tr*T(a,j,k);
+   id T(b?,k?,j?)*T(a?,j?,c?)*T(b?,c?,l?)=(-Tr/Nc*T(a,k,l));
+   id T(b?,j?,l?)*T(c?,l?,k?)*f(a?,b?,c?)=(i_*Nc*Tr*T(a,j,k));
 * length-two objects that give out df(k,j)
-   id T(a?,c?,j?)*T(a?,k?,l?)=-1/Nc*df(c, k)*df(j, l)/2 + df(c, l)*df(j, k)/2;
-   id T(a?,k?,l?)*T(a?,l?,j?)=Cf*df(k,j);
+   id T(a?,c?,j?)*T(a?,k?,l?)=(-1/Nc*df(c, j)*df(k, l)*Tr + df(c, l)*df(j, k)*Tr);
+   id T(a?,k?,l?)*T(a?,l?,j?)=(Cf*df(k,j));
 * length-two objects that give out da(a,b)
-   id T(a?,k?,l?)*T(b?,l?,k?)=Tr*da(a,b);
+   id T(a?,k?,l?)*T(b?,l?,k?)=(Tr*da(a,b));
    id f(a?,b?,c?)*f(d?,b?,c?)=Nc*da(a,d); 
 * simplify traces
    id T(b?,k?,k?)=0;
    id da(a?,a?)=Nc*Cf/Tr;
    id df(a?,a?)=Nc;
 * simplify combination of factors
-   id Nc^-2=2-Nc^2+Cf^2*Tr^-2;
-   id Nc^2=1+Nc*Cf/Tr;
+*   id Nc^-2=2-Nc^2+Cf^2*Tr^-2;
+*   id Nc^2=1+Nc*Cf/Tr;
    id Tr=1/2;
    id Tr^-1=2;
 * double f(a,b,c) simplify
 *  id f(a?,b?,e?)*f(c?,d?,e?)=-2 * { [T(a), T(b)] [T(c), T(d)]};
-   id f(a?,b?,e?)*f(c?,d?,e?)=-2 * (T(a,e,N1_?)*T(b,N1_?,N2_?) - T(b,e,N1_?)*T(a,N1_?,N2_?))*(T(c,N2_?,N3_?)*T(d,N3_?,e)-T(d,N2_?,N3_?)*T(c,N3_?,e));
+*   id f(a?,b?,e?)*f(c?,d?,e?)=-2 * (T(a,e,N1_?)*T(b,N1_?,N2_?) - T(b,e,N1_?)*T(a,N1_?,N2_?))*(T(c,N2_?,N3_?)*T(d,N3_?,e)-T(d,N2_?,N3_?)*T(c,N3_?,e));
 endrepeat;
 """
 
 color_sum = """
 **********************************************************
 *                  COLOUR SUM SIMPLIFY                   *
 **********************************************************
```

### Comparing `feynamp-0.0.5/feynamp/form/momentum.py` & `feynamp-0.0.5.12/feynamp/form/momentum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import List
 
 from feynml.feynmandiagram import FeynmanDiagram
 from feynmodel.feyn_model import FeynModel
 
 # from feynamp.form import *
-from feynamp.form import init, run, string_to_form
+from feynamp.form.form import init, run, string_to_form
 from feynamp.leg import find_leg_in_model
 from feynamp.log import warning
 from feynamp.momentum import insert_mass, insert_momentum
 
 momenta = """
 repeat;
     id P(Mu1?,Moma?)*P(Mu1?,Momb?) = Moma.Momb;
@@ -70,14 +70,15 @@
 def get_onshell(fds: List[FeynmanDiagram], model: FeynModel):
     if isinstance(fds, FeynmanDiagram):
         warning(
             "get_onshell is deprecated, use get_onshell with list of FeynmanDiagram"
         )
         fds = [fds]
     r = ""
+    # TODO might be redundant
     for fd in fds:
         for l in fd.legs:
             p = find_leg_in_model(fd, l, model)
             mom = insert_momentum(l.momentum.name)
             mass = insert_mass(string_to_form(p.mass.name))
             r += f"id {mom}.{mom} = {mass}^2;\n"
     return r
```

### Comparing `feynamp-0.0.5/feynamp/leg.py` & `feynamp-0.0.5.12/feynamp/leg.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5/feynamp/momentum.py` & `feynamp-0.0.5.12/feynamp/momentum.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5/feynamp/propagator.py` & `feynamp-0.0.5.12/feynamp/propagator.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5/feynamp/sympy/__init__.py` & `feynamp-0.0.5.12/feynamp/sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5/feynamp/sympy/color.py` & `feynamp-0.0.5.12/feynamp/sympy/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     expr = apply_T(expr)
     expr = apply_id(expr)
     return expr
 
 
 def apply_color_sum(expr):
     wi, wj, wk, ww = symbols("wi wj wk ww", cls=Wild)
-    expr = expr.replace(VC(wi, wk) * VC(wj, wk) * ww, delta_c(wi, wj))
-    expr = expr.replace(VA(wi, wk) * VA(wj, wk) * ww, delta_g(wi, wj))
+    expr = expr.replace(VC(wi, wk) * VC(wj, wk) * ww, ww * delta_c(wi, wj))
+    expr = expr.replace(VA(wi, wk) * VA(wj, wk) * ww, ww * delta_g(wi, wj))
     return expr
 
 
 def apply_delta(expr):
     expr = apply_delta_delta(expr)
     expr = apply_T_delta(expr)
     expr = apply_f_delta(expr)
```

### Comparing `feynamp-0.0.5/feynamp/sympy/lorentz.py` & `feynamp-0.0.5.12/feynamp/sympy/lorentz.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5/feynamp/vertex.py` & `feynamp-0.0.5.12/feynamp/vertex.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,58 +2,63 @@
 from typing import List
 
 import numpy as np
 from feynml.connector import Connector
 from feynml.id import generate_new_id
 from feynml.leg import Leg
 from feynml.propagator import Propagator
+from feynml.vertex import Vertex
 
 from feynamp.momentum import insert_momentum
 from feynamp.util import safe_index_replace
 
 
 def insert_color_types(s: str):
     """ """
     # We use the non greedy .*? to match multiple occurances individually
     s = re.sub(r"T\((.*?),(.*?),(.*?)\)", r"T(Glu\1,Col\2,Col\3)", s)
     s = re.sub(r"f\((.*?),(.*?),(.*?)\)", r"f(Glu\1,Glu\2,Glu\3)", s)
     s = re.sub(r"Identity\((.*?),(.*?)\)", r"Identity(Col\1,Col\2)", s)
     return s
 
 
-def insert_lorentz_types(s: str, connections: List[Connector]):
+def insert_lorentz_types(s: str, connections: List[Connector], vertex: Vertex):
     # We use the non greedy .*? to match multiple occurances individually
     s = re.sub(r"Gamma\((.*?),(.*?),(.*?)\)", r"Gamma(Mu\1,Spin\2,Spin\3)", s)
     s = re.sub(r"ProjP\((.*?),(.*?)\)", r"ProjP(Spin\1,Spin\2)", s)
     s = re.sub(r"ProjM\((.*?),(.*?)\)", r"ProjM(Spin\1,Spin\2)", s)
     s = re.sub(r"Metric\((.*?),(.*?)\)", r"Metric(Mu\1,Mu\2)", s)
     # use insert_momentum to replace the second argument to P
     matches = re.findall(r"P\((.*?),(.*?)\)", s)
     for g in matches:
         # find connection with g[1] id in connections
-        thec = None
+        repl = None
         for c in connections:
             if c.id == g[1] or "In" + str(c.id) == g[1] or "Out" + str(c.id) == g[1]:
-                thec = c
-                break
-        if thec is None:
+                # TODO: is this correct?
+                if c.goes_into(vertex):
+                    repl = "P(Mu" + g[0] + "," + insert_momentum(c.momentum.name) + ")"
+                    break
+                else:
+                    repl = (
+                        "(-P(Mu" + g[0] + "," + insert_momentum(c.momentum.name) + "))"
+                    )
+                    break
+        if repl is None:
             raise Exception(
                 f"Connection with id {g[1]} not found in connections {connections}"
             )
-        s = s.replace(
-            "P(" + g[0] + "," + g[1] + ")",
-            "P(Mu" + g[0] + "," + insert_momentum(c.momentum.name) + ")",
-        )
+        s = s.replace("P(" + g[0] + "," + g[1] + ")", repl)
     return s
 
 
-def insert_index_types(s):
-    s = insert_color_types(s)
-    s = insert_lorentz_types(s)
-    return s
+# def insert_index_types(s):
+#    s = insert_color_types(s)
+#    s = insert_lorentz_types(s)
+#    return s
 
 
 def get_vertex_math_string(fd, vertex, model):
     vv = get_vertex_math(fd, vertex, model)
     s = ""
     for v in vv:
         s += f"({v[0]})*({v[1]})*({v[2]}) + "
@@ -114,15 +119,15 @@
                     + str(v.connections[i].id),
                 )
             else:
                 raise Exception(
                     f"Connection {v.connections[i]} not a leg or propagator"
                 )
         if typed:
-            lor = insert_lorentz_types(lor, v.connections)
+            lor = insert_lorentz_types(lor, v.connections, vertex)
         lret.append(lor)
     ret = []
     for k, v in v.couplings.items():
         ret.append((v.value, cret[k[0]], lret[k[1]]))
     return ret
```

### Comparing `feynamp-0.0.5/pyproject.toml` & `feynamp-0.0.5.12/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynamp"
-version = "0.0.5"
+version = "0.0.5.12"
 description = "Compute Feynman diagrams"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynamp"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,15 +17,15 @@
 feynmodel = ">=0.0.5"
 #feynmodel = {path= "../feynmodel", develop = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-equation-database = ">=2024.3.30"
+equation-database = ">=2024.4.4"
 #equation-database = {path="../equation-database", develop = true}
 pytest = "*"
 pytest-cov =  "*"
 pytest-profiling =  "*"
 pytest-line-profiler-apn = ">=0.1.3"
 
 [tool.poetry.group.dev]
@@ -60,10 +60,11 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 addopts = [ "-v", "--cov=feynamp", "--cov-config=.coveragerc","--cov-append", "--cov-report=term", "--cov-report=xml", "--doctest-modules", "--ignore=docs/source/conf.py", "--ignore=debug"]
 filterwarnings = [
     'error',
     'ignore: pkg_resources is deprecated as an API:DeprecationWarning',
-    'ignore: Deprecated call to:DeprecationWarning'
+    'ignore: Deprecated call to:DeprecationWarning',
+    "ignore: 'cgi' is deprecated:DeprecationWarning",
 ]
```

