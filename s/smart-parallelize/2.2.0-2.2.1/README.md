# Comparing `tmp/smart_parallelize-2.2.0.tar.gz` & `tmp/smart_parallelize-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.2.0.tar", max compression
+gzip compressed data, was "smart_parallelize-2.2.1.tar", max compression
```

## Comparing `smart_parallelize-2.2.0.tar` & `smart_parallelize-2.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      554 2024-05-13 01:37:00.192639 smart_parallelize-2.2.0/README.md
--rw-r--r--   0        0        0      317 2024-05-21 19:28:56.577104 smart_parallelize-2.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.2.0/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4004 2024-05-14 17:03:12.517416 smart_parallelize-2.2.0/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0     4100 2024-05-13 16:25:38.243039 smart_parallelize-2.2.0/smart_parallelize/parallelize_DEP.py
--rw-r--r--   0        0        0     1820 2024-05-21 19:40:46.175222 smart_parallelize-2.2.0/smart_parallelize/parallelize_native.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 smart_parallelize-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      554 2024-05-13 01:37:00.192639 smart_parallelize-2.2.1/README.md
+-rw-r--r--   0        0        0      317 2024-05-21 19:46:43.572298 smart_parallelize-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.2.1/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-21 19:46:31.474437 smart_parallelize-2.2.1/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0     4328 2024-05-21 19:46:36.544808 smart_parallelize-2.2.1/smart_parallelize/parallelize_DEP.py
+-rw-r--r--   0        0        0     1824 2024-05-21 19:46:08.870023 smart_parallelize-2.2.1/smart_parallelize/parallelize_native.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 smart_parallelize-2.2.1/PKG-INFO
```

### Comparing `smart_parallelize-2.2.0/README.md` & `smart_parallelize-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.2.0/smart_parallelize/parallelize.py` & `smart_parallelize-2.2.1/smart_parallelize/parallelize.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from functools import wraps
+# from functools import wraps
 
-import numpy as np
-from ray.exceptions import RaySystemError
-from ray import available_resources, init, remote, get, put
-
-
-def get_mem_func():
-    try:
-        MEMORY = available_resources()['memory']
-    except RaySystemError:
-        init()
-        MEMORY = available_resources()['memory']
-    try:
-        CPUS = available_resources()['CPU']
-        MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
-    except KeyError:
-        # get number of cores
-        import multiprocessing
-        CPUS = multiprocessing.cpu_count()
-        MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
-    MEMORY = int(MEMORY)
-    CPUS   = int(CPUS)
-    MEM_PER_WORKER = int(MEM_PER_WORKER)
-    return MEMORY, CPUS, MEM_PER_WORKER
-
-try:
-	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
-except RaySystemError:
-	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
-
-
-def smart_parallelize(args2parallelize=1):
-    def decorator(function):
-        @wraps(function)
-        def wrapper(**kwargs):
-            @remote(memory=MEM_PER_WORKER)
-            def get_results(**kwargs):
-                par_args = list(kwargs.keys())[:args2parallelize]
-                other_args = list(kwargs.keys())[args2parallelize:]
-                data_par_args = [kwargs[i] for i in par_args]
-
-                results = []
-                for i, _ in enumerate(data_par_args[0]):
-                    kwargs_0 = kwargs.copy()
-                    for j, arg in enumerate(par_args):
-                        kwargs_0[arg] = data_par_args[j][i]
-                    for k, arg in enumerate(other_args):
-                        kwargs_0[arg] = kwargs[arg]
-                    r = function(**kwargs_0)
-                    results.append(r)
-                return results
+# import numpy as np
+# from ray.exceptions import RaySystemError
+# from ray import available_resources, init, remote, get, put
+
+
+# def get_mem_func():
+#     try:
+#         MEMORY = available_resources()['memory']
+#     except RaySystemError:
+#         init()
+#         MEMORY = available_resources()['memory']
+#     try:
+#         CPUS = available_resources()['CPU']
+#         MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
+#     except KeyError:
+#         # get number of cores
+#         import multiprocessing
+#         CPUS = multiprocessing.cpu_count()
+#         MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
+#     MEMORY = int(MEMORY)
+#     CPUS   = int(CPUS)
+#     MEM_PER_WORKER = int(MEM_PER_WORKER)
+#     return MEMORY, CPUS, MEM_PER_WORKER
+
+# try:
+# 	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
+# except RaySystemError:
+# 	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
+
+
+# def smart_parallelize(args2parallelize=1):
+#     def decorator(function):
+#         @wraps(function)
+#         def wrapper(**kwargs):
+#             @remote(memory=MEM_PER_WORKER)
+#             def get_results(**kwargs):
+#                 par_args = list(kwargs.keys())[:args2parallelize]
+#                 other_args = list(kwargs.keys())[args2parallelize:]
+#                 data_par_args = [kwargs[i] for i in par_args]
+
+#                 results = []
+#                 for i, _ in enumerate(data_par_args[0]):
+#                     kwargs_0 = kwargs.copy()
+#                     for j, arg in enumerate(par_args):
+#                         kwargs_0[arg] = data_par_args[j][i]
+#                     for k, arg in enumerate(other_args):
+#                         kwargs_0[arg] = kwargs[arg]
+#                     r = function(**kwargs_0)
+#                     results.append(r)
+#                 return results
             
