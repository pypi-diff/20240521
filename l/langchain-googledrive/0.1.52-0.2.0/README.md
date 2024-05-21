# Comparing `tmp/langchain_googledrive-0.1.52.tar.gz` & `tmp/langchain_googledrive-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_googledrive-0.1.52.tar", max compression
+gzip compressed data, was "langchain_googledrive-0.2.0.tar", max compression
```

## Comparing `langchain_googledrive-0.1.52.tar` & `langchain_googledrive-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.1.52/LICENSE.txt
--rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.1.52/README.md
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/__init__.py
--rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/document_loaders/__init__.py
--rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.52/langchain_googledrive/document_loaders/google_drive.py
--rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/retrievers/__init__.py
--rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.52/langchain_googledrive/retrievers/google_drive.py
--rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/tools/google_drive/__init__.py
--rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.52/langchain_googledrive/tools/google_drive/tool.py
--rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/utilities/__init__.py
--rw-r--r--   0        0        0    77982 2024-05-15 13:21:49.172506 langchain_googledrive-0.1.52/langchain_googledrive/utilities/google_drive.py
--rw-r--r--   0        0        0     3399 2024-03-19 17:23:21.113431 langchain_googledrive-0.1.52/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 langchain_googledrive-0.1.52/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/__init__.py
+-rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.0/langchain_googledrive/document_loaders/google_drive.py
+-rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/retrievers/__init__.py
+-rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.0/langchain_googledrive/retrievers/google_drive.py
+-rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/tools/google_drive/__init__.py
+-rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.0/langchain_googledrive/tools/google_drive/tool.py
+-rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/utilities/__init__.py
+-rw-r--r--   0        0        0    77814 2024-05-21 10:34:08.671404 langchain_googledrive-0.2.0/langchain_googledrive/utilities/google_drive.py
+-rw-r--r--   0        0        0     3376 2024-05-21 10:33:05.007999 langchain_googledrive-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 langchain_googledrive-0.2.0/PKG-INFO
```

### Comparing `langchain_googledrive-0.1.52/LICENSE.txt` & `langchain_googledrive-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.52/README.md` & `langchain_googledrive-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.52/langchain_googledrive/document_loaders/google_drive.py` & `langchain_googledrive-0.2.0/langchain_googledrive/document_loaders/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.52/langchain_googledrive/retrievers/google_drive.py` & `langchain_googledrive-0.2.0/langchain_googledrive/retrievers/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.52/langchain_googledrive/tools/google_drive/tool.py` & `langchain_googledrive-0.2.0/langchain_googledrive/tools/google_drive/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.52/langchain_googledrive/utilities/google_drive.py` & `langchain_googledrive-0.2.0/langchain_googledrive/utilities/google_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,20 @@
     ClassVar,
     Dict,
     Iterator,
     List,
     Literal,
     Optional,
     Protocol,
+    Sequence,
     Set,
     Type,
     Union,
     cast,
