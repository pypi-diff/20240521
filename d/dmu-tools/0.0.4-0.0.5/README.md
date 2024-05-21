# Comparing `tmp/dmu_tools-0.0.4.tar.gz` & `tmp/dmu_tools-0.0.5.tar.gz`

## Comparing `dmu_tools-0.0.4.tar` & `dmu_tools-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/Readme.md
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/test.ipynb
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/src/dmu_tools/__init__.py
--rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/src/dmu_tools/data_filter.py
--rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/src/dmu_tools/data_generator.py
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/src/dmu_tools/dmu.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/src/dmu_tools/tools.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/tests/test.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/README.md
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dmu_tools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/Readme.md
+-rw-r--r--   0        0        0   128925 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/TSD.lst
+-rw-r--r--   0        0        0  9453312 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/TSD_FCR_1_SOL
+-rw-r--r--   0        0        0 10392871 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/data.txt
+-rw-r--r--   0        0        0   570872 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/ebv.csv
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/test.ipynb
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/dmu_tools/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/dmu_tools/aic.py
+-rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/dmu_tools/data_filter.py
+-rw-r--r--   0        0        0    27161 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/dmu_tools/data_generator.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/dmu_tools/dmu.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/dmu_tools/draw_heritability.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/src/dmu_tools/tools.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 dmu_tools-0.0.5/PKG-INFO
```

### Comparing `dmu_tools-0.0.4/src/dmu_tools/data_filter.py` & `dmu_tools-0.0.5/src/dmu_tools/data_filter.py`

 * *Files identical despite different names*

### Comparing `dmu_tools-0.0.4/src/dmu_tools/data_generator.py` & `dmu_tools-0.0.5/src/dmu_tools/data_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from scipy import stats
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder
 import time
 
 # 数据处理
-
 class Data_Generator:
     def __init__(self, daily_data):
 
         self.raw_data = daily_data.copy()
         self.daily_data = self.get_daily_data()
         print("daily_data shape: ", self.daily_data.shape)
         self.id_encoder = self.get_id_encoder()
```

### Comparing `dmu_tools-0.0.4/src/dmu_tools/dmu.py` & `dmu_tools-0.0.5/src/dmu_tools/dmu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 import os
 from scipy.stats import pearsonr
+from .draw_heritability import draw_heritability as dh
 
 
 def read_sol(dir_sol):
     sol = pd.read_csv(dir_sol, header=None)[0].str.split(expand=True)
     sol.columns = sol.columns + 1
     return sol
 
@@ -24,16 +25,16 @@
 def cal_bv_cor(predict: dict, data: pd.DataFrame, pedigree: pd.DataFrame):
     """计算遗传力相关系数
     Args:
         predict (dict): 预测的个体与表型的对应字典
         data (pd.DataFrame): 原始数据，用来跑动物模型，最后一行为表型
         pedigree (pd.DataFrame): 家系
 
-        Returns:
-            float: 相关系数
+    Returns:
+        float: 相关系数
     """
     # 生成替换数据
     pre_data = get_replace_data(predict, data)
     # 运行
     try:
         pre_bv = cal_bv_ani(predict.keys(), pre_data, pedigree)
         ori_bv = cal_bv_ani(predict.keys(), data, pedigree)
@@ -69,15 +70,15 @@
     data["predict"] = data["id"].map(predict)
     data["predict"] = data["predict"].fillna(pheno)
     # 删除phenotype列
     data = data.drop(columns=[pheno.name])
     return data
 
 
-# 动物模型计算遗传力
+# 动物模型计算育种值
 def cal_bv_ani(target_ids: list, data, pedigree) -> dict:
     # 运行
     run_ani(data, pedigree)
     # 读取结果
     breeding_effects = get_breeding_effects(write_ani_dir() + ".sol")
     # 选取目标
     bv = {k: breeding_effects[k] for k in target_ids}