-            par_args = list(kwargs.keys())[:args2parallelize]
-            other_args = list(kwargs.keys())[args2parallelize:]
-            arg2parallelize_unsplit = [kwargs[i] for i in par_args]
-
-            # split into CPUS chunks
-            split_args = [np.array_split(i, CPUS) for i in arg2parallelize_unsplit]
-
-            workers = []
-            for i in range(CPUS):
-                inp_args = {}
-                for j, _ in enumerate(par_args):
-                    inp_args[par_args[j]] = split_args[j][i]
+#             par_args = list(kwargs.keys())[:args2parallelize]
+#             other_args = list(kwargs.keys())[args2parallelize:]
+#             arg2parallelize_unsplit = [kwargs[i] for i in par_args]
+
+#             # split into CPUS chunks
+#             split_args = [np.array_split(i, CPUS) for i in arg2parallelize_unsplit]
+
+#             workers = []
+#             for i in range(CPUS):
+#                 inp_args = {}
+#                 for j, _ in enumerate(par_args):
+#                     inp_args[par_args[j]] = split_args[j][i]
                 
-                for k, _ in enumerate(other_args):
-                    inp_args[other_args[k]] = kwargs[other_args[k]]
-                workers.append(get_results.remote(**inp_args))
+#                 for k, _ in enumerate(other_args):
+#                     inp_args[other_args[k]] = kwargs[other_args[k]]
+#                 workers.append(get_results.remote(**inp_args))
             
