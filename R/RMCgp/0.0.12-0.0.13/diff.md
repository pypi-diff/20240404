# Comparing `tmp/RMCgp-0.0.12.tar.gz` & `tmp/RMCgp-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RMCgp-0.0.12.tar", last modified: Fri Mar 29 07:09:20 2024, max compression
+gzip compressed data, was "RMCgp-0.0.13.tar", last modified: Thu Apr  4 01:49:24 2024, max compression
```

## Comparing `RMCgp-0.0.12.tar` & `RMCgp-0.0.13.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.707751 RMCgp-0.0.12/
--rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.12/LICENSE.txt
--rw-r--r--   0 taung      (501) staff       (20)      495 2024-03-29 07:09:20.707593 RMCgp-0.0.12/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.12/README.md
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.703714 RMCgp-0.0.12/RMC/
--rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.704149 RMCgp-0.0.12/RMC/costfunctions/
--rw-r--r--   0 taung      (501) staff       (20)       74 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/costfunctions/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      904 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/costfunctions/finalCosts.py
--rw-r--r--   0 taung      (501) staff       (20)      686 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/costfunctions/runningCosts.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.704426 RMCgp-0.0.12/RMC/design/
--rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/design/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      944 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/design/generate_design.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.704698 RMCgp-0.0.12/RMC/emulator/
--rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/emulator/GP.py
--rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/emulator/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.705116 RMCgp-0.0.12/RMC/model/
--rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/model/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     1654 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/model/hybridcontrol.py
--rw-r--r--   0 taung      (501) staff       (20)     8268 2024-03-29 03:58:20.000000 RMCgp-0.0.12/RMC/model/hybridrunner.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.705459 RMCgp-0.0.12/RMC/optimization/
--rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/optimization/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     2111 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/optimization/onestepOptimization.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.706024 RMCgp-0.0.12/RMC/simulate/
--rw-r--r--   0 taung      (501) staff       (20)      652 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/simulate/CIR.py
--rw-r--r--   0 taung      (501) staff       (20)      635 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/simulate/OU.py
--rw-r--r--   0 taung      (501) staff       (20)       62 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/simulate/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     3407 2024-03-29 03:57:09.000000 RMCgp-0.0.12/RMC/simulate/sim.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-03-29 07:09:20.707311 RMCgp-0.0.12/RMCgp.egg-info/
--rw-r--r--   0 taung      (501) staff       (20)      495 2024-03-29 07:09:20.000000 RMCgp-0.0.12/RMCgp.egg-info/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)      639 2024-03-29 07:09:20.000000 RMCgp-0.0.12/RMCgp.egg-info/SOURCES.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-03-29 07:09:20.000000 RMCgp-0.0.12/RMCgp.egg-info/dependency_links.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-03-29 07:09:20.000000 RMCgp-0.0.12/RMCgp.egg-info/not-zip-safe
--rw-r--r--   0 taung      (501) staff       (20)      137 2024-03-29 07:09:20.000000 RMCgp-0.0.12/RMCgp.egg-info/requires.txt
--rw-r--r--   0 taung      (501) staff       (20)        4 2024-03-29 07:09:20.000000 RMCgp-0.0.12/RMCgp.egg-info/top_level.txt
--rw-r--r--   0 taung      (501) staff       (20)       38 2024-03-29 07:09:20.707809 RMCgp-0.0.12/setup.cfg
--rw-r--r--   0 taung      (501) staff       (20)     1474 2024-03-29 07:08:50.000000 RMCgp-0.0.12/setup.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.796918 RMCgp-0.0.13/
+-rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.13/LICENSE.txt
+-rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-04 01:49:24.796659 RMCgp-0.0.13/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.13/README.md
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.792339 RMCgp-0.0.13/RMC/
+-rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.792795 RMCgp-0.0.13/RMC/costfunctions/
+-rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-01 23:53:14.000000 RMCgp-0.0.13/RMC/costfunctions/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      908 2024-04-02 05:45:17.000000 RMCgp-0.0.13/RMC/costfunctions/finalCosts.py
+-rw-r--r--   0 taung      (501) staff       (20)     2234 2024-04-02 00:02:53.000000 RMCgp-0.0.13/RMC/costfunctions/runningCosts.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.793079 RMCgp-0.0.13/RMC/design/
+-rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/design/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      943 2024-04-03 23:22:58.000000 RMCgp-0.0.13/RMC/design/generate_design.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.793355 RMCgp-0.0.13/RMC/emulator/
+-rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/emulator/GP.py
+-rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/emulator/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.793935 RMCgp-0.0.13/RMC/model/
+-rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/model/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     1834 2024-04-02 00:55:41.000000 RMCgp-0.0.13/RMC/model/hybridcontrol.py
+-rw-r--r--   0 taung      (501) staff       (20)    10355 2024-04-04 01:22:21.000000 RMCgp-0.0.13/RMC/model/hybridrunner.py
+-rw-r--r--   0 taung      (501) staff       (20)      376 2024-04-02 00:24:04.000000 RMCgp-0.0.13/RMC/model/test_inputs.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.794412 RMCgp-0.0.13/RMC/optimization/
+-rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/optimization/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     1973 2024-04-04 00:16:01.000000 RMCgp-0.0.13/RMC/optimization/onestepOptimization.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.795146 RMCgp-0.0.13/RMC/simulate/
+-rw-r--r--   0 taung      (501) staff       (20)      652 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/simulate/CIR.py
+-rw-r--r--   0 taung      (501) staff       (20)      635 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/simulate/OU.py
+-rw-r--r--   0 taung      (501) staff       (20)       62 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/simulate/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     3417 2024-04-03 21:15:18.000000 RMCgp-0.0.13/RMC/simulate/sim.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.796061 RMCgp-0.0.13/RMCgp.egg-info/
+-rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)      664 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/SOURCES.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/dependency_links.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/not-zip-safe
+-rw-r--r--   0 taung      (501) staff       (20)      137 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/requires.txt
+-rw-r--r--   0 taung      (501) staff       (20)        4 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/top_level.txt
+-rw-r--r--   0 taung      (501) staff       (20)       38 2024-04-04 01:49:24.796972 RMCgp-0.0.13/setup.cfg
+-rw-r--r--   0 taung      (501) staff       (20)     1474 2024-04-04 01:49:19.000000 RMCgp-0.0.13/setup.py
```

### Comparing `RMCgp-0.0.12/LICENSE.txt` & `RMCgp-0.0.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.12/README.md` & `RMCgp-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.12/RMC/costfunctions/finalCosts.py` & `RMCgp-0.0.13/RMC/costfunctions/finalCosts.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     def charging_eff(self):
         return self._charging_eff
     @charging_eff.setter
     def charging_eff(self,efficiency):
         self._charging_eff = efficiency
 
     def cost(self,I):
