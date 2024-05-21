# Comparing `tmp/virgo_modules-0.0.86.tar.gz` & `tmp/virgo_modules-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.86.tar", last modified: Thu May 16 12:04:14 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.87.tar", last modified: Tue May 21 14:13:26 2024, max compression
```

## Comparing `virgo_modules-0.0.86.tar` & `virgo_modules-0.0.87.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.888759 virgo_modules-0.0.86/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.86/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-05-16 12:04:14.886786 virgo_modules-0.0.86/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.86/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:04:14.889760 virgo_modules-0.0.86/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-05-16 10:57:12.000000 virgo_modules-0.0.86/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.743499 virgo_modules-0.0.86/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.796500 virgo_modules-0.0.86/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.878683 virgo_modules-0.0.86/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    71603 2024-05-13 19:18:08.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.825497 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-16 12:04:14.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.835959 virgo_modules-0.0.87/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.87/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-05-21 14:13:26.826506 virgo_modules-0.0.87/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.87/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:13:26.835959 virgo_modules-0.0.87/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-05-21 14:13:11.000000 virgo_modules-0.0.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.754350 virgo_modules-0.0.87/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.774359 virgo_modules-0.0.87/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.822508 virgo_modules-0.0.87/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    72002 2024-05-21 14:13:11.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.789400 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.86/LICENSE` & `virgo_modules-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.86/PKG-INFO` & `virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo_modules
-Version: 0.0.86
+Name: virgo-modules
+Version: 0.0.87
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.86/setup.py` & `virgo_modules-0.0.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.86",
+    version="0.0.87",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.86/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.87/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.86/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.87/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.86/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.87/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.86/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.87/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1024,15 +1024,14 @@
 
         states = list(df.hmm_feature.unique())
         states.sort()
         states_subtitles = [f'state {x}' for x in states]
         if len(states_subtitles)%2 == 1:
             states_subtitles = states_subtitles + [None]
 
-
         fig = make_subplots(
             rows= rows_subplot, cols=2,
             specs = [[{"type": "scatter"},{"type": "scatter"}]]*state_rows,
             vertical_spacing = 0.02, horizontal_spacing = 0.02,
             subplot_titles =  states_subtitles )
 
         ### only states scaled series
@@ -1103,14 +1102,19 @@
         fig.update_xaxes(title_text='State To', row=row_i, col=2)
         fig.update_yaxes(title_text='State From', row=row_i, col=2)
 
         ## returns of state
         df_ = df[['Date','hmm_feature','Close',"chain_return"]].sort_values('Date')
         df_['Daily_Returns'] = df['Close'].pct_change(7)
 
+        df_agg_returns = df_.groupby('hmm_feature', as_index = False).agg(median =('Daily_Returns','median')).copy()
+        current_state = df_.iloc[-1,:].hmm_feature
+        medain_state_return = df_agg_returns[ df_agg_returns.hmm_feature == current_state]['median'].values[0]
+        type_state = 'low state' if medain_state_return < 0 else 'high state'
+
         for state in states:
             dfi = df_[df_.hmm_feature == state]
             fig.add_trace(go.Box(y = dfi.chain_return, name=str(state),showlegend=False, marker_color = color_map[state] ),row=1, col=1)
 
         ## lengths chains by state dist
         if 'hmm_chain_order' in df.columns:
             df_agg = df.groupby(['hmm_feature','chain_id'],as_index = False).agg(length_by_chain = ('hmm_chain_order','max'))
@@ -1147,28 +1151,28 @@
             importances_df = importances_df.sort_values('median', ascending = False)
 
             for feature in importances_df.feature.unique():
                 dfi = importances_df[importances_df.feature == feature]
                 fig.add_trace(go.Box(x = dfi.importance, name=str(feature),showlegend=False ),row=2, col=2)
             fig.update_yaxes(visible=False, title="feature",row=2, col=2)
 
-        
         fig.update_layout(height=height_plot, width=1600, title_text = f'State model analysis: {self.ticket_name}', coloraxis=dict(colorbar_len=0.50))
 
         date_execution = datetime.datetime.today().strftime('%Y-%m-%d')
         current_step = df.iloc[-1,:].hmm_chain_order
         current_state = df.iloc[-1,:].hmm_feature
         message1 = str(current_state)
         message2 = str(current_step)
         message3 = str(date_execution)
 
         messages = {
             'current state':message1,
             'current step in state': message2,
             'execution date':message3,
+            'type state':type_state,
         }
         
         if self.show_plot:
             fig.show()
             print('---------------------------------------------------')
             print('------------------ strategy -----------------------')
             print('---------------------------------------------------')
@@ -1192,14 +1196,15 @@
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+'market_message.json',input_path = self.save_path+"market_message.json")
             
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + 'market_message.json', input_path = self.save_path + 'market_message.json', aws_credentials = self.aws_credentials)
         
         if self.return_figs:
             return fig, messages
+        
     def produce_forecasting_plot(self,predictions):
         """
         display forecasting plots
 
         Parameters
         ----------
         predictions (pd.DataFrame): asset predictions
```

### Comparing `virgo_modules-0.0.86/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.87/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.87/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo-modules
-Version: 0.0.86
+Name: virgo_modules
+Version: 0.0.87
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