-            test_inp = {}
-            for j, _ in enumerate(par_args):
-                test_inp[par_args[j]] = arg2parallelize_unsplit[j][0]
-            for k, _ in enumerate(other_args):
-                test_inp[other_args[k]] = kwargs[other_args[k]]
-
-            output = function(**test_inp)
-            if not isinstance(output, list) and not isinstance(output, tuple):
-                num_outputs = 1
-            else:
-                num_outputs = len(output)
-
-            retval = get(workers)
-
-            # retval = retval.reshape(len(arg2parallelize_unsplit[0]), num_outputs)
-
-            retval = [j for i in retval for j in i]
-
-            if num_outputs != 1:
-                outputs = []
-                for i in range(num_outputs):
-                    outputs.append([])
-                for i, _ in enumerate(retval):
-                    for j, _ in enumerate(retval[i]):
-                        outputs[j].append(retval[i][j])
-                retval = outputs
-                for i in range(num_outputs):
-                    outputs[i] = np.array(outputs[i])
-            else:
-                retval = np.array(retval)
-            return retval
-        return wrapper
-    return decorator
-
-
-if __name__ == "__main__":
-    import timeit
-
-    @smart_parallelize(args2parallelize=1)
-    def func(x, y):
-        return x
+#             test_inp = {}
+#             for j, _ in enumerate(par_args):
+#                 test_inp[par_args[j]] = arg2parallelize_unsplit[j][0]
+#             for k, _ in enumerate(other_args):
+#                 test_inp[other_args[k]] = kwargs[other_args[k]]
+
+#             output = function(**test_inp)
+#             if not isinstance(output, list) and not isinstance(output, tuple):
+#                 num_outputs = 1
+#             else:
+#                 num_outputs = len(output)
+
+#             retval = get(workers)
+
+#             # retval = retval.reshape(len(arg2parallelize_unsplit[0]), num_outputs)
+
+#             retval = [j for i in retval for j in i]
+
+#             if num_outputs != 1:
+#                 outputs = []
+#                 for i in range(num_outputs):
+#                     outputs.append([])
+#                 for i, _ in enumerate(retval):
+#                     for j, _ in enumerate(retval[i]):
+#                         outputs[j].append(retval[i][j])
+#                 retval = outputs
+#                 for i in range(num_outputs):
+#                     outputs[i] = np.array(outputs[i])
+#             else:
+#                 retval = np.array(retval)
+#             return retval
+#         return wrapper
+#     return decorator
+
+
+# if __name__ == "__main__":
+#     import timeit
+
+#     @smart_parallelize(args2parallelize=1)
+#     def func(x, y):
+#         return x
     
-    x = np.ones((31,2))
-    # y = np.ones((30,))*2
-    y = 2
-    start  = timeit.default_timer()
-    answer = func(x=x, y=y)
-    stop  = timeit.default_timer()
-    print(stop - start)
-    print(answer)
+#     x = np.ones((31,2))
+#     # y = np.ones((30,))*2
+#     y = 2
+#     start  = timeit.default_timer()
+#     answer = func(x=x, y=y)
+#     stop  = timeit.default_timer()
+#     print(stop - start)
+#     print(answer)
```

### Comparing `smart_parallelize-2.2.0/smart_parallelize/parallelize_DEP.py` & `smart_parallelize-2.2.1/smart_parallelize/parallelize_DEP.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-# import ray
-import numpy as np
-from time import sleep
-from ray.exceptions import RaySystemError
+# # import ray
+# import numpy as np
+# from time import sleep
+# from ray.exceptions import RaySystemError
 
 
 