-        return self.scale*np.maximum(self.Imax*self.constraint_level- I,0)
+        return self.scale*np.maximum(self._Imax*self.constraint_level- I,0)
     
     def derivative(self,I,B):
         # assume I follows I_prev + eta B( B>0) dt + 1/eta B(B<0 ) dt
-        dg_dB = -self.scale * (I< self.Imax*self.constraint_level ) * \
-            (self.charging_eff * (B>0) + 1/self.charging_eff * (B<0))
+        dg_dB = -self.scale * (I< self._Imax*self.constraint_level ) * \
+            (self._charging_eff * (B>0) + 1/self._charging_eff * (B<0))
         return dg_dB
```

### Comparing `RMCgp-0.0.12/RMC/design/generate_design.py` & `RMCgp-0.0.13/RMC/design/generate_design.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         W = sampler.random(n = self.N_samples)
         l_bounds = [self.X_lower,self.I_lower]
         u_bounds = [self.X_upper,self.I_upper]
         W= qmc.scale(W, l_bounds, u_bounds)
         X_designs = W[:,0]
         I_designs = W[:,1]
         return X_designs,I_designs
-    
+
```

### Comparing `RMCgp-0.0.12/RMC/emulator/GP.py` & `RMCgp-0.0.13/RMC/emulator/GP.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.12/RMC/model/hybridrunner.py` & `RMCgp-0.0.13/RMC/model/hybridrunner.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import GPy
 import numpy as np
 import warnings
 
 # Ignore all warnings
 warnings.filterwarnings("ignore")
 class runRMC():
