# Comparing `tmp/qtmodel-0.3.5.tar.gz` & `tmp/qtmodel-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.3.5.tar", last modified: Mon May 20 02:54:00 2024, max compression
+gzip compressed data, was "qtmodel-0.3.7.tar", last modified: Mon May 20 06:57:26 2024, max compression
```

## Comparing `qtmodel-0.3.5.tar` & `qtmodel-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 02:54:00.705455 qtmodel-0.3.5/
--rw-rw-rw-   0        0        0    37701 2024-05-20 02:54:00.704149 qtmodel-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 02:54:00.697132 qtmodel-0.3.5/qtmodel/
--rw-rw-rw-   0        0        0       91 2024-05-17 07:08:34.000000 qtmodel-0.3.5/qtmodel/__init__.py
--rw-rw-rw-   0        0        0      443 2024-05-20 02:17:18.000000 qtmodel-0.3.5/qtmodel/qt_db.py
--rw-rw-rw-   0        0        0     2386 2024-05-20 02:22:27.000000 qtmodel-0.3.5/qtmodel/qt_helper.py
--rw-rw-rw-   0        0        0    83069 2024-05-20 02:31:09.000000 qtmodel-0.3.5/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     8827 2024-05-17 07:53:59.000000 qtmodel-0.3.5/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0    14370 2024-05-20 02:45:48.000000 qtmodel-0.3.5/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-20 02:54:00.702770 qtmodel-0.3.5/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37701 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 02:54:00.705455 qtmodel-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-20 02:53:48.000000 qtmodel-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:57:26.306322 qtmodel-0.3.7/
+-rw-rw-rw-   0        0        0    41207 2024-05-20 06:57:26.305232 qtmodel-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    40779 2024-05-20 06:56:31.000000 qtmodel-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 06:57:26.296803 qtmodel-0.3.7/qtmodel/
+-rw-rw-rw-   0        0        0       91 2024-05-17 07:08:34.000000 qtmodel-0.3.7/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0      443 2024-05-20 02:17:18.000000 qtmodel-0.3.7/qtmodel/qt_db.py
+-rw-rw-rw-   0        0        0     2386 2024-05-20 02:22:27.000000 qtmodel-0.3.7/qtmodel/qt_helper.py
+-rw-rw-rw-   0        0        0    82991 2024-05-20 06:47:40.000000 qtmodel-0.3.7/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     9615 2024-05-20 06:55:32.000000 qtmodel-0.3.7/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0    14370 2024-05-20 02:45:48.000000 qtmodel-0.3.7/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:57:26.303157 qtmodel-0.3.7/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    41207 2024-05-20 06:57:25.000000 qtmodel-0.3.7/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 06:57:26.000000 qtmodel-0.3.7/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:57:25.000000 qtmodel-0.3.7/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 06:57:26.000000 qtmodel-0.3.7/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:57:26.306322 qtmodel-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-20 06:16:02.000000 qtmodel-0.3.7/setup.py
```

### Comparing `qtmodel-0.3.5/PKG-INFO` & `qtmodel-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,87 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.5
+Version: 0.3.7
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-##  初始化模型
+# 最新版本 V0.3.7 - 2024.05.20 
+- 优化部分调用
+##  项目管理
 ### initial