-def get_mem_func():
-    try:
-        MEMORY = ray.available_resources()['memory']
-    except ray.exceptions.RaySystemError:
-        ray.init()
-        MEMORY = ray.available_resources()['memory']
-    try:
-        CPUS = ray.available_resources()['CPU']
-        MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
-    except KeyError:
-        # get number of cores
-        import multiprocessing
-        CPUS = multiprocessing.cpu_count()
-        MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
-    MEMORY = int(MEMORY)
-    CPUS   = int(CPUS)
-    MEM_PER_WORKER = int(MEM_PER_WORKER)
-    return MEMORY, CPUS, MEM_PER_WORKER
-
-try:
-	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
-except RaySystemError:
-	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
-
-def smart_parallelize(func): 
-    '''FIRST ARG MUST BE ARG TO BE PARALLELIZED'''
-
-    def wrap(**kwargs): 
-        def f2(**kwargs):
-            par_args = list(kwargs.keys())[:n_args2parallelize]
-            data_par_args = [kwargs[i] for i in par_args]
-
-            results = []
-            for i, _ in enumerate(data_par_args[0]):
-                kwargs_0 = kwargs.copy()
-                for j, _ in enumerate(data_par_args):
-                    kwargs_0[par_args[j]] = data_par_args[j][i]
-                r = func(**kwargs_0)
-                results.append(r)
-            return results
-        @ray.remote(memory=MEM_PER_WORKER)
-        def get_results(**kwargs):
-            try:
-                args_names = ray.get(args_names_put)
-                args_vals  = ray.get(args_vals_put)
-                kwargs2 = dict(zip(args_names, args_vals))
-                kwargs.update(kwargs2)
-            except NameError:
-                pass
-            results = f2(**kwargs)
-            return results
+# def get_mem_func():
+#     try:
+#         MEMORY = ray.available_resources()['memory']
+#     except ray.exceptions.RaySystemError:
+#         ray.init()
+#         MEMORY = ray.available_resources()['memory']
+#     try:
+#         CPUS = ray.available_resources()['CPU']
+#         MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
+#     except KeyError:
+#         # get number of cores
+#         import multiprocessing
+#         CPUS = multiprocessing.cpu_count()
+#         MEM_PER_WORKER = (MEMORY / CPUS) * 0.8
+#     MEMORY = int(MEMORY)
+#     CPUS   = int(CPUS)
+#     MEM_PER_WORKER = int(MEM_PER_WORKER)
+#     return MEMORY, CPUS, MEM_PER_WORKER
+
+# try:
+# 	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
+# except RaySystemError:
+# 	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
+
+# def smart_parallelize(func): 
+#     '''FIRST ARG MUST BE ARG TO BE PARALLELIZED'''
+
+#     def wrap(**kwargs): 
+#         def f2(**kwargs):
+#             par_args = list(kwargs.keys())[:n_args2parallelize]
+#             data_par_args = [kwargs[i] for i in par_args]
+
+#             results = []
+#             for i, _ in enumerate(data_par_args[0]):
+#                 kwargs_0 = kwargs.copy()
+#                 for j, _ in enumerate(data_par_args):
+#                     kwargs_0[par_args[j]] = data_par_args[j][i]
+#                 r = func(**kwargs_0)
+#                 results.append(r)
+#             return results
+#         @ray.remote(memory=MEM_PER_WORKER)
+#         def get_results(**kwargs):
+#             try:
+#                 args_names = ray.get(args_names_put)
+#                 args_vals  = ray.get(args_vals_put)
+#                 kwargs2 = dict(zip(args_names, args_vals))
+#                 kwargs.update(kwargs2)
+#             except NameError:
+#                 pass
+#             results = f2(**kwargs)
+#             return results
         