-    def __init__(self,nsim,underlying_process,running_cost,final_cost,BESSparameters,batch_size,value_kernel,normalize_value,policy_kernel,normalize_policy):
+    def __init__(self,nsim,underlying_process,running_cost,final_cost,BESSparameters,batch_size,value_kernel,normalize_value,policy_kernel,normalize_policy,*args):
         self.nsim = nsim
         self.process = underlying_process
         self.nstep = self.process.nstep
         self.dt = self.process.dt
         self.t  = self.process.t
         self.batch_size = batch_size
         self.running_cost = running_cost
@@ -23,145 +23,179 @@
         self.Bmin = -self.Bmax
         self.Iub = (1-self.SOC_percen_lim)* self.Imax
         self.Ilb = self.SOC_percen_lim * self.Imax
         
         self.final_cost   = final_cost
         self.final_cost.Imax = self.Imax
         self.final_cost.charging_eff = self.charging_eff
-
-        self.value_kernel = value_kernel
-        self.policy_kernel= policy_kernel
-
+        
+        self.kernel_dic = {"RBF": GPy.kern.RBF, "Matern52":GPy.kern.Matern52 , "Matern32":GPy.kern.Matern32, None:None}
+        self.value_kernel = self.kernel_dic[value_kernel]
+        self.policy_kernel= self.kernel_dic[policy_kernel]
         self.value_normalizer = normalize_value
-        self.policy_kernel = policy_kernel
         self.policy_normalizer = normalize_policy
 
 
         self.values = [None]*self.nstep
-        self.policies = [None]*self.process.nstep
+        self.policies = [None]*self.nstep
         self.optimizer = onestepOptimizer(self.running_cost,self.charging_eff,self.dt)
         # final cost parameters are fixed
         # design parameters keep chanding -> dynamic
         # onestep optimizer initialization fixed, but reset q at each step, then set b,x,i, target
         
         self.targets = self.process.drift_p2
+        self.lower_targets = [None]* self.nstep
+        self.upper_targets = [None]*self.nstep
+        if len(args)==2:
+            self.lower_targets,self.upper_targets = args
         assert len(self.targets) == self.nstep, "Target length must be nstep total."
-        
-    def train_policy(self,X_train,I_train,target,opt_start):
+        assert len(self.lower_targets) == self.nstep, "Lower length must be nstep total."
+        assert len(self.upper_targets) == self.nstep, "Target length must be nstep total."
+
+
+        self.X_lowers,self.X_uppers = np.quantile(self.process.sim_trajectories, q =[0.005,0.995],axis = 0)
+    def train_policy(self,X_train,I_train,value_map,*args):
         assert len(X_train)==len(I_train)
         B_train = np.zeros(len(X_train))
 
         for i in range(len(B_train)):
-            B_train[i] = self.optimizer.optimize(X_train[i],I_train[i],target)
+            B_train[i] = self.optimizer.optimize(X_train[i],I_train[i],value_map,*args)
         control_input = np.column_stack((X_train,I_train))
         control_output= B_train.reshape(-1,1)
         if self.policy_kernel is None:
             kern = None
         else:
             kern = self.policy_kernel(control_input.shape[1],ARD = True)
-        kern  = GPy.kern.Matern32(input_dim=2,ARD= True)
-        control_map = policyGP(control_input,control_output,kernel =kern,normalizer= self.policy_normalizer)
+        
+
+        control_map = policyGP(control_input,control_output,kernel =kern,normalizer= True)
+        #control_map.optimize_restarts(num_restarts=2)
         control_map.optimize()