-    runtime_checkable, Sequence,
+    runtime_checkable,
 )
 from uuid import UUID, uuid4
 
 from langchain_core.documents import BaseDocumentTransformer, Document
 from langchain_core.load.serializable import Serializable
 from langchain_core.pydantic_v1 import (
     BaseModel,
@@ -54,22 +55,22 @@
     # Sub-classes should implement this method
     # as return list(self.lazy_load()).
     # This method returns a List which is materialized in memory.
     def load(self) -> List[Document]:
         ...
 
     def load_and_split(
-            self, text_splitter: Optional[BaseDocumentTransformer] = None
+        self, text_splitter: Optional[BaseDocumentTransformer] = None
     ) -> List[Document]:
         ...
 
     # Attention: This method will be upgraded into an abstractmethod once it's
     #            implemented in all the existing subclasses.
     def lazy_load(
-            self,
+        self,
     ) -> Iterator[Document]:
         ...
 
 
 FORMAT_INSTRUCTION = (
     "The input should be formatted as a list of entities separated"
     " with a space. As an example, a list of keywords is 'hello word'."
@@ -160,17 +161,17 @@
         self._cache[key] = value
         self._cache.move_to_end(key)
         if len(self._cache) > self._capacity:
             self._cache.popitem(last=False)
 
 
 def default_conv_loader(
-        mode: Literal["single", "elements"] = "single",
-        strategy: Literal["strategy", "fast"] = "fast",
-        ocr_languages: str = "eng",
+    mode: Literal["single", "elements"] = "single",
+    strategy: Literal["strategy", "fast"] = "fast",
+    ocr_languages: str = "eng",
 ) -> TYPE_CONV_MAPPING:
     mime_types_mapping: TYPE_CONV_MAPPING = {}
     try:
         from langchain_community.document_loaders import TextLoader
 
         mime_types_mapping.update(
             {
@@ -225,23 +226,23 @@
         )
     except ImportError:
         logger.info("Ignore RTF for GDrive (use `pip install pypandoc_binary`)")
     try:
         import unstructured  # noqa: F401 , type: ignore
         from langchain_community.document_loaders import (
             UnstructuredEPubLoader,
+            UnstructuredExcelLoader,
             UnstructuredFileLoader,
             UnstructuredHTMLLoader,
             UnstructuredImageLoader,
             UnstructuredMarkdownLoader,
             UnstructuredODTLoader,
             UnstructuredPDFLoader,
             UnstructuredPowerPointLoader,
             UnstructuredWordDocumentLoader,
-            UnstructuredExcelLoader,
         )
 
         try:
             import detectron2  # noqa: F401 , type: ignore
             import pdf2image  # type: ignore
             import pytesseract  # type: ignore
 
@@ -339,44 +340,44 @@
         "gdrive-by-name": MyPromptTemplate(
             input_variables=["query"],
             template="name contains '{query}' and trashed=false",
         ),
         "gdrive-by-name-in-folder": MyPromptTemplate(
             input_variables=["query", "folder_id"],
             template="name contains '{query}' "
-                     "and '{folder_id}' in parents "
-                     "and trashed=false",
+            "and '{folder_id}' in parents "
+            "and trashed=false",
         ),
         "gdrive-query-in-folder": MyPromptTemplate(
             input_variables=["query", "folder_id"],
             template="fullText contains '{query}' "
-                     "and '{folder_id}' in parents "
-                     "and trashed=false",
+            "and '{folder_id}' in parents "
+            "and trashed=false",
         ),
         "gdrive-mime-type": MyPromptTemplate(
             input_variables=["mime_type"],
             template="mimeType = '{mime_type}' and trashed=false",
         ),
         "gdrive-mime-type-in-folder": MyPromptTemplate(
             input_variables=["mime_type", "folder_id"],
             template="mimeType = '{mime_type}' "
-                     "and '{folder_id}' in parents "
-                     "and trashed=false",
+            "and '{folder_id}' in parents "
+            "and trashed=false",
         ),
         "gdrive-query-with-mime-type": MyPromptTemplate(
             input_variables=["query", "mime_type"],
             template="(fullText contains '{query}' "
-                     "and mimeType = '{mime_type}') "
-                     "and trashed=false",
+            "and mimeType = '{mime_type}') "
+            "and trashed=false",
         ),
         "gdrive-query-with-mime-type-and-folder": MyPromptTemplate(
             input_variables=["query", "mime_type", "folder_id"],
             template="((fullText contains '{query}') and mimeType = '{mime_type}') "
-                     "and '{folder_id}' in parents "
-                     "and trashed=false",
+            "and '{folder_id}' in parents "
+            "and trashed=false",
         ),
     }
 
 
 templates: Optional[Dict[str, PromptTemplate]] = None
 
 
@@ -705,15 +706,15 @@
     _no_data: UUID = Field(default_factory=uuid4)
 
     # Class var
     _default_page_size: ClassVar[int] = 50
 
     @root_validator
     def orderBy_is_compatible_with_recursive(
-            cls, values: Dict[str, Any]
+        cls, values: Dict[str, Any]
     ) -> Dict[str, Any]:
         if values["orderBy"] and values["recursive"]:
             raise ValueError("`orderBy` is incompatible with `recursive` parameter")
         return values
 
     _gdrive_list_params: ClassVar[Set[str]] = {
         "corpora",
@@ -879,16 +880,18 @@
         self._files = None
         self._docs = None
         self._spreadsheets = None
         self._slides = None
 
         if self.gsheet_mode != "elements":
             if self.gsheet_columns or self.gsheet_metadata_columns:
-                raise ValueError("gsheet_columns and gsheet_metadata_columns must be "
-                                 "used with gsheet_mode == 'elements'")
+                raise ValueError(
+                    "gsheet_columns and gsheet_metadata_columns must be "
+                    "used with gsheet_mode == 'elements'"
+                )
         self._creds = self._load_credentials(self.scopes)
 
         from googleapiclient.discovery import build  # type: ignore
 
         # self._params_dict: Dict[str, Union[str, int, float]] = {}
 
         self._files = build("drive", "v3", credentials=self._creds).files()
@@ -930,15 +933,20 @@
                 return name
         except HttpError:
             # Sometime, it's impossible to get the file name of a folder.
             # It's because a shortcut reference an inaccessible file.
             return "inaccessible-folder"
 
     def _get_file_by_id(self, file_id: str, **kwargs: Any) -> Dict:
-        get_kwargs = {**self._kwargs, **self._gdrive_kwargs, **kwargs, **{"fields": self.fields}}
+        get_kwargs = {
+            **self._kwargs,
+            **self._gdrive_kwargs,
+            **kwargs,
+            **{"fields": self.fields},
+        }
         get_kwargs = {
             key: get_kwargs[key]
             for key in get_kwargs
             if key in GoogleDriveUtilities._gdrive_get_params
         }
         return self.files.get(fileId=file_id, **get_kwargs).execute()
 
@@ -1207,15 +1215,15 @@
         if "owners" in file:
             meta["author"] = file["owners"][0]["displayName"]
         if file.get("description", "").strip():
             meta["summary"] = file["description"]
         return meta
 
     def lazy_get_relevant_documents(
-            self, query: Optional[str] = None, **kwargs: Any
+        self, query: Optional[str] = None, **kwargs: Any
     ) -> Iterator[Document]:
         """
         A generator to yield one document at a time.
         It's better for the memory.
 
         Args:
             query: Query string or None.
@@ -1244,17 +1252,17 @@
         # Purge template variables
         variables = {
             k: v
             for k, v in variables.items()
             if k in cast(PromptTemplate, self._template).input_variables
         }
         query_str = (
-                " "
-                + "".join(cast(PromptTemplate, self._template).format(**variables))
-                + " "
+            " "
+            + "".join(cast(PromptTemplate, self._template).format(**variables))
+            + " "
         )
         list_kwargs = {
             **self._gdrive_kwargs,
             **kwargs,
             **{
                 "pageSize": max(100, int(num_results * 1.5))
                 if num_results > 0
@@ -1280,26 +1288,26 @@
                     results = self.files.list(**list_kwargs).execute()
                     nextPageToken, files = (
                         results.get("nextPageToken"),
                         results["files"],
                     )
                     for file in files:
                         file_key = (
-                                file.get("webViewLink")
-                                or file.get("webContentLink")
-                                or file["id"]
+                            file.get("webViewLink")
+                            or file.get("webContentLink")
+                            or file["id"]
                         )
                         if file_key in file in documents_id:
                             logger.debug(f"Already yield the document {file['id']}")
                             continue
                         documents = self._get_document(file, current_mode)
                         for i, document in enumerate(documents):
                             document_key = (
-                                    document.metadata.get("source")
-                                    or document.metadata["gdriveId"]
+                                document.metadata.get("source")
+                                or document.metadata["gdriveId"]
                             )
                             if document_key in documents_id:
                                 # May by, with a link
                                 logger.debug(
                                     f"Already yield the document '{document_key}'"
                                 )
                                 continue
@@ -1335,29 +1343,29 @@
                             "Set 'folder_id' if you use 'recursive == True'"
                         )
 
                     nextPageToken = None
                     dir_template = OriginalPromptTemplate(
                         input_variables=["folder_id"],
                         template="(mimeType = 'application/vnd.google-apps.folder' "
-                                 "or mimeType = 'application/vnd.google-apps.shortcut') "
-                                 "and '{folder_id}' in parents and trashed=false",
+                        "or mimeType = 'application/vnd.google-apps.shortcut') "
+                        "and '{folder_id}' in parents and trashed=false",
                     )
                     subdir_query = "".join(dir_template.format(folder_id=folder_id))
                     while True:  # Manage pages
                         logger.debug(f"Search in subdir '{subdir_query}'")
                         list_kwargs = {
                             **self._gdrive_kwargs,
                             **kwargs,
                             **{
                                 "pageSize": max(100, int(num_results * 1.5))
                                 if num_results > 0
                                 else GoogleDriveUtilities._default_page_size,
                                 "fields": "nextPageToken, "
-                                          "files(id,name, mimeType, shortcutDetails)",
+                                "files(id,name, mimeType, shortcutDetails)",
                             },
                         }
                         # Purge list_kwargs
                         list_kwargs = {
                             key: list_kwargs[key]
                             for key in list_kwargs
                             if key in GoogleDriveUtilities._gdrive_list_params
@@ -1381,25 +1389,25 @@
                                         file["id"], file["name"]
                                     )
                                     logger.debug(
                                         f"Add the folder "
                                         f"'{file['name']}' ({file['id']})"
                                     )
                                 if (
-                                        mime_type == "application/vnd.google-apps.shortcut"
-                                        and self.follow_shortcut
+                                    mime_type == "application/vnd.google-apps.shortcut"
+                                    and self.follow_shortcut
                                 ):
                                     # Manage only shortcut to folder
                                     if "shortcutDetails" in file:
                                         target_mimetype = file["shortcutDetails"][
                                             "targetMimeType"
                                         ]
                                         if (
-                                                target_mimetype
-                                                == "application/vnd.google-apps.folder"
+                                            target_mimetype
+                                            == "application/vnd.google-apps.folder"
                                         ):
                                             recursive_folders.append(
                                                 file["shortcutDetails"]["targetId"]
                                             )
                                     else:
                                         logger.debug(
                                             f"Breaking shortcut '{file['name']}' "
@@ -1451,20 +1459,20 @@
             self._docs.close()
         if hasattr(self, "_spreadsheets") and self._spreadsheets:
             self._spreadsheets.close()
         if hasattr(self, "_slides") and self._slides:
             self._slides.close()
 
     def _extract_text(
-            self,
-            node: Any,
-            *,
-            key: str = "content",
-            path: str = "/textRun",
-            markdown: bool = True,
+        self,
+        node: Any,
+        *,
+        key: str = "content",
+        path: str = "/textRun",
+        markdown: bool = True,
     ) -> List[str]:
         def visitor(result: List[str], node: Any, parent: str) -> List[str]:
             if isinstance(node, dict):
                 if "paragraphMarker" in node:
                     result.append("- " if "bullet" in node["paragraphMarker"] else "")
                     return result
                 if "paragraph" in node:
@@ -1502,16 +1510,15 @@
                             # Split each portion and pad with space
                             for i, portion in enumerate(split_cell):
                                 if portion != "<br />":
                                     pure_portion = re.sub(
                                         r"\[(.*)\](?:\(.*\))", r"\1", portion
                                     )
                                     split_cell[i] = portion + (
-                                            " " * (
-                                            col_size[col_idx] - len(pure_portion))
+                                        " " * (col_size[col_idx] - len(pure_portion))
                                     )
                             # rebuild the body
                             row[col_idx] = "".join(split_cell)
                     # Now, build a markdown array
                     for row_idx, row in enumerate(rows):
                         row_result = ["| "]
                         for cell in row:
@@ -1524,17 +1531,16 @@
                             result.append("".join(row_result) + "\n")
                     return result
 
                 if key in node and isinstance(node.get(key), str):
                     if parent.endswith(path):
                         if node[key].strip():
                             if markdown and (
-                                    ("style" in node and "link" in node["style"])
-                                    or ("textStyle" in node and "link" in node[
-                                "textStyle"])
+                                ("style" in node and "link" in node["style"])
+                                or ("textStyle" in node and "link" in node["textStyle"])
                             ):
                                 style_node = (
                                     node["style"]
                                     if "style" in node
                                     else node["textStyle"]
                                 )
                                 link = style_node["link"]
@@ -1581,47 +1587,54 @@
         sheets = spreadsheet.get("sheets", [])
         single: List[str] = []
 
         for sheet in sheets:
             sheet_name = sheet["properties"]["title"]
             result = (
                 self._spreadsheets.values()
-                .get(spreadsheetId=file["id"], range=sheet_name, valueRenderOption="UNFORMATTED_VALUE")
+                .get(
+                    spreadsheetId=file["id"],
+                    range=sheet_name,
+                    valueRenderOption="UNFORMATTED_VALUE",
+                )
                 .execute()
             )
             values = result.get("values", [])
 
             if values:
                 width = max([len(v) for v in values])
                 headers = values[0]
                 if self.gsheet_mode == "elements":
                     for i, row in enumerate(values[1:], start=1):
                         content = []
                         if self.gsheet_columns and len(self.gsheet_columns) == 1:
-                            raw_content = f"{row[headers.index(self.gsheet_columns[0])]}\n"
+                            raw_content = (
+                                f"{row[headers.index(self.gsheet_columns[0])]}\n"
+                            )
                         else:
                             for j, v in enumerate(row):
-                                if (not self.gsheet_columns
-                                        or str(headers[j]).strip()
-                                        in self.gsheet_columns):
+                                if (
+                                    not self.gsheet_columns
+                                    or str(headers[j]).strip() in self.gsheet_columns
+                                ):
                                     title = (
                                         str(headers[j]).strip() + ": "
                                         if len(headers) > j
                                         else ""
                                     )
                                     content.append(f"{title}{str(v).strip()}\n")
 
                             raw_content = "".join(content)
                         metadata = self._extract_meta_data(file)
                         if "source" in metadata:
                             metadata["source"] = (
-                                    metadata["source"]
-                                    + "#gid="
-                                    + str(sheet["properties"]["sheetId"])
-                                    + f"&{i}"
+                                metadata["source"]
+                                + "#gid="
+                                + str(sheet["properties"]["sheetId"])
+                                + f"&{i}"
                             )
                         metadata["row"] = i
                         for col_name in self.gsheet_metadata_columns:
                             try:
                                 metadata[col_name] = row[headers.index(col_name)]
                             except ValueError:
                                 pass  # Ignore
@@ -1655,18 +1668,18 @@
                         page_content="\n<PAGE BREAK>\n".join(single),
                         metadata=self._extract_meta_data(file),
                     )
                 else:
                     raise ValueError(f"Invalid mode '{self.gslide_mode}'")
 
     def _only_obj(
-            self,
-            page_elements: List[Dict[str, Any]],
-            translateX: float = 0.0,
-            translateY: float = 0.0,
+        self,
+        page_elements: List[Dict[str, Any]],
+        translateX: float = 0.0,
+        translateY: float = 0.0,
     ) -> List[Dict[str, Any]]:
         only_objets: List[Any] = []
         for obj in page_elements:
             if "elementGroup" in obj:
                 group_translate_x = obj["transform"].get("translateX", translateX)
                 group_translate_y = obj["transform"].get("translateY", translateY)
                 only_objets.extend(
@@ -1680,18 +1693,18 @@
             elif "image" in obj:
                 pass
             else:
                 only_objets.append(obj)
         return only_objets
 
     def _sort_page_elements(
-            self,
-            page_elements: List[Dict[str, Any]],
-            translateX: float = 0.0,
-            translateY: float = 0.0,
+        self,
+        page_elements: List[Dict[str, Any]],
+        translateX: float = 0.0,
+        translateY: float = 0.0,
     ) -> List[Dict[str, Any]]:
         only_obj = self._only_obj(page_elements, 0, 0)
         return sorted(
             only_obj,
             key=lambda x: (
                 x["transform"].get("translateY", 0),
                 x["transform"].get("translateX", 0),
@@ -1733,15 +1746,15 @@
                         metadata=meta,
                     )
         elif self.gslide_mode == "elements":
             for slide in gslide["slides"]:
                 metadata = self._extract_meta_data(file)
                 if "source" in metadata:
                     metadata["source"] = (
-                            metadata["source"] + "#slide=file_id." + slide["objectId"]
+                        metadata["source"] + "#slide=file_id." + slide["objectId"]
                     )
                 if "pageElements" in slide:
                     page_elements = self._sort_page_elements(slide["pageElements"])
                     for i, line in enumerate(self._extract_text(page_elements)):
                         if line.strip():
                             m = metadata.copy()
                             if "source" in m:
@@ -1859,21 +1872,21 @@
         return v
 
     def run(self, query: str) -> str:
         """Run query through Google Drive and parse result."""
         snippets = []
         logger.debug(f"{query=}")
         for document in self.lazy_get_relevant_documents(
-                query=query, num_results=self.num_results
+            query=query, num_results=self.num_results
         ):
             content = document.page_content
             if (
-                    self.mode in ["snippets", "snippets-markdown"]
-                    and "summary" in document.metadata
-                    and document.metadata["summary"]
+                self.mode in ["snippets", "snippets-markdown"]
+                and "summary" in document.metadata
+                and document.metadata["summary"]
             ):
                 content = document.metadata["summary"]
             if self.mode == "snippets":
                 snippets.append(
                     f"Name: {document.metadata['name']}\n"
                     f"Source: {document.metadata['source']}\n" + f"Summary: {content}"
                 )
@@ -1882,15 +1895,15 @@
                     f"[{document.metadata['name']}]"
                     f"({document.metadata['source']})<br/>\n" + f"{content}"
                 )
             elif self.mode == "documents":
                 snippets.append(
                     f"Name: {document.metadata['name']}\n"
                     f"Source: {document.metadata['source']}\n" + f"Summary: "
-                                                                 f"{GoogleDriveUtilities._snippet_from_page_content(content)}"
+                    f"{GoogleDriveUtilities._snippet_from_page_content(content)}"
                 )
             elif self.mode == "documents-markdown":
                 snippets.append(
                     f"[{document.metadata['name']}]"
                     f"({document.metadata['source']})<br/>"
                     + f"{GoogleDriveUtilities._snippet_from_page_content(content)}"
                 )
@@ -1913,15 +1926,15 @@
             Like bing_search, a list of dictionaries with the following keys:
                 `snippet: The `description` of the result.
                 `title`: The title of the result.
                 `link`: The link to the result.
         """
         metadata_results = []
         for document in self.lazy_get_relevant_documents(
-                query=query, num_results=num_results
+            query=query, num_results=num_results
         ):
             metadata_result = {
                 "title": document.metadata["name"],
                 "link": document.metadata["source"],
             }
             if "summary" in document.metadata:
                 metadata_result["snippet"] = document.metadata["summary"]
```

### Comparing `langchain_googledrive-0.1.52/pyproject.toml` & `langchain_googledrive-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://www.github.com/pprados/langchain-googledrive"
 packages = [{ include = "langchain_googledrive" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-langchain_core = ">=0.1.14"
-langchain_community = ">=0.0.14"
+langchain_core = ">=0.2.0"
+langchain_community = ">=0.2.0"
 google-api-python-client = "^2.97"
 google-auth-httplib2 = ">=0.1"
 google-auth-oauthlib = ">=1.0"
 #pydantic = "^1.10.0"
 pdf2image = { version = "^1.16", optional = true }
 pypandoc_binary = { version = "^1.11", optional = true }
 torch = { version = ">=1,<3", optional = true }
@@ -61,15 +61,14 @@
 lark = "^1.1.5"
 pandas = "^2.0.0"
 pytest-mock = "^3.10.0"
 pytest-socket = "^0.6.0"
 syrupy = "^4.0.2"
 unstructured = "^0.10.8"
 twine = "^4.0.0"
-langchain = "^0.1.2"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 mypy = "^0.991"
 ruff = "^0.0.249"
```

### Comparing `langchain_googledrive-0.1.52/PKG-INFO` & `langchain_googledrive-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-googledrive
-Version: 0.1.52
+Version: 0.2.0
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/hwchase17/langchain/pull/5135) to be validated.
 Home-page: https://www.github.com/pprados/langchain-googledrive
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Requires-Dist: google-api-python-client (>=2.97,<3.0)
 Requires-Dist: google-auth-httplib2 (>=0.1)
 Requires-Dist: google-auth-oauthlib (>=1.0)
-Requires-Dist: langchain_community (>=0.0.14)
-Requires-Dist: langchain_core (>=0.1.14)
+Requires-Dist: langchain_community (>=0.2.0)
+Requires-Dist: langchain_core (>=0.2.0)
 Requires-Dist: pdf2image (>=1.16,<2.0) ; extra == "all"
 Requires-Dist: pypandoc_binary (>=1.11,<2.0) ; extra == "all"
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0) ; extra == "all"
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: torch (>=1,<3) ; extra == "all"
 Requires-Dist: unstructured[local-inference] (>=0.10.12,<0.11.0) ; extra == "all"
 Project-URL: Repository, https://www.github.com/pprados/langchain-googledrive
```