@@ -102,26 +103,36 @@
     pedigree.to_csv("ped.txt", sep=" ", index=False, header=False)
     os.system("run_dmuai.bat TSD")
 
 
 # 删除dmu生成文件
 def clean_dmu_files(excepts=[]):
     # 根据后缀删除
-    d_drop = [".SOL", ".log", ".LLIK", ".lst", ".PAROUT", ".RESIDUAL", ".PAROUT_STD", "data.txt", "ped.txt"]
+    d_drop = [
+        ".SOL",
+        ".log",
+        ".LLIK",
+        ".lst",
+        ".PAROUT",
+        ".RESIDUAL",
+        ".PAROUT_STD",
+        "data.txt",
+        "ped.txt",
+    ]
     for except_ in excepts:
         d_drop.remove(except_)
     for root, dirs, files in os.walk("./"):
         for file in files:
             for d in d_drop:
                 if file.endswith(d):
                     os.remove(os.path.join(root, file))
 
 
 # 生成动物模型的DIR文件
-def write_ani_dir(DIR="AAAAAAA"):
+def write_ani_dir(DIR="ANI"):
     try:
         os.system.remove(DIR + ".DIR")
     except:
         pass
     COMMENT = "\n"
     ANALYSE = "1 1 0 1"
     DATA = "ASCII (3,1,-999) ./data.txt"
@@ -171,82 +182,161 @@
         f.write(DMUAI_1 + "\n")
         f.write(DMUAI_2 + "\n")
         f.write(DMUAI_3 + "\n")
         f.write(DMUAI_4 + "\n")
         f.write(DMUAI_5 + "\n")
     return DIR
 
+
 # 计算遗传力
-def cal_bv(dir_lst:str ) -> float:
+def cal_bv(dir_lst: str) -> float:
     # 读取dir文件
     with open(dir_lst, "r") as f:
         # 出现 FINAL PARAMETERS ESTIMATED 之后
         # 出现 Covariance matrix for random effect no:            1
         pass
 
 
 # 测定日
-
 import pandas as pd
 import numpy as np
 import os
+from .aic import calculate_AIC
 from scipy.stats import pearsonr
 
-class testday_sol_reader:
 
-    def __init__(self, dir_sol, dir_data, id_index) -> None:
+class TestDay:
+    """测定日sol文件读取器"""
+
+    def __init__(
+        self,
+        dir_sol: str,
+        dir_lst: str,
+        dir_data: str,
+        id_index: int,
+        start_day: int,
+        end_day: int,
+    ) -> None:
         """
         :param dir_sol: sol文件路径
+        :param dir_lst: lst文件路径
         :param dir_data: data文件路径
         :param id_index: 个体号在data中在第几列
+        :param start_day: 开始时间
+        :param end_day: 结束时间
         """
-
         self.dir_sol = dir_sol
+        self.dir_lst = dir_lst
         self.dir_data = dir_data
         self.id_index = id_index
+        self.start_day = start_day
+        self.end_day = end_day
 
-        self.sol = self.read_sol()
-        self.data = self.read_data()
+        self.sol = self.__read_sol()
+        self.data = self.__read_data()
         self.effect_values = []
 
-    def read_sol(self):
+    def __read_sol(self):
         sol = pd.read_csv(self.dir_sol, header=None)
         # 使用str.split()函数分割数据并扩展成多列
         sol[["1", "2", "阶数", "4", "个体号", "6", "7", "8", "9"]] = sol[0].str.split(
             expand=True
         )
         sol = sol.drop(0, axis=1)
         sol = sol[sol["1"] == "4"]
         return sol
 
-    def read_data(self):
+    def __read_data(self):
         data = pd.read_csv(self.dir_data, header=None, sep=" ")
         return data
 
     def calculate_ebv(self):
-
+        """计算EBV
+        :return ebv: dict
+        """
         # 每个阶数上每个个体的sol列
         effect_values = {}
         for degree, group in self.sol.groupby("阶数"):
             # 获取该阶数的sol列值并创建DataFrame
             effect_value = group[["个体号", "8"]]
             # 将DataFrame添加到字典中
             effect_values[degree] = effect_value