-        self.MSE_evaluation(B_train.flatten(),control_map.predict(control_input)[0].flatten(),"Policy")
+
+        MSE = self.MSE_evaluation(control_output.flatten(),control_map.predict(control_input)[0].flatten(),"Policy",I_train)
+        while MSE>=1e-1:
+            X_lb,X_ub = np.min(X_train),np.max(X_train)
+            X_new,I_new = design_generator(50,X_lb,X_ub,self.Ilb,self.Iub).create_samples
+            new_control_input = np.column_stack((X_new,I_new))
+            new_control_output = np.zeros(50)
+            for i in range(len(new_control_output)):
+                new_control_output[i] = self.optimizer.optimize(X_new[i],I_new[i],value_map,*args)
+            new_control_output = new_control_output.reshape(-1,1)
+            control_map.set_XY(np.vstack((control_map.X, new_control_input)), np.vstack((control_map.Y, new_control_output)))
+            control_map.optimize_restarts(num_restarts=2)
+            control_map.optimize()
+            MSE = self.MSE_evaluation(control_map.Y.flatten(),control_map.predict(control_map.X)[0].flatten(),\
+                                        "Policy",control_map.X[:,1])
+        #print(len(control_map.optimization_runs))
         return control_map
 
-    def train_value(self,X_train,I_train,pointwisevalues,opt_start):
+    def train_value(self,X_train,I_train,pointwisevalues):
         value_input = np.column_stack((X_train,I_train))
         value_output= pointwisevalues.reshape(-1,1)
         if self.value_kernel is None:
             kern = None
         else:
             kern = self.value_kernel(value_input.shape[1],ARD = True)
-        kern  = GPy.kern.Matern52(input_dim=2,ARD= True)
-        value_map = valueGP(value_input,value_output,kernel= kern,normalizer=self.value_normalizer)
+
+        value_map = valueGP(value_input,value_output,kernel= kern,normalizer=True)
         value_map.optimize()
-        self.MSE_evaluation(value_output,value_map.predict(value_input)[0].flatten(),"Value")
+        self.MSE_evaluation(value_output.flatten(),value_map.predict(value_input)[0].flatten(),"Value")
         return value_map
     
-    def v_evaluation(self,X_prev,drift_p1,drift_p2,vol_p1,vol_p2,I_next,target,policy_map,value_map):
+    def v_evaluation(self,X_prev,drift_p1,drift_p2,vol_p1,vol_p2,I_next,policy_map,value_map,*args):
+        target,lower_target,upper_target = args
         assert isinstance(target,(int,float)), "One step target is a scalar"
         reshape_dim = 1 # no reshaping
         X_prev_rep = X_prev
         I_next_rep = I_next
         if self.batch_size!=0:  
             reshape_dim = self.batch_size
             X_prev_rep= np.repeat(X_prev,self.batch_size)
             I_next_rep= np.repeat(I_next,self.batch_size)
 
         X_next_rep= self.process.onestepsimulate(int(self.nsim*reshape_dim),X_prev_rep,drift_p1,drift_p2,vol_p1,vol_p2)
-        power_outputs = policy_map.predict(np.column_stack((X_prev_rep,I_next_rep)))[0].flatten()
+        power_outputs = policy_map.predict(np.column_stack((X_next_rep,I_next_rep)))[0].flatten()
         LB = np.maximum(self.Bmin,self.charging_eff*(self.Ilb- I_next_rep)/self.dt)
         UB = np.minimum(self.Bmax,(self.Iub-I_next_rep)/(self.charging_eff*self.dt))
+
         pos_outputs = np.where(power_outputs>0)
-        power_outputs[pos_outputs] = np.minimum(power_outputs[pos_outputs],X_next_rep[pos_outputs])
+        # cannot charge more than X is available
+        upper_charging_bound  = np.maximum(X_next_rep[pos_outputs]-target,0)
+        power_outputs[pos_outputs] = np.minimum(power_outputs[pos_outputs],upper_charging_bound)
         power_outputs = np.maximum(LB,np.minimum(power_outputs,UB))
         I_nextnext = I_next_rep + power_outputs *(self.charging_eff *(power_outputs>0) + 1/self.charging_eff * (power_outputs<0))*self.dt
         if isinstance(value_map,final_SOCcontraint):
