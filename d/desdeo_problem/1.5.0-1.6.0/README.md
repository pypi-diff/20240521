# Comparing `tmp/desdeo_problem-1.5.0.tar.gz` & `tmp/desdeo_problem-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desdeo_problem-1.5.0.tar", max compression
+gzip compressed data, was "desdeo_problem-1.6.0.tar", max compression
```

## Comparing `desdeo_problem-1.5.0.tar` & `desdeo_problem-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2022-04-29 11:12:23.433453 desdeo_problem-1.5.0/LICENSE
--rw-r--r--   0        0        0     2118 2022-04-29 11:12:23.433453 desdeo_problem-1.5.0/desdeo_problem/__init__.py
--rw-r--r--   0        0        0     7862 2022-04-29 11:12:23.433453 desdeo_problem-1.5.0/desdeo_problem/problem/Constraint.py
--rw-r--r--   0        0        0    32859 2022-08-26 12:58:38.483965 desdeo_problem-1.5.0/desdeo_problem/problem/Objective.py
--rw-r--r--   0        0        0    64505 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/problem/Problem.py
--rw-r--r--   0        0        0     5773 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/problem/Variable.py
--rw-r--r--   0        0        0     1660 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/problem/__init__.py
--rw-r--r--   0        0        0      742 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/surrogatemodels/SurrogateModels.py
--rw-r--r--   0        0        0      285 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/surrogatemodels/__init__.py
--rw-r--r--   0        0        0     2055 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/surrogatemodels/lipschitzian.py
--rw-r--r--   0        0        0     8977 2022-08-23 05:33:03.156285 desdeo_problem-1.5.0/desdeo_problem/testproblems/CarSideImpact.py
--rw-r--r--   0        0        0    58398 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/DBMOPP_generator.py
--rw-r--r--   0        0        0     1747 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/README.md
--rw-r--r--   0        0        0     4029 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/Region.py
--rw-r--r--   0        0        0      480 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/__init__.py
--rw-r--r--   0        0        0     2625 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/utilities.py
--rw-r--r--   0        0        0     1406 2022-04-29 11:45:29.426738 desdeo_problem-1.5.0/desdeo_problem/testproblems/DummyProblem.py
--rw-r--r--   0        0        0    28004 2022-08-23 05:33:03.156285 desdeo_problem-1.5.0/desdeo_problem/testproblems/EngineeringRealWorld.py
--rw-r--r--   0        0        0    54074 2022-09-01 06:24:30.395431 desdeo_problem-1.5.0/desdeo_problem/testproblems/GAA.py
--rw-r--r--   0        0        0     7079 2022-09-01 06:24:30.395431 desdeo_problem-1.5.0/desdeo_problem/testproblems/MultipleClutchBrakes.py
--rw-r--r--   0        0        0     2905 2022-05-27 11:27:44.062677 desdeo_problem-1.5.0/desdeo_problem/testproblems/RiverPollution.py
--rw-r--r--   0        0        0     3893 2022-04-29 11:12:23.436787 desdeo_problem-1.5.0/desdeo_problem/testproblems/TestProblems.py
--rw-r--r--   0        0        0     3041 2022-05-27 11:27:44.062677 desdeo_problem-1.5.0/desdeo_problem/testproblems/VehicleCrashworthiness.py
--rw-r--r--   0        0        0     1414 2022-08-26 08:23:41.724088 desdeo_problem-1.5.0/desdeo_problem/testproblems/__init__.py
--rw-r--r--   0        0        0      953 2023-03-02 09:38:32.170159 desdeo_problem-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 desdeo_problem-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-10-04 11:03:35.451714 desdeo_problem-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2116 2023-10-04 11:25:39.451686 desdeo_problem-1.6.0/desdeo_problem/__init__.py
+-rw-r--r--   0        0        0     7777 2023-10-04 11:44:34.564337 desdeo_problem-1.6.0/desdeo_problem/problem/Constraint.py
+-rw-r--r--   0        0        0    32770 2023-10-26 11:28:39.810867 desdeo_problem-1.6.0/desdeo_problem/problem/Objective.py
+-rw-r--r--   0        0        0    64813 2023-11-04 13:39:30.001033 desdeo_problem-1.6.0/desdeo_problem/problem/Problem.py
+-rw-r--r--   0        0        0     5655 2023-10-26 11:41:59.850949 desdeo_problem-1.6.0/desdeo_problem/problem/Variable.py
+-rw-r--r--   0        0        0     1660 2023-10-04 11:25:39.478692 desdeo_problem-1.6.0/desdeo_problem/problem/__init__.py
+-rw-r--r--   0        0        0      711 2023-10-26 11:42:25.895208 desdeo_problem-1.6.0/desdeo_problem/surrogatemodels/SurrogateModels.py
+-rw-r--r--   0        0        0      285 2023-10-04 11:25:39.476887 desdeo_problem-1.6.0/desdeo_problem/surrogatemodels/__init__.py
+-rw-r--r--   0        0        0     1990 2023-10-26 11:42:56.071792 desdeo_problem-1.6.0/desdeo_problem/surrogatemodels/lipschitzian.py
+-rw-r--r--   0        0        0     8798 2023-10-26 11:51:57.242695 desdeo_problem-1.6.0/desdeo_problem/testproblems/CarSideImpact.py
+-rw-r--r--   0        0        0    57149 2023-11-04 14:03:59.671020 desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/DBMOPP_generator.py
+-rw-r--r--   0        0        0     1747 2023-10-04 11:03:35.453865 desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/README.md
+-rw-r--r--   0        0        0     4029 2023-10-04 11:25:39.512036 desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/Region.py
+-rw-r--r--   0        0        0      480 2023-10-04 11:03:35.454113 desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/__init__.py
+-rw-r--r--   0        0        0     2625 2023-10-04 11:25:39.515468 desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/utilities.py
+-rw-r--r--   0        0        0     1403 2023-10-04 11:22:38.084741 desdeo_problem-1.6.0/desdeo_problem/testproblems/DummyProblem.py
+-rw-r--r--   0        0        0    28945 2023-10-26 11:50:52.150882 desdeo_problem-1.6.0/desdeo_problem/testproblems/EngineeringRealWorld.py
+-rw-r--r--   0        0        0    73770 2023-10-26 11:52:42.586037 desdeo_problem-1.6.0/desdeo_problem/testproblems/GAA.py
+-rw-r--r--   0        0        0     6613 2023-10-04 11:25:39.632604 desdeo_problem-1.6.0/desdeo_problem/testproblems/MultipleClutchBrakes.py
+-rw-r--r--   0        0        0     2926 2023-10-04 11:25:39.563336 desdeo_problem-1.6.0/desdeo_problem/testproblems/RiverPollution.py
+-rw-r--r--   0        0        0     3866 2023-10-04 11:25:39.605070 desdeo_problem-1.6.0/desdeo_problem/testproblems/TestProblems.py
+-rw-r--r--   0        0        0     3056 2023-10-04 11:35:57.466508 desdeo_problem-1.6.0/desdeo_problem/testproblems/VehicleCrashworthiness.py
+-rw-r--r--   0        0        0     1050 2023-10-04 11:29:22.436247 desdeo_problem-1.6.0/desdeo_problem/testproblems/__init__.py
+-rw-r--r--   0        0        0     2100 2024-05-21 11:50:19.556318 desdeo_problem-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 desdeo_problem-1.6.0/PKG-INFO
```

### Comparing `desdeo_problem-1.5.0/LICENSE` & `desdeo_problem-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `desdeo_problem-1.5.0/desdeo_problem/__init__.py` & `desdeo_problem-1.6.0/desdeo_problem/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     "GaussianProcessRegressor",
     "LipschitzianRegressor",
     "ModelError",
     "DiscreteDataProblem",
     "test_problem_builder",
     "DBMOPP_generator",
     "Region",
-    "get_2D_version", 
-    "euclidean_distance", 
-    "convhull", 
-    "in_hull", 
-    "get_random_angles", 
-    "between_lines_rooted_at_pivot", 
+    "get_2D_version",
+    "euclidean_distance",
+    "convhull",
+    "in_hull",
+    "get_random_angles",
+    "between_lines_rooted_at_pivot",
     "assign_design_dimension_projection",
 ]
 
 
 from desdeo_problem.problem import (
     ObjectiveError,
     ObjectiveEvaluationResults,
@@ -65,19 +65,20 @@
     DiscreteDataProblem,
     Variable,
     VariableBuilderError,
     VariableError,
     variable_builder,
 )
 
-from desdeo_problem.surrogatemodels import (
-    BaseRegressor,
-    GaussianProcessRegressor,
-    LipschitzianRegressor,
-    ModelError,
-)
+from desdeo_problem.surrogatemodels import BaseRegressor, GaussianProcessRegressor, LipschitzianRegressor, ModelError
 from desdeo_problem.testproblems.TestProblems import test_problem_builder
 
 from desdeo_problem.testproblems.DBMOPP.DBMOPP_generator import DBMOPP_generator
 from desdeo_problem.testproblems.DBMOPP.Region import Region
 
-from desdeo_problem.testproblems.DBMOPP.utilities import get_2D_version, euclidean_distance, get_random_angles, between_lines_rooted_at_pivot, assign_design_dimension_projection
+from desdeo_problem.testproblems.DBMOPP.utilities import (
+    get_2D_version,
+    euclidean_distance,
+    get_random_angles,
+    between_lines_rooted_at_pivot,
+    assign_design_dimension_projection,
+)
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/problem/Constraint.py` & `desdeo_problem-1.6.0/desdeo_problem/problem/Constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Module for problem constraint definition related classes and functions.
 
 """
 from abc import ABC, abstractmethod
-from os import path
-from typing import Callable, List
+from collections.abc import Callable
 
 import numpy as np
 
 
 class ConstraintError(Exception):
     """Raised when an error related to the Constraint class in encountered."""
 
@@ -33,15 +32,14 @@
             been violated. A positive value represents no violation and a
             negative value represents a violation. The absolute value of the
             returned float functions as an indicator of the severity of the
             violation (or how well the constraint holds, if the returned value
             of positive).
 
         """
-        pass
 
 
 class ScalarConstraint(ConstraintBase):
     """A simple scalar constraint that evaluates to a single scalar.
 
     Arguments:
         name (str): Name of the constraint.
@@ -57,21 +55,15 @@
             constraint.
         __n_objective_funs (int): Number of objective functions present in
             the constraint.
         __evaluator (Callable): A callable to evaluate the constraint.
 
     """
 
-    def __init__(
-        self,
-        name: str,
-        n_decision_vars: int,
-        n_objective_funs: int,
-        evaluator: Callable,
-    ) -> None:
+    def __init__(self, name: str, n_decision_vars: int, n_objective_funs: int, evaluator: Callable) -> None:
         self.__name: str = name
         self.__n_decision_vars: int = n_decision_vars
         self.__n_objective_funs: int = n_objective_funs
         self.__evaluator: Callable = evaluator
 
     @property
     def name(self) -> str:
@@ -80,15 +72,15 @@
         Returns:
             str: Name of the constraint
         """
         return self.__name
 
     @property
     def n_decision_vars(self) -> int:
-        """Property: number of decision variables
+        """Property: number of decision variables.
 
         Returns:
             int: Number of decision variables
         """
         return self.__n_decision_vars
 
     @property
@@ -152,21 +144,21 @@
             raise ConstraintError(msg)
         try:
             result = self.__evaluator(decision_vector, objective_vector)
         except (TypeError, IndexError) as e:
             msg = ("Bad arguments {} and {} supplied to the evaluator:" " {}").format(
                 str(decision_vector), objective_vector, str(e)
             )
-            raise ConstraintError(msg)
+            raise ConstraintError(msg) from e
 
         return result
 
 
-supported_operators: List[str] = ["==", "<", ">"]
-"""List[str]: Shows the operators supported in the
+supported_operators: list[str] = ["==", "<", ">"]
+"""list[str]: Shows the operators supported in the
 constraint_function_factory."""
 
 
 def constraint_function_factory(lhs: Callable, rhs: float, operator: str) -> Callable:
     """A function that creates an evaluator.
 
     This function creates an evaluator to be used with the ScalarConstraint
@@ -189,15 +181,15 @@
         direct indicator how the constraint is violated/agdreed with.
 
     Raises:
         ValueError: The supplied operator is not supported.
 
     """
     if operator not in supported_operators:
-        msg = "The operator {} supplied is not supported.".format(operator)
+        msg = f"The operator {operator} supplied is not supported."
         raise ValueError(msg)
 
     if operator == "==":
 
         def equals(decision_vector: np.ndarray, objective_vector: np.ndarray) -> float:
             return -abs(lhs(decision_vector, objective_vector) - rhs)
 
@@ -215,9 +207,9 @@
         def gt(decision_vector: np.ndarray, objective_vector: np.ndarray) -> float:
             return lhs(decision_vector, objective_vector) - rhs
 
         return gt
 
     else:
         # if for some reason a bad operator falls through
-        msg = "Bad operator argument supplied: {}".format(operator)
+        msg = f"Bad operator argument supplied: {operator}"
         raise ValueError(msg)
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/problem/Objective.py` & `desdeo_problem-1.6.0/desdeo_problem/problem/Objective.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Defines Objective classes to be used in Problems
 
 """
 
 from abc import ABC, abstractmethod
-from os import path
-from typing import Callable, Dict, List, NamedTuple, Tuple, Union
+from collections.abc import Callable
+from typing import NamedTuple
 
 import numpy as np
 import pandas as pd
 from desdeo_problem.surrogatemodels.SurrogateModels import BaseRegressor, ModelError
 
 
 class ObjectiveError(Exception):
@@ -22,16 +22,16 @@
         objectives (Union[float, np.ndarray]): The objective function value/s for the
             input vector.
         uncertainity (Union[None, float, np.ndarray]): The uncertainity in the
             objective value/s.
 
     """
 
-    objectives: Union[float, np.ndarray]
-    uncertainity: Union[None, float, np.ndarray] = None
+    objectives: float | np.ndarray
+    uncertainity: None | float | np.ndarray = None
 
     def __str__(self):
         """Stringify the result.
 
         Returns:
             str: result in string form
         """
@@ -47,54 +47,52 @@
     """The abstract base class for objectives."""
 
     def evaluate(self, decision_vector: np.ndarray, use_surrogate: bool = False) -> ObjectiveEvaluationResults:
         """Evaluates the objective according to a decision variable vector.
 
         Uses surrogate model if use_surrogates is true. If use_surrogates is False, uses
         func_evaluate which evaluates using the true objective function.
-        
+
         Arguments:
             decision_vector (np.ndarray): A vector of Variables to be used in
                 the evaluation of the objective.
             use_surrogate (bool) : A boolean which determines whether to use surrogates
                 or true function evaluator. False by default.
 
         """
         if use_surrogate:
             return self._surrogate_evaluate(decision_vector)
         else:
             return self._func_evaluate(decision_vector)
 
     @abstractmethod
     def _func_evaluate(self, decision_vector: np.ndarray) -> ObjectiveEvaluationResults:
-        """Evaluates the true objective value. 
+        """Evaluates the true objective value.
 
         Value is evaluated with the decision variable vector as the input.
         Uses the true (potentially expensive) evaluator if available.
 
         Arguments:
             decision_vector (np.ndarray): A vector of Variables to be used in
                 the evaluation of the objective.
 
         """
-        pass
 
     @abstractmethod
     def _surrogate_evaluate(self, decision_vector: np.ndarray) -> ObjectiveEvaluationResults:
-        """Evaluates the objective value. 
+        """Evaluates the objective value.
 
         Value is evaluated with the decision variable vector as the input.
         Uses the surrogartes if available.
 
         Arguments:
             decision_vector(np.ndarray): A vector of Variables to be used in
                 the evaluation of the objective.
 
         """
-        pass
 
 
 class VectorObjectiveBase(ABC):
     """The abstract base class for multiple objectives which are calculated at once."""
 
     def evaluate(self, decision_vector: np.ndarray, use_surrogate: bool = False) -> ObjectiveEvaluationResults:
         """Evaluates the objective according to a decision variable vector.
@@ -121,69 +119,66 @@
         Uses the true (potentially expensive) evaluator if available.
 
         Arguments:
             decision_vector (np.ndarray): A vector of Variables to be used in
                 the evaluation of the objective.
 
         """
-        pass
 
     @abstractmethod
     def _surrogate_evaluate(self, decision_vector: np.ndarray) -> ObjectiveEvaluationResults:
         """Evaluates the objective values according to a decision variable vector.
 
         Uses the surrogartes if available.
 
         Arguments:
             decision_vector (np.ndarray): A vector of Variables to be used in
                 the evaluation of the objective.
 
         """
-        pass
 
 
-# TODO: Depreciate
+# TODO @light-weaver: Depricate
 class ScalarObjective(ObjectiveBase):
     """A simple objective function that returns a scalar.
 
     To be depreciated
 
     Arguments:
         name (str): Name of the objective.
         evaluator (Callable): The function to evaluate the objective's value.
         lower_bound (float): The lower bound of the objective.
         upper_bound (float): The upper bound of the objective.
-        maximize (bool): Boolean to determine whether the objective is to be 
-                        maximized.                     
+        maximize (bool): Boolean to determine whether the objective is to be maximized.
 
     Attributes:
         __name (str): Name of the objective.
         __value (float): The current value of the objective function.
         __evaluator (Callable): The function to evaluate the objective's value.
         __lower_bound (float): The lower bound of the objective.
         __upper_bound (float): The upper bound of the objective.
-        maximize (List[bool]): List of boolean to determine whether the objectives are
+        maximize (list[bool]): List of boolean to determine whether the objectives are
             to be maximized. All false by default
 
     Raises:
         ObjectiveError: When ill formed bounds are given.
 
     """
 
     def __init__(
         self,
         name: str,
         evaluator: Callable,
         lower_bound: float = -np.inf,
         upper_bound: float = np.inf,
-        maximize: List[bool] = None,
+        maximize: list[bool] | None = None,
     ) -> None:
         # Check that the bounds make sense
         if not (lower_bound < upper_bound):
-            msg = ("Lower bound {} should be less than the upper bound " "{}.").format(lower_bound, upper_bound)
+            msg = f"Lower bound {lower_bound} should be less than the upper bound {upper_bound}."
             raise ObjectiveError(msg)
 
         self.__name: str = name
         self.__evaluator: Callable = evaluator
         self.__value: float = 0.0
         self.__lower_bound: float = lower_bound
         self.__upper_bound: float = upper_bound
@@ -258,16 +253,16 @@
         Raises:
             ObjectiveError: When a bad argument is supplied to the evaluator.
 
         """
         try:
             result = self.evaluator(decision_vector)
         except (TypeError, IndexError) as e:
-            msg = "Bad argument {} supplied to the evaluator: {}".format(str(decision_vector), str(e))
-            raise ObjectiveError(msg)
+            msg = f"Bad argument {decision_vector} supplied to the evaluator."
+            raise ObjectiveError(msg) from e
 
         # Store the value of the objective
         self.value = result
         uncertainity = np.full_like(result, np.nan, dtype=float)
         # Have to set dtype because if the tuple is of ints, then this array also
         # becomes dtype int. There's no nan value of int type
         return ObjectiveEvaluationResults(result, uncertainity)
@@ -291,80 +286,80 @@
     pass
 
 
 # TODO: Rename to "Objective"
 class VectorObjective(VectorObjectiveBase):
     """An objective function vector with one or more objective functions.
 
-    To be renamed to Objective
+     To be renamed to Objective
 
-    Attributes:
-        __name (List[str]): Names of the various objectives in a list
-        __evaluator (Callable): The function that evaluates the objective values
-        __lower_bounds (Union[List[float], np.ndarray), optional): Lower bounds
-            of the objective values. Defaults to None.
-        __upper_bounds (Union[List[float], np.ndarray), optional): Upper bounds
-            of the objective values. Defaults to None.
-        __maximize (List[bool]): *List* of boolean to determine whether the
-            objectives are to be maximized. All false by default
-        __n_of_objects (int): The number of objectives
-
-   Arguments:
-        name (List[str]): Names of the various objectives in a list
-        evaluator (Callable): The function that evaluates the objective values
-        lower_bounds (Union[List[float], np.ndarray), optional): Lower bounds of the
-            objective values. Defaults to None.
-        upper_bounds (Union[List[float], np.ndarray), optional): Upper bounds of the
-            objective values. Defaults to None.
-        maximize (List[bool]): *List* of boolean to determine whether the objectives are
-            to be maximized. All false by default
+     Attributes:
+         __name (list[str]): Names of the various objectives in a list
+         __evaluator (Callable): The function that evaluates the objective values
+         __lower_bounds (Union[list[float], np.ndarray), optional): Lower bounds
+             of the objective values. Defaults to None.
+         __upper_bounds (Union[list[float], np.ndarray), optional): Upper bounds
+             of the objective values. Defaults to None.
+         __maximize (list[bool]): *List* of boolean to determine whether the
+             objectives are to be maximized. All false by default
+         __n_of_objects (int): The number of objectives
 
-    Raises:
-        ObjectiveError: When lengths the input arrays are different.
-        ObjectiveError: When any of the lower bounds is not smaller than the
-            corresponding upper bound.
+    Arguments:
+         name (list[str]): Names of the various objectives in a list
+         evaluator (Callable): The function that evaluates the objective values
+         lower_bounds (Union[list[float], np.ndarray), optional): Lower bounds of the
+             objective values. Defaults to None.
+         upper_bounds (Union[list[float], np.ndarray), optional): Upper bounds of the
+             objective values. Defaults to None.
+         maximize (list[bool]): *List* of boolean to determine whether the objectives are
+             to be maximized. All false by default
+
+     Raises:
+         ObjectiveError: When lengths the input arrays are different.
+         ObjectiveError: When any of the lower bounds is not smaller than the
+             corresponding upper bound.
 
     """
 
     def __init__(
         self,
-        name: List[str],
+        name: list[str],
         evaluator: Callable,
-        lower_bounds: Union[List[float], np.ndarray] = None,
-        upper_bounds: Union[List[float], np.ndarray] = None,
-        maximize: List[bool] = None,
+        lower_bounds: list[float] | np.ndarray | None = None,
+        upper_bounds: list[float] | np.ndarray | None = None,
+        maximize: list[bool] | None = None,
     ):
         n_of_objectives = len(name)
         if lower_bounds is None:
             lower_bounds = np.full(n_of_objectives, -np.inf)
         if upper_bounds is None:
             upper_bounds = np.full(n_of_objectives, np.inf)
         lower_bounds = np.asarray(lower_bounds)
         upper_bounds = np.asarray(upper_bounds)
         # Check if list lengths are the same
-        if not (n_of_objectives == len(lower_bounds)):
+        if n_of_objectives != len(lower_bounds):
             msg = (
                 "The length of the list of names and the number of elements in the "
                 "lower_bounds array should be the same"
             )
             raise ObjectiveError(msg)
-        if not (n_of_objectives == len(upper_bounds)):
+        if n_of_objectives != len(upper_bounds):
             msg = (
                 "The length of the list of names and the number of elements in the "
                 "upper_bounds array should be the same"
             )
             raise ObjectiveError(msg)
         # Check if all lower bounds are smaller than the corresponding upper bounds
         if not (np.all(lower_bounds < upper_bounds)):
             msg = "Lower bounds should be less than the upper bound "
             raise ObjectiveError(msg)
-        self.__name: List[str] = name
+        self.__name: list[str] = name
         self.__n_of_objectives: int = n_of_objectives
         self.__evaluator: Callable = evaluator
-        self.__values: Tuple[float] = (0.0,) * n_of_objectives
+        self.__values: tuple[float] = (0.0,) * n_of_objectives
         self.__lower_bounds: np.ndarray = lower_bounds
         self.__upper_bounds: np.ndarray = upper_bounds
         if maximize is None:
             self.maximize = [False] * n_of_objectives
         else:
             self.maximize: bool = maximize
 
@@ -383,28 +378,28 @@
 
         Returns:
             int: the number of objectives
         """
         return self.__n_of_objectives
 
     @property
-    def values(self) -> Tuple[float]:
+    def values(self) -> tuple[float]:
         """Property: values
 
         Returns:
-            Tuple[float]: Evaluated value and uncertainty of evaluation
+            tuple[float]: Evaluated value and uncertainty of evaluation
         """
         return self.__values
 
     @values.setter
-    def values(self, values: Tuple[float]):
+    def values(self, values: tuple[float]):
         """Setter: values
 
         Arguments:
-            values (Tuple[float]): Value of the objective and its uncertainty.
+            values (tuple[float]): Value of the objective and its uncertainty.
         """
         self.__values = values
 
     @property
     def evaluator(self) -> Callable:
         """Property: evaluator
 
@@ -445,16 +440,16 @@
             ObjectiveError: When a bad argument is supplies to the evaluator or when
                 the evaluator returns an unexpected number of outputs.
 
         """
         try:
             result = self.evaluator(decision_vector)
         except (TypeError, IndexError) as e:
-            msg = "Bad argument {} supplied to the evaluator: {}".format(str(decision_vector), str(e))
-            raise ObjectiveError(msg)
+            msg = f"Bad argument {decision_vector} supplied to the evaluator."
+            raise ObjectiveError(msg) from e
         result = tuple(result)
 
         # Store the value of the objective
         self.values = result
         uncertainity = np.full_like(result, np.nan, dtype=float)
         # Have to set dtype because if the tuple is of ints, then this array also
         # becomes dtype int. There's no nan value of int type
@@ -477,74 +472,75 @@
         X (pd.DataFrame): Dataframe with corresponds the points where the
                             objective value is known.
         y (pd.Series): The objective values corresponding the points.
         variable_names (pd.Index): The names of the variables in X
         _model(BaseRegressor): Model of the data
 
     Arguments:
-        name (List[str]): The name of the objective. Should be the same as a
+        name (list[str]): The name of the objective. Should be the same as a
                             column name in the data.
         data (pd.DataFrame): The data in a pandas dataframe. The columns
                             should be named after variables/objective.
         evaluator (Union[None, Callable], optional): A python function that
             contains the analytical function or calls the simulator to get the
             true objective value. By default None, as this is not required.
         lower_bound (float, optional): Lower bound of the objective,
                                         by default -np.inf
         upper_bound (float, optional): Upper bound of the objective,
                                         by default np.inf
-        maximize (List[bool], optional): Boolean describing whether the
+        maximize (list[bool], optional): Boolean describing whether the
             objective is to be maximized or not, by default None, which
             defaults to [False], hence minimizes.
 
 
     Raises:
         ObjectiveError:  When the name provided during initialization does not
             match any name in the columns of the data provided during
             initilizaiton.
     """
+
     def __init__(
         self,
-        name: List[str],
+        name: list[str],
         data: pd.DataFrame,
-        evaluator: Union[None, Callable] = None,
+        evaluator: None | Callable = None,
         lower_bound: float = -np.inf,
         upper_bound: float = np.inf,
-        maximize: List[bool] = None,
+        maximize: list[bool] | None = None,
     ) -> None:
         if name in data.columns:
             super().__init__(name, evaluator, lower_bound, upper_bound, maximize)
         else:
             msg = f'Name "{name}" not found in the dataframe provided'
             raise ObjectiveError(msg)
         self.X = data.drop(name, axis=1)
         self.y = data[name]
         self.variable_names = self.X.columns
         self._model = None
-        self.__evaluator = evaluator #this is how we added analatycal function
+        self.__evaluator = evaluator  # this is how we added analatycal function
 
     def train(
         self,
         model: BaseRegressor,
-        model_parameters: Dict = None,
-        index: List[int] = None,
+        model_parameters: dict | None = None,
+        index: list[int] | None = None,
         data: pd.DataFrame = None,
     ):
         """Train surrogate model for the objective.
 
         Arguments:
             model (BaseRegressor): A regressor. The regressor, when
                 initialized, should have a fit method and a predict method.
                 The predict method should return the predicted objective value,
                 as well as the uncertainity value, in a tuple. If the
                 regressor does not support calculating uncertainity, return a
                 tuple of objective value and None.
-            model_parameters (Dict): **model_parameters is passed to the model
+            model_parameters (dict): **model_parameters is passed to the model
                                         when initialized.
-            index (List[int], optional): Indices of the samples (in self.X and
+            index (list[int], optional): Indices of the samples (in self.X and
                 self.y), to be used to train the surrogate model. By default
                 None, which trains the model on the entire dataset. This
                 behaviour may be changed in the future to support test-train
                 split or cross validation.
             data (pd.DataFrame, optional): Extra data to be used for training
                 only. This data is not saved. By default None, which then uses
                 self.X and self.y for training.
@@ -582,17 +578,17 @@
                             supplied to the model
 
         """
         if self._model is None:
             raise ObjectiveError("Model not trained yet")
         try:
             result, uncertainity = self._model.predict(decision_vector)
-        except ModelError:
+        except ModelError as e:
             msg = "Bad argument supplied to the model"
-            raise ObjectiveError(msg)
+            raise ObjectiveError(msg) from e
         return ObjectiveEvaluationResults(result, uncertainity)
 
     def _func_evaluate(self, decision_vector: np.ndarray) -> ObjectiveEvaluationResults:
         """Evaluate the values with analytical function.
 
         Arguments:
             decision_vector (np.ndarray): Variable values where evaluation is
@@ -605,113 +601,112 @@
             ObjectiveError: If the analytical function is not provided
 
         """
         if self.evaluator is None:
             msg = "No analytical function provided"
             raise ObjectiveError(msg)
         results = super()._func_evaluate(decision_vector)
-        #self.X = np.vstack((self.X, decision_vector))    #changes bhupinder and pouya made
-        #self.y = np.vstack((self.y, results.objectives)) #changes bhupinder and pouya made
-         
+        # self.X = np.vstack((self.X, decision_vector))    #changes bhupinder and pouya made
+        # self.y = np.vstack((self.y, results.objectives)) #changes bhupinder and pouya made
+
         return results
 
 
 class _ScalarDataObjective(ScalarDataObjective):
     pass
 
 
 class VectorDataObjective(VectorObjective):
-    """A Objective class for multi/valued objectives.      
+    """A Objective class for multi/valued objectives.
 
     Use when the an evaluator/simulator returns a multiple objective values or
     when there is no evaluator/simulator.
 
     Attributes:
         X (pd.DataFrame): Dataframe with corresponds the points where the
                             objective value is known.
         y (pd.Series): The objective values corresponding the points.
         variable_names (pd.Index): The names of the variables in X
-        _model(Dict): BaseRegressor (or None if not trained) models for each
+        _model(dict): BaseRegressor (or None if not trained) models for each
                         objective, keys are the names of objectives.
-        _model_trained(Dict): boolean if model is trained for each objective,
+        _model_trained(dict): boolean if model is trained for each objective,
                             keys are the names of objectives. Default false.
 
     Arguments:
-        name (List[str]): The name of the objective. Should be the same as a
+        name (list[str]): The name of the objective. Should be the same as a
                             column name in the data.
         data (pd.DataFrame): The data in a pandas dataframe. The columns
                             should be named after variables/objective.
         evaluator (Union[None, Callable], optional): A python function that
             contains the analytical function or calls the simulator to get the
             true objective value. By default None, as this is not required.
         lower_bound (float, optional): Lower bound of the objective,
                                         by default -np.inf
         upper_bound (float, optional): Upper bound of the objective,
                                         by default np.inf
-        maximize (List[bool], optional): Boolean describing whether the
+        maximize (list[bool], optional): Boolean describing whether the
             objective is to be maximized or not, by default None, which
             defaults to [False], hence minimizes.
 
 
     Raises:
         ObjectiveError:  When the name provided during initialization does not
             match any name in the columns of the data provided during
             initilizaiton.
 
     """
 
     def __init__(
         self,
-        name: List[str],
+        name: list[str],
         data: pd.DataFrame,
-        evaluator: Union[None, Callable] = None,
-        lower_bounds: Union[List[float], np.ndarray] = None,
-        upper_bounds: Union[List[float], np.ndarray] = None,
-        maximize: List[bool] = None,
+        evaluator: None | Callable = None,
+        lower_bounds: list[float] | np.ndarray | None = None,
+        upper_bounds: list[float] | np.ndarray | None = None,
+        maximize: list[bool] | None = None,
     ) -> None:
-
         if all(obj in data.columns for obj in name):
             super().__init__(name, evaluator, lower_bounds, upper_bounds, maximize)
         else:
             msg = f'Name "{name}" not found in the dataframe provided'
             raise ObjectiveError(msg)
         self.X = data.drop(name, axis=1)
         self.y = data[name]
         self.variable_names = self.X.columns
         self._model = dict.fromkeys(name)  # TODO: Make the set of keys immutable?
         self._model_trained = dict.fromkeys(name, False)
 
     def train(
         self,
-        models: Union[BaseRegressor, List[BaseRegressor]],
-        model_parameters: Union[Dict, List[Dict]] = None,
-        index: List[int] = None,
+        models: BaseRegressor | list[BaseRegressor],
+        model_parameters: dict | list[dict] | None = None,
+        index: list[int] | None = None,
         data: pd.DataFrame = None,
     ):
         """Train surrogate models for the objective.
 
         Arguments:
-            model (BaseRegressor or List[BaseRegressors]):
+            model (BaseRegressor or list[BaseRegressors]):
                 A regressor or a list of regressors. The regressor/s, when initialized,
                 should have a fit method and a predict method.
                 The predict method should return the predicted objective
                 value, as well as the uncertainity value, in a tuple. If the regressor does
                 not support calculating uncertainity, return a tuple of objective value and
                 None.
                 If a single regressor is provided, that regressor is used for all the
                 objectives.
                 If a list of regressors is provided, and if the list contains one regressor
                 for each objective, then those individual regressors are used to model the
                 objectives. If the number of regressors is not equal to the number of
                 objectives, an error is raised.
-            model_parameters (Dict or List[Dict]):
+            model_parameters (dict or list[dict]):
                 The parameters for the regressors. Should be a dict if a single regressor is
                 provided. If a list of regressors is provided, the parameters should be in a
                 list of dicts, same length as the list of regressors(= number of objs).
-            index (List[int], optional):
+            index (list[int], optional):
                 Indices of the samples (in self.X and self.y), to be used to train the
                 surrogate model. By default None, which trains the model on the entire
                 dataset. This behaviour may be changed in the future to support test-train
                 split or cross validation.
             data (pd.DataFrame, optional):
                 Extra data to be used for training only. This data is not saved. By default
                 None, which then uses self.X and self.y for training.
@@ -732,39 +727,39 @@
             models = [models] * len(self.name)
             model_parameters = [model_parameters] * len(self.name)
         elif not (len(models) == len(model_parameters) == self.n_of_objectives):
             msg = (
                 "The length of lists of models and parameters should be the same as"
                 "the number of objectives in this objective class"
             )
-        for model, model_params, name in zip(models, model_parameters, self.name):
+        for model, model_params, name in zip(models, model_parameters, self.name, strict=True):
             self._train_one_objective(name, model, model_params, index, data)
 
     def _train_one_objective(
         self,
         name: str,
         model: BaseRegressor,
-        model_parameters: Dict,
-        index: List[int] = None,
+        model_parameters: dict,
+        index: list[int] | None = None,
         data: pd.DataFrame = None,
     ):
         """Train surrogate model for the objective.
 
         Arguments:
             name (str): Name of the objective for which you want to train the
                         surrogate model
             model (BaseRegressor): A regressor. The regressor, when
                     initialized, should have a fit method and a predict method.
                     The predict method should return the predicted objective
                     value, as well as the uncertainity value, in a tuple. If
                     the regressor does not support calculating uncertainity,
                     return a tuple of objective value and None.
-            model_parameters (Dict): **model_parameters is passed to the model
+            model_parameters (dict): **model_parameters is passed to the model
                                     when initialized.
-            index (List[int], optional): Indices of the samples (in self.X and
+            index (list[int], optional): Indices of the samples (in self.X and
                     self.y), to be used to train the surrogate model. By
                     default None, which trains the model on the entire dataset.
                     This behaviour may be changed in the future to support
                     test-train split or cross validation.
             data (pd.DataFrame, optional): Extra data to be used for training
                     only. This data is not saved. By default None, which then
                     uses self.X and self.y for training.
@@ -816,15 +811,15 @@
         result = pd.DataFrame(index=range(decision_vector.shape[0]), columns=self.name)
         uncertainity = pd.DataFrame(index=range(decision_vector.shape[0]), columns=self.name)
         for name, model in self._model.items():
             try:
                 result[name], uncertainity[name] = model.predict(decision_vector)
             except ModelError:
                 msg = "Bad argument supplied to the model"
-                raise ObjectiveError(msg)
+                raise ObjectiveError(msg) from ModelError
         return ObjectiveEvaluationResults(result, uncertainity)
 
     def _func_evaluate(self, decision_vector: np.ndarray) -> ObjectiveEvaluationResults:
         """Evaluate the values with analytical function.
 
         Arguments:
             decision_vector (np.ndarray): Variable values where evaluation is
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/problem/Problem.py` & `desdeo_problem-1.6.0/desdeo_problem/problem/Problem.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,105 +9,104 @@
     MOProblem
     DataProblem
     ExperimentalProblem
     IOPISProblem
     DiscreteDataProblem
 """
 from abc import ABC, abstractmethod
+from collections.abc import Callable
 
-# , TypedDict coming in py3.8
 from functools import reduce
 from operator import iadd
-from typing import Callable, Dict, List, NamedTuple, Optional, Tuple, Union
+from typing import NamedTuple
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 
 from desdeo_problem.problem.Constraint import ScalarConstraint
 from desdeo_problem.problem.Objective import (
+    ScalarDataObjective,
+    ScalarObjective,
     VectorDataObjective,
     VectorObjective,
     _ScalarDataObjective,
     _ScalarObjective,
-    ScalarObjective,
-    ScalarDataObjective,
 )
-from desdeo_problem.surrogatemodels.SurrogateModels import BaseRegressor
 from desdeo_problem.problem.Variable import Variable
+from desdeo_problem.surrogatemodels.SurrogateModels import BaseRegressor
+from enum import Enum
 
 
 class ProblemError(Exception):
-    """Raised when an error related to the Problem class is encountered.
-
-    """
+    """Raised when an error related to the Problem class is encountered."""
 
 
 # TODO consider replacing namedtuple with attr.s for validation purposes.
 
 
 class EvaluationResults(NamedTuple):
     """The return object of <problem>.evaluate methods.
 
     Attributes:
         objectives (np.ndarray): The objective function values for each input
             vector.
-        fitness (np.ndarray): Equal to objective values if objective is to be
+        targets (np.ndarray): Equal to objective values if objective is to be
             minimized. Multiplied by (-1) if objective to be maximized.
         constraints (Union[None, np.ndarray]): The constraint values of the
             problem corresponding each input vector.
         uncertainity (Union[None, np.ndarray]): The uncertainity in the
             objective values.
 
     """
 
     objectives: np.ndarray
-    fitness: np.ndarray
-    constraints: Union[None, np.ndarray] = None
-    uncertainity: Union[None, np.ndarray] = None
+    targets: np.ndarray
+    constraints: None | np.ndarray = None
+    uncertainity: None | np.ndarray = None
 
     def __str__(self):
         """Textual output of attributes.
 
         Returns:
             str: The textual output of attributes
         """
         prnt_msg = (
             "Evaluation Results Object \n"
             f"Objective values are: \n{self.objectives}\n"
             f"Constraint violation values are: \n{self.constraints}\n"
-            f"Fitness values are: \n{self.fitness}\n"
+            f"Target values are: \n{self.targets}\n"
             f"Uncertainity values are: \n{self.uncertainity}\n"
         )
         return prnt_msg
 
 
 class ProblemBase(ABC):
     """The base class for the problems.
 
     All other problem classes should be derived from this.
 
     Attributes:
         nadir (np.ndarray): Nadir values for the problem, initiated = None
         ideal (np.ndarray): Ideal values for the problem, initiated = None
-        nadir_fitness (np.ndarray): Fitness values for nadir, initiated = None
-        ideal_fitness (np.ndarray): Fitness values for ideal, initiated = None
+        nadir_targets (np.ndarray): Target values for nadir, initiated = None
+        ideal_targets (np.ndarray): Target values for ideal, initiated = None
         __n_of_objectives (int): Number of objectives, initiated = 0
         __n_of_variables (int): Number of variables, initiated = 0
         __decision_vectors (np.ndarray): Array of decision variable vectors,
                                             initiated = None
         __objective_vectors (np.ndarray): Array of objective variable vectors,
                                             initiated = None
     """
 
     def __init__(self):
         self.nadir: np.ndarray = None
         self.ideal: np.ndarray = None
-        self.nadir_fitness: np.ndarray = None
-        self.ideal_fitness: np.ndarray = None
+        self.nadir_targets: np.ndarray = None
+        self.ideal_targets: np.ndarray = None
         self.__n_of_objectives: int = 0
         self.__n_of_variables: int = 0
         self.__decision_vectors: np.ndarray = None
         self.__objective_vectors: np.ndarray = None
 
     @property
     def n_of_objectives(self) -> int:
@@ -160,53 +159,50 @@
 
         Arguments:
             val (np.ndarray): the decision vector array
         """
         self.__decision_vectors = val
 
     @abstractmethod
-    def get_variable_bounds(self) -> Union[None, np.ndarray]:
+    def get_variable_bounds(self) -> None | np.ndarray:
         """Abstract method to get variable bounds"""
-        pass
 
     @abstractmethod
-    def evaluate(
-        self, decision_vectors: np.ndarray, use_surrogate: bool = False
-    ) -> EvaluationResults:
+    def evaluate(self, decision_vectors: np.ndarray, use_surrogate: bool = False) -> EvaluationResults:
         """Abstract method to evaluate problem.
-                                                                   
+
         Evaluates the problem using an ensemble of input vectors. Uses
         surrogate models if available. Otherwise, it uses the true evaluator.
 
         Arguments:
             decision_vectors (np.ndarray): An array of decision variable
             input vectors.
             use_surrogate (bool): A bool to control whether to use the true, potentially
             expensive function or a surrogate model to evaluate the objectives.
 
         Returns:
-            (Dict): Dict with the following keys:
+            (dict): dict with the following keys:
                 'objectives' (np.ndarray): The objective function values for each input
                     vector.
                 'constraints' (Union[np.ndarray, None]): The constraint values of the
                     problem corresponding each input vector.
-                'fitness' (np.ndarray): Equal to objective values if objective is to be
+                'targets' (np.ndarray): Equal to objective values if objective is to be
                     minimized. Multiplied by (-1) if objective to be maximized.
                 'uncertainity' (Union[np.ndarray, None]): The uncertainity in the
                     objective values.
 
         """
 
     @abstractmethod
-    def evaluate_constraint_values(self) -> Optional[np.ndarray]:
+    def evaluate_constraint_values(self) -> np.ndarray | None:
         """Abstract method to evaluate constraint values.
 
         Evaluate just the constraint function values using the attributes
         decision_vectors and objective_vectors
-        
+
         Note:
             Currently not supported by ScalarMOProblem
 
         """
 
 
 # TODO: Depreciate. Use MO problem in the future
@@ -215,90 +211,84 @@
 
     To be depreciated.
 
     A multiobjective optimization problem with user defined objective
     functions, constraints and variables.
     The objectives each return a single scalar.
 
-    Arguments:   
-        objectives (List[ScalarObjective]): A list containing the objectives of
+    Arguments:
+        objectives (list[ScalarObjective]): A list containing the objectives of
             the problem.
-        variables (List[Variable]): A list containing the variables of the
+        variables (list[Variable]): A list containing the variables of the
             problem.
-        constraints (List[ScalarConstraint]): A list containing the
+        constraints (list[ScalarConstraint]): A list containing the
             constraints of the problem. If no constraints exist, None may
             be supllied as the value.
         nadir (Optional[np.ndarray]): The nadir point of the problem.
         ideal (Optional[np.ndarray]): The ideal point of the problem.
 
     Attributes:
         __n_of_objectives (int): The number of objectives in the problem.
         __n_of_variables (int): The number of variables in the problem.
         __n_of_constraints (int): The number of constraints in the problem.
         __nadir (np.ndarray): The nadir point of the problem.
         __ideal (np.ndarray): The ideal point of the problem.
-        __objectives (List[ScalarObjective]): A list containing the objectives of
+        __objectives (list[ScalarObjective]): A list containing the objectives of
             the problem.
-        __constraints (List[ScalarConstraint]): A list conatining the constraints
+        __constraints (list[ScalarConstraint]): A list conatining the constraints
             of the problem.
 
     Raises:
         ProblemError: Ill formed nadir and/or ideal vectors are supplied.
 
     """
 
     def __init__(
         self,
-        objectives: List[ScalarObjective],
-        variables: List[Variable],
-        constraints: List[ScalarConstraint],
-        nadir: Optional[np.ndarray] = None,
-        ideal: Optional[np.ndarray] = None,
+        objectives: list[ScalarObjective],
+        variables: list[Variable],
+        constraints: list[ScalarConstraint],
+        nadir: np.ndarray | None = None,
+        ideal: np.ndarray | None = None,
     ) -> None:
         super().__init__()
-        self.__objectives: List[ScalarObjective] = objectives
-        self.__variables: List[Variable] = variables
-        self.__constraints: List[ScalarConstraint] = constraints
+        self.__objectives: list[ScalarObjective] = objectives
+        self.__variables: list[Variable] = variables
+        self.__constraints: list[ScalarConstraint] = constraints
 
         self.__n_of_objectives: int = len(self.objectives)
         self.__n_of_variables: int = len(self.variables)
 
         if self.constraints is not None:
             self.__n_of_constraints: int = len(self.constraints)
         else:
             self.__n_of_constraints = 0
 
         # Nadir vector must be the same size as the number of objectives
-        if nadir is not None:
-            if len(nadir) != self.n_of_objectives:
-                msg = (
-                    "The length of the nadir vector does not match the"
-                    "number of objectives: Length nadir {}, number of "
-                    "objectives {}."
-                ).format(len(nadir), self.n_of_objectives)
-                raise ProblemError(msg)
+        if nadir is not None and len(nadir) != self.n_of_objectives:
+            msg = (
+                f"The length of the nadir vector does not match the"
+                f"number of objectives: Length nadir {len(nadir)}, number of "
+                f"objectives {self.n_of_objectives}."
+            )
+            raise ProblemError(msg)
 
         # Ideal vector must be the same size as the number of objectives
-        if ideal is not None:
-            if len(ideal) != self.n_of_objectives:
-                msg = (
-                    "The length of the ideal vector does not match the"
-                    "number of objectives: Length ideal {}, number of "
-                    "objectives {}."
-                ).format(len(ideal), self.n_of_objectives)
-                raise ProblemError(msg)
+        if ideal is not None and len(ideal) != self.n_of_objectives:
+            msg = (
+                f"The length of the ideal vector does not match the"
+                f"number of objectives: Length ideal {len(ideal)}, number of "
+                f"objectives {self.n_of_objectives}."
+            )
+            raise ProblemError(msg)
 
         # Nadir and ideal vectors must match in size
-        if nadir is not None and ideal is not None:
-            if len(nadir) != len(ideal):
-                msg = (
-                    "The length of the nadir and ideal point don't match:"
-                    " length of nadir {}, length of ideal {}."
-                ).format(len(nadir), len(ideal))
-                raise ProblemError(msg)
+        if nadir is not None and ideal is not None and len(nadir) != len(ideal):
+            msg = f"The length of the nadir ({len(nadir)}) and ideal point ({len(ideal)}) don't match."
+            raise ProblemError(msg)
 
         self.__nadir = nadir
         self.__ideal = ideal
 
         # Multiplier to convert maximization to minimization
         max_multiplier = np.asarray([1, -1])
         to_maximize = [objective.maximize for objective in objectives]
@@ -321,64 +311,64 @@
 
         Arguments:
             int: the number of constraints.
         """
         self.__n_of_constraints = val
 
     @property
-    def objectives(self) -> List[ScalarObjective]:
+    def objectives(self) -> list[ScalarObjective]:
         """Property: the list of objectives.
 
         Returns:
-            List[ScalarObjective]: the list of objectives
+            list[ScalarObjective]: the list of objectives
         """
         return self.__objectives
 
     @objectives.setter
-    def objectives(self, val: List[ScalarObjective]):
+    def objectives(self, val: list[ScalarObjective]):
         """Setter: the list of objectives.
 
         Arguments:
-            val (List[ScalarObjective]): the list of objectives.
+            val (list[ScalarObjective]): the list of objectives.
         """
         self.__objectives = val
 
     @property
-    def variables(self) -> List[Variable]:
+    def variables(self) -> list[Variable]:
         """Property: the list of problem variables.
 
         Returns:
-            List[_ScalarObjective]: the list of problem variables
+            list[_ScalarObjective]: the list of problem variables
         """
         return self.__variables
 
     @variables.setter
-    def variables(self, val: List[Variable]):
+    def variables(self, val: list[Variable]):
         """Setter: the list of variables.
 
         Arguments:
-            val (List[_ScalarObjective]): the list of variables.
+            val (list[_ScalarObjective]): the list of variables.
         """
         self.__variables = val
 
     @property
-    def constraints(self) -> List[ScalarConstraint]:
+    def constraints(self) -> list[ScalarConstraint]:
         """Property: the list of constraints.
 
         Returns:
-            List[_ScalarObjective]: the list of constraints
+            list[_ScalarObjective]: the list of constraints
         """
         return self.__constraints
 
     @constraints.setter
-    def constraints(self, val: List[ScalarConstraint]):
+    def constraints(self, val: list[ScalarConstraint]):
         """Setter: the list of constraints.
 
         Arguments:
-            val (List[_ScalarObjective]): the list of constraints.
+            val (list[_ScalarObjective]): the list of constraints.
         """
         self.__constraints = val
 
     @property
     def n_of_objectives(self) -> int:
         """Property: the number of objectives.
 
@@ -449,15 +439,15 @@
 
         Arguments:
             val (np.ndarray): The ideal point of the problem.
 
         """
         self.__ideal = val
 
-    def get_variable_bounds(self) -> Union[np.ndarray, None]:
+    def get_variable_bounds(self) -> np.ndarray | None:
         """Get the variable bounds.
 
         Return the upper and lower bounds of each decision variable present
         in the problem as a 2D numpy array. The first column corresponds to the
         lower bounds of each variable, and the second column to the upper
         bound.
 
@@ -470,44 +460,44 @@
             bounds = np.ndarray((self.n_of_variables, 2))
             for ind, var in enumerate(self.variables):
                 bounds[ind] = np.array(var.get_bounds())
             return bounds
         else:
             return None
 
-    def get_variable_names(self) -> List[str]:
+    def get_variable_names(self) -> list[str]:
         """Get variable names.
 
         Return the variable names of the variables present in the problem in
         the order they were added.
 
         Returns:
-            List[str]: Names of the variables in the order they were added.
+            list[str]: Names of the variables in the order they were added.
 
         """
         return [var.name for var in self.variables]
 
-    def get_objective_names(self) -> List[str]:
+    def get_objective_names(self) -> list[str]:
         """Get objective names.
 
         Return the names of the objectives present in the problem in the
         order they were added.
 
         Returns:
-            List[str]: Names of the objectives in the order they were added.
+            list[str]: Names of the objectives in the order they were added.
 
         """
         return [obj.name for obj in self.objectives]
 
-    def get_uncertainty_names(self) -> List[str]:
+    def get_uncertainty_names(self) -> list[str]:
         """Return the names of the objectives present in the problem in the
         order they were added.
 
         Returns:
-            List[str]: Names of the objectives in the order they were added.
+            list[str]: Names of the objectives in the order they were added.
 
         """
         return [unc.name for unc in self.objectives]
 
     def get_variable_lower_bounds(self) -> np.ndarray:
         """Get variable lower bounds.
 
@@ -517,95 +507,86 @@
         Returns:
             np.ndarray: An array with the lower bounds of the variables.
         """
         return np.array([var.get_bounds()[0] for var in self.variables])
 
     def get_variable_upper_bounds(self) -> np.ndarray:
         """Get variable upper bounds.
-                                             
+
         Return the upper bounds of each variable as a list. The order of the
         bounds follows the order the variables were added to the problem.
         Returns:
             np.ndarray: An array with the upper bounds of the variables.
         """
         return np.array([var.get_bounds()[1] for var in self.variables])
 
-    def evaluate(
-        self, decision_vectors: np.ndarray, use_surrogate: bool = False
-    ) -> EvaluationResults:
+    def evaluate(self, decision_vectors: np.ndarray, use_surrogate: bool = False) -> EvaluationResults:
         """Evaluates the problem using an ensemble of input vectors.
 
         Arguments:
             decision_vectors (np.ndarray): An 2D array of decision variable
                 input vectors. Each column represent the values of each decision
                 variable.
 
         Returns:
-            Tuple[np.ndarray, Union[None, np.ndarray]]: If constraint are
+            tuple[np.ndarray, Union[None, np.ndarray]]: If constraint are
                 defined, returns the objective vector values and corresponding
                 constraint values. Or, if no constraints are defined, returns just
                 the objective vector values with None as the constraint values.
 
         Raises:
             ProblemError: The decision_vectors have wrong dimensions.
 
         """
         # Reshape decision_vectors with single row to work with the code
         if use_surrogate is True:
             raise NotImplementedError(
-                "Surrogates not yet supported in this class. "
-                "Use the '''DataProblem''' class instead."
+                "Surrogates not yet supported in this class. " "Use the '''DataProblem''' class instead."
             )
         shape = np.shape(decision_vectors)
         if len(shape) == 1:
             decision_vectors = np.reshape(decision_vectors, (1, shape[0]))
 
         (n_rows, n_cols) = np.shape(decision_vectors)
 
         if n_cols != self.n_of_variables:
             msg = (
-                "The length of the input vectors does not match the number "
-                "of variables in the problem: Input vector length {}, "
-                "number of variables {}."
-            ).format(n_cols, self.n_of_variables)
+                f"The length of the input vectors does not match the number "
+                f"of variables in the problem: Input vector length {n_cols}, "
+                f"number of variables {self.n_of_variables}."
+            )
             raise ProblemError(msg)
 
         objective_vectors: np.ndarray = np.ndarray(
             (n_rows, self.n_of_objectives), dtype=float
         )  # ??? Use np.zeros instead of this?
         uncertainity: np.ndarray = np.ndarray(
             (n_rows, self.n_of_objectives), dtype=float
         )  # ??? Use np.zeros instead of this?
         if self.n_of_constraints > 0:
-            constraint_values: np.ndarray = np.ndarray(
-                (n_rows, self.n_of_constraints), dtype=float
-            )
+            constraint_values: np.ndarray = np.ndarray((n_rows, self.n_of_constraints), dtype=float)
         else:
             constraint_values = None
 
         # Calculate the objective values
-        for (col_i, objective) in enumerate(self.objectives):
+        for col_i, objective in enumerate(self.objectives):
             results = objective.evaluate(decision_vectors)
             objective_vectors[:, col_i] = results.objectives
             uncertainity[:, col_i] = results.uncertainity
-        # Calculate fitness, which is always to be minimized
-        fitness = objective_vectors * self._max_multiplier
+        # Calculate targets, which is always to be minimized
+        targets = objective_vectors * self._max_multiplier
 
         # Calculate the constraint values
         if constraint_values is not None:
-            for (col_i, constraint) in enumerate(self.constraints):
-                constraint_values[:, col_i] = np.array(
-                    constraint.evaluate(decision_vectors, objective_vectors)
-                )
+            for col_i, constraint in enumerate(self.constraints):
+                constraint_values[:, col_i] = np.array(constraint.evaluate(decision_vectors, objective_vectors))
 
-        return EvaluationResults(
-            objective_vectors, fitness, constraint_values, uncertainity
-        )
+        return EvaluationResults(objective_vectors, targets, constraint_values, uncertainity)
 
-    def evaluate_constraint_values(self) -> Optional[np.ndarray]:
+    def evaluate_constraint_values(self) -> np.ndarray | None:
         """Evaluate constraint values.
 
         Evaluate just the constraint function values using the attributes
         decision_vectors and objective_vectors
 
         Raises:
             NotImplementedError
@@ -618,15 +599,15 @@
 
 
 # TODO: Depreciate. Use data problem in the future
 class ScalarDataProblem(ProblemBase):
     """A problem class for case where the data is pre-computed.
 
     To be depreciated
-    
+
     Defines a problem with pre-computed data representing a multiobjective
     optimization problem with scalar valued objective functions.
 
     Arguments:
         decision_vectors (np.ndarray): A 2D vector of decision_vectors. Each
             row represents a solution with the value for each decision_vectors
             defined on the columns.
@@ -636,15 +617,15 @@
             columns.
 
     Attributes:
         decision_vectors (np.ndarray): See args
         objective_vectors (np.ndarray): See args
         __epsilon (float): A small floating point number to shift the bounds of
             the variables. See, get_variable_bounds, default value 1e-6
-        __constraints (List[ScalarConstraint]): A list of defined constraints.
+        __constraints (list[ScalarConstraint]): A list of defined constraints.
         nadir (np.ndarray): The nadir point of the problem.
         ideal (np.ndarray): The ideal point of the problem.
         __model_exists (bool): is there a model for this problem
 
     Note:
         It is assumed that the decision_vectors and objectives follow a direct
         one-to-one mapping, i.e., the objective values on the ith row in
@@ -661,33 +642,27 @@
         # epsilon is used when computing the bounds. We don't want to exclude
         # any of the solutions that contain border values.
         # See get_variable_bounds
         self.__epsilon: float = 1e-6
         # Used to indicate if a model has been built to represent the model.
         # Used in the evaluation.
         self.__model_exists: bool = False
-        self.__constraints: List[ScalarConstraint] = []
+        self.__constraints: list[ScalarConstraint] = []
 
         try:
             self.n_of_variables = self.decision_vectors.shape[1]
         except IndexError as e:
-            msg = (
-                "Check the variable dimensions. Is it a 2D array? "
-                "Encountered '{}'".format(str(e))
-            )
-            raise ProblemError(msg)
+            msg = "Check the variable dimensions. Is it a 2D array?"
+            raise ProblemError(msg) from e
 
         try:
             self.n_of_objectives = self.objective_vectors.shape[1]
         except IndexError as e:
-            msg = (
-                "Check the objective dimensions. Is it a 2D array? "
-                "Encountered '{}'".format(str(e))
-            )
-            raise ProblemError(msg)
+            msg = "Check the objective dimensions. Is it a 2D array?"
+            raise ProblemError(msg) from e
 
         self.nadir = np.max(self.objective_vectors, axis=0)
         self.ideal = np.min(self.objective_vectors, axis=0)
 
     @property
     def epsilon(self) -> float:
         """Property: epsilon.
@@ -703,28 +678,28 @@
 
         Argument:
             val (float): epsilon value (for shifting the bounds of variables.)
         """
         self.__epsilon = val
 
     @property
-    def constraints(self) -> List[ScalarConstraint]:
+    def constraints(self) -> list[ScalarConstraint]:
         """Property: Constraints.
 
         Return:
-            List[ScalarConstraint]: list of the defined constraints
+            list[ScalarConstraint]: list of the defined constraints
         """
         return self.__constraints
 
     @constraints.setter
-    def constraints(self, val: List[ScalarConstraint]):
+    def constraints(self, val: list[ScalarConstraint]):
         """Setter: Constraints.
 
         Argument:
-            val (List[ScalarConstraint]): list of the constraints.
+            val (list[ScalarConstraint]): list of the constraints.
         """
         self.__constraints = val
 
     def get_variable_bounds(self):
         """Get the variable bounds.
 
         Returns:
@@ -740,38 +715,34 @@
             (
                 np.min(self.decision_vectors, axis=0) - self.epsilon,
                 np.max(self.decision_vectors, axis=0) + self.epsilon,
             ),
             axis=1,
         )
 
-    def evaluate_constraint_values(self) -> Optional[np.ndarray]:
+    def evaluate_constraint_values(self) -> np.ndarray | None:
         """Evaluate the constraint values.
-        
-        Evaluate the constraint values for each defined constraint. A positive value indicates that a constraint is adhered to, a negative
-        value indicates a violated constraint.
+
+        Evaluate the constraint values for each defined constraint. A positive value indicates that a constraint
+        is adhered to, a negative value indicates a violated constraint.
 
         Returns:
             Optional[np.ndarray]: A 2D array with each row representing the
                 constraint values for different objective vectors. One column for
                 each constraint. If no constraint function are defined, returns
                 None.
 
         """
         if len(self.constraints) == 0:
             return None
 
-        constraint_values = np.zeros(
-            (len(self.objective_vectors), len(self.constraints))
-        )
+        constraint_values = np.zeros((len(self.objective_vectors), len(self.constraints)))
 
         for ind, con in enumerate(self.constraints):
-            constraint_values[:, ind] = con.evaluate(
-                self.decision_vectors, self.objective_vectors
-            )
+            constraint_values[:, ind] = con.evaluate(self.decision_vectors, self.objective_vectors)
 
         return constraint_values
 
     def evaluate(self, decision_vectors: np.ndarray) -> np.ndarray:
         """Evaluate the values of the objectives at the given decision.
 
         Evaluate the values of the objectives corresponding to the decision
@@ -790,17 +761,15 @@
             decision_vectors to the closest decision variable present (using an
             L2 distance) in the problem and returns the corresponsing objective
             vector.
 
         """
         if not self.__model_exists:
             idx = np.unravel_index(
-                np.linalg.norm(
-                    self.decision_vectors - decision_vectors, axis=1
-                ).argmin(),
+                np.linalg.norm(self.decision_vectors - decision_vectors, axis=1).argmin(),
                 self.objective_vectors.shape,
                 order="F",
             )[0]
 
         else:
             msg = "Models not implemented yet for data based problems."
             raise NotImplementedError(msg)
@@ -811,111 +780,105 @@
 class MOProblem(ProblemBase):
     """An user defined multiobjective optimization problem.
 
     A multiobjective optimization problem with user defined objective
     functions, constraints, and variables.
 
     Arguments:
-        objectives (List[Union[ScalarObjective, VectorObjective]]): A list
+        objectives (list[Union[ScalarObjective, VectorObjective]]): A list
                         containing the objectives of the problem.
-        variables (List[Variable]): A list containing the variables of
+        variables (list[Variable]): A list containing the variables of
                         the problem.
-        constraints (List[ScalarConstraint]): A list of the constraints
+        constraints (list[ScalarConstraint]): A list of the constraints
                         of the problem.
         nadir (Optional[np.ndarray], optional): Nadir point of the problem.
                                                 Defaults to None.
         ideal (Optional[np.ndarray], optional): Ideal point of the problem.
                                                 Defaults to None.
     Attributes:
-        __objectives (List[Union[ScalarObjective, VectorObjective]]): A list
+        __objectives (list[Union[ScalarObjective, VectorObjective]]): A list
                         containing the objectives of the problem.
-        __variables (List[Variable]): A list containing the variables of
+        __variables (list[Variable]): A list containing the variables of
                         the problem.
-        __constraints (List[ScalarConstraint]): A list of the constraints
+        __constraints (list[ScalarConstraint]): A list of the constraints
                         of the problem.
         __nadir (Optional[np.ndarray], optional): Nadir point of the problem.
                                                 Defaults to None.
         __ideal (Optional[np.ndarray], optional): Ideal point of the problem.
                                                 Defaults to None.
         __n_of_variables (int): The number of variables
         __n_of_objectives (int): The number of objectives
 
     Raises:
         ProblemError: If ideal or nadir vectors are not the same size as
                 number of objectives.
 
     """
 
-    # TODO: use_surrogate : Union[bool, List[bool]]
+    # TODO: use_surrogate : Union[bool, list[bool]]
     def __init__(
         self,
-        objectives: List[Union[ScalarObjective, VectorObjective]],
-        variables: List[Variable],
-        constraints: List[ScalarConstraint] = None,
-        nadir: Optional[np.ndarray] = None,
-        ideal: Optional[np.ndarray] = None,
+        objectives: list[ScalarObjective | VectorObjective],
+        variables: list[Variable],
+        constraints: list[ScalarConstraint] | None = None,
+        nadir: np.ndarray | None = None,
+        ideal: np.ndarray | None = None,
     ):
         super().__init__()
-        self.__objectives: List[Union[ScalarObjective, VectorObjective]] = objectives
-        self.__variables: List[Variable] = variables
-        self.__constraints: List[ScalarConstraint] = constraints
+        self.__objectives: list[ScalarObjective | VectorObjective] = objectives
+        self.__variables: list[Variable] = variables
+        self.__constraints: list[ScalarConstraint] = constraints
         self.__n_of_variables: int = len(self.variables)
-        self.__n_of_objectives: int = sum(
-            map(self.number_of_objectives, self.__objectives)
-        )
+        self.__n_of_objectives: int = sum(map(self.number_of_objectives, self.__objectives))
         if self.constraints is not None:
             self.__n_of_constraints: int = len(self.constraints)
         else:
             self.__n_of_constraints = 0
 
         # Multiplier to convert maximization to minimization
         max_multiplier = np.asarray([1, -1])
         to_maximize = [objective.maximize for objective in objectives]
         # Does not work
         # to_maximize = sum(to_maximize, [])  # To flatten the list
-        to_maximize = (
-            np.hstack(to_maximize) * 1
-        )  # To flatten list and convert to zeros and ones
+        to_maximize = np.hstack(to_maximize) * 1  # To flatten list and convert to zeros and ones
         # to_maximize = np.asarray(to_maximize) * 1  # Convert to zeros and ones
         self._max_multiplier = max_multiplier[to_maximize]
 
-        self.nadir_fitness = np.full(self.__n_of_objectives, np.inf, dtype=float)
-        self.nadir = self.nadir_fitness * self._max_multiplier
-        self.ideal_fitness = np.full(self.__n_of_objectives, np.inf, dtype=float)
-        self.ideal = self.ideal_fitness * self._max_multiplier
+        self.nadir_targets = np.full(self.__n_of_objectives, np.inf, dtype=float)
+        self.nadir = self.nadir_targets * self._max_multiplier
+        self.ideal_targets = np.full(self.__n_of_objectives, np.inf, dtype=float)
+        self.ideal = self.ideal_targets * self._max_multiplier
 
         # Nadir vector must be the same size as the number of objectives
         if nadir is not None:
             if len(nadir) != self.n_of_objectives:
                 msg = (
-                    "The length of the nadir vector does not match the"
-                    "number of objectives: Length nadir {}, number of "
-                    "objectives {}."
-                ).format(len(nadir), self.n_of_objectives)
+                    f"The length of the nadir vector ({len(nadir)}) does not match the number of objectives "
+                    f"{self.n_of_objectives}."
+                )
                 raise ProblemError(msg)
             self.nadir = nadir
 
         # Ideal vector must be the same size as the number of objectives
         if ideal is not None:
             if len(ideal) != self.n_of_objectives:
                 msg = (
-                    "The length of the ideal vector does not match the"
-                    "number of objectives: Length ideal {}, number of "
-                    "objectives {}."
-                ).format(len(ideal), self.n_of_objectives)
+                    f"The length of the ideal vector ({len(ideal)}) does not match the number of objectives "
+                    f"{self.n_of_objectives}."
+                )
                 raise ProblemError(msg)
             self.ideal = ideal
 
-        self.nadir_fitness = self.nadir * self._max_multiplier
-        self.ideal_fitness = self.ideal * self._max_multiplier
+        self.nadir_targets = self.nadir * self._max_multiplier
+        self.ideal_targets = self.ideal * self._max_multiplier
 
         # Objective and variable names
         self.objective_names = self.get_objective_names()
         self.variable_names = self.get_variable_names()
-        self.fitness_names = self.objective_names
+        self.target_names = self.objective_names
 
     @property
     def n_of_constraints(self) -> int:
         """Property: number of constraints.
 
         Returns:
             int: Number of constraints
@@ -928,64 +891,64 @@
 
         Arguments:
             val (int): number of constraints
         """
         self.__n_of_constraints = val
 
     @property
-    def objectives(self) -> List[ScalarObjective]:
+    def objectives(self) -> list[ScalarObjective]:
         """Property: list of objectives.
 
         Returns:
-            List[ScalarObjective]: list of objectives
+            list[ScalarObjective]: list of objectives
         """
         return self.__objectives
 
     @objectives.setter
-    def objectives(self, val: List[ScalarObjective]):
+    def objectives(self, val: list[ScalarObjective]):
         """Setter: set list of objectives.
 
         Arguments:
-            val (List[ScalarObjective]): List of objectives
+            val (list[ScalarObjective]): list of objectives
         """
         self.__objectives = val
 
     @property
-    def variables(self) -> List[Variable]:
-        """Property: List of variables
+    def variables(self) -> list[Variable]:
+        """Property: list of variables
 
         Returns:
-            List[Variable]: list of variables
+            list[Variable]: list of variables
         """
         return self.__variables
 
     @variables.setter
-    def variables(self, val: List[Variable]):
+    def variables(self, val: list[Variable]):
         """Setter: set list of variables.
 
         Arguments:
-            val (List[Variable]): list of variables
+            val (list[Variable]): list of variables
         """
         self.__variables = val
 
     @property
-    def constraints(self) -> List[ScalarConstraint]:
+    def constraints(self) -> list[ScalarConstraint]:
         """Property: list of constraints.
 
         Returns:
-            List[ScalarConstraint]: list of constraints
+            list[ScalarConstraint]: list of constraints
         """
         return self.__constraints
 
     @constraints.setter
-    def constraints(self, val: List[ScalarConstraint]):
+    def constraints(self, val: list[ScalarConstraint]):
         """Setter: list of constraints.
 
         Arguments:
-            val (List[ScalarConstraint]): list of constraints
+            val (list[ScalarConstraint]): list of constraints
         """
         self.__constraints = val
 
     @property
     def n_of_objectives(self) -> int:
         """Property: number of objectives.
 
@@ -1000,20 +963,20 @@
 
         Arguments:
             val (int): number of objectives
         """
         self.__n_of_objectives = val
 
     @property
-    def n_of_fitnesses(self) -> int:
-        """Property: number of dimensions of the fitness matrix.
+    def n_of_targets(self) -> int:
+        """Property: number of dimensions of the targets matrix.
         May be different than the number of objectives in inherited classes.
 
         Returns:
-            int: number of fitness dimensions.
+            int: number of target dimensions.
         """
         return self.__n_of_objectives
 
     @property
     def n_of_variables(self) -> int:
         """Property: number of variables.
 
@@ -1028,41 +991,37 @@
 
         Arguments:
             val (int): number of variables
         """
         self.__n_of_variables = val
 
     @staticmethod
-    def number_of_objectives(
-        obj_instance: Union[ScalarObjective, VectorObjective]
-    ) -> int:
+    def number_of_objectives(obj_instance: ScalarObjective | VectorObjective) -> int:
         """Return the number of objectives in the given obj_instance.
 
         Arguments:
             obj_instance (Union[ScalarObjective, VectorObjective]): An instance of one of
                 the objective classes
 
         Raises:
             ProblemError: Raised when obj_instance is not an instance of the supported
                 classes
 
         Returns:
             int: Number of objectives in obj_instance
         """
-        if isinstance(obj_instance, _ScalarObjective):
-            return 1
-        elif isinstance(obj_instance, ScalarObjective):
+        if isinstance(obj_instance, _ScalarObjective | ScalarObjective):
             return 1
         elif isinstance(obj_instance, VectorObjective):
             return obj_instance.n_of_objectives
         else:
             msg = "Supported objective types: ScalarObjective and VectorObjective"
             raise ProblemError(msg)
 
-    def get_variable_bounds(self) -> Union[np.ndarray, None]:
+    def get_variable_bounds(self) -> np.ndarray | None:
         """Get variable bounds.
         Return the upper and lower bounds of each decision variable present
         in the problem as a 2D numpy array. The first column corresponds to the
         lower bounds of each variable, and the second column to the upper
         bound.
 
         Returns:
@@ -1074,42 +1033,42 @@
             bounds = np.ndarray((self.n_of_variables, 2))
             for ind, var in enumerate(self.variables):
                 bounds[ind] = np.array(var.get_bounds())
             return bounds
         else:
             return None
 
-    def get_variable_names(self) -> List[str]:
-        """Get variable names.     
+    def get_variable_names(self) -> list[str]:
+        """Get variable names.
         Return the variable names of the variables present in the problem in
         the order they were added.
 
         Returns:
-            List[str]: Names of the variables in the order they were added.
+            list[str]: Names of the variables in the order they were added.
 
         """
         return [var.name for var in self.variables]
 
-    def get_objective_names(self) -> List[str]:
-        """Get objective names.   
+    def get_objective_names(self) -> list[str]:
+        """Get objective names.
         Return the names of the objectives present in the problem in the
         order they were added.
 
         Returns:
-            List[str]: Names of the objectives in the order they were added.
+            list[str]: Names of the objectives in the order they were added.
 
         """
         obj_list = [[(obj.name)] for obj in self.objectives]
         return reduce(iadd, obj_list, [])
 
     # TODO: add  get_uncertainty_names() for uncertainty values
 
     def get_variable_lower_bounds(self) -> np.ndarray:
         """Get variable lower bounds.
-        
+
         Return the lower bounds of each variable as a list. The order of the bounds
         follows the order the variables were added to the problem.
 
         Returns:
             np.ndarray: An array with the lower bounds of the variables.
         """
         return np.array([var.get_bounds()[0] for var in self.variables])
@@ -1121,28 +1080,26 @@
         follows the order the variables were added to the problem.
 
         Returns:
             np.ndarray: An array with the upper bounds of the variables.
         """
         return np.array([var.get_bounds()[1] for var in self.variables])
 
-    def evaluate(
-        self, decision_vectors: np.ndarray, use_surrogate: bool = False
-    ) -> EvaluationResults:
+    def evaluate(self, decision_vectors: np.ndarray, use_surrogate: bool = False) -> EvaluationResults:
         """Evaluates the problem using an ensemble of input vectors.
 
         Arguments:
             decision_vectors (np.ndarray): An 2D array of decision variable
                 input vectors. Each column represent the values of each decision
                 variable.
             use_surrogate (bool): A bool to control whether to use the true, potentially
                 expensive function or a surrogate model to evaluate the objectives.
 
         Returns:
-            Tuple[np.ndarray, Union[None, np.ndarray]]: If constraint are
+            tuple[np.ndarray, Union[None, np.ndarray]]: If constraint are
             defined, returns the objective vector values and corresponding
             constraint values. Or, if no constraints are defined, returns just
             the objective vector values with None as the constraint values.
 
         Raises:
             ProblemError: The decision_vectors have wrong dimensions.
             ValueError: If decision_vectors violate the lower or upper bounds.
@@ -1151,98 +1108,82 @@
         # Reshape decision_vectors with single row to work with the code
         shape = np.shape(decision_vectors)
         if len(shape) == 1:
             decision_vectors = np.reshape(decision_vectors, (1, shape[0]))
 
         # Checking bounds; warn if bounds are breached.
         if np.any(self.get_variable_lower_bounds() > decision_vectors):
-            warn("Some decision variable values violate lower bounds")
+            warn("Some decision variable values violate lower bounds")  # NOQA: B028
         if np.any(self.get_variable_upper_bounds() < decision_vectors):
-            warn("Some decision variable values violate upper bounds")
+            warn("Some decision variable values violate upper bounds")  # NOQA: B028
 
         (n_rows, n_cols) = np.shape(decision_vectors)
 
         if n_cols != self.n_of_variables:
             msg = (
-                "The length of the input vectors does not match the number "
-                "of variables in the problem: Input vector length {}, "
-                "number of variables {}."
-            ).format(n_cols, self.n_of_variables)
+                f"The length of the input vectors does not match the number "
+                f"of variables in the problem: Input vector length {n_cols}, "
+                f"number of variables {self.n_of_variables}."
+            )
             raise ProblemError(msg)
 
-        objective_vectors, uncertainity = self.evaluate_objectives(
-            decision_vectors, use_surrogate=use_surrogate
-        )
+        objective_vectors, uncertainity = self.evaluate_objectives(decision_vectors, use_surrogate=use_surrogate)
 
-        constraint_values = self.evaluate_constraint_values(
-            decision_vectors, objective_vectors
-        )
+        constraint_values = self.evaluate_constraint_values(decision_vectors, objective_vectors)
 
-        # Calculate fitness, which is always to be minimized
-        fitness = self.evaluate_fitness(objective_vectors)
+        # Calculate targets, which is always to be minimized
+        targets = self.evaluate_targets(objective_vectors)
 
         # Update ideal values
-        self.update_ideal(objective_vectors, fitness)
+        self.update_ideal(objective_vectors, targets)
 
-        return EvaluationResults(
-            objective_vectors, fitness, constraint_values, uncertainity
-        )
+        return EvaluationResults(objective_vectors, targets, constraint_values, uncertainity)
 
-    def evaluate_objectives(
-        self, decision_vectors: np.ndarray, use_surrogate: bool = False
-    ) -> Tuple[np.ndarray]:
+    def evaluate_objectives(self, decision_vectors: np.ndarray, use_surrogate: bool = False) -> tuple[np.ndarray]:
         """Evaluate objective values of the problem
 
         Arguments:
            decision_vectors (np.ndarray): An 2D array of decision variable
                 input vectors. Each column represent the values of each
                 decision variable.
            use_surrogate (bool): A bool to control whether to use the true,
                 potentially expensive function or a surrogate model to
                 evaluate the objectives.
 
         Returns:
-            Tuple[np.ndarray]: Objective vector values with their uncertainty.
+            tuple[np.ndarray]: Objective vector values with their uncertainty.
 
         """
         (n_rows, n_cols) = np.shape(decision_vectors)
-        objective_vectors: np.ndarray = np.ndarray(
-            (n_rows, self.n_of_objectives), dtype=float
-        )
+        objective_vectors: np.ndarray = np.ndarray((n_rows, self.n_of_objectives), dtype=float)
 
-        uncertainity: np.ndarray = np.ndarray(
-            (n_rows, self.n_of_objectives), dtype=float
-        )
+        uncertainity: np.ndarray = np.ndarray((n_rows, self.n_of_objectives), dtype=float)
 
         obj_column = 0
         for objective in self.objectives:
             elem_in_curr_obj = self.number_of_objectives(objective)
 
             if elem_in_curr_obj == 1:
                 results = objective.evaluate(decision_vectors, use_surrogate)
                 objective_vectors[:, obj_column] = results.objectives
                 uncertainity[:, obj_column] = results.uncertainity
             elif elem_in_curr_obj > 1:
                 # results = list(map(objective.evaluate, decision_vectors))
                 results = objective.evaluate(decision_vectors, use_surrogate)
 
-                objective_vectors[
-                    :, obj_column : obj_column + elem_in_curr_obj
-                ] = results.objectives
-
-                uncertainity[
-                    :, obj_column : obj_column + elem_in_curr_obj
-                ] = results.uncertainity
+                objective_vectors[:, obj_column : obj_column + elem_in_curr_obj] = results.objectives
+
+                uncertainity[:, obj_column : obj_column + elem_in_curr_obj] = results.uncertainity
 
             obj_column = obj_column + elem_in_curr_obj
         return (objective_vectors, uncertainity)
 
     def evaluate_constraint_values(
         self, decision_vectors: np.ndarray, objective_vectors: np.ndarray
-    ) -> Optional[np.ndarray]:
+    ) -> np.ndarray | None:
         """Evaluate constraint values
 
         Evaluate just the constraint function values using the attributes
         decision_vectors and objective_vectors
 
         Arguments:
             decision_vectors (np.ndarray): An 2D array of decision variable
@@ -1261,89 +1202,85 @@
         Note:
             Currently not supported by ScalarMOProblem
 
         """
         if self.n_of_constraints == 0:
             return None
         (n_rows, n_cols) = np.shape(decision_vectors)
-        constraint_values: np.ndarray = np.ndarray(
-            (n_rows, self.n_of_constraints), dtype=float
-        )
+        constraint_values: np.ndarray = np.ndarray((n_rows, self.n_of_constraints), dtype=float)
 
-        for (col_i, constraint) in enumerate(self.constraints):
-            constraint_values[:, col_i] = np.array(
-                constraint.evaluate(decision_vectors, objective_vectors)
-            )
+        for col_i, constraint in enumerate(self.constraints):
+            constraint_values[:, col_i] = np.array(constraint.evaluate(decision_vectors, objective_vectors))
         return constraint_values
 
-    def evaluate_fitness(self, objective_vectors: np.ndarray) -> np.ndarray:
-        """Evaluate fitness of the objectives.
+    def evaluate_targets(self, objective_vectors: np.ndarray) -> np.ndarray:
+        """Evaluate targets of the objectives.
 
         Arguments:
             objective_vectors (np.ndarray): objective vector array
 
         Returns:
-            np.ndarray: fitness of each objective vector
+            np.ndarray: targets of each objective vector
 
         """
         return objective_vectors * self._max_multiplier
 
-    def update_ideal(self, objective_vectors: np.ndarray, fitness: np.ndarray):
+    def update_ideal(self, objective_vectors: np.ndarray, targets: np.ndarray):
         """Update the ideal vector
 
         Arguments:
             objective_vectors (np.ndarray): Objective vectors
-            fitness (np.ndarray): fittness of objective vectors.
+            targets (np.ndarray): fittness of objective vectors.
 
         """
-        self.ideal_fitness = np.amin(np.vstack((self.ideal_fitness, fitness)), axis=0)
-        self.ideal = self.ideal_fitness * self._max_multiplier
+        self.ideal_targets = np.amin(np.vstack((self.ideal_targets, targets)), axis=0)
+        self.ideal = self.ideal_targets * self._max_multiplier
 
 
 # TODO: Make this the "main" Problem class?
 class DataProblem(MOProblem):
     """A class for a data based problem.
 
     A problem class for data-based problem. This supports surrogate modelling.
     Data should be given in the form of a pandas dataframe.
-    
+
     Arguments:
         data (pd.DataFrame): The input data. This will be used for training the model.
-        variable_names (List[str]): Names of the variables in the dataframe provided.
-        objective_names (List[str]): Names of the objectices in the dataframe provided.
+        variable_names (list[str]): Names of the variables in the dataframe provided.
+        objective_names (list[str]): Names of the objectices in the dataframe provided.
         bounds (pd.DataFrame, optional): A pandas DataFrame containing the upper and
             lower bounds of the decision variables. Column names have to be same as
             variable_names. Row names have to be "lower_bound" and "upper_bound".
-        objectives (List[Union[ScalarDataObjective,VectorDataObjective,]], optional):
+        objectives (list[Union[ScalarDataObjective,VectorDataObjective,]], optional):
             Objective instances, currently not supported. Defaults to None.
-        variables (List[Variable], optional): Variable instances. Defaults to None.
+        variables (list[Variable], optional): Variable instances. Defaults to None.
             Currently not supported.
-        constraints (List[ScalarConstraint], optional): Constraint instances.
+        constraints (list[ScalarConstraint], optional): Constraint instances.
             Defaults to None, which means that there are no constraints.
         nadir (Optional[np.ndarray], optional): Nadir of the problem. Defaults to None.
         ideal (Optional[np.ndarray], optional): Ideal of the problem. Defaults to None.
     Raises:
         ProblemError: When input data is not a dataframe.
         ProblemError: When given objective or variable names are not in dataframe column
         NotImplementedError: When objective instances are passed
         NotImplementedError: When variable instances are passed
     """
 
     def __init__(
         self,
         data: pd.DataFrame,
-        variable_names: List[str],
-        objective_names: List[str],
+        variable_names: list[str],
+        objective_names: list[str],
         bounds: pd.DataFrame = None,
         maximize: pd.DataFrame = None,
-        objectives: List[Union[ScalarDataObjective, VectorDataObjective]] = None,
-        variables: List[Variable] = None,
-        constraints: List[ScalarConstraint] = None,
-        nadir: Optional[np.ndarray] = None,
-        ideal: Optional[np.ndarray] = None,
+        objectives: list[ScalarDataObjective | VectorDataObjective] | None = None,
+        variables: list[Variable] | None = None,
+        constraints: list[ScalarConstraint] | None = None,
+        nadir: np.ndarray | None = None,
+        ideal: np.ndarray | None = None,
     ):
         if not isinstance(data, pd.DataFrame):
             msg = "Please provide data in the pandas dataframe format"
             raise ProblemError(msg)
         if not all(obj in data.columns for obj in objective_names):
             msg = "Provided objective names not found in provided dataframe columns"
             raise ProblemError(msg)
@@ -1352,17 +1289,15 @@
             raise ProblemError(msg)
         if bounds is not None:
             if not all(var in variable_names for var in bounds.columns):
                 msg = "A mismatch in the variable names in the bounds dataframe"
                 raise ProblemError(msg)
             bounds_row_names = ["lower_bound", "upper_bound"]
             if not all(row_name in bounds_row_names for row_name in bounds.index):
-                msg = (
-                    f"'bounds' should contain the following indices: {bounds_row_names}"
-                )
+                msg = f"'bounds' should contain the following indices: {bounds_row_names}"
                 raise ProblemError(msg)
         if maximize is not None:
             if not all(obj in objective_names for obj in maximize.columns):
                 msg = "maximize DataFrame should only contain objectives"
                 raise ProblemError(msg)
             if not all(obj in maximize.columns for obj in objective_names):
                 msg = "All objectives should be in the maximize DataFrame"
@@ -1378,110 +1313,98 @@
         if variables is not None:
             msg = "Support for custom variables objects not implemented yet"
             raise NotImplementedError(msg)
         if objectives is None:
             objectives = []
             for obj in objective_names:
                 objectives.append(
-                    ScalarDataObjective(
-                        data=data[variable_names + [obj]],
-                        name=obj,
-                        maximize=maximize[obj].tolist(),
-                    )
+                    ScalarDataObjective(data=data[*variable_names, obj], name=obj, maximize=maximize[obj].tolist())
                 )
         if variables is None:
             variables = []
             for var in variable_names:
                 initial_value = data[var].mean(axis=0)
                 if bounds is None:
                     lower_bound = data[var].min(axis=0)
                     upper_bound = data[var].max(axis=0)
                 else:
                     lower_bound = bounds[var]["lower_bound"]
                     upper_bound = bounds[var]["upper_bound"]
                 variables.append(
-                    Variable(
-                        name=var,
-                        initial_value=initial_value,
-                        lower_bound=lower_bound,
-                        upper_bound=upper_bound,
-                    )
+                    Variable(name=var, initial_value=initial_value, lower_bound=lower_bound, upper_bound=upper_bound)
                 )
         super().__init__(objectives, variables, constraints)
 
     def train(
         self,
-        models: Union[BaseRegressor, List[BaseRegressor]],
-        model_parameters: Union[Dict, List[Dict]] = None,
-        index: List[int] = None,
+        models: BaseRegressor | list[BaseRegressor],
+        model_parameters: dict | list[dict] | None = None,
+        index: list[int] | None = None,
         data: pd.DataFrame = None,
     ):
         """Train surrogate models for all the objectives.
 
         The models should have a fit method and a predict method. The predict method
         should return predicted values as well as uncertainity value (even if they are
         none.)
 
         Arguments:
-            models (Union[BaseRegressor, List[BaseRegressor]]): The class for the
+            models (Union[BaseRegressor, list[BaseRegressor]]): The class for the
                 surrogate modelling algorithm.
-            models_parameters: Dict or List[Dict]
+            models_parameters: dict or list[dict]
                 The parameters for the regressors. Should be a dict if a single regressor is
                 provided. If a list of regressors is provided, the parameters should be in a
                 list of dicts, same length as the list of regressors(= number of objs).
-            index (List[int], optional): The indices of the samples to be used for
+            index (list[int], optional): The indices of the samples to be used for
                 training the surrogate model. If no values are proveded, all samples are
                 used.
             data (pd.DataFrame, optional): Use this argument if some external data is
                 to be used for training. Defaults to None.
 
         Raises:
             ProblemError: If VectorDataObjective is used as one of the objective
             instances. They are not supported yet.
         """
         if not isinstance(models, list):
             models = [models] * len(self.get_objective_names())
             model_parameters = [model_parameters] * len(self.get_objective_names())
         elif len(models) == 1:
             models = models * len(self.get_objective_names())
-        for model, model_params, name in zip(
-            models, model_parameters, self.get_objective_names()
-        ):
+        for model, model_params, name in zip(models, model_parameters, self.get_objective_names(), strict=True):
             self.train_one_objective(name, model, model_params, index, data)
 
     def train_one_objective(
         self,
         name: str,
         model: BaseRegressor,
-        model_parameters: Dict,
-        index: List[int] = None,
+        model_parameters: dict,
+        index: list[int] | None = None,
         data: pd.DataFrame = None,
     ):
         """Train one objective at a time, otherwise same is the train method.
 
         Arguments:
             name (str): Name of the objective to be trained.
             model (BaseRegressor): The class for the surrogate modelling algorithm.
-            model_parameters (Dict): **model_parameters is passed to the model when
+            model_parameters (dict): **model_parameters is passed to the model when
                 initialized.
-            index (List[int], optional): The indices of the samples to be used for
+            index (list[int], optional): The indices of the samples to be used for
                 training the surrogate model. If no values are proveded, all samples are
                 used.
             data (pd.DataFrame, optional): Use this argument if some external data is
                 to be used for training. Defaults to None.
 
         Raises:
             ProblemError: If name is not in the list of objective names.
             ProblemError: If VectorDataObjective is used as one of the objective
                 instances. They are not supported yet.
         """
         if name not in self.get_objective_names():
             raise ProblemError(
-                f'"{name}" not found in the list of'
-                f"original objective names: {self.get_objective_names()}"
+                f'"{name}" not found in the list of' f"original objective names: {self.get_objective_names()}"
             )
         obj_index = self.get_objective_names().index(name)
         if isinstance(self.objectives[obj_index], _ScalarDataObjective):
             self.objectives[obj_index].train(model, model_parameters, index, data)
         if isinstance(self.objectives[obj_index], ScalarDataObjective):
             self.objectives[obj_index].train(model, model_parameters, index, data)
         else:
@@ -1490,207 +1413,238 @@
 
 
 class ExperimentalProblem(MOProblem):
     """A problem class for data-based problem. This supports surrogate modelling.
     Data should be given in the form of a pandas dataframe.
     self.archive is created to save the true function evaluations and update the
     surrogate models if needed.
-    self.archive updates whenever a true function evaluation happens.  
-  
+    self.archive updates whenever a true function evaluation happens.
+
     Arguments:
         data (pd.DataFrame): The input data. This will be used for training the model.
-        variable_names (List[str]): Names of the variables in the dataframe provided.
-        objective_names (List[str]): Names of the objectices in the dataframe provided.
-        objectives (List[Union[ScalarDataObjective,VectorDataObjective,]], optional):
+        variable_names (list[str]): Names of the variables in the dataframe provided.
+        objective_names (list[str]): Names of the objectices in the dataframe provided.
+        objectives (list[Union[ScalarDataObjective,VectorDataObjective,]], optional):
             Objective instances, currently not supported. Defaults to None.
-        variables (List[Variable], optional): Variable instances. Defaults to None.
+        variables (list[Variable], optional): Variable instances. Defaults to None.
             Currently not supported.
-        constraints (List[ScalarConstraint], optional): Constraint instances.
+        constraints (list[ScalarConstraint], optional): Constraint instances.
             Defaults to None, which means that there are no constraints.
         nadir (Optional[np.ndarray], optional): Nadir of the problem. Defaults to None.
         ideal (Optional[np.ndarray], optional): Ideal of the problem. Defaults to None.
-    
+
     Raises:
         ProblemError: When input data is not a dataframe.
         ProblemError: When given objective or variable names are not in dataframe column
         NotImplementedError: When objective instances are passed
         NotImplementedError: When variable instances are passed
 
     Note:
         not properly implemented!
 
     """
 
     def __init__(
         self,
-        variable_names: List[str],
-        objective_names: List[str],
-        uncertainity_names: List[str],
-        evaluators: Union[None, List[Callable]] = None,
-        dimensions_data: pd.DataFrame = None,
+        variable_names: list[str],
+        objective_names: list[str],
+        bounds: pd.DataFrame,
         data: pd.DataFrame = None,
-        objective_functions: List[Tuple[List[str], Callable]] = None,
-        constraints: List[Tuple[List[str], Callable]] = None,
+        maximize: list[bool] | None = None,
+        variable_types: list[str] | None = None,
+        objective_functions: list[Callable] | None = None,
+        constraints: list[Callable] | None = None,
+        # uncertainity_names: list[str],
     ):
         # TODO: add the archiving here for true evaluations.
 
-        self.uncertainity_names = uncertainity_names  #  will be removed later
-        if not isinstance(data, pd.DataFrame):
-            msg = "Please provide data in the pandas dataframe format"
-            raise ProblemError(msg)
-        if not all(obj in data.columns for obj in objective_names):
-            msg = "Provided objective names not found in provided dataframe columns"
-            raise ProblemError(msg)
-        if not all(var in data.columns for var in variable_names):
-            msg = "Provided variable names not found in provided dataframe columns"
-            raise ProblemError(msg)
-        # TODO: Implement the rest
+        if maximize is None:
+            maximize = [False] * len(objective_names)
+        elif (not isinstance(maximize, list)) or (len(maximize) != len(objective_names)):
+            raise ProblemError("maximize should be a list of bools of the same length as objective_names")
+
+        if variable_types is None:
+            variable_types = ["RealNumber"] * len(variable_names)
+
+        # First bool = obj functions are provided.
+        # Second bool = Data is provided.
+        class AllowedStates(Enum):
+            ANALYTICAL = True, False
+            OFFLINE = False, True
+            ONLINE = True, True
+
+        match (objective_functions is not None, data is not None):
+            case AllowedStates.ANALYTICAL:
+                self.conductAnalyticalChecks()
+            case AllowedStates.OFFLINE:
+                self.conductOfflineChecks(data, objective_names, variable_names, bounds)
+            case AllowedStates.ONLINE:
+                self.conductAnalyticalChecks()
+                self.conductOfflineChecks(data, objective_names, variable_names, bounds)
+            case _:
+                raise ProblemError("Invalid combination of inputs. You must either provide data or evaluators.")
+
         objectives = []
-        self.archive = (
-            data
-        )  # this is for model management to archive the solutions and decision variables
-        # check if evaluator is NOne in that case make a list of nones and the lenght of the list is the same as obj_names
+        self.archive = data  # this is for model management to archive the solutions and decision variables
+        # check if evaluator is NOne in that case make a list of nones and the lenght of the list is
+        # the same as obj_names
         # check if evaluator is the same lenght as obj_names if not rais a problem error
-        for obj, evaluator in zip(objective_names, evaluators):
-            objectives.append(
-                ScalarDataObjective(
-                    data=data[variable_names + [obj]], name=obj, evaluator=evaluator
-                )
-            )
+        for obj, func in zip(objective_names, objective_functions, strict=True):  # TODO: Allow Vector objectives
+            objectives.append(ScalarDataObjective(data=data[*variable_names, obj], name=obj, evaluator=func))
 
         variables = []
         for var in variable_names:
             initial_value = data[var].mean(axis=0)
             lower_bound = data[var].min(axis=0)
             upper_bound = data[var].max(axis=0)
             variables.append(
-                Variable(
-                    name=var,
-                    initial_value=initial_value,
-                    lower_bound=lower_bound,
-                    upper_bound=upper_bound,
-                )
+                Variable(name=var, initial_value=initial_value, lower_bound=lower_bound, upper_bound=upper_bound)
             )
         super().__init__(objectives, variables, constraints)
 
+    @staticmethod
+    def conductAnalyticalChecks(objective_names, objective_functions):
+        pass
+
+    @staticmethod
+    def conductOfflineChecks(data, objective_names, variable_names, bounds):
+        if not isinstance(data, pd.DataFrame):
+            msg = "Please provide data in the pandas dataframe format"
+            raise ProblemError(msg)
+        if not all(obj in data.columns for obj in objective_names):
+            msg = "Provided objective names not found in provided dataframe columns"
+            raise ProblemError(msg)
+        if not all(var in data.columns for var in variable_names):
+            msg = "Provided variable names not found in provided dataframe columns"
+            raise ProblemError(msg)
+        if bounds is not None:
+            if not all(var in variable_names for var in bounds.columns):
+                msg = "A mismatch in the variable names in the bounds dataframe"
+                raise ProblemError(msg)
+            bounds_row_names = ["lower_bound", "upper_bound"]
+            if not all(row_name in bounds_row_names for row_name in bounds.index):
+                msg = f"'bounds' should contain the following indices: {bounds_row_names}"
+                raise ProblemError(msg)
+        else:
+            if data[variable_names].min() < bounds["lower_bound"]:
+                raise ProblemError("Some decision variable values violate lower bounds")
+            if data[variable_names].max() > bounds["upper_bound"]:
+                raise ProblemError("Some decision variable values violate upper bounds")
+
     def train(
         self,
-        models: Union[BaseRegressor, List[BaseRegressor]],
-        model_parameters: Union[Dict, List[Dict]] = None,
-        index: List[int] = None,
-        data: pd.DataFrame = None,
+        models: BaseRegressor | list[BaseRegressor],
+        model_parameters: dict | list[dict] | None = None,
+        index: list[int] | None = None,
+        data: pd.DataFrame | None = None,
     ):
-        """Train surrogate models for all the objectives. 
-        
-        The models should have a fit method and a predict method. The predict 
+        """Train surrogate models for all the objectives.
+
+        The models should have a fit method and a predict method. The predict
         method should return predicted values as well as uncertainity value
         (even if they are none.)
 
         Arguments:
-            models (Union[BaseRegressor, List[BaseRegressor]]): The class for the
+            models (Union[BaseRegressor, list[BaseRegressor]]): The class for the
                 surrogate modelling algorithm.
-            models_parameters: Dict or List[Dict]
+            models_parameters: dict or list[dict]
                 The parameters for the regressors. Should be a dict if a single regressor is
                 provided. If a list of regressors is provided, the parameters should be in a
                 list of dicts, same length as the list of regressors(= number of objs).
-            index (List[int], optional): The indices of the samples to be used for
+            index (list[int], optional): The indices of the samples to be used for
                 training the surrogate model. If no values are proveded, all samples are
                 used.
             data (pd.DataFrame, optional): Use this argument if some external data is
                 to be used for training. Defaults to None.
 
         Raises:
             ProblemError: If VectorDataObjective is used as one of the objective
                 instances. They are not supported yet.
         """
+        # TODO @light-weaver: data argument is unused
         data = self.archive  # for updating the data after updating the surrogates
         if not isinstance(models, list):
             models = [models] * len(self.get_objective_names())
             model_parameters = [model_parameters] * len(self.get_objective_names())
         elif len(models) == 1:
             models = models * len(self.get_objective_names())
-        for model, model_params, name in zip(
-            models, model_parameters, self.get_objective_names()
-        ):
+        for model, model_params, name in zip(models, model_parameters, self.get_objective_names(), strict=True):
             self.train_one_objective(name, model, model_params, index, data)
 
     def train_one_objective(
         self,
         name: str,
         model: BaseRegressor,
-        model_parameters: Dict,
-        index: List[int] = None,
+        model_parameters: dict,
+        index: list[int] | None = None,
         data: pd.DataFrame = None,
     ):
         """Train one objective at a time, otherwise same is the train method.
 
         Arguments:
             name (str): Name of the objective to be trained.
             model (BaseRegressor): The class for the surrogate modelling algorithm.
-            model_parameters (Dict): **model_parameters is passed to the model when
+            model_parameters (dict): **model_parameters is passed to the model when
                 initialized.
-            index (List[int], optional): The indices of the samples to be used for
+            index (list[int], optional): The indices of the samples to be used for
                 training the surrogate model. If no values are proveded, all samples are
                 used.
             data (pd.DataFrame, optional): Use this argument if some external data is
                 to be used for training. Defaults to None.
 
         Raises:
             ProblemError: If name is not in the list of objective names.
             ProblemError: If VectorDataObjective is used as one of the objective
                 instances. They are not supported yet.
         """
         if name not in self.get_objective_names():
             raise ProblemError(
-                f'"{name}" not found in the list of'
-                f"original objective names: {self.get_objective_names()}"
+                f'"{name}" not found in the list of' f"original objective names: {self.get_objective_names()}"
             )
         obj_index = self.get_objective_names().index(name)
-        if isinstance(self.objectives[obj_index], _ScalarDataObjective):
-            self.objectives[obj_index].train(model, model_parameters, index, data)
-        elif isinstance(self.objectives[obj_index], ScalarDataObjective):
+        if isinstance(self.objectives[obj_index], _ScalarDataObjective | ScalarDataObjective):
             self.objectives[obj_index].train(model, model_parameters, index, data)
         else:
             msg = "Support for VectorDataObjective not supported yet"
             raise ProblemError(msg)
 
-    def evaluate(
-        self, decision_vectors: np.ndarray, use_surrogate: bool
-    ) -> EvaluationResults:
-
+    def evaluate(self, decision_vectors: np.ndarray, use_surrogate: bool) -> EvaluationResults:
         names = np.hstack((self.variable_names, self.objective_names))
         new_results = super().evaluate(decision_vectors, use_surrogate=use_surrogate)
 
         # The following is for achiving solutions with true function evaluations
-        if use_surrogate == False:
+        if use_surrogate is False:
             new_samples = np.hstack((decision_vectors, new_results.objectives))
             new_data = pd.DataFrame(data=new_samples, columns=names)
             self.archive = self.archive.append(new_data)
         return new_results
 
+    def discrete_solver(self, scalarizer: Callable):
+        fitness = self.da
+
 
 class DiscreteDataProblem:
     """A problem class for data-based problems with discrete values.
 
     These data values are computed representing a set of non-dominated points.
 
     Arguments:
         data (pd.DataFrame): The input data.
-        variable_names (List[str]): Names of the variables in the dataframe provided.
-        objective_names (List[str]): Names of the objectices in the dataframe provided.
+        variable_names (list[str]): Names of the variables in the dataframe provided.
+        objective_names (list[str]): Names of the objectices in the dataframe provided.
         nadir (np.ndarray): Nadir of the problem.
         ideal (np.ndarray): Ideal of the problem.
-    
+
     """
 
     def __init__(
         self,
         data: pd.DataFrame,
-        variable_names: List[str],
-        objective_names: List[str],
+        variable_names: list[str],
+        objective_names: list[str],
         ideal: np.ndarray,
         nadir: np.ndarray,
     ):
         self.decision_variables = data[variable_names].values
         self.variable_names = variable_names
         self.objectives = data[objective_names].values
         self.objective_names = objective_names
@@ -1703,12 +1657,12 @@
 
         Given a vector of decision variables, finds the closest point in
         the given data and returns its index.
         A simple euclidean distance is used.
 
         Arguments:
             x (np.ndarray): A 1D vector containing decision variables.
-        
+
         Returns:
             int: The index of the closest point in the data computed for x.
         """
         return np.argmin(np.linalg.norm(x - self.decision_variables, axis=1))
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/problem/Variable.py` & `desdeo_problem-1.6.0/desdeo_problem/problem/Variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 """Desdeo-problem variable related definitions.
 
 This file includes definition of Variable class (with initial and current
 values and value bounds), variable_builder, and error classes for Variable
 and VariableBuilder.
 """
-
-from os import path
-from typing import List, Tuple, Union
-
 import numpy as np
 
 
 class VariableError(Exception):
     """Raised when an error is encountered during the handling of the
     Variable objects.
 
     """
 
-    pass
-
 
 class VariableBuilderError(Exception):
     """Raised when an error is encountered during the handling of the
     Variable objects.
 
     """
 
-    pass
-
 
 class Variable:
     """Simple variable with a name, initial value and bounds.
 
     Arguments:
         name (str): Name of the variable
         initial_value (float): The initial value of the variable.
@@ -49,35 +41,31 @@
 
     Raises:
         VariableError: Bounds are incorrect.
 
     """
 
     def __init__(
-        self,
-        name: str,
-        initial_value: float,
-        lower_bound: float = -np.inf,
-        upper_bound: float = np.inf,
+        self, name: str, initial_value: float, lower_bound: float = -np.inf, upper_bound: float = np.inf
     ) -> None:
-
         self.__name: str = name
         self.__initial_value: float
         self.__lower_bound: float
         self.__upper_bound: float
         self.__current_value: float  # NOTE: This is probably a useless attr
         # Check that the bounds make sense
         if not (lower_bound < upper_bound):
-            msg = ("Lower bound {} should be less than the upper bound " "{}.").format(lower_bound, upper_bound)
+            msg = f"Lower bound {lower_bound} should be less than the upper bound {upper_bound}."
             raise VariableError(msg)
 
         # Check that the initial value is between the bounds
         if not (lower_bound <= initial_value <= upper_bound):
-            msg = "The initial value {} should be between the " "upper ({}) and lower ({}) bounds.".format(
-                initial_value, lower_bound, upper_bound
+            msg = (
+                f"The initial value {initial_value} should be between"
+                f"the upper ({upper_bound}) and lower ({lower_bound}) bounds."
             )
             raise VariableError(msg)
 
         self.__lower_bound = lower_bound
         self.__upper_bound = upper_bound
         self.__initial_value = initial_value
         self.__current_value = initial_value
@@ -115,31 +103,31 @@
 
         Args:
             float: The updated value for the current_value variable.
 
         """
         self.__current_value = value
 
-    def get_bounds(self) -> Tuple[float, float]:
+    def get_bounds(self) -> tuple[float, float]:
         """Return the bounds of the variables as a tuple.
 
         Returns:
             tuple(float, float): A tuple consisting of (lower_bound,
                 upper_bound)
 
         """
         return (self.__lower_bound, self.__upper_bound)
 
 
 def variable_builder(
-    names: List[str],
-    initial_values: Union[List[float], np.ndarray],
-    lower_bounds: Union[List[float], np.ndarray] = None,
-    upper_bounds: Union[List[float], np.ndarray] = None,
-) -> List[Variable]:
+    names: list[str],
+    initial_values: list[float] | np.ndarray,
+    lower_bounds: list[float] | np.ndarray | None = None,
+    upper_bounds: list[float] | np.ndarray | None = None,
+) -> list[Variable]:
     """Automatically build all variable objects.
 
     Arguments:
         names (List[str]): Names of the variables
         initial_values (np.ndarray): Initial values taken by the variables.
         lower_bounds (Union[List[float], np.ndarray], optional): Lower bounds of the
             variables. If None, it defaults to negative infinity. Defaults to None.
@@ -152,30 +140,32 @@
     Returns:
         List[Variable]: List of variable objects
     """
     # assert that all inputs have the same size
     num_of_variables = len(names)
     if initial_values is None:
         initial_values = [None] * num_of_variables
-    if not (num_of_variables == len(initial_values)):
+    if num_of_variables != len(initial_values):
         msg = (
             "The length of the list of names and the number of elements in the "
             "initial_values array should be the same"
         )
         raise VariableBuilderError(msg)
     if lower_bounds is None:
         lower_bounds = [-np.inf] * num_of_variables
-    if not (num_of_variables == len(lower_bounds)):
+    if num_of_variables != len(lower_bounds):
         msg = (
             "The length of the list of names and the number of elements in the " "lower_bounds array should be the same"
         )
         raise VariableBuilderError(msg)
     if upper_bounds is None:
         upper_bounds = [np.inf] * num_of_variables
-    if not (num_of_variables == len(upper_bounds)):
+    if num_of_variables != len(upper_bounds):
         msg = (
             "The length of the list of names and the number of elements in the " "upper_bounds array should be the same"
         )
         raise VariableBuilderError(msg)
     # if most checks passed
-    variables = [Variable(*var_data) for var_data in zip(names, initial_values, lower_bounds, upper_bounds)]
+    variables = [
+        Variable(*var_data) for var_data in zip(names, initial_values, lower_bounds, upper_bounds, strict=True)
+    ]
     return variables
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/problem/__init__.py` & `desdeo_problem-1.6.0/desdeo_problem/problem/__init__.py`

 * *Files identical despite different names*

