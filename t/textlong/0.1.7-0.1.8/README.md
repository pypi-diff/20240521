# Comparing `tmp/textlong-0.1.7.tar.gz` & `tmp/textlong-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlong-0.1.7.tar", max compression
+gzip compressed data, was "textlong-0.1.8.tar", max compression
```

## Comparing `textlong-0.1.7.tar` & `textlong-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.7/LICENSE
--rw-r--r--   0        0        0     1604 2024-05-18 06:08:22.626599 textlong-0.1.7/README.md
--rw-r--r--   0        0        0      950 2024-05-20 01:52:35.288407 textlong-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.7/textlong/.pypirc
--rw-r--r--   0        0        0      605 2024-05-20 01:52:14.392217 textlong-0.1.7/textlong/__init__.py
--rw-r--r--   0        0        0       22 2024-05-20 01:52:27.691763 textlong-0.1.7/textlong/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.7/textlong/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.7/textlong/agents/base.py
--rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.7/textlong/agents/prompt.py
--rw-r--r--   0        0        0     2370 2024-05-19 07:03:51.711272 textlong-0.1.7/textlong/ai.py
--rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.7/textlong/base.py
--rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.7/textlong/command.py
--rw-r--r--   0        0        0      304 2024-05-19 00:35:41.802269 textlong-0.1.7/textlong/config.py
--rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.7/textlong/docs/__init__.py
--rw-r--r--   0        0        0     3591 2024-05-19 12:16:37.280829 textlong-0.1.7/textlong/docs/writing_help.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.7/textlong/document_loaders/__init__.py
--rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.7/textlong/document_loaders/base.py
--rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.7/textlong/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.7/textlong/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.7/textlong/memory/__init__.py
--rw-r--r--   0        0        0     8113 2024-05-20 01:45:32.350495 textlong-0.1.7/textlong/memory/base.py
--rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.7/textlong/memory/history.py
--rw-r--r--   0        0        0     2708 2024-05-20 01:50:58.318560 textlong-0.1.7/textlong/memory/memory_manager.py
--rw-r--r--   0        0        0    10875 2024-05-19 08:17:29.283447 textlong-0.1.7/textlong/node.py
--rw-r--r--   0        0        0     6673 2024-05-19 15:21:55.942882 textlong-0.1.7/textlong/projects.py
--rw-r--r--   0        0        0      121 2024-05-18 02:19:48.770966 textlong-0.1.7/textlong/prompts/__init__.py
--rw-r--r--   0        0        0     4187 2024-05-19 14:26:02.963118 textlong-0.1.7/textlong/prompts/hub.py
--rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.7/textlong/prompts/main.py
--rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.7/textlong/prompts/translate.py
--rw-r--r--   0        0        0     6114 2024-05-19 14:26:40.868005 textlong-0.1.7/textlong/prompts/writing_prompt.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.7/textlong/retrievers/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.7/textlong/retrievers/base.py
--rw-r--r--   0        0        0     3213 2024-05-19 07:30:31.509304 textlong-0.1.7/textlong/serialize.py
--rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.1.7/textlong/state.py
--rw-r--r--   0        0        0     1983 2024-05-19 15:29:28.868426 textlong-0.1.7/textlong/tree.py
--rw-r--r--   0        0        0     3563 2024-05-19 15:30:49.311152 textlong-0.1.7/textlong/writing.py
--rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 textlong-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1604 2024-05-18 06:08:22.626599 textlong-0.1.8/README.md
+-rw-r--r--   0        0        0      950 2024-05-21 03:40:50.273162 textlong-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.8/textlong/.pypirc
+-rw-r--r--   0        0        0      638 2024-05-20 22:20:34.997733 textlong-0.1.8/textlong/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-21 03:40:14.226971 textlong-0.1.8/textlong/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.8/textlong/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.8/textlong/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.8/textlong/agents/prompt.py
+-rw-r--r--   0        0        0     2370 2024-05-19 07:03:51.711272 textlong-0.1.8/textlong/ai.py
+-rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.8/textlong/base.py
+-rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.8/textlong/command.py
+-rw-r--r--   0        0        0      399 2024-05-20 13:06:13.568404 textlong-0.1.8/textlong/config.py
+-rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.8/textlong/docs/__init__.py
+-rw-r--r--   0        0        0     3591 2024-05-19 12:16:37.280829 textlong-0.1.8/textlong/docs/writing_help.py
+-rw-r--r--   0        0        0      113 2024-05-20 14:16:45.955689 textlong-0.1.8/textlong/document_loaders/__init__.py
+-rw-r--r--   0        0        0     5160 2024-05-20 14:00:52.675879 textlong-0.1.8/textlong/document_loaders/base.py
+-rw-r--r--   0        0        0     3089 2024-05-20 14:36:58.320633 textlong-0.1.8/textlong/document_loaders/qa_excel.py
+-rw-r--r--   0        0        0      813 2024-05-20 14:13:34.220746 textlong-0.1.8/textlong/document_loaders/qa_markdown.py
+-rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.8/textlong/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.8/textlong/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.8/textlong/memory/__init__.py
+-rw-r--r--   0        0        0     7990 2024-05-21 00:14:39.945505 textlong-0.1.8/textlong/memory/base.py
+-rw-r--r--   0        0        0     3320 2024-05-20 02:18:02.245645 textlong-0.1.8/textlong/memory/file_store.py
+-rw-r--r--   0        0        0     2708 2024-05-20 01:50:58.318560 textlong-0.1.8/textlong/memory/memory_manager.py
+-rw-r--r--   0        0        0    10875 2024-05-19 08:17:29.283447 textlong-0.1.8/textlong/node.py
+-rw-r--r--   0        0        0     6673 2024-05-20 22:08:33.246467 textlong-0.1.8/textlong/projects.py
+-rw-r--r--   0        0        0      243 2024-05-20 22:39:35.717193 textlong-0.1.8/textlong/prompts/__init__.py
+-rw-r--r--   0        0        0     4581 2024-05-21 02:04:23.542824 textlong-0.1.8/textlong/prompts/hub.py
+-rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.8/textlong/prompts/main.py
+-rw-r--r--   0        0        0     1327 2024-05-20 23:32:21.329587 textlong-0.1.8/textlong/prompts/qa_prompt.py
+-rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.8/textlong/prompts/translate.py
+-rw-r--r--   0        0        0     6043 2024-05-20 16:58:59.906388 textlong-0.1.8/textlong/prompts/writing_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.8/textlong/retrievers/__init__.py
+-rw-r--r--   0        0        0     3109 2024-05-20 23:14:36.258930 textlong-0.1.8/textlong/retrievers/base.py
+-rw-r--r--   0        0        0     3213 2024-05-19 07:30:31.509304 textlong-0.1.8/textlong/serialize.py
+-rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.1.8/textlong/state.py
+-rw-r--r--   0        0        0     1983 2024-05-19 15:29:28.868426 textlong-0.1.8/textlong/tree.py
+-rw-r--r--   0        0        0     3563 2024-05-19 15:30:49.311152 textlong-0.1.8/textlong/writing.py
+-rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 textlong-0.1.8/PKG-INFO
```

### Comparing `textlong-0.1.7/LICENSE` & `textlong-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/README.md` & `textlong-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/pyproject.toml` & `textlong-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textlong"
-version = "0.1.7"
+version = "0.1.8"
 description = "A framework designed to produce long-texts with GPT or other large language models."
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/textlong"
 repository = "https://github.com/arcstep/textlong.git"
 license = "MIT"
 readme = "README.md"