-            pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target) * self.dt + value_map.cost(I_nextnext)
+            pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target,lower_target,upper_target) * self.dt + value_map.cost(I_nextnext)
         if isinstance(value_map,GPy.core.GP):
             inp = np.column_stack((X_next_rep,I_nextnext))
-            pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target) * self.dt + value_map.predict(inp)[0].flatten()
+            pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target,lower_target,upper_target) * self.dt + value_map.predict(inp)[0].flatten()
         pointwise_v = np.mean(pointwise_v.reshape(-1,reshape_dim),axis = 1)
 
         return pointwise_v
     
     def solve(self):
-        self.X_lowers = self.process.mean_vec - 2.5 * self.process.std_vec
-        self.X_uppers = self.process.mean_vec - 2.5 * self.process.std_vec
+
 
         # need to be fixed
         #self.X_lowers[0] = self.process.mean_vec[0] - 2.5*self.process.std_vec[3]
         #self.X_uppers[0] = self.process.mean_vec[0] + 2.5*self.process.std_vec[3]
 
         self.values[-1] = self.final_cost 
         X_prev,I_next = design_generator(self.nsim,self.X_lowers[-3],self.X_uppers[-3],self.Ilb,self.Iub).create_samples
         X_next = self.process.onestepsimulate(self.nsim,X_prev,self.process.drift_p1[-2],self.process.drift_p2[-2],\
                                               self.process.diffusion_p1[-2],self.process.diffusion_p2[-2])
-        self.optimizer.q = self.values[-1]
-        self.policies[-1] = self.train_policy(X_next,I_next,self.targets[-1],None)
+        self.policies[-1] = self.train_policy(X_next,I_next,self.values[-1],self.targets[-1],self.lower_targets[-1],self.upper_targets[-1])
 
         
         pointwise_values = self.v_evaluation(X_prev,self.process.drift_p1[-2],self.process.drift_p2[-2],\
                                              self.process.diffusion_p1[-2],self.process.diffusion_p2[-2],\
-                                             I_next,self.targets[-1],self.policies[-1],self.values[-1])
+                                             I_next,self.policies[-1],self.values[-1],\
+                                                self.targets[-1],self.lower_targets[-1],self.upper_targets[-1])
         
         for iStep in range(self.nstep-1,0,-1):
-            self.values[iStep-1] = self.train_value(X_prev,I_next,pointwise_values,opt_start=None)
-            
+            self.values[iStep-1] = self.train_value(X_prev,I_next,pointwise_values)
+
             print("Timestep: "+ str(self.t[iStep]))
 
             print("_"*50)
 
             if iStep!=1:
                 X_prev,I_next = design_generator(self.nsim,self.X_lowers[iStep-2],self.X_uppers[iStep-2],self.Ilb,self.Iub).create_samples
                 X_next = self.process.onestepsimulate(self.nsim,X_prev,self.process.drift_p1[iStep-2],self.process.drift_p2[iStep-2],\
                                                 self.process.diffusion_p1[iStep-2],self.process.diffusion_p2[iStep-2])
-                self.optimizer.q = self.values[iStep-1]
-                self.policies[iStep-1] = self.train_policy(X_next,I_next,self.targets[iStep-1],None)
+
+                self.policies[iStep-1] = self.train_policy(X_next,I_next,self.values[iStep-1],self.targets[iStep-1],self.lower_targets[iStep-1],self.upper_targets[iStep-1])
 
         
                 pointwise_values = self.v_evaluation(X_prev,self.process.drift_p1[iStep-2],self.process.drift_p2[iStep-2],\
                                              self.process.diffusion_p1[iStep-2],self.process.diffusion_p2[iStep-2],\
-                                             I_next,self.targets[iStep-1],self.policies[iStep-1],self.values[iStep-1])
+                                             I_next,self.policies[iStep-1],self.values[iStep-1],\
+                                            self.targets[iStep-1],self.lower_targets[iStep-1],self.upper_targets[iStep-1])
         
             else:
-                X_next,I_next = design_generator(self.nsim,self.X_lowers[0],self.X_uppers[0],self.Ilb,self.Iub).create_samples
-                self.optimizer.q = self.values[iStep-1]
-                self.policies[iStep-1] = self.train_policy(X_next,I_next,self.targets[iStep-1],None)
+                X_0,I_0 = design_generator(self.nsim,self.X_lowers[0],self.X_uppers[0],self.Ilb,self.Iub).create_samples
+                #self.optimizer.q = self.values[iStep-1]
+                self.policies[iStep-1] = self.train_policy(X_0,I_0,self.values[iStep-1],self.targets[iStep-1],self.lower_targets[iStep-1],self.upper_targets[iStep-1])
+                print("Timestep: "+ str(self.t[iStep-1]))
+                print("_"*50)
 
     @property
     def policy_maps(self):
         return self.policies
     
     @property
     def value_maps(self):
-        return self.value_maps
+        return self.values
     
-    def MSE_evaluation(self,y_true,GP_output,map_type):
+    def MSE_evaluation(self,y_true,GP_output,map_type,*args):
         if map_type == "Policy":
-            p1 = np.maximum(self.Bmin,np.minimum(y_true,self.Bmax))
-            p2 = np.maximum(self.Bmin,np.minimum(GP_output,self.Bmax))
+            cur_I = args[0]
+            LB = np.maximum(self.Bmin,self.charging_eff*(self.Ilb- cur_I)/self.dt)
+            UB = np.minimum(self.Bmax,(self.Iub-cur_I)/(self.charging_eff*self.dt))
+            p1 = np.maximum(LB,np.minimum(y_true,UB))
+            p2 = np.maximum(LB,np.minimum(GP_output,UB))
             MSE = np.mean((p1-p2)**2)
         else:
-            MSE = np.mean((y_true - GP_output))
+            MSE = np.mean((y_true - GP_output)**2)
         print(f"{map_type} GP MSE: " + str(MSE))
+        return MSE
```

### Comparing `RMCgp-0.0.12/RMC/optimization/onestepOptimization.py` & `RMCgp-0.0.13/RMC/optimization/onestepOptimization.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,51 +6,41 @@
 class onestepOptimizer():
 
     def __init__(self,running_cost,charging_eff,dt):
         
         self.running_cost = running_cost
         self.charging_eff = charging_eff
         self.dt           = dt
-        self._q           = None
 
-    @property
-    def q(self):
-        return self._q
-
-    @q.setter
-    def q(self,mdl):
-        self._q = mdl
-
-    def cost_togo(self,B,X,I,target):
+    def cost_togo(self,B,X,I,q,*args):
         assert isinstance(B,(list,np.ndarray)), "B must be array of length 1."
         # starting here no B allowed only B[0]
         next_step = np.array([X,I +B[0]*(self.charging_eff*(B[0]>0) + 1/self.charging_eff * (B[0]<0))*self.dt])
-        if isinstance(self.q,final_SOCcontraint):
-            q_val = self.q.cost(next_step[1])
-        if isinstance(self.q,GPy.core.GP):
-            q_val = self.q.predict(next_step.reshape(1,-1))[0].flatten()[0]
-
-        cost = self.running_cost.cost(B[0],X,target) * self.dt + q_val
+        if isinstance(q,final_SOCcontraint):
+            q_val = q.cost(next_step[1])
+        if isinstance(q,GPy.core.GP):
+            q_val = q.predict(next_step.reshape(1,-1))[0].flatten()[0]
 
+        cost = self.running_cost.cost(B[0],X,*args) * self.dt + q_val
         return cost
 
-    def cost_togo_derivative(self,B,X,I,target):
+    def cost_togo_derivative(self,B,X,I,q,*args):
 
         assert isinstance(B,(list,np.ndarray)), "B must be array of length 1."
         # starting here no B allowed only B[0]
         next_step = np.array([X,I +B[0]*(self.charging_eff*(B[0]>0) + 1/self.charging_eff * (B[0]<0))*self.dt])