-        try:
-            n_args2parallelize = kwargs['n_args2parallelize']
-            # delete n_args2parallelize from kwargs
-            del kwargs['n_args2parallelize']
-        except KeyError:
-            n_args2parallelize = 1
-
-        par_args = list(kwargs.keys())[:n_args2parallelize]
-        arg2parallelize_unsplit = [kwargs[i] for i in par_args]
-
-        # split into CPUS chunks
-        arg2parallelize = [np.array_split(i, CPUS) for i in arg2parallelize_unsplit]
-
-        arg_names = list(kwargs.keys())[n_args2parallelize:]
-        arg_vals  = list(kwargs.values())[n_args2parallelize:]
-
-        if len(arg_names) != 0:
-            args_names_put = ray.put(arg_names)
-            args_vals_put  = ray.put(arg_vals)
-
-        workers = []
-        for i in range(len(arg2parallelize[0])):
-            if len(arg2parallelize[0][i]) == 0:
-                continue
-            # par_arg    = {list(kwargs.keys())[0]:arg2parallelize[i]}
-            par_arg = {}
-            for j in range(len(par_args)):
-                par_arg[par_args[j]] = arg2parallelize[j][i]
-            workers.append(get_results.remote(**par_arg))
-        result = ray.get(workers)
-
-        r_test = result[0][0]
-        if isinstance(r_test, tuple):
-            n_outputs = len(r_test)
-        else:
-            n_outputs = 1
-
-        results = []
-        for i in range(n_outputs):
-            results.append([])
-        for j in range(len(result)):
-            for output in result[j]:
-                if n_outputs > 1:
-                    for k in range(n_outputs):
-                        results[k].append(output[k])
-                else:
-                    results[0].append(output)
-
-        return results
-    return wrap 
-
-
-if __name__ == "__main__":
-    import timeit
-    from scipy.integrate import quad
-
-    @smart_parallelize
-    def func(x):
-        return x
+#         try:
+#             n_args2parallelize = kwargs['n_args2parallelize']
+#             # delete n_args2parallelize from kwargs
+#             del kwargs['n_args2parallelize']
+#         except KeyError:
+#             n_args2parallelize = 1
+
+#         par_args = list(kwargs.keys())[:n_args2parallelize]
+#         arg2parallelize_unsplit = [kwargs[i] for i in par_args]
+
+#         # split into CPUS chunks
+#         arg2parallelize = [np.array_split(i, CPUS) for i in arg2parallelize_unsplit]
+
+#         arg_names = list(kwargs.keys())[n_args2parallelize:]
+#         arg_vals  = list(kwargs.values())[n_args2parallelize:]
+
+#         if len(arg_names) != 0:
+#             args_names_put = ray.put(arg_names)
+#             args_vals_put  = ray.put(arg_vals)
+
+#         workers = []
+#         for i in range(len(arg2parallelize[0])):
+#             if len(arg2parallelize[0][i]) == 0:
+#                 continue
+#             # par_arg    = {list(kwargs.keys())[0]:arg2parallelize[i]}
+#             par_arg = {}
+#             for j in range(len(par_args)):
+#                 par_arg[par_args[j]] = arg2parallelize[j][i]
+#             workers.append(get_results.remote(**par_arg))
+#         result = ray.get(workers)
+
+#         r_test = result[0][0]
+#         if isinstance(r_test, tuple):
+#             n_outputs = len(r_test)
+#         else:
+#             n_outputs = 1
+
+#         results = []
+#         for i in range(n_outputs):
+#             results.append([])
+#         for j in range(len(result)):
+#             for output in result[j]:
+#                 if n_outputs > 1:
+#                     for k in range(n_outputs):
+#                         results[k].append(output[k])
+#                 else:
+#                     results[0].append(output)
+
+#         return results
+#     return wrap 
+
+
+# if __name__ == "__main__":
+#     import timeit
+#     from scipy.integrate import quad
+
+#     @smart_parallelize
+#     def func(x):
+#         return x
     
-    x = np.ones((30,2))
-    y = np.ones((30,))*2
-    # y = 2
-    start  = timeit.default_timer()
-    answer = func(x=x)
-    stop  = timeit.default_timer()
-    print(stop - start)
-    print(answer)
-
-
-    # start  = timeit.default_timer()
-    # answer = []
-    # for i, val in enumerate(x):
-    #     sleep(1)
-    #     answer.append(val+y)
-    # stop = timeit.default_timer()
-    # print(stop - start)
+#     x = np.ones((30,2))
+#     y = np.ones((30,))*2
+#     # y = 2
+#     start  = timeit.default_timer()
+#     answer = func(x=x)
+#     stop  = timeit.default_timer()
+#     print(stop - start)
+#     print(answer)
+
+
+#     # start  = timeit.default_timer()
+#     # answer = []
+#     # for i, val in enumerate(x):
+#     #     sleep(1)
+#     #     answer.append(val+y)
+#     # stop = timeit.default_timer()
+#     # print(stop - start)
```

### Comparing `smart_parallelize-2.2.0/smart_parallelize/parallelize_native.py` & `smart_parallelize-2.2.1/smart_parallelize/parallelize_native.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from multiprocessing import Pool
 from time import sleep
 
 
-print('testing')
-sleep(1)
+# print('testing')
+# sleep(1)
 
 def smart_parallelize(func, args2parallelize, *args):
     args2par = list(args[:args2parallelize])
     argsnotpar = [list(args[args2parallelize:])*len(args2par[0])]
     if len(argsnotpar[0]) != 0:
         inputs = zip(*args2par, *argsnotpar)
     else:
```

### Comparing `smart_parallelize-2.2.0/PKG-INFO` & `smart_parallelize-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.2.0
+Version: 2.2.1
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