-初始化模型
+初始化模型,新建模型
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.initial()
 ```  
+### open_file
+打开bfmd文件
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.open_file("a.bfmd")
+```  
+### save_file
+保存bfmd文件
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.save_file("a.bfmd")
+```  
+### close_project
+关闭项目
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.close_project()
+```  
+### import_command
+导入命令
+> 参数:  
+> command:命令字符  
+> command_type:命令类型 1-桥通命令  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_command("*SECTION")
+```  
+### export_file
+导入命令
+> 参数:  
+> file_path:导出文件(.mct/.qdat/.PGF/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.export_file("a.mct")
+```  
+### import_file
+导入命令
+> 参数:  
+> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_file("a.mct")
+```  
+### do_solve
+运行分析
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.do_solve()
+```  
 ##  节点单元操作
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
 ```Python
@@ -617,15 +675,15 @@
 > _规范:1-公规 2-铁规_  
 > _张拉方式:1-一次张拉 2-超张拉_  
 > _松弛类型：1-一般松弛 2-低松弛_  
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.add_tendon_property(name="钢束1",tendon_type="先张",material_id=1,duct_type=1,steel_type=1,
+mdb.add_tendon_property(name="钢束1",tendon_type=0,material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=(1,1,1))
 ```  
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
 > property_name:钢束特性名称  
@@ -786,14 +844,16 @@
 > load_type:荷载类型  
 > _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
 > coord_system:坐标系  
 > _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
 > group_name:荷载组名  
+> load_bias:偏心荷载 (是否偏心,0-中心 1-偏心,偏心坐标系-int,偏心距离)  
+> projected:是否投影  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
@@ -1038,16 +1098,14 @@
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_case(index=1)
 mdb.remove_load_case(name="工况1")
 mdb.remove_load_case()
 ```  
-### test_print
-测试运行
 ##  施工阶段
 ### add_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
@@ -1132,11 +1190,74 @@
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
+```
+## 结果提取
+### get_element_stress
+获取单元应力,支持单个单元和单元列表
+> 参数:  
+> element_id: 单元编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_element_stress(1,stage_id=1)
+odb.get_element_stress([1,2,3],stage_id=1)
+odb.get_element_stress(1,operation=True,case_name="工况名")
+```  
+### get_element_force
+获取单元内力,支持单个单元和单元列表
+> 参数:  
+> element_id: 单元编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_element_force(1,stage_id=1)
+odb.get_element_force([1,2,3],stage_id=1)
+odb.get_element_force(1,operation=True,case_name="工况名")
+```  
+### get_reaction
+获取节点,支持单个节点和节点列表
+> 参数:  
+> node_id: 节点编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_reaction(1,stage_id=1)
+odb.get_reaction([1,2,3],stage_id=1)
+odb.get_reaction(1,operation=True,case_name="工况名")
+```  
+### get_node_displacement
+获取节点,支持单个节点和节点列表
+> 参数:  
+> node_id: 节点号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_node_displacement(1,stage_id=1)
+odb.get_node_displacement([1,2,3],stage_id=1)
+odb.get_node_displacement(1,operation=True,case_name="工况名")
 ```  
 
-
-
```

### Comparing `qtmodel-0.3.5/README.md` & `qtmodel-0.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,73 @@
-##  初始化模型
+# 最新版本 V0.3.7 - 2024.05.20 
+- 优化部分调用
+##  项目管理
 ### initial
-初始化模型
+初始化模型,新建模型
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.initial()
 ```  
+### open_file
+打开bfmd文件
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.open_file("a.bfmd")
+```  
+### save_file
+保存bfmd文件
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.save_file("a.bfmd")
+```  
+### close_project
+关闭项目
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.close_project()
+```  
+### import_command
+导入命令
+> 参数:  
+> command:命令字符  
+> command_type:命令类型 1-桥通命令  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_command("*SECTION")
+```  
+### export_file
+导入命令
+> 参数:  
+> file_path:导出文件(.mct/.qdat/.PGF/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.export_file("a.mct")
+```  
+### import_file
+导入命令
+> 参数:  
+> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_file("a.mct")
+```  
+### do_solve
+运行分析
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.do_solve()
+```  
 ##  节点单元操作
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
 ```Python
@@ -603,15 +661,15 @@
 > _规范:1-公规 2-铁规_  
 > _张拉方式:1-一次张拉 2-超张拉_  
 > _松弛类型：1-一般松弛 2-低松弛_  
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.add_tendon_property(name="钢束1",tendon_type="先张",material_id=1,duct_type=1,steel_type=1,
+mdb.add_tendon_property(name="钢束1",tendon_type=0,material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=(1,1,1))
 ```  
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
 > property_name:钢束特性名称  