```

### Comparing `textlong-0.1.7/textlong/__init__.py` & `textlong-0.1.8/textlong/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from textlong.document_loaders.base import (
+from textlong.document_loaders import (
     LocalFilesLoader,
-    LocalFilesQALoader,
+    QAExcelsLoader,
+    QAMarkdownLoader,
 )
 
 from textlong.retrievers.base import (
     AskDocumentTool,
+    format_qa_docs,
     create_qa_chain,
     create_qa_toolkits,
 )
 
 from textlong.agents.base import (
     PROMPT_REACT,
     PROMPT_COT,
```

### Comparing `textlong-0.1.7/textlong/agents/base.py` & `textlong-0.1.8/textlong/agents/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/agents/prompt.py` & `textlong-0.1.8/textlong/agents/prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/ai.py` & `textlong-0.1.8/textlong/ai.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/base.py` & `textlong-0.1.8/textlong/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/command.py` & `textlong-0.1.8/textlong/command.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/docs/writing_help.py` & `textlong-0.1.8/textlong/docs/writing_help.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/langgraph/tools_calling.py` & `textlong-0.1.8/textlong/langgraph/tools_calling.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/memory/base.py` & `textlong-0.1.8/textlong/memory/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,21 +188,19 @@
         memory = config["configurable"]["memory"]
         store = memory.chat_memory
 
         # 获得输入
         inputs = run.inputs
         input_val = inputs[self.input_messages_key]
         input_messages = self._get_input_messages(input_val)
-        print("input_messages:", input_messages)
 
         # 获得输出
         output_val = run.outputs
         output_messages = self._get_output_messages(output_val)
         store.add_messages(input_messages + output_messages)
-        print("store:", store)
 
     def _merge_configs(self, *configs: Optional[RunnableConfig]) -> RunnableConfig:
         config = super()._merge_configs(*configs)
         expected_keys = [field_spec.id for field_spec in self.history_factory_config]
 
         configurable = config.get("configurable", {})
 
@@ -219,10 +217,9 @@
                 f"Expected keys are {sorted(expected_keys)}."
                 f"When using via .invoke() or .stream(), pass in a config; "
                 f"e.g., chain.invoke({example_input}, {example_config})"
             )
 
         memory = self.memory_manager.get_memory_factory(configurable["session_id"])
         config["configurable"]["memory"] = memory
-        # print("_merge_configs:", memory)
         
         return config
```

### Comparing `textlong-0.1.7/textlong/memory/memory_manager.py` & `textlong-0.1.8/textlong/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/node.py` & `textlong-0.1.8/textlong/node.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/projects.py` & `textlong-0.1.8/textlong/projects.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/prompts/hub.py` & `textlong-0.1.8/textlong/prompts/hub.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,23 +3,18 @@
     MessagesPlaceholder,
     SystemMessagePromptTemplate,
     AIMessagePromptTemplate,
     HumanMessagePromptTemplate,
     load_prompt as load_str_prompt,
 )
 from ..config import get_textlong_folder, _PROMPTS_FOLDER_NAME