-
-
         ebv = {}
         for id in self.data[self.id_index].unique():
             ebv[id] = 0
+        for degree in range(1, self.sol["阶数"].astype(int).max() + 1):
+            # 此阶数所有个体各个时间上的log值
+            log_value = {}
+            for id, group in self.data.groupby(by=self.id_index):
+                log_value[id] = list(group[self.id_index + degree])
+            # 累加EBV
+            for id in self.data[self.id_index].unique():
+                effect_value = effect_values[str(degree)]
 
+                effect_value_filtered = effect_value[effect_value["个体号"] == str(id)][
+                    "8"
+                ]
+                if not effect_value_filtered.empty:
+                    effect_value = float(effect_value_filtered.iloc[0])
+                else:
+                    print("The dataframe didn't match the filtering criteria.")
+                ebv[id] += (pd.Series(log_value[id]) * effect_value).mean()
+                # ebv[id] += effect_value
+        # 将ebv转换为DataFrame
+        ebv = pd.DataFrame(pd.Series(ebv), columns=["EBV"])
+        ebv.index.name = "ID"
+        ebv.to_csv("ebv.csv")
+        return ebv
+    
+    def calculate_se(self):
+        """
+        计算标准误差
+        :return: se: dict
+        """
+        # 每个阶数上每个个体的sol列
+        effect_values = {}
+        for degree, group in self.sol.groupby("阶数"):
+            # 获取该阶数的sol列值并创建DataFrame
+            effect_value = group[["个体号", "9"]]
+            # 将DataFrame添加到字典中
+            effect_values[degree] = effect_value
+        ebv = {}
+        for id in self.data[self.id_index].unique():
+            ebv[id] = 0
         for degree in range(1, self.sol["阶数"].astype(int).max() + 1):
-            print(degree)
             # 此阶数所有个体各个时间上的log值
             log_value = {}
             for id, group in self.data.groupby(by=self.id_index):
                 log_value[id] = list(group[self.id_index + degree])
             # 累加EBV
             for id in self.data[self.id_index].unique():
                 effect_value = effect_values[str(degree)]
-                effect_value = float(effect_value[effect_value["个体号"] == str(id)]["8"])
+
+                effect_value_filtered = effect_value[effect_value["个体号"] == str(id)][
+                    "8"
+                ]
+                if not effect_value_filtered.empty:
+                    effect_value = float(effect_value_filtered.iloc[0])
+                else:
+                    print("The dataframe didn't match the filtering criteria.")
                 ebv[id] += (pd.Series(log_value[id]) * effect_value).mean()
                 # ebv[id] += effect_value
-        return ebv
+        # 将ebv转换为DataFrame
+        ebv = pd.DataFrame(pd.Series(ebv), columns=["EBV"])
+        ebv.index.name = "ID"
+        ebv.to_csv("ebv.csv")
+        return ebv
+
+    def draw_heritability(self):
+        """画遗传力图"""
+        dh(self.start_day, self.end_day, self.dir_lst)
+
+    def calculate_AIC(self):
+        """计算AIC"""
+        return calculate_AIC(self.dir_lst)
+
+    def analyse(self):
+        """分析"""
+        self.calculate_ebv()
+        self.draw_heritability()
+        self.calculate_AIC()
+        return "TESTDAY"
```

### Comparing `dmu_tools-0.0.4/LICENSE` & `dmu_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dmu_tools-0.0.4/pyproject.toml` & `dmu_tools-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dmu_tools"
-version = "0.0.4"
-authors = [
-  { name="Di Pan", email="994485784@qq.com" },
-]
+version = "0.0.5"
 description = "Tools for DMU"
 readme = "README.md"
 requires-python = ">=3.7"
+license = { text = "MIT License" }
+authors = [
+  { name = "Di Pan", email = "994485784@qq.com" }
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: OS Independent"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+Homepage = "https://github.com/pypa/sampleproject"
+"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