@@ -772,14 +830,16 @@
 > load_type:荷载类型  
 > _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
 > coord_system:坐标系  
 > _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
 > group_name:荷载组名  
+> load_bias:偏心荷载 (是否偏心,0-中心 1-偏心,偏心坐标系-int,偏心距离)  
+> projected:是否投影  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
@@ -1024,16 +1084,14 @@
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_case(index=1)
 mdb.remove_load_case(name="工况1")
 mdb.remove_load_case()
 ```  
-### test_print
-测试运行
 ##  施工阶段
 ### add_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
@@ -1118,9 +1176,73 @@
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
-```  
-
+```
+## 结果提取
+### get_element_stress
+获取单元应力,支持单个单元和单元列表
+> 参数:  
+> element_id: 单元编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_element_stress(1,stage_id=1)
+odb.get_element_stress([1,2,3],stage_id=1)
+odb.get_element_stress(1,operation=True,case_name="工况名")
+```  
+### get_element_force
+获取单元内力,支持单个单元和单元列表
+> 参数:  
+> element_id: 单元编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_element_force(1,stage_id=1)
+odb.get_element_force([1,2,3],stage_id=1)
+odb.get_element_force(1,operation=True,case_name="工况名")
+```  
+### get_reaction
+获取节点,支持单个节点和节点列表
+> 参数:  
+> node_id: 节点编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_reaction(1,stage_id=1)
+odb.get_reaction([1,2,3],stage_id=1)
+odb.get_reaction(1,operation=True,case_name="工况名")
+```  
+### get_node_displacement
+获取节点,支持单个节点和节点列表
+> 参数:  
+> node_id: 节点号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_node_displacement(1,stage_id=1)
+odb.get_node_displacement([1,2,3],stage_id=1)
+odb.get_node_displacement(1,operation=True,case_name="工况名")
+```
```

### Comparing `qtmodel-0.3.5/qtmodel/qt_helper.py` & `qtmodel-0.3.7/qtmodel/qt_helper.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.5/qtmodel/qt_mdb.py` & `qtmodel-0.3.7/qtmodel/qt_mdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,14 @@
     """
     Mdb类负责建模相关操作
     """
 
     def __int__(self):
         self.initial()
 
-    # region 获取模型信息
-    @staticmethod
-    def get_app_stage():
-        return qt_model.GetApplicationStage()
-
-    # endregion
-
     # region 项目管理
     @staticmethod
     def initial():
         """
         初始化模型,新建模型
         example:
                 mdb.initial()
@@ -75,27 +68,27 @@
     @staticmethod
     def export_file(file_path: str):
         """
             导入命令
             Args:
                 file_path:导出文件(.mct/.qdat/.PGF/.3dx)
             example:
-                qt_model.ExportFile("a.mct")
+                mdb.export_file("a.mct")
             Returns: 无
         """
         qt_model.ExportFile(file_path)
 
     @staticmethod
     def import_file(file_path: str):
         """
             导入命令
             Args:
                 file_path:导入文件(.mct/.qdat/.dxf/.3dx)
             example:
-                qt_model.ImportFile("a.mct")
+                mdb.import_file("a.mct")
             Returns: 无
         """
         qt_model.ImportFile(file_path)
 
     @staticmethod
     def do_solve():
         """