-from .writing_prompt import (
-    create_writing_help_prompt,
-    create_writing_init_prompt,
-    create_writing_todo_prompt,
-)
 import os
 import json
 
-def save_chat_prompt(template: ChatPromptTemplate, template_id: str, project_id: str, id="0", user_id="default_user"):
+def save_chat_prompt(template: ChatPromptTemplate, template_id: str, project_id: str="default", id="0", user_id="public"):
     """
     保存提示语模板。
     """
     prompt_path = os.path.join(get_textlong_folder(), user_id, project_id, _PROMPTS_FOLDER_NAME, id, template_id)
 
     for i, p in enumerate(template.messages):
         if isinstance(p, SystemMessagePromptTemplate):
@@ -42,51 +37,59 @@
     for k, v in template.partial_variables.items():
         if v != None:
             path = os.path.join(prompt_path, f"var_{k}.md")
             os.makedirs(os.path.dirname(path), exist_ok=True)
             with open(path, 'w', encoding='utf-8') as f:
                 f.write(f'{v}')
 
-def load_chat_prompt(template_id: str, project_id: str=None, id="0", user_id="default_user"):
+def load_chat_prompt(template_id: str, project_id: str="default", id: str="0", user_id: str="public", in_memory: bool=True):
     """
     加载提示语模板和partial变量的字符串。    
     目前不支持在partial中使用嵌套模板。
     """
-    if project_id == None:
-        if template_id == "help":
-            return create_writing_help_prompt()
+    prompt_path = os.path.join(get_textlong_folder(), user_id, project_id, _PROMPTS_FOLDER_NAME, id, template_id)
+    if in_memory or not os.path.exists(prompt_path):
+        if template_id == "qa":
+            from .qa_prompt import create_qa_prompt
+            template = create_qa_prompt()
+        elif template_id == "help":
+            from .writing_prompt import create_writing_help_prompt
+            template = create_writing_help_prompt()
         elif template_id == "init":
-            return create_writing_init_prompt()
+            from .writing_prompt import create_writing_init_prompt
+            template = create_writing_init_prompt()
         elif template_id == "outline":
-            return create_writing_todo_prompt(content_type="outline")
+            from .writing_prompt import create_writing_todo_prompt
+            template = create_writing_todo_prompt(content_type="outline")
         elif template_id == "paragraph":
-            return create_writing_todo_prompt(content_type="paragraph")
+            from .writing_prompt import create_writing_todo_prompt
+            template = create_writing_todo_prompt(content_type="paragraph")
         else:
-            raise ValueError(f"模板ID必须为 [init|outline|paragraph|help] 中的一个, [{template_id}]不能支持！")
-
-    prompt_path = os.path.join(get_textlong_folder(), user_id, project_id, _PROMPTS_FOLDER_NAME, id, template_id)
-    if not os.path.exists(prompt_path):
-        raise FileNotFoundError(f"提示语模板 {template_id} 不存在")
+            raise ValueError(f"模板ID[{template_id}]不能支持！")
+        
+        if not in_memory:
+            save_chat_prompt(template, template_id, project_id, id, user_id)
+        return template
 
     messages = []
     partial_variables = {}
 
     for filename in sorted(os.listdir(prompt_path)):
         path = os.path.join(prompt_path, filename)
 
         message = None
         if filename.endswith('_system.json'):
             prompt = load_str_prompt(path)
-            message = SystemMessagePromptTemplate.from_template(prompt.template)
+            message = SystemMessagePromptTemplate.from_template(prompt.template, template_format='mustache')
         elif filename.endswith('_ai.json'):
             prompt = load_str_prompt(path)