### Comparing `desdeo_problem-1.5.0/desdeo_problem/surrogatemodels/SurrogateModels.py` & `desdeo_problem-1.6.0/desdeo_problem/surrogatemodels/SurrogateModels.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from abc import ABC, abstractmethod
-from typing import Tuple
 
 import numpy as np
 from sklearn.gaussian_process import GaussianProcessRegressor as GPR
 
 
 class ModelError(Exception):
-    """Raised when an error related to the surrogate models classes is encountered.
-
-    """
+    """Raised when an error related to the surrogate models classes is encountered."""
 
 
 # TODO: Add more sklearn methods here
 
 
 class BaseRegressor(ABC):
     @abstractmethod
     def fit(self, X: np.ndarray, y: np.ndarray):
         pass
 
     @abstractmethod
-    def predict(self, X: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+    def predict(self, X: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
         pass
 
 
 class GaussianProcessRegressor(GPR, BaseRegressor):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/surrogatemodels/lipschitzian.py` & `desdeo_problem-1.6.0/desdeo_problem/surrogatemodels/lipschitzian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import numpy as np
 import pandas as pd
 
 from desdeo_problem.surrogatemodels.SurrogateModels import BaseRegressor, ModelError
 
 
 class LipschitzianRegressor(BaseRegressor):
-    def __init__(self, L: float = None):
+    def __init__(self, L: float | None = None):
         self.L: float = L
         self.X: np.ndarray = None
         self.y: np.ndarray = None
 
     def fit(self, X, y):
-        if isinstance(X, (pd.DataFrame, pd.Series)):
+        if isinstance(X, pd.DataFrame | pd.Series):
             X = X.values
-        if isinstance(y, (pd.DataFrame, pd.Series)):
+        if isinstance(y, pd.DataFrame | pd.Series):
             y = y.values.reshape(-1, 1)
 
         # Make a 2-D array if needed
         y = np.atleast_1d(y)
         if y.ndim == 1:
             y = y.reshape(-1, 1)
 
@@ -41,23 +41,18 @@
 
     def self_distance(self, arr):
         if arr.ndim == 1:
             dist = np.abs(np.subtract(arr[None, :], arr[:, None]))
         elif arr.ndim == 2:
             dist = np.sum(np.abs(np.subtract(arr[None, :, :], arr[:, None, :])), axis=2)
         else:
-            msg = (
-                f"Array of wrong dimension. Expected dimension = 1 or 2. Recieved "
-                f"dimension = {arr.ndim}"
-            )
+            msg = f"Array of wrong dimension. Expected dimension = 1 or 2. Recieved " f"dimension = {arr.ndim}"
             raise ModelError(msg)
         return dist
 
     def distance(self, array1, array2):
         if array1.ndim == 1:
             array1 = array1.reshape(-1, 1)
         if array2.ndim == 1:
             array2 = array2.reshape(-1, 1)
-        dist = np.sum(
-            np.abs(np.subtract(array1[None, :, :], array2[:, None, :])), axis=2
-        )
+        dist = np.sum(np.abs(np.subtract(array1[None, :, :], array2[:, None, :])), axis=2)
         return dist
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/CarSideImpact.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/CarSideImpact.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,176 +1,172 @@
 """
 Car-side impact problem.
 
 Three-objective problem from:
 
-Jain, H. & Deb, K. (2014). An Evolutionary Many-Objective Optimization Algorithm 
-Using Reference-Point Based Nondominated Sorting Approach, Part II: Handling Constraints 
-and Extending to an Adaptive Approach. IEEE transactions on evolutionary computation, 
-18(4), 602-622. https://doi.org/10.1109/TEVC.2013.2281534 
+Jain, H. & Deb, K. (2014). An Evolutionary Many-Objective Optimization Algorithm
+Using Reference-Point Based Nondominated Sorting Approach, Part II: Handling Constraints
+and Extending to an Adaptive Approach. IEEE transactions on evolutionary computation,
+18(4), 602-622. https://doi.org/10.1109/TEVC.2013.2281534
 
 Optional fourth objective from:
 
-Tanabe, R. & Ishibuchi, H. (2020). An easy-to-use real-world 
-multi-objective optimization problem suite. 
-Applied soft computing, 89, 106078. 
+Tanabe, R. & Ishibuchi, H. (2020). An easy-to-use real-world
+multi-objective optimization problem suite.
+Applied soft computing, 89, 106078.
 https://doi.org/10.1016/j.asoc.2020.106078
 
 Variable names from:
 
-Deb, K., Gupta, S., Daum, D., Branke, J., Mall, A. & Padmanabhan, D. (2009). 
-Reliability-Based Optimization Using Evolutionary Algorithms. 
-IEEE transactions on evolutionary computation, 13(5), 1054-1074. 
-https://doi.org/10.1109/TEVC.2009.2014361 
+Deb, K., Gupta, S., Daum, D., Branke, J., Mall, A. & Padmanabhan, D. (2009).
+Reliability-Based Optimization Using Evolutionary Algorithms.
+IEEE transactions on evolutionary computation, 13(5), 1054-1074.
+https://doi.org/10.1109/TEVC.2009.2014361
 
 """
 
 from desdeo_problem.problem.Variable import Variable
 from desdeo_problem.problem.Objective import ScalarObjective
-from desdeo_problem.problem.Problem import MOProblem, ProblemBase
-from desdeo_problem import ScalarConstraint, problem
+from desdeo_problem.problem.Problem import MOProblem
+from desdeo_problem import ScalarConstraint
 
 import numpy as np
 
-def car_side_impact(three_obj: bool = True, var_iv: np.array = np.array([1, 0.9, 1, 1, 1.75, 0.8, 0.8])) -> MOProblem:
-    """ Car-side impact problem.
-    
+
+def car_side_impact(three_obj: bool = True, var_iv: np.array = (1, 0.9, 1, 1, 1.75, 0.8, 0.8)) -> MOProblem:
+    """Car-side impact problem.
+
     Arguments:
-        three_obj (bool): If true, utilize three objectives version. 
+        three_obj (bool): If true, utilize three objectives version.
             If false, utilize four objectives version. Default is true.
         var_iv (np.array): Optional, initial variable values.
-            Defaults are [1, 0.9, 1, 1, 1.75, 0.8, 0.8]. 
-            x1 ∈ [0.5, 1.5], x2 ∈ [0.45, 1.35], x3 ∈ [0.5, 1.5], 
+            Defaults are [1, 0.9, 1, 1, 1.75, 0.8, 0.8].
+            x1 ∈ [0.5, 1.5], x2 ∈ [0.45, 1.35], x3 ∈ [0.5, 1.5],
             x4 ∈ [0.5, 1.5], x5 ∈ [0.875, 2.625],
             x6 ∈ [0.4, 1.2] and x7 ∈ [0.4, 1.2].
 
     Returns:
         MOProblem: a problem object.
     """
 
     # Check the number of variables
-    if (np.shape(np.atleast_2d(var_iv)[0]) != (7,)):
+    var_iv = np.atleast_2d(var_iv)
+    if np.shape(var_iv[0]) != (7,):
         raise RuntimeError("Number of variables must be seven")
 
     # Lower bounds
     lb = np.array([0.5, 0.45, 0.5, 0.5, 0.875, 0.4, 0.4])
-    
+
     # Upper bounds
     ub = np.array([1.5, 1.35, 1.5, 1.5, 2.625, 1.2, 1.2])
 
     # Check the variable bounds
     if np.any(lb > var_iv) or np.any(ub < var_iv):
         raise ValueError("Initial variable values need to be between lower and upper bounds")
-        
+
     def v_mbp(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            10.58 - 0.674 * x[:, 0] * x[:, 1] - 0.67275 * x[:, 1]
-        )
-    
+        return 10.58 - 0.674 * x[:, 0] * x[:, 1] - 0.67275 * x[:, 1]
+
     def v_fd(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            16.45 - 0.489 * x[:, 2] * x[:, 6] - 0.843 * x[:, 4] * x[:, 5]
-        )
+        return 16.45 - 0.489 * x[:, 2] * x[:, 6] - 0.843 * x[:, 4] * x[:, 5]
 
     # Objective functions
     def f_1(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
         return (
-            1.98 + 4.9 * x[:, 0] + 6.67 * x[:, 1] + 6.98 * x[:, 2] +
-            4.01 * x[:, 3] + 1.78 * x[:, 4] + 10**-5 * x[:, 5] + 2.73 * x[:, 6]
+            1.98
+            + 4.9 * x[:, 0]
+            + 6.67 * x[:, 1]
+            + 6.98 * x[:, 2]
+            + 4.01 * x[:, 3]
+            + 1.78 * x[:, 4]
+            + 10**-5 * x[:, 5]
+            + 2.73 * x[:, 6]
         )
 
     def f_2(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            4.72 - 0.5 * x[:, 3] - 0.19 * x[:, 1] * x[:, 2]
-        )
-    
+        return 4.72 - 0.5 * x[:, 3] - 0.19 * x[:, 1] * x[:, 2]
+
     def f_3(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            0.5 * (v_mbp(x) + v_fd(x))
-        )
+        return 0.5 * (v_mbp(x) + v_fd(x))
 
     # Constrain functions
-    def g_1(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_1(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            1 - 1.16 + 0.3717 * x[:, 1] * x[:, 3] + 0.0092928 * x[:, 2]
-        )
+        return 1 - 1.16 + 0.3717 * x[:, 1] * x[:, 3] + 0.0092928 * x[:, 2]
 
-    def g_2(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_2(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
         return (
-            0.32 - 0.261 + 0.0159 * x[:, 0] * x[:, 1] + 0.06486 * x[:, 0] +
-            0.019 * x[:, 1] * x[:, 6] - 0.0144 * x[:, 2] * x[:, 4] - 0.0154464 * x[:, 5]
+            0.32
+            - 0.261
+            + 0.0159 * x[:, 0] * x[:, 1]
+            + 0.06486 * x[:, 0]
+            + 0.019 * x[:, 1] * x[:, 6]
+            - 0.0144 * x[:, 2] * x[:, 4]
+            - 0.0154464 * x[:, 5]
         )
 
-    def g_3(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_3(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
         return (
-            0.32 - 0.214 - 0.00817 * x[:, 4] + 0.045195 * x[:, 0] + 0.0135168 * x[:, 0] -
-            0.03099 * x[:, 1] * x[:, 5] + 0.018 * x[:, 1] * x[:, 6] -
-            0.007176 * x[:, 2] - 0.023232 * x[:, 2] + 0.00364 * x[:, 4] *
-            x[:, 5] + 0.018 * x[:, 1]**2
+            0.32
+            - 0.214
+            - 0.00817 * x[:, 4]
+            + 0.045195 * x[:, 0]
+            + 0.0135168 * x[:, 0]
+            - 0.03099 * x[:, 1] * x[:, 5]
+            + 0.018 * x[:, 1] * x[:, 6]
+            - 0.007176 * x[:, 2]
+            - 0.023232 * x[:, 2]
+            + 0.00364 * x[:, 4] * x[:, 5]
+            + 0.018 * x[:, 1] ** 2
         )
-            
-    def g_4(x: np.ndarray, _ = None) -> np.ndarray:
+
+    def g_4(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            0.32 - 0.74 + 0.61 * x[:, 1] + 0.031296 * x[:, 2] +
-            0.031872 * x[:, 6] - 0.227 * x[:, 1]**2
-        )
+        return 0.32 - 0.74 + 0.61 * x[:, 1] + 0.031296 * x[:, 2] + 0.031872 * x[:, 6] - 0.227 * x[:, 1] ** 2
 
-    def g_5(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_5(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            32 - 28.98 - 3.818 * x[:, 2] + 4.2 * x[:, 0] * x[:, 1] -
-            1.27296 * x[:, 5] + 2.68065 * x[:, 6]
-        )
+        return 32 - 28.98 - 3.818 * x[:, 2] + 4.2 * x[:, 0] * x[:, 1] - 1.27296 * x[:, 5] + 2.68065 * x[:, 6]
 
-    def g_6(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_6(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            32 - 33.86 - 2.95 * x[:, 2] + 5.057 * x[:, 0] * x[:, 1] +
-            3.795 * x[:, 1] + 3.4431 * x[:, 6] - 1.45728
-        )
+        return 32 - 33.86 - 2.95 * x[:, 2] + 5.057 * x[:, 0] * x[:, 1] + 3.795 * x[:, 1] + 3.4431 * x[:, 6] - 1.45728
 
-    def g_7(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_7(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            32 - 46.36 + 9.9 * x[:, 1] + 4.4505 * x[:, 0]
-        )
+        return 32 - 46.36 + 9.9 * x[:, 1] + 4.4505 * x[:, 0]
 
-    def g_8(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_8(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            4 - f_2(x)
-        )
+        return 4 - f_2(x)
 
-    def g_9(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_9(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            9.9 - v_mbp(x)
-        )
+        return 9.9 - v_mbp(x)
 
-    def g_10(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_10(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            15.7 - v_fd(x)
-        )
+        return 15.7 - v_fd(x)
 
     objective_1 = ScalarObjective(name="minimize the weight of the car", evaluator=f_1, maximize=[False])
-    objective_2 = ScalarObjective(name="minimize the pubic force experienced by a passenger", 
-        evaluator=f_2, maximize=[False])
+    objective_2 = ScalarObjective(
+        name="minimize the pubic force experienced by a passenger", evaluator=f_2, maximize=[False]
+    )
     objective_3 = ScalarObjective(
-        name="minimize the average velocity of the V-pillar responsible for whitstanding the impact load", 
-        evaluator=f_3, maximize=[False])
+        name="minimize the average velocity of the V-pillar responsible for whitstanding the impact load",
+        evaluator=f_3,
+        maximize=[False],
+    )
 
     if three_obj:
         objectives = [objective_1, objective_2, objective_3]
 
         # Cons with three objective functions
         cons_1 = ScalarConstraint("c_1", 7, 3, g_1)
         cons_2 = ScalarConstraint("c_2", 7, 3, g_2)
@@ -181,15 +177,15 @@
         cons_7 = ScalarConstraint("c_7", 7, 3, g_7)
         cons_8 = ScalarConstraint("c_8", 7, 3, g_8)
         cons_9 = ScalarConstraint("c_9", 7, 3, g_9)
         cons_10 = ScalarConstraint("c_10", 7, 3, g_10)
 
     else:
         # If three_obj is false, then problem is with 4 objectives.
-        
+
         # the sum of constraint violations
         def f_4(x: np.ndarray) -> np.ndarray:
             x = np.atleast_2d(x)
             sum1 = g_1(x)
             sum2 = g_2(x)
             sum3 = g_3(x)
             sum4 = g_4(x)
@@ -223,23 +219,22 @@
         cons_5 = ScalarConstraint("c_5", 7, 4, g_5)
         cons_6 = ScalarConstraint("c_6", 7, 4, g_6)
         cons_7 = ScalarConstraint("c_7", 7, 4, g_7)
         cons_8 = ScalarConstraint("c_8", 7, 4, g_8)
         cons_9 = ScalarConstraint("c_9", 7, 4, g_9)
         cons_10 = ScalarConstraint("c_10", 7, 4, g_10)
 
-
     constraints = [cons_1, cons_2, cons_3, cons_4, cons_5, cons_6, cons_7, cons_8, cons_9, cons_10]
 
     x_1 = Variable("Thickness of B-Pillar inner", 1, 0.5, 1.5)
     x_2 = Variable("Thickness of B-Pillar reinforcement", 0.9, 0.45, 1.35)
     x_3 = Variable("Thickness of floor side inner", 1, 0.5, 1.5)
     x_4 = Variable("Thickness of cross members", 1, 0.5, 1.5)
-    x_5 = Variable("Thickness of door beam", 1.75,  0.875, 2.625)
+    x_5 = Variable("Thickness of door beam", 1.75, 0.875, 2.625)
     x_6 = Variable("Thickness of door beltline reinforcement", 0.8, 0.4, 1.2)
     x_7 = Variable("Thickness of roof rail", 0.8, 0.4, 1.2)
 
     variables = [x_1, x_2, x_3, x_4, x_5, x_6, x_7]
 
     problem = MOProblem(variables=variables, objectives=objectives, constraints=constraints)
 
-    return problem
+    return problem
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/DBMOPP_generator.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/DBMOPP_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import functools
 from time import time
-from typing import Dict, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 from descartes import PolygonPatch
-from desdeo_problem.problem import (
-    MOProblem,
-    ScalarConstraint,
-    VectorObjective,
-    variable_builder,
-)
+from desdeo_problem.problem import MOProblem, ScalarConstraint, VectorObjective, variable_builder
 from desdeo_problem.testproblems.DBMOPP.Region import Attractor, AttractorRegion, Region
 from desdeo_problem.testproblems.DBMOPP.utilities import (
     assign_design_dimension_projection,
     between_lines_rooted_at_pivot,
     euclidean_distance,
     get_2D_version,
     get_random_angles,
@@ -96,25 +90,15 @@
         ndo: int = 0,
         vary_sol_density: bool = False,
         vary_objective_scales: bool = False,
         prop_neutral: float = 0,
         nm: int = 10000,
     ) -> None:
         msg = self._validate_args(
-            k,
-            n,
-            nlp,
-            ndr,
-            ngp,
-            prop_constraint_checker,
-            pareto_set_type,
-            constraint_type,
-            ndo,
-            prop_neutral,
-            nm,
+            k, n, nlp, ndr, ngp, prop_constraint_checker, pareto_set_type, constraint_type, ndo, prop_neutral, nm
         )
         if msg != "":
             raise Exception(msg)
         self.k = k
         self.n = n
         self.nlp = nlp
         self.ndr = ndr
@@ -251,34 +235,20 @@
                 return self.evaluate_constraint(x, region)
             for i in range(x.shape[0]):
                 res = np.concatenate((res, self.evaluate_constraint(x[i], region)))
             return res
 
         if self.constraint_type in [1, 2, 3, 4]:
             for i, region in enumerate(self.obj.hard_constraint_regions):
-                const_evaluator = functools.partial(eval_wrapper,  region=region)
-                constraints.append(
-                    ScalarConstraint(
-                        f"hard constraint {i}",
-                        self.n,
-                        self.k,
-                        evaluator=const_evaluator,
-                    )
-                )
+                const_evaluator = functools.partial(eval_wrapper, region=region)
+                constraints.append(ScalarConstraint(f"hard constraint {i}", self.n, self.k, evaluator=const_evaluator))
         elif self.constraint_type in [5, 6, 7, 8]:
             for i, region in enumerate(self.obj.soft_constraint_regions):
                 const_evaluator = functools.partial(eval_wrapper, region=region)
-                constraints.append(
-                    ScalarConstraint(
-                        f"soft constraint {i}",
-                        self.n,
-                        self.k,
-                        evaluator=const_evaluator,
-                    )
-                )
+                constraints.append(ScalarConstraint(f"soft constraint {i}", self.n, self.k, evaluator=const_evaluator))
         else:
             const_evaluator = None
 
         if const_evaluator is None:
             return MOProblem(objectives, variables)
         return MOProblem(objectives, variables, constraints)
 
@@ -319,15 +289,15 @@
     def evaluate(self, x):
         x = np.atleast_2d(x)
         self.check_valid_length(x)
         z = get_2D_version(x, self.obj.pi1, self.obj.pi2)
         return self.evaluate_2D(z)
 
     # used inside of DBMOPP object.
-    def evaluate_2D(self, x) -> Dict:
+    def evaluate_2D(self, x) -> dict:
         """
         Evaluate x in problem instance in 2 dimensions
 
         Args:
             x (np.ndarray): The decision vector to be evaluated
 
         Returns:
@@ -706,15 +676,14 @@
             self.obj.soft_constraint_regions = self.obj.centre_regions
             for i in range(len(self.obj.soft_constraint_regions)):
                 self.obj.soft_constraint_regions[i].radius = self.obj.soft_constraint_regions[i].radius * r
 
     def place_discontinunities_neutral_and_checker_constraints(self):
         print("Assigning any checker soft/hard constraint regions and neutral regions\n", self.prop_contraint_checker)
         if (self.prop_contraint_checker + self.prop_neutral) > 0:
-
             S = (np.random.rand(self.nm, 2) * 2) - 1
             print(S.shape)
             for _i, centre_region in enumerate(self.obj.centre_regions):
                 to_remove = centre_region.is_inside(S, True)
                 not_to_remove = np.logical_not(to_remove)
                 S = S[not_to_remove, :]
 
@@ -778,15 +747,15 @@
             regions.append(region)
             S = S[:-1, :]  # remove last row
 
             d = euclidean_distance(S, region.centre)
             Idx = d > r  # this was d > r before
             S = S[Idx, :]  # Remove covered points
             # flake8 does not like this. TODO: fix but make sure logic won't change, will break constraints
-            covered_count = (Idx == False).sum() + 1
+            covered_count = (Idx is False).sum() + 1
 
             allocation += covered_count / self.nm
 
         return np.array(regions), S
 
     # used for moproblem
     def check_region_prob(self, regions, x, include_boundary):
@@ -915,20 +884,15 @@
                         ans["in_pareto_region"] = not ans[
                             "in_pareto_region"
                         ]  # special case where last region is split at the two sides, should not get here everytime
 
         return ans
 
     def update_with_discontinuity(self, x, y):
-        return self.update(
-            self.obj.discontinuous_regions,
-            self.obj.discontinuous_region_objective_value_offset,
-            x,
-            y,
-        )
+        return self.update(self.obj.discontinuous_regions, self.obj.discontinuous_region_objective_value_offset, x, y)
 
     def update_with_neutrality(self, x, y):
         return self.update(self.obj.neutral_regions, self.obj.neutral_region_objective_values, x, y)
 
     def update(self, regions, offsets, x, y):
         if regions is None:
             return y
@@ -1015,22 +979,15 @@
 
         fig, ax = plt.subplots(subplot_kw={"projection": "3d"})
         ax.set_xlim(-1, 1)
         ax.set_ylim(-1, 1)
         ax.view_init(elev=90, azim=-90)
 
         surf = ax.plot_surface(
-            x,
-            y,
-            z.T,
-            cmap=cm.plasma,
-            linewidth=0,
-            antialiased=False,
-            vmin=np.nanmin(z),
-            vmax=np.nanmax(z),
+            x, y, z.T, cmap=cm.plasma, linewidth=0, antialiased=False, vmin=np.nanmin(z), vmax=np.nanmax(z)
         )
 
         fig.colorbar(surf, shrink=0.5, aspect=5)
         # plt.show()
 
     def plot_pareto_set_members(self, resolution=500):
         if resolution < 1:
@@ -1117,93 +1074,64 @@
         neutral_idx = 1
         # label contiguos neutral areas
         for i in range(res):
             for j in range(res):
                 # if not dominated and not yet assigned to a neutral area
                 if dominated[i, j] == 0 and neutral_areas[i, j] < 0:
                     neutral_areas = self.identify_neutral_area_members(
-                        i,
-                        j,
-                        neutral_areas,
-                        neutral_idx,
-                        dominated,
-                        neutral_neighbours,
-                        moore_neighbourhood,
-                        offset,
+                        i, j, neutral_areas, neutral_idx, dominated, neutral_neighbours, moore_neighbourhood, offset
                     )
                     neutral_idx = neutral_idx + 1
 
         # identify basins of attraction
         basins = np.ones((res, res)) * -1
         basins[neutral_areas > 0] = 0
         processed = np.zeros((res, res))
         number_distinct_neutral_regions = np.max(np.max(neutral_areas))  # check if this is correct
         destination = [[] for d in range(res)]
         for i in range(res):
             for j in range(res):
                 if processed[i, j] == 0:
                     processed, destination, _ = self.update_destinations(
-                        i,
-                        j,
-                        processed,
-                        destination,
-                        dominating_neighbours,
-                        neutral_areas,
-                        offset,
+                        i, j, processed, destination, dominating_neighbours, neutral_areas, offset
                     )
 
         # now fill value in basins
         for i in range(res):
             for j in range(res):
                 if neutral_areas[i, j] > 0:
                     basins[i, j] = 0
                 else:
                     if len(destination[i, j]) == 1:
                         # put between 0.25 and 0.75, graded by which basin it leads to
                         basins[i, j] = 0.25 + destination[i, j] / (2 * number_distinct_neutral_regions)
                     else:
                         basins[i, j] = 1
 
-        return (
-            basins,
-            neutral_areas,
-            dominated,
-            destination,
-            dominating_neighbours,
-            offset,
-        )
+        return (basins, neutral_areas, dominated, destination, dominating_neighbours, offset)
 
     def identify_dominating_neighbours(self, z, i, j, res, moore_neighbourhood, offset):
         if moore_neighbourhood:
             n = 8
         else:
             n = 4
         dominating_neighbours = np.zeros((n, 1))
         neutral_neighbours = np.zeros((n, 1))
 
         for k in range(n):
             if i + offset[k, 1] > 0 and i + offset[k, 1] <= res and j + offset[k, 2] > 0 and j + offset[k, 2] <= res:
-                (
-                    dominating_neighbours[k],
-                    neutral_neighbours[k],
-                ) = self.vector_is_dominated_or_neutral(z[:, i, j], z[:, i + offset[k, 1] + offset[k, 2]])
+                (dominating_neighbours[k], neutral_neighbours[k]) = self.vector_is_dominated_or_neutral(
+                    z[:, i, j], z[:, i + offset[k, 1] + offset[k, 2]]
+                )
 
         dominated = np.any(dominating_neighbours)  # check its same as matlabs any
         return dominating_neighbours, neutral_neighbours, dominated
 
     def identify_neutral_area_members(
-        self,
-        i,
-        j,
-        neutral_areas,
-        n_idx,
-        dominated,
-        neutral_neighbours,
-        moore_neighbourhood,
-        offset,
+        self, i, j, neutral_areas, n_idx, dominated, neutral_neighbours, moore_neighbourhood, offset
     ):
         pass
 
     def update_destinations(self, i, j, processed, destination, dominating_neighbours, neutral_areas, offset):
         pass
         # TODO: make work on 0s and 1s instead of true and falses, since np arrays are using 0s as false and 1s as true
 
@@ -1275,37 +1203,33 @@
 
         z = process_dims(z, x[0], self.obj.pi1)
         z = process_dims(z, x[1], self.obj.pi2)
         return z
 
     # returns random pareto set member uniformly from the Pareto set and the point in 2D it maps to
     # should not be used during optimization
-    def get_Pareto_set_member(self) -> Tuple:
+    def get_Pareto_set_member(self) -> tuple:
         # while not legal point obtained, get random pareto centre
         invalid = True
         x = []
         point = []
         low = np.min(self.obj.pareto_set_indices)
         high = np.max(self.obj.pareto_set_indices)
         centres = self.obj.centre_regions
         iters = 0
 
         while invalid:
-
             k = np.random.randint(low, high + 1)  # + self.nlp + self.ndr. +1 bc randint is [)
             angle = np.random.rand() * 2.0 * np.pi
 
             # 2D case
             if self.constraint_type == 2 or self.constraint_type == 6:
                 # if centre constraints used, randomly choose angle and use that radius from
                 # Pareto set centre list and project
-                x = centres[k].centre + [
-                    centres[k].radius * np.cos(angle),
-                    centres[k].radius * np.sin(angle),
-                ]
+                x = centres[k].centre + [centres[k].radius * np.cos(angle), centres[k].radius * np.sin(angle)]
                 invalid = False
             else:
                 # generate random point in Circle
                 r = centres[k].radius * np.sqrt(np.random.rand())
                 x = centres[k].centre + [r * np.cos(angle), r * np.sin(angle)]
                 if self.is_pareto_2D(x):
                     invalid = False
@@ -1340,28 +1264,24 @@
         results = []
         results2d = []
         k = low
 
         while len(results2d) < points:
             invalid = True
             while invalid and len(centre_list) <= len(centres):
-
                 if k >= high:
                     k = low
                 # k = np.random.randint(low, high) #+ self.nlp + self.ndr
                 angle = np.random.rand() * 2.0 * np.pi
 
                 # 2D case
                 if self.constraint_type == 2 or self.constraint_type == 6:
                     # if centre constraints used, randomly choose angle and use that radius from
                     # Pareto set centre list and project
-                    x = centres[k].centre + [
-                        centres[k].radius * np.cos(angle),
-                        centres[k].radius * np.sin(angle),
-                    ]
+                    x = centres[k].centre + [centres[k].radius * np.cos(angle), centres[k].radius * np.sin(angle)]
                     invalid = False
                 else:
                     # generate random point in Circle
                     r = centres[k].radius * np.sqrt(np.random.rand())
                     x = centres[k].centre + [r * np.cos(angle), r * np.sin(angle)]
                     if self.is_pareto_2D(x):
                         if k not in centre_list:
@@ -1380,15 +1300,14 @@
                 point = x
             results.append(x)
             results2d.append(point)
         return results, results2d
 
 
 if __name__ == "__main__":
-
     n_objectives = 5
     n_variables = 5
     n_local_pareto_regions = 2
     n_dominance_res_regions = 0
     n_global_pareto_regions = 4
     const_space = 0.6
     pareto_set_type = 2
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/README.md` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/README.md`

 * *Files identical despite different names*

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/Region.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/Region.py`

 * *Files identical despite different names*

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/DBMOPP/utilities.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/DBMOPP/utilities.py`

 * *Files identical despite different names*

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/DummyProblem.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/DummyProblem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from desdeo_problem.problem.Variable import Variable
 from desdeo_problem.problem.Objective import ScalarObjective
 from desdeo_problem.problem.Problem import MOProblem
 
 import numpy as np
 
+
 def dummy_problem() -> MOProblem:
     """An example on how to implement a problem with 3 objectives and 4 variables and no constraints.
 
     Returns:
         MOProblem: a problem object.
     """
+
     def f1(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
 
         # sum the rows
         return np.sum(x, axis=1)
 
     def f2(x: np.ndarray) -> np.ndarray:
@@ -42,9 +44,7 @@
 
     variables = [variable_1, variable_2, variable_3, variable_4]
 
     # instantiate MOProblem object
     problem = MOProblem(objectives, variables)
 
     return problem
-
-
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/MultipleClutchBrakes.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/MultipleClutchBrakes.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,196 +4,152 @@
 Osyczka, A. (1992). Computer aided multicriterion optimization 
 system (CAMOS) : software package in FORTRAN.
 
 """
 
 from desdeo_problem.problem.Variable import Variable
 from desdeo_problem.problem.Objective import ScalarObjective
-from desdeo_problem.problem.Problem import MOProblem, ProblemBase
-from desdeo_problem import ScalarConstraint, problem
+from desdeo_problem.problem.Problem import MOProblem
+from desdeo_problem import ScalarConstraint
 
 import numpy as np
 
+
 def multiple_clutch_brakes(var_iv: np.array = np.array([67.5, 92.5, 2.25, 650, 6])) -> MOProblem:
     """ Multiple clutch brake problem.
     
     Arguments:
         var_iv (np.array): Optional, initial variable values.
             Defaults are [67.5, 92.5, 2.25, 650, 6]. 
             x1 ∈ [55, 80], x2 ∈ [75, 110], x3 ∈ [1.5, 3], 
             x4 ∈ [300, 1000] and x5 ∈ {2, ..., 10}
 
     Returns:
         MOProblem: a problem object.
     """
 
     # Check the number of variables
-    if (np.shape(np.atleast_2d(var_iv)[0]) != (5,)):
+    if np.shape(np.atleast_2d(var_iv)[0]) != (5,):
         raise RuntimeError("Number of variables must be seven")
 
     # Lower bounds
     lb = np.array([55, 75, 1.5, 300, 2])
-    
+
     # Upper bounds
     ub = np.array([80, 110, 3, 1000, 10])
 
     # Check the variable bounds
     if np.any(lb > var_iv) or np.any(ub < var_iv):
         raise ValueError("Initial variable values need to be between lower and upper bounds")
 
     def m_h(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
         return (
-            (2/3) * 0.5 * x[:,3] * (np.round(x[:,4])) * 
-            ((x[:,1]**3 - x[:,0]**3) / (x[:,1]**2 - x[:,0]**2))
-            * 0.001 # This line is from Jussi's Matlab code
-            
+            (2 / 3)
+            * 0.5
+            * x[:, 3]
+            * (np.round(x[:, 4]))
+            * ((x[:, 1] ** 3 - x[:, 0] ** 3) / (x[:, 1] ** 2 - x[:, 0] ** 2))
+            * 0.001  # This line is from Jussi's Matlab code
             # Mh = (2/3) * mu* x(5-1) * x(6-1) * ((x(3-1)^3-x(2-1)^3)/(x(3-1)^2-x(2-1)^2)) * 0.001; %convert to Nm
         )
 
     def p_rz(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            x[:, 3] / (np.pi * x[:, 1]**2 - np.pi * x[:, 0]**2)
-        )
-    
+        return x[:, 3] / (np.pi * x[:, 1] ** 2 - np.pi * x[:, 0] ** 2)
+
     def v_sr(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            (np.pi * (2/3 * ((x[:, 1]**3 - x[:, 0]**3) / 
-            (x[:, 1]**2 - x[:, 0]**2))) * 250) / 30
-        )
+        return (np.pi * (2 / 3 * ((x[:, 1] ** 3 - x[:, 0] ** 3) / (x[:, 1] ** 2 - x[:, 0] ** 2))) * 250) / 30
 
     # Objective functions
     def f_1(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            np.pi * ((x[:, 1]**2 - x[:, 0]**2)) * (x[:, 2] * (np.round(x[:, 4]) + 1)) * 0.0000078
-        )
+        return np.pi * ((x[:, 1] ** 2 - x[:, 0] ** 2)) * (x[:, 2] * (np.round(x[:, 4]) + 1)) * 0.0000078
 
     def f_2(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            (55 * ((np.pi * 250) / 30)) / ((m_h(x)) + 3)
-        )
-    
+        return (55 * ((np.pi * 250) / 30)) / ((m_h(x)) + 3)
+
     def f_3(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            np.round(x[:, 4])
-        )
+        return np.round(x[:, 4])
 
     def f_4(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            x[:, 1]
-        )
+        return x[:, 1]
 
     def f_5(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            x[:, 3]
-        )
+        return x[:, 3]
 
     # Constraint functions
-    def g_1(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_1(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            x[:, 0] - 55
-        )
+        return x[:, 0] - 55
 
-    def g_2(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_2(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            110 - x[:, 1]
-        )
+        return 110 - x[:, 1]
 
-    def g_3(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_3(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            x[:, 1] - x[:, 0] - 20 
-        )
+        return x[:, 1] - x[:, 0] - 20
 
-    def g_4(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_4(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            x[:, 2] - 1.5
-        )
+        return x[:, 2] - 1.5
 
-    def g_5(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_5(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            3 - x[:, 2]
-        )
+        return 3 - x[:, 2]
 
-    def g_6(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_6(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            30 - (np.round(x[:, 4]) + 1) * (x[:, 2] + 0.5)
-        )
+        return 30 - (np.round(x[:, 4]) + 1) * (x[:, 2] + 0.5)
 
-    def g_7(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_7(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            10 - (np.round(x[:, 4]) + 1)
-        )
+        return 10 - (np.round(x[:, 4]) + 1)
 
-    def g_8(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_8(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            np.round(x[:, 4]) - 1
-        )
-    
-    def g_9(x: np.ndarray, _ = None) -> np.ndarray:
+        return np.round(x[:, 4]) - 1
+
+    def g_9(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            10 - p_rz(x)
-        )
+        return 10 - p_rz(x)
 
-    def g_10(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_10(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            10 * 2000 - (p_rz(x) * v_sr(x))
-        )
+        return 10 * 2000 - (p_rz(x) * v_sr(x))
 
-    def g_11(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_11(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            2000 - v_sr(x)
-        )
+        return 2000 - v_sr(x)
 
-    def g_12(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_12(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            15 - f_2(x)
-        )
+        return 15 - f_2(x)
 
-    def g_13(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_13(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            m_h(x) - (1.5 * 40)
-        )
-            
-    def g_14(x: np.ndarray, _ = None) -> np.ndarray:
+        return m_h(x) - (1.5 * 40)
+
+    def g_14(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            f_2(x)
-        )
+        return f_2(x)
 
-    def g_15(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_15(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            x[:, 3]
-        )
+        return x[:, 3]
 
-    def g_16(x: np.ndarray, _ = None) -> np.ndarray:
+    def g_16(x: np.ndarray, _=None) -> np.ndarray:
         x = np.atleast_2d(x)
-        return (
-            1000 - x[:, 3]
-        )
+        return 1000 - x[:, 3]
 
     objective_1 = ScalarObjective(name="mass of the brake", evaluator=f_1, maximize=[False])
     objective_2 = ScalarObjective(name="stopping time", evaluator=f_2, maximize=[False])
     objective_3 = ScalarObjective(name="number of friction surfaces", evaluator=f_3, maximize=[False])
     objective_4 = ScalarObjective(name="outer radius", evaluator=f_4, maximize=[False])
     objective_5 = ScalarObjective(name="actuating force", evaluator=f_5, maximize=[False])
 
@@ -212,22 +168,37 @@
     cons_11 = ScalarConstraint("c_11", 5, 5, g_11)
     cons_12 = ScalarConstraint("c_12", 5, 5, g_12)
     cons_13 = ScalarConstraint("c_13", 5, 5, g_13)
     cons_14 = ScalarConstraint("c_14", 5, 5, g_14)
     cons_15 = ScalarConstraint("c_15", 5, 5, g_15)
     cons_16 = ScalarConstraint("c_16", 5, 5, g_16)
 
-
-    constraints = [cons_1, cons_2, cons_3, cons_4, cons_5, cons_6, cons_7, cons_8, 
-        cons_9, cons_10, cons_11, cons_12, cons_13, cons_14, cons_15, cons_16]
+    constraints = [
+        cons_1,
+        cons_2,
+        cons_3,
+        cons_4,
+        cons_5,
+        cons_6,
+        cons_7,
+        cons_8,
+        cons_9,
+        cons_10,
+        cons_11,
+        cons_12,
+        cons_13,
+        cons_14,
+        cons_15,
+        cons_16,
+    ]
 
     x_1 = Variable("inner radius", 67.5, 55, 80)
     x_2 = Variable("outer radius", 92.5, 75, 110)
     x_3 = Variable("thickness of the disc", 2.25, 1.5, 3)
     x_4 = Variable("actuating force", 650, 300, 1000)
     x_5 = Variable("number of friction surfaces", 6, 2, 10)
 
     variables = [x_1, x_2, x_3, x_4, x_5]
 
     problem = MOProblem(variables=variables, objectives=objectives, constraints=constraints)
 
-    return problem
+    return problem
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/RiverPollution.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/RiverPollution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from desdeo_problem.problem.Variable import Variable
 from desdeo_problem.problem.Objective import ScalarObjective
-from desdeo_problem.problem.Problem import MOProblem, ProblemBase
+from desdeo_problem.problem.Problem import MOProblem
 
 import numpy as np
 
+
 def river_pollution_problem(five_obj: bool = True, var_iv: np.array = np.array([0.5, 0.5])) -> MOProblem:
     """The river pollution problem with 4 or 5 objectives.
 
     NARULA, S. C. & WEISTROFFER, H. R. (1989). A flexible method for 
     nonlinear multicriteria decisionmaking problems. IEEE transactions on 
     systems, man, and cybernetics, 19(4), 883-887.
 
@@ -16,52 +17,56 @@
             version if false. Default is true. 
         var_iv (np.array): Optional, initial variable values. Must be between 0.3 and 1.0.
             Defaults are 0.5 and 0.5. 
 
     Returns:
         MOProblem: a problem object.
     """
-    
+
     if np.any(1 < var_iv) or np.any(var_iv < 0.3):
 
         raise ValueError("Initial variable values need to be between lower and upper bounds")
 
     def f_1(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return -4.07 - 2.27*x[:, 0]
+        return -4.07 - 2.27 * x[:, 0]
 
     def f_2(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return -2.60 - 0.03*x[:, 0] - 0.02*x[:, 1] - 0.01 / (1.39 - x[:, 0]**2) - 0.30 / (1.39 - x[:, 1]**2)
+        return -2.60 - 0.03 * x[:, 0] - 0.02 * x[:, 1] - 0.01 / (1.39 - x[:, 0] ** 2) - 0.30 / (1.39 - x[:, 1] ** 2)
 
     def f_3(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return -8.21 + 0.71 / (1.09 - x[:, 0]**2)
+        return -8.21 + 0.71 / (1.09 - x[:, 0] ** 2)
 
     def f_4(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
-        return -0.96 + 0.96 / (1.09 - x[:, 1]**2)
-    
+        return -0.96 + 0.96 / (1.09 - x[:, 1] ** 2)
+
     objective_1 = ScalarObjective(name="the DO level in the city", evaluator=f_1, maximize=[True])
     objective_2 = ScalarObjective(name="the DO level at the municipality border", evaluator=f_2, maximize=[True])
-    objective_3 = ScalarObjective(name="the percent return on investment at the fishery", evaluator=f_3, maximize=[True])
+    objective_3 = ScalarObjective(
+        name="the percent return on investment at the fishery", evaluator=f_3, maximize=[True]
+    )
     objective_4 = ScalarObjective(name="the addition to the tax rate of city", evaluator=f_4, maximize=[True])
-    
 
     if five_obj:
+
         def f_5(x: np.ndarray) -> np.ndarray:
             return np.max([np.abs(x[:, 0] - 0.65), np.abs(x[:, 1] - 0.65)], axis=0)
 
-        objective_5 = ScalarObjective(name="BOD removed form the water close to the ideal value of 0.65", evaluator=f_5, maximize=[False])
+        objective_5 = ScalarObjective(
+            name="BOD removed form the water close to the ideal value of 0.65", evaluator=f_5, maximize=[False]
+        )
         objectives = [objective_1, objective_2, objective_3, objective_4, objective_5]
     else:
-        # If five_obj is false, then problem is with 4 objectives. 
+        # If five_obj is false, then problem is with 4 objectives.
         objectives = [objective_1, objective_2, objective_3, objective_4]
 
     x_1 = Variable("the proportionate amount of BOD removed from water at the fishery", var_iv[0], 0.3, 1.0)
     x_2 = Variable("the proportionate amount of BOD removed from water at the city", var_iv[1], 0.3, 1.0)
 
     variables = [x_1, x_2]
-    
+
     problem = MOProblem(variables=variables, objectives=objectives)
 
     return problem
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/TestProblems.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/TestProblems.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         "DTLZ3": dtlz.DTLZ3,
         "DTLZ4": dtlz.DTLZ4,
         "DTLZ5": dtlz.DTLZ5,
         "DTLZ6": dtlz.DTLZ6,
         "DTLZ7": dtlz.DTLZ7,
     }
     num_var = {"ZDT1": 30, "ZDT2": 30, "ZDT3": 30, "ZDT4": 10, "ZDT6": 10}
-    if not (name in problems.keys()):
+    if name not in problems.keys():
         msg = "Specified Problem not yet supported.\n The supported problems are:" + str(problems.keys())
         raise ProblemError(msg)
     if "ZDT" in name:
         if n_of_variables is None:
             n_of_variables = num_var[name]
         if n_of_objectives is None:
             n_of_objectives = 2
@@ -70,18 +70,15 @@
         msg = "How did you end up here?"
         raise ProblemError(msg)
     lower_limits = obj_func.min_bounds
     upper_limits = obj_func.max_bounds
     var_names = ["x" + str(i + 1) for i in range(n_of_variables)]
     obj_names = ["f" + str(i + 1) for i in range(n_of_objectives)]
     variables = variable_builder(
-        names=var_names,
-        initial_values=lower_limits,
-        lower_bounds=lower_limits,
-        upper_bounds=upper_limits,
+        names=var_names, initial_values=lower_limits, lower_bounds=lower_limits, upper_bounds=upper_limits
     )
 
     # Because optproblems can only handle one objective at a time
     def modified_obj_func(x):
         if isinstance(x, list):
             if len(x) == n_of_variables:
                 return [obj_func(x)]
```

### Comparing `desdeo_problem-1.5.0/desdeo_problem/testproblems/VehicleCrashworthiness.py` & `desdeo_problem-1.6.0/desdeo_problem/testproblems/VehicleCrashworthiness.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from desdeo_problem.problem.Variable import Variable
 from desdeo_problem.problem.Objective import ScalarObjective
-from desdeo_problem.problem.Problem import MOProblem, ProblemBase
+from desdeo_problem.problem.Problem import MOProblem
 
 import numpy as np
 
+
 def vehicle_crashworthiness(var_iv: np.array = np.array([2, 2, 2, 2, 2])) -> MOProblem:
     """The crash safety design problem with 3 objectives.
 
     Liao, X., Li, Q., Yang, X., Zhang, W. & Li, W. (2007).
     Multiobjective optimization for crash safety design of vehicles
     using stepwise regression model. Structural and multidisciplinary
     optimization, 35(6), 561-569. https://doi.org/10.1007/s00158-007-0163-x
@@ -16,15 +17,15 @@
         var_iv (np.array): Optional, initial variable values. Must be between
             1 and 3. Defaults are [2, 2, 2, 2, 2].
 
     Returns:
         MOProblem: a problem object.
     """
 
-    if np.any(3 < var_iv) or np.any(var_iv < 1):
+    if np.any(var_iv > 3) or np.any(var_iv < 1):
         raise ValueError("Initial variable values need to be between lower and upper bounds")
 
     # Mass
     def f_1(x: np.ndarray) -> np.ndarray:
         x = np.atleast_2d(x)
         return (
             1640.2823
@@ -65,26 +66,28 @@
             - 0.0118 * x[:, 1] * x[:, 3]
             - 0.0204 * x[:, 2] * x[:, 3]
             - 0.008 * x[:, 2] * x[:, 4]
             - 0.0241 * x[:, 1] ** 2
             + 0.0109 * x[:, 3] ** 2
         )
 
-
-
     objective_1 = ScalarObjective(name="the mass of the vehicle", evaluator=f_1, maximize=[False])
-    objective_2 = ScalarObjective(name="acceleration-induced biomechanical damage of occupants", evaluator=f_2, maximize=[False])
-    objective_3 = ScalarObjective(name="the toe board intrusion in the 'offset-frontal crash'", evaluator=f_3, maximize=[False])
+    objective_2 = ScalarObjective(
+        name="acceleration-induced biomechanical damage of occupants", evaluator=f_2, maximize=[False]
+    )
+    objective_3 = ScalarObjective(
+        name="the toe board intrusion in the 'offset-frontal crash'", evaluator=f_3, maximize=[False]
+    )
 
     objectives = [objective_1, objective_2, objective_3]
 
     x_1 = Variable("x_1", var_iv[0], 1.0, 3.0)
     x_2 = Variable("x_2", var_iv[1], 1.0, 3.0)
     x_3 = Variable("x_3", var_iv[2], 1.0, 3.0)
     x_4 = Variable("x_4", var_iv[3], 1.0, 3.0)
     x_5 = Variable("x_5", var_iv[4], 1.0, 3.0)
 
     variables = [x_1, x_2, x_3, x_4, x_5]
 
     problem = MOProblem(variables=variables, objectives=objectives)
 
-    return problem
+    return problem
```

### Comparing `desdeo_problem-1.5.0/PKG-INFO` & `desdeo_problem-1.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: desdeo-problem
-Version: 1.5.0
+Name: desdeo_problem
+Version: 1.6.0
 Summary: This package contains the problem classes for desdeo framework.
 License: MIT
 Author: Bhupinder Saini
 Author-email: bhupinder.s.saini@jyu.fi
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Shapely (>=1.8.0,<2.0.0)
 Requires-Dist: descartes (>=1.1.0,<2.0.0)
 Requires-Dist: desdeo-tools (>=1.8.0,<2.0.0)
 Requires-Dist: diversipy (>=0.8.0,<0.9.0)
 Requires-Dist: optproblems (>=1.2,<2.0)
 Requires-Dist: scikit-learn (>=1.1,<2.0)
```

