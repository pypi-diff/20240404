# Comparing `tmp/osier-0.2.1.tar.gz` & `tmp/osier-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osier-0.2.1.tar", last modified: Tue Nov  1 15:44:55 2022, max compression
+gzip compressed data, was "osier-0.3.tar", last modified: Thu Apr  4 13:51:12 2024, max compression
```

## Comparing `osier-0.2.1.tar` & `osier-0.3.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-11-01 15:44:55.984548 osier-0.2.1/
--rw-rw-rw-   0        0        0     1570 2022-09-09 16:14:54.000000 osier-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2545 2022-11-01 15:44:55.983552 osier-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1567 2022-10-04 18:20:06.000000 osier-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-01 15:44:55.960612 osier-0.2.1/osier/
--rw-rw-rw-   0        0        0       79 2022-10-28 22:21:40.000000 osier-0.2.1/osier/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:44:55.981558 osier-0.2.1/osier/models/
--rw-rw-rw-   0        0        0        0 2022-10-04 18:20:06.000000 osier-0.2.1/osier/models/__init__.py
--rw-rw-rw-   0        0        0    22120 2022-11-01 01:23:12.000000 osier-0.2.1/osier/models/dispatch.py
--rw-rw-rw-   0        0        0    19420 2022-10-28 22:21:40.000000 osier-0.2.1/osier/technology.py
--rw-rw-rw-   0        0        0     1656 2022-10-28 22:21:40.000000 osier-0.2.1/osier/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:44:55.978605 osier-0.2.1/osier.egg-info/
--rw-rw-rw-   0        0        0     2545 2022-11-01 15:44:55.000000 osier-0.2.1/osier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2022-11-01 15:44:55.000000 osier-0.2.1/osier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-01 15:44:55.000000 osier-0.2.1/osier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2022-11-01 15:44:55.000000 osier-0.2.1/osier.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-01 15:44:55.000000 osier-0.2.1/osier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-01 15:44:55.984548 osier-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     3303 2022-11-01 15:19:43.000000 osier-0.2.1/setup.py
+drwxr-xr-x   0 samdotson   (501) staff       (20)        0 2024-04-04 13:51:12.165692 osier-0.3/
+-rw-r--r--   0 samdotson   (501) staff       (20)     1541 2023-06-16 18:47:23.000000 osier-0.3/LICENSE
+-rw-r--r--   0 samdotson   (501) staff       (20)     3584 2024-04-04 13:51:12.164857 osier-0.3/PKG-INFO
+-rw-r--r--   0 samdotson   (501) staff       (20)     1965 2024-04-04 13:45:01.000000 osier-0.3/README.md
+drwxr-xr-x   0 samdotson   (501) staff       (20)        0 2024-04-04 13:51:12.154434 osier-0.3/osier/
+-rw-r--r--   0 samdotson   (501) staff       (20)      433 2024-02-27 21:57:54.000000 osier-0.3/osier/__init__.py
+-rw-r--r--   0 samdotson   (501) staff       (20)     9760 2023-06-23 18:15:43.000000 osier-0.3/osier/equations.py
+drwxr-xr-x   0 samdotson   (501) staff       (20)        0 2024-04-04 13:51:12.158615 osier-0.3/osier/models/
+-rw-r--r--   0 samdotson   (501) staff       (20)        0 2023-06-16 18:47:23.000000 osier-0.3/osier/models/__init__.py
+-rw-r--r--   0 samdotson   (501) staff       (20)     8514 2024-04-04 13:45:01.000000 osier-0.3/osier/models/capacity_expansion.py
+-rw-r--r--   0 samdotson   (501) staff       (20)     9830 2023-06-23 18:15:43.000000 osier-0.3/osier/models/deap_runner.py
+-rw-r--r--   0 samdotson   (501) staff       (20)    24494 2024-02-29 17:11:31.000000 osier-0.3/osier/models/dispatch.py
+-rw-r--r--   0 samdotson   (501) staff       (20)     7750 2023-06-16 18:47:23.000000 osier-0.3/osier/tech_library.py
+-rw-r--r--   0 samdotson   (501) staff       (20)    26563 2024-01-27 23:04:19.000000 osier-0.3/osier/technology.py
+-rw-r--r--   0 samdotson   (501) staff       (20)     4304 2024-04-04 11:42:06.000000 osier-0.3/osier/utils.py
+drwxr-xr-x   0 samdotson   (501) staff       (20)        0 2024-04-04 13:51:12.163012 osier-0.3/osier.egg-info/
+-rw-r--r--   0 samdotson   (501) staff       (20)     3584 2024-04-04 13:51:12.000000 osier-0.3/osier.egg-info/PKG-INFO
+-rw-r--r--   0 samdotson   (501) staff       (20)      492 2024-04-04 13:51:12.000000 osier-0.3/osier.egg-info/SOURCES.txt
+-rw-r--r--   0 samdotson   (501) staff       (20)        1 2024-04-04 13:51:12.000000 osier-0.3/osier.egg-info/dependency_links.txt
+-rw-r--r--   0 samdotson   (501) staff       (20)      208 2024-04-04 13:51:12.000000 osier-0.3/osier.egg-info/requires.txt
+-rw-r--r--   0 samdotson   (501) staff       (20)        6 2024-04-04 13:51:12.000000 osier-0.3/osier.egg-info/top_level.txt
+-rw-r--r--   0 samdotson   (501) staff       (20)       38 2024-04-04 13:51:12.165881 osier-0.3/setup.cfg
+-rw-r--r--   0 samdotson   (501) staff       (20)     3290 2024-04-04 13:45:45.000000 osier-0.3/setup.py
+drwxr-xr-x   0 samdotson   (501) staff       (20)        0 2024-04-04 13:51:12.162080 osier-0.3/tests/
+-rw-r--r--   0 samdotson   (501) staff       (20)     1368 2023-06-23 18:15:43.000000 osier-0.3/tests/test_deaprunner.py
+-rw-r--r--   0 samdotson   (501) staff       (20)     5184 2024-02-27 14:33:24.000000 osier-0.3/tests/test_equations.py
+-rw-r--r--   0 samdotson   (501) staff       (20)    11170 2023-06-16 18:47:23.000000 osier-0.3/tests/test_models.py
+-rw-r--r--   0 samdotson   (501) staff       (20)    14372 2023-06-16 18:47:23.000000 osier-0.3/tests/test_technology.py
+-rw-r--r--   0 samdotson   (501) staff       (20)     1489 2024-04-04 11:42:06.000000 osier-0.3/tests/test_utils.py
```

### Comparing `osier-0.2.1/LICENSE` & `osier-0.3/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, Advanced Reactors and Fuel Cycles
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, Advanced Reactors and Fuel Cycles
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `osier-0.2.1/osier/models/dispatch.py` & `osier-0.3/osier/models/dispatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,540 +1,613 @@
-import pandas as pd
-import numpy as np
-import pyomo.environ as pe
-import pyomo.opt as po
-from pyomo.environ import ConcreteModel
-from unyt import unyt_array, hr, MW
-import itertools as it
-from osier.technology import _validate_quantity, _validate_unit
-from osier.utils import synchronize_units
-import warnings
-
-_freq_opts = {'D': 'day',
-              'H': 'hour',
-              'S': 'second',
-              'T': 'minute'}
-LARGE_NUMBER = 1e40
-
-
-class DispatchModel():
-    """
-    The :class:`DispatchModel` class creates and solves a basic dispatch
-    model from the perspective of a "grid operator." The model uses
-    `pyomo <https://pyomo.readthedocs.io/en/stable/index.html>`_
-    to create and solve a linear programming model.
-    The mathematical formulation for this problem is:
-
-    Minimize
-
-
-    .. math::
-        \\text{C}_{\\text{total}} = \\sum_t^T \\sum_u^U
-        \\left[c^{\\text{fuel}}_{u,t} + c^{\\text{om,var}}_{u,t}\\right]x_{u,t}
-
-    Such that,
-
-    1. The generation meets demand within a user-specified tolerance
-    (undersupply and oversupply)
-
-    .. math::
-        \\sum_u^Ux_{u,t} &\\geq \\left(1-\\text{undersupply}\\right)\\text{D}_t
-        \\ \\forall \\ t \\in T
-
-        \\sum_u^Ux_{u,t} &\\leq \\left(1+\\text{oversupply}\\right)\\text{D}_t
-        \\ \\forall \\ t \\in T
-
-    2. A technology's generation (:math:`x_u`) does not exceed its capacity to
-    generate at any time, :math:`t`.
-
-    .. math::
-        x_{u,t} \\leq \\textbf{CAP}_{u}\\Delta t \\ \\forall \\ u,t \\in U,T
-
-    3. Technologies may not exceed their ramp up rate,
-
-    .. math::
-        \\frac{x_{r,t} - x_{r,t-1}}{\\Delta t} = \\Delta P_{r,t} \\leq
-        (\\text{ramp up})\\textbf{CAP}_u\\Delta t \\ \\forall \\ r,t
-        \\in R \\subset U, T
-
-    or ramp down rate,
-
-    .. math::
-        \\frac{x_{r,t} - x_{r,t-1}}{\\Delta t} = \\Delta P_{r,t} \\leq
-        -(\\text{ramp down})\\textbf{CAP}_u\\Delta t \\ \\forall \\ r,t
-        \\in R \\subset U, T .
-
-    Parameters
-    ----------
-    technology_list : list of :class:`osier.Technology`
-        The list of :class:`Technology` objects to dispatch -- i.e. decide
-        how much energy each technology should produce.
-    net_demand : list, :class:`numpy.ndarray`, :class:`unyt.array.unyt_array`, :class:`pandas.DataFrame`
-        The remaining energy demand to be fulfilled by the technologies in
-        :attr:`technology_list`. The `values` of an object passed as
-        `net_demand` are used to create a supply constraint. See
-        :attr:`oversupply` and :attr:`undersupply`.
-        If a :class:`pandas.DataFrame` is passed, :mod:`osier` will try
-        inferring a `time_delta` from the dataframe index. Otherwise, the
-        :attr:`time_delta` must be passed or the default is used.
-    time_delta : str, :class:`unyt.unyt_quantity`, float, int
-        Specifies the amount of time between two time slices. The default is
-        one hour. Can be overridden by specifying a unit with the value. For
-        example:
-
-        >>> time_delta = "5 minutes"
-        >>> from unyt import days
-        >>> time_delta = 30*days
-
-        would both work.
-    power_units : str, :class:`unyt.unit_object`
-        Specifies the units for the power demand. The default is :attr:`MW`.
-        Can be overridden by specifying a unit with the value.
-    solver : str
-        Indicates which solver to use. May require separate installation.
-        Accepts: ['cplex', 'cbc']. Other solvers will be added in the future.
-    lower_bound : float
-        The minimum amount of energy each technology can produce per time
-        period. Default is 0.0.
-    oversupply : float
-        The amount of allowed oversupply as a percentage of demand.
-        Default is 0.0 (no oversupply allowed).
-    undersupply : float
-        The amount of allowed undersupply as a percentage of demand.
-        Default is 0.0 (no undersupply allowed).
-
-    Attributes
-    ----------
-    model : :class:`pyomo.environ.ConcreteModel`
-        The :mod:`pyomo` model class that converts python code into a
-        set of linear equations.
-    objective : float
-        The result of the model's objective function. Only instantiated
-        after :meth:`DispatchModel.solve()` is called.
-    n_timesteps : int
-        The number of timesteps in the model.
-    upper_bound : float
-        The upper bound for all decision variables. Chosen to be equal
-        to the maximum capacity of all technologies in :attr:`tech_set`.
-    storage_upper_bound : float
-        The upper bound for storage decision variables.
-    penalty : float
-        The penalty applied to the objective function to eliminate
-        simultaneous charging and discharging. Users may need to tune
-        this parameter. Default is 1.0.
-
-    model_initialized : bool
-        Indicates whether :attr:`DispatchModel.model` has been populated
-        with equations yet. This is set to ``True`` after
-        :meth:`DispatchModel._write_model_equations()` has been called.
-    indices : list of tuples
-        The list of tuples representing the product of the
-        :attr:`tech_set` and :attr:`time_set` attributes.
-    tech_set : list of str
-        A list of the unique technology names in the simulation.
-    capacity_dict : dict
-        A dictionary of {name : capacity} pairs.
-    efficiency_dict : dict
-        A dictionary of {name : efficiency} pairs.
-    time_set : iterable
-        The result of ``range(self.n_timesteps)``.
-    cost_params : list
-        The set of cost parameters for each technology. Corresponds to
-        a list of values. Size is equal to the product of the number of
-        timesteps and the number of technologies in the model.
-    ramp_up_params : list
-        The set of ramp_up parameters. Only initialized if there is a
-        ramping technology.
-    ramp_down_params : list
-        The set of ramp_down parameters. Only initialized if there is a
-        ramping technology.
-    ramping_techs : list
-        The subset of :attr:`tech_set` containing ramping technologies.
-
-    Notes
-    -----
-    1. Technically, :attr:`solver` will accept any solver that :class:`pyomo`
-    can use. We only list two solvers because those are the only solvers
-    in the :mod:`osier` test suite.
-
-    2. The default value for :attr:`time_delta` in :attr:`__init__` is
-    `None`. This is replaced by a setter method in :class:`Dispatch`.
-
-    3. This formulation uses a :attr:`penalty` parameter  to prevent unphysical
-    behavior because it preserves the problem's linearity. Some formulations
-    may use a binary variable to prevent simultaneous charging and discharing.
-    However, this changes the problem to a mixed-integer linear program which
-    requires a more sophisticated solver such as ``gurobi``.
-
-    4. :meth:`_write_model_equations` may be called before :meth:`solve` if
-    users wish to add their own constraints or parameters to the problem.
-    """
-
-    def __init__(self,
-                 technology_list,
-                 net_demand,
-                 time_delta=None,
-                 power_units=MW,
-                 solver='cplex',
-                 lower_bound=0.0,
-                 oversupply=0.0,
-                 undersupply=0.0,
-                 penalty=1e-4):
-        self.net_demand = net_demand
-        self.time_delta = time_delta
-        self.power_units = power_units
-        self.lower_bound = lower_bound
-        self.oversupply = oversupply
-        self.undersupply = undersupply
-        self.penalty = penalty
-        self.model = ConcreteModel()
-        self.solver = solver
-        self.results = None
-        self.objective = None
-        self.model_initialized = False
-
-        self.technology_list = synchronize_units(
-            technology_list,
-            unit_power=power_units,
-            unit_time=self.time_delta.units)
-
-    @property
-    def time_delta(self):
-        return self._time_delta
-
-    @time_delta.setter
-    def time_delta(self, value):
-        if value:
-            valid_quantity = _validate_quantity(value, dimension='time')
-            self._time_delta = valid_quantity
-        else:
-            if isinstance(self.net_demand, pd.DataFrame):
-                try:
-                    freq_list = list(self.net_demand.index.inferred_freq)
-                    freq_key = freq_list[-1]
-                    try:
-                        value = float(freq_list[0])
-                    except ValueError:
-                        warnings.warn((f"Could not convert value "
-                                       f"{freq_list[0]} to float. "
-                                       "Setting to 1.0."),
-                                      UserWarning)
-                        value = 1.0
-                    self._time_delta = _validate_quantity(
-                        f"{value} {_freq_opts[freq_key]}", dimension='time')
-                except KeyError:
-                    warnings.warn(
-                        (f"Could not infer time delta with freq {freq_key} "
-                         "from pandas dataframe. Setting delta to 1 hour."),
-                        UserWarning)
-                    self._time_delta = 1 * hr
-            else:
-                self._time_delta = 1 * hr
-
-    @property
-    def power_units(self):
-        return self._power_units
-
-    @power_units.setter
-    def power_units(self, value):
-        if value:
-            valid_quantity = _validate_unit(value, dimension='power')
-            self._power_units = valid_quantity
-        else:
-            warnings.warn(f"Could not infer power units. Unit set to MW.")
-            self._power_units = MW
-
-    @property
-    def n_timesteps(self):
-        return len(self.net_demand)
-
-    @property
-    def tech_set(self):
-        tech_names = [t.technology_name for t in self.technology_list]
-        return tech_names
-
-    @property
-    def capacity_dict(self):
-        capacity_set = unyt_array([t.capacity for t in self.technology_list])
-        return dict(zip(self.tech_set, capacity_set))
-
-    @property
-    def efficiency_dict(self):
-        capacity_set = [t.efficiency for t in self.technology_list]
-        return dict(zip(self.tech_set, capacity_set))
-
-    @property
-    def time_set(self):
-        return range(self.n_timesteps)
-
-    @property
-    def indices(self):
-        return list(it.product(self.tech_set, self.time_set))
-
-    @property
-    def cost_params(self):
-        v_costs = np.array([
-            (t.variable_cost_ts(self.n_timesteps))
-            for t in self.technology_list
-        ]).flatten()
-        return dict(zip(self.indices, v_costs))
-
-    @property
-    def storage_techs(self):
-        return [t.technology_name
-                for t in self.technology_list
-                if hasattr(t, "storage_capacity")]
-
-    @property
-    def storage_upper_bound(self):
-        caps = unyt_array([t.storage_capacity
-                           for t in self.technology_list
-                           if hasattr(t, "storage_capacity")])
-        return caps.max().to_value()
-
-    @property
-    def max_storage_params(self):
-        storage_dict = {t.technology_name: t.storage_capacity.to_value()
-                        for t in self.technology_list
-                        if hasattr(t, "storage_capacity")}
-        return storage_dict
-
-    @property
-    def initial_storage_params(self):
-        storage_dict = {t.technology_name: t.initial_storage.to_value()
-                        for t in self.technology_list
-                        if hasattr(t, "initial_storage")}
-        return storage_dict
-
-    @property
-    def ramping_techs(self):
-        return [t.technology_name
-                for t in self.technology_list
-                if hasattr(t, 'ramp_up')]
-
-    @property
-    def ramp_up_params(self):
-        rates_dict = {
-            t.technology_name: (
-                t.ramp_up *
-                self.time_delta).to_value() for t in self.technology_list
-            if hasattr(t, 'ramp_up')}
-        return rates_dict
-
-    @property
-    def ramp_down_params(self):
-        rates_dict = {
-            t.technology_name: (
-                t.ramp_down *
-                self.time_delta).to_value() for t in self.technology_list
-            if hasattr(t, 'ramp_up')}
-        return rates_dict
-
-    @property
-    def upper_bound(self):
-        caps = unyt_array([t.capacity for t in self.technology_list])
-        return caps.max().to_value()
-
-    def _create_model_indices(self):
-        self.model.Generators = pe.Set(initialize=self.tech_set, ordered=True)
-        self.model.Time = pe.Set(initialize=self.time_set, ordered=True)
-        if len(self.ramping_techs) > 0:
-            self.model.RampingTechs = pe.Set(initialize=self.ramping_techs,
-                                             ordered=True,
-                                             within=self.model.Generators)
-        if len(self.storage_techs) > 0:
-            self.model.StorageTech = pe.Set(initialize=self.storage_techs,
-                                            ordered=True,
-                                            within=self.model.Generators)
-
-    def _create_demand_param(self):
-        self.model.Demand = pe.Param(self.model.Time, initialize=dict(
-            zip(self.model.Time, np.array(self.net_demand))))
-
-    def _create_cost_param(self):
-        self.model.VariableCost = pe.Param(
-            self.model.Generators,
-            self.model.Time,
-            initialize=self.cost_params)
-
-    def _create_ramping_params(self):
-        self.model.ramp_up = pe.Param(
-            self.model.RampingTechs, initialize=self.ramp_up_params)
-        self.model.ramp_down = pe.Param(
-            self.model.RampingTechs, initialize=self.ramp_down_params)
-
-    def _create_max_storage_params(self):
-        self.model.storage_capacity = pe.Param(
-            self.model.StorageTech, initialize=self.max_storage_params
-        )
-
-    def _create_init_storage_params(self):
-        self.model.initial_storage = pe.Param(
-            self.model.StorageTech, initialize=self.initial_storage_params
-        )
-
-    def _create_model_variables(self):
-        self.model.x = pe.Var(self.model.Generators, self.model.Time,
-                              domain=pe.NonNegativeReals,
-                              bounds=(self.lower_bound, self.upper_bound))
-
-        if len(self.storage_techs) > 0:
-            self.model.storage_level = pe.Var(
-                self.model.StorageTech,
-                self.model.Time,
-                domain=pe.NonNegativeReals,
-                bounds=(
-                    self.lower_bound,
-                    self.storage_upper_bound))
-            self.model.charge = pe.Var(self.model.StorageTech, self.model.Time,
-                                       domain=pe.NonNegativeReals,
-                                       bounds=(self.lower_bound,
-                                               self.upper_bound))
-
-    def _objective_function(self):
-        expr = sum(self.model.VariableCost[g, t] * self.model.x[g, t]
-                   for g in self.model.Generators for t in self.model.Time)
-        if len(self.storage_techs) > 0:
-            expr += sum(self.model.x[s, t] + self.model.charge[s, t]
-                        for s in self.model.StorageTech for t in self.model.Time) * self.penalty
-        self.model.objective = pe.Objective(sense=pe.minimize, expr=expr)
-
-    def _supply_constraints(self):
-        self.model.oversupply = pe.ConstraintList()
-        self.model.undersupply = pe.ConstraintList()
-        for t in self.model.Time:
-            generation = sum(self.model.x[g, t] for g in self.model.Generators)
-            if len(self.storage_techs) > 0:
-                generation -= sum(self.model.charge[s, t]
-                                  for s in self.model.StorageTech)
-            over_demand = self.model.Demand[t] * (1 + self.oversupply)
-            under_demand = self.model.Demand[t] * (1 - self.undersupply)
-            self.model.oversupply.add(generation <= over_demand)
-            self.model.undersupply.add(generation >= under_demand)
-
-    def _generation_constraint(self):
-        self.model.gen_limit = pe.ConstraintList()
-        for g in self.model.Generators:
-            unit_capacity = (self.capacity_dict[g] * self.time_delta).to_value()
-
-            for t in self.model.Time:
-                unit_generation = self.model.x[g, t]
-                self.model.gen_limit.add(unit_generation <= unit_capacity)
-
-    def _ramping_constraints(self):
-        self.model.ramp_up_limit = pe.ConstraintList()
-        self.model.ramp_down_limit = pe.ConstraintList()
-
-        for r in self.model.RampingTechs:
-            ramp_up = self.model.ramp_up[r]
-            ramp_down = self.model.ramp_down[r]
-            for t in self.model.Time:
-                if t != self.model.Time.first():
-                    t_prev = self.model.Time.prev(t)
-                    previous_gen = self.model.x[r, t_prev]
-                    current_gen = self.model.x[r, t]
-                    delta_power = (current_gen - previous_gen) / \
-                        self.time_delta.to_value()
-                    self.model.ramp_up_limit.add(delta_power <= ramp_up)
-                    self.model.ramp_down_limit.add(delta_power >= -ramp_down)
-
-    def _storage_constraints(self):
-        self.model.discharge_limit = pe.ConstraintList()
-        self.model.charge_limit = pe.ConstraintList()
-        self.model.charge_rate_limit = pe.ConstraintList()
-        self.model.storage_limit = pe.ConstraintList()
-        self.model.set_storage = pe.ConstraintList()
-        for s in self.model.StorageTech:
-            efficiency = self.efficiency_dict[s]
-            storage_cap = self.model.storage_capacity[s]
-            unit_capacity = (self.capacity_dict[s] * self.time_delta).to_value()
-            initial_storage = self.model.initial_storage[s]
-            for t in self.model.Time:
-                self.model.charge_rate_limit.add(
-                    self.model.charge[s, t] <= unit_capacity)
-                if t == self.model.Time.first():
-                    self.model.set_storage.add(self.model.storage_level[s, t]
-                                               == initial_storage)
-                    self.model.discharge_limit.add(
-                        self.model.x[s, t] <= initial_storage)
-                    self.model.charge_limit.add(self.model.charge[s, t]
-                                                <= storage_cap
-                                                - initial_storage)
-                else:
-                    t_prev = self.model.Time.prev(t)
-                    previous_storage = self.model.storage_level[s, t_prev]
-                    current_discharge = self.model.x[s, t]
-                    current_charge = self.model.charge[s, t]
-                    self.model.set_storage.add(
-                        self.model.storage_level[s, t]
-                        == previous_storage
-                        + np.sqrt(efficiency) * current_charge
-                        - np.sqrt(efficiency) * current_discharge
-                    )
-                    self.model.charge_limit.add(
-                        np.sqrt(efficiency) * current_charge
-                        <= storage_cap - previous_storage)
-                    self.model.discharge_limit.add(
-                        current_discharge <= previous_storage)
-                self.model.storage_limit.add(
-                    self.model.storage_level[s, t] <= storage_cap)
-
-    def _write_model_equations(self):
-
-        self._create_model_indices()
-        self._create_demand_param()
-        self._create_cost_param()
-        self._create_model_variables()
-        self._objective_function()
-        self._supply_constraints()
-        self._generation_constraint()
-        if len(self.ramping_techs) > 0:
-            self._create_ramping_params()
-            self._ramping_constraints()
-        if len(self.storage_techs) > 0:
-            self._create_init_storage_params()
-            self._create_max_storage_params()
-            self._storage_constraints()
-        self.model_initialized = True
-
-    def _format_results(self):
-        df = pd.DataFrame(index=self.model.Time)
-        for g in self.model.Generators:
-            df[g] = [self.model.x[g, t].value for t in self.model.Time]
-
-        if len(self.storage_techs) > 0:
-            for s in self.model.StorageTech:
-                df[f"{s}_charge"] = [-1 * self.model.charge[s, t].value
-                                     for t in self.model.Time]
-                df[f"{s}_level"] = [self.model.storage_level[s, t].value
-                                    for t in self.model.Time]
-        return df
-
-    def solve(self, solver=None):
-        """
-        Executes the model solve. Model equations are written at the
-        time the method is called.
-
-        Parameters
-        ----------
-        solver : str
-            Indicates which solver to use. If no solver is specified,
-            the default :attr:`DispatchModel.solver` attribute is used.
-            Default is ['cplex'].
-        """
-        if not self.model_initialized:
-            self._write_model_equations()
-
-        if solver:
-            optimizer = po.SolverFactory(solver)
-        else:
-            optimizer = po.SolverFactory(self.solver)
-
-        results = optimizer.solve(self.model, tee=True)
-        try:
-            self.objective = self.model.objective()
-        except ValueError:
-            warnings.warn(
-                f"Infeasible or no solution. Objective set to {LARGE_NUMBER}")
-            self.objective = LARGE_NUMBER
-
-        self.results = self._format_results()
+import pandas as pd
+import numpy as np
+import pyomo.environ as pe
+import pyomo.opt as po
+from pyomo.environ import ConcreteModel
+from unyt import unyt_array, hr, MW, kW, GW
+import itertools as it
+from osier import Technology
+from osier.technology import _validate_quantity, _validate_unit
+from osier.utils import synchronize_units
+import warnings
+import logging
+import time
+
+
+_freq_opts = {'D': 'day',
+              'H': 'hour',
+              'S': 'second',
+              'T': 'minute'}
+LARGE_NUMBER = 1e20
+MEDIUM_NUMBER = 1e10
+BLACKOUT_COST = 10 * (1 / (kW * hr))  # M$/kWh
+
+
+curtailment_tech = Technology(technology_name='Curtailment',
+                              technology_type='removal',
+                              dispatchable=True,
+                              capacity=MEDIUM_NUMBER)
+reliability_tech = Technology(technology_name='LoadLoss',
+                              technology_type='matching',
+                              dispatchable=True,
+                              fuel_cost=BLACKOUT_COST,
+                              capacity=MEDIUM_NUMBER)
+
+
+class DispatchModel():
+    """
+    The :class:`DispatchModel` class creates and solves a basic dispatch
+    model from the perspective of a "grid operator." The model uses
+    `pyomo <https://pyomo.readthedocs.io/en/stable/index.html>`_
+    to create and solve a linear programming model.
+    The mathematical formulation for this problem is:
+
+    Minimize
+
+
+    .. math::
+        \\text{C}_{\\text{total}} = \\sum_t^T \\sum_u^U
+        \\left[c^{\\text{fuel}}_{u,t} + c^{\\text{om,var}}_{u,t}\\right]x_{u,t}
+
+    Such that,
+
+    1. The generation meets demand within a user-specified tolerance
+    (undersupply and oversupply)
+
+    .. math::
+        \\sum_u^Ux_{u,t} &\\geq \\left(1-\\text{undersupply}\\right)\\text{D}_t
+        \\ \\forall \\ t \\in T
+
+        \\sum_u^Ux_{u,t} &\\leq \\left(1+\\text{oversupply}\\right)\\text{D}_t
+        \\ \\forall \\ t \\in T
+
+    2. A technology's generation (:math:`x_u`) does not exceed its capacity to
+    generate at any time, :math:`t`.
+
+    .. math::
+        x_{u,t} \\leq \\textbf{CAP}_{u}\\Delta t \\ \\forall \\ u,t \\in U,T
+
+    3. Technologies may not exceed their ramp up rate,
+
+    .. math::
+        \\frac{x_{r,t} - x_{r,t-1}}{\\Delta t} = \\Delta P_{r,t} \\leq
+        (\\text{ramp up})\\textbf{CAP}_u\\Delta t \\ \\forall \\ r,t
+        \\in R \\subset U, T
+
+    or ramp down rate,
+
+    .. math::
+        \\frac{x_{r,t} - x_{r,t-1}}{\\Delta t} = \\Delta P_{r,t} \\leq
+        -(\\text{ramp down})\\textbf{CAP}_u\\Delta t \\ \\forall \\ r,t
+        \\in R \\subset U, T .
+
+    Parameters
+    ----------
+    technology_list : list of :class:`osier.Technology`
+        The list of :class:`Technology` objects to dispatch -- i.e. decide
+        how much energy each technology should produce.
+    net_demand : list, :class:`numpy.ndarray`, :class:`unyt.array.unyt_array`, :class:`pandas.DataFrame`
+        The remaining energy demand to be fulfilled by the technologies in
+        :attr:`technology_list`. The `values` of an object passed as
+        `net_demand` are used to create a supply constraint. See
+        :attr:`oversupply` and :attr:`undersupply`.
+        If a :class:`pandas.DataFrame` is passed, :mod:`osier` will try
+        inferring a `time_delta` from the dataframe index. Otherwise, the
+        :attr:`time_delta` must be passed or the default is used.
+    time_delta : str, :class:`unyt.unyt_quantity`, float, int
+        Specifies the amount of time between two time slices. The default is
+        one hour. Can be overridden by specifying a unit with the value. For
+        example:
+
+        >>> time_delta = "5 minutes"
+        >>> from unyt import days
+        >>> time_delta = 30*days
+
+        would both work.
+    power_units : str, :class:`unyt.unit_object`
+        Specifies the units for the power demand. The default is :attr:`MW`.
+        Can be overridden by specifying a unit with the value.
+    solver : str
+        Indicates which solver to use. May require separate installation.
+        Accepts: ['cplex', 'cbc']. Other solvers will be added in the future.
+    lower_bound : float
+        The minimum amount of energy each technology can produce per time
+        period. Default is 0.0.
+    oversupply : float
+        The amount of allowed oversupply as a percentage of demand.
+        Default is 0.0 (no oversupply allowed).
+    undersupply : float
+        The amount of allowed undersupply as a percentage of demand.
+        Default is 0.0 (no undersupply allowed).
+    verbosity : Optional, int
+        Sets the logging level for the simulation. Accepts `logging.LEVEL`
+        or integer where LEVEL is {10:DEBUG, 20:INFO, 30:WARNING, 40:ERROR, 50:CRITICAL}.
+    curtailment : boolean
+        Indicates if the model should enable a curtailment option.
+    allow_blackout : boolean
+        If True, a "reliability" technology is added to the model that will
+        fulfill the mismatch in supply and demand. This reliability technology
+        has a variable cost of 1e4 $/MWh. The value must be higher than the
+        variable cost of any other technology to prevent a pathological
+        preference for blackouts. Default is False.
+
+    Attributes
+    ----------
+    model : :class:`pyomo.environ.ConcreteModel`
+        The :mod:`pyomo` model class that converts python code into a
+        set of linear equations.
+    objective : float
+        The result of the model's objective function. Only instantiated
+        after :meth:`DispatchModel.solve()` is called.
+    n_timesteps : int
+        The number of timesteps in the model.
+    upper_bound : float
+        The upper bound for all decision variables. Chosen to be equal
+        to the maximum capacity of all technologies in :attr:`tech_set`.
+    storage_upper_bound : float
+        The upper bound for storage decision variables.
+    penalty : float
+        The penalty applied to the objective function to eliminate
+        simultaneous charging and discharging. Users may need to tune
+        this parameter. Default is 1e-4.
+    model_initialized : bool
+        Indicates whether :attr:`DispatchModel.model` has been populated
+        with equations yet. This is set to ``True`` after
+        :meth:`DispatchModel._write_model_equations()` has been called.
+    indices : list of tuples
+        The list of tuples representing the product of the
+        :attr:`tech_set` and :attr:`time_set` attributes.
+    tech_set : list of str
+        A list of the unique technology names in the simulation.
+    capacity_dict : dict
+        A dictionary of {name : capacity} pairs.
+    efficiency_dict : dict
+        A dictionary of {name : efficiency} pairs.
+    time_set : iterable
+        The result of ``range(self.n_timesteps)``.
+    cost_params : list
+        The set of cost parameters for each technology. Corresponds to
+        a list of values. Size is equal to the product of the number of
+        timesteps and the number of technologies in the model.
+    ramp_up_params : list
+        The set of ramp_up parameters. Only initialized if there is a
+        ramping technology.
+    ramp_down_params : list
+        The set of ramp_down parameters. Only initialized if there is a
+        ramping technology.
+    ramping_techs : list
+        The subset of :attr:`tech_set` containing ramping technologies.
+
+    Notes
+    -----
+    1. Technically, :attr:`solver` will accept any solver that :class:`pyomo`
+    can use. We only list two solvers because those are the only solvers
+    in the :mod:`osier` test suite.
+
+    2. The default value for :attr:`time_delta` in :attr:`__init__` is
+    `None`. This is replaced by a setter method in :class:`Dispatch`.
+
+    3. This formulation uses a :attr:`penalty` parameter  to prevent unphysical
+    behavior because it preserves the problem's linearity. Some formulations
+    may use a binary variable to prevent simultaneous charging and discharing.
+    However, this changes the problem to a mixed-integer linear program which
+    requires a more sophisticated solver such as ``gurobi``.
+
+    4. :meth:`_write_model_equations` may be called before :meth:`solve` if
+    users wish to add their own constraints or parameters to the problem.
+    """
+
+    def __init__(self,
+                 technology_list,
+                 net_demand,
+                 time_delta=None,
+                 solver='cplex',
+                 lower_bound=0.0,
+                 oversupply=0.0,
+                 undersupply=0.0,
+                 verbosity=50,
+                 penalty=1e-4,
+                 power_units=MW,
+                 curtailment=True,
+                 allow_blackout=False,
+                 **kwargs):
+        self.net_demand = net_demand
+        self.time_delta = time_delta
+        self.lower_bound = lower_bound
+        self.oversupply = oversupply
+        self.undersupply = undersupply
+        self.penalty = penalty
+        self.model = ConcreteModel()
+        self.solver = solver
+        self.results = None
+        self.objective = None
+        self.model_initialized = False
+        self.verbosity = verbosity
+        if self.verbosity > 10:
+            self.verbose = False
+        else: 
+            self.verbose = True
+        self.curtailment = curtailment
+        self.allow_blackout = allow_blackout
+
+        if isinstance(net_demand, unyt_array):
+            self.power_units = net_demand.units
+        else:
+            self.power_units = power_units
+
+        if ((self.curtailment) and (self.allow_blackout)):
+            sync_list = technology_list + [curtailment_tech, reliability_tech]
+        elif self.curtailment:
+            sync_list = technology_list + [curtailment_tech]
+        elif self.allow_blackout:
+            sync_list = technology_list + [reliability_tech]
+        else:
+            sync_list = technology_list
+
+        self.technology_list = synchronize_units(
+            sync_list,
+            unit_power=self.power_units,
+            unit_time=self.time_delta.units)
+
+        
+        logging.getLogger('pyomo.core').setLevel(verbosity)
+
+    @property
+    def time_delta(self):
+        return self._time_delta
+
+    @time_delta.setter
+    def time_delta(self, value):
+        if value:
+            valid_quantity = _validate_quantity(value, dimension='time')
+            self._time_delta = valid_quantity
+        else:
+            if isinstance(self.net_demand, pd.DataFrame):
+                try:
+                    freq_list = list(self.net_demand.index.inferred_freq)
+                    freq_key = freq_list[-1]
+                    try:
+                        value = float(freq_list[0])
+                    except ValueError:
+                        warnings.warn((f"Could not convert value "
+                                       f"{freq_list[0]} to float. "
+                                       "Setting to 1.0."),
+                                      UserWarning)
+                        value = 1.0
+                    self._time_delta = _validate_quantity(
+                        f"{value} {_freq_opts[freq_key]}", dimension='time')
+                except KeyError:
+                    warnings.warn(
+                        (f"Could not infer time delta with freq {freq_key} "
+                         "from pandas dataframe. Setting delta to 1 hour."),
+                        UserWarning)
+                    self._time_delta = 1 * hr
+            else:
+                self._time_delta = 1 * hr
+
+    @property
+    def power_units(self):
+        return self._power_units
+
+    @power_units.setter
+    def power_units(self, value):
+        if value:
+            valid_quantity = _validate_unit(value, dimension='power')
+            self._power_units = valid_quantity
+        else:
+            warnings.warn(f"Could not infer power units. Unit set to MW.")
+            self._power_units = MW
+
+    @property
+    def n_timesteps(self):
+        return len(self.net_demand)
+
+    @property
+    def tech_set(self):
+        tech_names = [t.technology_name for t in self.technology_list]
+        return tech_names
+
+    @property
+    def capacity_dict(self):
+        capacity_set = unyt_array([t.capacity for t in self.technology_list])
+        return dict(zip(self.tech_set, capacity_set))
+
+    @property
+    def efficiency_dict(self):
+        capacity_set = [t.efficiency for t in self.technology_list]
+        return dict(zip(self.tech_set, capacity_set))
+
+    @property
+    def time_set(self):
+        return range(self.n_timesteps)
+
+    @property
+    def indices(self):
+        return list(it.product(self.tech_set, self.time_set))
+
+    @property
+    def cost_params(self):
+        v_costs = np.array([
+            (t.variable_cost_ts(self.n_timesteps))
+            for t in self.technology_list
+        ]).flatten()
+        return dict(zip(self.indices, v_costs))
+
+    @property
+    def storage_techs(self):
+        return [t.technology_name
+                for t in self.technology_list
+                if hasattr(t, "storage_capacity")]
+
+    @property
+    def storage_upper_bound(self):
+        caps = unyt_array([t.storage_capacity
+                           for t in self.technology_list
+                           if hasattr(t, "storage_capacity")])
+        return caps.max().to_value()
+
+    @property
+    def max_storage_params(self):
+        storage_dict = {t.technology_name: t.storage_capacity.to_value()
+                        for t in self.technology_list
+                        if hasattr(t, "storage_capacity")}
+        return storage_dict
+
+    @property
+    def initial_storage_params(self):
+        storage_dict = {t.technology_name: t.initial_storage.to_value()
+                        for t in self.technology_list
+                        if hasattr(t, "initial_storage")}
+        return storage_dict
+
+    @property
+    def ramping_techs(self):
+        return [t.technology_name
+                for t in self.technology_list
+                if hasattr(t, 'ramp_up')]
+
+    @property
+    def ramp_up_params(self):
+        rates_dict = {
+            t.technology_name: (
+                t.ramp_up *
+                self.time_delta).to_value() for t in self.technology_list
+            if hasattr(t, 'ramp_up')}
+        return rates_dict
+
+    @property
+    def ramp_down_params(self):
+        rates_dict = {
+            t.technology_name: (
+                t.ramp_down *
+                self.time_delta).to_value() for t in self.technology_list
+            if hasattr(t, 'ramp_up')}
+        return rates_dict
+
+    @property
+    def upper_bound(self):
+        caps = unyt_array([t.capacity for t in self.technology_list])
+        return caps.max().to_value()
+
+    def _create_model_indices(self):
+        self.model.Generators = pe.Set(initialize=self.tech_set, ordered=True)
+        self.model.Time = pe.Set(initialize=self.time_set, ordered=True)
+        if len(self.ramping_techs) > 0:
+            self.model.RampingTechs = pe.Set(initialize=self.ramping_techs,
+                                             ordered=True,
+                                             within=self.model.Generators)
+        if len(self.storage_techs) > 0:
+            self.model.StorageTech = pe.Set(initialize=self.storage_techs,
+                                            ordered=True,
+                                            within=self.model.Generators)
+
+    def _create_demand_param(self):
+        self.model.Demand = pe.Param(self.model.Time, initialize=dict(
+            zip(self.model.Time, np.array(self.net_demand))))
+
+    def _create_cost_param(self):
+        self.model.VariableCost = pe.Param(
+            self.model.Generators,
+            self.model.Time,
+            initialize=self.cost_params)
+
+    def _create_ramping_params(self):
+        self.model.ramp_up = pe.Param(
+            self.model.RampingTechs, initialize=self.ramp_up_params)
+        self.model.ramp_down = pe.Param(
+            self.model.RampingTechs, initialize=self.ramp_down_params)
+
+    def _create_max_storage_params(self):
+        self.model.storage_capacity = pe.Param(
+            self.model.StorageTech, initialize=self.max_storage_params
+        )
+
+    def _create_init_storage_params(self):
+        self.model.initial_storage = pe.Param(
+            self.model.StorageTech, initialize=self.initial_storage_params
+        )
+
+    def _create_model_variables(self):
+        self.model.x = pe.Var(self.model.Generators, self.model.Time,
+                              domain=pe.NonNegativeReals,
+                              bounds=(self.lower_bound, self.upper_bound))
+
+        if len(self.storage_techs) > 0:
+            self.model.storage_level = pe.Var(
+                self.model.StorageTech,
+                self.model.Time,
+                domain=pe.NonNegativeReals,
+                bounds=(
+                    self.lower_bound,
+                    self.storage_upper_bound))
+            self.model.charge = pe.Var(self.model.StorageTech, self.model.Time,
+                                       domain=pe.NonNegativeReals,
+                                       bounds=(self.lower_bound,
+                                               self.upper_bound))
+
+    def _objective_function(self):
+        expr = sum(self.model.VariableCost[g, t] * self.model.x[g, t]
+                   for g in self.model.Generators for t in self.model.Time)
+        if len(self.storage_techs) > 0:
+            expr += sum(self.model.x[s, t] + self.model.charge[s, t]
+                        for s in self.model.StorageTech
+                        for t in self.model.Time) * self.penalty
+        self.model.objective = pe.Objective(sense=pe.minimize, expr=expr)
+
+    def _supply_constraints(self):
+        self.model.oversupply = pe.ConstraintList()
+        self.model.undersupply = pe.ConstraintList()
+        for t in self.model.Time:
+            generation = sum(self.model.x[g, t] for g in self.model.Generators
+                             if g != 'Curtailment')
+            if self.curtailment:
+                generation -= self.model.x['Curtailment', t]
+            if len(self.storage_techs) > 0:
+                generation -= sum(self.model.charge[s, t]
+                                  for s in self.model.StorageTech)
+            over_demand = self.model.Demand[t] * (1 + self.oversupply)
+            under_demand = self.model.Demand[t] * (1 - self.undersupply)
+            self.model.oversupply.add(generation <= over_demand)
+            self.model.undersupply.add(generation >= under_demand)
+
+    def _generation_constraint(self):
+        self.model.gen_limit = pe.ConstraintList()
+        for g in self.model.Generators:
+            unit_capacity = (
+                self.capacity_dict[g] *
+                self.time_delta).to_value()
+
+            for t in self.model.Time:
+                unit_generation = self.model.x[g, t]
+                self.model.gen_limit.add(unit_generation <= unit_capacity)
+
+    def _ramping_constraints(self):
+        self.model.ramp_up_limit = pe.ConstraintList()
+        self.model.ramp_down_limit = pe.ConstraintList()
+
+        for r in self.model.RampingTechs:
+            ramp_up = self.model.ramp_up[r]
+            ramp_down = self.model.ramp_down[r]
+            for t in self.model.Time:
+                if t != self.model.Time.first():
+                    t_prev = self.model.Time.prev(t)
+                    previous_gen = self.model.x[r, t_prev]
+                    current_gen = self.model.x[r, t]
+                    delta_power = (current_gen - previous_gen) / \
+                        self.time_delta.to_value()
+                    self.model.ramp_up_limit.add(delta_power <= ramp_up)
+                    self.model.ramp_down_limit.add(delta_power >= -ramp_down)
+
+    def _storage_constraints(self):
+        self.model.discharge_limit = pe.ConstraintList()
+        self.model.charge_limit = pe.ConstraintList()
+        self.model.charge_rate_limit = pe.ConstraintList()
+        self.model.storage_limit = pe.ConstraintList()
+        self.model.set_storage = pe.ConstraintList()
+        for s in self.model.StorageTech:
+            efficiency = self.efficiency_dict[s]
+            storage_cap = self.model.storage_capacity[s]
+            unit_capacity = (
+                self.capacity_dict[s] *
+                self.time_delta).to_value()
+            initial_storage = self.model.initial_storage[s]
+            for t in self.model.Time:
+                self.model.charge_rate_limit.add(
+                    self.model.charge[s, t] <= unit_capacity)
+                if t == self.model.Time.first():
+                    self.model.set_storage.add(self.model.storage_level[s, t]
+                                               == initial_storage)
+                    self.model.discharge_limit.add(
+                        self.model.x[s, t] <= initial_storage)
+                    self.model.charge_limit.add(self.model.charge[s, t]
+                                                <= storage_cap
+                                                - initial_storage)
+                else:
+                    t_prev = self.model.Time.prev(t)
+                    previous_storage = self.model.storage_level[s, t_prev]
+                    current_discharge = self.model.x[s, t]
+                    current_charge = self.model.charge[s, t]
+                    self.model.set_storage.add(
+                        self.model.storage_level[s, t]
+                        == previous_storage
+                        + np.sqrt(efficiency) * current_charge
+                        - np.sqrt(efficiency) * current_discharge
+                    )
+                    self.model.charge_limit.add(
+                        np.sqrt(efficiency) * current_charge
+                        <= storage_cap - previous_storage)
+                    self.model.discharge_limit.add(
+                        current_discharge <= previous_storage)
+                self.model.storage_limit.add(
+                    self.model.storage_level[s, t] <= storage_cap)
+
+    def _write_model_equations(self):
+
+        self._create_model_indices()
+        self._create_demand_param()
+        self._create_cost_param()
+        self._create_model_variables()
+        self._objective_function()
+        self._supply_constraints()
+        self._generation_constraint()
+        if len(self.ramping_techs) > 0:
+            self._create_ramping_params()
+            self._ramping_constraints()
+        if len(self.storage_techs) > 0:
+            self._create_init_storage_params()
+            self._create_max_storage_params()
+            self._storage_constraints()
+        self.model_initialized = True
+
+    def _format_results(self):
+        df = pd.DataFrame(index=self.model.Time)
+        for g in self.model.Generators:
+            if g == 'Curtailment':
+                df[g] = [-1 * self.model.x[g, t].value for t in self.model.Time]
+            else:
+                df[g] = [self.model.x[g, t].value for t in self.model.Time]
+
+        if len(self.storage_techs) > 0:
+            for s in self.model.StorageTech:
+                df[f"{s}_charge"] = [-1 * self.model.charge[s, t].value
+                                     for t in self.model.Time]
+                df[f"{s}_level"] = [self.model.storage_level[s, t].value
+                                    for t in self.model.Time]
+
+        df["Cost"] = np.array(sum(self.model.VariableCost[g, t] * self.model.x[g, t].value
+                                  for g in self.model.Generators) for t in self.model.Time)
+
+        return df
+
+    def solve(self, solver=None):
+        """
+        Executes the model solve. Model equations are written at the
+        time the method is called.
+
+        Parameters
+        ----------
+        solver : str
+            Indicates which solver to use. If no solver is specified,
+            the default :attr:`DispatchModel.solver` attribute is used.
+            Default is ['cplex'].
+        """
+        if not self.model_initialized:
+            self._write_model_equations()
+
+        if solver:
+            optimizer = po.SolverFactory(solver)
+        else:
+            optimizer = po.SolverFactory(self.solver)
+
+        results = optimizer.solve(self.model, tee=self.verbose)
+        try:
+            self.objective = self.model.objective()
+        except ValueError:
+            if self.verbosity <= 30:
+                warnings.warn(
+                    f"Infeasible or no solution. Objective set to {LARGE_NUMBER}")
+            self.objective = LARGE_NUMBER
+
+        try:
+            self.results = self._format_results()
+        except TypeError:
+            self.results = None
```