-            message = AIMessagePromptTemplate.from_template(prompt.template)
+            message = AIMessagePromptTemplate.from_template(prompt.template, template_format='mustache')
         elif filename.endswith('_human.json'):
             prompt = load_str_prompt(path)
-            message = HumanMessagePromptTemplate.from_template(prompt.template)
+            message = HumanMessagePromptTemplate.from_template(prompt.template, template_format='mustache')
         elif filename.endswith('_placeholder.json'):
             with open(path, 'r') as f:
                 data = json.load(f)
                 message = MessagesPlaceholder(**data)
         elif filename.startswith('var_') and filename.endswith('.md'):
             with open(path, 'r') as f:
                 text = f.read()
```

### Comparing `textlong-0.1.7/textlong/prompts/main.py` & `textlong-0.1.8/textlong/prompts/main.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/prompts/writing_prompt.py` & `textlong-0.1.8/textlong/prompts/writing_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,24 +86,25 @@
 _AUTO_OUTLINE_OR_PARAGRAPH_PROMPT = """
 你现在的任务是编写《{{title}}》，字数大约为{{words_advice}}字。
 扩写依据为：{{howto}}
 注意，你所写的内容是下面总提纲的一部份：
 {{outline_exist}}
 """
 
-def create_writing_help_prompt(system_prompt:str = None):
+def create_writing_help_prompt():
     """咨询系统如何使用"""
 
     prompt = ChatPromptTemplate.from_messages([
-        ("system", system_prompt or HELP_SYSTEM_PROMPT),
+        ("system", "{{task_instruction}}"),
         ("ai", "我有哪些资料可以参考？"),
         ("human", "你的资料如下：\n{{doc}}"),
         MessagesPlaceholder(variable_name="history"),
         ("human", "{{task}}"),
     ], template_format="mustache").partial(
+        task_instruction=HELP_SYSTEM_PROMPT,
         doc=WRITING_HELP
     )
     
     return prompt
 
 def create_writing_init_prompt():
     main_prompt = MAIN_PROMPT
@@ -113,19 +114,16 @@
     
     prompt = ChatPromptTemplate.from_messages([
         ("system", main_prompt),
         ("ai", "OK"),
         MessagesPlaceholder(variable_name="history"),
         ("human", "{{task}}"),
     ], template_format="mustache").partial(
-        # 任务指南
         task_instruction=task_prompt,
-        # 输出格式要求
         output_format=output_prompt,
-        # JSON严格控制
         json_instruction=json_instruction,
     )
 
     return prompt
 
 def create_writing_todo_prompt(content_type: str="paragraph"):
     main_prompt = MAIN_PROMPT
```

### Comparing `textlong-0.1.7/textlong/retrievers/base.py` & `textlong-0.1.8/textlong/retrievers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,37 +17,40 @@
 请始终使用中文回答。
 
 {context}
 
 问题: {question}
 """
 
-def format_docs(docs: List[str]) -> str:
-    return "\n\n".join([d.page_content for d in docs])
+def format_qa_docs(docs: List[str]) -> str:
+    """
+    如果 Document 中包含的 metadata['answer'] 属性就优先采纳。
+    """
+    return "\n\n".join([d.metadata['answer'] or d.page_content for d in docs])
 
 def convert_message_to_str(message: Union[BaseMessage, str]) -> str:
     if isinstance(message, BaseMessage):
         return message.content
     else:
         return message
 
 def create_qa_chain(llm: Runnable, retriever: Callable, prompt: str = DEFAULT_QA_CHAIN_PROMPT) -> Callable:
     """
     使用 create_qa_chain 构建的LCEL链时，参数应当是一个消息。
     
-    例如：    
+    例如：
     chain = creat_qa_chain(llm, rectriever)
-    chain.invoke("langchain_chinese是啥？")
+    chain.invoke("textlong是啥？")
     """
 
     _prompt = ChatPromptTemplate.from_template(prompt)
 
     return (
         {
-            "context": (lambda x: convert_message_to_str(x)) | retriever | format_docs,
+            "context": (lambda x: convert_message_to_str(x)) | retriever | format_qa_docs,
             "question": lambda x: convert_message_to_str(x) ,
         }
         | _prompt
         | llm
     )
 
 def make_safe_tool(func: Callable) -> Callable:
```

### Comparing `textlong-0.1.7/textlong/serialize.py` & `textlong-0.1.8/textlong/serialize.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/state.py` & `textlong-0.1.8/textlong/state.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/tree.py` & `textlong-0.1.8/textlong/tree.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/textlong/writing.py` & `textlong-0.1.8/textlong/writing.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.7/PKG-INFO` & `textlong-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textlong
-Version: 0.1.7
+Version: 0.1.8
 Summary: A framework designed to produce long-texts with GPT or other large language models.
 Home-page: https://github.com/arcstep/textlong
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