@@ -245,17 +238,17 @@
         """
         if node_ids is None and ele_type != 4:
             raise Exception("操作错误,请输入此单元所需节点列表,[i,j]")
         if node_ids is None and ele_type == 4:
             raise Exception("操作错误,请输入此板单元所需节点列表,[i,j,k,l]")
         if ele_type == 1:
             qt_model.AddBeam(id=index, idI=node_ids[0], idJ=node_ids[1], betaAngle=beta_angle, materialId=mat_id, sectionId=sec_id)
-        elif index == 2:
+        elif ele_type == 2:
             qt_model.AddCable(id=index, idI=node_ids[0], idJ=node_ids[1], betaAngle=beta_angle, materialId=mat_id, sectionId=sec_id)
-        elif sec_id == 3:
+        elif ele_type == 3:
             qt_model.AddLink(id=index, idI=node_ids[0], idJ=node_ids[1], betaAngle=beta_angle, materialId=mat_id, sectionId=sec_id)
         else:
             qt_model.AddPlate(id=index, idI=node_ids[0], idJ=node_ids[1], idK=node_ids[2], idL=node_ids[3], betaAngle=beta_angle,
                               materialId=mat_id,
                               sectionId=sec_id)
 
     @staticmethod
@@ -295,14 +288,16 @@
             mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
             mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
         Returns: 无
         """
         list_material = ["混凝土", "钢材", "预应力", "钢丝", "钢筋", "自定义"]
         if material_type not in list_material:
             raise Exception(f"操作错误,material_type不在指定列表:{list_material}中")