-        if isinstance(self.q,final_SOCcontraint):
-            q_derivative= self.q.derivative(next_step[1],B[0])
-        if isinstance(self.q,GPy.core.GP):
-            q_derivative = self.q.predictive_gradients(next_step.reshape(1,-1))[0][:,1].flatten()[0] 
+        if isinstance(q,final_SOCcontraint):
+            q_derivative= q.derivative(next_step[1],B[0])
+        if isinstance(q,GPy.core.GP):
+            q_derivative = q.predictive_gradients(next_step.reshape(1,-1))[0][:,1].flatten()[0] 
             q_derivative = q_derivative * (self.charging_eff * (B[0]>0) + 1/self.charging_eff * (B[0]<0))
 
-        cost_derivative = self.running_cost.derivative(B[0],X,target) * self.dt + q_derivative* self.dt
+        cost_derivative = self.running_cost.derivative(B[0],X,*args) * self.dt + q_derivative* self.dt
         return cost_derivative
-    
-    def optimize(self,X,I,target):
 
+    def optimize(self,X,I,q,*remainingargs):
+        target = remainingargs[0]
         starter = X- target
 
         opt_B = scipy.optimize.minimize(self.cost_togo, jac= self.cost_togo_derivative,x0=starter, \
-                                       args=(X,I,target),method = "L-BFGS-B",bounds=None)
+                                       args=(X,I,q,*remainingargs),method = "L-BFGS-B",bounds=None)
         return opt_B.x[0]
```

### Comparing `RMCgp-0.0.12/RMC/simulate/CIR.py` & `RMCgp-0.0.13/RMC/simulate/CIR.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.12/RMC/simulate/OU.py` & `RMCgp-0.0.13/RMC/simulate/OU.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.12/RMC/simulate/sim.py` & `RMCgp-0.0.13/RMC/simulate/sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def std_vec(self):
         return np.std(self.sim_trajectories,axis= 0, ddof = 1)
 
     def onestepsimulate(self,nsim,X_start,drift_p1,drift_p2,vol_p1,vol_p2):
         dW = np.random.normal(0,1,size = nsim) * np.sqrt(self.dt)
         X_next = np.abs(X_start +self.drift(drift_p1,drift_p2,X_start) * self.dt +\
                             self.diffusion(vol_p1,vol_p2,X_start)* dW)
-        return X_next
+        return X_next.flatten()
     def cor(self,i,j):
         if i <=0 or i >= self.nstep+1:
             raise ValueError("Invalid index for i.")
         if j <= 0 or j >= self.nstep+1:
             raise ValueError("Invalid index for j.")
         
         return np.corrcoef(self.sim_trajectories[:,i],self.sim_trajectories[:,j])[0,1]
```

### Comparing `RMCgp-0.0.12/RMCgp.egg-info/SOURCES.txt` & `RMCgp-0.0.13/RMCgp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 RMC/design/__init__.py
 RMC/design/generate_design.py
 RMC/emulator/GP.py
 RMC/emulator/__init__.py
 RMC/model/__init__.py
 RMC/model/hybridcontrol.py
 RMC/model/hybridrunner.py
+RMC/model/test_inputs.py
 RMC/optimization/__init__.py
 RMC/optimization/onestepOptimization.py
 RMC/simulate/CIR.py
 RMC/simulate/OU.py
 RMC/simulate/__init__.py
 RMC/simulate/sim.py
 RMCgp.egg-info/PKG-INFO
```

### Comparing `RMCgp-0.0.12/setup.py` & `RMCgp-0.0.13/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "GPy>=1.13.0",
     "scikit-learn>=1.3.0",
     "scipy>=1.1.4",
     "matplotlib>=3.8.0"
 ]
 
 setuptools.setup(name='RMCgp',
-                 version='0.0.12',
+                 version='0.0.13',
                  author='Thiha Aung',
                  author_email='taung@ucsb.edu',
                  maintainer='Thiha Aung',
                  maintainer_email='taung@ucsb.edu',
                  description='RMC for stochastic control.',
                  long_description=readme,
                  url='https://github.com/thihaa2019/RMCgp',
```

