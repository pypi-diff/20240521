# Comparing `tmp/fuo_qqmusic-1.0.3.tar.gz` & `tmp/fuo_qqmusic-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_qqmusic-1.0.3.tar", last modified: Sun Apr 21 10:31:31 2024, max compression
+gzip compressed data, was "fuo_qqmusic-1.0.4.tar", last modified: Tue May 21 15:48:01 2024, max compression
```

## Comparing `fuo_qqmusic-1.0.3.tar` & `fuo_qqmusic-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/fuo_qqmusic/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23378 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/fuo_qqmusic/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.810260 fuo_qqmusic-1.0.4/fuo_qqmusic/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23472 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/fuo_qqmusic/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/setup.py
```

### Comparing `fuo_qqmusic-1.0.3/PKG-INFO` & `fuo_qqmusic-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo_qqmusic
-Version: 1.0.3
+Version: 1.0.4
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 Keywords: feeluown,plugin,qqmusic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `fuo_qqmusic-1.0.3/README.md` & `fuo_qqmusic-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 ## 使用说明
 
 ### 登录
 在网页登录微信/QQ后（在任意网站），复制请求中的 cookies 至程序登录框，
 [操作示例](https://github.com/feeluown/feeluown-qqmusic/issues/6)。
 
 ## changelog
+### 1.0.4 (2024-05-21)
+- 歌手歌曲排序切换为”按热度排序”
+- 修复推荐歌单接口
+
 ### 1.0.3 (2024-04-21)
 - 适配 feeluown 4.1.3 的新主页功能
 
 ### 1.0.2 (2024-03-04)
 - 修复获取歌单封面失败的问题 #21
 - 修复获取歌曲播放链接失败的问题 #20
```

### Comparing `fuo_qqmusic-1.0.3/fuo_qqmusic/__init__.py` & `fuo_qqmusic-1.0.4/fuo_qqmusic/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.3/fuo_qqmusic/api.py` & `fuo_qqmusic-1.0.4/fuo_qqmusic/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,15 @@
             'req_0': {
                 'module': 'music.musichallSong.SongListInter',
                 'method': 'GetSingerSongList',
                 'param': {
                     'singerid': artist_id,
                     'begin': (page - 1) * page_size,
                     'num': page_size,
+                    'order': 1,  # 热门/新，不带这个字段就是按歌曲新旧排序
                     # 有 newsong 字段时，服务端会返回含有 file 字段的字典
                     'newsong': 1
                 }},
             'comm': {
                 'g_tk': self.get_token_from_cookies(),
                 'uin': self._uin,
                 'format': 'json',
```

### Comparing `fuo_qqmusic-1.0.3/fuo_qqmusic/assets/icon.svg` & `fuo_qqmusic-1.0.4/fuo_qqmusic/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.3/fuo_qqmusic/provider.py` & `fuo_qqmusic-1.0.4/fuo_qqmusic/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,37 +236,66 @@
         data = self.api.playlist_detail(int(identifier), limit=1000)
         return _deserialize(data, QQPlaylistSchema)
 
     def playlist_create_songs_rd(self, playlist):
         songs = self._model_cache_get_or_fetch(playlist, "songs")
         return create_reader(songs)
 
-    def rec_list_daily_playlists(self):
+    def __rec_hot_playlists(self):
         user = self.get_current_user()
         if user is None:
             return []
         # pids = self.api.get_recommend_playlists_ids()
         # rec_playlists = [QQPlaylistModel.get(pid) for pid in pids]
         playlists = self.api.recommend_playlists()
         for pl in playlists:
             pl["dissid"] = pl["content_id"]
             pl["dissname"] = pl["title"]
             pl["logo"] = pl["cover"]
         return [_deserialize(playlist, QQPlaylistSchema) for playlist in playlists]
 
+    def rec_list_daily_playlists(self):
+        # TODO: cache API result
+        feed = self.api.get_recommend_feed()
+        shelf = None
+        for shelf_ in feed['v_shelf']:
+            # I guess 10046 means 'song'.
+            if shelf_['extra_info'].get('moduleID', '').startswith('playlist'):
+                shelf = shelf_
+                break
+        if shelf is None:
+            return []
+        playlists = []
+        for batch in shelf['v_niche']:
+            for card in batch['v_card']:
+                print(card['title'], card['jumptype'])
+                if card['jumptype'] == 10014:  # 10014->playlist
+                    playlists.append(
+                        PlaylistModel(identifier=str(card['id']),
+                                      source=SOURCE,
+                                      name=card['title'],
+                                      cover=card['cover'],
+                                      description=card['miscellany']['rcmdtemplate'])
+                    )
+        return playlists
+
     def rec_a_collection_of_songs(self):
         # TODO: cache API result
         feed = self.api.get_recommend_feed()
         shelf = None
-        for shelf in feed['v_shelf']:
+        for shelf_ in feed['v_shelf']:
             # I guess 10046 means 'song'.
-            if shelf['miscellany'].get('jumptype') == 10046:
-                shelf = shelf
+            if int(shelf_['miscellany'].get('jumptype', 0)) == 10046:
+                shelf = shelf_
+                break
         if shelf is None:
-            return '', []
+            return Collection(name='',
+                              type_=CollectionType.only_songs,
+                              models=[],
+                              description='')
         title = shelf['title_content'] or shelf['title_template']
         song_ids = []
         for batch in shelf['v_niche']:
             for card in batch['v_card']:
                 if card['jumptype'] == 10046:
                     song_id = int(card['id'])
                     if song_id not in song_ids:
```

### Comparing `fuo_qqmusic-1.0.3/fuo_qqmusic/provider_ui.py` & `fuo_qqmusic-1.0.4/fuo_qqmusic/provider_ui.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.3/fuo_qqmusic/schemas.py` & `fuo_qqmusic-1.0.4/fuo_qqmusic/schemas.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/PKG-INFO` & `fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo-qqmusic
-Version: 1.0.3
+Version: 1.0.4
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 Keywords: feeluown,plugin,qqmusic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `fuo_qqmusic-1.0.3/setup.py` & `fuo_qqmusic-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 
 
 setup(
     name='fuo_qqmusic',
-    version='1.0.3',
+    version='1.0.4',
     description='feeluown qqmusic plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=[
         'fuo_qqmusic',
     ],
     package_data={
```