+        if material_type == "自定义":
+            modified = True
         if modified and len(data_info) != 4:
             raise Exception("操作错误,modify_info数据无效!")
         if not modified:
             qt_model.AddMaterial(id=index, name=name, materialType=material_type, standardName=standard,
                                  database=database, constructFactor=construct_factor, isModified=modified)
         else:
             qt_model.AddMaterial(id=index, name=name, materialType=material_type, standardName=standard,
```

### Comparing `qtmodel-0.3.5/qtmodel/qt_odb.py` & `qtmodel-0.3.7/qtmodel/qt_odb.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,18 @@
         Args:
             element_id: 单元编号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
+        example:
+            odb.get_element_stress(1,stage_id=1)
+            odb.get_element_stress([1,2,3],stage_id=1)
+            odb.get_element_stress(1,operation=True,case_name="工况名")
         Returns:
             list[ElementStress] or ElementStress
         """
         if type(element_id) != int and type(element_id) != list:
             raise TypeError("类型错误,element_id仅支持 int和 list[int]")
         bf_list = qt_model.GetElementStress(element_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
@@ -62,14 +66,18 @@
         Args:
             element_id: 单元编号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
+        example:
+            odb.get_element_force(1,stage_id=1)
+            odb.get_element_force([1,2,3],stage_id=1)
+            odb.get_element_force(1,operation=True,case_name="工况名")
         Returns:
             list[ElementForce] or ElementForce
         """
         if type(element_id) != int and type(element_id) != list:
             raise TypeError("类型错误,element_id仅支持 int和 list[int]")
         bf_list = qt_model.GetElementForce(element_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
@@ -101,14 +109,18 @@
         Args:
             node_id: 节点编号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
+        example:
+            odb.get_reaction(1,stage_id=1)
+            odb.get_reaction([1,2,3],stage_id=1)
+            odb.get_reaction(1,operation=True,case_name="工况名")
         Returns:
             list[SupportReaction] or SupportReaction
         """
         if type(node_id) != int and type(node_id) != list:
             raise TypeError("类型错误,beam_id int和 list[int]")
         bs_list = qt_model.GetSupportReaction(node_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
@@ -126,14 +138,18 @@
         Args:
             node_id: 节点号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
+        example:
+            odb.get_node_displacement(1,stage_id=1)
+            odb.get_node_displacement([1,2,3],stage_id=1)
+            odb.get_node_displacement(1,operation=True,case_name="工况名")
         Returns:
             list[NodeDisplacement] or NodeDisplacement
         """
         if type(node_id) != int and type(node_id) != list:
             raise TypeError("类型错误,node_id仅支持 int和 list[int]")
         bf_list = qt_model.GetNodeDisplacement(node_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
```

### Comparing `qtmodel-0.3.5/qtmodel/res_db.py` & `qtmodel-0.3.7/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.5/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.3.7/qtmodel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,87 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.5
+Version: 0.3.7
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-##  初始化模型
+# 最新版本 V0.3.7 - 2024.05.20 
+- 优化部分调用
+##  项目管理
 ### initial
-初始化模型
+初始化模型,新建模型
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.initial()
 ```  
+### open_file
+打开bfmd文件
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.open_file("a.bfmd")
+```  
+### save_file
+保存bfmd文件
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.save_file("a.bfmd")
+```  
+### close_project
+关闭项目
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.close_project()
+```  
+### import_command
+导入命令
+> 参数:  
+> command:命令字符  
+> command_type:命令类型 1-桥通命令  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_command("*SECTION")
+```  
+### export_file
+导入命令
+> 参数:  
+> file_path:导出文件(.mct/.qdat/.PGF/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.export_file("a.mct")
+```  
+### import_file
+导入命令
+> 参数:  
+> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_file("a.mct")
+```  
+### do_solve
+运行分析
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.do_solve()
+```  
 ##  节点单元操作
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
 ```Python
@@ -617,15 +675,15 @@
 > _规范:1-公规 2-铁规_  
 > _张拉方式:1-一次张拉 2-超张拉_  
 > _松弛类型：1-一般松弛 2-低松弛_  
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.add_tendon_property(name="钢束1",tendon_type="先张",material_id=1,duct_type=1,steel_type=1,
+mdb.add_tendon_property(name="钢束1",tendon_type=0,material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=(1,1,1))
 ```  
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
 > property_name:钢束特性名称  
@@ -786,14 +844,16 @@
 > load_type:荷载类型  
 > _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
 > coord_system:坐标系  
 > _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
 > group_name:荷载组名  
+> load_bias:偏心荷载 (是否偏心,0-中心 1-偏心,偏心坐标系-int,偏心距离)  
+> projected:是否投影  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
@@ -1038,16 +1098,14 @@
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_case(index=1)
 mdb.remove_load_case(name="工况1")
 mdb.remove_load_case()
 ```  
-### test_print
-测试运行
 ##  施工阶段
 ### add_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
@@ -1132,11 +1190,74 @@
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
+```
+## 结果提取
+### get_element_stress
+获取单元应力,支持单个单元和单元列表
+> 参数:  
+> element_id: 单元编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_element_stress(1,stage_id=1)
+odb.get_element_stress([1,2,3],stage_id=1)
+odb.get_element_stress(1,operation=True,case_name="工况名")
+```  
+### get_element_force
+获取单元内力,支持单个单元和单元列表
+> 参数:  
+> element_id: 单元编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_element_force(1,stage_id=1)
+odb.get_element_force([1,2,3],stage_id=1)
+odb.get_element_force(1,operation=True,case_name="工况名")
+```  
+### get_reaction
+获取节点,支持单个节点和节点列表
+> 参数:  
+> node_id: 节点编号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_reaction(1,stage_id=1)
+odb.get_reaction([1,2,3],stage_id=1)
+odb.get_reaction(1,operation=True,case_name="工况名")
+```  
+### get_node_displacement
+获取节点,支持单个节点和节点列表
+> 参数:  
+> node_id: 节点号  
+> stage_id: 施工极端号  
+> result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
+> increment_type: 1-全量    2-增量  
+> operation: 是否为运营阶段  
+> case_name: 运营阶段所需荷载工况名  
+```Python
+# 示例代码
+from qtmodel import odb
+odb.get_node_displacement(1,stage_id=1)
+odb.get_node_displacement([1,2,3],stage_id=1)
+odb.get_node_displacement(1,operation=True,case_name="工况名")
 ```  
 
-
-
```

### Comparing `qtmodel-0.3.5/setup.py` & `qtmodel-0.3.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.3.5",
+    version="0.3.7",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

